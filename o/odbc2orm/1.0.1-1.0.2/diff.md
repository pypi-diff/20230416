# Comparing `tmp/odbc2orm-1.0.1.tar.gz` & `tmp/odbc2orm-1.0.2-cp38-cp38-win32.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odbc2orm-1.0.1.tar", last modified: Sun Apr 16 13:51:59 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

