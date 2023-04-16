# Comparing `tmp/fastapi_cruddy_framework-0.0.6.tar.gz` & `tmp/fastapi_cruddy_framework-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_cruddy_framework-0.0.6.tar", max compression
+gzip compressed data, was "fastapi_cruddy_framework-0.0.7.tar", max compression
```

## Comparing `fastapi_cruddy_framework-0.0.6.tar` & `fastapi_cruddy_framework-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1074 2023-03-03 18:31:12.339513 fastapi_cruddy_framework-0.0.6/LICENSE
--rw-r--r--   0        0        0    26534 2023-03-13 02:18:05.751986 fastapi_cruddy_framework-0.0.6/README.md
--rw-r--r--   0        0        0      979 2023-03-12 22:09:19.968403 fastapi_cruddy_framework-0.0.6/fastapi_cruddy_framework/__init__.py
--rw-r--r--   0        0        0     4533 2023-03-13 01:33:27.636779 fastapi_cruddy_framework-0.0.6/fastapi_cruddy_framework/adapters.py
--rw-r--r--   0        0        0    17594 2023-03-13 02:03:11.297401 fastapi_cruddy_framework-0.0.6/fastapi_cruddy_framework/controller.py
--rw-r--r--   0        0        0       46 2023-03-03 18:31:12.343965 fastapi_cruddy_framework-0.0.6/fastapi_cruddy_framework/inflector.py
--rw-r--r--   0        0        0    23431 2023-03-13 01:49:56.950353 fastapi_cruddy_framework-0.0.6/fastapi_cruddy_framework/repository.py
--rw-r--r--   0        0        0    19346 2023-03-13 00:39:10.961031 fastapi_cruddy_framework-0.0.6/fastapi_cruddy_framework/resource.py
--rw-r--r--   0        0        0     2282 2023-03-03 18:31:12.344318 fastapi_cruddy_framework-0.0.6/fastapi_cruddy_framework/router.py
--rw-r--r--   0        0        0     2633 2023-03-12 22:38:10.624971 fastapi_cruddy_framework-0.0.6/fastapi_cruddy_framework/schemas.py
--rw-r--r--   0        0        0      468 2023-03-12 23:34:17.002508 fastapi_cruddy_framework-0.0.6/fastapi_cruddy_framework/util.py
--rw-r--r--   0        0        0     4840 2023-03-12 21:25:52.778408 fastapi_cruddy_framework-0.0.6/fastapi_cruddy_framework/uuid.py
--rw-r--r--   0        0        0     1895 2023-03-12 17:07:21.347066 fastapi_cruddy_framework-0.0.6/pyproject.toml
--rw-r--r--   0        0        0    27901 1970-01-01 00:00:00.000000 fastapi_cruddy_framework-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-04-15 22:07:32.387542 fastapi_cruddy_framework-0.0.7/LICENSE
+-rw-r--r--   0        0        0    29689 2023-04-16 00:33:35.866892 fastapi_cruddy_framework-0.0.7/README.md
+-rw-r--r--   0        0        0      979 2023-04-15 22:07:32.387542 fastapi_cruddy_framework-0.0.7/fastapi_cruddy_framework/__init__.py
+-rw-r--r--   0        0        0     4533 2023-04-15 22:07:32.387542 fastapi_cruddy_framework-0.0.7/fastapi_cruddy_framework/adapters.py
+-rw-r--r--   0        0        0    17466 2023-04-16 00:39:33.654484 fastapi_cruddy_framework-0.0.7/fastapi_cruddy_framework/controller.py
+-rw-r--r--   0        0        0       46 2023-04-15 22:07:32.387542 fastapi_cruddy_framework-0.0.7/fastapi_cruddy_framework/inflector.py
+-rw-r--r--   0        0        0    24682 2023-04-16 00:38:48.250535 fastapi_cruddy_framework-0.0.7/fastapi_cruddy_framework/repository.py
+-rw-r--r--   0        0        0    19346 2023-04-15 22:07:32.387542 fastapi_cruddy_framework-0.0.7/fastapi_cruddy_framework/resource.py
+-rw-r--r--   0        0        0     2282 2023-04-15 22:07:32.391543 fastapi_cruddy_framework-0.0.7/fastapi_cruddy_framework/router.py
+-rw-r--r--   0        0        0     2633 2023-04-15 22:07:32.391543 fastapi_cruddy_framework-0.0.7/fastapi_cruddy_framework/schemas.py
+-rw-r--r--   0        0        0      468 2023-04-15 22:07:32.391543 fastapi_cruddy_framework-0.0.7/fastapi_cruddy_framework/util.py
+-rw-r--r--   0        0        0     4840 2023-04-15 22:07:32.391543 fastapi_cruddy_framework-0.0.7/fastapi_cruddy_framework/uuid.py
+-rw-r--r--   0        0        0     1895 2023-04-16 00:12:37.160738 fastapi_cruddy_framework-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0    31056 1970-01-01 00:00:00.000000 fastapi_cruddy_framework-0.0.7/PKG-INFO
```

### Comparing `fastapi_cruddy_framework-0.0.6/LICENSE` & `fastapi_cruddy_framework-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-0.0.6/README.md` & `fastapi_cruddy_framework-0.0.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -181,14 +181,59 @@
 
 <b>Updating Relationships:</b>
 * You can update relationships via either CREATE or UPDATE actions against each base resource! 
 
 
 As you will discover, your resource's create and update models will automatically gain "shadow" properties where one-to-many and many-to-many relationships exist. These properties expect a client to send a list of IDs that specify the foreign records that relate to the target record. So - if a user is a member of many groups, and a group can have many users, you could update the users in a group by sending a property `"users": [1,2,3,4,5]` within the `group` payload object you send to the `POST /groups` or `PATCH /groups` routes/actions. It will all be clear when you look at the SWAGGER docs generated for your API.
 
+<b>Lifecycle hooks</b>
+
+The following lifecycle hook methods, which can be defined in user-space code, receive the following information from fastapi-cruddy-framework:
+
+`lifecycle_before_create` - Record without an ID. Values altered on this record in the lifecycle hook will be persisted to the DB.
+
+`lifecycle_after_create` - Record with an ID, as returned from the database.
+
+`lifecycle_before_update` - A key-values dictionary to be applied to the database, and the primary key id of the record which will be updated. Values altered in the dictionary will be applied to the DB update.
+
+`lifecycle_after_update` - Record with an ID, as returned from the database
+
+`lifecycle_before_delete` - Record with an ID, as returned from the database.
+
+`lifecycle_after_delete` - Record with an ID, as returned from the database. This record no longer exists in the database.
+
+`lifecycle_before_get_one` - A primary key value that will be used to fetch the record from the database.
+
+`lifecycle_after_get_one` - Record with an ID, as returned from the database.
+
+`lifecycle_before_get_all` - Recieves a query configuration object. Any user-space modifications to this object will impact the query made by fastapi-cruddy-framework. This method is also invoked when a foreign Resource queries a relationship that affects the Resource where you plug in this hook.
+
+`lifecycle_after_get_all` - Receives a BulkDTO object, containing the database objects retrieved by a get_all query, as well as the query metadata. This method is also invoked when a foreign Resource queries a relationship that affects the Resource where you plug in this hook.
+
+`lifecycle_before_set_relations` - Receives a relationship configuration object which containts information about the record id affected, the relationship being altered, and the new list of relations for this relationship type.
+```
+{
+    "id": id, # The database id whos relationship are about to be altered (of your defined PK type)
+    "relation": relation, # The relationship that is about to change (string)
+    "relations": relations # An array of foreign ids that will now define this relationship (Framework will attempt to discard old relations)
+}
+```
+
+`lifecycle_after_set_relations` - Receives a completed mapping of the affected relational change, which can be used to echo changes to other databases or services.
+
+```
+{
+    "model": model, # The CruddyModel affected by this relationship change
+    "relation_conf": relation_conf, # The configuration object from lifecycle_before_set_relations
+    "relation_type": MANYTOMANY, # An SQL Alchemy relationship-type identifier (MANYTOMANY or ONETOMANY)
+    "related_table": foreign_table, # The table that ultimately represents the far-side of this relationship (not the join table!)
+    "related_field": field_name, # The field on the related_table that represents the far side of the relationship
+    "updated_db_count": result # The number of records now in the database associated with this relationship. If the number is different than the length of relation_conf.relations, you probably have a non-nullable field on the far-side of this relationship.
+}
+```
 
 Resource Definition Options (And Defaults!):
 ```python
 id_type: Union[Type[int], Type[UUID]] = int,
 # You SHOULD pass in 'adapter'
 adapter: Union[BaseAdapter, SqliteAdapter, MysqlAdapter, PostgresqlAdapter, None] = None,
 # The following adapter specific options will probably get removed. You don't need to pass them in.
```

#### html2text {}

```diff
@@ -125,29 +125,70 @@
 automatically gain "shadow" properties where one-to-many and many-to-many
 relationships exist. These properties expect a client to send a list of IDs
 that specify the foreign records that relate to the target record. So - if a
 user is a member of many groups, and a group can have many users, you could
 update the users in a group by sending a property `"users": [1,2,3,4,5]` within
 the `group` payload object you send to the `POST /groups` or `PATCH /groups`
 routes/actions. It will all be clear when you look at the SWAGGER docs
-generated for your API. Resource Definition Options (And Defaults!): ```python
-id_type: Union[Type[int], Type[UUID]] = int, # You SHOULD pass in 'adapter'
-adapter: Union[BaseAdapter, SqliteAdapter, MysqlAdapter, PostgresqlAdapter,
-None] = None, # The following adapter specific options will probably get
-removed. You don't need to pass them in. # They exist solely in the event you
-are defining disparate resources and want the resources to # automatically
-build their own adapters. This is probably not a great idea. adapter_type:
-Literal["mysql", "postgresql"] = "postgresql", db_mode: Literal["memory",
-"file"] = "memory", db_path: Union[str, None] = None, connection_uri="",
-pool_size=4, max_overflow=64, # link_prefix will be applied at the beginning of
-each relationship link on each record. # This can help with things like sub-
-domains, or CORS with your API, and will allow you # to point your
-relationships endpoints at a complete URL. You could pass in something like #
-https://api.mydomain.com, which would make a relationship link look like #
-https://api.mydomain.com/resource/{id}/relationship link_prefix="", # Path
+generated for your API. Lifecycle hooks The following lifecycle hook methods,
+which can be defined in user-space code, receive the following information from
+fastapi-cruddy-framework: `lifecycle_before_create` - Record without an ID.
+Values altered on this record in the lifecycle hook will be persisted to the
+DB. `lifecycle_after_create` - Record with an ID, as returned from the
+database. `lifecycle_before_update` - A key-values dictionary to be applied to
+the database, and the primary key id of the record which will be updated.
+Values altered in the dictionary will be applied to the DB update.
+`lifecycle_after_update` - Record with an ID, as returned from the database
+`lifecycle_before_delete` - Record with an ID, as returned from the database.
+`lifecycle_after_delete` - Record with an ID, as returned from the database.
+This record no longer exists in the database. `lifecycle_before_get_one` - A
+primary key value that will be used to fetch the record from the database.
+`lifecycle_after_get_one` - Record with an ID, as returned from the database.
+`lifecycle_before_get_all` - Recieves a query configuration object. Any user-
+space modifications to this object will impact the query made by fastapi-
+cruddy-framework. This method is also invoked when a foreign Resource queries a
+relationship that affects the Resource where you plug in this hook.
+`lifecycle_after_get_all` - Receives a BulkDTO object, containing the database
+objects retrieved by a get_all query, as well as the query metadata. This
+method is also invoked when a foreign Resource queries a relationship that
+affects the Resource where you plug in this hook.
+`lifecycle_before_set_relations` - Receives a relationship configuration object
+which containts information about the record id affected, the relationship
+being altered, and the new list of relations for this relationship type. ```
+{ "id": id, # The database id whos relationship are about to be altered (of
+your defined PK type) "relation": relation, # The relationship that is about to
+change (string) "relations": relations # An array of foreign ids that will now
+define this relationship (Framework will attempt to discard old relations) }
+``` `lifecycle_after_set_relations` - Receives a completed mapping of the
+affected relational change, which can be used to echo changes to other
+databases or services. ``` { "model": model, # The CruddyModel affected by this
+relationship change "relation_conf": relation_conf, # The configuration object
+from lifecycle_before_set_relations "relation_type": MANYTOMANY, # An SQL
+Alchemy relationship-type identifier (MANYTOMANY or ONETOMANY) "related_table":
+foreign_table, # The table that ultimately represents the far-side of this
+relationship (not the join table!) "related_field": field_name, # The field on
+the related_table that represents the far side of the relationship
+"updated_db_count": result # The number of records now in the database
+associated with this relationship. If the number is different than the length
+of relation_conf.relations, you probably have a non-nullable field on the far-
+side of this relationship. } ``` Resource Definition Options (And Defaults!):
+```python id_type: Union[Type[int], Type[UUID]] = int, # You SHOULD pass in
+'adapter' adapter: Union[BaseAdapter, SqliteAdapter, MysqlAdapter,
+PostgresqlAdapter, None] = None, # The following adapter specific options will
+probably get removed. You don't need to pass them in. # They exist solely in
+the event you are defining disparate resources and want the resources to #
+automatically build their own adapters. This is probably not a great idea.
+adapter_type: Literal["mysql", "postgresql"] = "postgresql", db_mode: Literal
+["memory", "file"] = "memory", db_path: Union[str, None] = None,
+connection_uri="", pool_size=4, max_overflow=64, # link_prefix will be applied
+at the beginning of each relationship link on each record. # This can help with
+things like sub-domains, or CORS with your API, and will allow you # to point
+your relationships endpoints at a complete URL. You could pass in something
+like # https://api.mydomain.com, which would make a relationship link look like
+# https://api.mydomain.com/resource/{id}/relationship link_prefix="", # Path
 specifies where this resource resides within the API. This is generated for you
 by # default. Only change if you know what you are doing. Ember.js would expect
 a resource path # to be the pluralized name of its base model. So a 'user'
 resource should be accessible at # '/users', and all of its sub-routes and
 actions are nested under that route. path: str = None, # The "tags" list
 corresponds with the fastapi "tags" list. You can alter this if needed. # It is
 defined for you initially as the singular name of your resource model. User -
```

### Comparing `fastapi_cruddy_framework-0.0.6/fastapi_cruddy_framework/__init__.py` & `fastapi_cruddy_framework-0.0.7/fastapi_cruddy_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-0.0.6/fastapi_cruddy_framework/adapters.py` & `fastapi_cruddy_framework-0.0.7/fastapi_cruddy_framework/adapters.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-0.0.6/fastapi_cruddy_framework/controller.py` & `fastapi_cruddy_framework-0.0.7/fastapi_cruddy_framework/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -386,15 +386,14 @@
         result = await repository.create(data=the_thing)
         relations_modified = await SaveRelationships(
             id=getattr(result, repository.primary_key),
             record=the_thing_with_rels,
             relation_config_map=relations,
             repository=repository,
         )
-        # print(f"modified {relations_modified} relationships")
         # Add error logic?
         return single_schema(data=result)
 
     @controller.patch(
         "/{id}",
         response_model=single_schema,
         response_model_exclude_none=True,
@@ -406,15 +405,14 @@
         result = await repository.update(id=id, data=the_thing)
         relations_modified = await SaveRelationships(
             id=getattr(result, repository.primary_key),
             record=the_thing_with_rels,
             relation_config_map=relations,
             repository=repository,
         )
-        # print(f"modified {relations_modified} relationships")
         # Add error logic?
         return single_schema(data=result)
 
     @controller.delete(
         "/{id}",
         response_model=single_schema,
         response_model_exclude_none=True,
```

### Comparing `fastapi_cruddy_framework-0.0.6/fastapi_cruddy_framework/repository.py` & `fastapi_cruddy_framework-0.0.7/fastapi_cruddy_framework/repository.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import math
+from logging import getLogger
 from sqlalchemy import (
     update as _update,
     delete as _delete,
     or_,
     and_,
     not_,
     func,
     column,
 )
 from sqlalchemy.sql import select, update
 from sqlalchemy.sql.schema import Table, Column
-from sqlalchemy.orm import RelationshipProperty
+from sqlalchemy.orm import RelationshipProperty, ONETOMANY, MANYTOMANY
 from sqlmodel import inspect
 from typing import Union, List, Dict
 from pydantic.types import Json
 from .schemas import (
     BulkDTO,
     CruddyModel,
 )
@@ -22,14 +23,17 @@
 from .util import get_pk, possible_id_types, lifecycle_types
 
 
 def exists(something):
     return something != None
 
 
+LOGGER = getLogger(__file__)
+
+
 # -------------------------------------------------------------------------------------------
 # REPOSITORY MANAGER
 # -------------------------------------------------------------------------------------------
 class AbstractRepository:
     adapter: Union[BaseAdapter, SqliteAdapter, MysqlAdapter, PostgresqlAdapter]
     update_model: CruddyModel
     create_model: CruddyModel
@@ -446,15 +450,24 @@
                 )
                 count_query = select(func.count(1)).select_from(find_tgt_query)
                 result = (await session.execute(count_query)).scalar() or 0
             else:
                 result = 0
 
         if exists(self.lifecycle["after_set_relations"]):
-            await self.lifecycle["after_set_relations"](result)
+            await self.lifecycle["after_set_relations"](
+                {
+                    "model": self.model,
+                    "relation_conf": relation_conf,
+                    "relation_type": MANYTOMANY,
+                    "related_table": foreign_table,
+                    "related_field": validation_target_col.name,
+                    "updated_db_count": result,
+                }
+            )
 
         return result
 
     # There should probably be a configuration flag to disable this form of unsafe relationship update
     async def set_one_many_relations(
         self,
         id: possible_id_types,
@@ -465,19 +478,33 @@
 
         if exists(self.lifecycle["before_set_relations"]):
             await self.lifecycle["before_set_relations"](relation_conf)
 
         model_relation: RelationshipProperty = getattr(
             inspect(self.model).relationships, relation_conf["relation"]
         )
-        related_model = model_relation.foreign_resource.repository.model
-        related_model_pk = get_pk(related_model)
-        related_model_id: Column = getattr(related_model, related_model_pk)
-        far_col: Column = next(iter(model_relation.orm_relationship.remote_side))
-        far_col_name = far_col.name
+        pairs = list(model_relation.local_remote_pairs)
+        found = False
+        for v in pairs:
+            local: Column = v[0]
+            remote: Column = v[1]
+            if local.table.name == self.model.__tablename__:
+                related_model: Table = remote.table
+                far_col_name: str = remote.key
+                far_col = remote
+                found = True
+                # origin_table = local.table
+                # origin_key = local.key
+                # This is the link from our origin model to the join table
+        if not found:
+            raise RuntimeError(
+                "This should be impossible, but there was not a valid one-to-many relationship"
+            )
+
+        rel_pk, related_model_id = related_model.primary_key.columns.items()[0]
 
         clear_query = (
             update(table=related_model)
             .values({far_col_name: None})
             .where(far_col.in_([relation_conf["id"]]))
         )
         alter_query = (
@@ -489,30 +516,38 @@
         find_tgt_query = select(related_model).where(
             and_(
                 far_col == relation_conf["id"],
                 related_model_id.in_(relation_conf["relations"]),
             )
         )
         count_query = select(func.count(1)).select_from(find_tgt_query)
-
         async with self.adapter.getSession() as session:
             if far_col.nullable:
                 await session.execute(clear_query)
             else:
-                print(
-                    f"Unable to clear relations for {related_model.__name__}.{far_col_name}. Column does not allow null values"
+                LOGGER.warn(
+                    f"Unable to clear relations for {related_model.name}.{far_col_name}. Column does not allow null values"
                 )
 
             await session.execute(
                 alter_query
             )  # .rowcount # also affected by removing returning
             alter_result = (await session.execute(count_query)).scalar() or 0
 
         if exists(self.lifecycle["after_set_relations"]):
-            await self.lifecycle["after_set_relations"](alter_result)
+            await self.lifecycle["after_set_relations"](
+                {
+                    "model": self.model,
+                    "relation_conf": relation_conf,
+                    "relation_type": ONETOMANY,
+                    "related_table": related_model,
+                    "related_field": far_col_name,
+                    "updated_db_count": alter_result,
+                }
+            )
 
         return alter_result
 
     # Initial, simple, query forge. Invalid attrs or ops are just dropped.
     # Improvements to make:
     # 1. Table joins for relationships.
     # 2. Make relationships searchable too!
```

### Comparing `fastapi_cruddy_framework-0.0.6/fastapi_cruddy_framework/resource.py` & `fastapi_cruddy_framework-0.0.7/fastapi_cruddy_framework/resource.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-0.0.6/fastapi_cruddy_framework/router.py` & `fastapi_cruddy_framework-0.0.7/fastapi_cruddy_framework/router.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-0.0.6/fastapi_cruddy_framework/schemas.py` & `fastapi_cruddy_framework-0.0.7/fastapi_cruddy_framework/schemas.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-0.0.6/fastapi_cruddy_framework/uuid.py` & `fastapi_cruddy_framework-0.0.7/fastapi_cruddy_framework/uuid.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-0.0.6/pyproject.toml` & `fastapi_cruddy_framework-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-cruddy-framework"
-version = "0.0.6"
+version = "0.0.7"
 description = "A holistic CRUD/MVC framework for FastAPI, with endpoint policies and relationships"
 authors = ["mdconaway <mdconaway@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "fastapi_cruddy_framework"}]
 homepage = "https://github.com/mdconaway/fastapi-cruddy-framework"
 repository = "https://github.com/mdconaway/fastapi-cruddy-framework"
 keywords = ["fastapi", "crud", "mvc", "orm", "ember", "sails", "json"]
```

### Comparing `fastapi_cruddy_framework-0.0.6/PKG-INFO` & `fastapi_cruddy_framework-0.0.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-cruddy-framework
-Version: 0.0.6
+Version: 0.0.7
 Summary: A holistic CRUD/MVC framework for FastAPI, with endpoint policies and relationships
 Home-page: https://github.com/mdconaway/fastapi-cruddy-framework
 Keywords: fastapi,crud,mvc,orm,ember,sails,json
 Author: mdconaway
 Author-email: mdconaway@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -211,14 +211,59 @@
 
 <b>Updating Relationships:</b>
 * You can update relationships via either CREATE or UPDATE actions against each base resource! 
 
 
 As you will discover, your resource's create and update models will automatically gain "shadow" properties where one-to-many and many-to-many relationships exist. These properties expect a client to send a list of IDs that specify the foreign records that relate to the target record. So - if a user is a member of many groups, and a group can have many users, you could update the users in a group by sending a property `"users": [1,2,3,4,5]` within the `group` payload object you send to the `POST /groups` or `PATCH /groups` routes/actions. It will all be clear when you look at the SWAGGER docs generated for your API.
 
+<b>Lifecycle hooks</b>
+
+The following lifecycle hook methods, which can be defined in user-space code, receive the following information from fastapi-cruddy-framework:
+
+`lifecycle_before_create` - Record without an ID. Values altered on this record in the lifecycle hook will be persisted to the DB.
+
+`lifecycle_after_create` - Record with an ID, as returned from the database.
+
+`lifecycle_before_update` - A key-values dictionary to be applied to the database, and the primary key id of the record which will be updated. Values altered in the dictionary will be applied to the DB update.
+
+`lifecycle_after_update` - Record with an ID, as returned from the database
+
+`lifecycle_before_delete` - Record with an ID, as returned from the database.
+
+`lifecycle_after_delete` - Record with an ID, as returned from the database. This record no longer exists in the database.
+
+`lifecycle_before_get_one` - A primary key value that will be used to fetch the record from the database.
+
+`lifecycle_after_get_one` - Record with an ID, as returned from the database.
+
+`lifecycle_before_get_all` - Recieves a query configuration object. Any user-space modifications to this object will impact the query made by fastapi-cruddy-framework. This method is also invoked when a foreign Resource queries a relationship that affects the Resource where you plug in this hook.
+
+`lifecycle_after_get_all` - Receives a BulkDTO object, containing the database objects retrieved by a get_all query, as well as the query metadata. This method is also invoked when a foreign Resource queries a relationship that affects the Resource where you plug in this hook.
+
+`lifecycle_before_set_relations` - Receives a relationship configuration object which containts information about the record id affected, the relationship being altered, and the new list of relations for this relationship type.
+```
+{
+    "id": id, # The database id whos relationship are about to be altered (of your defined PK type)
+    "relation": relation, # The relationship that is about to change (string)
+    "relations": relations # An array of foreign ids that will now define this relationship (Framework will attempt to discard old relations)
+}
+```
+
+`lifecycle_after_set_relations` - Receives a completed mapping of the affected relational change, which can be used to echo changes to other databases or services.
+
+```
+{
+    "model": model, # The CruddyModel affected by this relationship change
+    "relation_conf": relation_conf, # The configuration object from lifecycle_before_set_relations
+    "relation_type": MANYTOMANY, # An SQL Alchemy relationship-type identifier (MANYTOMANY or ONETOMANY)
+    "related_table": foreign_table, # The table that ultimately represents the far-side of this relationship (not the join table!)
+    "related_field": field_name, # The field on the related_table that represents the far side of the relationship
+    "updated_db_count": result # The number of records now in the database associated with this relationship. If the number is different than the length of relation_conf.relations, you probably have a non-nullable field on the far-side of this relationship.
+}
+```
 
 Resource Definition Options (And Defaults!):
 ```python
 id_type: Union[Type[int], Type[UUID]] = int,
 # You SHOULD pass in 'adapter'
 adapter: Union[BaseAdapter, SqliteAdapter, MysqlAdapter, PostgresqlAdapter, None] = None,
 # The following adapter specific options will probably get removed. You don't need to pass them in.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi-cruddy-framework Version: 0.0.6 Summary: A
+Metadata-Version: 2.1 Name: fastapi-cruddy-framework Version: 0.0.7 Summary: A
 holistic CRUD/MVC framework for FastAPI, with endpoint policies and
 relationships Home-page: https://github.com/mdconaway/fastapi-cruddy-framework
 Keywords: fastapi,crud,mvc,orm,ember,sails,json Author: mdconaway Author-email:
 mdconaway@users.noreply.github.com Requires-Python: >=3.8,<4.0 Classifier:
 Development Status :: 4 - Beta Classifier: Environment :: Web Environment
 Classifier: Framework :: FastAPI Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
@@ -143,29 +143,70 @@
 automatically gain "shadow" properties where one-to-many and many-to-many
 relationships exist. These properties expect a client to send a list of IDs
 that specify the foreign records that relate to the target record. So - if a
 user is a member of many groups, and a group can have many users, you could
 update the users in a group by sending a property `"users": [1,2,3,4,5]` within
 the `group` payload object you send to the `POST /groups` or `PATCH /groups`
 routes/actions. It will all be clear when you look at the SWAGGER docs
-generated for your API. Resource Definition Options (And Defaults!): ```python
-id_type: Union[Type[int], Type[UUID]] = int, # You SHOULD pass in 'adapter'
-adapter: Union[BaseAdapter, SqliteAdapter, MysqlAdapter, PostgresqlAdapter,
-None] = None, # The following adapter specific options will probably get
-removed. You don't need to pass them in. # They exist solely in the event you
-are defining disparate resources and want the resources to # automatically
-build their own adapters. This is probably not a great idea. adapter_type:
-Literal["mysql", "postgresql"] = "postgresql", db_mode: Literal["memory",
-"file"] = "memory", db_path: Union[str, None] = None, connection_uri="",
-pool_size=4, max_overflow=64, # link_prefix will be applied at the beginning of
-each relationship link on each record. # This can help with things like sub-
-domains, or CORS with your API, and will allow you # to point your
-relationships endpoints at a complete URL. You could pass in something like #
-https://api.mydomain.com, which would make a relationship link look like #
-https://api.mydomain.com/resource/{id}/relationship link_prefix="", # Path
+generated for your API. Lifecycle hooks The following lifecycle hook methods,
+which can be defined in user-space code, receive the following information from
+fastapi-cruddy-framework: `lifecycle_before_create` - Record without an ID.
+Values altered on this record in the lifecycle hook will be persisted to the
+DB. `lifecycle_after_create` - Record with an ID, as returned from the
+database. `lifecycle_before_update` - A key-values dictionary to be applied to
+the database, and the primary key id of the record which will be updated.
+Values altered in the dictionary will be applied to the DB update.
+`lifecycle_after_update` - Record with an ID, as returned from the database
+`lifecycle_before_delete` - Record with an ID, as returned from the database.
+`lifecycle_after_delete` - Record with an ID, as returned from the database.
+This record no longer exists in the database. `lifecycle_before_get_one` - A
+primary key value that will be used to fetch the record from the database.
+`lifecycle_after_get_one` - Record with an ID, as returned from the database.
+`lifecycle_before_get_all` - Recieves a query configuration object. Any user-
+space modifications to this object will impact the query made by fastapi-
+cruddy-framework. This method is also invoked when a foreign Resource queries a
+relationship that affects the Resource where you plug in this hook.
+`lifecycle_after_get_all` - Receives a BulkDTO object, containing the database
+objects retrieved by a get_all query, as well as the query metadata. This
+method is also invoked when a foreign Resource queries a relationship that
+affects the Resource where you plug in this hook.
+`lifecycle_before_set_relations` - Receives a relationship configuration object
+which containts information about the record id affected, the relationship
+being altered, and the new list of relations for this relationship type. ```
+{ "id": id, # The database id whos relationship are about to be altered (of
+your defined PK type) "relation": relation, # The relationship that is about to
+change (string) "relations": relations # An array of foreign ids that will now
+define this relationship (Framework will attempt to discard old relations) }
+``` `lifecycle_after_set_relations` - Receives a completed mapping of the
+affected relational change, which can be used to echo changes to other
+databases or services. ``` { "model": model, # The CruddyModel affected by this
+relationship change "relation_conf": relation_conf, # The configuration object
+from lifecycle_before_set_relations "relation_type": MANYTOMANY, # An SQL
+Alchemy relationship-type identifier (MANYTOMANY or ONETOMANY) "related_table":
+foreign_table, # The table that ultimately represents the far-side of this
+relationship (not the join table!) "related_field": field_name, # The field on
+the related_table that represents the far side of the relationship
+"updated_db_count": result # The number of records now in the database
+associated with this relationship. If the number is different than the length
+of relation_conf.relations, you probably have a non-nullable field on the far-
+side of this relationship. } ``` Resource Definition Options (And Defaults!):
+```python id_type: Union[Type[int], Type[UUID]] = int, # You SHOULD pass in
+'adapter' adapter: Union[BaseAdapter, SqliteAdapter, MysqlAdapter,
+PostgresqlAdapter, None] = None, # The following adapter specific options will
+probably get removed. You don't need to pass them in. # They exist solely in
+the event you are defining disparate resources and want the resources to #
+automatically build their own adapters. This is probably not a great idea.
+adapter_type: Literal["mysql", "postgresql"] = "postgresql", db_mode: Literal
+["memory", "file"] = "memory", db_path: Union[str, None] = None,
+connection_uri="", pool_size=4, max_overflow=64, # link_prefix will be applied
+at the beginning of each relationship link on each record. # This can help with
+things like sub-domains, or CORS with your API, and will allow you # to point
+your relationships endpoints at a complete URL. You could pass in something
+like # https://api.mydomain.com, which would make a relationship link look like
+# https://api.mydomain.com/resource/{id}/relationship link_prefix="", # Path
 specifies where this resource resides within the API. This is generated for you
 by # default. Only change if you know what you are doing. Ember.js would expect
 a resource path # to be the pluralized name of its base model. So a 'user'
 resource should be accessible at # '/users', and all of its sub-routes and
 actions are nested under that route. path: str = None, # The "tags" list
 corresponds with the fastapi "tags" list. You can alter this if needed. # It is
 defined for you initially as the singular name of your resource model. User -
```

