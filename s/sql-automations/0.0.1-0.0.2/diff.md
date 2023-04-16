# Comparing `tmp/sql_automations-0.0.1.tar.gz` & `tmp/sql_automations-0.0.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sql_automations-0.0.1.tar", last modified: Sun Apr 16 00:34:27 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

