# Comparing `tmp/nobuco-0.1.0.tar.gz` & `tmp/nobuco-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nobuco-0.1.0.tar", last modified: Sat Apr 15 10:52:46 2023, max compression
+gzip compressed data, was "nobuco-0.1.1.tar", last modified: Sun Apr 16 17:34:39 2023, max compression
```

## Comparing `nobuco-0.1.0.tar` & `nobuco-0.1.1.tar`

### file list

```diff
@@ -1,70 +1,71 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-15 10:52:46.601614 nobuco-0.1.0/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2023-03-02 20:53:15.000000 nobuco-0.1.0/LICENSE
--rw-rw-r--   0 alex      (1000) alex      (1000)       14 2023-04-15 10:44:29.000000 nobuco-0.1.0/MANIFEST.in
--rw-rw-r--   0 alex      (1000) alex      (1000)    17512 2023-04-15 10:52:46.601614 nobuco-0.1.0/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)    15678 2023-04-15 10:25:52.000000 nobuco-0.1.0/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-15 10:52:46.597614 nobuco-0.1.0/docs/
--rw-rw-r--   0 alex      (1000) alex      (1000)    64876 2023-03-25 20:16:55.000000 nobuco-0.1.0/docs/channel_ordering.png
--rw-rw-r--   0 alex      (1000) alex      (1000)    63145 2023-03-25 20:46:53.000000 nobuco-0.1.0/docs/channel_ordering_forced.png
--rw-rw-r--   0 alex      (1000) alex      (1000)    70703 2023-03-24 09:18:07.000000 nobuco-0.1.0/docs/control_if.png
--rw-rw-r--   0 alex      (1000) alex      (1000)     2110 2023-04-05 14:55:45.000000 nobuco-0.1.0/docs/converter_inside_converter1.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    26497 2023-04-05 19:25:33.000000 nobuco-0.1.0/docs/converter_inside_converter1.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     2319 2023-04-05 14:56:10.000000 nobuco-0.1.0/docs/converter_inside_converter2.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    30325 2023-04-05 19:25:54.000000 nobuco-0.1.0/docs/converter_inside_converter2.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     3070 2023-04-06 09:06:34.000000 nobuco-0.1.0/docs/essentials1.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    35615 2023-04-06 09:06:58.000000 nobuco-0.1.0/docs/essentials1.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     2811 2023-04-05 14:47:00.000000 nobuco-0.1.0/docs/essentials2.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    32971 2023-04-05 19:22:33.000000 nobuco-0.1.0/docs/essentials2.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     2281 2023-04-05 14:48:33.000000 nobuco-0.1.0/docs/essentials3.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    28090 2023-04-05 19:22:46.000000 nobuco-0.1.0/docs/essentials3.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     1559 2023-04-05 14:51:28.000000 nobuco-0.1.0/docs/inplace1.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    18606 2023-04-05 19:23:57.000000 nobuco-0.1.0/docs/inplace1.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     1050 2023-04-05 14:52:17.000000 nobuco-0.1.0/docs/inplace2.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    11981 2023-04-05 19:24:22.000000 nobuco-0.1.0/docs/inplace2.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     1195 2023-04-05 14:52:18.000000 nobuco-0.1.0/docs/inplace3.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    14409 2023-04-05 19:25:18.000000 nobuco-0.1.0/docs/inplace3.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     6859 2023-03-24 11:40:17.000000 nobuco-0.1.0/docs/inplace_empty.png
--rw-rw-r--   0 alex      (1000) alex      (1000)    82036 2023-03-03 12:08:40.000000 nobuco-0.1.0/docs/tutorial.png
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-15 10:52:46.597614 nobuco-0.1.0/nobuco/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2021-06-04 16:18:38.000000 nobuco-0.1.0/nobuco/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      798 2023-03-07 13:07:06.000000 nobuco-0.1.0/nobuco/commons.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-15 10:52:46.597614 nobuco-0.1.0/nobuco/convert/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-10-12 10:30:24.000000 nobuco-0.1.0/nobuco/convert/__init__.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)    12608 2023-03-13 12:38:17.000000 nobuco-0.1.0/nobuco/convert/converter.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-15 10:52:46.601614 nobuco-0.1.0/nobuco/convert/layers/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-12-06 13:02:40.000000 nobuco-0.1.0/nobuco/convert/layers/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4992 2023-03-08 10:21:14.000000 nobuco-0.1.0/nobuco/convert/layers/channel_order.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4894 2023-03-07 15:12:41.000000 nobuco-0.1.0/nobuco/convert/layers/container.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      313 2022-12-06 13:05:18.000000 nobuco-0.1.0/nobuco/convert/layers/stub.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      918 2023-03-08 10:08:07.000000 nobuco-0.1.0/nobuco/convert/layers/weight.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3497 2023-03-07 10:32:51.000000 nobuco-0.1.0/nobuco/convert/validation.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-15 10:52:46.601614 nobuco-0.1.0/nobuco/converters/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-11-11 15:28:31.000000 nobuco-0.1.0/nobuco/converters/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2049 2023-03-06 15:27:24.000000 nobuco-0.1.0/nobuco/converters/channel_ordering.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)    72007 2023-04-15 10:16:15.000000 nobuco-0.1.0/nobuco/converters/impl.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     2459 2023-03-13 12:32:55.000000 nobuco-0.1.0/nobuco/converters/node_converter.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      384 2022-12-21 13:41:52.000000 nobuco-0.1.0/nobuco/converters/ops.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2002 2023-03-03 18:45:12.000000 nobuco-0.1.0/nobuco/converters/tensor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1322 2023-03-08 10:20:55.000000 nobuco-0.1.0/nobuco/converters/type_cast.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-15 10:52:46.601614 nobuco-0.1.0/nobuco/entity/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-10-12 10:29:29.000000 nobuco-0.1.0/nobuco/entity/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3152 2023-03-03 13:25:51.000000 nobuco-0.1.0/nobuco/entity/keras.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13052 2023-03-10 22:09:16.000000 nobuco-0.1.0/nobuco/entity/pytorch.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      187 2023-03-03 13:30:15.000000 nobuco-0.1.0/nobuco/funcs.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-15 10:52:46.601614 nobuco-0.1.0/nobuco/trace/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-10-12 09:47:48.000000 nobuco-0.1.0/nobuco/trace/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1409 2023-03-10 22:09:16.000000 nobuco-0.1.0/nobuco/trace/tensor_storage.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9354 2023-03-10 20:01:46.000000 nobuco-0.1.0/nobuco/trace/trace.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2632 2023-03-10 22:18:16.000000 nobuco-0.1.0/nobuco/util.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-15 10:52:46.601614 nobuco-0.1.0/nobuco/vis/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-02-28 17:54:05.000000 nobuco-0.1.0/nobuco/vis/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1952 2023-03-10 22:09:16.000000 nobuco-0.1.0/nobuco/vis/console_stylizer.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3172 2023-03-10 22:09:16.000000 nobuco-0.1.0/nobuco/vis/html_stylizer.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-15 10:52:46.597614 nobuco-0.1.0/nobuco.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)    17512 2023-04-15 10:52:46.000000 nobuco-0.1.0/nobuco.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     1473 2023-04-15 10:52:46.000000 nobuco-0.1.0/nobuco.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-04-15 10:52:46.000000 nobuco-0.1.0/nobuco.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       11 2023-04-15 10:52:46.000000 nobuco-0.1.0/nobuco.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        7 2023-04-15 10:52:46.000000 nobuco-0.1.0/nobuco.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)      758 2023-04-15 10:52:26.000000 nobuco-0.1.0/pyproject.toml
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-04-15 10:52:46.601614 nobuco-0.1.0/setup.cfg
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-16 17:34:39.031311 nobuco-0.1.1/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2023-03-02 20:53:15.000000 nobuco-0.1.1/LICENSE
+-rw-rw-r--   0 alex      (1000) alex      (1000)       14 2023-04-15 10:44:29.000000 nobuco-0.1.1/MANIFEST.in
+-rw-rw-r--   0 alex      (1000) alex      (1000)    17729 2023-04-16 17:34:39.031311 nobuco-0.1.1/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)    15895 2023-04-16 17:33:51.000000 nobuco-0.1.1/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-16 17:34:39.027311 nobuco-0.1.1/docs/
+-rw-rw-r--   0 alex      (1000) alex      (1000)    64876 2023-03-25 20:16:55.000000 nobuco-0.1.1/docs/channel_ordering.png
+-rw-rw-r--   0 alex      (1000) alex      (1000)    63145 2023-03-25 20:46:53.000000 nobuco-0.1.1/docs/channel_ordering_forced.png
+-rw-rw-r--   0 alex      (1000) alex      (1000)    70703 2023-03-24 09:18:07.000000 nobuco-0.1.1/docs/control_if.png
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2110 2023-04-05 14:55:45.000000 nobuco-0.1.1/docs/converter_inside_converter1.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)    26497 2023-04-05 19:25:33.000000 nobuco-0.1.1/docs/converter_inside_converter1.svg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2319 2023-04-05 14:56:10.000000 nobuco-0.1.1/docs/converter_inside_converter2.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)    30325 2023-04-05 19:25:54.000000 nobuco-0.1.1/docs/converter_inside_converter2.svg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3070 2023-04-06 09:06:34.000000 nobuco-0.1.1/docs/essentials1.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)    35615 2023-04-06 09:06:58.000000 nobuco-0.1.1/docs/essentials1.svg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2811 2023-04-05 14:47:00.000000 nobuco-0.1.1/docs/essentials2.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)    32971 2023-04-05 19:22:33.000000 nobuco-0.1.1/docs/essentials2.svg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2281 2023-04-05 14:48:33.000000 nobuco-0.1.1/docs/essentials3.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)    28090 2023-04-05 19:22:46.000000 nobuco-0.1.1/docs/essentials3.svg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1559 2023-04-05 14:51:28.000000 nobuco-0.1.1/docs/inplace1.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)    18606 2023-04-05 19:23:57.000000 nobuco-0.1.1/docs/inplace1.svg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1050 2023-04-05 14:52:17.000000 nobuco-0.1.1/docs/inplace2.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11981 2023-04-05 19:24:22.000000 nobuco-0.1.1/docs/inplace2.svg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1195 2023-04-05 14:52:18.000000 nobuco-0.1.1/docs/inplace3.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14409 2023-04-05 19:25:18.000000 nobuco-0.1.1/docs/inplace3.svg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6859 2023-03-24 11:40:17.000000 nobuco-0.1.1/docs/inplace_empty.png
+-rw-rw-r--   0 alex      (1000) alex      (1000)   926558 2023-04-16 10:49:50.000000 nobuco-0.1.1/docs/nobuco.png
+-rw-rw-r--   0 alex      (1000) alex      (1000)    82036 2023-03-03 12:08:40.000000 nobuco-0.1.1/docs/tutorial.png
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-16 17:34:39.027311 nobuco-0.1.1/nobuco/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2021-06-04 16:18:38.000000 nobuco-0.1.1/nobuco/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      798 2023-03-07 13:07:06.000000 nobuco-0.1.1/nobuco/commons.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-16 17:34:39.027311 nobuco-0.1.1/nobuco/convert/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-10-12 10:30:24.000000 nobuco-0.1.1/nobuco/convert/__init__.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)    12608 2023-03-13 12:38:17.000000 nobuco-0.1.1/nobuco/convert/converter.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-16 17:34:39.027311 nobuco-0.1.1/nobuco/convert/layers/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-12-06 13:02:40.000000 nobuco-0.1.1/nobuco/convert/layers/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4992 2023-03-08 10:21:14.000000 nobuco-0.1.1/nobuco/convert/layers/channel_order.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4894 2023-03-07 15:12:41.000000 nobuco-0.1.1/nobuco/convert/layers/container.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      313 2022-12-06 13:05:18.000000 nobuco-0.1.1/nobuco/convert/layers/stub.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      918 2023-03-08 10:08:07.000000 nobuco-0.1.1/nobuco/convert/layers/weight.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3497 2023-03-07 10:32:51.000000 nobuco-0.1.1/nobuco/convert/validation.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-16 17:34:39.027311 nobuco-0.1.1/nobuco/converters/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-11-11 15:28:31.000000 nobuco-0.1.1/nobuco/converters/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2049 2023-03-06 15:27:24.000000 nobuco-0.1.1/nobuco/converters/channel_ordering.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)    71864 2023-04-16 17:28:21.000000 nobuco-0.1.1/nobuco/converters/impl.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     2459 2023-03-13 12:32:55.000000 nobuco-0.1.1/nobuco/converters/node_converter.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      384 2022-12-21 13:41:52.000000 nobuco-0.1.1/nobuco/converters/ops.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2002 2023-03-03 18:45:12.000000 nobuco-0.1.1/nobuco/converters/tensor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1322 2023-03-08 10:20:55.000000 nobuco-0.1.1/nobuco/converters/type_cast.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-16 17:34:39.027311 nobuco-0.1.1/nobuco/entity/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-10-12 10:29:29.000000 nobuco-0.1.1/nobuco/entity/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3152 2023-03-03 13:25:51.000000 nobuco-0.1.1/nobuco/entity/keras.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13052 2023-03-10 22:09:16.000000 nobuco-0.1.1/nobuco/entity/pytorch.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      187 2023-03-03 13:30:15.000000 nobuco-0.1.1/nobuco/funcs.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-16 17:34:39.031311 nobuco-0.1.1/nobuco/trace/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-10-12 09:47:48.000000 nobuco-0.1.1/nobuco/trace/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1409 2023-03-10 22:09:16.000000 nobuco-0.1.1/nobuco/trace/tensor_storage.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9354 2023-03-10 20:01:46.000000 nobuco-0.1.1/nobuco/trace/trace.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2632 2023-03-10 22:18:16.000000 nobuco-0.1.1/nobuco/util.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-16 17:34:39.031311 nobuco-0.1.1/nobuco/vis/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-02-28 17:54:05.000000 nobuco-0.1.1/nobuco/vis/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1952 2023-03-10 22:09:16.000000 nobuco-0.1.1/nobuco/vis/console_stylizer.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3172 2023-03-10 22:09:16.000000 nobuco-0.1.1/nobuco/vis/html_stylizer.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-16 17:34:39.027311 nobuco-0.1.1/nobuco.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)    17729 2023-04-16 17:34:39.000000 nobuco-0.1.1/nobuco.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1489 2023-04-16 17:34:39.000000 nobuco-0.1.1/nobuco.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-04-16 17:34:39.000000 nobuco-0.1.1/nobuco.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       17 2023-04-16 17:34:39.000000 nobuco-0.1.1/nobuco.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        7 2023-04-16 17:34:39.000000 nobuco-0.1.1/nobuco.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)      770 2023-04-16 17:34:03.000000 nobuco-0.1.1/pyproject.toml
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-04-16 17:34:39.031311 nobuco-0.1.1/setup.cfg
```

### Comparing `nobuco-0.1.0/LICENSE` & `nobuco-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.0/PKG-INFO` & `nobuco-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobuco
-Version: 0.1.0
+Version: 0.1.1
 Summary: Pytorch to Tensorflow conversion made somewhat easy
 Author-email: Alexander Lutsenko <lex.lutsenko@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Alexander Lutsenko
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,16 +30,17 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+<img src="docs/nobuco.png" width="100%">
 
-**No** **Bu**llshit **Co**nverter is a tool that lets you translate pytorch models into tensorflow graphs without losing your mind.
+**No** **Bu**llshit **Co**nverter is a tool that helps you translate pytorch models into tensorflow graphs without losing your mind.
 
 - Supports a wide range of architectures
   - [x] Control flow ops (If, While)
   - [x] Recurrent layers (LSTM, GRU)
   - [x] Arbitrary torch functions
 - Simple
 - Flexible
@@ -76,14 +77,20 @@
         x = nn.Hardsigmoid()(x)
         x = 1 - x[:, ::2] * x[:, 1::2]
         return x
 ````
 
 The process is exactly what you would expect. Instantiate the module, create dummy inputs and call the magic function:
 
+```python
+from nobuco.convert.converter import pytorch_to_keras
+from nobuco.commons import ChannelOrder, ChannelOrderingStrategy
+from nobuco.convert.layers.weight import WeightLayer
+```
+
 ````python
 dummy_image = torch.rand(size=(1, 3, 256, 256))
 pytorch_module = MyModule().eval()
 
 keras_model = pytorch_to_keras(
     pytorch_module,
     args=[dummy_image], kwargs=None,
@@ -125,15 +132,15 @@
 And the happy result:
 
 <img src="docs/tutorial.png" width="30%">
 
 The example above is artificial but it illustrates the point.
 It's not feasible to provide a node converter for every existing pytorch op. There's literally [thousands](https://dev-discuss.pytorch.org/t/where-do-the-2000-pytorch-operators-come-from-more-than-you-wanted-to-know/) of them! 
 Best we can do without the converter constantly lacking essential functionality, being riddled with bugs, doing weird stuff and breaking apart with every other PT/TF release 
-is to keep the system simple and customizable, make it clear where a problem comes from and let the _user_ sort things out.
+is to keep the tool simple and customizable, make it clear where a problem comes from and let the _user_ sort things out.
 Usually it's easy for a human to translate an isolated operation from one framework to another.
 Reproducing the graph structure is a different matter entirely. Good thing Nobuco has you covered.
 
 ## Channel order wizardry
 
 Some operations assume its input tensors have a channel dimension. 
 And as you probably know, pytorch and tensorflow do not agree on the layout of such tensors.
@@ -152,15 +159,15 @@
   - Convenient for converting channel-aware operations (convolution, batchnorm).
 - `FORCE_PYTORCH_ORDER`
   - Input tensors entering the node will look exactly as they do in the original pytorch graph. 
   - Use it when the node does not interpret its input tensors as having a channel dimension (linear, matmul). 
 - `MINIMUM_TRANSPOSITIONS`
   - The channel order is decided by a majority vote (whichever prevails among the inputs). This way the number of coercions (i.e. tensor transpositions) is kept to the minimum.
   It also means whenever there's only one input, it will be left untouched.
-  - Best choice for element-wise ops (most of activations).
+  - Best choice for element-wise ops (most activations).
 - `MANUAL`
   - You are on your own. In exchange for unrestricted freedom, you take responsibility to coerce input tensors to suitable channel order and to also annotate output tensors with their order.
 
 The simple lazy approach makes wonders in most situations, but sometimes it produces suboptimal graphs.
 Consider the code below. Imagine this is some sort of text processing network. 
 It first applies a GRU layer which assumes the inputs do not have a channel dimension, so its input/output layouts are the same in both pytorch and tensorflow.
 But then, the outputs are passed to a couple of 1D convolutions which are channel-aware. 
@@ -245,15 +252,15 @@
 ```
 
 <img src="docs/inplace2.svg" width="100%">
 
 You see, tensorflow graphs (and many other formats like ONNX) do not support in-place ops.
 So when we take slice (`x[:, 1:2, 16:25, 8::2]`) in TF/ONNX, the result is not a view of the original tensor but a copy. 
 This copy is then passed to `relu` (which is not in-place either), and its result is not used anywhere. 
-As you can see above, the output tensors of `__getitem__` and `relu_` are <span style="color:gray">grayed out</span>, and these operations a not included in the graph.
+As you can see above, the output tensors of `__getitem__` and `relu_` are <span style="color:gray">grayed out</span>, and these operations are excluded from the graph.
 In fact, it's empty:
 
 <img src="docs/inplace_empty.png" width="30%">
 
 The easiest way of fixing this is to explicitly assign the result to the slice.
 Conveniently enough, most standard in-place operations in pytorch do return their modified arguments as outputs.
 
@@ -295,15 +302,15 @@
             x = x - 1
         x = self.conv_shared(x)
         return x
 ```
 
 Of course, it's possible to translate the dynamic module into a tensorflow layer
 (don't forget to decorate it with `@tf.function` for autograph to kick in).
-But what if it contains inner modules, do we have to replicate them in tensorflow all by hand?
+But what if it contains inner modules, do you replicate them in tensorflow all by hand?
 Not unless you want to! 
 Just convert them separately and use the resulting graph inside the parent layer.
 
 ```python
 class ControlIfKeras(tf.keras.layers.Layer):
     def __init__(self, conv_pre, conv_true, conv_false, conv_shared, *args, **kwargs):
         super().__init__(*args, **kwargs)
```

### Comparing `nobuco-0.1.0/README.md` & `nobuco-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+<img src="docs/nobuco.png" width="100%">
 
-**No** **Bu**llshit **Co**nverter is a tool that lets you translate pytorch models into tensorflow graphs without losing your mind.
+**No** **Bu**llshit **Co**nverter is a tool that helps you translate pytorch models into tensorflow graphs without losing your mind.
 
 - Supports a wide range of architectures
   - [x] Control flow ops (If, While)
   - [x] Recurrent layers (LSTM, GRU)
   - [x] Arbitrary torch functions
 - Simple
 - Flexible
@@ -40,14 +41,20 @@
         x = nn.Hardsigmoid()(x)
         x = 1 - x[:, ::2] * x[:, 1::2]
         return x
 ````
 
 The process is exactly what you would expect. Instantiate the module, create dummy inputs and call the magic function:
 
+```python
+from nobuco.convert.converter import pytorch_to_keras
+from nobuco.commons import ChannelOrder, ChannelOrderingStrategy
+from nobuco.convert.layers.weight import WeightLayer
+```
+
 ````python
 dummy_image = torch.rand(size=(1, 3, 256, 256))
 pytorch_module = MyModule().eval()
 
 keras_model = pytorch_to_keras(
     pytorch_module,
     args=[dummy_image], kwargs=None,
@@ -89,15 +96,15 @@
 And the happy result:
 
 <img src="docs/tutorial.png" width="30%">
 
 The example above is artificial but it illustrates the point.
 It's not feasible to provide a node converter for every existing pytorch op. There's literally [thousands](https://dev-discuss.pytorch.org/t/where-do-the-2000-pytorch-operators-come-from-more-than-you-wanted-to-know/) of them! 
 Best we can do without the converter constantly lacking essential functionality, being riddled with bugs, doing weird stuff and breaking apart with every other PT/TF release 
-is to keep the system simple and customizable, make it clear where a problem comes from and let the _user_ sort things out.
+is to keep the tool simple and customizable, make it clear where a problem comes from and let the _user_ sort things out.
 Usually it's easy for a human to translate an isolated operation from one framework to another.
 Reproducing the graph structure is a different matter entirely. Good thing Nobuco has you covered.
 
 ## Channel order wizardry
 
 Some operations assume its input tensors have a channel dimension. 
 And as you probably know, pytorch and tensorflow do not agree on the layout of such tensors.
@@ -116,15 +123,15 @@
   - Convenient for converting channel-aware operations (convolution, batchnorm).
 - `FORCE_PYTORCH_ORDER`
   - Input tensors entering the node will look exactly as they do in the original pytorch graph. 
   - Use it when the node does not interpret its input tensors as having a channel dimension (linear, matmul). 
 - `MINIMUM_TRANSPOSITIONS`
   - The channel order is decided by a majority vote (whichever prevails among the inputs). This way the number of coercions (i.e. tensor transpositions) is kept to the minimum.
   It also means whenever there's only one input, it will be left untouched.
-  - Best choice for element-wise ops (most of activations).
+  - Best choice for element-wise ops (most activations).
 - `MANUAL`
   - You are on your own. In exchange for unrestricted freedom, you take responsibility to coerce input tensors to suitable channel order and to also annotate output tensors with their order.
 
 The simple lazy approach makes wonders in most situations, but sometimes it produces suboptimal graphs.
 Consider the code below. Imagine this is some sort of text processing network. 
 It first applies a GRU layer which assumes the inputs do not have a channel dimension, so its input/output layouts are the same in both pytorch and tensorflow.
 But then, the outputs are passed to a couple of 1D convolutions which are channel-aware. 
@@ -209,15 +216,15 @@
 ```
 
 <img src="docs/inplace2.svg" width="100%">
 
 You see, tensorflow graphs (and many other formats like ONNX) do not support in-place ops.
 So when we take slice (`x[:, 1:2, 16:25, 8::2]`) in TF/ONNX, the result is not a view of the original tensor but a copy. 
 This copy is then passed to `relu` (which is not in-place either), and its result is not used anywhere. 
-As you can see above, the output tensors of `__getitem__` and `relu_` are <span style="color:gray">grayed out</span>, and these operations a not included in the graph.
+As you can see above, the output tensors of `__getitem__` and `relu_` are <span style="color:gray">grayed out</span>, and these operations are excluded from the graph.
 In fact, it's empty:
 
 <img src="docs/inplace_empty.png" width="30%">
 
 The easiest way of fixing this is to explicitly assign the result to the slice.
 Conveniently enough, most standard in-place operations in pytorch do return their modified arguments as outputs.
 
@@ -259,15 +266,15 @@
             x = x - 1
         x = self.conv_shared(x)
         return x
 ```
 
 Of course, it's possible to translate the dynamic module into a tensorflow layer
 (don't forget to decorate it with `@tf.function` for autograph to kick in).
-But what if it contains inner modules, do we have to replicate them in tensorflow all by hand?
+But what if it contains inner modules, do you replicate them in tensorflow all by hand?
 Not unless you want to! 
 Just convert them separately and use the resulting graph inside the parent layer.
 
 ```python
 class ControlIfKeras(tf.keras.layers.Layer):
     def __init__(self, conv_pre, conv_true, conv_false, conv_shared, *args, **kwargs):
         super().__init__(*args, **kwargs)
```

### Comparing `nobuco-0.1.0/docs/channel_ordering.png` & `nobuco-0.1.1/docs/channel_ordering.png`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.0/docs/channel_ordering_forced.png` & `nobuco-0.1.1/docs/channel_ordering_forced.png`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.0/docs/control_if.png` & `nobuco-0.1.1/docs/control_if.png`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.0/docs/converter_inside_converter1.html` & `nobuco-0.1.1/docs/converter_inside_converter1.html`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.0/docs/converter_inside_converter1.svg` & `nobuco-0.1.1/docs/converter_inside_converter1.svg`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.0/docs/converter_inside_converter2.html` & `nobuco-0.1.1/docs/converter_inside_converter2.html`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.0/docs/converter_inside_converter2.svg` & `nobuco-0.1.1/docs/converter_inside_converter2.svg`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.0/docs/essentials1.html` & `nobuco-0.1.1/docs/essentials1.html`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.0/docs/essentials1.svg` & `nobuco-0.1.1/docs/essentials1.svg`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.0/docs/essentials2.html` & `nobuco-0.1.1/docs/essentials2.html`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.0/docs/essentials2.svg` & `nobuco-0.1.1/docs/essentials2.svg`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.0/docs/essentials3.html` & `nobuco-0.1.1/docs/essentials3.html`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.0/docs/essentials3.svg` & `nobuco-0.1.1/docs/essentials3.svg`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.0/docs/inplace1.html` & `nobuco-0.1.1/docs/inplace1.html`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.0/docs/inplace1.svg` & `nobuco-0.1.1/docs/inplace1.svg`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.0/docs/inplace2.html` & `nobuco-0.1.1/docs/inplace2.html`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.0/docs/inplace2.svg` & `nobuco-0.1.1/docs/inplace2.svg`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.0/docs/inplace3.html` & `nobuco-0.1.1/docs/inplace3.html`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.0/docs/inplace3.svg` & `nobuco-0.1.1/docs/inplace3.svg`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.0/docs/inplace_empty.png` & `nobuco-0.1.1/docs/inplace_empty.png`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.0/docs/tutorial.png` & `nobuco-0.1.1/docs/tutorial.png`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.0/nobuco/commons.py` & `nobuco-0.1.1/nobuco/commons.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.0/nobuco/convert/converter.py` & `nobuco-0.1.1/nobuco/convert/converter.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.0/nobuco/convert/layers/channel_order.py` & `nobuco-0.1.1/nobuco/convert/layers/channel_order.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.0/nobuco/convert/layers/container.py` & `nobuco-0.1.1/nobuco/convert/layers/container.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.0/nobuco/convert/layers/weight.py` & `nobuco-0.1.1/nobuco/convert/layers/weight.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.0/nobuco/convert/validation.py` & `nobuco-0.1.1/nobuco/convert/validation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.0/nobuco/converters/channel_ordering.py` & `nobuco-0.1.1/nobuco/converters/channel_ordering.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.0/nobuco/converters/impl.py` & `nobuco-0.1.1/nobuco/converters/impl.py`

 * *Files 0% similar despite different names*

```diff
@@ -501,90 +501,90 @@
         if pad_layer is not None:
             input = pad_layer(input)
         output = conv(input)
         return output
     return func
 
 
-# @converter(F.conv2d)
-# def conv2d(input: Tensor, weight: Tensor, bias: Optional[Tensor] = None, stride: Union[_int, _size] = 1,
-#                     padding: str = "valid", dilation: Union[_int, _size] = 1, groups: _int = 1):
-#
-#     out_filters, in_filters, kh, kw = weight.shape
-#
-#     weights = weight.detach().numpy()
-#     if groups == out_filters and groups != 1:
-#         weights = tf.transpose(weights, (2, 3, 0, 1))
-#     elif groups == 1:
-#         weights = tf.transpose(weights, (2, 3, 1, 0))
-#     else:
-#         weights = tf.transpose(weights, (2, 3, 1, 0))
-#
-#     if bias is not None:
-#         biases = bias.detach().numpy()
-#         params = [weights, biases]
-#         use_bias = True
-#     else:
-#         params = [weights]
-#         use_bias = False
-#
-#     if padding != 0 and padding != (0, 0) and padding != 'valid':
-#         pad_layer = keras.layers.ZeroPadding2D(padding)
-#     else:
-#         pad_layer = None
-#
-#     if groups == out_filters and groups != 1:
-#         conv = keras.layers.DepthwiseConv2D(kernel_size=(kh, kw),
-#                                       strides=stride,
-#                                       padding='valid',
-#                                       dilation_rate=dilation,
-#                                       groups=groups,
-#                                       use_bias=use_bias,
-#                                       weights=params
-#                                       )
-#     elif groups == 1:
-#         conv = keras.layers.Conv2D(filters=out_filters,
-#                              kernel_size=(kh, kw),
-#                              strides=stride,
-#                              padding='valid',
-#                              dilation_rate=dilation,
-#                              groups=groups,
-#                              use_bias=use_bias,
-#                              weights=params
-#                              )
-#     else:
-#         def split_params(params, groups, axis):
-#             params_split = [np.split(p, groups, axis=axis) for p in params]
-#             return list(zip(*params_split))
-#
-#         params_split = split_params(params, groups, axis=-1)
-#
-#         def grouped_conv2d(inputs, filters, kernel_size, strides, groups, dilation=dilation):
-#             splits = tf.split(inputs, groups, axis=-1)
-#             convolved_splits = [
-#                 keras.layers.Conv2D(filters // groups,
-#                                     kernel_size=kernel_size,
-#                                     strides=strides,
-#                                     padding='valid',
-#                                     dilation_rate=dilation,
-#                                     use_bias=use_bias,
-#                                     weights=params_split[i]
-#                                     )(split)
-#                 for i, split in enumerate(splits)
-#             ]
-#             return tf.concat(convolved_splits, -1)
-#
-#         conv = lambda x: grouped_conv2d(x, out_filters, kernel_size=(kh, kw), strides=stride, groups=groups, dilation=dilation)
-#
-#     def func(input, *args, **kwargs):
-#         if pad_layer is not None:
-#             input = pad_layer(input)
-#         output = conv(input)
-#         return output
-#     return func
+@converter(F.conv2d)
+def conv2d(input: Tensor, weight: Tensor, bias: Optional[Tensor] = None, stride: Union[_int, _size] = 1,
+                    padding: str = "valid", dilation: Union[_int, _size] = 1, groups: _int = 1):
+
+    out_filters, in_filters, kh, kw = weight.shape
+
+    weights = weight.detach().numpy()
+    if groups == out_filters and groups != 1:
+        weights = tf.transpose(weights, (2, 3, 0, 1))
+    elif groups == 1:
+        weights = tf.transpose(weights, (2, 3, 1, 0))
+    else:
+        weights = tf.transpose(weights, (2, 3, 1, 0))
+
+    if bias is not None:
+        biases = bias.detach().numpy()
+        params = [weights, biases]
+        use_bias = True
+    else:
+        params = [weights]
+        use_bias = False
+
+    if padding != 0 and padding != (0, 0) and padding != 'valid':
+        pad_layer = keras.layers.ZeroPadding2D(padding)
+    else:
+        pad_layer = None
+
+    if groups == out_filters and groups != 1:
+        conv = keras.layers.DepthwiseConv2D(kernel_size=(kh, kw),
+                                      strides=stride,
+                                      padding='valid',
+                                      dilation_rate=dilation,
+                                      groups=groups,
+                                      use_bias=use_bias,
+                                      weights=params
+                                      )
+    elif groups == 1:
+        conv = keras.layers.Conv2D(filters=out_filters,
+                             kernel_size=(kh, kw),
+                             strides=stride,
+                             padding='valid',
+                             dilation_rate=dilation,
+                             groups=groups,
+                             use_bias=use_bias,
+                             weights=params
+                             )
+    else:
+        def split_params(params, groups, axis):
+            params_split = [np.split(p, groups, axis=axis) for p in params]
+            return list(zip(*params_split))
+
+        params_split = split_params(params, groups, axis=-1)
+
+        def grouped_conv2d(inputs, filters, kernel_size, strides, groups, dilation=dilation):
+            splits = tf.split(inputs, groups, axis=-1)
+            convolved_splits = [
+                keras.layers.Conv2D(filters // groups,
+                                    kernel_size=kernel_size,
+                                    strides=strides,
+                                    padding='valid',
+                                    dilation_rate=dilation,
+                                    use_bias=use_bias,
+                                    weights=params_split[i]
+                                    )(split)
+                for i, split in enumerate(splits)
+            ]
+            return tf.concat(convolved_splits, -1)
+
+        conv = lambda x: grouped_conv2d(x, out_filters, kernel_size=(kh, kw), strides=stride, groups=groups, dilation=dilation)
+
+    def func(input, *args, **kwargs):
+        if pad_layer is not None:
+            input = pad_layer(input)
+        output = conv(input)
+        return output
+    return func
 
 
 @converter(nn.ConvTranspose2d)
 def convTranspose2d(self, input: Tensor, output_size: Optional[List[int]] = None):
     weight = self.weight
     bias = self.bias
     groups = self.groups
```

### Comparing `nobuco-0.1.0/nobuco/converters/node_converter.py` & `nobuco-0.1.1/nobuco/converters/node_converter.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.0/nobuco/converters/tensor.py` & `nobuco-0.1.1/nobuco/converters/tensor.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.0/nobuco/converters/type_cast.py` & `nobuco-0.1.1/nobuco/converters/type_cast.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.0/nobuco/entity/keras.py` & `nobuco-0.1.1/nobuco/entity/keras.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.0/nobuco/entity/pytorch.py` & `nobuco-0.1.1/nobuco/entity/pytorch.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.0/nobuco/trace/tensor_storage.py` & `nobuco-0.1.1/nobuco/trace/tensor_storage.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.0/nobuco/trace/trace.py` & `nobuco-0.1.1/nobuco/trace/trace.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.0/nobuco/util.py` & `nobuco-0.1.1/nobuco/util.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.0/nobuco/vis/console_stylizer.py` & `nobuco-0.1.1/nobuco/vis/console_stylizer.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.0/nobuco/vis/html_stylizer.py` & `nobuco-0.1.1/nobuco/vis/html_stylizer.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.0/nobuco.egg-info/PKG-INFO` & `nobuco-0.1.1/nobuco.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobuco
-Version: 0.1.0
+Version: 0.1.1
 Summary: Pytorch to Tensorflow conversion made somewhat easy
 Author-email: Alexander Lutsenko <lex.lutsenko@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Alexander Lutsenko
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,16 +30,17 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+<img src="docs/nobuco.png" width="100%">
 
-**No** **Bu**llshit **Co**nverter is a tool that lets you translate pytorch models into tensorflow graphs without losing your mind.
+**No** **Bu**llshit **Co**nverter is a tool that helps you translate pytorch models into tensorflow graphs without losing your mind.
 
 - Supports a wide range of architectures
   - [x] Control flow ops (If, While)
   - [x] Recurrent layers (LSTM, GRU)
   - [x] Arbitrary torch functions
 - Simple
 - Flexible
@@ -76,14 +77,20 @@
         x = nn.Hardsigmoid()(x)
         x = 1 - x[:, ::2] * x[:, 1::2]
         return x
 ````
 
 The process is exactly what you would expect. Instantiate the module, create dummy inputs and call the magic function:
 
+```python
+from nobuco.convert.converter import pytorch_to_keras
+from nobuco.commons import ChannelOrder, ChannelOrderingStrategy
+from nobuco.convert.layers.weight import WeightLayer
+```
+
 ````python
 dummy_image = torch.rand(size=(1, 3, 256, 256))
 pytorch_module = MyModule().eval()
 
 keras_model = pytorch_to_keras(
     pytorch_module,
     args=[dummy_image], kwargs=None,
@@ -125,15 +132,15 @@
 And the happy result:
 
 <img src="docs/tutorial.png" width="30%">
 
 The example above is artificial but it illustrates the point.
 It's not feasible to provide a node converter for every existing pytorch op. There's literally [thousands](https://dev-discuss.pytorch.org/t/where-do-the-2000-pytorch-operators-come-from-more-than-you-wanted-to-know/) of them! 
 Best we can do without the converter constantly lacking essential functionality, being riddled with bugs, doing weird stuff and breaking apart with every other PT/TF release 
-is to keep the system simple and customizable, make it clear where a problem comes from and let the _user_ sort things out.
+is to keep the tool simple and customizable, make it clear where a problem comes from and let the _user_ sort things out.
 Usually it's easy for a human to translate an isolated operation from one framework to another.
 Reproducing the graph structure is a different matter entirely. Good thing Nobuco has you covered.
 
 ## Channel order wizardry
 
 Some operations assume its input tensors have a channel dimension. 
 And as you probably know, pytorch and tensorflow do not agree on the layout of such tensors.
@@ -152,15 +159,15 @@
   - Convenient for converting channel-aware operations (convolution, batchnorm).
 - `FORCE_PYTORCH_ORDER`
   - Input tensors entering the node will look exactly as they do in the original pytorch graph. 
   - Use it when the node does not interpret its input tensors as having a channel dimension (linear, matmul). 
 - `MINIMUM_TRANSPOSITIONS`
   - The channel order is decided by a majority vote (whichever prevails among the inputs). This way the number of coercions (i.e. tensor transpositions) is kept to the minimum.
   It also means whenever there's only one input, it will be left untouched.
-  - Best choice for element-wise ops (most of activations).
+  - Best choice for element-wise ops (most activations).
 - `MANUAL`
   - You are on your own. In exchange for unrestricted freedom, you take responsibility to coerce input tensors to suitable channel order and to also annotate output tensors with their order.
 
 The simple lazy approach makes wonders in most situations, but sometimes it produces suboptimal graphs.
 Consider the code below. Imagine this is some sort of text processing network. 
 It first applies a GRU layer which assumes the inputs do not have a channel dimension, so its input/output layouts are the same in both pytorch and tensorflow.
 But then, the outputs are passed to a couple of 1D convolutions which are channel-aware. 
@@ -245,15 +252,15 @@
 ```
 
 <img src="docs/inplace2.svg" width="100%">
 
 You see, tensorflow graphs (and many other formats like ONNX) do not support in-place ops.
 So when we take slice (`x[:, 1:2, 16:25, 8::2]`) in TF/ONNX, the result is not a view of the original tensor but a copy. 
 This copy is then passed to `relu` (which is not in-place either), and its result is not used anywhere. 
-As you can see above, the output tensors of `__getitem__` and `relu_` are <span style="color:gray">grayed out</span>, and these operations a not included in the graph.
+As you can see above, the output tensors of `__getitem__` and `relu_` are <span style="color:gray">grayed out</span>, and these operations are excluded from the graph.
 In fact, it's empty:
 
 <img src="docs/inplace_empty.png" width="30%">
 
 The easiest way of fixing this is to explicitly assign the result to the slice.
 Conveniently enough, most standard in-place operations in pytorch do return their modified arguments as outputs.
 
@@ -295,15 +302,15 @@
             x = x - 1
         x = self.conv_shared(x)
         return x
 ```
 
 Of course, it's possible to translate the dynamic module into a tensorflow layer
 (don't forget to decorate it with `@tf.function` for autograph to kick in).
-But what if it contains inner modules, do we have to replicate them in tensorflow all by hand?
+But what if it contains inner modules, do you replicate them in tensorflow all by hand?
 Not unless you want to! 
 Just convert them separately and use the resulting graph inside the parent layer.
 
 ```python
 class ControlIfKeras(tf.keras.layers.Layer):
     def __init__(self, conv_pre, conv_true, conv_false, conv_shared, *args, **kwargs):
         super().__init__(*args, **kwargs)
```

### Comparing `nobuco-0.1.0/nobuco.egg-info/SOURCES.txt` & `nobuco-0.1.1/nobuco.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 docs/inplace1.html
 docs/inplace1.svg
 docs/inplace2.html
 docs/inplace2.svg
 docs/inplace3.html
 docs/inplace3.svg
 docs/inplace_empty.png
+docs/nobuco.png
 docs/tutorial.png
 nobuco/__init__.py
 nobuco/commons.py
 nobuco/funcs.py
 nobuco/util.py
 nobuco.egg-info/PKG-INFO
 nobuco.egg-info/SOURCES.txt
```

### Comparing `nobuco-0.1.0/pyproject.toml` & `nobuco-0.1.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nobuco"
-version = "0.1.0"
+version = "0.1.1"
 description = "Pytorch to Tensorflow conversion made somewhat easy"
 readme = "README.md"
 authors = [
   { name="Alexander Lutsenko", email="lex.lutsenko@gmail.com" },
 ]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 keywords = ["pytorch", "tensorflow", "keras", "converter"]
 dependencies = [
     "sty >= 1.0.0",
+    "numpy"
 ]
 requires-python = ">=3.7"
 
 [project.urls]
 "Homepage" = "https://github.com/AlexanderLutsenko/nobuco"
 "Bug Tracker" = "https://github.com/AlexanderLutsenko/nobuco/issues"
```

