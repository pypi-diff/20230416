# Comparing `tmp/nimocr-0.1.tar.gz` & `tmp/nimocr-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nimocr-0.1.tar", last modified: Sun Apr 16 10:16:07 2023, max compression
+gzip compressed data, was "nimocr-0.1.1.tar", last modified: Sun Apr 16 10:39:35 2023, max compression
```

## Comparing `nimocr-0.1.tar` & `nimocr-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,24 @@
-drwxr-xr-x   0 nim        (501) staff       (20)        0 2023-04-16 10:16:07.755516 nimocr-0.1/
--rw-r--r--   0 nim        (501) staff       (20)      209 2023-04-16 10:16:07.755317 nimocr-0.1/PKG-INFO
--rw-r--r--   0 nim        (501) staff       (20)       15 2023-04-13 03:27:01.000000 nimocr-0.1/README.md
-drwxr-xr-x   0 nim        (501) staff       (20)        0 2023-04-16 10:16:07.755071 nimocr-0.1/nimocr.egg-info/
--rw-r--r--   0 nim        (501) staff       (20)      209 2023-04-16 10:16:07.000000 nimocr-0.1/nimocr.egg-info/PKG-INFO
--rw-r--r--   0 nim        (501) staff       (20)      200 2023-04-16 10:16:07.000000 nimocr-0.1/nimocr.egg-info/SOURCES.txt
--rw-r--r--   0 nim        (501) staff       (20)        1 2023-04-16 10:16:07.000000 nimocr-0.1/nimocr.egg-info/dependency_links.txt
--rw-r--r--   0 nim        (501) staff       (20)       44 2023-04-16 10:16:07.000000 nimocr-0.1/nimocr.egg-info/entry_points.txt
--rw-r--r--   0 nim        (501) staff       (20)       98 2023-04-16 10:16:07.000000 nimocr-0.1/nimocr.egg-info/requires.txt
--rw-r--r--   0 nim        (501) staff       (20)        1 2023-04-16 10:16:07.000000 nimocr-0.1/nimocr.egg-info/top_level.txt
--rw-r--r--   0 nim        (501) staff       (20)       38 2023-04-16 10:16:07.755570 nimocr-0.1/setup.cfg
--rw-r--r--   0 nim        (501) staff       (20)      603 2023-04-16 10:16:05.000000 nimocr-0.1/setup.py
+drwxr-xr-x   0 nim        (501) staff       (20)        0 2023-04-16 10:39:35.457438 nimocr-0.1.1/
+-rw-r--r--   0 nim        (501) staff       (20)      211 2023-04-16 10:39:35.457198 nimocr-0.1.1/PKG-INFO
+-rw-r--r--   0 nim        (501) staff       (20)       15 2023-04-13 03:27:01.000000 nimocr-0.1.1/README.md
+drwxr-xr-x   0 nim        (501) staff       (20)        0 2023-04-16 10:39:35.454317 nimocr-0.1.1/model/
+-rw-r--r--   0 nim        (501) staff       (20)        0 2023-04-16 10:29:48.000000 nimocr-0.1.1/model/__init__.py
+-rw-r--r--   0 nim        (501) staff       (20)     4387 2023-04-16 08:23:30.000000 nimocr-0.1.1/model/image_list.py
+drwxr-xr-x   0 nim        (501) staff       (20)        0 2023-04-16 10:39:35.455700 nimocr-0.1.1/nimocr.egg-info/
+-rw-r--r--   0 nim        (501) staff       (20)      211 2023-04-16 10:39:35.000000 nimocr-0.1.1/nimocr.egg-info/PKG-INFO
+-rw-r--r--   0 nim        (501) staff       (20)      365 2023-04-16 10:39:35.000000 nimocr-0.1.1/nimocr.egg-info/SOURCES.txt
+-rw-r--r--   0 nim        (501) staff       (20)        1 2023-04-16 10:39:35.000000 nimocr-0.1.1/nimocr.egg-info/dependency_links.txt
+-rw-r--r--   0 nim        (501) staff       (20)       41 2023-04-16 10:39:35.000000 nimocr-0.1.1/nimocr.egg-info/entry_points.txt
+-rw-r--r--   0 nim        (501) staff       (20)       98 2023-04-16 10:39:35.000000 nimocr-0.1.1/nimocr.egg-info/requires.txt
+-rw-r--r--   0 nim        (501) staff       (20)       21 2023-04-16 10:39:35.000000 nimocr-0.1.1/nimocr.egg-info/top_level.txt
+drwxr-xr-x   0 nim        (501) staff       (20)        0 2023-04-16 10:39:35.456055 nimocr-0.1.1/presenter/
+-rw-r--r--   0 nim        (501) staff       (20)        0 2023-04-16 10:29:53.000000 nimocr-0.1.1/presenter/__init__.py
+-rw-r--r--   0 nim        (501) staff       (20)     3961 2023-04-16 07:10:40.000000 nimocr-0.1.1/presenter/presenter.py
+-rw-r--r--   0 nim        (501) staff       (20)       88 2023-04-16 10:37:04.000000 nimocr-0.1.1/pyproject.toml
+-rw-r--r--   0 nim        (501) staff       (20)       38 2023-04-16 10:39:35.457504 nimocr-0.1.1/setup.cfg
+-rw-r--r--   0 nim        (501) staff       (20)      602 2023-04-16 10:37:55.000000 nimocr-0.1.1/setup.py
+drwxr-xr-x   0 nim        (501) staff       (20)        0 2023-04-16 10:39:35.456866 nimocr-0.1.1/view/
+-rw-r--r--   0 nim        (501) staff       (20)        0 2023-04-16 10:29:58.000000 nimocr-0.1.1/view/__init__.py
+-rw-r--r--   0 nim        (501) staff       (20)     4589 2023-04-16 10:07:42.000000 nimocr-0.1.1/view/dialog.py
+-rw-r--r--   0 nim        (501) staff       (20)     7586 2023-04-16 10:14:03.000000 nimocr-0.1.1/view/main_window.py
+-rw-r--r--   0 nim        (501) staff       (20)     6961 2023-04-16 07:10:40.000000 nimocr-0.1.1/view/widget.py
```

### Comparing `nimocr-0.1/setup.py` & `nimocr-0.1.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
 setup(
     name='nimocr',
-    version='0.1',
+    version='0.1.1',
     packages=find_packages(),
     install_requires=[
         "numpy==1.24.2",
         "opencv_python==4.7.0.72",
         "pandas==2.0.0",
         "Pillow==9.5.0",
         "PyQt6==6.5.0",
         "setuptools==67.6.1"
     ],
     entry_points={
         'console_scripts': [
-            'annotator=annotator:run',
+            'nimocr=annotator:run',
         ],
     },
     author='Chatcharin Sangbutsarakum',
     author_email='chatcharinsang@gmail.com',
     description='OCR Annotator Tool',
     url='https://github.com/what-in-the-nim/ocr-annotator',
 )
```

