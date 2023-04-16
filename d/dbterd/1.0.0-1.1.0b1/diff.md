# Comparing `tmp/dbterd-1.0.0.tar.gz` & `tmp/dbterd-1.1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbterd-1.0.0.tar", max compression
+gzip compressed data, was "dbterd-1.1.0b1.tar", max compression
```

## Comparing `dbterd-1.0.0.tar` & `dbterd-1.1.0b1.tar`

### file list

```diff
@@ -1,31 +1,32 @@
--rw-r--r--   0        0        0     1067 2023-04-08 04:12:54.602296 dbterd-1.0.0/LICENSE
--rw-r--r--   0        0        0     4396 2023-04-08 04:12:54.602296 dbterd-1.0.0/README.md
--rw-r--r--   0        0        0        0 2023-04-08 04:12:54.610296 dbterd-1.0.0/dbterd/__init__.py
--rw-r--r--   0        0        0       37 2023-04-08 04:12:54.610296 dbterd-1.0.0/dbterd/__main__.py
--rw-r--r--   0        0        0        0 2023-04-08 04:12:54.610296 dbterd-1.0.0/dbterd/adapters/__init__.py
--rw-r--r--   0        0        0     1949 2023-04-08 04:12:54.610296 dbterd-1.0.0/dbterd/adapters/base.py
--rw-r--r--   0        0        0      344 2023-04-08 04:12:54.610296 dbterd-1.0.0/dbterd/adapters/factory.py
--rw-r--r--   0        0        0        0 2023-04-08 04:12:54.610296 dbterd-1.0.0/dbterd/adapters/targets/__init__.py
--rw-r--r--   0        0        0      281 2023-04-08 04:12:54.610296 dbterd-1.0.0/dbterd/adapters/targets/dbml/__init__.py
--rw-r--r--   0        0        0       72 2023-04-08 04:12:54.610296 dbterd-1.0.0/dbterd/adapters/targets/dbml/constants.py
--rw-r--r--   0        0        0        0 2023-04-08 04:12:54.610296 dbterd-1.0.0/dbterd/adapters/targets/dbml/engine/__init__.py
--rw-r--r--   0        0        0     6489 2023-04-08 04:12:54.610296 dbterd-1.0.0/dbterd/adapters/targets/dbml/engine/engine.py
--rw-r--r--   0        0        0      648 2023-04-08 04:12:54.610296 dbterd-1.0.0/dbterd/adapters/targets/dbml/engine/meta.py
--rw-r--r--   0        0        0        0 2023-04-08 04:12:54.610296 dbterd-1.0.0/dbterd/adapters/targets/dbml/strategies/__init__.py
--rw-r--r--   0        0        0      165 2023-04-08 04:12:54.610296 dbterd-1.0.0/dbterd/adapters/targets/dbml/strategies/dbml_test_relationship.py
--rw-r--r--   0        0        0       49 2023-04-08 04:12:54.610296 dbterd-1.0.0/dbterd/adapters/targets/dbml/strategies/default.py
--rw-r--r--   0        0        0      198 2023-04-08 04:12:54.610296 dbterd-1.0.0/dbterd/adapters/worker.py
--rw-r--r--   0        0        0        0 2023-04-08 04:12:54.610296 dbterd-1.0.0/dbterd/cli/__init__.py
--rw-r--r--   0        0        0     1732 2023-04-08 04:12:54.610296 dbterd-1.0.0/dbterd/cli/main.py
--rw-r--r--   0        0        0     2200 2023-04-08 04:12:54.610296 dbterd-1.0.0/dbterd/cli/params.py
--rw-r--r--   0        0        0      284 2023-04-08 04:12:54.610296 dbterd-1.0.0/dbterd/default.py
--rw-r--r--   0        0        0        0 2023-04-08 04:12:54.610296 dbterd-1.0.0/dbterd/helpers/__init__.py
--rw-r--r--   0        0        0      721 2023-04-08 04:12:54.610296 dbterd-1.0.0/dbterd/helpers/cli_messaging.py
--rw-r--r--   0        0        0      877 2023-04-08 04:12:54.610296 dbterd-1.0.0/dbterd/helpers/dict.py
--rw-r--r--   0        0        0     4076 2023-04-08 04:12:54.610296 dbterd-1.0.0/dbterd/helpers/file.py
--rw-r--r--   0        0        0     1022 2023-04-08 04:12:54.610296 dbterd-1.0.0/dbterd/helpers/jsonify.py
--rw-r--r--   0        0        0      976 2023-04-08 04:12:54.610296 dbterd-1.0.0/dbterd/helpers/log.py
--rw-r--r--   0        0        0     1605 2023-04-08 04:12:54.610296 dbterd-1.0.0/dbterd/helpers/yaml.py
--rw-r--r--   0        0        0       94 2023-04-08 04:12:54.610296 dbterd-1.0.0/dbterd/main.py
--rw-r--r--   0        0        0     2131 2023-04-08 04:13:12.910004 dbterd-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     5484 1970-01-01 00:00:00.000000 dbterd-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-16 06:29:54.505994 dbterd-1.1.0b1/LICENSE
+-rw-r--r--   0        0        0     4504 2023-04-16 06:29:54.505994 dbterd-1.1.0b1/README.md
+-rw-r--r--   0        0        0        0 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/__init__.py
+-rw-r--r--   0        0        0       37 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/adapters/algos/__init__.py
+-rw-r--r--   0        0        0      648 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/adapters/algos/meta.py
+-rw-r--r--   0        0        0     5833 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/adapters/algos/test_relationship.py
+-rw-r--r--   0        0        0     1997 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/adapters/base.py
+-rw-r--r--   0        0        0      344 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/adapters/factory.py
+-rw-r--r--   0        0        0        0 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/adapters/targets/__init__.py
+-rw-r--r--   0        0        0      132 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/adapters/targets/constants.py
+-rw-r--r--   0        0        0      304 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/adapters/targets/dbml/__init__.py
+-rw-r--r--   0        0        0      978 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/adapters/targets/dbml/dbml_test_relationship.py
+-rw-r--r--   0        0        0       49 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/adapters/targets/default.py
+-rw-r--r--   0        0        0      316 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/adapters/targets/mermaid/__init__.py
+-rw-r--r--   0        0        0     1190 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/adapters/targets/mermaid/mermaid_test_relationship.py
+-rw-r--r--   0        0        0      198 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/adapters/worker.py
+-rw-r--r--   0        0        0        0 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/cli/__init__.py
+-rw-r--r--   0        0        0     1732 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/cli/main.py
+-rw-r--r--   0        0        0     2200 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/cli/params.py
+-rw-r--r--   0        0        0      284 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/default.py
+-rw-r--r--   0        0        0        0 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/helpers/__init__.py
+-rw-r--r--   0        0        0      721 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/helpers/cli_messaging.py
+-rw-r--r--   0        0        0      877 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/helpers/dict.py
+-rw-r--r--   0        0        0     4076 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/helpers/file.py
+-rw-r--r--   0        0        0     1022 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/helpers/jsonify.py
+-rw-r--r--   0        0        0      976 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/helpers/log.py
+-rw-r--r--   0        0        0     1605 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/helpers/yaml.py
+-rw-r--r--   0        0        0       94 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/main.py
+-rw-r--r--   0        0        0     2133 2023-04-16 06:30:10.730031 dbterd-1.1.0b1/pyproject.toml
+-rw-r--r--   0        0        0     5594 1970-01-01 00:00:00.000000 dbterd-1.1.0b1/PKG-INFO
```

### Comparing `dbterd-1.0.0/LICENSE` & `dbterd-1.1.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbterd-1.0.0/README.md` & `dbterd-1.1.0b1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # dbterd
-CLI to generate DBML file from dbt artifact files (required: `manifest.json`, `catalog.json`)
+CLI to generate Diagram-as-a-code file ([DBML](https://dbdiagram.io/d), [Mermaid](https://mermaid-js.github.io/mermaid-live-editor/)) from dbt artifact files (required: `manifest.json`, `catalog.json`)
 > Version 0.1: only required `manifest.json`
 
 [![PyPI version](https://badge.fury.io/py/dbterd.svg)](https://pypi.org/project/dbterd/)
 ![python-cli](https://img.shields.io/badge/CLI-Python-FFCE3E?labelColor=14354C&logo=python&logoColor=white)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![python](https://img.shields.io/badge/Python-3.9|3.10|3.11-3776AB.svg?style=flat&logo=python&logoColor=white)](https://www.python.org)
 [![codecov](https://codecov.io/gh/datnguye/dbterd/branch/main/graph/badge.svg?token=N7DMQBLH4P)](https://codecov.io/gh/datnguye/dbterd)
```

### Comparing `dbterd-1.0.0/dbterd/adapters/base.py` & `dbterd-1.1.0b1/dbterd/adapters/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,26 +29,27 @@
 
     def __read_catalog(self, cp: str):
         cli_messaging.check_existence(cp, self.filename_catalog)
         with cli_messaging.handle_read_errors(self.filename_catalog):
             return file_handlers.read_catalog(cp)
 
     def __run_by_strategy(self, **kwargs):
-        target_module = factory.load_executor(name=kwargs["target"])
-        operation_dispatcher = getattr(target_module, "run_operation_dispatcher")
-        strategy_func = operation_dispatcher.get(
+        target = factory.load_executor(name=kwargs["target"])  # import {target}
+        run_operation_dispatcher = getattr(target, "run_operation_dispatcher")
+        operation_default = getattr(target, "run_operation_default")
+        operation = run_operation_dispatcher.get(
             f"{kwargs['target']}_{kwargs['algo']}",
-            getattr(target_module, "operation_default"),
+            operation_default,
         )
         manifest = self.__read_manifest(
             mp=kwargs.get("manifest_path") or kwargs["artifacts_dir"],
             mv=kwargs["manifest_version"],
         )
         catalog = self.__read_catalog(
             cp=kwargs.get("manifest_path") or kwargs["artifacts_dir"]
         )
 
-        result = strategy_func(manifest=manifest, catalog=catalog, **kwargs)
+        result = operation(manifest=manifest, catalog=catalog, **kwargs)
         path = kwargs["output"] + f"/{result[0]}"
         with open(path, "w") as f:
             logger.info(path)
             f.write(result[1])
```

### Comparing `dbterd-1.0.0/dbterd/adapters/targets/dbml/engine/engine.py` & `dbterd-1.1.0b1/dbterd/adapters/algos/test_relationship.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from dbterd.adapters.targets.dbml.engine.meta import Column, Ref, Table
+from dbterd.adapters.algos.meta import Column, Ref, Table
 
 
 def parse(manifest, catalog, **kwargs):
     # Parse Table
     tables = get_tables(manifest, catalog)
     # Apply selection
     select_rule = (kwargs.get("select") or "").lower().split(":")
-    resource_type_rule = kwargs.get("resource_type") or ""
+    resource_types = kwargs.get("resource_type") or ""
 
     def filter_table_select(table):
         if select_rule[0].startswith("schema"):
             schema = f"{table.database}.{table.schema}"
             return schema.startswith(select_rule[-1]) or table.schema.startswith(
                 select_rule[-1]
             )
         else:
             return table.name.startswith(select_rule[-1])
 
     tables = [table for table in tables if filter_table_select(table)]
-    tables = [table for table in tables if table.resource_type in resource_type_rule]
+    tables = [table for table in tables if table.resource_type in resource_types]
 
     # -- apply exclusion (take care of name only)
 
     exclude_rule = kwargs.get("exclude")
     if exclude_rule:
         tables = [table for table in tables if not table.name.startswith(exclude_rule)]
 
@@ -46,30 +46,15 @@
                 table.columns.append(Column(name=relationship.column_map[0]))
             if (
                 table.name == relationship.table_map[1]
                 and relationship.column_map[1].lower() not in table_columns
             ):
                 table.columns.append(Column(name=relationship.column_map[1]))
 
-    # Build DBML content
-    dbml = "//Tables (based on the selection criteria)\n"
-    for table in tables:
-        dbml += f"//--configured at schema: {table.database}.{table.schema}\n"
-        dbml += """Table \"{table}\" {{\n{columns}\n}}\n""".format(
-            table=table.name,
-            columns="\n".join([f'  "{x.name}" "{x.data_type}"' for x in table.columns]),
-        )
-
-    dbml += "//Refs (based on the DBT Relationship Tests)\n"
-    for rel in relationships:
-        key_from = f'"{rel.table_map[1]}"."{rel.column_map[1]}"'
-        key_to = f'"{rel.table_map[0]}"."{rel.column_map[0]}"'
-        dbml += f"Ref: {key_from} > {key_to}\n"
-
-    return dbml
+    return (tables, relationships)
 
 
 def get_tables(manifest, catalog):
     """Extract tables from dbt artifacts"""
 
     def create_table_and_columns(table_name, resource, catalog_resource=None):
         table = Table(
```

### Comparing `dbterd-1.0.0/dbterd/adapters/targets/dbml/engine/meta.py` & `dbterd-1.1.0b1/dbterd/adapters/algos/meta.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.0.0/dbterd/cli/main.py` & `dbterd-1.1.0b1/dbterd/cli/main.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.0.0/dbterd/cli/params.py` & `dbterd-1.1.0b1/dbterd/cli/params.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.0.0/dbterd/helpers/cli_messaging.py` & `dbterd-1.1.0b1/dbterd/helpers/cli_messaging.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.0.0/dbterd/helpers/dict.py` & `dbterd-1.1.0b1/dbterd/helpers/dict.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.0.0/dbterd/helpers/file.py` & `dbterd-1.1.0b1/dbterd/helpers/file.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.0.0/dbterd/helpers/jsonify.py` & `dbterd-1.1.0b1/dbterd/helpers/jsonify.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.0.0/dbterd/helpers/log.py` & `dbterd-1.1.0b1/dbterd/helpers/log.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.0.0/dbterd/helpers/yaml.py` & `dbterd-1.1.0b1/dbterd/helpers/yaml.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.0.0/pyproject.toml` & `dbterd-1.1.0b1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbterd"
-version = "1.0.0"
+version = "1.1.0b1"
 description = "dbterd is a Command Line Interface (CLI) to convert dbt manifest.json file to diagram file"
 authors = ["Dat Nguyen <datnguyen.it09@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/datnguye/dbterd"
 repository = "https://github.com/datnguye/dbterd"
 keywords = ["flake8", "markdown", "lint"]
```

### Comparing `dbterd-1.0.0/PKG-INFO` & `dbterd-1.1.0b1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbterd
-Version: 1.0.0
+Version: 1.1.0b1
 Summary: dbterd is a Command Line Interface (CLI) to convert dbt manifest.json file to diagram file
 Home-page: https://github.com/datnguye/dbterd
 License: MIT
 Keywords: flake8,markdown,lint
 Author: Dat Nguyen
 Author-email: datnguyen.it09@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -21,15 +21,15 @@
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: dbt-artifacts-parser (>=0.2.3,<0.3.0)
 Requires-Dist: sqlparse (>=0.4.3,<0.5.0)
 Project-URL: Repository, https://github.com/datnguye/dbterd
 Description-Content-Type: text/markdown
 
 # dbterd
-CLI to generate DBML file from dbt artifact files (required: `manifest.json`, `catalog.json`)
+CLI to generate Diagram-as-a-code file ([DBML](https://dbdiagram.io/d), [Mermaid](https://mermaid-js.github.io/mermaid-live-editor/)) from dbt artifact files (required: `manifest.json`, `catalog.json`)
 > Version 0.1: only required `manifest.json`
 
 [![PyPI version](https://badge.fury.io/py/dbterd.svg)](https://pypi.org/project/dbterd/)
 ![python-cli](https://img.shields.io/badge/CLI-Python-FFCE3E?labelColor=14354C&logo=python&logoColor=white)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![python](https://img.shields.io/badge/Python-3.9|3.10|3.11-3776AB.svg?style=flat&logo=python&logoColor=white)](https://www.python.org)
 [![codecov](https://codecov.io/gh/datnguye/dbterd/branch/main/graph/badge.svg?token=N7DMQBLH4P)](https://codecov.io/gh/datnguye/dbterd)
```

