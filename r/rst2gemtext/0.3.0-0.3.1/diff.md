# Comparing `tmp/rst2gemtext-0.3.0.tar.gz` & `tmp/rst2gemtext-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rst2gemtext-0.3.0.tar", last modified: Mon Mar  6 12:47:44 2023, max compression
+gzip compressed data, was "rst2gemtext-0.3.1.tar", last modified: Sun Apr 16 11:07:30 2023, max compression
```

## Comparing `rst2gemtext-0.3.0.tar` & `rst2gemtext-0.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 12:47:44.461843 rst2gemtext-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-03-06 12:47:38.000000 rst2gemtext-0.3.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-03-06 12:47:44.461843 rst2gemtext-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-03-06 12:47:38.000000 rst2gemtext-0.3.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-06 12:47:38.000000 rst2gemtext-0.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 12:47:44.461843 rst2gemtext-0.3.0/rst2gemtext.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-03-06 12:47:44.000000 rst2gemtext-0.3.0/rst2gemtext.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-03-06 12:47:44.000000 rst2gemtext-0.3.0/rst2gemtext.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 12:47:44.000000 rst2gemtext-0.3.0/rst2gemtext.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-06 12:47:44.000000 rst2gemtext-0.3.0/rst2gemtext.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-06 12:47:44.000000 rst2gemtext-0.3.0/rst2gemtext.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-06 12:47:44.000000 rst2gemtext-0.3.0/rst2gemtext.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    26597 2023-03-06 12:47:38.000000 rst2gemtext-0.3.0/rst2gemtext.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-06 12:47:44.461843 rst2gemtext-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-03-06 12:47:38.000000 rst2gemtext-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:07:30.361971 rst2gemtext-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-04-16 11:07:27.000000 rst2gemtext-0.3.1/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     6409 2023-04-16 11:07:30.361971 rst2gemtext-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-04-16 11:07:27.000000 rst2gemtext-0.3.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-16 11:07:27.000000 rst2gemtext-0.3.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:07:30.361971 rst2gemtext-0.3.1/rst2gemtext.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6409 2023-04-16 11:07:30.000000 rst2gemtext-0.3.1/rst2gemtext.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-16 11:07:30.000000 rst2gemtext-0.3.1/rst2gemtext.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 11:07:30.000000 rst2gemtext-0.3.1/rst2gemtext.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-16 11:07:30.000000 rst2gemtext-0.3.1/rst2gemtext.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-16 11:07:30.000000 rst2gemtext-0.3.1/rst2gemtext.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-16 11:07:30.000000 rst2gemtext-0.3.1/rst2gemtext.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27437 2023-04-16 11:07:27.000000 rst2gemtext-0.3.1/rst2gemtext.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 11:07:30.361971 rst2gemtext-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-16 11:07:27.000000 rst2gemtext-0.3.1/setup.py
```

### Comparing `rst2gemtext-0.3.0/COPYING` & `rst2gemtext-0.3.1/COPYING`

 * *Files identical despite different names*

### Comparing `rst2gemtext-0.3.0/PKG-INFO` & `rst2gemtext-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rst2gemtext
-Version: 0.3.0
+Version: 0.3.1
 Summary: Converts reStructuredText to Gemtext (Gemini markup format)
 Home-page: https://github.com/flozz/rst2gemtext
 Author: Fabien LOISON
 License: GPLv3
 Project-URL: Source Code, https://github.com/flozz/rst2gemtext
 Project-URL: Issues, https://github.com/flozz/rst2gemtext/issues
 Project-URL: Chat, https://discord.gg/P77sWhuSs4
@@ -167,15 +167,19 @@
 
 
 Changelog
 ---------
 
 * **[NEXT]** (changes on ``master``, but not released yet):
 
-  * Nothing yet :)
+  * Nothing yet ;)
+
+* **v0.3.1:**
+
+  * Fixed truncated tables when last row contains bullet lists (@flozz, #1)
 
 * **v0.3.0:**
 
   * Handle admonitons (``admonition``, ``attention``, ``caution``, ``danger``,
     ``error``, ``hint``, ``important``, ``note``, ``tip`` and ``warning``
     nodes) (@flozz)
```

### Comparing `rst2gemtext-0.3.0/README.rst` & `rst2gemtext-0.3.1/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -152,15 +152,19 @@
 
 
 Changelog
 ---------
 
 * **[NEXT]** (changes on ``master``, but not released yet):
 
-  * Nothing yet :)
+  * Nothing yet ;)
+
+* **v0.3.1:**
+
+  * Fixed truncated tables when last row contains bullet lists (@flozz, #1)
 
 * **v0.3.0:**
 
   * Handle admonitons (``admonition``, ``attention``, ``caution``, ``danger``,
     ``error``, ``hint``, ``important``, ``note``, ``tip`` and ``warning``
     nodes) (@flozz)
```

### Comparing `rst2gemtext-0.3.0/rst2gemtext.egg-info/PKG-INFO` & `rst2gemtext-0.3.1/rst2gemtext.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rst2gemtext
-Version: 0.3.0
+Version: 0.3.1
 Summary: Converts reStructuredText to Gemtext (Gemini markup format)
 Home-page: https://github.com/flozz/rst2gemtext
 Author: Fabien LOISON
 License: GPLv3
 Project-URL: Source Code, https://github.com/flozz/rst2gemtext
 Project-URL: Issues, https://github.com/flozz/rst2gemtext/issues
 Project-URL: Chat, https://discord.gg/P77sWhuSs4
@@ -167,15 +167,19 @@
 
 
 Changelog
 ---------
 
 * **[NEXT]** (changes on ``master``, but not released yet):
 
-  * Nothing yet :)
+  * Nothing yet ;)
+
+* **v0.3.1:**
+
+  * Fixed truncated tables when last row contains bullet lists (@flozz, #1)
 
 * **v0.3.0:**
 
   * Handle admonitons (``admonition``, ``attention``, ``caution``, ``danger``,
     ``error``, ``hint``, ``important``, ``note``, ``tip`` and ``warning``
     nodes) (@flozz)
```

### Comparing `rst2gemtext-0.3.0/rst2gemtext.py` & `rst2gemtext-0.3.1/rst2gemtext.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,47 @@
     :param str text: The text to cleanup.
     :rtype: str
     :return: The cleaned text.
     """
     return text.replace("\r\n", " ").replace("\n", " ").replace("\r", " ")
 
 
+def flatten_node_tree(nodes):
+    """Iterates recursively on given nodes and returns a flat list of the
+    nodes.
+
+    :param list<Node> nodes: A list of ``Node``.
+
+    :rtype: list<Node>
+    """
+    result_nodes = []
+    for node in nodes:
+        if isinstance(node, NodeGroup):
+            result_nodes += flatten_node_tree(node.nodes)
+        else:
+            result_nodes.append(node)
+    return result_nodes
+
+
+def search_lines_recursive(rst_node):
+    """Search recusrively for line numbers in rst nodes.
+
+    :param rst_node: any rst node from docutils.
+
+    :rtype: list<int>
+    """
+    lines = []
+    if rst_node.line:
+        lines.append(rst_node.line)
+    if rst_node.children:
+        for child_rst_node in rst_node.children:
+            lines += search_lines_recursive(child_rst_node)
+    return lines
+
+
 def parse_rst(rst_text, source_path="document"):
     """Parses a reStructuredText document.
 
     :param str rst_text: The reStructuredText to parse.
     :param str source_path: The path of the source reStructuredText file
                             (optional, but required if the document contains an
                             ``include`` directive)
@@ -710,22 +743,22 @@
         nodes = self._split_nodes(rst_node)
         preformatted_text_node = nodes.pop(0)
 
         title = ""
         line_min = math.inf
         line_max = 0
 
-        for node in nodes:
+        for node in flatten_node_tree(nodes):
             if isinstance(node, TitleNode):
                 title = node.rawtext
                 continue
-            if not node.rst_node.line:
-                continue
-            line_min = min(line_min, node.rst_node.line)
-            line_max = max(line_max, node.rst_node.line)
+            lines = search_lines_recursive(node.rst_node)
+            if lines:
+                line_min = min(line_min, *lines)
+                line_max = max(line_max, *lines)
         line_min -= 1
         line_max += 1
 
         table_lines = self.document._original_rst.split("\n")[line_min - 1 : line_max]
         indent = len(re.match(r"^(\s*).*$", table_lines[0]).group(1))
 
         preformatted_text_node.append_text(
```

### Comparing `rst2gemtext-0.3.0/setup.py` & `rst2gemtext-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 long_description = ""
 if os.path.isfile("README.rst"):
     long_description = open("README.rst", "r", encoding="UTF-8").read()
 
 
 setup(
     name="rst2gemtext",
-    version="0.3.0",
+    version="0.3.1",
     description="Converts reStructuredText to Gemtext (Gemini markup format)",
     url="https://github.com/flozz/rst2gemtext",
     project_urls={
         "Source Code": "https://github.com/flozz/rst2gemtext",
         "Issues": "https://github.com/flozz/rst2gemtext/issues",
         "Chat": "https://discord.gg/P77sWhuSs4",
         "Donate": "https://github.com/flozz/rst2gemtext#support-this-project",
```

