# Comparing `tmp/texproject-0.8.6.tar.gz` & `tmp/texproject-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "texproject-0.8.6.tar", last modified: Sat Feb 25 12:55:24 2023, max compression
+gzip compressed data, was "texproject-0.8.7.tar", last modified: Sun Apr 16 20:48:28 2023, max compression
```

## Comparing `texproject-0.8.6.tar` & `texproject-0.8.7.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-02-25 12:55:24.881845 texproject-0.8.6/
--rw-r--r--   0 alexrutar   (501) staff       (20)     1067 2022-01-21 18:39:53.000000 texproject-0.8.6/LICENSE
--rw-r--r--   0 alexrutar   (501) staff       (20)      108 2022-02-27 13:35:18.000000 texproject-0.8.6/MANIFEST.in
--rw-r--r--   0 alexrutar   (501) staff       (20)     6471 2023-02-25 12:55:24.881999 texproject-0.8.6/PKG-INFO
--rw-r--r--   0 alexrutar   (501) staff       (20)     5994 2023-02-25 10:19:50.000000 texproject-0.8.6/README.md
--rw-r--r--   0 alexrutar   (501) staff       (20)      359 2022-11-06 14:30:17.000000 texproject-0.8.6/pyproject.toml
--rw-r--r--   0 alexrutar   (501) staff       (20)      935 2023-02-25 12:55:24.882982 texproject-0.8.6/setup.cfg
-drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-02-25 12:55:24.866367 texproject-0.8.6/src/
-drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-02-25 12:55:24.872574 texproject-0.8.6/src/texproject/
--rw-r--r--   0 alexrutar   (501) staff       (20)      214 2023-02-25 12:54:02.000000 texproject-0.8.6/src/texproject/__init__.py
--rw-r--r--   0 alexrutar   (501) staff       (20)       63 2021-12-14 22:57:13.000000 texproject-0.8.6/src/texproject/__main__.py
--rw-r--r--   0 alexrutar   (501) staff       (20)     3440 2023-01-08 08:55:35.000000 texproject-0.8.6/src/texproject/base.py
--rw-r--r--   0 alexrutar   (501) staff       (20)    17277 2023-02-25 10:25:15.000000 texproject-0.8.6/src/texproject/command.py
--rw-r--r--   0 alexrutar   (501) staff       (20)     5653 2022-12-20 21:15:22.000000 texproject-0.8.6/src/texproject/control.py
-drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-02-25 12:55:24.876269 texproject-0.8.6/src/texproject/defaults/
--rw-r--r--   0 alexrutar   (501) staff       (20)        0 2021-12-22 01:04:12.000000 texproject-0.8.6/src/texproject/defaults/__init__.py
--rw-r--r--   0 alexrutar   (501) staff       (20)     1186 2022-11-23 22:47:39.000000 texproject-0.8.6/src/texproject/defaults/config.toml
--rw-r--r--   0 alexrutar   (501) staff       (20)      115 2022-11-19 14:45:53.000000 texproject-0.8.6/src/texproject/defaults/template.toml
--rw-r--r--   0 alexrutar   (501) staff       (20)      299 2022-01-13 12:30:10.000000 texproject-0.8.6/src/texproject/error.py
--rw-r--r--   0 alexrutar   (501) staff       (20)    10385 2023-02-25 10:21:39.000000 texproject-0.8.6/src/texproject/filesystem.py
--rw-r--r--   0 alexrutar   (501) staff       (20)     5879 2023-02-25 10:15:50.000000 texproject-0.8.6/src/texproject/git.py
--rw-r--r--   0 alexrutar   (501) staff       (20)    10908 2022-11-24 00:01:51.000000 texproject-0.8.6/src/texproject/output.py
--rw-r--r--   0 alexrutar   (501) staff       (20)    12788 2023-01-08 08:55:35.000000 texproject-0.8.6/src/texproject/template.py
-drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-02-25 12:55:24.880883 texproject-0.8.6/src/texproject/templates/
--rw-r--r--   0 alexrutar   (501) staff       (20)        0 2022-01-05 23:14:40.000000 texproject-0.8.6/src/texproject/templates/__init__.py
--rw-r--r--   0 alexrutar   (501) staff       (20)       61 2021-01-19 13:47:15.000000 texproject-0.8.6/src/texproject/templates/arxiv_autotex.txt
--rw-r--r--   0 alexrutar   (501) staff       (20)      304 2021-12-16 13:57:44.000000 texproject-0.8.6/src/texproject/templates/base.tex
--rw-r--r--   0 alexrutar   (501) staff       (20)      308 2022-11-19 23:06:18.000000 texproject-0.8.6/src/texproject/templates/bibinfo.tex
--rw-r--r--   0 alexrutar   (501) staff       (20)       67 2020-07-09 06:18:10.000000 texproject-0.8.6/src/texproject/templates/bibliography.tex
--rw-r--r--   0 alexrutar   (501) staff       (20)      520 2023-02-25 10:09:01.000000 texproject-0.8.6/src/texproject/templates/build.yaml
--rw-r--r--   0 alexrutar   (501) staff       (20)      842 2022-11-23 22:38:53.000000 texproject-0.8.6/src/texproject/templates/classinfo.tex
--rw-r--r--   0 alexrutar   (501) staff       (20)       64 2021-12-21 16:46:46.000000 texproject-0.8.6/src/texproject/templates/gitignore
--rwxr-xr-x   0 alexrutar   (501) staff       (20)      559 2022-03-23 18:03:46.000000 texproject-0.8.6/src/texproject/templates/pre-commit
--rw-r--r--   0 alexrutar   (501) staff       (20)       17 2020-07-08 17:23:05.000000 texproject-0.8.6/src/texproject/templates/project_macro_file.tex
--rw-r--r--   0 alexrutar   (501) staff       (20)     4292 2023-02-25 10:10:38.000000 texproject-0.8.6/src/texproject/term.py
--rw-r--r--   0 alexrutar   (501) staff       (20)     4992 2022-11-23 23:46:55.000000 texproject-0.8.6/src/texproject/utils.py
-drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-02-25 12:55:24.874791 texproject-0.8.6/src/texproject.egg-info/
--rw-r--r--   0 alexrutar   (501) staff       (20)     6471 2023-02-25 12:55:24.000000 texproject-0.8.6/src/texproject.egg-info/PKG-INFO
--rw-r--r--   0 alexrutar   (501) staff       (20)     1103 2023-02-25 12:55:24.000000 texproject-0.8.6/src/texproject.egg-info/SOURCES.txt
--rw-r--r--   0 alexrutar   (501) staff       (20)        1 2023-02-25 12:55:24.000000 texproject-0.8.6/src/texproject.egg-info/dependency_links.txt
--rw-r--r--   0 alexrutar   (501) staff       (20)       47 2023-02-25 12:55:24.000000 texproject-0.8.6/src/texproject.egg-info/entry_points.txt
--rw-r--r--   0 alexrutar   (501) staff       (20)       53 2023-02-25 12:55:24.000000 texproject-0.8.6/src/texproject.egg-info/requires.txt
--rw-r--r--   0 alexrutar   (501) staff       (20)       11 2023-02-25 12:55:24.000000 texproject-0.8.6/src/texproject.egg-info/top_level.txt
-drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-02-25 12:55:24.881399 texproject-0.8.6/test/
--rw-r--r--   0 alexrutar   (501) staff       (20)     7589 2023-02-25 10:26:13.000000 texproject-0.8.6/test/test_first.py
+drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-04-16 20:48:28.753260 texproject-0.8.7/
+-rw-r--r--   0 alexrutar   (501) staff       (20)     1067 2023-04-16 20:46:26.000000 texproject-0.8.7/LICENSE
+-rw-r--r--   0 alexrutar   (501) staff       (20)      108 2022-02-27 13:35:18.000000 texproject-0.8.7/MANIFEST.in
+-rw-r--r--   0 alexrutar   (501) staff       (20)     6471 2023-04-16 20:48:28.753380 texproject-0.8.7/PKG-INFO
+-rw-r--r--   0 alexrutar   (501) staff       (20)     5994 2023-04-16 20:46:26.000000 texproject-0.8.7/README.md
+-rw-r--r--   0 alexrutar   (501) staff       (20)      359 2022-11-06 14:30:17.000000 texproject-0.8.7/pyproject.toml
+-rw-r--r--   0 alexrutar   (501) staff       (20)      935 2023-04-16 20:48:28.753894 texproject-0.8.7/setup.cfg
+drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-04-16 20:48:28.740460 texproject-0.8.7/src/
+drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-04-16 20:48:28.746535 texproject-0.8.7/src/texproject/
+-rw-r--r--   0 alexrutar   (501) staff       (20)      214 2023-04-16 20:47:02.000000 texproject-0.8.7/src/texproject/__init__.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)       63 2021-12-14 22:57:13.000000 texproject-0.8.7/src/texproject/__main__.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)     3440 2023-04-16 20:46:26.000000 texproject-0.8.7/src/texproject/base.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)    17277 2023-02-25 18:19:54.000000 texproject-0.8.7/src/texproject/command.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)     5653 2022-12-20 21:15:22.000000 texproject-0.8.7/src/texproject/control.py
+drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-04-16 20:48:28.749724 texproject-0.8.7/src/texproject/defaults/
+-rw-r--r--   0 alexrutar   (501) staff       (20)        0 2021-12-22 01:04:12.000000 texproject-0.8.7/src/texproject/defaults/__init__.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)     1186 2022-11-23 22:47:39.000000 texproject-0.8.7/src/texproject/defaults/config.toml
+-rw-r--r--   0 alexrutar   (501) staff       (20)      115 2022-11-19 14:45:53.000000 texproject-0.8.7/src/texproject/defaults/template.toml
+-rw-r--r--   0 alexrutar   (501) staff       (20)      299 2022-01-13 12:30:10.000000 texproject-0.8.7/src/texproject/error.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)    10385 2023-04-16 20:46:26.000000 texproject-0.8.7/src/texproject/filesystem.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)     5889 2023-04-16 20:46:17.000000 texproject-0.8.7/src/texproject/git.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)    10908 2022-11-24 00:01:51.000000 texproject-0.8.7/src/texproject/output.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)    12788 2023-04-16 20:46:26.000000 texproject-0.8.7/src/texproject/template.py
+drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-04-16 20:48:28.752666 texproject-0.8.7/src/texproject/templates/
+-rw-r--r--   0 alexrutar   (501) staff       (20)        0 2022-01-05 23:14:40.000000 texproject-0.8.7/src/texproject/templates/__init__.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)       61 2021-01-19 13:47:15.000000 texproject-0.8.7/src/texproject/templates/arxiv_autotex.txt
+-rw-r--r--   0 alexrutar   (501) staff       (20)      304 2021-12-16 13:57:44.000000 texproject-0.8.7/src/texproject/templates/base.tex
+-rw-r--r--   0 alexrutar   (501) staff       (20)      308 2022-11-19 23:06:18.000000 texproject-0.8.7/src/texproject/templates/bibinfo.tex
+-rw-r--r--   0 alexrutar   (501) staff       (20)       67 2020-07-09 06:18:10.000000 texproject-0.8.7/src/texproject/templates/bibliography.tex
+-rw-r--r--   0 alexrutar   (501) staff       (20)      520 2023-02-25 18:19:54.000000 texproject-0.8.7/src/texproject/templates/build.yaml
+-rw-r--r--   0 alexrutar   (501) staff       (20)      842 2022-11-23 22:38:53.000000 texproject-0.8.7/src/texproject/templates/classinfo.tex
+-rw-r--r--   0 alexrutar   (501) staff       (20)       64 2021-12-21 16:46:46.000000 texproject-0.8.7/src/texproject/templates/gitignore
+-rwxr-xr-x   0 alexrutar   (501) staff       (20)      559 2022-03-23 18:03:46.000000 texproject-0.8.7/src/texproject/templates/pre-commit
+-rw-r--r--   0 alexrutar   (501) staff       (20)       17 2020-07-08 17:23:05.000000 texproject-0.8.7/src/texproject/templates/project_macro_file.tex
+-rw-r--r--   0 alexrutar   (501) staff       (20)     4292 2023-04-16 20:46:26.000000 texproject-0.8.7/src/texproject/term.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)     4992 2022-11-23 23:46:55.000000 texproject-0.8.7/src/texproject/utils.py
+drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-04-16 20:48:28.748847 texproject-0.8.7/src/texproject.egg-info/
+-rw-r--r--   0 alexrutar   (501) staff       (20)     6471 2023-04-16 20:48:28.000000 texproject-0.8.7/src/texproject.egg-info/PKG-INFO
+-rw-r--r--   0 alexrutar   (501) staff       (20)     1103 2023-04-16 20:48:28.000000 texproject-0.8.7/src/texproject.egg-info/SOURCES.txt
+-rw-r--r--   0 alexrutar   (501) staff       (20)        1 2023-04-16 20:48:28.000000 texproject-0.8.7/src/texproject.egg-info/dependency_links.txt
+-rw-r--r--   0 alexrutar   (501) staff       (20)       47 2023-04-16 20:48:28.000000 texproject-0.8.7/src/texproject.egg-info/entry_points.txt
+-rw-r--r--   0 alexrutar   (501) staff       (20)       53 2023-04-16 20:48:28.000000 texproject-0.8.7/src/texproject.egg-info/requires.txt
+-rw-r--r--   0 alexrutar   (501) staff       (20)       11 2023-04-16 20:48:28.000000 texproject-0.8.7/src/texproject.egg-info/top_level.txt
+drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-04-16 20:48:28.752986 texproject-0.8.7/test/
+-rw-r--r--   0 alexrutar   (501) staff       (20)     7589 2023-02-25 18:19:54.000000 texproject-0.8.7/test/test_first.py
```

### Comparing `texproject-0.8.6/LICENSE` & `texproject-0.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `texproject-0.8.6/PKG-INFO` & `texproject-0.8.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: texproject
-Version: 0.8.6
+Version: 0.8.7
 Summary: An automatic LaTeX project manager.
 Home-page: https://github.com/alexrutar/texproject
 Author: Alex Rutar
 Author-email: a@rutar.org
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `texproject-0.8.6/README.md` & `texproject-0.8.7/README.md`

 * *Files identical despite different names*

### Comparing `texproject-0.8.6/setup.cfg` & `texproject-0.8.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `texproject-0.8.6/src/texproject/base.py` & `texproject-0.8.7/src/texproject/base.py`

 * *Files identical despite different names*

### Comparing `texproject-0.8.6/src/texproject/command.py` & `texproject-0.8.7/src/texproject/command.py`

 * *Files identical despite different names*

### Comparing `texproject-0.8.6/src/texproject/control.py` & `texproject-0.8.7/src/texproject/control.py`

 * *Files identical despite different names*

### Comparing `texproject-0.8.6/src/texproject/defaults/config.toml` & `texproject-0.8.7/src/texproject/defaults/config.toml`

 * *Files identical despite different names*

### Comparing `texproject-0.8.6/src/texproject/filesystem.py` & `texproject-0.8.7/src/texproject/filesystem.py`

 * *Files identical despite different names*

### Comparing `texproject-0.8.6/src/texproject/git.py` & `texproject-0.8.7/src/texproject/git.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
                 FORMAT_MESSAGE.error("Remote repository already exists!"), *FAIL
             )
         else:
             gh_command = [
                 "gh",
                 "repo",
                 "create",
-                "--d",
+                "--description",
                 self.description,
                 "--source",
                 str(proj_path.dir),
                 "--remote",
                 "origin",
                 "--push",
                 _format_repo_name(self.repo_name, proj_path),
```

### Comparing `texproject-0.8.6/src/texproject/output.py` & `texproject-0.8.7/src/texproject/output.py`

 * *Files identical despite different names*

### Comparing `texproject-0.8.6/src/texproject/template.py` & `texproject-0.8.7/src/texproject/template.py`

 * *Files identical despite different names*

### Comparing `texproject-0.8.6/src/texproject/templates/build.yaml` & `texproject-0.8.7/src/texproject/templates/build.yaml`

 * *Files identical despite different names*

### Comparing `texproject-0.8.6/src/texproject/templates/classinfo.tex` & `texproject-0.8.7/src/texproject/templates/classinfo.tex`

 * *Files identical despite different names*

### Comparing `texproject-0.8.6/src/texproject/templates/pre-commit` & `texproject-0.8.7/src/texproject/templates/pre-commit`

 * *Files identical despite different names*

### Comparing `texproject-0.8.6/src/texproject/term.py` & `texproject-0.8.7/src/texproject/term.py`

 * *Files identical despite different names*

### Comparing `texproject-0.8.6/src/texproject/utils.py` & `texproject-0.8.7/src/texproject/utils.py`

 * *Files identical despite different names*

### Comparing `texproject-0.8.6/src/texproject.egg-info/PKG-INFO` & `texproject-0.8.7/src/texproject.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: texproject
-Version: 0.8.6
+Version: 0.8.7
 Summary: An automatic LaTeX project manager.
 Home-page: https://github.com/alexrutar/texproject
 Author: Alex Rutar
 Author-email: a@rutar.org
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `texproject-0.8.6/src/texproject.egg-info/SOURCES.txt` & `texproject-0.8.7/src/texproject.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `texproject-0.8.6/test/test_first.py` & `texproject-0.8.7/test/test_first.py`

 * *Files identical despite different names*

