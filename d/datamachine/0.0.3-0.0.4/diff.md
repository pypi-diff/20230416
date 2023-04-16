# Comparing `tmp/datamachine-0.0.3.tar.gz` & `tmp/datamachine-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamachine-0.0.3.tar", last modified: Sun Apr 16 00:54:18 2023, max compression
+gzip compressed data, was "datamachine-0.0.4.tar", last modified: Sun Apr 16 02:19:00 2023, max compression
```

## Comparing `datamachine-0.0.3.tar` & `datamachine-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 00:54:18.164503 datamachine-0.0.3/
--rw-rw-rw-   0        0        0     1074 2023-04-13 18:31:43.000000 datamachine-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      755 2023-04-16 00:54:18.165505 datamachine-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      139 2023-04-13 18:21:44.000000 datamachine-0.0.3/README.md
--rw-rw-rw-   0        0        0      652 2023-04-16 00:53:45.000000 datamachine-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      634 2023-04-16 00:54:18.170510 datamachine-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-16 00:54:18.148584 datamachine-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-16 00:54:18.152076 datamachine-0.0.3/src/datamachine/
--rw-rw-rw-   0        0        0       99 2023-04-16 00:10:59.000000 datamachine-0.0.3/src/datamachine/__init__.py
--rw-rw-rw-   0        0        0     4888 2023-04-16 00:19:32.000000 datamachine-0.0.3/src/datamachine/modular.py
-drwxrwxrwx   0        0        0        0 2023-04-16 00:54:18.164503 datamachine-0.0.3/src/datamachine.egg-info/
--rw-rw-rw-   0        0        0      755 2023-04-16 00:54:18.000000 datamachine-0.0.3/src/datamachine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-04-16 00:54:18.000000 datamachine-0.0.3/src/datamachine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 00:54:18.000000 datamachine-0.0.3/src/datamachine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-16 00:54:18.000000 datamachine-0.0.3/src/datamachine.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 02:19:00.360741 datamachine-0.0.4/
+-rw-rw-rw-   0        0        0     1074 2023-04-13 18:31:43.000000 datamachine-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      755 2023-04-16 02:19:00.360741 datamachine-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      139 2023-04-13 18:21:44.000000 datamachine-0.0.4/README.md
+-rw-rw-rw-   0        0        0      652 2023-04-16 02:18:35.000000 datamachine-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      634 2023-04-16 02:19:00.362728 datamachine-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-16 02:19:00.343848 datamachine-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-04-16 02:19:00.348050 datamachine-0.0.4/src/datamachine/
+-rw-rw-rw-   0        0        0       99 2023-04-16 00:10:59.000000 datamachine-0.0.4/src/datamachine/__init__.py
+-rw-rw-rw-   0        0        0     5175 2023-04-16 02:13:41.000000 datamachine-0.0.4/src/datamachine/modular.py
+drwxrwxrwx   0        0        0        0 2023-04-16 02:19:00.359749 datamachine-0.0.4/src/datamachine.egg-info/
+-rw-rw-rw-   0        0        0      755 2023-04-16 02:19:00.000000 datamachine-0.0.4/src/datamachine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-04-16 02:19:00.000000 datamachine-0.0.4/src/datamachine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 02:19:00.000000 datamachine-0.0.4/src/datamachine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-16 02:19:00.000000 datamachine-0.0.4/src/datamachine.egg-info/top_level.txt
```

### Comparing `datamachine-0.0.3/LICENSE` & `datamachine-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `datamachine-0.0.3/PKG-INFO` & `datamachine-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamachine
-Version: 0.0.3
+Version: 0.0.4
 Summary: A data machine made of modular Python notebooks
 Home-page: https://pypi.org/project/datamachine
 Author: Dave Killough
 Author-email: Dave Killough <dave.killough@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `datamachine-0.0.3/pyproject.toml` & `datamachine-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "datamachine"
-version = "0.0.3"
+version = "0.0.4"
 dependencies = []
 authors = [
   { name="Dave Killough", email="dave.killough@gmail.com" },
 ]
 description = "A data machine made of modular Python notebooks"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `datamachine-0.0.3/setup.cfg` & `datamachine-0.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 6174 616d 6163 6869 6e65 0d0a   = datamachine..
-00000020: 7665 7273 696f 6e20 3d20 302e 302e 330d  version = 0.0.3.
+00000020: 7665 7273 696f 6e20 3d20 302e 302e 340d  version = 0.0.4.
 00000030: 0a61 7574 686f 7220 3d20 4461 7665 204b  .author = Dave K
 00000040: 696c 6c6f 7567 680d 0a61 7574 686f 725f  illough..author_
 00000050: 656d 6169 6c20 3d20 6461 7665 2e6b 696c  email = dave.kil
 00000060: 6c6f 7567 6840 676d 6169 6c2e 636f 6d0d  lough@gmail.com.
 00000070: 0a64 6573 6372 6970 7469 6f6e 203d 2041  .description = A
 00000080: 2064 6174 6120 6d61 6368 696e 6520 6d61   data machine ma
 00000090: 6465 206f 6620 6d6f 6475 6c61 7220 5079  de of modular Py
```

### Comparing `datamachine-0.0.3/src/datamachine/modular.py` & `datamachine-0.0.4/src/datamachine/modular.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,14 +59,17 @@
             code += '\n# ' + '# '.join(cell['source'])
         # We want a blank newline after each cell's output.
         # And the last line of source doesn't have a newline usually.
         code += '\n\n'
     return code
 
 def import_notebook(link, attr = None):
+    folder = 'datamachine_temp'
+    if not os.path.exists(folder):
+        os.makedirs(folder)
     if '//colab.' in link:
         file_id = link.split('/')[-1] # get ID 
         url = GOOGLE_EXPORT + file_id
     elif '//raw.github' in link:
         url = link
     else: # search the index 
         index = import_notebook(MACHINE_INDEX) 
@@ -74,26 +77,29 @@
             print(link,' is not in the machine index')
             return
         i = index.IMPORTS[link]['link'] 
         ret = import_notebook(i)
         return ret
 
     rint = random.randint(10_000_000, 99_999_999) 
-    name = 'dmi_' + str(rint)
-    file = name + '.ipynb'
+    name = folder + os.path.sep + 'import' + str(rint)
+    filename = name + '.ipynb'
     with urlopen(url) as r:
-        with open(file, 'wb') as out_file:
+        with open(filename, 'wb') as out_file:
             shutil.copyfileobj(r, out_file) 
-    with open(file) as f:
+    with open(filename) as f:
         nb = json.load(f)
         with open(name + '.py','w') as text_file:
             text_file.write(code_from_ipynb(nb))
-    module = importlib.import_module(name)
-    loaded = [key for key in sys.modules.keys() if key.startswith('dmi_')]
-    delete = [f for f in glob.glob("dmi_*") if f.split('.')[0] not in loaded]
+    module = importlib.import_module(name.replace(os.path.sep,'.'))
+    loaded = [key for key in sys.modules.keys() 
+                if key.startswith('datamachine_temp.import')]
+    delete = [f for f in glob.glob("datamachine_temp/import*") 
+                if f.split('.')[0].replace(os.path.sep,'.') not in loaded]
+    print(loaded, delete) 
     for f in delete:
         os.remove(f)    
     if attr == None:
         return module
     else:
         return getattr(module, attr)
```

### Comparing `datamachine-0.0.3/src/datamachine.egg-info/PKG-INFO` & `datamachine-0.0.4/src/datamachine.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamachine
-Version: 0.0.3
+Version: 0.0.4
 Summary: A data machine made of modular Python notebooks
 Home-page: https://pypi.org/project/datamachine
 Author: Dave Killough
 Author-email: Dave Killough <dave.killough@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
```

