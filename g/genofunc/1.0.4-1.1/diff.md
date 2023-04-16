# Comparing `tmp/genofunc-1.0.4.tar.gz` & `tmp/genofunc-1.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/genofunc-1.0.4.tar", last modified: Mon Apr 10 06:16:43 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

