# Comparing `tmp/xsget-0.1.7.tar.gz` & `tmp/xsget-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xsget-0.1.7.tar", last modified: Sun Feb 26 05:25:54 2023, max compression
+gzip compressed data, was "xsget-0.1.8.tar", last modified: Sun Apr 16 04:35:30 2023, max compression
```

## Comparing `xsget-0.1.7.tar` & `xsget-0.1.8.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      104 2023-02-10 13:27:30.849891 xsget-0.1.7/.coveragerc
--rw-r--r--   0        0        0     1904 2023-01-15 07:21:25.732720 xsget-0.1.7/.gitignore
--rw-r--r--   0        0        0     2607 2023-02-22 13:52:10.966997 xsget-0.1.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0       36 2023-02-25 14:16:23.136929 xsget-0.1.7/.python-version
--rw-r--r--   0        0        0     3535 2023-02-26 05:24:50.080897 xsget-0.1.7/CHANGELOG.md
--rw-r--r--   0        0        0     1151 2023-02-24 15:10:29.264883 xsget-0.1.7/CONTRIBUTING.md
--rw-r--r--   0        0        0    31956 2022-09-03 12:07:10.610397 xsget-0.1.7/LICENSE.md
--rw-r--r--   0        0        0     5056 2023-02-23 13:36:02.949862 xsget-0.1.7/README.md
--rw-r--r--   0        0        0      782 2022-04-27 22:12:30.758460 xsget-0.1.7/docs/Makefile
--rw-r--r--   0        0        0      804 2022-04-27 22:12:30.758460 xsget-0.1.7/docs/make.bat
-lrwxr-xr-x   0        0        0        0 2022-04-27 22:12:30.758460 xsget-0.1.7/docs/source/CHANGELOG.md -> ../../CHANGELOG.md
-lrwxr-xr-x   0        0        0        0 2022-04-27 22:12:30.758460 xsget-0.1.7/docs/source/CONTRIBUTING.md -> ../../CONTRIBUTING.md
-lrwxr-xr-x   0        0        0        0 2022-04-27 22:12:30.758460 xsget-0.1.7/docs/source/LICENSE.md -> ../../LICENSE.md
-lrwxr-xr-x   0        0        0        0 2022-04-27 22:12:30.758460 xsget-0.1.7/docs/source/README.md -> ../../README.md
--rw-r--r--   0        0        0    63990 2022-04-27 22:12:30.758460 xsget-0.1.7/docs/source/_static/logo.png
--rw-r--r--   0        0        0     2473 2022-09-28 15:08:05.153213 xsget-0.1.7/docs/source/conf.py
--rw-r--r--   0        0        0      202 2022-05-06 12:58:04.555971 xsget-0.1.7/docs/source/index.rst
--rw-r--r--   0        0        0      533 2022-04-27 22:12:30.758460 xsget-0.1.7/docs/source/xsget.rst
--rw-r--r--   0        0        0      471 2022-07-16 05:50:26.995584 xsget-0.1.7/docs/source/xstxt.md
--rw-r--r--   0        0        0      426 2023-02-21 14:57:25.314938 xsget-0.1.7/locales/en/LC_MESSAGES/xstxt.mo
--rw-r--r--   0        0        0      616 2023-02-17 13:42:32.541336 xsget-0.1.7/locales/en/LC_MESSAGES/xstxt.po
--rw-r--r--   0        0        0      571 2023-02-21 14:58:21.773141 xsget-0.1.7/locales/xstxt.pot
--rw-r--r--   0        0        0      427 2023-02-21 14:57:25.322937 xsget-0.1.7/locales/zh/LC_MESSAGES/xstxt.mo
--rw-r--r--   0        0        0      617 2023-02-17 13:42:32.545336 xsget-0.1.7/locales/zh/LC_MESSAGES/xstxt.po
--rw-r--r--   0        0        0     2865 2023-02-25 14:44:39.282514 xsget-0.1.7/pyproject.toml
--rw-r--r--   0        0        0        0 2022-09-15 14:02:04.220660 xsget-0.1.7/tests/__init__.py
--rw-r--r--   0        0        0      257 2022-06-04 02:46:26.216686 xsget-0.1.7/tests/conftest.py
--rw-r--r--   0        0        0     4457 2023-02-09 13:19:09.435934 xsget-0.1.7/tests/test_xsget.py
--rw-r--r--   0        0        0     8839 2023-02-02 14:36:35.484168 xsget-0.1.7/tests/test_xstxt.py
--rw-r--r--   0        0        0     4295 2023-02-26 05:25:03.809086 xsget-0.1.7/xsget/__init__.py
--rw-r--r--   0        0        0      355 2022-07-01 22:44:04.742450 xsget-0.1.7/xsget/book.py
--rw-r--r--   0        0        0      920 2022-12-27 10:58:29.556852 xsget-0.1.7/xsget/chapter.py
--rw-r--r--   0        0        0    13868 2023-02-10 13:27:52.461329 xsget-0.1.7/xsget/xsget.py
--rw-r--r--   0        0        0     1526 2022-12-27 10:58:29.556852 xsget-0.1.7/xsget/xsget.toml
--rw-r--r--   0        0        0    17131 2023-02-21 15:09:55.740261 xsget-0.1.7/xsget/xstxt.py
--rw-r--r--   0        0        0     3408 2023-02-01 09:54:23.862432 xsget-0.1.7/xsget/xstxt.toml
--rw-r--r--   0        0        0     7025 1970-01-01 00:00:00.000000 xsget-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      104 2023-03-18 10:31:29.623190 xsget-0.1.8/.coveragerc
+-rw-r--r--   0        0        0     1919 2023-03-24 14:01:29.280123 xsget-0.1.8/.gitignore
+-rw-r--r--   0        0        0     2607 2023-04-15 13:24:35.236799 xsget-0.1.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       36 2023-04-05 23:46:00.757628 xsget-0.1.8/.python-version
+-rw-r--r--   0        0        0     4120 2023-04-16 04:34:20.701509 xsget-0.1.8/CHANGELOG.md
+-rw-r--r--   0        0        0     1590 2023-04-14 14:54:29.535457 xsget-0.1.8/CONTRIBUTING.md
+-rw-r--r--   0        0        0    31956 2022-09-03 12:07:10.610397 xsget-0.1.8/LICENSE.md
+-rw-r--r--   0        0        0     5145 2023-03-20 15:47:55.552686 xsget-0.1.8/README.md
+-rw-r--r--   0        0        0      782 2022-04-27 22:12:30.758460 xsget-0.1.8/docs/Makefile
+-rw-r--r--   0        0        0      804 2022-04-27 22:12:30.758460 xsget-0.1.8/docs/make.bat
+lrwxr-xr-x   0        0        0        0 2022-04-27 22:12:30.758460 xsget-0.1.8/docs/source/CHANGELOG.md -> ../../CHANGELOG.md
+lrwxr-xr-x   0        0        0        0 2022-04-27 22:12:30.758460 xsget-0.1.8/docs/source/CONTRIBUTING.md -> ../../CONTRIBUTING.md
+lrwxr-xr-x   0        0        0        0 2022-04-27 22:12:30.758460 xsget-0.1.8/docs/source/LICENSE.md -> ../../LICENSE.md
+lrwxr-xr-x   0        0        0        0 2022-04-27 22:12:30.758460 xsget-0.1.8/docs/source/README.md -> ../../README.md
+-rw-r--r--   0        0        0    63990 2022-04-27 22:12:30.758460 xsget-0.1.8/docs/source/_static/logo.png
+-rw-r--r--   0        0        0     2473 2022-09-28 15:08:05.153213 xsget-0.1.8/docs/source/conf.py
+-rw-r--r--   0        0        0      202 2022-05-06 12:58:04.555971 xsget-0.1.8/docs/source/index.rst
+-rw-r--r--   0        0        0      533 2022-04-27 22:12:30.758460 xsget-0.1.8/docs/source/xsget.rst
+-rw-r--r--   0        0        0      471 2022-07-16 05:50:26.995584 xsget-0.1.8/docs/source/xstxt.md
+-rw-r--r--   0        0        0      426 2023-03-24 23:09:21.188668 xsget-0.1.8/locales/en/LC_MESSAGES/xstxt.mo
+-rw-r--r--   0        0        0      616 2023-03-06 13:28:02.776464 xsget-0.1.8/locales/en/LC_MESSAGES/xstxt.po
+-rw-r--r--   0        0        0      571 2023-03-25 09:30:21.493991 xsget-0.1.8/locales/xstxt.pot
+-rw-r--r--   0        0        0      427 2023-03-24 23:09:21.192668 xsget-0.1.8/locales/zh/LC_MESSAGES/xstxt.mo
+-rw-r--r--   0        0        0      617 2023-03-06 13:28:02.776464 xsget-0.1.8/locales/zh/LC_MESSAGES/xstxt.po
+-rw-r--r--   0        0        0     2998 2023-04-08 06:52:10.846647 xsget-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-09-15 14:02:04.220660 xsget-0.1.8/tests/__init__.py
+-rw-r--r--   0        0        0      257 2022-06-04 02:46:26.216686 xsget-0.1.8/tests/conftest.py
+-rw-r--r--   0        0        0     4863 2023-04-08 07:01:14.579946 xsget-0.1.8/tests/test_xsget.py
+-rw-r--r--   0        0        0     8758 2023-03-21 13:38:27.613019 xsget-0.1.8/tests/test_xstxt.py
+-rw-r--r--   0        0        0     4295 2023-04-16 04:34:33.621575 xsget-0.1.8/xsget/__init__.py
+-rw-r--r--   0        0        0      355 2022-07-01 22:44:04.742450 xsget-0.1.8/xsget/book.py
+-rw-r--r--   0        0        0      920 2023-02-28 09:58:00.269999 xsget-0.1.8/xsget/chapter.py
+-rw-r--r--   0        0        0    13457 2023-04-14 14:01:38.733820 xsget-0.1.8/xsget/xsget.py
+-rw-r--r--   0        0        0     1526 2022-12-27 10:58:29.556852 xsget-0.1.8/xsget/xsget.toml
+-rw-r--r--   0        0        0    17162 2023-04-06 23:39:41.532743 xsget-0.1.8/xsget/xstxt.py
+-rw-r--r--   0        0        0     3408 2023-02-01 09:54:23.862432 xsget-0.1.8/xsget/xstxt.toml
+-rw-r--r--   0        0        0     7328 1970-01-01 00:00:00.000000 xsget-0.1.8/PKG-INFO
```

### Comparing `xsget-0.1.7/.gitignore` & `xsget-0.1.8/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -131,11 +131,13 @@
 
 # Pyre type checker
 .pyre/
 
 # Misc.
 *.html
 *.sqlite3
+*.prof
+*.lprof
 /xsget.toml
 /xstxt.toml
 book.txt
 TODO
```

### Comparing `xsget-0.1.7/.pre-commit-config.yaml` & `xsget-0.1.8/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -7,26 +7,26 @@
       - id: trailing-whitespace
       - id: end-of-file-fixer
         exclude: "locales/.*$"
       - id: check-yaml
       - id: check-toml
 
   - repo: https://github.com/abravalheri/validate-pyproject
-    rev: v0.12.1
+    rev: v0.12.2
     hooks:
       - id: validate-pyproject
         name: validate pyproject
 
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.2
+    rev: v2.2.4
     hooks:
       - id: codespell
 
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: v3.0.0-alpha.4
+    rev: v3.0.0-alpha.6
     hooks:
       - id: prettier
 
   - repo: https://github.com/pycqa/isort
     rev: 5.11.5
     hooks:
       - id: isort
@@ -34,15 +34,15 @@
           - isort[pyproject]
         args:
           - --profile=black
           - --line-length=79
           - --py=311
 
   - repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
       - id: black
         language_version: python3.11
         args:
           - --line-length=79
           - --target-version=py311
 
@@ -50,15 +50,15 @@
     rev: 1.13.0
     hooks:
       - id: blacken-docs
         additional_dependencies:
           - black==22.8.0
 
   - repo: https://github.com/PyCQA/autoflake
-    rev: v2.0.1
+    rev: v2.0.2
     hooks:
       - id: autoflake
         args:
           - --in-place
           - --remove-unused-variables
           - --remove-all-unused-imports
         language: python
@@ -95,13 +95,13 @@
           - xsget
           - tests
           - --py-version=3.7
           - --disable=R0801,W0612
           - --unsafe-load-any-extension=y
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.0.0
+    rev: v1.2.0
     hooks:
       - id: mypy
         exclude: docs/
         additional_dependencies:
           - types-aiofiles
```

### Comparing `xsget-0.1.7/CHANGELOG.md` & `xsget-0.1.8/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -3,16 +3,43 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [0-based versioning](https://0ver.org/).
 
 ## [Unreleased]
 
+## v0.1.8 - 2023-04-16
+
+### Added
+
+- Add multiprocessor support for `pytest`
+
+### Changed
+
+- Deprecate and remove `is_relative_url` and `relative_to_absolute_url`
+  function in favour of lxml's `make_links_absolute` function
+
+### Fixed
+
+- Set `index.html` as default filename for index page if missing
+- Rename `-w` to `-wf` option to prevent duplicate with `--width`
+- Update translations
+
+### Changed
+
+- Reduce number of browser session to prevent locking
+- Remove explicit config for async in tests
+- Refactor async tests
+
 ## v0.1.7 - 2023-02-26
 
+### Changed
+
+- Show longer chapter title in debugging log
+
 ### Added
 
 - Add `-oi` or `--output-individual-file` to create a txt file for its
   corresponding html file
 
 ### Changed
```

### Comparing `xsget-0.1.7/LICENSE.md` & `xsget-0.1.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `xsget-0.1.7/README.md` & `xsget-0.1.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -17,16 +17,18 @@
 python3 -m pip install -e git+https://github.com/kianmeng/xsget.git
 playwright install
 ```
 
 ## xsget
 
 ```console
-$ xsget -h
+xsget -h
+```
 
+```console
 usage: xsget [-l CSS_PATH] [-p URL_PARAM] [-g [FILENAME] | -c [FILENAME]] [-r]
              [-t] [-b] [-bs SESSION] [-bd DELAY] [-d] [-h] [-V]
              URL
 
 xsget is a console app that crawl and download online novel.
   website: https://github.com/kianmeng/xsget
   issues: https://github.com/kianmeng/xsget/issues
@@ -64,22 +66,23 @@
   xsget http://localhost
   xsget http://localhost/page[1-100].html
 ```
 
 ## xstxt
 
 ```console
-$ xstxt -h
-
+xstxt -h
+```
 
+```console
 usage: xstxt [-pt CSS_PATH] [-pb CSS_PATH] [-la LANGUAGE] [-ps SEPARATOR]
              [-rh REGEX REGEX] [-rt REGEX REGEX] [-bt TITLE] [-ba AUTHOR]
              [-ic INDENT_CHARS] [-fw] [-oi] [-i GLOB_PATTERN]
              [-e GLOB_PATTERN] [-l TOTAL_FILES] [-w WIDTH] [-o FILENAME]
-             [-g [FILENAME] | -c [FILENAME]] [-d] [-h] [-V]
+             [-g [FILENAME] | -c [FILENAME]] [-wf] [-d] [-h] [-V]
 
 xstxt is a cli app that extract content from HTML to text file.
   website: https://github.com/kianmeng/xsget
   issues: https://github.com/kianmeng/xsget/issues
 
 optional arguments:
   -pt CSS_PATH, --title-css-path CSS_PATH
@@ -114,14 +117,16 @@
         set the line width for wrapping (default: 0, 0 to disable)
   -o FILENAME, --output FILENAME
         set output txt file name (default: 'book.txt')
   -g [FILENAME], --generate-config-file [FILENAME]
         generate config file from options (default: 'xstxt.toml')
   -c [FILENAME], --config-file [FILENAME]
         load config from file (default: 'xstxt.toml')
+  -wf, --watch-files
+        enable watch on file changes
   -d, --debug
         show debugging log and stacktrace
   -h, --help
         show this help message and exit
   -V, --version
         show program's version number and exit
```

### Comparing `xsget-0.1.7/docs/Makefile` & `xsget-0.1.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `xsget-0.1.7/docs/make.bat` & `xsget-0.1.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `xsget-0.1.7/docs/source/_static/logo.png` & `xsget-0.1.8/docs/source/_static/logo.png`

 * *Files identical despite different names*

### Comparing `xsget-0.1.7/docs/source/conf.py` & `xsget-0.1.8/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `xsget-0.1.7/docs/source/xsget.rst` & `xsget-0.1.8/docs/source/xsget.rst`

 * *Files identical despite different names*

### Comparing `xsget-0.1.7/locales/en/LC_MESSAGES/xstxt.po` & `xsget-0.1.8/locales/en/LC_MESSAGES/xstxt.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR ORGANIZATION
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
-"POT-Creation-Date: 2023-02-17 21:42+0800\n"
+"POT-Creation-Date: 2023-03-06 04:01+0800\n"
 "PO-Revision-Date: 2023-01-12 21:43+0800\n"
 "Last-Translator: \n"
 "Language-Team: \n"
 "Language: en\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "Generated-By: pygettext.py 1.5\n"
 "X-Generator: Poedit 3.1.1\n"
 
-#: xsget/xstxt.py:324
+#: xsget/xstxt.py:310
 msgid "title:"
 msgstr "Title:"
 
-#: xsget/xstxt.py:326
+#: xsget/xstxt.py:312
 msgid "author:"
 msgstr "Author:"
```

### Comparing `xsget-0.1.7/locales/xstxt.pot` & `xsget-0.1.8/locales/xstxt.pot`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR ORGANIZATION
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"POT-Creation-Date: 2023-02-17 21:42+0800\n"
+"POT-Creation-Date: 2023-03-06 04:01+0800\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: pygettext.py 1.5\n"
 
 
-#: xsget/xstxt.py:324
+#: xsget/xstxt.py:310
 msgid "title:"
 msgstr ""
 
-#: xsget/xstxt.py:326
+#: xsget/xstxt.py:312
 msgid "author:"
 msgstr ""
```

### Comparing `xsget-0.1.7/locales/zh/LC_MESSAGES/xstxt.po` & `xsget-0.1.8/locales/zh/LC_MESSAGES/xstxt.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR ORGANIZATION
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
-"POT-Creation-Date: 2023-02-17 21:42+0800\n"
+"POT-Creation-Date: 2023-03-06 04:01+0800\n"
 "PO-Revision-Date: 2023-01-12 21:38+0800\n"
 "Last-Translator: \n"
 "Language-Team: \n"
 "Language: zh_CN\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "Generated-By: pygettext.py 1.5\n"
 "X-Generator: Poedit 3.1.1\n"
 
-#: xsget/xstxt.py:324
+#: xsget/xstxt.py:310
 msgid "title:"
 msgstr "书名："
 
-#: xsget/xstxt.py:326
+#: xsget/xstxt.py:312
 msgid "author:"
 msgstr "作者："
```

### Comparing `xsget-0.1.7/pyproject.toml` & `xsget-0.1.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
   "bs4",
   "lxml",
   "natsort",
   "playwright",
   "regex",
   "tomlkit",
   "user_agent",
+  "cssselect",
 ]
 dynamic = [
   "description",
   "version",
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -41,29 +42,33 @@
 [project.optional-dependencies]
 dev = [
   "black",
   "isort",
   "pre-commit",
   "tox<4",
   "tox-pyenv",
+  "line-profiler",
 ]
 doc = [
   "myst_parser",
   "sphinx",
   "sphinx_autobuild",
   "sphinx_copybutton",
   "sphinx-autodoc-typehints",
 ]
 test = [
+  "aioresponses",
   "playwright",
   "pytest",
   "pytest-asyncio",
   "pytest-console-scripts",
   "pytest-cov",
+  "pytest-xdist",
   "pytest-mock",
+  "pytest-playwright",
   "types-aiofiles",
 ]
 
 [project.urls]
 Issues = "https://github.com/kianmeng/xsget/issues"
 Source = "https://github.com/kianmeng/xsget"
 
@@ -82,21 +87,21 @@
 [tox]
 isolated_build = True
 envlist = py3{7,8,9,10,11}
 
 [testenv]
 description = testing against {basepython}
 deps = .[test]
-commands = pytest --hide-run-results
+commands = pytest --numprocesses auto --hide-run-results
 
 [testenv:cover]
 description = generate code coverage report in html
 basepython = python3.11
 deps = .[test]
-commands = pytest --cov=xsget --cov-report term-missing --cov-report html {toxinidir}/tests
+commands = pytest --numprocesses auto --cov=xsget --cov-report term-missing --cov-report html {toxinidir}/tests
 
 [testenv:doc]
 description = generate sphinx documentation in html
 basepython = python3.11
 deps = .[doc]
 commands = sphinx-build {toxinidir}/docs/source/ {toxinidir}/docs/_build/html
```

### Comparing `xsget-0.1.7/tests/test_xsget.py` & `xsget-0.1.8/tests/test_xsget.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 # pylint: disable=missing-module-docstring,missing-function-docstring
 
 import argparse
+from pathlib import Path
 from shlex import split as argv
 
+import aiohttp
+from aioresponses import aioresponses
+
 from xsget import __version__
 from xsget.xsget import (
     extract_urls,
+    fetch_url_by_aiohttp,
     http_headers,
-    is_relative_url,
     url_to_filename,
 )
 
 DEFAULT_URL = "http://localhost"
 
 
 def test_repo_urls_in_help_message(script_runner):
@@ -29,37 +33,35 @@
 
 def test_invalid_url(script_runner):
     ret = script_runner.run(*argv("xsget example.com"))
     assert "error: invalid url: example.com" in ret.stdout
 
 
 def test_range_in_url(script_runner):
-    ret = script_runner.run(*argv("xsget -d -t https://localhost/[1-2].html"))
+    ret = script_runner.run(*argv(f"xsget -d -t {DEFAULT_URL}/[1-2].html"))
     logs = [
-        "INFO: xsget.xsget: Found url: https://localhost/1.html",
-        "INFO: xsget.xsget: Found url: https://localhost/2.html",
+        f"INFO: xsget.xsget: Found url: {DEFAULT_URL}/1.html",
+        f"INFO: xsget.xsget: Found url: {DEFAULT_URL}/2.html",
     ]
     for log in logs:
         assert log in ret.stdout
 
 
 def test_leading_range_in_url(script_runner):
-    ret = script_runner.run(
-        *argv("xsget -d -t https://localhost/a0[1-2].html")
-    )
+    ret = script_runner.run(*argv(f"xsget -d -t {DEFAULT_URL}/a0[1-2].html"))
     logs = [
-        "INFO: xsget.xsget: Found url: https://localhost/a01.html",
-        "INFO: xsget.xsget: Found url: https://localhost/a02.html",
+        f"INFO: xsget.xsget: Found url: {DEFAULT_URL}/a01.html",
+        f"INFO: xsget.xsget: Found url: {DEFAULT_URL}/a02.html",
     ]
     for log in logs:
         assert log in ret.stdout
 
 
 def test_raise_exception_for_invalid_range_in_url(script_runner):
-    ret = script_runner.run(*argv("xsget -d -t https://localhost/[2-1].html"))
+    ret = script_runner.run(*argv(f"xsget -d -t {DEFAULT_URL}/[2-1].html"))
     logs = [
         "ERROR: xsget.xsget: error: invalid url range, start: 2, end: 1",
         "Exception: invalid url range, start: 2, end: 1",
     ]
     for log in logs:
         assert log in ret.stdout
 
@@ -82,14 +84,16 @@
 def test_version(script_runner):
     ret = script_runner.run(*argv("xsget -V"))
     assert f"xsget {__version__}" in ret.stdout
 
 
 def test_url_to_filename():
     expected = [
+        ("http://a.com", "index.html"),
+        ("http://a.com/", "index.html"),
         ("http://a.com/123", "123.html"),
         ("http://a.com/123/456", "456.html"),
         ("http://a.com/123/456/789", "789.html"),
         ("http://a.com/123.html", "123.html"),
     ]
     for url, filename in expected:
         assert url_to_filename(url) == filename
@@ -98,24 +102,14 @@
         ("http://a.com/123?id=aaa", "id", "aaa.html"),
         ("http://a.com/456.php?tid=abc", "tid", "abc.html"),
     ]
     for url, url_param, filename in expected:
         assert url_to_filename(url, url_param) == filename
 
 
-def test_is_relative_url():
-    expected = [
-        ("http://a.com/123", False),
-        ("//a.com/123/456", True),
-        ("/123/456.html", True),
-    ]
-    for url, result in expected:
-        assert is_relative_url(url) == result
-
-
 def test_extract_urls():
     html = """
         <html>
         <body>
         <div class="toc">
             <a href="http://a.com/123"/>a</a>
             <a href="http://a.com/123/789.html"/>b</a>
@@ -149,7 +143,22 @@
         )
         assert extract_urls(html, config) == expected_urls
 
 
 def test_user_agent():
     user_agent = http_headers()["User-Agent"]
     assert "Mozilla/5.0" in user_agent
+
+
+async def test_fetch_url_by_aiohttp(tmpdir):
+    session = aiohttp.ClientSession()
+
+    with aioresponses() as mocked:
+        config = argparse.Namespace(url_param_as_filename="")
+        mocked.get(DEFAULT_URL, status=200, body="test")
+
+        resp = await fetch_url_by_aiohttp(session, DEFAULT_URL, config)
+        assert resp.status == 200
+        mocked.assert_called_once_with(DEFAULT_URL)
+
+        with open(Path(tmpdir, "index.html"), encoding="utf8") as file:
+            assert file.read() == "test"
```

### Comparing `xsget-0.1.7/tests/test_xstxt.py` & `xsget-0.1.8/tests/test_xstxt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 # pylint: disable=missing-module-docstring,missing-function-docstring
 import argparse
 import re
 from pathlib import Path
 
-import pytest
-
 from xsget import __version__
 from xsget.book import Book
 from xsget.chapter import Chapter
 from xsget.xstxt import (
     extract_chapter,
     gen_single_txt,
     get_html_files,
@@ -91,15 +89,14 @@
 
 def test_get_no_html_files(caplog):
     path = "foobar/*.html"
     assert get_html_files([path], 0, []) == []
     assert f"No input files found in: {path}" in caplog.text
 
 
-@pytest.mark.asyncio()
 async def test_extract_chapter():
     html = """
         <html>
         <head><title>My Title</title></head>
         <body>
             <div id="content">My Content</div>
         </body>
@@ -117,19 +114,18 @@
     chapter.filename = "123.html"
     assert chapter.filename == "123.html"
     assert chapter.title == "My Title"
     assert chapter.content == "My Content"
     assert str(chapter) == "My Title\n\nMy Content"
     assert (
         repr(chapter)
-        == "Chapter(filename='123.html', title='My Ti', content='My Co')"
+        == "Chapter(filename='123.html', title='My Title', content='My Co')"
     )
 
 
-@pytest.mark.asyncio()
 async def test_extract_chapter_with_html_replace():
     html = """
         <html>
         <head><title>My Title</title></head>
         <body>
             <div id="content">
             &nbsp;&nbsp;&nbsp;&nbsp;Paragraph1
@@ -166,15 +162,14 @@
             "22",
             "3333Paragraph3",
         ]
     )
     assert re.match(match_regex, str(chapter))
 
 
-@pytest.mark.asyncio()
 async def test_extract_chapter_without_css_path():
     html = """
         <html>
         <head><title>My Title</title></head>
         <body>
             <div id="content">My Content</div>
         </body>
```

### Comparing `xsget-0.1.7/xsget/__init__.py` & `xsget-0.1.8/xsget/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from datetime import datetime as dt
 from importlib.resources import read_text
 from pathlib import Path
 from typing import Dict
 
 import tomlkit
 
-__version__ = "0.1.7"
+__version__ = "0.1.8"
 
 _logger = logging.getLogger(__name__)
 
 
 class ConfigFileCorruptedError(Exception):
     """Config file corrupted after reading."""
```

### Comparing `xsget-0.1.7/xsget/chapter.py` & `xsget-0.1.8/xsget/chapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     filename: str = field(default="")
 
     def __repr__(self):
         """For debugging output."""
         return "{}(filename='{}', title='{}', content='{}')".format(
             self.__class__.__name__,
             self.filename,
-            self.title[:5],
+            self.title[:8],
             self.content[:5].strip(),
         )
 
     def __str__(self):
         """For string representation."""
         if self.title and self.content:
             return "{}\n\n{}".format(self.title, self.content)
```

### Comparing `xsget-0.1.7/xsget/xsget.py` & `xsget-0.1.8/xsget/xsget.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,30 +17,32 @@
 
 import argparse
 import asyncio
 import logging
 import re
 import sys
 from pathlib import Path
-from typing import Any, Dict, List, Sequence
-from urllib.parse import parse_qs, unquote, urljoin, urlparse
+from typing import Any, Dict, List, Optional, Sequence
+from urllib.parse import parse_qs, unquote, urlparse
 
 import aiohttp
-from bs4 import BeautifulSoup, UnicodeDammit
+import lxml.html as lxml_html
+from bs4 import UnicodeDammit
 from playwright.async_api import async_playwright
 from user_agent import generate_user_agent
 
 from xsget import __version__, load_or_create_config, setup_logging
 
 CONFIG_FILE = "xsget.toml"
 
 __usages__ = """
 examples:
   xsget http://localhost
   xsget http://localhost/page[1-100].html
+  xsget -g -l "a" -p "id" http://localhost
 
 """
 
 _logger = logging.getLogger(__name__)
 
 
 def url_to_filename(url: str, url_param_as_filename: str = ""):
@@ -51,73 +53,42 @@
         url_param_as_filename (str): Extract the set URL param value as
         filename. Default to False.
 
     Returns:
         str: The generated filename.
     """
     parsed_url = urlparse(unquote(url))
-
     if url_param_as_filename != "":
         query = parse_qs(parsed_url.query)
         if url_param_as_filename in query:
             return "".join(query[url_param_as_filename]) + ".html"
 
-    return (
+    filename = (
         parsed_url.path.rstrip("/").split("/")[-1].replace(".html", "")
         + ".html"
     )
+    return "index.html" if filename == ".html" else filename
 
 
-def is_relative_url(url: str) -> bool:
-    """Check if an URL is a relative URL or URL without schema.
-
-    Args:
-        url(str): An URL for verification.
-
-    Returns:
-        bool: Whether the URL is relative or without schema.
-    """
-    uparse = urlparse(url)
-    return uparse.netloc == "" or uparse.scheme == ""
-
-
-def relative_to_absolute_url(base_url: str, path: str) -> str:
-    """Convert relative URL to absolute URL.
-
-    Args:
-        base_url(str): The base URL.
-        path(str): The path of an URL.
-
-    Returns:
-        str: The full absolute URL.
-    """
-    return urljoin(base_url, path)
-
-
-def extract_urls(
-    decoded_html: BeautifulSoup, config: argparse.Namespace
-) -> List[str]:
+def extract_urls(decoded_html: str, config: argparse.Namespace) -> List[str]:
     """Extract URLs from HTML base on the CSS Path.
 
     Args:
-        decoded_html (BeautifulSoup): The decoded HTML string
+        decoded_html (str): The decoded HTML string
         config (argparse.Namespace): Config from command line
 
     Returns:
         List[str]: A list of URL for downloading
     """
-    html = BeautifulSoup(decoded_html, features="lxml")
-    urls = []
-
-    for atag in html.select(config.link_css_path):
-        page_url = atag.get("href")
-        if page_url and is_relative_url(page_url):
-            page_url = relative_to_absolute_url(config.url, page_url)
+    doc = lxml_html.fromstring(decoded_html)
+    doc.make_links_absolute(config.url, resolve_base_href=True)
 
-        urls.append(page_url)
+    urls = []
+    for atag in doc.cssselect(config.link_css_path):
+        urls.append(atag.get("href"))
 
     return urls
 
 
 async def fetch_url_by_aiohttp(
     session: Any, url: str, config: argparse.Namespace
 ) -> None:
@@ -141,14 +112,16 @@
             )
 
             with open(filename, "w", encoding=resp.charset) as file:
                 file.write(content)
                 _logger.info("Fetching %s", unquote(str(resp.url)))
                 _logger.info("Saving %s", filename)
 
+            return resp
+
     # Log as error instead of raising exception as we want to continue with
     # other downloads.
     except aiohttp.ClientResponseError as error:
         _logger.error("error: %s", error)
 
     except aiohttp.client_exceptions.InvalidURL as error:
         raise Exception(f"invalid url: {error}") from error
@@ -229,16 +202,25 @@
 
     Returns:
         tuple: Custom HTTP headers, but only User-Agent for now
     """
     return {"User-Agent": generate_user_agent()}
 
 
-def build_parser(args=None) -> argparse.ArgumentParser:
-    """Build the CLI parser."""
+def build_parser(
+    args: Optional[Sequence[str]] = None,
+) -> argparse.ArgumentParser:
+    """Build the CLI parser.
+
+    Args:
+        args (list|None): A list of flags from command line.
+
+    Returns:
+        argparse.ArgumentParser: Argument parser.
+    """
     args = args or []
 
     parser = argparse.ArgumentParser(
         add_help=False,
         description=_doc(),
         epilog=__usages__,
         formatter_class=lambda prog: argparse.RawTextHelpFormatter(
@@ -332,15 +314,15 @@
         dest="browser",
         help="crawl by actual browser (default: '%(default)s')",
     )
 
     parser.add_argument(
         "-bs",
         "--browser-session",
-        default=5,
+        default=2,
         dest="browser_session",
         help="set the number of browser session (default: %(default)s)",
         type=int,
         metavar="SESSION",
     )
 
     parser.add_argument(
```

### Comparing `xsget-0.1.7/xsget/xsget.toml` & `xsget-0.1.8/xsget/xsget.toml`

 * *Files identical despite different names*

### Comparing `xsget-0.1.7/xsget/xstxt.py` & `xsget-0.1.8/xsget/xstxt.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,16 +34,16 @@
 
 from xsget import __version__, load_or_create_config, setup_logging
 from xsget.book import Book
 from xsget.chapter import Chapter
 
 __usages__ = """
 examples:
-  xstxt -i *.html
-  xstxt -oi -i *.html
+  xstxt --input *.html
+  xstxt --output-individual-file --input *.html
 
 """
 
 # Unicode integer in hexadecimal for these characters.
 FULLWIDTH_EXCLAMATION_MARK = 0xFF01
 EXCLAMATION_MARK = 0x21
 TILDE = 0x7E
```

### Comparing `xsget-0.1.7/xsget/xstxt.toml` & `xsget-0.1.8/xsget/xstxt.toml`

 * *Files identical despite different names*

### Comparing `xsget-0.1.7/PKG-INFO` & `xsget-0.1.8/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xsget
-Version: 0.1.7
+Version: 0.1.8
 Summary: Console tools to download online novel and convert to text file.
 Author-email: "Kian-Meng, Ang" <kianmeng@cpan.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
@@ -21,30 +21,35 @@
 Requires-Dist: bs4
 Requires-Dist: lxml
 Requires-Dist: natsort
 Requires-Dist: playwright
 Requires-Dist: regex
 Requires-Dist: tomlkit
 Requires-Dist: user_agent
+Requires-Dist: cssselect
 Requires-Dist: black ; extra == "dev"
 Requires-Dist: isort ; extra == "dev"
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: tox<4 ; extra == "dev"
 Requires-Dist: tox-pyenv ; extra == "dev"
+Requires-Dist: line-profiler ; extra == "dev"
 Requires-Dist: myst_parser ; extra == "doc"
 Requires-Dist: sphinx ; extra == "doc"
 Requires-Dist: sphinx_autobuild ; extra == "doc"
 Requires-Dist: sphinx_copybutton ; extra == "doc"
 Requires-Dist: sphinx-autodoc-typehints ; extra == "doc"
+Requires-Dist: aioresponses ; extra == "test"
 Requires-Dist: playwright ; extra == "test"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-asyncio ; extra == "test"
 Requires-Dist: pytest-console-scripts ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
+Requires-Dist: pytest-xdist ; extra == "test"
 Requires-Dist: pytest-mock ; extra == "test"
+Requires-Dist: pytest-playwright ; extra == "test"
 Requires-Dist: types-aiofiles ; extra == "test"
 Project-URL: Issues, https://github.com/kianmeng/xsget/issues
 Project-URL: Source, https://github.com/kianmeng/xsget
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: test
 
@@ -67,16 +72,18 @@
 python3 -m pip install -e git+https://github.com/kianmeng/xsget.git
 playwright install
 ```
 
 ## xsget
 
 ```console
-$ xsget -h
+xsget -h
+```
 
+```console
 usage: xsget [-l CSS_PATH] [-p URL_PARAM] [-g [FILENAME] | -c [FILENAME]] [-r]
              [-t] [-b] [-bs SESSION] [-bd DELAY] [-d] [-h] [-V]
              URL
 
 xsget is a console app that crawl and download online novel.
   website: https://github.com/kianmeng/xsget
   issues: https://github.com/kianmeng/xsget/issues
@@ -114,22 +121,23 @@
   xsget http://localhost
   xsget http://localhost/page[1-100].html
 ```
 
 ## xstxt
 
 ```console
-$ xstxt -h
-
+xstxt -h
+```
 
+```console
 usage: xstxt [-pt CSS_PATH] [-pb CSS_PATH] [-la LANGUAGE] [-ps SEPARATOR]
              [-rh REGEX REGEX] [-rt REGEX REGEX] [-bt TITLE] [-ba AUTHOR]
              [-ic INDENT_CHARS] [-fw] [-oi] [-i GLOB_PATTERN]
              [-e GLOB_PATTERN] [-l TOTAL_FILES] [-w WIDTH] [-o FILENAME]
-             [-g [FILENAME] | -c [FILENAME]] [-d] [-h] [-V]
+             [-g [FILENAME] | -c [FILENAME]] [-wf] [-d] [-h] [-V]
 
 xstxt is a cli app that extract content from HTML to text file.
   website: https://github.com/kianmeng/xsget
   issues: https://github.com/kianmeng/xsget/issues
 
 optional arguments:
   -pt CSS_PATH, --title-css-path CSS_PATH
@@ -164,14 +172,16 @@
         set the line width for wrapping (default: 0, 0 to disable)
   -o FILENAME, --output FILENAME
         set output txt file name (default: 'book.txt')
   -g [FILENAME], --generate-config-file [FILENAME]
         generate config file from options (default: 'xstxt.toml')
   -c [FILENAME], --config-file [FILENAME]
         load config from file (default: 'xstxt.toml')
+  -wf, --watch-files
+        enable watch on file changes
   -d, --debug
         show debugging log and stacktrace
   -h, --help
         show this help message and exit
   -V, --version
         show program's version number and exit
```

