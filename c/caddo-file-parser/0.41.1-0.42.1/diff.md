# Comparing `tmp/caddo-file-parser-0.41.1.tar.gz` & `tmp/caddo-file-parser-0.42.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caddo-file-parser-0.41.1.tar", last modified: Mon Apr  3 15:01:28 2023, max compression
+gzip compressed data, was "caddo-file-parser-0.42.1.tar", last modified: Sun Apr 16 13:46:47 2023, max compression
```

## Comparing `caddo-file-parser-0.41.1.tar` & `caddo-file-parser-0.42.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:01:28.984217 caddo-file-parser-0.41.1/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-03 15:01:28.984217 caddo-file-parser-0.41.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-03 15:01:17.000000 caddo-file-parser-0.41.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:01:28.984217 caddo-file-parser-0.41.1/caddo_file_parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 15:01:17.000000 caddo-file-parser-0.41.1/caddo_file_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-04-03 15:01:17.000000 caddo-file-parser-0.41.1/caddo_file_parser/caddo_file_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:01:28.984217 caddo-file-parser-0.41.1/caddo_file_parser/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 15:01:17.000000 caddo-file-parser-0.41.1/caddo_file_parser/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-03 15:01:17.000000 caddo-file-parser-0.41.1/caddo_file_parser/models/caddo_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-03 15:01:17.000000 caddo-file-parser-0.41.1/caddo_file_parser/models/index_set.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-03 15:01:17.000000 caddo-file-parser-0.41.1/caddo_file_parser/models/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:01:28.984217 caddo-file-parser-0.41.1/caddo_file_parser/settings/
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-03 15:01:17.000000 caddo-file-parser-0.41.1/caddo_file_parser/settings/generation_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-03 15:01:17.000000 caddo-file-parser-0.41.1/caddo_file_parser/settings/generation_settings_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:01:28.984217 caddo-file-parser-0.41.1/caddo_file_parser/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 15:01:17.000000 caddo-file-parser-0.41.1/caddo_file_parser/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-03 15:01:17.000000 caddo-file-parser-0.41.1/caddo_file_parser/test/file_reading_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-03 15:01:17.000000 caddo-file-parser-0.41.1/caddo_file_parser/test/file_saving_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-03 15:01:17.000000 caddo-file-parser-0.41.1/caddo_file_parser/test/settings_loader_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:01:28.984217 caddo-file-parser-0.41.1/caddo_file_parser/validation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 15:01:17.000000 caddo-file-parser-0.41.1/caddo_file_parser/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8981 2023-04-03 15:01:17.000000 caddo-file-parser-0.41.1/caddo_file_parser/validation/caddo_file_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-03 15:01:17.000000 caddo-file-parser-0.41.1/caddo_file_parser/validation/settings_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 15:01:28.984217 caddo-file-parser-0.41.1/caddo_file_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-03 15:01:28.000000 caddo-file-parser-0.41.1/caddo_file_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-03 15:01:28.000000 caddo-file-parser-0.41.1/caddo_file_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 15:01:28.000000 caddo-file-parser-0.41.1/caddo_file_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-03 15:01:28.000000 caddo-file-parser-0.41.1/caddo_file_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-03 15:01:28.000000 caddo-file-parser-0.41.1/caddo_file_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-03 15:01:17.000000 caddo-file-parser-0.41.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 15:01:28.984217 caddo-file-parser-0.41.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:46:47.916298 caddo-file-parser-0.42.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-16 13:46:47.912298 caddo-file-parser-0.42.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-16 13:46:36.000000 caddo-file-parser-0.42.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:46:47.912298 caddo-file-parser-0.42.1/caddo_file_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 13:46:36.000000 caddo-file-parser-0.42.1/caddo_file_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-04-16 13:46:36.000000 caddo-file-parser-0.42.1/caddo_file_parser/caddo_file_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:46:47.912298 caddo-file-parser-0.42.1/caddo_file_parser/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 13:46:36.000000 caddo-file-parser-0.42.1/caddo_file_parser/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-16 13:46:36.000000 caddo-file-parser-0.42.1/caddo_file_parser/models/caddo_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 13:46:36.000000 caddo-file-parser-0.42.1/caddo_file_parser/models/index_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-16 13:46:36.000000 caddo-file-parser-0.42.1/caddo_file_parser/models/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:46:47.912298 caddo-file-parser-0.42.1/caddo_file_parser/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-16 13:46:36.000000 caddo-file-parser-0.42.1/caddo_file_parser/settings/generation_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-16 13:46:36.000000 caddo-file-parser-0.42.1/caddo_file_parser/settings/generation_settings_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:46:47.912298 caddo-file-parser-0.42.1/caddo_file_parser/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 13:46:36.000000 caddo-file-parser-0.42.1/caddo_file_parser/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-16 13:46:36.000000 caddo-file-parser-0.42.1/caddo_file_parser/test/file_reading_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-16 13:46:36.000000 caddo-file-parser-0.42.1/caddo_file_parser/test/file_saving_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-16 13:46:36.000000 caddo-file-parser-0.42.1/caddo_file_parser/test/settings_loader_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:46:47.912298 caddo-file-parser-0.42.1/caddo_file_parser/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 13:46:36.000000 caddo-file-parser-0.42.1/caddo_file_parser/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8981 2023-04-16 13:46:36.000000 caddo-file-parser-0.42.1/caddo_file_parser/validation/caddo_file_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-16 13:46:36.000000 caddo-file-parser-0.42.1/caddo_file_parser/validation/settings_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:46:47.912298 caddo-file-parser-0.42.1/caddo_file_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-16 13:46:47.000000 caddo-file-parser-0.42.1/caddo_file_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-16 13:46:47.000000 caddo-file-parser-0.42.1/caddo_file_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 13:46:47.000000 caddo-file-parser-0.42.1/caddo_file_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-16 13:46:47.000000 caddo-file-parser-0.42.1/caddo_file_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-16 13:46:47.000000 caddo-file-parser-0.42.1/caddo_file_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-16 13:46:36.000000 caddo-file-parser-0.42.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 13:46:47.916298 caddo-file-parser-0.42.1/setup.cfg
```

### Comparing `caddo-file-parser-0.41.1/caddo_file_parser/caddo_file_parser.py` & `caddo-file-parser-0.42.1/caddo_file_parser/caddo_file_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,19 +59,28 @@
                 "train_indexes": train_indexes,
                 "test_indexes": test_indexes,
                 "seed": seed
             }
             with open(f"index_set_{index_set_number}_run_{run.number}.yaml", 'w') as file:
                 yaml.dump(file_content, file, Dumper=Dumper, default_flow_style=False)
 
+    def copy_file(self, from_path, new_file_name):
+        try:
+            shutil.copy2(from_path, new_file_name)
+        except:
+            print(f"{new_file_name} already exists in current directory""")
+
     def pack_to_caddo_file(self, caddo_file):
         filenames = []
         for run in caddo_file.runs:
             filenames += [f"index_set_{index_set.number}_run_{run.number}.yaml" for index_set in run.index_sets]
-        shutil.copy2(caddo_file.settings.data_settings_file_path, 'settings.yaml')
+        self.copy_file(caddo_file.settings.data_settings_file_path, "settings.yaml")
+        self.copy_file(caddo_file.settings.data_splitting_folding_seeds_file_path, "seeds.yaml")
+        self.copy_file(caddo_file.settings.data_input_path, "data.csv")
+
         filenames += ["data.csv"] + ['settings.yaml'] + ["seeds.yaml"]
         with zipfile.ZipFile(f"{caddo_file.settings.data_output_file_name}.caddo", "w") as archive:
             for filename in filenames:
                 archive.write(filename)
 
     def remove_unused_file(self, caddo_file):
         for run in caddo_file.runs:
```

### Comparing `caddo-file-parser-0.41.1/caddo_file_parser/models/index_set.py` & `caddo-file-parser-0.42.1/caddo_file_parser/models/index_set.py`

 * *Files identical despite different names*

### Comparing `caddo-file-parser-0.41.1/caddo_file_parser/settings/generation_settings.py` & `caddo-file-parser-0.42.1/caddo_file_parser/settings/generation_settings.py`

 * *Files identical despite different names*

### Comparing `caddo-file-parser-0.41.1/caddo_file_parser/settings/generation_settings_loader.py` & `caddo-file-parser-0.42.1/caddo_file_parser/settings/generation_settings_loader.py`

 * *Files identical despite different names*

### Comparing `caddo-file-parser-0.41.1/caddo_file_parser/test/file_saving_test.py` & `caddo-file-parser-0.42.1/caddo_file_parser/test/file_saving_test.py`

 * *Files identical despite different names*

### Comparing `caddo-file-parser-0.41.1/caddo_file_parser/validation/caddo_file_validator.py` & `caddo-file-parser-0.42.1/caddo_file_parser/validation/caddo_file_validator.py`

 * *Files identical despite different names*

### Comparing `caddo-file-parser-0.41.1/caddo_file_parser/validation/settings_validator.py` & `caddo-file-parser-0.42.1/caddo_file_parser/validation/settings_validator.py`

 * *Files identical despite different names*

### Comparing `caddo-file-parser-0.41.1/caddo_file_parser.egg-info/SOURCES.txt` & `caddo-file-parser-0.42.1/caddo_file_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

