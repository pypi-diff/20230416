# Comparing `tmp/manga2pdf-0.0.4.tar.gz` & `tmp/manga2pdf-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manga2pdf-0.0.4.tar", last modified: Mon Apr 10 12:18:27 2023, max compression
+gzip compressed data, was "manga2pdf-0.1.0.tar", last modified: Sun Apr 16 05:49:21 2023, max compression
```

## Comparing `manga2pdf-0.0.4.tar` & `manga2pdf-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 shun       (501) staff       (20)        0 2023-04-10 12:18:27.381574 manga2pdf-0.0.4/
--rw-r--r--   0 shun       (501) staff       (20)     1063 2023-03-12 05:13:58.000000 manga2pdf-0.0.4/LICENSE
--rw-r--r--   0 shun       (501) staff       (20)     5624 2023-04-10 12:18:27.381455 manga2pdf-0.0.4/PKG-INFO
--rw-r--r--   0 shun       (501) staff       (20)     5080 2023-04-01 11:10:27.000000 manga2pdf-0.0.4/README.md
--rw-r--r--   0 shun       (501) staff       (20)       38 2023-04-10 12:18:27.381604 manga2pdf-0.0.4/setup.cfg
--rw-r--r--   0 shun       (501) staff       (20)     1035 2023-04-10 10:22:02.000000 manga2pdf-0.0.4/setup.py
-drwxr-xr-x   0 shun       (501) staff       (20)        0 2023-04-10 12:18:27.380649 manga2pdf-0.0.4/src/
-drwxr-xr-x   0 shun       (501) staff       (20)        0 2023-04-10 12:18:27.381298 manga2pdf-0.0.4/src/manga2pdf.egg-info/
--rw-r--r--   0 shun       (501) staff       (20)     5624 2023-04-10 12:18:27.000000 manga2pdf-0.0.4/src/manga2pdf.egg-info/PKG-INFO
--rw-r--r--   0 shun       (501) staff       (20)      267 2023-04-10 12:18:27.000000 manga2pdf-0.0.4/src/manga2pdf.egg-info/SOURCES.txt
--rw-r--r--   0 shun       (501) staff       (20)        1 2023-04-10 12:18:27.000000 manga2pdf-0.0.4/src/manga2pdf.egg-info/dependency_links.txt
--rw-r--r--   0 shun       (501) staff       (20)       45 2023-04-10 12:18:27.000000 manga2pdf-0.0.4/src/manga2pdf.egg-info/entry_points.txt
--rw-r--r--   0 shun       (501) staff       (20)       46 2023-04-10 12:18:27.000000 manga2pdf-0.0.4/src/manga2pdf.egg-info/requires.txt
--rw-r--r--   0 shun       (501) staff       (20)       10 2023-04-10 12:18:27.000000 manga2pdf-0.0.4/src/manga2pdf.egg-info/top_level.txt
--rw-r--r--   0 shun       (501) staff       (20)    17429 2023-04-10 10:18:41.000000 manga2pdf-0.0.4/src/manga2pdf.py
+drwxr-xr-x   0 shun       (501) staff       (20)        0 2023-04-16 05:49:21.417041 manga2pdf-0.1.0/
+-rw-r--r--   0 shun       (501) staff       (20)     1063 2023-03-12 05:13:58.000000 manga2pdf-0.1.0/LICENSE
+-rw-r--r--   0 shun       (501) staff       (20)     5913 2023-04-16 05:49:21.416910 manga2pdf-0.1.0/PKG-INFO
+-rw-r--r--   0 shun       (501) staff       (20)     5369 2023-04-15 20:09:50.000000 manga2pdf-0.1.0/README.md
+-rw-r--r--   0 shun       (501) staff       (20)       38 2023-04-16 05:49:21.417106 manga2pdf-0.1.0/setup.cfg
+-rw-r--r--   0 shun       (501) staff       (20)     1052 2023-04-16 05:42:55.000000 manga2pdf-0.1.0/setup.py
+drwxr-xr-x   0 shun       (501) staff       (20)        0 2023-04-16 05:49:21.415760 manga2pdf-0.1.0/src/
+drwxr-xr-x   0 shun       (501) staff       (20)        0 2023-04-16 05:49:21.416721 manga2pdf-0.1.0/src/manga2pdf.egg-info/
+-rw-r--r--   0 shun       (501) staff       (20)     5913 2023-04-16 05:49:21.000000 manga2pdf-0.1.0/src/manga2pdf.egg-info/PKG-INFO
+-rw-r--r--   0 shun       (501) staff       (20)      288 2023-04-16 05:49:21.000000 manga2pdf-0.1.0/src/manga2pdf.egg-info/SOURCES.txt
+-rw-r--r--   0 shun       (501) staff       (20)        1 2023-04-16 05:49:21.000000 manga2pdf-0.1.0/src/manga2pdf.egg-info/dependency_links.txt
+-rw-r--r--   0 shun       (501) staff       (20)       45 2023-04-16 05:49:21.000000 manga2pdf-0.1.0/src/manga2pdf.egg-info/entry_points.txt
+-rw-r--r--   0 shun       (501) staff       (20)       46 2023-04-16 05:49:21.000000 manga2pdf-0.1.0/src/manga2pdf.egg-info/requires.txt
+-rw-r--r--   0 shun       (501) staff       (20)       24 2023-04-16 05:49:21.000000 manga2pdf-0.1.0/src/manga2pdf.egg-info/top_level.txt
+-rw-r--r--   0 shun       (501) staff       (20)    17683 2023-04-15 20:21:17.000000 manga2pdf-0.1.0/src/manga2pdf.py
+-rw-r--r--   0 shun       (501) staff       (20)    18189 2023-04-15 20:21:57.000000 manga2pdf-0.1.0/src/manga2pdf_gui.py
```

### Comparing `manga2pdf-0.0.4/LICENSE` & `manga2pdf-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `manga2pdf-0.0.4/PKG-INFO` & `manga2pdf-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manga2pdf
-Version: 0.0.4
+Version: 0.1.0
 Summary: Convert manga/comic files(zip, epub, etc.) or directory containing image files (jpg, png, etc.) to PDF.
 Home-page: https://github.com/mashu3/manga2pdf
 Author: mashu3
 License: MIT
 Keywords: manga comic pdf converter
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
@@ -86,9 +86,17 @@
 $ manga2pdf my_manga.epub -o my_manga_spread.pdf
 ```
 - To convert `my_comic.epub` to `my_comic.pdf` with a TwoPage view and left binding:
 ```
 $ manga2pdf my_comic.epub -o my_comic.pdf -p TwoPageLeft -d L2R
 ```
 
+## GUI
+To launch the graphical user interface:
+```
+$ manga2pdf -gui
+``` 
+The interface supports English and Japanese, and all settings that can be specified via the command line are available.
+The GUI is currently under development and additional features are planned for future updates.
+
 ## Author
 [mashu3](https://github.com/mashu3)
```

### Comparing `manga2pdf-0.0.4/README.md` & `manga2pdf-0.1.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -71,9 +71,17 @@
 $ manga2pdf my_manga.epub -o my_manga_spread.pdf
 ```
 - To convert `my_comic.epub` to `my_comic.pdf` with a TwoPage view and left binding:
 ```
 $ manga2pdf my_comic.epub -o my_comic.pdf -p TwoPageLeft -d L2R
 ```
 
+## GUI
+To launch the graphical user interface:
+```
+$ manga2pdf -gui
+``` 
+The interface supports English and Japanese, and all settings that can be specified via the command line are available.
+The GUI is currently under development and additional features are planned for future updates.
+
 ## Author
 [mashu3](https://github.com/mashu3)
```

### Comparing `manga2pdf-0.0.4/setup.py` & `manga2pdf-0.1.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.4"
+VERSION = "0.1.0"
 
 INSTALL_REQUIRES = (
     "img2pdf",
     "Pillow",
     "pikepdf",
     "rarfile",
     "beautifulsoup4"
@@ -23,15 +23,15 @@
     description="Convert manga/comic files(zip, epub, etc.) or directory containing image files (jpg, png, etc.) to PDF.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     keywords="manga comic pdf converter",
     url="https://github.com/mashu3/manga2pdf",
     license='MIT',
     package_dir={"": "src"},
-    py_modules=["manga2pdf"],
+    py_modules=["manga2pdf", "manga2pdf_gui"],
     packages = find_packages("src"),
     classifiers=CLASSIFIERS,
     install_requires=INSTALL_REQUIRES,
     entry_points={
         "console_scripts": [
             "manga2pdf=manga2pdf:main",
         ]
```

### Comparing `manga2pdf-0.0.4/src/manga2pdf.egg-info/PKG-INFO` & `manga2pdf-0.1.0/src/manga2pdf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manga2pdf
-Version: 0.0.4
+Version: 0.1.0
 Summary: Convert manga/comic files(zip, epub, etc.) or directory containing image files (jpg, png, etc.) to PDF.
 Home-page: https://github.com/mashu3/manga2pdf
 Author: mashu3
 License: MIT
 Keywords: manga comic pdf converter
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
@@ -86,9 +86,17 @@
 $ manga2pdf my_manga.epub -o my_manga_spread.pdf
 ```
 - To convert `my_comic.epub` to `my_comic.pdf` with a TwoPage view and left binding:
 ```
 $ manga2pdf my_comic.epub -o my_comic.pdf -p TwoPageLeft -d L2R
 ```
 
+## GUI
+To launch the graphical user interface:
+```
+$ manga2pdf -gui
+``` 
+The interface supports English and Japanese, and all settings that can be specified via the command line are available.
+The GUI is currently under development and additional features are planned for future updates.
+
 ## Author
 [mashu3](https://github.com/mashu3)
```

### Comparing `manga2pdf-0.0.4/src/manga2pdf.py` & `manga2pdf-0.1.0/src/manga2pdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -328,36 +328,40 @@
 TwoColumnRight -> Separate Cover, Scrolling Spread View''')
     parser.add_argument('-d', '--direction', type=str, default='R2L', choices=['L2R', 'R2L'],
                         help='''\
 L2R -> Left Binding
 (default)R2L -> Right Binding''')
     parser.add_argument('-j', '--jpeg', action='store_true', help='Convert images to JPEG')
     parser.add_argument('-g', '--grayscale', action='store_true', help='Convert images to grayscale')
-
+    parser.add_argument('-gui', action='store_true', help='Launch GUI')
 
     args = parser.parse_args()
-    if args.input_path is None:
-        parser.print_usage()
-        parser.print_help()
-        sys.exit(1)
-    if not os.path.isdir(args.input_path):
-        ext = os.path.splitext(args.input_path)[1].lower()
-        if not ext in ['.zip', '.cbz', '.rar', '.cbr', '.epub']:
-            print('Error: The input file format is not supported. The currently supported formats are: .zip, .cbz, .rar, .cbr, and .epub.')
+    if args.gui:
+        import manga2pdf_gui
+        manga2pdf_gui.launch_gui()
+    else:
+        if args.input_path is None:
+            parser.print_usage()
+            parser.print_help()
             sys.exit(1)
-    if args.output_path is not None:
-        if not args.output_path.endswith('.pdf'):
-            print('Error: The output file must be an PDF file.')
+        if not os.path.isdir(args.input_path):
+            ext = os.path.splitext(args.input_path)[1].lower()
+            if not ext in ['.zip', '.cbz', '.rar', '.cbr', '.epub']:
+                print('Error: The input file format is not supported. The currently supported formats are: .zip, .cbz, .rar, .cbr, and .epub.')
+                sys.exit(1)
+        if args.output_path is not None:
+            if not args.output_path.endswith('.pdf'):
+                print('Error: The output file must be an PDF file.')
+                sys.exit(1)
+        if args.grayscale and args.jpeg:
+            print('Error: Cannot specify both --grayscale and --jpeg options.')
             sys.exit(1)
-    if args.grayscale and args.jpeg:
-        print('Error: Cannot specify both --grayscale and --jpeg options.')
-        sys.exit(1)
-    
-    converter = MangaPdfConverter(args.input_path, args.output_path, args.pagelayout, args.direction)
-    if args.jpeg:
-        converter.set_convert_to_jpeg(True)
-    elif args.grayscale:
-        converter.set_convert_to_grayscale(True)
-    converter.convert()
+        
+        converter = MangaPdfConverter(args.input_path, args.output_path, args.pagelayout, args.direction)
+        if args.jpeg:
+            converter.set_convert_to_jpeg(True)
+        elif args.grayscale:
+            converter.set_convert_to_grayscale(True)
+        converter.convert()
 
 if __name__ == '__main__':
     main()
```

