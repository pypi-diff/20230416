# Comparing `tmp/synspace-0.2.0.tar.gz` & `tmp/synspace-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synspace-0.2.0.tar", last modified: Mon Jan 16 17:28:15 2023, max compression
+gzip compressed data, was "synspace-0.3.0.tar", last modified: Sat Apr 15 22:46:31 2023, max compression
```

## Comparing `synspace-0.2.0.tar` & `synspace-0.3.0.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 17:28:15.649895 synspace-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-01-16 17:25:19.000000 synspace-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-01-16 17:25:19.000000 synspace-0.2.0/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-01-16 17:28:15.645895 synspace-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-01-16 17:25:19.000000 synspace-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-16 17:28:15.649895 synspace-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-01-16 17:25:19.000000 synspace-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 17:28:15.645895 synspace-0.2.0/synspace/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-01-16 17:25:19.000000 synspace-0.2.0/synspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-01-16 17:25:19.000000 synspace-0.2.0/synspace/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-01-16 17:25:19.000000 synspace-0.2.0/synspace/draw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 17:28:15.645895 synspace-0.2.0/synspace/reos/
--rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-01-16 17:25:19.000000 synspace-0.2.0/synspace/reos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 17:28:15.645895 synspace-0.2.0/synspace/rxn_data/
--rw-r--r--   0 runner    (1001) docker     (123)  2671984 2023-01-16 17:25:19.000000 synspace-0.2.0/synspace/rxn_data/blocks.pk.bz2
--rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-01-16 17:25:19.000000 synspace-0.2.0/synspace/rxn_data/rxns.json
--rw-r--r--   0 runner    (1001) docker     (123)     7424 2023-01-16 17:25:19.000000 synspace-0.2.0/synspace/synspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-01-16 17:25:19.000000 synspace-0.2.0/synspace/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-16 17:25:19.000000 synspace-0.2.0/synspace/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 17:28:15.645895 synspace-0.2.0/synspace.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-01-16 17:28:15.000000 synspace-0.2.0/synspace.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-01-16 17:28:15.000000 synspace-0.2.0/synspace.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-16 17:28:15.000000 synspace-0.2.0/synspace.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-01-16 17:28:15.000000 synspace-0.2.0/synspace.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-16 17:28:15.000000 synspace-0.2.0/synspace.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 22:46:31.914486 synspace-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-15 22:43:33.000000 synspace-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-15 22:43:33.000000 synspace-0.3.0/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-15 22:46:31.914486 synspace-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-15 22:43:33.000000 synspace-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 22:46:31.914486 synspace-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-15 22:43:33.000000 synspace-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 22:46:31.910486 synspace-0.3.0/synspace/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-15 22:43:33.000000 synspace-0.3.0/synspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-04-15 22:43:33.000000 synspace-0.3.0/synspace/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-15 22:43:33.000000 synspace-0.3.0/synspace/draw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 22:46:31.910486 synspace-0.3.0/synspace/reos/
+-rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-04-15 22:43:33.000000 synspace-0.3.0/synspace/reos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 22:46:31.914486 synspace-0.3.0/synspace/rxn_data/
+-rw-r--r--   0 runner    (1001) docker     (123)  2671984 2023-04-15 22:43:33.000000 synspace-0.3.0/synspace/rxn_data/blocks.pk.bz2
+-rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-04-15 22:43:33.000000 synspace-0.3.0/synspace/rxn_data/rxns.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-04-15 22:43:33.000000 synspace-0.3.0/synspace/synspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-04-15 22:43:33.000000 synspace-0.3.0/synspace/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-15 22:43:33.000000 synspace-0.3.0/synspace/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 22:46:31.910486 synspace-0.3.0/synspace.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-15 22:46:31.000000 synspace-0.3.0/synspace.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-15 22:46:31.000000 synspace-0.3.0/synspace.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 22:46:31.000000 synspace-0.3.0/synspace.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-15 22:46:31.000000 synspace-0.3.0/synspace.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-15 22:46:31.000000 synspace-0.3.0/synspace.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 22:46:31.914486 synspace-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-04-15 22:43:33.000000 synspace-0.3.0/tests/test_syngen.py
```

### Comparing `synspace-0.2.0/LICENSE` & `synspace-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `synspace-0.2.0/PKG-INFO` & `synspace-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synspace
-Version: 0.2.0
+Version: 0.3.0
 Summary: Generative model based on forward synthesis rules
 Home-page: https://github.com/whitead/synspace
 Author: Andrew White
 Author-email: andrew.white@rochester.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -15,15 +15,15 @@
 
 # synspace
 
 **This is early-stage code that is in progress. It is in flux**
 
 This package generates a local chemical space around a given molecule using retro and forward synthesis rules. The reactions used are the 50 robust medchem reactions proposed by [Hartenfeller et al.](https://pubs.acs.org/doi/10.1021/ci200379p). The retrosynthesis is done either via [PostEra Mannifold](https://postera.ai/) if you have an API key, or by reversing the 50 robust reactions. The purchasable building blocks come from the [Purchasable Mcule supplier building block catalogs](https://mcule.com/database/). All of these things can be customized though. 
 
-<img src="https://user-images.githubusercontent.com/908389/210176534-028fb745-0114-4697-aad7-bfe14f1e9360.png" alt="chemical space showing a molecule space that is predicted not to cross the blood brain barrier along with three synthetically feasible modifications" width=500>
+<img src="https://user-images.githubusercontent.com/908389/212747862-577182f2-a880-46ec-a0e1-33fe7f5d9987.png" alt="chemical space showing a molecule space that is predicted not to cross the blood brain barrier along with three synthetically feasible modifications" width=500>
 
 
 ## Installation
 
 ```sh
 pip install synspace
 ```
```

### Comparing `synspace-0.2.0/README.md` & `synspace-0.3.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # synspace
 
 **This is early-stage code that is in progress. It is in flux**
 
 This package generates a local chemical space around a given molecule using retro and forward synthesis rules. The reactions used are the 50 robust medchem reactions proposed by [Hartenfeller et al.](https://pubs.acs.org/doi/10.1021/ci200379p). The retrosynthesis is done either via [PostEra Mannifold](https://postera.ai/) if you have an API key, or by reversing the 50 robust reactions. The purchasable building blocks come from the [Purchasable Mcule supplier building block catalogs](https://mcule.com/database/). All of these things can be customized though. 
 
-<img src="https://user-images.githubusercontent.com/908389/210176534-028fb745-0114-4697-aad7-bfe14f1e9360.png" alt="chemical space showing a molecule space that is predicted not to cross the blood brain barrier along with three synthetically feasible modifications" width=500>
+<img src="https://user-images.githubusercontent.com/908389/212747862-577182f2-a880-46ec-a0e1-33fe7f5d9987.png" alt="chemical space showing a molecule space that is predicted not to cross the blood brain barrier along with three synthetically feasible modifications" width=500>
 
 
 ## Installation
 
 ```sh
 pip install synspace
 ```
```

### Comparing `synspace-0.2.0/setup.py` & `synspace-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `synspace-0.2.0/synspace/data.py` & `synspace-0.3.0/synspace/data.py`

 * *Files identical despite different names*

### Comparing `synspace-0.2.0/synspace/draw.py` & `synspace-0.3.0/synspace/draw.py`

 * *Files identical despite different names*

### Comparing `synspace-0.2.0/synspace/reos/__init__.py` & `synspace-0.3.0/synspace/reos/__init__.py`

 * *Files identical despite different names*

### Comparing `synspace-0.2.0/synspace/rxn_data/blocks.pk.bz2` & `synspace-0.3.0/synspace/rxn_data/blocks.pk.bz2`

 * *Files identical despite different names*

### Comparing `synspace-0.2.0/synspace/rxn_data/rxns.json` & `synspace-0.3.0/synspace/rxn_data/rxns.json`

 * *Files identical despite different names*

### Comparing `synspace-0.2.0/synspace/synspace.py` & `synspace-0.3.0/synspace/synspace.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,42 +20,46 @@
     filter=True,
     _pbar=None,
 ):
     if type(mol) == str:
         mol = Chem.MolFromSmiles(mol)
     if type(steps) == int:
         steps = (0, steps)
+    mols, props = None, None
     if use_mannifold is None:
         use_mannifold = os.environ.get("POSTERA_API_KEY") is not None
     if use_mannifold:
         if _pbar:
             _pbar.set_description("⚗️Synspace Retrosynthesis (Mannifold)⚗️")
         mols, props = mannifold_retro(mol)
     else:
-        if _pbar:
+        if _pbar and steps[0] > 0:
             _pbar.set_description("⚗️Synspace Retrosynthesis...⚗️")
-        mols, props = retro(mol, rxns=rxns, strict=False if strict is None else strict)
-        for _ in range(steps[0] - 1):
+        if steps[0] > 0:
+            mols, props = retro(mol, rxns=rxns, strict=False if strict is None else strict)
+        for _ in range(steps[0]-1):
             to_add = []
             for m, p in zip(mols, props):
                 ms, ps = retro(
                     m,
                     rxns=rxns,
                     strict=False if strict is None else strict,
                     start_props=p,
                 )
                 to_add.append((ms, ps))
             for m, p in to_add:
                 mols.extend(m)
                 props.extend(p)
                 if _pbar:
                     _pbar.update(len(mols))
-        mols, props = remove_dups(mols, props)
+            mols, props = remove_dups(mols, props) 
     if _pbar:
         _pbar.set_description("⚗️Forward synthesis...⚗️")
+    if mols is None:
+        mols, props = [mol], [{"rxn-name": "", "rxn": "", "match": ()}]
     for i in range(steps[1]):
         to_add = []
         for m, p in zip(mols, props):
             ms, ps = forward(
                 m,
                 blocks=blocks,
                 samples=nblocks,
@@ -70,15 +74,16 @@
             props.extend(p)
         # poor estimate that we can allow 1/steps *  threshold for each step
         mols, props = sort_mols(
             *remove_dups(mols, props),
             mol,
             threshold=threshold / steps[1] if i < steps[1] - 1 else threshold,
         )
-        mols, props = reos_filter(mols, props)
+        if filter:
+            mols, props = reos_filter(mols, props)
         mols, props = mols[:num_samples], props[:num_samples]
         if _pbar:
             _pbar.update(len(mols))
     return mols, props
 
 
 def mannifold_retro(query_mol):
@@ -208,14 +213,14 @@
             if len(p) == 1 or (len(p) > 0 and not strict):
                 rsmi = ".".join([Chem.MolToSmiles(r) for r in reactants])
                 for m, s in extract(p):
                     out.append(m)
                     props.append(
                         {
                             "rxn-name": n.replace("_", " "),
-                            "rxn": f"{s}>>{smi}",
+                            "rxn": f"{rsmi}>>{s}",
                             "match": match,
                         }
                     )
                     if start_props:
                         merge_props(start_props, props[-1])
     return [mol] + out, [{"rxn-name": "", "rxn": "", "match": ()}] + props
```

### Comparing `synspace-0.2.0/synspace/utils.py` & `synspace-0.3.0/synspace/utils.py`

 * *Files identical despite different names*

### Comparing `synspace-0.2.0/synspace.egg-info/PKG-INFO` & `synspace-0.3.0/synspace.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synspace
-Version: 0.2.0
+Version: 0.3.0
 Summary: Generative model based on forward synthesis rules
 Home-page: https://github.com/whitead/synspace
 Author: Andrew White
 Author-email: andrew.white@rochester.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -15,15 +15,15 @@
 
 # synspace
 
 **This is early-stage code that is in progress. It is in flux**
 
 This package generates a local chemical space around a given molecule using retro and forward synthesis rules. The reactions used are the 50 robust medchem reactions proposed by [Hartenfeller et al.](https://pubs.acs.org/doi/10.1021/ci200379p). The retrosynthesis is done either via [PostEra Mannifold](https://postera.ai/) if you have an API key, or by reversing the 50 robust reactions. The purchasable building blocks come from the [Purchasable Mcule supplier building block catalogs](https://mcule.com/database/). All of these things can be customized though. 
 
-<img src="https://user-images.githubusercontent.com/908389/210176534-028fb745-0114-4697-aad7-bfe14f1e9360.png" alt="chemical space showing a molecule space that is predicted not to cross the blood brain barrier along with three synthetically feasible modifications" width=500>
+<img src="https://user-images.githubusercontent.com/908389/212747862-577182f2-a880-46ec-a0e1-33fe7f5d9987.png" alt="chemical space showing a molecule space that is predicted not to cross the blood brain barrier along with three synthetically feasible modifications" width=500>
 
 
 ## Installation
 
 ```sh
 pip install synspace
 ```
```

