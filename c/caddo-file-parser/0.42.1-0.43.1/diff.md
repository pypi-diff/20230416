# Comparing `tmp/caddo-file-parser-0.42.1.tar.gz` & `tmp/caddo-file-parser-0.43.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caddo-file-parser-0.42.1.tar", last modified: Sun Apr 16 13:46:47 2023, max compression
+gzip compressed data, was "caddo-file-parser-0.43.1.tar", last modified: Sun Apr 16 14:54:13 2023, max compression
```

## Comparing `caddo-file-parser-0.42.1.tar` & `caddo-file-parser-0.43.1.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:46:47.916298 caddo-file-parser-0.42.1/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-16 13:46:47.912298 caddo-file-parser-0.42.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-16 13:46:36.000000 caddo-file-parser-0.42.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:46:47.912298 caddo-file-parser-0.42.1/caddo_file_parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 13:46:36.000000 caddo-file-parser-0.42.1/caddo_file_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-04-16 13:46:36.000000 caddo-file-parser-0.42.1/caddo_file_parser/caddo_file_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:46:47.912298 caddo-file-parser-0.42.1/caddo_file_parser/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 13:46:36.000000 caddo-file-parser-0.42.1/caddo_file_parser/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-16 13:46:36.000000 caddo-file-parser-0.42.1/caddo_file_parser/models/caddo_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 13:46:36.000000 caddo-file-parser-0.42.1/caddo_file_parser/models/index_set.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-16 13:46:36.000000 caddo-file-parser-0.42.1/caddo_file_parser/models/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:46:47.912298 caddo-file-parser-0.42.1/caddo_file_parser/settings/
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-16 13:46:36.000000 caddo-file-parser-0.42.1/caddo_file_parser/settings/generation_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-16 13:46:36.000000 caddo-file-parser-0.42.1/caddo_file_parser/settings/generation_settings_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:46:47.912298 caddo-file-parser-0.42.1/caddo_file_parser/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 13:46:36.000000 caddo-file-parser-0.42.1/caddo_file_parser/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-16 13:46:36.000000 caddo-file-parser-0.42.1/caddo_file_parser/test/file_reading_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-16 13:46:36.000000 caddo-file-parser-0.42.1/caddo_file_parser/test/file_saving_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-16 13:46:36.000000 caddo-file-parser-0.42.1/caddo_file_parser/test/settings_loader_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:46:47.912298 caddo-file-parser-0.42.1/caddo_file_parser/validation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 13:46:36.000000 caddo-file-parser-0.42.1/caddo_file_parser/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8981 2023-04-16 13:46:36.000000 caddo-file-parser-0.42.1/caddo_file_parser/validation/caddo_file_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-16 13:46:36.000000 caddo-file-parser-0.42.1/caddo_file_parser/validation/settings_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:46:47.912298 caddo-file-parser-0.42.1/caddo_file_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-16 13:46:47.000000 caddo-file-parser-0.42.1/caddo_file_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-16 13:46:47.000000 caddo-file-parser-0.42.1/caddo_file_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 13:46:47.000000 caddo-file-parser-0.42.1/caddo_file_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-16 13:46:47.000000 caddo-file-parser-0.42.1/caddo_file_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-16 13:46:47.000000 caddo-file-parser-0.42.1/caddo_file_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-16 13:46:36.000000 caddo-file-parser-0.42.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 13:46:47.916298 caddo-file-parser-0.42.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:54:13.318815 caddo-file-parser-0.43.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-16 14:54:13.318815 caddo-file-parser-0.43.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-16 14:53:58.000000 caddo-file-parser-0.43.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-16 14:53:58.000000 caddo-file-parser-0.43.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 14:54:13.322815 caddo-file-parser-0.43.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:54:13.314815 caddo-file-parser-0.43.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:54:13.318815 caddo-file-parser-0.43.1/src/caddo_file_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 14:53:58.000000 caddo-file-parser-0.43.1/src/caddo_file_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6978 2023-04-16 14:53:58.000000 caddo-file-parser-0.43.1/src/caddo_file_parser/caddo_file_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:54:13.318815 caddo-file-parser-0.43.1/src/caddo_file_parser/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 14:53:58.000000 caddo-file-parser-0.43.1/src/caddo_file_parser/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-16 14:53:58.000000 caddo-file-parser-0.43.1/src/caddo_file_parser/models/caddo_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 14:53:58.000000 caddo-file-parser-0.43.1/src/caddo_file_parser/models/index_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-16 14:53:58.000000 caddo-file-parser-0.43.1/src/caddo_file_parser/models/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:54:13.318815 caddo-file-parser-0.43.1/src/caddo_file_parser/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-16 14:53:58.000000 caddo-file-parser-0.43.1/src/caddo_file_parser/settings/generation_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-16 14:53:58.000000 caddo-file-parser-0.43.1/src/caddo_file_parser/settings/generation_settings_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:54:13.318815 caddo-file-parser-0.43.1/src/caddo_file_parser/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 14:53:58.000000 caddo-file-parser-0.43.1/src/caddo_file_parser/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-16 14:53:58.000000 caddo-file-parser-0.43.1/src/caddo_file_parser/test/file_reading_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-16 14:53:58.000000 caddo-file-parser-0.43.1/src/caddo_file_parser/test/file_saving_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-16 14:53:58.000000 caddo-file-parser-0.43.1/src/caddo_file_parser/test/settings_loader_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:54:13.318815 caddo-file-parser-0.43.1/src/caddo_file_parser/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 14:53:58.000000 caddo-file-parser-0.43.1/src/caddo_file_parser/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8981 2023-04-16 14:53:58.000000 caddo-file-parser-0.43.1/src/caddo_file_parser/validation/caddo_file_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-16 14:53:58.000000 caddo-file-parser-0.43.1/src/caddo_file_parser/validation/settings_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:54:13.318815 caddo-file-parser-0.43.1/src/caddo_file_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-16 14:54:13.000000 caddo-file-parser-0.43.1/src/caddo_file_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-16 14:54:13.000000 caddo-file-parser-0.43.1/src/caddo_file_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 14:54:13.000000 caddo-file-parser-0.43.1/src/caddo_file_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-16 14:54:13.000000 caddo-file-parser-0.43.1/src/caddo_file_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-16 14:54:13.000000 caddo-file-parser-0.43.1/src/caddo_file_parser.egg-info/top_level.txt
```

### Comparing `caddo-file-parser-0.42.1/caddo_file_parser/caddo_file_parser.py` & `caddo-file-parser-0.43.1/src/caddo_file_parser/caddo_file_parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -63,39 +63,41 @@
             with open(f"index_set_{index_set_number}_run_{run.number}.yaml", 'w') as file:
                 yaml.dump(file_content, file, Dumper=Dumper, default_flow_style=False)
 
     def copy_file(self, from_path, new_file_name):
         try:
             shutil.copy2(from_path, new_file_name)
         except:
-            print(f"{new_file_name} already exists in current directory""")
+            print(f"{new_file_name} already exists in current directory")
 
     def pack_to_caddo_file(self, caddo_file):
         filenames = []
         for run in caddo_file.runs:
             filenames += [f"index_set_{index_set.number}_run_{run.number}.yaml" for index_set in run.index_sets]
         self.copy_file(caddo_file.settings.data_settings_file_path, "settings.yaml")
         self.copy_file(caddo_file.settings.data_splitting_folding_seeds_file_path, "seeds.yaml")
         self.copy_file(caddo_file.settings.data_input_path, "data.csv")
 
         filenames += ["data.csv"] + ['settings.yaml'] + ["seeds.yaml"]
         with zipfile.ZipFile(f"{caddo_file.settings.data_output_file_name}.caddo", "w") as archive:
             for filename in filenames:
                 archive.write(filename)
 
+    def remove_if_file_was_copied_to_working_dir(self, settings_file_path, file_name):
+        if settings_file_path != file_name and settings_file_path != f"./{file_name}":
+            os.remove(file_name)
+
     def remove_unused_file(self, caddo_file):
         for run in caddo_file.runs:
             filenames = [f"index_set_{index_set.number}_run_{run.number}.yaml" for index_set in run.index_sets]
             for file in filenames:
                 os.remove(file)
-        os.remove("data.csv")
-        os.remove('settings.yaml')
-        if caddo_file.settings.data_splitting_folding_seeds_file_path != "seeds.yaml" \
-                and caddo_file.settings.data_settings_file_path != "./seeds.yaml":
-            os.remove("seeds.yaml")
+        self.remove_if_file_was_copied_to_working_dir(caddo_file.settings.data_splitting_folding_seeds_file_path, "seeds.yaml")
+        self.remove_if_file_was_copied_to_working_dir(caddo_file.settings.data_settings_file_path, "settings.yaml")
+        self.remove_if_file_was_copied_to_working_dir(caddo_file.settings.data_input_path, "data.csv")
 
     def read_data(self, file_name) -> CaddoFile:
         with zipfile.ZipFile(file_name + ".caddo", "r") as zf:
             generation_settings = self.read_settings(zf)
             data = self.read_csv_data(zf, generation_settings)
             runs = self.read_runs(zf, generation_settings)
             seeds = self.read_seeds_from_zip(zf, generation_settings)
```

### Comparing `caddo-file-parser-0.42.1/caddo_file_parser/models/index_set.py` & `caddo-file-parser-0.43.1/src/caddo_file_parser/models/index_set.py`

 * *Files identical despite different names*

### Comparing `caddo-file-parser-0.42.1/caddo_file_parser/settings/generation_settings.py` & `caddo-file-parser-0.43.1/src/caddo_file_parser/settings/generation_settings.py`

 * *Files identical despite different names*

### Comparing `caddo-file-parser-0.42.1/caddo_file_parser/settings/generation_settings_loader.py` & `caddo-file-parser-0.43.1/src/caddo_file_parser/settings/generation_settings_loader.py`

 * *Files identical despite different names*

### Comparing `caddo-file-parser-0.42.1/caddo_file_parser/test/file_saving_test.py` & `caddo-file-parser-0.43.1/src/caddo_file_parser/test/file_saving_test.py`

 * *Files identical despite different names*

### Comparing `caddo-file-parser-0.42.1/caddo_file_parser/validation/caddo_file_validator.py` & `caddo-file-parser-0.43.1/src/caddo_file_parser/validation/caddo_file_validator.py`

 * *Files identical despite different names*

### Comparing `caddo-file-parser-0.42.1/caddo_file_parser/validation/settings_validator.py` & `caddo-file-parser-0.43.1/src/caddo_file_parser/validation/settings_validator.py`

 * *Files identical despite different names*

### Comparing `caddo-file-parser-0.42.1/caddo_file_parser.egg-info/SOURCES.txt` & `caddo-file-parser-0.43.1/src/caddo_file_parser.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 README.md
 pyproject.toml
-caddo_file_parser/__init__.py
-caddo_file_parser/caddo_file_parser.py
-caddo_file_parser.egg-info/PKG-INFO
-caddo_file_parser.egg-info/SOURCES.txt
-caddo_file_parser.egg-info/dependency_links.txt
-caddo_file_parser.egg-info/requires.txt
-caddo_file_parser.egg-info/top_level.txt
-caddo_file_parser/models/__init__.py
-caddo_file_parser/models/caddo_file.py
-caddo_file_parser/models/index_set.py
-caddo_file_parser/models/run.py
-caddo_file_parser/settings/generation_settings.py
-caddo_file_parser/settings/generation_settings_loader.py
-caddo_file_parser/test/__init__.py
-caddo_file_parser/test/file_reading_test.py
-caddo_file_parser/test/file_saving_test.py
-caddo_file_parser/test/settings_loader_test.py
-caddo_file_parser/validation/__init__.py
-caddo_file_parser/validation/caddo_file_validator.py
-caddo_file_parser/validation/settings_validator.py
+setup.cfg
+src/caddo_file_parser/__init__.py
+src/caddo_file_parser/caddo_file_parser.py
+src/caddo_file_parser.egg-info/PKG-INFO
+src/caddo_file_parser.egg-info/SOURCES.txt
+src/caddo_file_parser.egg-info/dependency_links.txt
+src/caddo_file_parser.egg-info/requires.txt
+src/caddo_file_parser.egg-info/top_level.txt
+src/caddo_file_parser/models/__init__.py
+src/caddo_file_parser/models/caddo_file.py
+src/caddo_file_parser/models/index_set.py
+src/caddo_file_parser/models/run.py
+src/caddo_file_parser/settings/generation_settings.py
+src/caddo_file_parser/settings/generation_settings_loader.py
+src/caddo_file_parser/test/__init__.py
+src/caddo_file_parser/test/file_reading_test.py
+src/caddo_file_parser/test/file_saving_test.py
+src/caddo_file_parser/test/settings_loader_test.py
+src/caddo_file_parser/validation/__init__.py
+src/caddo_file_parser/validation/caddo_file_validator.py
+src/caddo_file_parser/validation/settings_validator.py
```

