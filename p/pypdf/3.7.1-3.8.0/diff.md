# Comparing `tmp/pypdf-3.7.1.tar.gz` & `tmp/pypdf-3.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypdf-3.7.1.tar", last modified: Sun Apr  9 20:24:56 2023, max compression
+gzip compressed data, was "pypdf-3.8.0.tar", last modified: Sun Apr 16 19:18:29 2023, max compression
```

## Comparing `pypdf-3.7.1.tar` & `pypdf-3.8.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0      488 2022-12-10 23:30:58.176669 pypdf-3.7.1/.git-blame-ignore-revs
--rw-r--r--   0        0        0      542 2023-03-29 15:43:03.262713 pypdf-3.7.1/.readthedocs.yaml
--rw-r--r--   0        0        0    34734 2023-04-09 20:24:43.743420 pypdf-3.7.1/CHANGELOG.md
--rw-r--r--   0        0        0     3377 2023-03-19 10:45:11.184383 pypdf-3.7.1/CONTRIBUTORS.md
--rw-r--r--   0        0        0     1605 2022-12-10 23:30:58.184669 pypdf-3.7.1/LICENSE
--rw-r--r--   0        0        0       34 2022-12-10 23:30:58.184669 pypdf-3.7.1/MANIFEST.in
--rw-r--r--   0        0        0     4729 2023-04-09 16:59:02.663368 pypdf-3.7.1/README.md
--rw-r--r--   0        0        0     1234 2023-03-04 08:55:07.145847 pypdf-3.7.1/pypdf/__init__.py
--rw-r--r--   0        0        0    14870 2023-03-18 15:07:48.665105 pypdf-3.7.1/pypdf/_cmap.py
--rw-r--r--   0        0        0     1674 2023-02-28 08:12:53.909178 pypdf-3.7.1/pypdf/_codecs/__init__.py
--rw-r--r--   0        0        0   431492 2022-12-31 10:47:18.999493 pypdf-3.7.1/pypdf/_codecs/adobe_glyphs.py
--rw-r--r--   0        0        0     4269 2022-12-31 10:47:18.999493 pypdf-3.7.1/pypdf/_codecs/pdfdoc.py
--rw-r--r--   0        0        0     2630 2023-02-28 08:12:53.909178 pypdf-3.7.1/pypdf/_codecs/std.py
--rw-r--r--   0        0        0     3734 2022-12-31 10:47:18.999493 pypdf-3.7.1/pypdf/_codecs/symbol.py
--rw-r--r--   0        0        0     3742 2022-12-31 10:47:18.999493 pypdf-3.7.1/pypdf/_codecs/zapfding.py
--rw-r--r--   0        0        0    45635 2023-03-31 16:21:44.806544 pypdf-3.7.1/pypdf/_encryption.py
--rw-r--r--   0        0        0    30650 2023-03-04 11:49:14.882511 pypdf-3.7.1/pypdf/_merger.py
--rw-r--r--   0        0        0    82250 2023-03-31 15:39:30.774654 pypdf-3.7.1/pypdf/_page.py
--rw-r--r--   0        0        0     7186 2023-03-04 08:55:07.145847 pypdf-3.7.1/pypdf/_page_labels.py
--rw-r--r--   0        0        0     1920 2023-04-08 20:27:58.305582 pypdf-3.7.1/pypdf/_protocols.py
--rw-r--r--   0        0        0    86026 2023-04-09 16:59:02.667368 pypdf-3.7.1/pypdf/_reader.py
--rw-r--r--   0        0        0    12788 2023-03-31 16:21:44.806544 pypdf-3.7.1/pypdf/_security.py
--rw-r--r--   0        0        0    10008 2023-03-12 09:43:33.014879 pypdf-3.7.1/pypdf/_text_extraction/__init__.py
--rw-r--r--   0        0        0    14915 2023-04-08 20:27:58.305582 pypdf-3.7.1/pypdf/_utils.py
--rw-r--r--   0        0        0       22 2023-04-09 20:22:59.891064 pypdf-3.7.1/pypdf/_version.py
--rw-r--r--   0        0        0   122863 2023-04-08 20:27:58.309582 pypdf-3.7.1/pypdf/_writer.py
--rw-r--r--   0        0        0    16147 2023-04-09 16:59:02.667368 pypdf-3.7.1/pypdf/constants.py
--rw-r--r--   0        0        0     1631 2023-03-04 08:55:07.149847 pypdf-3.7.1/pypdf/errors.py
--rw-r--r--   0        0        0    25921 2023-04-09 16:59:02.667368 pypdf-3.7.1/pypdf/filters.py
--rw-r--r--   0        0        0     4549 2023-04-09 16:59:02.667368 pypdf-3.7.1/pypdf/generic/__init__.py
--rw-r--r--   0        0        0    17368 2023-04-08 20:27:58.309582 pypdf-3.7.1/pypdf/generic/_annotations.py
--rw-r--r--   0        0        0    24854 2023-04-08 20:27:58.309582 pypdf-3.7.1/pypdf/generic/_base.py
--rw-r--r--   0        0        0    54781 2023-04-08 20:27:58.309582 pypdf-3.7.1/pypdf/generic/_data_structures.py
--rw-r--r--   0        0        0     5427 2023-03-04 08:55:07.149847 pypdf-3.7.1/pypdf/generic/_fit.py
--rw-r--r--   0        0        0     1195 2023-02-28 08:19:03.524706 pypdf-3.7.1/pypdf/generic/_outline.py
--rw-r--r--   0        0        0     8826 2023-03-04 08:55:07.149847 pypdf-3.7.1/pypdf/generic/_rectangle.py
--rw-r--r--   0        0        0     6405 2023-03-04 11:49:14.882511 pypdf-3.7.1/pypdf/generic/_utils.py
--rw-r--r--   0        0        0     6880 2023-03-04 08:55:07.153847 pypdf-3.7.1/pypdf/pagerange.py
--rw-r--r--   0        0        0     1369 2023-02-28 08:12:53.917178 pypdf-3.7.1/pypdf/papersizes.py
--rw-r--r--   0        0        0        0 2022-12-31 10:47:19.003493 pypdf-3.7.1/pypdf/py.typed
--rw-r--r--   0        0        0     2135 2023-03-29 15:43:03.266713 pypdf-3.7.1/pypdf/types.py
--rw-r--r--   0        0        0    17879 2023-03-29 15:43:03.266713 pypdf-3.7.1/pypdf/xmp.py
--rw-r--r--   0        0        0     7326 2023-04-09 16:59:02.667368 pypdf-3.7.1/pyproject.toml
--rw-r--r--   0        0        0     1585 2023-02-05 10:26:02.030123 pypdf-3.7.1/setup.cfg
--rw-r--r--   0        0        0     6763 1970-01-01 00:00:00.000000 pypdf-3.7.1/PKG-INFO
+-rw-r--r--   0        0        0      488 2022-12-10 23:30:58.176669 pypdf-3.8.0/.git-blame-ignore-revs
+-rw-r--r--   0        0        0      542 2023-03-29 15:43:03.262713 pypdf-3.8.0/.readthedocs.yaml
+-rw-r--r--   0        0        0    35126 2023-04-16 19:18:25.439058 pypdf-3.8.0/CHANGELOG.md
+-rw-r--r--   0        0        0     3475 2023-04-16 09:09:24.301502 pypdf-3.8.0/CONTRIBUTORS.md
+-rw-r--r--   0        0        0     1605 2022-12-10 23:30:58.184669 pypdf-3.8.0/LICENSE
+-rw-r--r--   0        0        0       34 2022-12-10 23:30:58.184669 pypdf-3.8.0/MANIFEST.in
+-rw-r--r--   0        0        0     4729 2023-04-09 16:59:02.663368 pypdf-3.8.0/README.md
+-rw-r--r--   0        0        0     1234 2023-03-04 08:55:07.145847 pypdf-3.8.0/pypdf/__init__.py
+-rw-r--r--   0        0        0    14962 2023-04-16 09:09:24.301502 pypdf-3.8.0/pypdf/_cmap.py
+-rw-r--r--   0        0        0     1674 2023-02-28 08:12:53.909178 pypdf-3.8.0/pypdf/_codecs/__init__.py
+-rw-r--r--   0        0        0   431492 2022-12-31 10:47:18.999493 pypdf-3.8.0/pypdf/_codecs/adobe_glyphs.py
+-rw-r--r--   0        0        0     4269 2022-12-31 10:47:18.999493 pypdf-3.8.0/pypdf/_codecs/pdfdoc.py
+-rw-r--r--   0        0        0     2630 2023-02-28 08:12:53.909178 pypdf-3.8.0/pypdf/_codecs/std.py
+-rw-r--r--   0        0        0     3734 2022-12-31 10:47:18.999493 pypdf-3.8.0/pypdf/_codecs/symbol.py
+-rw-r--r--   0        0        0     3742 2022-12-31 10:47:18.999493 pypdf-3.8.0/pypdf/_codecs/zapfding.py
+-rw-r--r--   0        0        0    45635 2023-03-31 16:21:44.806544 pypdf-3.8.0/pypdf/_encryption.py
+-rw-r--r--   0        0        0    30706 2023-04-16 16:12:02.507479 pypdf-3.8.0/pypdf/_merger.py
+-rw-r--r--   0        0        0    82921 2023-04-16 09:09:24.305502 pypdf-3.8.0/pypdf/_page.py
+-rw-r--r--   0        0        0     7186 2023-03-04 08:55:07.145847 pypdf-3.8.0/pypdf/_page_labels.py
+-rw-r--r--   0        0        0     1920 2023-04-08 20:27:58.305582 pypdf-3.8.0/pypdf/_protocols.py
+-rw-r--r--   0        0        0    86085 2023-04-16 09:09:24.305502 pypdf-3.8.0/pypdf/_reader.py
+-rw-r--r--   0        0        0    12788 2023-03-31 16:21:44.806544 pypdf-3.8.0/pypdf/_security.py
+-rw-r--r--   0        0        0    10008 2023-03-12 09:43:33.014879 pypdf-3.8.0/pypdf/_text_extraction/__init__.py
+-rw-r--r--   0        0        0    14912 2023-04-16 12:58:54.105217 pypdf-3.8.0/pypdf/_utils.py
+-rw-r--r--   0        0        0       22 2023-04-16 19:17:18.914887 pypdf-3.8.0/pypdf/_version.py
+-rw-r--r--   0        0        0   122863 2023-04-16 09:09:24.305502 pypdf-3.8.0/pypdf/_writer.py
+-rw-r--r--   0        0        0    16147 2023-04-09 16:59:02.667368 pypdf-3.8.0/pypdf/constants.py
+-rw-r--r--   0        0        0     1631 2023-03-04 08:55:07.149847 pypdf-3.8.0/pypdf/errors.py
+-rw-r--r--   0        0        0    25921 2023-04-09 16:59:02.667368 pypdf-3.8.0/pypdf/filters.py
+-rw-r--r--   0        0        0     4549 2023-04-09 16:59:02.667368 pypdf-3.8.0/pypdf/generic/__init__.py
+-rw-r--r--   0        0        0    17368 2023-04-08 20:27:58.309582 pypdf-3.8.0/pypdf/generic/_annotations.py
+-rw-r--r--   0        0        0    24854 2023-04-08 20:27:58.309582 pypdf-3.8.0/pypdf/generic/_base.py
+-rw-r--r--   0        0        0    54890 2023-04-10 07:47:24.160491 pypdf-3.8.0/pypdf/generic/_data_structures.py
+-rw-r--r--   0        0        0     5427 2023-03-04 08:55:07.149847 pypdf-3.8.0/pypdf/generic/_fit.py
+-rw-r--r--   0        0        0     1195 2023-02-28 08:19:03.524706 pypdf-3.8.0/pypdf/generic/_outline.py
+-rw-r--r--   0        0        0     8826 2023-03-04 08:55:07.149847 pypdf-3.8.0/pypdf/generic/_rectangle.py
+-rw-r--r--   0        0        0     6405 2023-03-04 11:49:14.882511 pypdf-3.8.0/pypdf/generic/_utils.py
+-rw-r--r--   0        0        0     6880 2023-03-04 08:55:07.153847 pypdf-3.8.0/pypdf/pagerange.py
+-rw-r--r--   0        0        0     1369 2023-02-28 08:12:53.917178 pypdf-3.8.0/pypdf/papersizes.py
+-rw-r--r--   0        0        0        0 2022-12-31 10:47:19.003493 pypdf-3.8.0/pypdf/py.typed
+-rw-r--r--   0        0        0     2135 2023-03-29 15:43:03.266713 pypdf-3.8.0/pypdf/types.py
+-rw-r--r--   0        0        0    17879 2023-03-29 15:43:03.266713 pypdf-3.8.0/pypdf/xmp.py
+-rw-r--r--   0        0        0     7425 2023-04-10 18:00:48.219069 pypdf-3.8.0/pyproject.toml
+-rw-r--r--   0        0        0     1585 2023-02-05 10:26:02.030123 pypdf-3.8.0/setup.cfg
+-rw-r--r--   0        0        0     6763 1970-01-01 00:00:00.000000 pypdf-3.8.0/PKG-INFO
```

### Comparing `pypdf-3.7.1/.readthedocs.yaml` & `pypdf-3.8.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.1/CHANGELOG.md` & `pypdf-3.8.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,24 @@
 # CHANGELOG
 
+## Version 3.7.2, 2023-04-16
+
+### New Features (ENH)
+-  Add transform method to Transformation class (#1765)
+-  Cope with UC2 fonts in text_extraction (#1785)
+
+### Robustness (ROB)
+-  Invalid startxref pointing 1 char before (#1784)
+
+### Maintenance (MAINT)
+-  Mark code handling old parameters as deprecated (#1798)
+
+[Full Changelog](https://github.com/py-pdf/pypdf/compare/3.7.1...3.7.2)
+
+
 ## Version 3.7.1, 2023-04-09
 
 ### Security (SEC)
 -  Warn about PDF encryption security (#1755)
 
 ### Robustness (ROB)
 -  Prevent loop in Cloning (#1770)
```

### Comparing `pypdf-3.7.1/CONTRIBUTORS.md` & `pypdf-3.8.0/CONTRIBUTORS.md`

 * *Files 2% similar despite different names*

```diff
@@ -21,26 +21,28 @@
 * [Karvonen, Harry](https://github.com/Hatell/)
 * [Kotler, Mitchell](https://github.com/mitchelljkotler)
 * [KourFrost](https://github.com/KourFrost)
 * [Lightup1](https://github.com/Lightup1)
 * [Majumder, Jonah](https://github.com/jonahmajumder)
 * [Manini, Lorenzo](https://github.com/lorenzomanini)
 * [maxbeer99](https://github.com/maxbeer99)
+* [nalin-udhaar](https://github.com/nalin-udhaar)
 * [McNeil, Karen](https://github.com/karenlmcneil): Arabic Language Support
 * [Mérino, Antoine](https://github.com/Merinorus)
 * [Paternault, Louis](https://framagit.org/spalax)
 * [Perrensen, Olsen](https://github.com/olsonperrensen)
 * [Pinheiro, Arthur](https://github.com/xilopaint)
 * [programmarchy](https://github.com/programmarchy)
 * [pubpub-zz](https://github.com/pubpub-zz): involved in community development
 * [Rogmann, Sascha](https://github.com/srogmann)
 * [robbiebusinessacc](https://github.com/robbiebusinessacc)
 * [sietzeberends](https://github.com/sietzeberends)
 * [Stüber, Timo](https://github.com/omit66)
 * [Thoma, Martin](https://github.com/MartinThoma): Maintainer of pypdf since April 2022. I hope to build a great community with many awesome contributors. [LinkedIn](https://www.linkedin.com/in/martin-thoma/) | [StackOverflow](https://stackoverflow.com/users/562769/martin-thoma) | [Blog](https://martin-thoma.com/)
+* [Thomas, Reuben](https://github.com/rrthomas)
 * [WevertonGomes](https://github.com/WevertonGomesCosta)
 * [Wilson, Huon](https://github.com/huonw)
 * ztravis
 
 ## Adding a new contributor
 
 Contributors are:
```

### Comparing `pypdf-3.7.1/LICENSE` & `pypdf-3.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.1/README.md` & `pypdf-3.8.0/README.md`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.1/pypdf/__init__.py` & `pypdf-3.8.0/pypdf/__init__.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.1/pypdf/_cmap.py` & `pypdf-3.8.0/pypdf/_cmap.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,14 +89,15 @@
 _predefined_cmap: Dict[str, str] = {
     "/Identity-H": "utf-16-be",
     "/Identity-V": "utf-16-be",
     "/GB-EUC-H": "gbk",  # TBC
     "/GB-EUC-V": "gbk",  # TBC
     "/GBpc-EUC-H": "gb2312",  # TBC
     "/GBpc-EUC-V": "gb2312",  # TBC
+    # UCS2 in code
 }
 
 
 # manually extracted from http://mirrors.ctan.org/fonts/adobe/afm/Adobe-Core35_AFMs-229.tar.gz
 _default_fonts_space_width: Dict[str, int] = {
     "/Courrier": 600,
     "/Courier-Bold": 600,
@@ -142,14 +143,16 @@
         try:
             # already done : enc = NameObject.unnumber(enc.encode()).decode()
             # for #xx decoding
             if enc in charset_encoding:
                 encoding = charset_encoding[enc].copy()
             elif enc in _predefined_cmap:
                 encoding = _predefined_cmap[enc]
+            elif "-UCS2-" in enc:
+                encoding = "utf-16-be"
             else:
                 raise Exception("not found")
         except Exception:
             warnings.warn(
                 f"Advanced encoding {enc} not implemented yet",
                 PdfReadWarning,
             )
```

### Comparing `pypdf-3.7.1/pypdf/_codecs/__init__.py` & `pypdf-3.8.0/pypdf/_codecs/__init__.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.1/pypdf/_codecs/adobe_glyphs.py` & `pypdf-3.8.0/pypdf/_codecs/adobe_glyphs.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.1/pypdf/_codecs/pdfdoc.py` & `pypdf-3.8.0/pypdf/_codecs/pdfdoc.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.1/pypdf/_codecs/std.py` & `pypdf-3.8.0/pypdf/_codecs/std.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.1/pypdf/_codecs/symbol.py` & `pypdf-3.8.0/pypdf/_codecs/symbol.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.1/pypdf/_codecs/zapfding.py` & `pypdf-3.8.0/pypdf/_codecs/zapfding.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.1/pypdf/_encryption.py` & `pypdf-3.8.0/pypdf/_encryption.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.1/pypdf/_merger.py` & `pypdf-3.8.0/pypdf/_merger.py`

 * *Files 1% similar despite different names*

```diff
@@ -700,26 +700,26 @@
             fit: The fit of the destination page.
         """
         if page_number is not None and pagenum is not None:
             raise ValueError(
                 "The argument pagenum of add_outline_item is deprecated. "
                 "Use page_number only."
             )
-        if pagenum is not None:
+        if pagenum is not None:  # deprecated
             old_term = "pagenum"
             new_term = "page_number"
             warnings.warn(
                 (
                     f"{old_term} is deprecated as an argument and will be "
                     f"removed in pypdf==4.0.0. Use {new_term} instead"
                 ),
                 DeprecationWarning,
             )
             page_number = pagenum
-        if page_number is None:
+        if page_number is None:  # deprecated
             raise ValueError("page_number may not be None")
         writer = self.output
         if writer is None:
             raise RuntimeError(ERR_CLOSED_WRITER)
         return writer.add_outline_item(
             title,
             page_number,
@@ -807,26 +807,26 @@
             page_number: Page number this destination points at.
         """
         if page_number is not None and pagenum is not None:
             raise ValueError(
                 "The argument pagenum of add_named_destination is deprecated. "
                 "Use page_number only."
             )
-        if pagenum is not None:
+        if pagenum is not None:  # deprecated
             old_term = "pagenum"
             new_term = "page_number"
             warnings.warn(
                 (
                     f"{old_term} is deprecated as an argument and will be "
                     f"removed in pypdf==4.0.0. Use {new_term} instead"
                 ),
                 DeprecationWarning,
             )
             page_number = pagenum
-        if page_number is None:
+        if page_number is None:  # deprecated
             raise ValueError("page_number may not be None")
         dest = Destination(
             TextStringObject(title),
             NumberObject(page_number),
             Fit.fit_horizontally(top=826),
         )
         self.named_dests.append(dest)
```

### Comparing `pypdf-3.7.1/pypdf/_page.py` & `pypdf-3.8.0/pypdf/_page.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,14 +205,33 @@
             matrix[0][1],
             matrix[1][0],
             matrix[1][1],
             matrix[2][0],
             matrix[2][1],
         )
 
+    def transform(self, m: "Transformation") -> "Transformation":
+        """
+        Apply one transformation to another.
+
+        Args:
+            m: a Transformation to apply.
+
+        Returns:
+            A new ``Transformation`` instance
+
+        Example:
+            >>> from pypdf import Transformation
+            >>> op = Transformation((1, 0, 0, -1, 0, height)) # vertical mirror
+            >>> op = Transformation().transform(Transformation((-1, 0, 0, 1, iwidth, 0))) # horizontal mirror
+            >>> page.add_transformation(op)
+        """
+        ctm = Transformation.compress(matrix_multiply(self.matrix, m.matrix))
+        return Transformation(ctm)
+
     def translate(self, tx: float = 0, ty: float = 0) -> "Transformation":
         """
         Translate the contents of a page.
 
         Args:
             tx: The translation along the x-axis.
             ty: The translation along the y-axis.
```

### Comparing `pypdf-3.7.1/pypdf/_page_labels.py` & `pypdf-3.8.0/pypdf/_page_labels.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.1/pypdf/_protocols.py` & `pypdf-3.8.0/pypdf/_protocols.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.1/pypdf/_reader.py` & `pypdf-3.8.0/pypdf/_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1875,14 +1875,16 @@
             startxref:
 
         Returns:
             0 means no issue, other values represent specific issues.
         """
         stream.seek(startxref - 1, 0)  # -1 to check character before
         line = stream.read(1)
+        if line == b"j":
+            line = stream.read(1)
         if line not in b"\r\n \t":
             return 1
         line = stream.read(4)
         if line != b"xref":
             # not an xref so check if it is an XREF object
             line = b""
             while line in b"0123456789 \t":
```

### Comparing `pypdf-3.7.1/pypdf/_security.py` & `pypdf-3.8.0/pypdf/_security.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.1/pypdf/_text_extraction/__init__.py` & `pypdf-3.8.0/pypdf/_text_extraction/__init__.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.1/pypdf/_utils.py` & `pypdf-3.8.0/pypdf/_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 ]
 
 StreamType = IO
 StrByteType = Union[str, StreamType]
 
 DEPR_MSG_NO_REPLACEMENT = "{} is deprecated and will be removed in pypdf {}."
 DEPR_MSG_NO_REPLACEMENT_HAPPENED = "{} is deprecated and was removed in pypdf {}."
-DEPR_MSG = "{} is deprecated and will be removed in pypdf 3.0.0. Use {} instead."
+DEPR_MSG = "{} is deprecated and will be removed in pypdf {}. Use {} instead."
 DEPR_MSG_HAPPENED = "{} is deprecated and was removed in pypdf {}. Use {} instead."
 
 
 def _get_max_pdf_version_header(header1: bytes, header2: bytes) -> bytes:
     versions = (
         b"%PDF-1.3",
         b"%PDF-1.4",
@@ -383,15 +383,15 @@
     raise DeprecationError(msg)
 
 
 def deprecate_with_replacement(
     old_name: str, new_name: str, removed_in: str = "3.0.0"
 ) -> None:
     """Raise an exception that a feature will be removed, but has a replacement."""
-    deprecate(DEPR_MSG.format(old_name, new_name, removed_in), 4)
+    deprecate(DEPR_MSG.format(old_name, removed_in, new_name), 4)
 
 
 def deprecation_with_replacement(
     old_name: str, new_name: str, removed_in: str = "3.0.0"
 ) -> None:
     """Raise an exception that a feature was already removed, but has a replacement."""
     deprecation(DEPR_MSG_HAPPENED.format(old_name, removed_in, new_name))
```

### Comparing `pypdf-3.7.1/pypdf/_writer.py` & `pypdf-3.8.0/pypdf/_writer.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.1/pypdf/constants.py` & `pypdf-3.8.0/pypdf/constants.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.1/pypdf/errors.py` & `pypdf-3.8.0/pypdf/errors.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.1/pypdf/filters.py` & `pypdf-3.8.0/pypdf/filters.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.1/pypdf/generic/__init__.py` & `pypdf-3.8.0/pypdf/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.1/pypdf/generic/_annotations.py` & `pypdf-3.8.0/pypdf/generic/_annotations.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.1/pypdf/generic/_base.py` & `pypdf-3.8.0/pypdf/generic/_base.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.1/pypdf/generic/_data_structures.py` & `pypdf-3.8.0/pypdf/generic/_data_structures.py`

 * *Files 0% similar despite different names*

```diff
@@ -293,14 +293,15 @@
     @property
     def xmp_metadata(self) -> Optional[PdfObject]:
         """
         Retrieve XMP (Extensible Metadata Platform) data relevant to the this
         object, if available.
 
         Stability: Added in v1.12, will exist for all future v1.x releases.
+        See Table 315 – Additional entries in a metadata stream dictionary
 
         Returns:
           Returns a {@link #xmp.XmpInformation XmlInformation} instance
           that can be used to access XMP metadata from the document.  Can also
           return None if no metadata was found on the document root.
         """
         from ..xmp import XmpInformation
@@ -986,14 +987,15 @@
         self.pdf = pdf_dest
         self.operations = list(cast("ContentStream", src).operations)
         self.forced_encoding = cast("ContentStream", src).forced_encoding
         # no need to call DictionaryObjection or anything
         # like super(DictionaryObject,self)._clone(src, pdf_dest, force_duplicate, ignore_fields)
 
     def __parse_content_stream(self, stream: StreamType) -> None:
+        # 7.8.2 Content Streams
         stream.seek(0, 0)
         operands: List[Union[int, str, PdfObject]] = []
         while True:
             peek = read_non_whitespace(stream)
             if peek == b"" or peek == 0:
                 break
             stream.seek(-1, 1)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pypdf-3.7.1/pypdf/generic/_fit.py` & `pypdf-3.8.0/pypdf/generic/_fit.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.1/pypdf/generic/_outline.py` & `pypdf-3.8.0/pypdf/generic/_outline.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.1/pypdf/generic/_rectangle.py` & `pypdf-3.8.0/pypdf/generic/_rectangle.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.1/pypdf/generic/_utils.py` & `pypdf-3.8.0/pypdf/generic/_utils.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.1/pypdf/pagerange.py` & `pypdf-3.8.0/pypdf/pagerange.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.1/pypdf/papersizes.py` & `pypdf-3.8.0/pypdf/papersizes.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.1/pypdf/types.py` & `pypdf-3.8.0/pypdf/types.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.1/pypdf/xmp.py` & `pypdf-3.8.0/pypdf/xmp.py`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.1/pyproject.toml` & `pypdf-3.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,17 @@
 # Regexes for lines to exclude from consideration
 exclude_lines = [
     # Have to re-enable the standard pragma
     "pragma: no cover",
     "@overload",
     "deprecated",
 
+    # Don't complain about type-checking code not being hit by unit tests
+    "if TYPE_CHECKING",
+
     # Don't complain about missing debug-only code:
     "def __repr__",
     "def __str__",
     "if self\\.debug",
 
     # Don't complain if tests don't hit defensive assertion code:
     "raise AssertionError",
```

### Comparing `pypdf-3.7.1/setup.cfg` & `pypdf-3.8.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pypdf-3.7.1/PKG-INFO` & `pypdf-3.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypdf
-Version: 3.7.1
+Version: 3.8.0
 Summary: A pure-python PDF library capable of splitting, merging, cropping, and transforming PDF files
 Author-email: Mathieu Fenniak <biziqe@mathieu.fenniak.net>
 Maintainer-email: Martin Thoma <info@martin-thoma.de>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

