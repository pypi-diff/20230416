# Comparing `tmp/ib110hw-0.1.0.tar.gz` & `tmp/ib110hw-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ib110hw-0.1.0.tar", last modified: Sun Apr 16 21:02:35 2023, max compression
+gzip compressed data, was "ib110hw-0.1.1.tar", last modified: Sun Apr 16 21:36:31 2023, max compression
```

## Comparing `ib110hw-0.1.0.tar` & `ib110hw-0.1.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 21:02:35.575616 ib110hw-0.1.0/
--rw-rw-rw-   0        0        0     1090 2023-01-20 12:57:50.000000 ib110hw-0.1.0/LICENSE
--rw-rw-rw-   0        0        0    26611 2023-04-16 21:02:35.575616 ib110hw-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0    26229 2023-04-16 20:59:38.000000 ib110hw-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-16 21:02:35.575616 ib110hw-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      649 2023-04-16 21:00:19.000000 ib110hw-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-16 21:02:35.531004 ib110hw-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-16 21:02:35.541619 ib110hw-0.1.0/src/ib110hw/
--rw-rw-rw-   0        0        0        0 2023-02-08 22:35:52.000000 ib110hw-0.1.0/src/ib110hw/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 21:02:35.562615 ib110hw-0.1.0/src/ib110hw/automaton/
--rw-rw-rw-   0        0        0        0 2022-10-30 17:04:59.000000 ib110hw-0.1.0/src/ib110hw/automaton/__init__.py
--rw-rw-rw-   0        0        0     2304 2023-04-16 00:59:04.000000 ib110hw-0.1.0/src/ib110hw/automaton/base.py
--rw-rw-rw-   0        0        0     8262 2023-04-16 19:56:06.000000 ib110hw-0.1.0/src/ib110hw/automaton/dfa.py
--rw-rw-rw-   0        0        0     8539 2023-04-16 19:56:24.000000 ib110hw-0.1.0/src/ib110hw/automaton/nfa.py
--rw-rw-rw-   0        0        0     1439 2023-02-10 23:11:04.000000 ib110hw-0.1.0/src/ib110hw/automaton/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-16 21:02:35.569615 ib110hw-0.1.0/src/ib110hw/turing/
--rw-rw-rw-   0        0        0        0 2022-11-28 20:58:41.000000 ib110hw-0.1.0/src/ib110hw/turing/__init__.py
--rw-rw-rw-   0        0        0     4911 2023-04-11 20:33:53.000000 ib110hw-0.1.0/src/ib110hw/turing/_helpers.py
--rw-rw-rw-   0        0        0     1239 2023-04-06 00:41:42.000000 ib110hw-0.1.0/src/ib110hw/turing/base.py
--rw-rw-rw-   0        0        0     4606 2023-04-11 17:53:39.000000 ib110hw-0.1.0/src/ib110hw/turing/dtm.py
--rw-rw-rw-   0        0        0     5704 2023-04-06 00:44:32.000000 ib110hw-0.1.0/src/ib110hw/turing/mtm.py
--rw-rw-rw-   0        0        0     3474 2023-04-06 00:42:49.000000 ib110hw-0.1.0/src/ib110hw/turing/tape.py
--rw-rw-rw-   0        0        0     1357 2023-04-11 20:31:00.000000 ib110hw-0.1.0/src/ib110hw/turing/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-16 21:02:35.557614 ib110hw-0.1.0/src/ib110hw.egg-info/
--rw-rw-rw-   0        0        0    26611 2023-04-16 21:02:35.000000 ib110hw-0.1.0/src/ib110hw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      611 2023-04-16 21:02:35.000000 ib110hw-0.1.0/src/ib110hw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 21:02:35.000000 ib110hw-0.1.0/src/ib110hw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-16 21:02:35.000000 ib110hw-0.1.0/src/ib110hw.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-16 21:02:35.573614 ib110hw-0.1.0/tests/
--rw-rw-rw-   0        0        0     7220 2023-04-16 19:57:54.000000 ib110hw-0.1.0/tests/test_dfa.py
--rw-rw-rw-   0        0        0     2369 2023-04-02 20:51:44.000000 ib110hw-0.1.0/tests/test_dtm.py
--rw-rw-rw-   0        0        0     2028 2023-04-02 20:51:33.000000 ib110hw-0.1.0/tests/test_mtm.py
--rw-rw-rw-   0        0        0     8579 2023-04-16 19:57:58.000000 ib110hw-0.1.0/tests/test_nfa.py
+drwxrwxrwx   0        0        0        0 2023-04-16 21:36:31.507216 ib110hw-0.1.1/
+-rw-rw-rw-   0        0        0     1090 2023-01-20 12:57:50.000000 ib110hw-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0    26595 2023-04-16 21:36:31.507216 ib110hw-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    26213 2023-04-16 21:05:41.000000 ib110hw-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-16 21:36:31.508216 ib110hw-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      649 2023-04-16 21:36:12.000000 ib110hw-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 21:36:31.466218 ib110hw-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-16 21:36:31.472217 ib110hw-0.1.1/src/ib110hw/
+-rw-rw-rw-   0        0        0        0 2023-02-08 22:35:52.000000 ib110hw-0.1.1/src/ib110hw/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 21:36:31.493217 ib110hw-0.1.1/src/ib110hw/automaton/
+-rw-rw-rw-   0        0        0        0 2022-10-30 17:04:59.000000 ib110hw-0.1.1/src/ib110hw/automaton/__init__.py
+-rw-rw-rw-   0        0        0     2304 2023-04-16 00:59:04.000000 ib110hw-0.1.1/src/ib110hw/automaton/base.py
+-rw-rw-rw-   0        0        0     8262 2023-04-16 19:56:06.000000 ib110hw-0.1.1/src/ib110hw/automaton/dfa.py
+-rw-rw-rw-   0        0        0     8539 2023-04-16 19:56:24.000000 ib110hw-0.1.1/src/ib110hw/automaton/nfa.py
+-rw-rw-rw-   0        0        0     1439 2023-02-10 23:11:04.000000 ib110hw-0.1.1/src/ib110hw/automaton/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-16 21:36:31.501217 ib110hw-0.1.1/src/ib110hw/turing/
+-rw-rw-rw-   0        0        0        0 2022-11-28 20:58:41.000000 ib110hw-0.1.1/src/ib110hw/turing/__init__.py
+-rw-rw-rw-   0        0        0     4911 2023-04-11 20:33:53.000000 ib110hw-0.1.1/src/ib110hw/turing/_helpers.py
+-rw-rw-rw-   0        0        0     1239 2023-04-06 00:41:42.000000 ib110hw-0.1.1/src/ib110hw/turing/base.py
+-rw-rw-rw-   0        0        0     4606 2023-04-11 17:53:39.000000 ib110hw-0.1.1/src/ib110hw/turing/dtm.py
+-rw-rw-rw-   0        0        0     5704 2023-04-06 00:44:32.000000 ib110hw-0.1.1/src/ib110hw/turing/mtm.py
+-rw-rw-rw-   0        0        0     3474 2023-04-06 00:42:49.000000 ib110hw-0.1.1/src/ib110hw/turing/tape.py
+-rw-rw-rw-   0        0        0     1186 2023-04-16 21:34:51.000000 ib110hw-0.1.1/src/ib110hw/turing/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-16 21:36:31.488215 ib110hw-0.1.1/src/ib110hw.egg-info/
+-rw-rw-rw-   0        0        0    26595 2023-04-16 21:36:31.000000 ib110hw-0.1.1/src/ib110hw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      611 2023-04-16 21:36:31.000000 ib110hw-0.1.1/src/ib110hw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 21:36:31.000000 ib110hw-0.1.1/src/ib110hw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-16 21:36:31.000000 ib110hw-0.1.1/src/ib110hw.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 21:36:31.505216 ib110hw-0.1.1/tests/
+-rw-rw-rw-   0        0        0     7220 2023-04-16 19:57:54.000000 ib110hw-0.1.1/tests/test_dfa.py
+-rw-rw-rw-   0        0        0     2369 2023-04-02 20:51:44.000000 ib110hw-0.1.1/tests/test_dtm.py
+-rw-rw-rw-   0        0        0     2028 2023-04-02 20:51:33.000000 ib110hw-0.1.1/tests/test_mtm.py
+-rw-rw-rw-   0        0        0     8579 2023-04-16 19:57:58.000000 ib110hw-0.1.1/tests/test_nfa.py
```

### Comparing `ib110hw-0.1.0/LICENSE` & `ib110hw-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.0/PKG-INFO` & `ib110hw-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ib110hw
-Version: 0.1.0
+Version: 0.1.1
 Home-page: https://github.com/pilatmartin/ib110hw
 Author: Martin Pilát
 Author-email: 8pilatmartin8@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -16,22 +16,22 @@
 
 Using virtual environment is of course optional, but recommended.
 
 ```sh
 # Bash
 $ python3 -m venv <name> 
 $ source <name>/bin/activate
-$ pip install ib110hw_testing
+$ pip install ib110hw
 ```
 
 ```powershell
 # Windows Powershell
 PS> py -m venv <name> 
 PS> <name>\Scripts\Activate.ps1
-PS> pip install ib110hw_testing
+PS> pip install ib110hw
 ```
 
 Below is an overview of how these computational models can be used. Further documentation is located in the files with the implementation.
 
 # FINITE AUTOMATA
 
 This library supports **deterministic** and **nondeterministic** finite automata. You can find the implementation of these models in the module `automaton`. Consider the class located in the `base.py` as abstract, its only purpose is to avoid duplicity in the implementation of these models.
```

### Comparing `ib110hw-0.1.0/README.md` & `ib110hw-0.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 
 Using virtual environment is of course optional, but recommended.
 
 ```sh
 # Bash
 $ python3 -m venv <name> 
 $ source <name>/bin/activate
-$ pip install ib110hw_testing
+$ pip install ib110hw
 ```
 
 ```powershell
 # Windows Powershell
 PS> py -m venv <name> 
 PS> <name>\Scripts\Activate.ps1
-PS> pip install ib110hw_testing
+PS> pip install ib110hw
 ```
 
 Below is an overview of how these computational models can be used. Further documentation is located in the files with the implementation.
 
 # FINITE AUTOMATA
 
 This library supports **deterministic** and **nondeterministic** finite automata. You can find the implementation of these models in the module `automaton`. Consider the class located in the `base.py` as abstract, its only purpose is to avoid duplicity in the implementation of these models.
```

### Comparing `ib110hw-0.1.0/setup.py` & `ib110hw-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ib110hw",
-    version="0.1.0",
+    version="0.1.1",
     author="Martin Pilát",
     author_email="8pilatmartin8@gmail.com",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

### Comparing `ib110hw-0.1.0/src/ib110hw/automaton/base.py` & `ib110hw-0.1.1/src/ib110hw/automaton/base.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.0/src/ib110hw/automaton/dfa.py` & `ib110hw-0.1.1/src/ib110hw/automaton/dfa.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.0/src/ib110hw/automaton/nfa.py` & `ib110hw-0.1.1/src/ib110hw/automaton/nfa.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.0/src/ib110hw/automaton/utils.py` & `ib110hw-0.1.1/src/ib110hw/automaton/utils.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.0/src/ib110hw/turing/_helpers.py` & `ib110hw-0.1.1/src/ib110hw/turing/_helpers.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.0/src/ib110hw/turing/base.py` & `ib110hw-0.1.1/src/ib110hw/turing/base.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.0/src/ib110hw/turing/dtm.py` & `ib110hw-0.1.1/src/ib110hw/turing/dtm.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.0/src/ib110hw/turing/mtm.py` & `ib110hw-0.1.1/src/ib110hw/turing/mtm.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.0/src/ib110hw/turing/tape.py` & `ib110hw-0.1.1/src/ib110hw/turing/tape.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.0/src/ib110hw/turing/utils.py` & `ib110hw-0.1.1/src/ib110hw/turing/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -39,13 +39,8 @@
         initial_state=init,
         rej_states=rej,
         transitions=transitions,
     )
 
 
 if __name__ == "__main__":
-    machine = load_dtm_from_file("./turing/test.txt")
-    # machine.write_to_tape("abba")
-    # print(machine.tape)
-    # print(machine.transitions)
-
-    # machine.simulate()
+    pass
```

### Comparing `ib110hw-0.1.0/src/ib110hw.egg-info/PKG-INFO` & `ib110hw-0.1.1/src/ib110hw.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ib110hw
-Version: 0.1.0
+Version: 0.1.1
 Home-page: https://github.com/pilatmartin/ib110hw
 Author: Martin Pilát
 Author-email: 8pilatmartin8@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -16,22 +16,22 @@
 
 Using virtual environment is of course optional, but recommended.
 
 ```sh
 # Bash
 $ python3 -m venv <name> 
 $ source <name>/bin/activate
-$ pip install ib110hw_testing
+$ pip install ib110hw
 ```
 
 ```powershell
 # Windows Powershell
 PS> py -m venv <name> 
 PS> <name>\Scripts\Activate.ps1
-PS> pip install ib110hw_testing
+PS> pip install ib110hw
 ```
 
 Below is an overview of how these computational models can be used. Further documentation is located in the files with the implementation.
 
 # FINITE AUTOMATA
 
 This library supports **deterministic** and **nondeterministic** finite automata. You can find the implementation of these models in the module `automaton`. Consider the class located in the `base.py` as abstract, its only purpose is to avoid duplicity in the implementation of these models.
```

### Comparing `ib110hw-0.1.0/src/ib110hw.egg-info/SOURCES.txt` & `ib110hw-0.1.1/src/ib110hw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.0/tests/test_dfa.py` & `ib110hw-0.1.1/tests/test_dfa.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.0/tests/test_dtm.py` & `ib110hw-0.1.1/tests/test_dtm.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.0/tests/test_mtm.py` & `ib110hw-0.1.1/tests/test_mtm.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.0/tests/test_nfa.py` & `ib110hw-0.1.1/tests/test_nfa.py`

 * *Files identical despite different names*

