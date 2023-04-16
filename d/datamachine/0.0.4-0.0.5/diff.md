# Comparing `tmp/datamachine-0.0.4.tar.gz` & `tmp/datamachine-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamachine-0.0.4.tar", last modified: Sun Apr 16 02:19:00 2023, max compression
+gzip compressed data, was "datamachine-0.0.5.tar", last modified: Sun Apr 16 02:45:06 2023, max compression
```

## Comparing `datamachine-0.0.4.tar` & `datamachine-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 02:19:00.360741 datamachine-0.0.4/
--rw-rw-rw-   0        0        0     1074 2023-04-13 18:31:43.000000 datamachine-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      755 2023-04-16 02:19:00.360741 datamachine-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      139 2023-04-13 18:21:44.000000 datamachine-0.0.4/README.md
--rw-rw-rw-   0        0        0      652 2023-04-16 02:18:35.000000 datamachine-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0      634 2023-04-16 02:19:00.362728 datamachine-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-16 02:19:00.343848 datamachine-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-04-16 02:19:00.348050 datamachine-0.0.4/src/datamachine/
--rw-rw-rw-   0        0        0       99 2023-04-16 00:10:59.000000 datamachine-0.0.4/src/datamachine/__init__.py
--rw-rw-rw-   0        0        0     5175 2023-04-16 02:13:41.000000 datamachine-0.0.4/src/datamachine/modular.py
-drwxrwxrwx   0        0        0        0 2023-04-16 02:19:00.359749 datamachine-0.0.4/src/datamachine.egg-info/
--rw-rw-rw-   0        0        0      755 2023-04-16 02:19:00.000000 datamachine-0.0.4/src/datamachine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-04-16 02:19:00.000000 datamachine-0.0.4/src/datamachine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 02:19:00.000000 datamachine-0.0.4/src/datamachine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-16 02:19:00.000000 datamachine-0.0.4/src/datamachine.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 02:45:06.453410 datamachine-0.0.5/
+-rw-rw-rw-   0        0        0     1074 2023-04-13 18:31:43.000000 datamachine-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      755 2023-04-16 02:45:06.454410 datamachine-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      139 2023-04-13 18:21:44.000000 datamachine-0.0.5/README.md
+-rw-rw-rw-   0        0        0      652 2023-04-16 02:44:49.000000 datamachine-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0      634 2023-04-16 02:45:06.455410 datamachine-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-16 02:45:06.439724 datamachine-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-04-16 02:45:06.444631 datamachine-0.0.5/src/datamachine/
+-rw-rw-rw-   0        0        0       99 2023-04-16 00:10:59.000000 datamachine-0.0.5/src/datamachine/__init__.py
+-rw-rw-rw-   0        0        0     5051 2023-04-16 02:31:46.000000 datamachine-0.0.5/src/datamachine/modular copy.py
+-rw-rw-rw-   0        0        0     5028 2023-04-16 02:43:28.000000 datamachine-0.0.5/src/datamachine/modular.py
+drwxrwxrwx   0        0        0        0 2023-04-16 02:45:06.453410 datamachine-0.0.5/src/datamachine.egg-info/
+-rw-rw-rw-   0        0        0      755 2023-04-16 02:45:06.000000 datamachine-0.0.5/src/datamachine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2023-04-16 02:45:06.000000 datamachine-0.0.5/src/datamachine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 02:45:06.000000 datamachine-0.0.5/src/datamachine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-16 02:45:06.000000 datamachine-0.0.5/src/datamachine.egg-info/top_level.txt
```

### Comparing `datamachine-0.0.4/LICENSE` & `datamachine-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `datamachine-0.0.4/PKG-INFO` & `datamachine-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamachine
-Version: 0.0.4
+Version: 0.0.5
 Summary: A data machine made of modular Python notebooks
 Home-page: https://pypi.org/project/datamachine
 Author: Dave Killough
 Author-email: Dave Killough <dave.killough@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `datamachine-0.0.4/pyproject.toml` & `datamachine-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "datamachine"
-version = "0.0.4"
+version = "0.0.5"
 dependencies = []
 authors = [
   { name="Dave Killough", email="dave.killough@gmail.com" },
 ]
 description = "A data machine made of modular Python notebooks"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `datamachine-0.0.4/setup.cfg` & `datamachine-0.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `datamachine-0.0.4/src/datamachine/modular.py` & `datamachine-0.0.5/src/datamachine/modular copy.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,19 +35,14 @@
 ##############################################################################
 # This source has been auto generated from an IPython/Jupyter notebook file. #
 # Please modify the origin file                                              #
 ##############################################################################
 """
 
 def code_from_ipynb(nb):
-    """
-    Get the code for a given notebook
-
-    nb is passed in as a dictionary that's a parsed ipynb file
-    """
     code = PREAMBLE
     for cell in nb['cells']:
         if cell['cell_type'] == 'code':
             # transform the input to executable Python
             src = cell['source']
             if src[0].startswith('#run'): 
                 code += '\n# ' + '# '.join(cell['source'])
@@ -75,15 +70,14 @@
         index = import_notebook(MACHINE_INDEX) 
         if link not in index.IMPORTS:
             print(link,' is not in the machine index')
             return
         i = index.IMPORTS[link]['link'] 
         ret = import_notebook(i)
         return ret
-
     rint = random.randint(10_000_000, 99_999_999) 
     name = folder + os.path.sep + 'import' + str(rint)
     filename = name + '.ipynb'
     with urlopen(url) as r:
         with open(filename, 'wb') as out_file:
             shutil.copyfileobj(r, out_file) 
     with open(filename) as f:
@@ -91,15 +85,15 @@
         with open(name + '.py','w') as text_file:
             text_file.write(code_from_ipynb(nb))
     module = importlib.import_module(name.replace(os.path.sep,'.'))
     loaded = [key for key in sys.modules.keys() 
                 if key.startswith('datamachine_temp.import')]
     delete = [f for f in glob.glob("datamachine_temp/import*") 
                 if f.split('.')[0].replace(os.path.sep,'.') not in loaded]
-    print(loaded, delete) 
+    #print(loaded, delete) 
     for f in delete:
         os.remove(f)    
     if attr == None:
         return module
     else:
         return getattr(module, attr)
```

### Comparing `datamachine-0.0.4/src/datamachine.egg-info/PKG-INFO` & `datamachine-0.0.5/src/datamachine.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamachine
-Version: 0.0.4
+Version: 0.0.5
 Summary: A data machine made of modular Python notebooks
 Home-page: https://pypi.org/project/datamachine
 Author: Dave Killough
 Author-email: Dave Killough <dave.killough@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
```

