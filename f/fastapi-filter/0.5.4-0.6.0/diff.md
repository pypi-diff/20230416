# Comparing `tmp/fastapi_filter-0.5.4.tar.gz` & `tmp/fastapi_filter-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_filter-0.5.4.tar", max compression
+gzip compressed data, was "fastapi_filter-0.6.0.tar", max compression
```

## Comparing `fastapi_filter-0.5.4.tar` & `fastapi_filter-0.6.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1070 2023-03-16 07:42:46.455632 fastapi_filter-0.5.4/LICENSE
--rw-r--r--   0        0        0     1945 2023-03-16 07:42:46.455632 fastapi_filter-0.5.4/README.md
--rw-r--r--   0        0        0      107 2023-03-16 07:42:46.455632 fastapi_filter-0.5.4/fastapi_filter/__init__.py
--rw-r--r--   0        0        0        0 2023-03-16 07:42:46.455632 fastapi_filter-0.5.4/fastapi_filter/base/__init__.py
--rw-r--r--   0        0        0     7764 2023-03-16 07:42:46.455632 fastapi_filter-0.5.4/fastapi_filter/base/filter.py
--rw-r--r--   0        0        0        0 2023-03-16 07:42:46.455632 fastapi_filter-0.5.4/fastapi_filter/contrib/__init__.py
--rw-r--r--   0        0        0       50 2023-03-16 07:42:46.455632 fastapi_filter-0.5.4/fastapi_filter/contrib/mongoengine/__init__.py
--rw-r--r--   0        0        0     2511 2023-03-16 07:42:46.455632 fastapi_filter-0.5.4/fastapi_filter/contrib/mongoengine/filter.py
--rw-r--r--   0        0        0       50 2023-03-16 07:42:46.455632 fastapi_filter-0.5.4/fastapi_filter/contrib/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     3816 2023-03-16 07:42:46.455632 fastapi_filter-0.5.4/fastapi_filter/contrib/sqlalchemy/filter.py
--rw-r--r--   0        0        0        0 2023-03-16 07:42:46.455632 fastapi_filter-0.5.4/fastapi_filter/py.typed
--rw-r--r--   0        0        0     2309 2023-03-16 07:42:46.459632 fastapi_filter-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     3044 1970-01-01 00:00:00.000000 fastapi_filter-0.5.4/setup.py
--rw-r--r--   0        0        0     3388 1970-01-01 00:00:00.000000 fastapi_filter-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-16 13:44:15.342773 fastapi_filter-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1945 2023-04-16 13:44:15.342773 fastapi_filter-0.6.0/README.md
+-rw-r--r--   0        0        0      107 2023-04-16 13:44:15.342773 fastapi_filter-0.6.0/fastapi_filter/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-16 13:44:15.342773 fastapi_filter-0.6.0/fastapi_filter/base/__init__.py
+-rw-r--r--   0        0        0     7764 2023-04-16 13:44:15.342773 fastapi_filter-0.6.0/fastapi_filter/base/filter.py
+-rw-r--r--   0        0        0        0 2023-04-16 13:44:15.342773 fastapi_filter-0.6.0/fastapi_filter/contrib/__init__.py
+-rw-r--r--   0        0        0       50 2023-04-16 13:44:15.342773 fastapi_filter-0.6.0/fastapi_filter/contrib/mongoengine/__init__.py
+-rw-r--r--   0        0        0     2511 2023-04-16 13:44:15.342773 fastapi_filter-0.6.0/fastapi_filter/contrib/mongoengine/filter.py
+-rw-r--r--   0        0        0       50 2023-04-16 13:44:15.342773 fastapi_filter-0.6.0/fastapi_filter/contrib/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     4466 2023-04-16 13:44:15.342773 fastapi_filter-0.6.0/fastapi_filter/contrib/sqlalchemy/filter.py
+-rw-r--r--   0        0        0        0 2023-04-16 13:44:15.342773 fastapi_filter-0.6.0/fastapi_filter/py.typed
+-rw-r--r--   0        0        0     2309 2023-04-16 13:44:15.346773 fastapi_filter-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3044 1970-01-01 00:00:00.000000 fastapi_filter-0.6.0/setup.py
+-rw-r--r--   0        0        0     3388 1970-01-01 00:00:00.000000 fastapi_filter-0.6.0/PKG-INFO
```

### Comparing `fastapi_filter-0.5.4/LICENSE` & `fastapi_filter-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_filter-0.5.4/README.md` & `fastapi_filter-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_filter-0.5.4/fastapi_filter/base/filter.py` & `fastapi_filter-0.6.0/fastapi_filter/base/filter.py`

 * *Files identical despite different names*

### Comparing `fastapi_filter-0.5.4/fastapi_filter/contrib/mongoengine/filter.py` & `fastapi_filter-0.6.0/fastapi_filter/contrib/mongoengine/filter.py`

 * *Files identical despite different names*

### Comparing `fastapi_filter-0.5.4/fastapi_filter/contrib/sqlalchemy/filter.py` & `fastapi_filter-0.6.0/fastapi_filter/contrib/sqlalchemy/filter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,49 @@
 # -*- coding: utf-8 -*-
 from enum import Enum
 from typing import Union
+from warnings import warn
 
 from pydantic import validator
 from sqlalchemy import or_
 from sqlalchemy.orm import Query
 from sqlalchemy.sql.selectable import Select
 
 from ...base.filter import BaseFilterModel
 
+
+def _backward_compatible_value_for_like_and_ilike(value):
+    """Adds % if not in value to be backward compatible.
+
+    Args:
+        value: The value to filter.
+
+    Returns:
+        Either the unmodified value if a percent sign is present, the value wrapped in % otherwise to preserve
+        current behavior.
+    """
+    if "%" not in value:
+        warn(
+            "You must pass the % character explicitly to use the like and ilike operators.",
+            DeprecationWarning,
+        )
+        value = f"%{value}%"
+    return value
+
+
 _orm_operator_transformer = {
     "neq": lambda value: ("__ne__", value),
     "gt": lambda value: ("__gt__", value),
     "gte": lambda value: ("__ge__", value),
     "in": lambda value: ("in_", value),
     "isnull": lambda value: ("is_", None) if value is True else ("is_not", None),
     "lt": lambda value: ("__lt__", value),
     "lte": lambda value: ("__le__", value),
-    "like": lambda value: ("like", f"%{value}%"),
-    "ilike": lambda value: ("ilike", f"%{value}%"),
+    "like": lambda value: ("like", _backward_compatible_value_for_like_and_ilike(value)),
+    "ilike": lambda value: ("ilike", _backward_compatible_value_for_like_and_ilike(value)),
     # XXX(arthurio): Mysql excludes None values when using `in` or `not in` filters.
     "not": lambda value: ("is_not", value),
     "not_in": lambda value: ("not_in", value),
 }
 """Operators à la Django.
 
 Examples:
```

### Comparing `fastapi_filter-0.5.4/pyproject.toml` & `fastapi_filter-0.6.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
   "mongoengine.*",
   "uvicorn.*",
 ]
 ignore_missing_imports = true
 
 [tool.poetry]
 name = "fastapi-filter"
-version = "0.5.4"
+version = "0.6.0"
 description = "FastAPI filter"
 authors = ["Arthur Rio <arthur.rio44@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/arthurio/fastapi-filter"
 classifiers = [
     "Natural Language :: English",
@@ -49,37 +49,37 @@
 SQLAlchemy = {version = ">=1.4.36,<2.1.0", optional = true}
 fastapi = ">=0.78,<1.0"
 mongoengine = {version = ">=0.24.1,<0.28.0", optional = true}
 pydantic = ">=1.10.0,<2.0.0"
 python = ">=3.8,<3.12"
 
 [tool.poetry.dev-dependencies]
-Faker = "^17.6.0"
-SQLAlchemy-Utils = "^0.40.0"
+Faker = "^18.0.0"
+SQLAlchemy-Utils = "^0.41.0"
 aiosqlite = "^0.18.0"
 bandit = "^1.7.5"
 black = "^23.1.0"
 flake8 = "^5.0.4"
 flake8-breakpoint = "^1.1.0"
 flake8-builtins = "^2.1.0"
 flake8-docstrings = "^1.7.0"
-flake8-simplify = "^0.19.3"
+flake8-simplify = "^0.20.0"
 flynt = "^0.77"
 greenlet = "^2.0.2"
-httpx = "^0.23.3"
+httpx = "^0.24.0"
 ipython = "^8.11.0"
 isort = "^5.12.0"
 mkdocs-material = "^9.1.2"
 mypy = "^1.1"
 mypy-extensions = "^1.0.0"
 pre-commit = "^3.1.1"
 pudb = "^2022.1.3"
 pydantic = {extras = ["email"], version = "^1.10.0"}
 pytest = "^7.2.2"
-pytest-asyncio = "^0.20.3"
+pytest-asyncio = "^0.21.0"
 pytest-cov = "^4.0.0"
 pytest-pudb = "^0.7.0"
 python-lsp-server = "^1.7.1"
 requests = "^2.28.2"
 tomli = "^2.0.1"
 types-click = "^7.1.8"
 types-setuptools = "^67.6.0"
```

### Comparing `fastapi_filter-0.5.4/setup.py` & `fastapi_filter-0.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 extras_require = \
 {'all': ['SQLAlchemy>=1.4.36,<2.1.0', 'mongoengine>=0.24.1,<0.28.0'],
  'mongoengine': ['mongoengine>=0.24.1,<0.28.0'],
  'sqlalchemy': ['SQLAlchemy>=1.4.36,<2.1.0']}
 
 setup_kwargs = {
     'name': 'fastapi-filter',
-    'version': '0.5.4',
+    'version': '0.6.0',
     'description': 'FastAPI filter',
     'long_description': '[![pypi downloads](https://img.shields.io/pypi/dm/fastapi-filter?color=%232E73B2&logo=python&logoColor=%23F9D25F)](https://pypi.org/project/fastapi-filter)\n[![codecov](https://codecov.io/gh/arthurio/fastapi-filter/branch/main/graph/badge.svg?token=I1DVBL1682)](https://codecov.io/gh/arthurio/fastapi-filter)\n[![Netlify Status](https://api.netlify.com/api/v1/badges/83451c4f-76dd-4154-9b2d-61f654eb0704/deploy-status)](https://fastapi-filter.netlify.app/)\n[![CodeQL](https://github.com/arthurio/fastapi-filter/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/arthurio/fastapi-filter/actions/workflows/codeql-analysis.yml)\n\n# FastAPI filter\n\n## Compatibility\n\n**Required:**\n  * Python: >=3.8, <3.12\n  * Fastapi: >=0.78, <1.0\n  * Pydantic: >=1.10.0, <2.0.0\n\n\n**Optional**\n  * MongoEngine: >=0.24.1, <0.28.0\n  * SQLAlchemy: >=1.4.36, <2.1.0\n\n## Installation\n\n```bash\n# Basic version\npip install fastapi-filter\n\n# With backends\npip install fastapi-filter[all]\n\n# More selective\npip install fastapi-filter[sqlalchemy]\npip install fastapi-filter[mongoengine]\n```\n\n## Documentation\n\nPlease visit: [https://fastapi-filter.netlify.app/](https://fastapi-filter.netlify.app/)\n\n## Examples\n\n![Swagger UI](https://raw.githubusercontent.com/arthurio/fastapi-filter/main/docs/swagger-ui.png)\n\nYou can play with examples:\n\n```bash\npip install poetry\npoetry install\npython examples/fastapi_filter_sqlalchemy.py\n```\n\n### Filter\n\nhttps://user-images.githubusercontent.com/950449/176737541-0e36b72f-38e2-4368-abfa-8bbc0c82e8ae.mp4\n\n### Order by\n\nhttps://user-images.githubusercontent.com/950449/176747056-ea82d6b9-cb3b-43eb-aec7-96ba0bc79e8b.mp4\n\n## Contribution\n\nYou can run tests with `pytest`.\n\n```bash\npip install poetry\npoetry install --extras all\npytest\n```\n\n<img width="884" alt="arthur_Arthurs-MacBook-Pro-2___code_fastapi-filter" src="https://user-images.githubusercontent.com/950449/176737623-a77f15d6-4e60-4c06-bdb7-b3d77f346a54.png">\n',
     'author': 'Arthur Rio',
     'author_email': 'arthur.rio44@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/arthurio/fastapi-filter',
```

### Comparing `fastapi_filter-0.5.4/PKG-INFO` & `fastapi_filter-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-filter
-Version: 0.5.4
+Version: 0.6.0
 Summary: FastAPI filter
 Home-page: https://github.com/arthurio/fastapi-filter
 License: MIT
 Author: Arthur Rio
 Author-email: arthur.rio44@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: Framework :: FastAPI
```

