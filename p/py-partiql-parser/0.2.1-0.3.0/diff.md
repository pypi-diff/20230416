# Comparing `tmp/py-partiql-parser-0.2.1.tar.gz` & `tmp/py-partiql-parser-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-partiql-parser-0.2.1.tar", last modified: Thu Apr 13 22:55:42 2023, max compression
+gzip compressed data, was "py-partiql-parser-0.3.0.tar", last modified: Sun Apr 16 13:50:03 2023, max compression
```

## Comparing `py-partiql-parser-0.2.1.tar` & `py-partiql-parser-0.3.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:55:42.781393 py-partiql-parser-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-13 22:55:24.000000 py-partiql-parser-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-04-13 22:55:42.777392 py-partiql-parser-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-13 22:55:24.000000 py-partiql-parser-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:55:42.777392 py-partiql-parser-0.2.1/py_partiql_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-13 22:55:24.000000 py-partiql-parser-0.2.1/py_partiql_parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:55:42.777392 py-partiql-parser-0.2.1/py_partiql_parser/_internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 22:55:24.000000 py-partiql-parser-0.2.1/py_partiql_parser/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-13 22:55:24.000000 py-partiql-parser-0.2.1/py_partiql_parser/_internal/case_insensitive_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-13 22:55:24.000000 py-partiql-parser-0.2.1/py_partiql_parser/_internal/clause_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-13 22:55:24.000000 py-partiql-parser-0.2.1/py_partiql_parser/_internal/csv_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-13 22:55:24.000000 py-partiql-parser-0.2.1/py_partiql_parser/_internal/from_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-04-13 22:55:24.000000 py-partiql-parser-0.2.1/py_partiql_parser/_internal/json_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-04-13 22:55:24.000000 py-partiql-parser-0.2.1/py_partiql_parser/_internal/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-04-13 22:55:24.000000 py-partiql-parser-0.2.1/py_partiql_parser/_internal/select_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-04-13 22:55:24.000000 py-partiql-parser-0.2.1/py_partiql_parser/_internal/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-04-13 22:55:24.000000 py-partiql-parser-0.2.1/py_partiql_parser/_internal/where_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:55:42.777392 py-partiql-parser-0.2.1/py_partiql_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-04-13 22:55:42.000000 py-partiql-parser-0.2.1/py_partiql_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-13 22:55:42.000000 py-partiql-parser-0.2.1/py_partiql_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 22:55:42.000000 py-partiql-parser-0.2.1/py_partiql_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-13 22:55:42.000000 py-partiql-parser-0.2.1/py_partiql_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-13 22:55:42.000000 py-partiql-parser-0.2.1/py_partiql_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-13 22:55:35.000000 py-partiql-parser-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 22:55:42.781393 py-partiql-parser-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:55:42.777392 py-partiql-parser-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-04-13 22:55:24.000000 py-partiql-parser-0.2.1/tests/test_aws_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-04-13 22:55:24.000000 py-partiql-parser-0.2.1/tests/test_csv_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-13 22:55:24.000000 py-partiql-parser-0.2.1/tests/test_dynamodb_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-13 22:55:24.000000 py-partiql-parser-0.2.1/tests/test_from_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-04-13 22:55:24.000000 py-partiql-parser-0.2.1/tests/test_json_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-13 22:55:24.000000 py-partiql-parser-0.2.1/tests/test_select_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-13 22:55:24.000000 py-partiql-parser-0.2.1/tests/test_select_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-13 22:55:24.000000 py-partiql-parser-0.2.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-13 22:55:24.000000 py-partiql-parser-0.2.1/tests/test_where_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:50:03.474916 py-partiql-parser-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-16 13:49:46.000000 py-partiql-parser-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-16 13:50:03.474916 py-partiql-parser-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-16 13:49:46.000000 py-partiql-parser-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:50:03.470916 py-partiql-parser-0.3.0/py_partiql_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-16 13:49:46.000000 py-partiql-parser-0.3.0/py_partiql_parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:50:03.474916 py-partiql-parser-0.3.0/py_partiql_parser/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 13:49:46.000000 py-partiql-parser-0.3.0/py_partiql_parser/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-16 13:49:46.000000 py-partiql-parser-0.3.0/py_partiql_parser/_internal/case_insensitive_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-16 13:49:46.000000 py-partiql-parser-0.3.0/py_partiql_parser/_internal/clause_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-16 13:49:46.000000 py-partiql-parser-0.3.0/py_partiql_parser/_internal/csv_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-04-16 13:49:46.000000 py-partiql-parser-0.3.0/py_partiql_parser/_internal/from_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-04-16 13:49:46.000000 py-partiql-parser-0.3.0/py_partiql_parser/_internal/json_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-04-16 13:49:46.000000 py-partiql-parser-0.3.0/py_partiql_parser/_internal/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-04-16 13:49:46.000000 py-partiql-parser-0.3.0/py_partiql_parser/_internal/select_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-04-16 13:49:46.000000 py-partiql-parser-0.3.0/py_partiql_parser/_internal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-04-16 13:49:46.000000 py-partiql-parser-0.3.0/py_partiql_parser/_internal/where_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:50:03.474916 py-partiql-parser-0.3.0/py_partiql_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-16 13:50:03.000000 py-partiql-parser-0.3.0/py_partiql_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-04-16 13:50:03.000000 py-partiql-parser-0.3.0/py_partiql_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 13:50:03.000000 py-partiql-parser-0.3.0/py_partiql_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-16 13:50:03.000000 py-partiql-parser-0.3.0/py_partiql_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-16 13:50:03.000000 py-partiql-parser-0.3.0/py_partiql_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-16 13:49:56.000000 py-partiql-parser-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-16 13:50:03.474916 py-partiql-parser-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:50:03.474916 py-partiql-parser-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-04-16 13:49:46.000000 py-partiql-parser-0.3.0/tests/test_csv_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-04-16 13:49:46.000000 py-partiql-parser-0.3.0/tests/test_dynamodb_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-16 13:49:46.000000 py-partiql-parser-0.3.0/tests/test_from_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-04-16 13:49:46.000000 py-partiql-parser-0.3.0/tests/test_json_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-16 13:49:46.000000 py-partiql-parser-0.3.0/tests/test_query_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-04-16 13:49:46.000000 py-partiql-parser-0.3.0/tests/test_s3_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-16 13:49:46.000000 py-partiql-parser-0.3.0/tests/test_select_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-16 13:49:46.000000 py-partiql-parser-0.3.0/tests/test_select_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-16 13:49:46.000000 py-partiql-parser-0.3.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-04-16 13:49:46.000000 py-partiql-parser-0.3.0/tests/test_where_parser.py
```

### Comparing `py-partiql-parser-0.2.1/LICENSE` & `py-partiql-parser-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.2.1/PKG-INFO` & `py-partiql-parser-0.3.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,44 +1,41 @@
-Metadata-Version: 2.1
-Name: py-partiql-parser
-Version: 0.2.1
-Summary: Pure Python PartiQL Parser
-Author-email: Bert Blommers <info@bertblommers.nl>
-License: MIT
-Keywords: pypartiql,parser
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # py-partiql-parser
 A tokenizer/parser/executor for the PartiQL-language, in Python.
 
 Much beta, such wow. Feel free to raise any issues you encounter.
 
-## Usage
-```
-original_json = {"a1": "b1", "a2": "b2"}
-from py_partiql_parser import Parser
-parser = Parser(source_data={"s3object": original_json})
+## S3 Usage
+```python
+import json
+from py_partiql_parser import S3SelectParser
+
+original_json = json.dumps({"a1": "b1", "a2": "b2"})
+parser = S3SelectParser(source_data={"s3object": original_json})
 result = parser.parse("SELECT * FROM s3object")
 ```
+## DynamoDB Usage
+```python
+import json
+from py_partiql_parser import DynamoDBStatementParser
+
+original_json = json.dumps({"a1": "b1", "a2": "b2"})
+parser = DynamoDBStatementParser(source_data={"table1", original_json})
+result = parser.parse("SELECT * from table1 WHERE a1 = ?", parameters=[{"S": "b1"}])
+```
+
 
 ## Meat
 The important logic of this library can be found here: https://github.com/bblommers/py-partiql-parser/blob/main/py_partiql_parser/_internal/parser.py
 
 It is implemented as a naive, dependency-free, TDD-first tokenizer.
 
-## Tests
-Tests based on real-world examples from users/AWS, and can be found here:
-https://github.com/getmoto/py-partiql-parser/blob/main/tests/test_aws_examples.py
-
 ## Outstanding
  - Support for functions such as `count(*)`
  - Support for CSV conversion. A start has been made in `_internal/csv_converter.py`
  - .. and I'm sure many other things.
 
 ## Notes
 The first iteration of this library was based on the spec, found here: https://partiql.org/assets/PartiQL-Specification.pdf
 
 AWS doesn't follow its own spec though, most notably:
  - a file containing a list (with multiple JSON documents) cannot be queried normally (`select *` returns everything, but you cannot `select key` for each document in the list)
- - `select values` is not supported
+ - `select values` is not supported
```

### Comparing `py-partiql-parser-0.2.1/README.md` & `py-partiql-parser-0.3.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,52 @@
+Metadata-Version: 2.1
+Name: py-partiql-parser
+Version: 0.3.0
+Summary: Pure Python PartiQL Parser
+Author-email: Bert Blommers <info@bertblommers.nl>
+License: MIT
+Keywords: pypartiql,parser
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 # py-partiql-parser
 A tokenizer/parser/executor for the PartiQL-language, in Python.
 
 Much beta, such wow. Feel free to raise any issues you encounter.
 
-## Usage
-```
-original_json = {"a1": "b1", "a2": "b2"}
-from py_partiql_parser import Parser
-parser = Parser(source_data={"s3object": original_json})
+## S3 Usage
+```python
+import json
+from py_partiql_parser import S3SelectParser
+
+original_json = json.dumps({"a1": "b1", "a2": "b2"})
+parser = S3SelectParser(source_data={"s3object": original_json})
 result = parser.parse("SELECT * FROM s3object")
 ```
+## DynamoDB Usage
+```python
+import json
+from py_partiql_parser import DynamoDBStatementParser
+
+original_json = json.dumps({"a1": "b1", "a2": "b2"})
+parser = DynamoDBStatementParser(source_data={"table1", original_json})
+result = parser.parse("SELECT * from table1 WHERE a1 = ?", parameters=[{"S": "b1"}])
+```
+
 
 ## Meat
 The important logic of this library can be found here: https://github.com/bblommers/py-partiql-parser/blob/main/py_partiql_parser/_internal/parser.py
 
 It is implemented as a naive, dependency-free, TDD-first tokenizer.
 
-## Tests
-Tests based on real-world examples from users/AWS, and can be found here:
-https://github.com/getmoto/py-partiql-parser/blob/main/tests/test_aws_examples.py
-
 ## Outstanding
  - Support for functions such as `count(*)`
  - Support for CSV conversion. A start has been made in `_internal/csv_converter.py`
  - .. and I'm sure many other things.
 
 ## Notes
 The first iteration of this library was based on the spec, found here: https://partiql.org/assets/PartiQL-Specification.pdf
 
 AWS doesn't follow its own spec though, most notably:
  - a file containing a list (with multiple JSON documents) cannot be queried normally (`select *` returns everything, but you cannot `select key` for each document in the list)
- - `select values` is not supported
+ - `select values` is not supported
```

### Comparing `py-partiql-parser-0.2.1/py_partiql_parser/_internal/case_insensitive_dict.py` & `py-partiql-parser-0.3.0/py_partiql_parser/_internal/case_insensitive_dict.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-try:
-    from collections import Mapping, MutableMapping
-except ImportError:
+import sys
+
+if sys.version_info[:2] >= (3, 8):
     from collections.abc import Mapping, MutableMapping
+else:
+    from collections import Mapping, MutableMapping
 from collections import OrderedDict
 
 
 class CaseInsensitiveDict(MutableMapping):
     # Taken from https://raw.githubusercontent.com/kennethreitz/requests/v2.25.1/requests/structures.py
 
     def __init__(self, data=None, **kwargs):
```

### Comparing `py-partiql-parser-0.2.1/py_partiql_parser/_internal/clause_tokenizer.py` & `py-partiql-parser-0.3.0/py_partiql_parser/_internal/clause_tokenizer.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.2.1/py_partiql_parser/_internal/csv_converter.py` & `py-partiql-parser-0.3.0/py_partiql_parser/_internal/csv_converter.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,14 +9,12 @@
         values = line.split(",")
         if len(headers) == 0:
             if headers_included:
                 headers = values
                 continue
             else:
                 headers = [f"_{x}" for x in range(1, len(values) + 1)]
-        output += (
-            json.dumps({f"{headers[idx]}": key for idx, key in enumerate(values)})
-            + "\n"
-        )
+        line = json.dumps({f"{headers[idx]}": key for idx, key in enumerate(values)})
+        output += f"{line}\n"
     if output.endswith("\n"):
         output = output.rstrip("\n")
     return output
```

### Comparing `py-partiql-parser-0.2.1/py_partiql_parser/_internal/from_parser.py` & `py-partiql-parser-0.3.0/py_partiql_parser/_internal/from_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
                     current_phrase = ""
                     section = "ALIAS"
                 elif section == "NAME":
                     name = current_phrase
                     current_phrase = ""
                     section = "AS"
                 elif section == "ALIAS":
-                    alias = current_phrase
+                    alias = current_phrase  # noqa
                     current_phrase = ""
                     section = "NAME"
                 continue
             if c == ",":
                 if section == "NAME":
                     clauses[current_phrase] = current_phrase
                 elif section == "ALIAS":
```

### Comparing `py-partiql-parser-0.2.1/py_partiql_parser/_internal/json_parser.py` & `py-partiql-parser-0.3.0/py_partiql_parser/_internal/json_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 
 class JsonParser:
     def parse(self, original, tokenizer=None, only_parse_initial=False) -> Any:
         if not (original.startswith("{") or original.startswith("[")):
             # Doesn't look like JSON - let's return as a variable
             return original if original.isnumeric() else Variable(original)
         section = None  # DICT_KEY | KEY_TO_VALUE | DICT_VAL | OBJECT_END
+        dict_key = None
         current_phrase = ""
         result: Dict[Any, Any] = CaseInsensitiveDict()
         tokenizer = tokenizer or ClauseTokenizer(original)
         while True:
             c = tokenizer.next()
             if not c:
                 break
```

### Comparing `py-partiql-parser-0.2.1/py_partiql_parser/_internal/parser.py` & `py-partiql-parser-0.3.0/py_partiql_parser/_internal/parser.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,78 @@
 import re
 
-from typing import Dict, Any, Union, List, AnyStr
+from typing import Dict, Any, Union, List, AnyStr, Optional
 
 from .from_parser import FromParser
 from .json_parser import JsonParser
 from .select_parser import SelectParser
-from .where_parser import WhereParser
-from .utils import is_dict
+from .where_parser import DynamoDBWhereParser, S3WhereParser, WhereParser
+from .utils import is_dict, QueryMetadata
 
 
 class Parser:
     RETURN_TYPE = Union[Dict[AnyStr, Any], List]
 
-    def __init__(self, source_data: Dict[str, str], query_has_table_prefix=True):
+    def __init__(
+        self,
+        source_data: Dict[str, str],
+        table_prefix: Optional[str],
+        where_parser,
+    ):
         # Source data is in the format: {source: json}
         # Where 'json' is one or more json documents separated by a newline
         self.documents = source_data
-        self.query_has_table_prefix = query_has_table_prefix
+        self.table_prefix = table_prefix
+        self.where_parser = where_parser
 
-    def parse(self, query: str) -> List[Dict[str, Any]]:
+    def parse(self, query: str, parameters=None) -> List[Dict[str, Any]]:
         query = query.replace("\n", " ")
         clauses = re.split("SELECT | FROM | WHERE ", query, flags=re.IGNORECASE)
         # First clause is whatever comes in front of SELECT - which should be nothing
         _ = clauses[0]
         # FROM
         from_clauses = FromParser().parse(clauses[2])
         source_data = self.documents[list(from_clauses.values())[0].lower()]
         source_data = JsonParser().parse(source_data)
         if is_dict(source_data):
             source_data = [source_data]  # type: ignore
 
         # WHERE
         if len(clauses) > 3:
             where_clause = clauses[3]
-            source_data = WhereParser(source_data, self.query_has_table_prefix).parse(
-                where_clause
-            )
+            source_data = self.where_parser(source_data).parse(where_clause, parameters)
 
         # SELECT
         select_clause = clauses[1]
-        return SelectParser().parse(select_clause, from_clauses, source_data)
+        return SelectParser(self.table_prefix).parse(
+            select_clause, from_clauses, source_data
+        )
+
+
+class S3SelectParser(Parser):
+    def __init__(self, source_data: Dict[str, str]):
+        super().__init__(
+            source_data, table_prefix="s3object", where_parser=S3WhereParser
+        )
+
+
+class DynamoDBStatementParser(Parser):
+    def __init__(self, source_data: Dict[str, str]):
+        super().__init__(
+            source_data, table_prefix=None, where_parser=DynamoDBWhereParser
+        )
+
+    @classmethod
+    def get_query_metadata(cls, query: str):
+        query = query.replace("\n", " ")
+        clauses = re.split("SELECT | FROM | WHERE ", query, flags=re.IGNORECASE)
+
+        from_clauses = FromParser().parse(clauses[2])
+
+        # WHERE
+        if len(clauses) > 3:
+            where_clause = clauses[3]
+            where = WhereParser.parse_where_clause(where_clause)
+        else:
+            where = None
+
+        return QueryMetadata(tables=from_clauses, where_clauses=where)
```

### Comparing `py-partiql-parser-0.2.1/py_partiql_parser/_internal/select_parser.py` & `py-partiql-parser-0.3.0/py_partiql_parser/_internal/select_parser.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,33 @@
-from typing import Dict, Any, List
+from typing import Dict, Any, List, Optional
 
-from .case_insensitive_dict import CaseInsensitiveDict
 from .clause_tokenizer import ClauseTokenizer
-from .utils import find_nested_data_in_object
+from .utils import find_nested_data_in_object, MissingVariable
 
 
 class SelectClause:
-    def __init__(self, value: str):
+    def __init__(self, value: str, table_prefix: Optional[str] = None):
+        self.table_prefix = table_prefix
         self.value = value.strip()
 
     def select(self, aliases: Dict[str, str], document: Dict[str, Any]):
         if self.value == "*":
-            # return document[alias]
-            return document["s3object"]
+            if self.table_prefix:
+                return document[self.table_prefix]
+            else:
+                return document
         if "." in self.value:
             key, remaining = self.value.split(".", maxsplit=1)
             return find_nested_data_in_object(
                 select_clause=remaining, json_doc=document[aliases.get(key, key)]
             )
+        elif not self.table_prefix:
+            return find_nested_data_in_object(
+                select_clause=self.value, json_doc=document
+            )
         else:
             return document[aliases.get(self.value, self.value)]
 
     def __repr__(self):
         return f"<SelectClause({self.value})>"
 
     def __eq__(self, other):
@@ -44,47 +50,56 @@
             isinstance(other, FunctionClause)
             and other.value == self.value
             and other.function_name == self.function_name
         )
 
 
 class SelectParser:
+    def __init__(self, table_prefix: Optional[str]):
+        self.table_prefix = table_prefix
+
     def parse(
         self,
         select_clause: str,
         aliases: Dict[str, Any],
         documents: List[Dict[str, Any]],
     ) -> List[Dict[str, Any]]:
-        clauses = self.parse_clauses(select_clause)
+        clauses = SelectParser.parse_clauses(select_clause, prefix=self.table_prefix)
 
         for clause in clauses:
             if isinstance(clause, FunctionClause):
                 return [clause.execute(aliases, documents)]
 
         result: List[Dict[str, Any]] = []
 
         for json_document in documents:
+            if self.table_prefix is not None:
+                json_document = {self.table_prefix: json_document}
             filtered_document = dict()
             for clause in clauses:
-                # TODO: go through all keys, the table/file can be called anything - not just 's3object'
-                attr = clause.select(aliases, {"s3object": json_document})
-                if attr is not None:
+                attr = clause.select(aliases, json_document)
+                if attr is not None and not isinstance(attr, MissingVariable):
                     filtered_document.update(attr)
             result.append(filtered_document)
         return result
 
-    def parse_clauses(self, select_clause: str) -> List[SelectClause]:
+    @classmethod
+    def parse_clauses(
+        cls, select_clause: str, prefix: Optional[str] = None
+    ) -> List[SelectClause]:
         results = []
         tokenizer = ClauseTokenizer(select_clause)
         current_clause = fn_name = ""
         while True:
             c = tokenizer.next()
             if not c or c in [","]:
                 if current_clause != "":
-                    results.append(SelectClause(current_clause))
+                    results.append(
+                        SelectClause(value=current_clause, table_prefix=prefix)
+                    )
                 if not c:
                     break
                 else:
                     current_clause = ""
                     continue
             if c in ["("]:
                 fn_name = current_clause
```

### Comparing `py-partiql-parser-0.2.1/py_partiql_parser/_internal/utils.py` & `py-partiql-parser-0.3.0/py_partiql_parser/_internal/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from .case_insensitive_dict import CaseInsensitiveDict
 from .json_parser import MissingVariable, Variable
-from typing import Any, Dict, List, Union
+from typing import Any, Dict, List, Tuple, Union
 
 
 def is_dict(dct):
     return isinstance(dct, dict) or isinstance(dct, CaseInsensitiveDict)
 
 
 def find_nested_data(
@@ -76,7 +76,21 @@
 
 def find_value_in_document(keys: List[str], json_doc):
     if not is_dict(json_doc):
         return None
     if len(keys) == 1:
         return json_doc.get(keys[0])
     return find_value_in_document(keys[1:], json_doc.get(keys[0], {}))
+
+
+class QueryMetadata:
+    def __init__(
+        self, tables: Dict[str, str], where_clauses: List[Tuple[List[str], str]] = None
+    ):
+        self._tables = tables
+        self._where_clauses = where_clauses or []
+
+    def get_table_names(self) -> List[str]:
+        return list(self._tables.values())
+
+    def get_filter_names(self) -> List[str]:
+        return [".".join(keys) for keys, _ in self._where_clauses]
```

### Comparing `py-partiql-parser-0.2.1/py_partiql_parser.egg-info/SOURCES.txt` & `py-partiql-parser-0.3.0/py_partiql_parser.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 README.md
 pyproject.toml
+setup.cfg
 py_partiql_parser/__init__.py
 py_partiql_parser.egg-info/PKG-INFO
 py_partiql_parser.egg-info/SOURCES.txt
 py_partiql_parser.egg-info/dependency_links.txt
 py_partiql_parser.egg-info/requires.txt
 py_partiql_parser.egg-info/top_level.txt
 py_partiql_parser/_internal/__init__.py
@@ -13,16 +14,17 @@
 py_partiql_parser/_internal/csv_converter.py
 py_partiql_parser/_internal/from_parser.py
 py_partiql_parser/_internal/json_parser.py
 py_partiql_parser/_internal/parser.py
 py_partiql_parser/_internal/select_parser.py
 py_partiql_parser/_internal/utils.py
 py_partiql_parser/_internal/where_parser.py
-tests/test_aws_examples.py
 tests/test_csv_converter.py
 tests/test_dynamodb_examples.py
 tests/test_from_parser.py
 tests/test_json_parser.py
+tests/test_query_metadata.py
+tests/test_s3_examples.py
 tests/test_select_functions.py
 tests/test_select_parser.py
 tests/test_utils.py
 tests/test_where_parser.py
```

### Comparing `py-partiql-parser-0.2.1/tests/test_aws_examples.py` & `py-partiql-parser-0.3.0/tests/test_s3_examples.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import pytest
 import sure  # noqa
-from py_partiql_parser import Parser
+from py_partiql_parser import S3SelectParser
 from . import input_json_list, json_as_lines
 
 
 # https://aws.amazon.com/blogs/storage/querying-data-without-servers-or-databases-using-amazon-s3-select/
 
 
 input_data_csv = """Name,PhoneNumber,City,Occupation
@@ -19,23 +19,23 @@
 
 input_json_object = {"a1": "b1", "a2": "b2"}
 
 
 @pytest.mark.xfail(reason="CSV functionality not yet implemented")
 def test_aws_sample__csv():
     query = "SELECT * FROM s3object s where s.\"Name\" = 'Jane'"
-    x = Parser(source_data={"s3object": input_data_csv}).parse(query)
+    x = S3SelectParser(source_data={"s3object": input_data_csv}).parse(query)
 
 
 @pytest.mark.xfail(
     reason="this shouldn't work, as it doesn't work against AWS. Input should be a string where line is a document, not a list"
 )
 def test_aws_sample__json__search_by_name():
     query = "SELECT * FROM s3object s where s.\"Name\" = 'Jane'"
-    result = Parser(source_data={"s3object": input_json_list}).parse(query)
+    result = S3SelectParser(source_data={"s3object": input_json_list}).parse(query)
     result.should.equal(
         [
             {
                 "Name": "Jane",
                 "PhoneNumber": "(949) 555-6704",
                 "City": "Chicago",
                 "Occuption": "Developer",
@@ -48,15 +48,15 @@
     "query",
     [
         "SELECT * FROM s3object s where s.City = 'Chicago'",
         "SELECT * FROM s3object s where s.\"City\" = 'Chicago'",
     ],
 )
 def test_aws_sample__json__search_by_city(query):
-    result = Parser(source_data={"s3object": json_as_lines}).parse(query)
+    result = S3SelectParser(source_data={"s3object": json_as_lines}).parse(query)
     result.should.have.length_of(4)
     result.should.contain(
         {
             "Name": "Jane",
             "PhoneNumber": "(949) 555-6704",
             "City": "Chicago",
             "Occuption": "Developer",
@@ -86,15 +86,15 @@
             "Occuption": "Developer",
         }
     )
 
 
 def test_aws_sample__json_select_multiple_attrs__search_by_city():
     query = "SELECT s.name, s.city FROM s3object s where s.\"City\" = 'Chicago'"
-    result = Parser(source_data={"s3object": json_as_lines}).parse(query)
+    result = S3SelectParser(source_data={"s3object": json_as_lines}).parse(query)
     result.should.have.length_of(4)
     result.should.contain(
         {
             "Name": "Jane",
             "City": "Chicago",
         }
     )
@@ -116,27 +116,50 @@
             "City": "Chicago",
         }
     )
 
 
 def test_aws_sample__object_select_all():
     query = "SELECT * FROM s3object"
-    result = Parser(source_data={"s3object": json.dumps(input_json_object)}).parse(
-        query
-    )
+    result = S3SelectParser(
+        source_data={"s3object": json.dumps(input_json_object)}
+    ).parse(query)
     result.should.equal([input_json_object])
 
 
 def test_aws_sample__s3object_is_case_insensitive():
     query = "SELECT * FROM s3obJEct"
-    result = Parser(source_data={"s3object": json.dumps(input_json_object)}).parse(
-        query
-    )
+    result = S3SelectParser(
+        source_data={"s3object": json.dumps(input_json_object)}
+    ).parse(query)
+    result.should.equal([input_json_object])
+
+
+def test_aws_sample__object_select_everything():
+    query = "SELECT s FROM s3object AS s"
+    result = S3SelectParser(
+        source_data={"s3object": json.dumps(input_json_object)}
+    ).parse(query)
     result.should.equal([input_json_object])
 
 
 def test_aws_sample__object_select_attr():
     query = "SELECT s.a1 FROM s3object AS s"
-    result = Parser(source_data={"s3object": json.dumps(input_json_object)}).parse(
-        query
-    )
+    result = S3SelectParser(
+        source_data={"s3object": json.dumps(input_json_object)}
+    ).parse(query)
     result.should.equal([{"a1": "b1"}])
+
+
+def test_case_insensitivity():
+    # Filter by lower case "city"
+    query = "SELECT * from s3object where s3object.city = 'Los Angeles'"
+    # Data has upper case CITY
+    all_rows = (
+        json.dumps({"Name": "Sam", "CITY": "Irvine"})
+        + "\n"
+        + json.dumps({"Name": "Vinod", "City": "Los Angeles"})
+    )
+    parser = S3SelectParser(source_data={"s3object": all_rows})
+    assert parser.parse(query, parameters=None) == [
+        {"Name": "Vinod", "City": "Los Angeles"}
+    ]
```

### Comparing `py-partiql-parser-0.2.1/tests/test_csv_converter.py` & `py-partiql-parser-0.3.0/tests/test_csv_converter.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.2.1/tests/test_from_parser.py` & `py-partiql-parser-0.3.0/tests/test_from_parser.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.2.1/tests/test_json_parser.py` & `py-partiql-parser-0.3.0/tests/test_json_parser.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.2.1/tests/test_select_functions.py` & `py-partiql-parser-0.3.0/tests/test_select_functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pytest
-from py_partiql_parser import Parser
+from py_partiql_parser import S3SelectParser
 from . import json_as_lines
 
 
 class TestCount:
     def setup_method(self):
-        self.parser = Parser(source_data={"s3object": json_as_lines})
+        self.parser = S3SelectParser(source_data={"s3object": json_as_lines})
 
     @pytest.mark.parametrize(
         "query,key,result",
         [
             ["select count(*) from s3object", "_1", 7],
             ["select count(s) from s3object s", "_1", 7],
             ["select count(s) from s3object as s", "_1", 7],
```

### Comparing `py-partiql-parser-0.2.1/tests/test_select_parser.py` & `py-partiql-parser-0.3.0/tests/test_select_parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 import pytest
 from py_partiql_parser._internal.select_parser import SelectParser
 from py_partiql_parser._internal.select_parser import SelectClause, FunctionClause
 
 
 def test_select_all_clause():
-    result = SelectParser().parse_clauses("*")
+    result = SelectParser(table_prefix=None).parse_clauses("*")
     assert result == [SelectClause("*")]
 
 
 def test_parse_simple_clause():
-    result = SelectParser().parse_clauses("s.name")
+    result = SelectParser(table_prefix=None).parse_clauses("s.name")
     assert result == [SelectClause("s.name")]
 
 
 def test_parse_multiple_clauses():
-    result = SelectParser().parse_clauses("s.name, s.city")
+    result = SelectParser(table_prefix=None).parse_clauses("s.name, s.city")
     assert result == [SelectClause("s.name"), SelectClause("s.city")]
 
 
 def test_parse_function_clause():
-    result = SelectParser().parse_clauses("count(*)")
+    result = SelectParser(table_prefix=None).parse_clauses("count(*)")
     assert result == [FunctionClause(function_name="count", value="*")]
 
 
 @pytest.mark.xfail(message="Not yet implemented")
 def test_parse_function_alias_clause():
-    result = SelectParser().parse_clauses("count(*) as cnt")
+    result = SelectParser(table_prefix=None).parse_clauses("count(*) as cnt")
     assert result == [FunctionClause(function_name="count", value="*")]
 
 
 def test_parse_mix_of_function_and_regular_clauses():
-    result = SelectParser().parse_clauses("count(*), s.city, max(s.citizens)")
+    result = SelectParser(table_prefix=None).parse_clauses(
+        "count(*), s.city, max(s.citizens)"
+    )
     assert len(result) == 3
     assert FunctionClause(function_name="count", value="*") in result
     assert FunctionClause(function_name="max", value="s.citizens") in result
     assert SelectClause(value="s.city") in result
```

### Comparing `py-partiql-parser-0.2.1/tests/test_utils.py` & `py-partiql-parser-0.3.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.2.1/tests/test_where_parser.py` & `py-partiql-parser-0.3.0/tests/test_where_parser.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,68 @@
-import pytest
-from py_partiql_parser._internal.parser import WhereParser
+from py_partiql_parser._internal.where_parser import WhereParser
+from py_partiql_parser._internal.where_parser import S3WhereParser
+from py_partiql_parser._internal.where_parser import DynamoDBWhereParser
 
 
 class TestWhereClause:
     def test_single_key(self):
         where_clause = "s3object.city = 'Chicago'"
-        assert WhereParser({}, False).parse_where_clause(where_clause) == (
-            ["s3object", "city"],
-            "Chicago",
-        )
+        assert WhereParser.parse_where_clause(where_clause) == [
+            (
+                ["s3object", "city"],
+                "Chicago",
+            )
+        ]
 
     def test_nested_key(self):
         where_clause = "s3object.city.street = 'Chicago'"
-        assert WhereParser({}, False).parse_where_clause(where_clause) == (
-            ["s3object", "city", "street"],
-            "Chicago",
-        )
+        assert WhereParser.parse_where_clause(where_clause) == [
+            (
+                ["s3object", "city", "street"],
+                "Chicago",
+            )
+        ]
 
     def test_quoted_key(self):
         where_clause = "s3object.\"city\" = 'Chicago'"
-        assert WhereParser({}, False).parse_where_clause(where_clause) == (
-            ["s3object", "city"],
-            "Chicago",
-        )
+        assert WhereParser.parse_where_clause(where_clause) == [
+            (
+                ["s3object", "city"],
+                "Chicago",
+            )
+        ]
 
     def test_quoted_nested_key(self):
         where_clause = "s3object.\"city details\".street = 'Chicago'"
-        assert WhereParser({}, False).parse_where_clause(where_clause) == (
-            ["s3object", "city details", "street"],
-            "Chicago",
-        )
+        assert WhereParser.parse_where_clause(where_clause) == [
+            (
+                ["s3object", "city details", "street"],
+                "Chicago",
+            )
+        ]
 
     def test_multiple_keys(self):
-        where_clause = "s3object.city = 'Chicago', s3object.name = 'Tommy'"
-        assert WhereParser({}, False).parse_where_clause(where_clause) == (
-            ["s3object", "city"],
-            "Chicago",
-        )
+        where_clause = "s3.city = 'Chicago' AND s3.name = 'Tommy'"
+        assert WhereParser.parse_where_clause(where_clause) == [
+            (
+                ["s3", "city"],
+                "Chicago",
+            ),
+            (["s3", "name"], "Tommy"),
+        ]
+
+    def test_multiple_keys_with_question_marks(self):
+        where_clause = "s3.city = ? AND s3.name = ?"
+        assert WhereParser.parse_where_clause(where_clause) == [
+            (
+                ["s3", "city"],
+                "?",
+            ),
+            (["s3", "name"], "?"),
+        ]
 
 
 class TestFilter:
     all_rows = [
         {"Name": "Sam", "city": "Irvine"},
         {"Name": "Vinod", "city": "Los Angeles"},
         {"Name": "Jeff", "city": "Seattle"},
@@ -49,55 +71,38 @@
         {"Name": "Mary", "city": "Chicago", "notes": {"extra": "y"}},
         {"Name": "Kate", "city": "Chicago", "notes": {"extra": "n"}},
     ]
 
     def test_simple(self):
         filter_keys = ["s3object", "city"]
         filter_value = "Los Angeles"
-        assert WhereParser(
-            TestFilter.all_rows, query_has_table_prefix=True
-        ).filter_rows(filter_keys=filter_keys, filter_value=filter_value,) == [
-            {"Name": "Vinod", "city": "Los Angeles"}
-        ]
+        assert S3WhereParser(TestFilter.all_rows).filter_rows(
+            _filters=[(filter_keys, filter_value)]
+        ) == [{"Name": "Vinod", "city": "Los Angeles"}]
 
     def test_without_prefix(self):
         filter_keys = ["city"]
         filter_value = "Los Angeles"
-        assert WhereParser(
-            TestFilter.all_rows, query_has_table_prefix=False
-        ).filter_rows(filter_keys=filter_keys, filter_value=filter_value,) == [
-            {"Name": "Vinod", "city": "Los Angeles"}
-        ]
+        assert DynamoDBWhereParser(TestFilter.all_rows).filter_rows(
+            _filters=[(filter_keys, filter_value)]
+        ) == [{"Name": "Vinod", "city": "Los Angeles"}]
 
     def test_alias(self):
         filter_keys = ["s", "city"]
         filter_value = "Los Angeles"
-        assert WhereParser(
-            TestFilter.all_rows, query_has_table_prefix=True
-        ).filter_rows(filter_keys=filter_keys, filter_value=filter_value,) == [
-            {"Name": "Vinod", "city": "Los Angeles"}
-        ]
+        assert S3WhereParser(TestFilter.all_rows).filter_rows(
+            _filters=[(filter_keys, filter_value)]
+        ) == [{"Name": "Vinod", "city": "Los Angeles"}]
 
     def test_alias_nested_key(self):
         filter_keys = ["s3object", "notes", "extra"]
         filter_value = "y"
-        assert WhereParser(
-            TestFilter.all_rows, query_has_table_prefix=True
-        ).filter_rows(filter_keys=filter_keys, filter_value=filter_value,) == [
-            {"Name": "Mary", "city": "Chicago", "notes": {"extra": "y"}}
-        ]
+        assert S3WhereParser(TestFilter.all_rows).filter_rows(
+            _filters=[(filter_keys, filter_value)]
+        ) == [{"Name": "Mary", "city": "Chicago", "notes": {"extra": "y"}}]
 
-    @pytest.mark.xfail(message="Not yet implemented")
-    def test_case_insensitivity(self):
-        # Filter by lower case "city"
-        filter_keys = ["s3object", "city"]
-        filter_value = "Chicago"
-        # Data has upper case CITY
-        all_rows = [
-            {"Name": "Sam", "CITY": "Irvine"},
-            {"Name": "Vinod", "City": "Los Angeles"},
-        ]
-        assert WhereParser().filter_rows(
-            filter_keys=filter_keys,
-            filter_value=filter_value,
-            all_rows=all_rows,
-        ) == [{"Name": "Jane", "City": "Chicago"}]
+
+class TestDynamoDBParse:
+    def test_parameters(self):
+        parser = DynamoDBWhereParser(source_data=TestFilter.all_rows)
+        resp = parser.parse("notes = ?", parameters=[{"extra": "n"}])
+        assert resp == [{"Name": "Kate", "city": "Chicago", "notes": {"extra": "n"}}]
```

