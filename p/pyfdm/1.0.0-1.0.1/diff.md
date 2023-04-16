# Comparing `tmp/pyfdm-1.0.0.tar.gz` & `tmp/pyfdm-1.0.1.win-amd64.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfdm-1.0.0.tar", last modified: Mon Sep 26 11:02:04 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

