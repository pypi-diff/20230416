# Comparing `tmp/pyfollower-0.0.1.tar.gz` & `tmp/pyfollower-0.1.1-cp38-cp38-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyfollower-0.0.1.tar", last modified: Sun Apr 16 12:06:49 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

