# Comparing `tmp/wxr2md-0.1.0.tar.gz` & `tmp/wxr2md-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wxr2md-0.1.0.tar", max compression
+gzip compressed data, was "wxr2md-0.2.0.tar", max compression
```

## Comparing `wxr2md-0.1.0.tar` & `wxr2md-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1069 2023-04-08 12:12:59.425373 wxr2md-0.1.0/LICENSE
--rw-r--r--   0        0        0     1148 2023-04-09 14:19:39.772819 wxr2md-0.1.0/README.md
--rw-r--r--   0        0        0      528 2023-04-09 14:06:33.981289 wxr2md-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1035 2023-04-09 14:52:43.045863 wxr2md-0.1.0/wxr2md/__main__.py
--rw-r--r--   0        0        0     4527 2023-04-09 13:44:01.861969 wxr2md-0.1.0/wxr2md/lib.py
--rw-r--r--   0        0        0     1756 1970-01-01 00:00:00.000000 wxr2md-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-08 12:12:59.425373 wxr2md-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1756 2023-04-16 11:53:03.465753 wxr2md-0.2.0/README.md
+-rw-r--r--   0        0        0      528 2023-04-16 11:55:01.336082 wxr2md-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1992 2023-04-16 11:46:35.837046 wxr2md-0.2.0/wxr2md/__main__.py
+-rw-r--r--   0        0        0     4767 2023-04-16 11:46:35.837399 wxr2md-0.2.0/wxr2md/lib.py
+-rw-r--r--   0        0        0     2364 1970-01-01 00:00:00.000000 wxr2md-0.2.0/PKG-INFO
```

### Comparing `wxr2md-0.1.0/LICENSE` & `wxr2md-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wxr2md-0.1.0/pyproject.toml` & `wxr2md-0.2.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wxr2md"
-version = "0.1.0"
+version = "0.2.0"
 description = "Converter for WordPress eXport RSS (WXR) files into Markdown files"
 authors = ["Dion Susanto <nikolasdion@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 keywords = ["wxr", "wordpress", "markdown"]
 repository = "https://github.com/nikolasdion/wxr2md"
```

### Comparing `wxr2md-0.1.0/wxr2md/lib.py` & `wxr2md-0.2.0/wxr2md/lib.py`

 * *Files 21% similar despite different names*

```diff
@@ -22,98 +22,104 @@
     """Unique ID of the post"""
     title: str
     """Title of the post as displayed in the page, can be None"""
     name: str
     """Name in the URL of the post"""
     content: str
     """Content, in markdown format"""
-    pub_date: str
-    """From pubDate element, RFC 822 format"""
-    post_date: datetime
-    """From wordpress metadata"""
-    post_modified: datetime
-    """From wordpress metadata"""
+    date: datetime
+    """Date posted, from wordpress metadata"""
+    modified: datetime
+    """Date last modified, from wordpress metadata"""
     categories: list[str]
     """List of categories/tags this post is associated with"""
     is_draft: bool
 
+    DATE_IN_BODY_FORMAT = "%a %d %b %Y, %I:%M"
+
     @classmethod
     def from_element(cls, element: ElementTree.Element):
         """Create a post from an XML element"""
         title = element.find("title").text
         name = element.find("wp:post_name", NAMESPACES).text
         id = element.find("wp:post_id", NAMESPACES).text
         content = element.find("content:encoded", NAMESPACES).text
         if content is not None:
             content = markdownify(content)
 
-        pub_date = element.find("pubDate", NAMESPACES).text
-
         try:
-            post_date = datetime.fromisoformat(
-                element.find("wp:post_date", NAMESPACES).text
-            )
+            date = datetime.fromisoformat(element.find("wp:post_date", NAMESPACES).text)
         except ValueError:
-            post_date = None
+            date = None
 
         try:
-            post_modified = datetime.fromisoformat(
+            modified = datetime.fromisoformat(
                 element.find("wp:post_modified", NAMESPACES).text
             )
         except ValueError:
-            post_modified = None
+            modified = None
 
         categories = [e.text for e in element.findall("category")]
         is_draft = element.find("wp:status", NAMESPACES).text == "draft"
 
         return cls(
             title=title,
             name=name,
             id=id,
             content=content,
-            pub_date=pub_date,
-            post_date=post_date,
-            post_modified=post_modified,
+            date=date,
+            modified=modified,
             categories=categories,
             is_draft=is_draft,
         )
 
-    def md_metadata(self) -> str:
+    def md_frontmatter(self) -> str:
         """Generate YAML metadata lines to be included in the markdown string"""
         lines = []
         lines.append("---")
         lines.append(f"id: {self.id}")
+        lines.append("layout: post")
         lines.append(f"title: {self.title}")
-        lines.append(f"post_date: {self.post_date}")
-        lines.append(f"post_modified: {self.post_modified}")
-        lines.append(f"categories: {self.categories}")
+        lines.append(f"date: {self.date}")
+        lines.append(f"modified: {self.modified}")
+        if len(self.categories) > 0:
+            lines.append(f"categories: {self.categories}")
+        if self.is_draft:
+            lines.append("draft: true")
         lines.append("---")
         lines.append("")
         return "\n".join(lines)
 
-    def md_body(self) -> str:
+    def md_body(self, include_title=False, include_date=False) -> str:
         """Generate markdown text body lines"""
         lines = []
-        if self.title is not None:
+        if self.title is not None and include_title:
             lines.append(f"# {self.title}")
             lines.append("")
-        if self.pub_date is not None:
-            lines.append(f"_{self.pub_date}_")
+        if self.date is not None and include_date:
+            lines.append(f"_{self.date.strftime(self.DATE_IN_BODY_FORMAT)}_")
             lines.append("")
         if self.content is not None:
             lines.append(f"{self.content}")
             lines.append("")
         return "\n".join(lines)
 
-    def to_md(self) -> str:
+    def to_md(
+        self,
+        frontmatter=True,
+        title_in_body=True,
+        date_in_body=True,
+    ) -> str:
         """Convert post into a markdown string"""
-        metadata = self.md_metadata()
-        body = self.md_body()
-
-        return metadata + "\n" + body
+        md = ""
+        if frontmatter:
+            md += self.md_frontmatter()
+            md += "\n"
+        md += self.md_body(title_in_body, date_in_body)
+        return md
 
 
 @dataclass
 class Blog:
     """Represents a WordPress blog"""
 
     title: str
```

