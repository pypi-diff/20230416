# Comparing `tmp/pluralkit-1.1.1.tar.gz` & `tmp/pluralkit-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pluralkit-1.1.1.tar", last modified: Fri Dec 30 23:51:52 2022, max compression
+gzip compressed data, was "pluralkit-1.1.2.tar", last modified: Sun Apr 16 00:48:33 2023, max compression
```

## Comparing `pluralkit-1.1.1.tar` & `pluralkit-1.1.2.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2022-12-30 23:51:52.235798 pluralkit-1.1.1/
--rw-rw-r--   0 k         (1001) k         (1001)     1068 2022-12-30 16:02:53.000000 pluralkit-1.1.1/LICENSE
--rw-rw-r--   0 k         (1001) k         (1001)      267 2022-12-30 16:02:53.000000 pluralkit-1.1.1/MANIFEST.in
--rw-rw-r--   0 k         (1001) k         (1001)     5450 2022-12-30 23:51:52.235798 pluralkit-1.1.1/PKG-INFO
--rw-rw-r--   0 k         (1001) k         (1001)     3519 2022-12-30 16:02:53.000000 pluralkit-1.1.1/README.md
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2022-12-30 23:51:52.231798 pluralkit-1.1.1/docs/
--rw-rw-r--   0 k         (1001) k         (1001)      634 2022-12-30 16:02:53.000000 pluralkit-1.1.1/docs/Makefile
--rw-rw-r--   0 k         (1001) k         (1001)      652 2022-12-30 16:02:53.000000 pluralkit-1.1.1/docs/README.md
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2022-12-30 23:51:52.231798 pluralkit-1.1.1/docs/_build/
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2022-12-30 23:51:52.231798 pluralkit-1.1.1/docs/_build/html/
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2022-12-30 23:51:52.231798 pluralkit-1.1.1/docs/_build/html/_sources/
--rw-rw-r--   0 k         (1001) k         (1001)     1273 2022-12-30 16:02:53.000000 pluralkit-1.1.1/docs/_build/html/_sources/index.rst.txt
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2022-12-30 23:51:52.231798 pluralkit-1.1.1/docs/_build/html/_sources/source/
--rw-rw-r--   0 k         (1001) k         (1001)     3929 2022-12-30 19:14:51.000000 pluralkit-1.1.1/docs/_build/html/_sources/source/changelog.rst.txt
--rw-rw-r--   0 k         (1001) k         (1001)    12062 2022-12-30 16:22:51.000000 pluralkit-1.1.1/docs/_build/html/_sources/source/quickstart.rst.txt
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2022-12-30 23:51:52.231798 pluralkit-1.1.1/docs/_build/html/_sources/source/v1/
--rw-rw-r--   0 k         (1001) k         (1001)     1761 2022-12-30 16:02:53.000000 pluralkit-1.1.1/docs/_build/html/_sources/source/v1/api.rst.txt
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2022-12-30 23:51:52.231798 pluralkit-1.1.1/docs/_build/html/_sources/source/v2/
--rw-rw-r--   0 k         (1001) k         (1001)     2943 2022-12-30 18:59:51.000000 pluralkit-1.1.1/docs/_build/html/_sources/source/v2/api.rst.txt
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2022-12-30 23:51:52.231798 pluralkit-1.1.1/docs/_build/html/_static/
--rw-rw-r--   0 k         (1001) k         (1001)        0 2022-12-30 16:23:23.000000 pluralkit-1.1.1/docs/_build/html/_static/__init__.py
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2022-12-30 23:51:52.231798 pluralkit-1.1.1/docs/_build/html/_static/vendor/
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2022-12-30 23:51:52.231798 pluralkit-1.1.1/docs/_build/html/_static/vendor/fontawesome/
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2022-12-30 23:51:52.231798 pluralkit-1.1.1/docs/_build/html/_static/vendor/fontawesome/5.13.0/
--rw-rw-r--   0 k         (1001) k         (1001)     1548 2022-12-30 16:23:23.000000 pluralkit-1.1.1/docs/_build/html/_static/vendor/fontawesome/5.13.0/LICENSE.txt
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2022-12-30 23:51:52.231798 pluralkit-1.1.1/docs/_build/html/_static/vendor/lato_latin-ext/
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2022-12-30 23:51:52.231798 pluralkit-1.1.1/docs/_build/html/_static/vendor/lato_latin-ext/1.44.1/
--rw-rw-r--   0 k         (1001) k         (1001)     1054 2022-12-30 16:23:23.000000 pluralkit-1.1.1/docs/_build/html/_static/vendor/lato_latin-ext/1.44.1/LICENSE.md
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2022-12-30 23:51:52.231798 pluralkit-1.1.1/docs/_build/html/_static/vendor/open-sans_all/
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2022-12-30 23:51:52.231798 pluralkit-1.1.1/docs/_build/html/_static/vendor/open-sans_all/1.44.1/
--rw-rw-r--   0 k         (1001) k         (1001)     1054 2022-12-30 16:23:23.000000 pluralkit-1.1.1/docs/_build/html/_static/vendor/open-sans_all/1.44.1/LICENSE.md
--rw-rw-r--   0 k         (1001) k         (1001)     3312 2022-12-30 16:02:53.000000 pluralkit-1.1.1/docs/conf.py
--rw-rw-r--   0 k         (1001) k         (1001)     1273 2022-12-30 16:02:53.000000 pluralkit-1.1.1/docs/index.rst
--rw-rw-r--   0 k         (1001) k         (1001)      234 2022-12-30 16:02:53.000000 pluralkit-1.1.1/docs/requirements.txt
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2022-12-30 23:51:52.231798 pluralkit-1.1.1/docs/source/
--rw-rw-r--   0 k         (1001) k         (1001)     3932 2022-12-30 19:15:15.000000 pluralkit-1.1.1/docs/source/changelog.rst
--rw-rw-r--   0 k         (1001) k         (1001)    12062 2022-12-30 16:22:51.000000 pluralkit-1.1.1/docs/source/quickstart.rst
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2022-12-30 23:51:52.231798 pluralkit-1.1.1/docs/source/v1/
--rw-rw-r--   0 k         (1001) k         (1001)     1761 2022-12-30 16:02:53.000000 pluralkit-1.1.1/docs/source/v1/api.rst
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2022-12-30 23:51:52.231798 pluralkit-1.1.1/docs/source/v2/
--rw-rw-r--   0 k         (1001) k         (1001)     2943 2022-12-30 18:59:51.000000 pluralkit-1.1.1/docs/source/v2/api.rst
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2022-12-30 23:51:52.231798 pluralkit-1.1.1/pluralkit/
--rw-rw-r--   0 k         (1001) k         (1001)      252 2022-12-30 16:02:53.000000 pluralkit-1.1.1/pluralkit/__init__.py
--rw-rw-r--   0 k         (1001) k         (1001)      248 2022-12-30 23:48:52.000000 pluralkit-1.1.1/pluralkit/__version__.py
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2022-12-30 23:51:52.235798 pluralkit-1.1.1/pluralkit/v1/
--rw-rw-r--   0 k         (1001) k         (1001)      217 2022-12-30 16:02:53.000000 pluralkit-1.1.1/pluralkit/v1/__init__.py
--rw-rw-r--   0 k         (1001) k         (1001)    32468 2022-12-30 16:02:53.000000 pluralkit-1.1.1/pluralkit/v1/client.py
--rw-rw-r--   0 k         (1001) k         (1001)     2824 2022-12-30 16:02:53.000000 pluralkit-1.1.1/pluralkit/v1/errors.py
--rw-rw-r--   0 k         (1001) k         (1001)    38036 2022-12-30 16:02:53.000000 pluralkit-1.1.1/pluralkit/v1/models.py
--rw-rw-r--   0 k         (1001) k         (1001)     4302 2022-12-30 16:02:53.000000 pluralkit-1.1.1/pluralkit/v1/utils.py
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2022-12-30 23:51:52.235798 pluralkit-1.1.1/pluralkit/v2/
--rw-rw-r--   0 k         (1001) k         (1001)      666 2022-12-30 18:59:05.000000 pluralkit-1.1.1/pluralkit/v2/__init__.py
--rw-rw-r--   0 k         (1001) k         (1001)    49619 2022-12-30 18:30:46.000000 pluralkit-1.1.1/pluralkit/v2/client.py
--rw-rw-r--   0 k         (1001) k         (1001)     2821 2022-12-30 16:02:53.000000 pluralkit-1.1.1/pluralkit/v2/errors.py
--rw-rw-r--   0 k         (1001) k         (1001)    38702 2022-12-30 23:40:11.000000 pluralkit-1.1.1/pluralkit/v2/models.py
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2022-12-30 23:51:52.231798 pluralkit-1.1.1/pluralkit.egg-info/
--rw-rw-r--   0 k         (1001) k         (1001)     5450 2022-12-30 23:51:52.000000 pluralkit-1.1.1/pluralkit.egg-info/PKG-INFO
--rw-rw-r--   0 k         (1001) k         (1001)     1166 2022-12-30 23:51:52.000000 pluralkit-1.1.1/pluralkit.egg-info/SOURCES.txt
--rw-rw-r--   0 k         (1001) k         (1001)        1 2022-12-30 23:51:52.000000 pluralkit-1.1.1/pluralkit.egg-info/dependency_links.txt
--rw-rw-r--   0 k         (1001) k         (1001)      188 2022-12-30 23:51:52.000000 pluralkit-1.1.1/pluralkit.egg-info/requires.txt
--rw-rw-r--   0 k         (1001) k         (1001)       10 2022-12-30 23:51:52.000000 pluralkit-1.1.1/pluralkit.egg-info/top_level.txt
--rw-rw-r--   0 k         (1001) k         (1001)       38 2022-12-30 23:51:52.235798 pluralkit-1.1.1/setup.cfg
--rw-rw-r--   0 k         (1001) k         (1001)     2217 2022-12-30 16:02:53.000000 pluralkit-1.1.1/setup.py
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2022-12-30 23:51:52.235798 pluralkit-1.1.1/tests/
--rw-rw-r--   0 k         (1001) k         (1001)     6785 2022-12-30 16:02:53.000000 pluralkit-1.1.1/tests/test_member.py
--rw-rw-r--   0 k         (1001) k         (1001)      503 2022-12-30 16:02:53.000000 pluralkit-1.1.1/tests/test_misc.py
--rw-rw-r--   0 k         (1001) k         (1001)     2671 2022-12-30 16:02:53.000000 pluralkit-1.1.1/tests/test_system.py
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-04-16 00:48:33.764970 pluralkit-1.1.2/
+-rw-rw-r--   0 k         (1001) k         (1001)     1068 2022-12-30 16:02:53.000000 pluralkit-1.1.2/LICENSE
+-rw-rw-r--   0 k         (1001) k         (1001)      267 2022-12-30 16:02:53.000000 pluralkit-1.1.2/MANIFEST.in
+-rw-rw-r--   0 k         (1001) k         (1001)     5450 2023-04-16 00:48:33.764970 pluralkit-1.1.2/PKG-INFO
+-rw-rw-r--   0 k         (1001) k         (1001)     3519 2022-12-30 16:02:53.000000 pluralkit-1.1.2/README.md
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-04-16 00:48:33.760970 pluralkit-1.1.2/docs/
+-rw-rw-r--   0 k         (1001) k         (1001)      634 2022-12-30 16:02:53.000000 pluralkit-1.1.2/docs/Makefile
+-rw-rw-r--   0 k         (1001) k         (1001)      652 2022-12-30 16:02:53.000000 pluralkit-1.1.2/docs/README.md
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-04-16 00:48:33.760970 pluralkit-1.1.2/docs/_build/
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-04-16 00:48:33.760970 pluralkit-1.1.2/docs/_build/html/
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-04-16 00:48:33.760970 pluralkit-1.1.2/docs/_build/html/_sources/
+-rw-rw-r--   0 k         (1001) k         (1001)     1273 2022-12-30 16:02:53.000000 pluralkit-1.1.2/docs/_build/html/_sources/index.rst.txt
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-04-16 00:48:33.760970 pluralkit-1.1.2/docs/_build/html/_sources/source/
+-rw-rw-r--   0 k         (1001) k         (1001)     3929 2022-12-30 19:14:51.000000 pluralkit-1.1.2/docs/_build/html/_sources/source/changelog.rst.txt
+-rw-rw-r--   0 k         (1001) k         (1001)    12062 2022-12-30 16:22:51.000000 pluralkit-1.1.2/docs/_build/html/_sources/source/quickstart.rst.txt
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-04-16 00:48:33.760970 pluralkit-1.1.2/docs/_build/html/_sources/source/v1/
+-rw-rw-r--   0 k         (1001) k         (1001)     1761 2022-12-30 16:02:53.000000 pluralkit-1.1.2/docs/_build/html/_sources/source/v1/api.rst.txt
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-04-16 00:48:33.764970 pluralkit-1.1.2/docs/_build/html/_sources/source/v2/
+-rw-rw-r--   0 k         (1001) k         (1001)     2943 2022-12-30 18:59:51.000000 pluralkit-1.1.2/docs/_build/html/_sources/source/v2/api.rst.txt
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-04-16 00:48:33.764970 pluralkit-1.1.2/docs/_build/html/_static/
+-rw-rw-r--   0 k         (1001) k         (1001)        0 2022-12-30 16:23:23.000000 pluralkit-1.1.2/docs/_build/html/_static/__init__.py
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-04-16 00:48:33.760970 pluralkit-1.1.2/docs/_build/html/_static/vendor/
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-04-16 00:48:33.760970 pluralkit-1.1.2/docs/_build/html/_static/vendor/fontawesome/
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-04-16 00:48:33.764970 pluralkit-1.1.2/docs/_build/html/_static/vendor/fontawesome/5.13.0/
+-rw-rw-r--   0 k         (1001) k         (1001)     1548 2022-12-30 16:23:23.000000 pluralkit-1.1.2/docs/_build/html/_static/vendor/fontawesome/5.13.0/LICENSE.txt
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-04-16 00:48:33.760970 pluralkit-1.1.2/docs/_build/html/_static/vendor/lato_latin-ext/
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-04-16 00:48:33.764970 pluralkit-1.1.2/docs/_build/html/_static/vendor/lato_latin-ext/1.44.1/
+-rw-rw-r--   0 k         (1001) k         (1001)     1054 2022-12-30 16:23:23.000000 pluralkit-1.1.2/docs/_build/html/_static/vendor/lato_latin-ext/1.44.1/LICENSE.md
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-04-16 00:48:33.760970 pluralkit-1.1.2/docs/_build/html/_static/vendor/open-sans_all/
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-04-16 00:48:33.764970 pluralkit-1.1.2/docs/_build/html/_static/vendor/open-sans_all/1.44.1/
+-rw-rw-r--   0 k         (1001) k         (1001)     1054 2022-12-30 16:23:23.000000 pluralkit-1.1.2/docs/_build/html/_static/vendor/open-sans_all/1.44.1/LICENSE.md
+-rw-rw-r--   0 k         (1001) k         (1001)     3312 2022-12-30 16:02:53.000000 pluralkit-1.1.2/docs/conf.py
+-rw-rw-r--   0 k         (1001) k         (1001)     1273 2022-12-30 16:02:53.000000 pluralkit-1.1.2/docs/index.rst
+-rw-rw-r--   0 k         (1001) k         (1001)      234 2022-12-30 16:02:53.000000 pluralkit-1.1.2/docs/requirements.txt
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-04-16 00:48:33.764970 pluralkit-1.1.2/docs/source/
+-rw-rw-r--   0 k         (1001) k         (1001)     3932 2022-12-30 19:15:15.000000 pluralkit-1.1.2/docs/source/changelog.rst
+-rw-rw-r--   0 k         (1001) k         (1001)    12062 2022-12-30 16:22:51.000000 pluralkit-1.1.2/docs/source/quickstart.rst
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-04-16 00:48:33.764970 pluralkit-1.1.2/docs/source/v1/
+-rw-rw-r--   0 k         (1001) k         (1001)     1761 2022-12-30 16:02:53.000000 pluralkit-1.1.2/docs/source/v1/api.rst
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-04-16 00:48:33.764970 pluralkit-1.1.2/docs/source/v2/
+-rw-rw-r--   0 k         (1001) k         (1001)     2943 2022-12-30 18:59:51.000000 pluralkit-1.1.2/docs/source/v2/api.rst
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-04-16 00:48:33.764970 pluralkit-1.1.2/pluralkit/
+-rw-rw-r--   0 k         (1001) k         (1001)      252 2022-12-31 00:26:34.000000 pluralkit-1.1.2/pluralkit/__init__.py
+-rw-rw-r--   0 k         (1001) k         (1001)      248 2023-04-16 00:45:21.000000 pluralkit-1.1.2/pluralkit/__version__.py
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-04-16 00:48:33.764970 pluralkit-1.1.2/pluralkit/v1/
+-rw-rw-r--   0 k         (1001) k         (1001)      217 2022-12-30 16:02:53.000000 pluralkit-1.1.2/pluralkit/v1/__init__.py
+-rw-rw-r--   0 k         (1001) k         (1001)    32468 2022-12-30 16:02:53.000000 pluralkit-1.1.2/pluralkit/v1/client.py
+-rw-rw-r--   0 k         (1001) k         (1001)     2824 2022-12-30 16:02:53.000000 pluralkit-1.1.2/pluralkit/v1/errors.py
+-rw-rw-r--   0 k         (1001) k         (1001)    38036 2022-12-30 16:02:53.000000 pluralkit-1.1.2/pluralkit/v1/models.py
+-rw-rw-r--   0 k         (1001) k         (1001)     4302 2022-12-30 16:02:53.000000 pluralkit-1.1.2/pluralkit/v1/utils.py
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-04-16 00:48:33.764970 pluralkit-1.1.2/pluralkit/v2/
+-rw-rw-r--   0 k         (1001) k         (1001)      666 2022-12-30 18:59:05.000000 pluralkit-1.1.2/pluralkit/v2/__init__.py
+-rw-rw-r--   0 k         (1001) k         (1001)    49619 2022-12-30 18:30:46.000000 pluralkit-1.1.2/pluralkit/v2/client.py
+-rw-rw-r--   0 k         (1001) k         (1001)     2821 2022-12-30 16:02:53.000000 pluralkit-1.1.2/pluralkit/v2/errors.py
+-rw-rw-r--   0 k         (1001) k         (1001)    38954 2023-04-16 00:40:49.000000 pluralkit-1.1.2/pluralkit/v2/models.py
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-04-16 00:48:33.764970 pluralkit-1.1.2/pluralkit.egg-info/
+-rw-rw-r--   0 k         (1001) k         (1001)     5450 2023-04-16 00:48:33.000000 pluralkit-1.1.2/pluralkit.egg-info/PKG-INFO
+-rw-rw-r--   0 k         (1001) k         (1001)     1166 2023-04-16 00:48:33.000000 pluralkit-1.1.2/pluralkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 k         (1001) k         (1001)        1 2023-04-16 00:48:33.000000 pluralkit-1.1.2/pluralkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 k         (1001) k         (1001)      188 2023-04-16 00:48:33.000000 pluralkit-1.1.2/pluralkit.egg-info/requires.txt
+-rw-rw-r--   0 k         (1001) k         (1001)       10 2023-04-16 00:48:33.000000 pluralkit-1.1.2/pluralkit.egg-info/top_level.txt
+-rw-rw-r--   0 k         (1001) k         (1001)       38 2023-04-16 00:48:33.764970 pluralkit-1.1.2/setup.cfg
+-rw-rw-r--   0 k         (1001) k         (1001)     2217 2022-12-31 00:34:09.000000 pluralkit-1.1.2/setup.py
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-04-16 00:48:33.764970 pluralkit-1.1.2/tests/
+-rw-rw-r--   0 k         (1001) k         (1001)     6785 2022-12-30 16:02:53.000000 pluralkit-1.1.2/tests/test_member.py
+-rw-rw-r--   0 k         (1001) k         (1001)      503 2022-12-30 16:02:53.000000 pluralkit-1.1.2/tests/test_misc.py
+-rw-rw-r--   0 k         (1001) k         (1001)     2671 2022-12-30 16:02:53.000000 pluralkit-1.1.2/tests/test_system.py
```

### Comparing `pluralkit-1.1.1/LICENSE` & `pluralkit-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.1/PKG-INFO` & `pluralkit-1.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pluralkit
-Version: 1.1.1
+Version: 1.1.2
 Summary: Python wrapper for PluralKit's API.
 Home-page: https://github.com/almonds0166/pluralkit.py
 Author: Madison Landry, Alyx Warner
 Author-email: pkpy@mit.edu
 License: MIT
 Project-URL: Documentation, https://pluralkit.readthedocs.io/en/latest/
 Project-URL: Issue tracker, https://github.com/almonds0166/pluralkit.py/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pluralkit Version: 1.1.1 Summary: Python wrapper
+Metadata-Version: 2.1 Name: pluralkit Version: 1.1.2 Summary: Python wrapper
 for PluralKit's API. Home-page: https://github.com/almonds0166/pluralkit.py
 Author: Madison Landry, Alyx Warner Author-email: pkpy@mit.edu License: MIT
 Project-URL: Documentation, https://pluralkit.readthedocs.io/en/latest/
 Project-URL: Issue tracker, https://github.com/almonds0166/pluralkit.py/issues
 Description: # pluralkit.py [![PyPi Version](https://img.shields.io/pypi/v/
 pluralkit.svg)](https://pypi.python.org/pypi/pluralkit/) [![Documentation
 Status](https://readthedocs.org/projects/pluralkit/badge/?version=latest)]
```

### Comparing `pluralkit-1.1.1/README.md` & `pluralkit-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.1/docs/Makefile` & `pluralkit-1.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.1/docs/README.md` & `pluralkit-1.1.2/docs/README.md`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.1/docs/_build/html/_sources/index.rst.txt` & `pluralkit-1.1.2/docs/_build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.1/docs/_build/html/_sources/source/changelog.rst.txt` & `pluralkit-1.1.2/docs/_build/html/_sources/source/changelog.rst.txt`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.1/docs/_build/html/_sources/source/quickstart.rst.txt` & `pluralkit-1.1.2/docs/_build/html/_sources/source/quickstart.rst.txt`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.1/docs/_build/html/_sources/source/v1/api.rst.txt` & `pluralkit-1.1.2/docs/_build/html/_sources/source/v1/api.rst.txt`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.1/docs/_build/html/_sources/source/v2/api.rst.txt` & `pluralkit-1.1.2/docs/_build/html/_sources/source/v2/api.rst.txt`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.1/docs/_build/html/_static/vendor/fontawesome/5.13.0/LICENSE.txt` & `pluralkit-1.1.2/docs/_build/html/_static/vendor/fontawesome/5.13.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.1/docs/_build/html/_static/vendor/lato_latin-ext/1.44.1/LICENSE.md` & `pluralkit-1.1.2/docs/_build/html/_static/vendor/lato_latin-ext/1.44.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.1/docs/_build/html/_static/vendor/open-sans_all/1.44.1/LICENSE.md` & `pluralkit-1.1.2/docs/_build/html/_static/vendor/open-sans_all/1.44.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.1/docs/conf.py` & `pluralkit-1.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.1/docs/index.rst` & `pluralkit-1.1.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.1/docs/source/changelog.rst` & `pluralkit-1.1.2/docs/source/changelog.rst`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.1/docs/source/quickstart.rst` & `pluralkit-1.1.2/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.1/docs/source/v1/api.rst` & `pluralkit-1.1.2/docs/source/v1/api.rst`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.1/docs/source/v2/api.rst` & `pluralkit-1.1.2/docs/source/v2/api.rst`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.1/pluralkit/v1/client.py` & `pluralkit-1.1.2/pluralkit/v1/client.py`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.1/pluralkit/v1/errors.py` & `pluralkit-1.1.2/pluralkit/v1/errors.py`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.1/pluralkit/v1/models.py` & `pluralkit-1.1.2/pluralkit/v1/models.py`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.1/pluralkit/v1/utils.py` & `pluralkit-1.1.2/pluralkit/v1/utils.py`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.1/pluralkit/v2/__init__.py` & `pluralkit-1.1.2/pluralkit/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.1/pluralkit/v2/client.py` & `pluralkit-1.1.2/pluralkit/v2/client.py`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.1/pluralkit/v2/errors.py` & `pluralkit-1.1.2/pluralkit/v2/errors.py`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.1/pluralkit/v2/models.py` & `pluralkit-1.1.2/pluralkit/v2/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,31 +38,42 @@
     OFF = "off"
     FRONT = "front"
     LATCH = "latch"
     MEMBER = "member"
 
     def json(self): return self.value
 
+def _to_json(value):
+    """Robust method to deep convert Model objects
+    """
+    if hasattr(value, "json"):
+        return value.json()
+    
+    if isinstance(value, (list, set, tuple)):
+        return [_to_json(v) for v in value]
+    
+    if isinstance(value, (dict,)):
+        return {k: _to_json(v) for k, v in value.items()}
+    
+    return value
+
 # Base class for all models
 
 class Model:
     """Base class for all models.
     """
 
     def json(self):
         """Return a JSON object representing this model.
         """
         model = {}
         for k, v in self.__dict__.items():
-            if not k.startswith("_"):
-                if hasattr(v, "json"):
-                    # recurse
-                    model[k] = v.json()
-                elif v is not None:
-                    model[k] = v
+            if k.startswith("_"): continue
+            if v is None: continue
+            model[k] = _to_json(v)
 
         return model
 
     def __init__(self, json, ignore_keys=None):
         """Simple way to convert from API JSON object to the superclass
         """
         if ignore_keys is None: ignore_keys = ()
```

### Comparing `pluralkit-1.1.1/pluralkit.egg-info/PKG-INFO` & `pluralkit-1.1.2/pluralkit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pluralkit
-Version: 1.1.1
+Version: 1.1.2
 Summary: Python wrapper for PluralKit's API.
 Home-page: https://github.com/almonds0166/pluralkit.py
 Author: Madison Landry, Alyx Warner
 Author-email: pkpy@mit.edu
 License: MIT
 Project-URL: Documentation, https://pluralkit.readthedocs.io/en/latest/
 Project-URL: Issue tracker, https://github.com/almonds0166/pluralkit.py/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pluralkit Version: 1.1.1 Summary: Python wrapper
+Metadata-Version: 2.1 Name: pluralkit Version: 1.1.2 Summary: Python wrapper
 for PluralKit's API. Home-page: https://github.com/almonds0166/pluralkit.py
 Author: Madison Landry, Alyx Warner Author-email: pkpy@mit.edu License: MIT
 Project-URL: Documentation, https://pluralkit.readthedocs.io/en/latest/
 Project-URL: Issue tracker, https://github.com/almonds0166/pluralkit.py/issues
 Description: # pluralkit.py [![PyPi Version](https://img.shields.io/pypi/v/
 pluralkit.svg)](https://pypi.python.org/pypi/pluralkit/) [![Documentation
 Status](https://readthedocs.org/projects/pluralkit/badge/?version=latest)]
```

### Comparing `pluralkit-1.1.1/pluralkit.egg-info/SOURCES.txt` & `pluralkit-1.1.2/pluralkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.1/setup.py` & `pluralkit-1.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.1/tests/test_member.py` & `pluralkit-1.1.2/tests/test_member.py`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.1/tests/test_system.py` & `pluralkit-1.1.2/tests/test_system.py`

 * *Files identical despite different names*

