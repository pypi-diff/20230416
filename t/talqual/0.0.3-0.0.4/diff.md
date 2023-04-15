# Comparing `tmp/talqual-0.0.3.tar.gz` & `tmp/talqual-0.0.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talqual-0.0.3.tar", last modified: Sat Apr 15 22:09:43 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

