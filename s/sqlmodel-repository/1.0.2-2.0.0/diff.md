# Comparing `tmp/sqlmodel_repository-1.0.2.tar.gz` & `tmp/sqlmodel_repository-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlmodel_repository-1.0.2.tar", max compression
+gzip compressed data, was "sqlmodel_repository-2.0.0.tar", max compression
```

## Comparing `sqlmodel_repository-1.0.2.tar` & `sqlmodel_repository-2.0.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0    35149 2023-04-09 16:14:21.173404 sqlmodel_repository-1.0.2/LICENSE
--rw-r--r--   0        0        0     5575 2023-04-09 16:14:21.173404 sqlmodel_repository-1.0.2/README.md
--rw-r--r--   0        0        0     1502 2023-04-09 16:14:41.753399 sqlmodel_repository-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      199 2023-04-09 16:14:41.753399 sqlmodel_repository-1.0.2/sqlmodel_repository/__init__.py
--rw-r--r--   0        0        0     7761 2023-04-09 16:14:21.177404 sqlmodel_repository-1.0.2/sqlmodel_repository/base_repository.py
--rw-r--r--   0        0        0      167 2023-04-09 16:14:21.177404 sqlmodel_repository-1.0.2/sqlmodel_repository/entity.py
--rw-r--r--   0        0        0      589 2023-04-09 16:14:21.177404 sqlmodel_repository-1.0.2/sqlmodel_repository/exceptions.py
--rw-r--r--   0        0        0     5841 2023-04-09 16:14:21.177404 sqlmodel_repository-1.0.2/sqlmodel_repository/repository.py
--rw-r--r--   0        0        0     6143 1970-01-01 00:00:00.000000 sqlmodel_repository-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-16 09:29:08.992709 sqlmodel_repository-2.0.0/LICENSE
+-rw-r--r--   0        0        0     5752 2023-04-16 09:29:08.992709 sqlmodel_repository-2.0.0/README.md
+-rw-r--r--   0        0        0     1524 2023-04-16 09:29:18.660712 sqlmodel_repository-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      199 2023-04-16 09:29:18.656712 sqlmodel_repository-2.0.0/sqlmodel_repository/__init__.py
+-rw-r--r--   0        0        0    13925 2023-04-16 09:29:08.992709 sqlmodel_repository-2.0.0/sqlmodel_repository/base_repository.py
+-rw-r--r--   0        0        0      167 2023-04-16 09:29:08.992709 sqlmodel_repository-2.0.0/sqlmodel_repository/entity.py
+-rw-r--r--   0        0        0      589 2023-04-16 09:29:08.992709 sqlmodel_repository-2.0.0/sqlmodel_repository/exceptions.py
+-rw-r--r--   0        0        0      543 2023-04-16 09:29:08.992709 sqlmodel_repository-2.0.0/sqlmodel_repository/logger.py
+-rw-r--r--   0        0        0     2640 2023-04-16 09:29:08.992709 sqlmodel_repository-2.0.0/sqlmodel_repository/repository.py
+-rw-r--r--   0        0        0     6364 1970-01-01 00:00:00.000000 sqlmodel_repository-2.0.0/PKG-INFO
```

### Comparing `sqlmodel_repository-1.0.2/LICENSE` & `sqlmodel_repository-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlmodel_repository-1.0.2/README.md` & `sqlmodel_repository-2.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -80,14 +80,16 @@
 class PetRepository(AbstractRepository[Pet]):
     """Repository to manage pets"""
 
 class ShelterRepository(AbstractRepository[Shelter]):
     """Repository to manage shelters"""
 ```
 
+Optionally, you may pass a `logger` keyword argument to the repository to log the operations. The logger should be a `structlog` logger with enabled `JSONRenderer`. If no logger is provided the repository will use its default logger (`SQLModelRepositoryLogger`).
+
 Done 🚀 You can now use the repository to perform the operations on your entities. e.g.:
 
 ```python
 from sqlmodel import col
 
 # Create a new shelter
 shelter = ShelterRepository().create(Shelter(name="Shelter 1"))
@@ -109,19 +111,15 @@
 Each `Repository` comes with a set of **typed methods** to perform common CRUD operations on your entities:
 
 - `create`: Create a new record of an entity
 - `create_batch`: Create a batch of records of an entity
 
 ______________________________________________________________________
 
-- `find`: Find all records of an entity that match the given filters
-
-______________________________________________________________________
-
-- `get_by_id`: Get a single record by its ID
+- `get`: Get a single record by its ID
 - `get_batch`: Get all records of an entity that match the given filters
 - `get_batch_by_ids`: Get a batch of records by their IDs
 - `get_all`: Get all records of an entity
 
 ______________________________________________________________________
 
 - `update`: Update an entity instance
@@ -136,19 +134,20 @@
 - `delete_batch`: Delete a batch of entity instances
 - `delete_batch_by_ids`: Delete a batch of entities by their IDs
 
 ### BaseRepository
 
 If you require more flexibility, you may also use the `BaseRepository` which provides more granular operations. The `BaseRepository` provides the following methods:
 
-- `_create`: Create a new record of an entity
-- `_create_batch`: Create a batch of records of an entity
-- `_update`: Update an entity instance
-- `_update_batch`: Update a batch of entity instances with the same values
-- `_get`: Get a single record by its ID
-- `_get_batch`: Get all records of an entity that match the given filters
-- `_delete`: Delete an entity instance
-- `_delete_batch`: Delete a batch of entity instances
+- `create`: Create a new record of an entity
+- `create_batch`: Create a batch of records of an entity
+- `update`: Update an entity instance
+- `update_batch`: Update a batch of entity instances with the same values
+- `get`: Get a single record by its ID
+- `get_batch`: Get all records of an entity that match the given filters
+- `find`: Find all records of an entity that match the given filters
+- `delete`: Delete an entity instance
+- `delete_batch`: Delete a batch of entity instances
 
 ## Examples
 
 For a more detailed example, check out our [tests/integration/scenarios](tests/integration/scenarios) directory. We do not currently offer a full example application.
```

### Comparing `sqlmodel_repository-1.0.2/pyproject.toml` & `sqlmodel_repository-2.0.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -4,19 +4,20 @@
 
 [tool.poetry]
 authors = ["Jonas Scholl <jonas@code-specialist.com>", "Yannic Schröer <yannic@code-specialist.com>"]
 description = "Repository pattern implementation for SQLModel (SQLAlchemy)"
 license = "MIT"
 name = "sqlmodel-repository"
 readme = "README.md"
-version = "1.0.2"
+version = "2.0.0"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 sqlmodel = "^0.0.8"
+structlog = "^23.1.0"
 
 [tool.poetry.dev-dependencies]
 psycopg2-binary = "^2.9.5"
 pylint = "^2.15.8"
 pylint-quotes = "^0.2.3"
 pytest = "^7.2.0"
 pytest-cov = "^4.0.0"
```

### Comparing `sqlmodel_repository-1.0.2/sqlmodel_repository/exceptions.py` & `sqlmodel_repository-2.0.0/sqlmodel_repository/exceptions.py`

 * *Files identical despite different names*

### Comparing `sqlmodel_repository-1.0.2/PKG-INFO` & `sqlmodel_repository-2.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: sqlmodel-repository
-Version: 1.0.2
+Version: 2.0.0
 Summary: Repository pattern implementation for SQLModel (SQLAlchemy)
 License: MIT
 Author: Jonas Scholl
 Author-email: jonas@code-specialist.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: sqlmodel (>=0.0.8,<0.0.9)
+Requires-Dist: structlog (>=23.1.0,<24.0.0)
 Description-Content-Type: text/markdown
 
 # SQLModel Repository - Python Repository Pattern Implementation for SQLModel
 
 [![CodeQL](https://github.com/code-specialist/python-repository/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/code-specialist/python-repository/actions/workflows/github-code-scanning/codeql) [![Tests](https://github.com/code-specialist/python-repository/actions/workflows/test.yaml/badge.svg)](https://github.com/code-specialist/python-repository/actions/workflows/test.yaml)
 
 SQLModel Repository implements the repository pattern and provides simple, robust and reliable CRUD operations for [SQLModels](https://sqlmodel.tiangolo.com/). The repository pattern is a great way to encapsulate the logic of your application and to separate the business logic from the data access layer.
@@ -96,14 +97,16 @@
 class PetRepository(AbstractRepository[Pet]):
     """Repository to manage pets"""
 
 class ShelterRepository(AbstractRepository[Shelter]):
     """Repository to manage shelters"""
 ```
 
+Optionally, you may pass a `logger` keyword argument to the repository to log the operations. The logger should be a `structlog` logger with enabled `JSONRenderer`. If no logger is provided the repository will use its default logger (`SQLModelRepositoryLogger`).
+
 Done 🚀 You can now use the repository to perform the operations on your entities. e.g.:
 
 ```python
 from sqlmodel import col
 
 # Create a new shelter
 shelter = ShelterRepository().create(Shelter(name="Shelter 1"))
@@ -125,19 +128,15 @@
 Each `Repository` comes with a set of **typed methods** to perform common CRUD operations on your entities:
 
 - `create`: Create a new record of an entity
 - `create_batch`: Create a batch of records of an entity
 
 ______________________________________________________________________
 
-- `find`: Find all records of an entity that match the given filters
-
-______________________________________________________________________
-
-- `get_by_id`: Get a single record by its ID
+- `get`: Get a single record by its ID
 - `get_batch`: Get all records of an entity that match the given filters
 - `get_batch_by_ids`: Get a batch of records by their IDs
 - `get_all`: Get all records of an entity
 
 ______________________________________________________________________
 
 - `update`: Update an entity instance
@@ -152,20 +151,21 @@
 - `delete_batch`: Delete a batch of entity instances
 - `delete_batch_by_ids`: Delete a batch of entities by their IDs
 
 ### BaseRepository
 
 If you require more flexibility, you may also use the `BaseRepository` which provides more granular operations. The `BaseRepository` provides the following methods:
 
-- `_create`: Create a new record of an entity
-- `_create_batch`: Create a batch of records of an entity
-- `_update`: Update an entity instance
-- `_update_batch`: Update a batch of entity instances with the same values
-- `_get`: Get a single record by its ID
-- `_get_batch`: Get all records of an entity that match the given filters
-- `_delete`: Delete an entity instance
-- `_delete_batch`: Delete a batch of entity instances
+- `create`: Create a new record of an entity
+- `create_batch`: Create a batch of records of an entity
+- `update`: Update an entity instance
+- `update_batch`: Update a batch of entity instances with the same values
+- `get`: Get a single record by its ID
+- `get_batch`: Get all records of an entity that match the given filters
+- `find`: Find all records of an entity that match the given filters
+- `delete`: Delete an entity instance
+- `delete_batch`: Delete a batch of entity instances
 
 ## Examples
 
 For a more detailed example, check out our [tests/integration/scenarios](tests/integration/scenarios) directory. We do not currently offer a full example application.
```

