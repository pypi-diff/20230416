# Comparing `tmp/pydbantic-0.0.8-py3-none-any.whl.zip` & `tmp/pydbantic-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 18830 bytes, number of entries: 10
--rw-r--r--  2.0 unx       83 b- defN 21-Nov-09 09:24 pydbantic/__init__.py
--rw-r--r--  2.0 unx     5108 b- defN 21-Nov-09 09:24 pydbantic/cache.py
--rw-r--r--  2.0 unx    18711 b- defN 21-Nov-09 09:24 pydbantic/core.py
--rw-r--r--  2.0 unx    19847 b- defN 21-Nov-09 09:24 pydbantic/database.py
--rw-r--r--  2.0 unx     3266 b- defN 21-Nov-09 09:24 pydbantic/translations.py
--rw-r--r--  2.0 unx    11357 b- defN 21-Nov-09 09:24 pydbantic-0.0.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     8452 b- defN 21-Nov-09 09:24 pydbantic-0.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 21-Nov-09 09:24 pydbantic-0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 21-Nov-09 09:24 pydbantic-0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      784 b- defN 21-Nov-09 09:24 pydbantic-0.0.8.dist-info/RECORD
-10 files, 67710 bytes uncompressed, 17506 bytes compressed:  74.1%
+Zip file size: 18806 bytes, number of entries: 10
+-rw-r--r--  2.0 unx       83 b- defN 21-Nov-09 20:32 pydbantic/__init__.py
+-rw-r--r--  2.0 unx     5005 b- defN 21-Nov-09 20:32 pydbantic/cache.py
+-rw-r--r--  2.0 unx    18587 b- defN 21-Nov-09 20:32 pydbantic/core.py
+-rw-r--r--  2.0 unx    19847 b- defN 21-Nov-09 20:32 pydbantic/database.py
+-rw-r--r--  2.0 unx     3266 b- defN 21-Nov-09 20:32 pydbantic/translations.py
+-rw-r--r--  2.0 unx    11357 b- defN 21-Nov-09 20:32 pydbantic-0.0.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8452 b- defN 21-Nov-09 20:32 pydbantic-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 21-Nov-09 20:32 pydbantic-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 21-Nov-09 20:32 pydbantic-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      784 b- defN 21-Nov-09 20:32 pydbantic-0.0.9.dist-info/RECORD
+10 files, 67483 bytes uncompressed, 17482 bytes compressed:  74.1%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: pydbantic/database.py
 Comment: 
 
 Filename: pydbantic/translations.py
 Comment: 
 
-Filename: pydbantic-0.0.8.dist-info/LICENSE
+Filename: pydbantic-0.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: pydbantic-0.0.8.dist-info/METADATA
+Filename: pydbantic-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: pydbantic-0.0.8.dist-info/WHEEL
+Filename: pydbantic-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: pydbantic-0.0.8.dist-info/top_level.txt
+Filename: pydbantic-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: pydbantic-0.0.8.dist-info/RECORD
+Filename: pydbantic-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pydbantic/cache.py

```diff
@@ -61,41 +61,41 @@
         self.flags = {}
 
         self.log = log
     def invalidate(self, flag: str):
         """
         invalidates cache flagged input flag str
         """
-        if not flag in self.flags:
+        if flag not in self.flags:
             return
         for timestamp in self.flags[flag]:
-            if not timestamp in  self.timestamp_to_cache:
+            if timestamp not in self.timestamp_to_cache:
                 continue
             _,cached_key, _ = self.timestamp_to_cache[timestamp]
             del self.timestamp_to_cache[timestamp]
             del self.cache[cached_key]
         del self.flags[flag]
     def check_size_and_clear(self):
         if len(self.timestamp_to_cache) < self.size:
             return
         while len(self.timestamp_to_cache) >= self.size:
             cache_time = self.access_history.popleft()
-            if not cache_time in self.timestamp_to_cache:
+            if cache_time not in self.timestamp_to_cache:
                 continue
             _, cache_key, _ = self.timestamp_to_cache[cache_time]
             del self.timestamp_to_cache[cache_time]
-            if cache_key in self.cache and not self.cache[cache_key] == cache_time:
+            if cache_key in self.cache and self.cache[cache_key] != cache_time:
                 continue
             del self.cache[cache_key]
             self.log.debug(f"# cach_key '{cache_key}' cleared due to cache length of {self.size} exceeded")
 
     def update_timestamp(self, cached_key, flag):
-        if not cached_key in self:
+        if cached_key not in self:
             return
-        
+
         old_time = self.cache[cached_key]
         new_time = time.time()
 
         self.timestamp_to_cache[new_time] = self.timestamp_to_cache[old_time]
         del self.timestamp_to_cache[old_time]
 
         self.cache[cached_key] = new_time
@@ -104,62 +104,59 @@
     def __iter__(self):
         return (
             (cache_key, self.timestamp_to_cache[timestamp][0]) 
             for cache_key, timestamp in self.cache.copy().items()
         )
 
     def __getitem__(self, cached_key):
-        if not cached_key in self:
+        if cached_key not in self:
             return None
 
         cache_time = self.cache[cached_key]
-        if not cache_time in self.timestamp_to_cache:
+        if cache_time not in self.timestamp_to_cache:
             del self.cache[cached_key]
             return None
 
         cache_row, _, flag = self.timestamp_to_cache[cache_time]
         self.update_timestamp(cached_key, flag)
         return cache_row
 
     def __setitem__(self, cached_key, row_and_flag: tuple):
         row, flag = row_and_flag
         cache_time = time.time()
         if cached_key in self.cache:
             old_cache_time = self.cache[cached_key]
             del self.timestamp_to_cache[old_cache_time]
-        
+
         self.cache[cached_key] = cache_time
         self.timestamp_to_cache[cache_time] = (row, cached_key, flag)
         if flag:
-            if not flag in self.flags:
+            if flag not in self.flags:
                 self.flags[flag] = set()
             self.flags[flag].add(cache_time)
-            
+
         self.access_history.append(cache_time)
         self.check_size_and_clear()
 
     def __delitem__(self, cached_key) -> None:
-        if not cached_key in self.cache:
-            return
-        
-        if not cached_key in self.cache:
+        if cached_key not in self.cache:
             return
 
         cache_time = self.cache.pop(cached_key)
         if cache_time in self.timestamp_to_cache:
             del self.timestamp_to_cache[cache_time]
 
     def __contains__(self, cached_key):
         return cached_key in self.cache
 
 async def cache_main():
     cache = Redis()
     await cache.set('test', ('value', 'test_flag'))
     cache_result = await cache.get('test')
-    print(f"cache_result", cache_result)
+    print('cache_result', cache_result)
 
 
 if __name__ == '__main__':
     cache = Cache(size=50)
     for i in range(100):
         cache[i] = i, 'test'
```

## pydbantic/core.py

```diff
@@ -67,15 +67,15 @@
 
     @classmethod
     def setup(cls, database):
         
         if not hasattr(cls.__metadata__, 'metadata'):
             cls.init_set_metadata(database.metadata)
             cls.init_set_database(database)
-        if not cls.__name__ in cls.__metadata__.tables:
+        if cls.__name__ not in cls.__metadata__.tables:
             cls.generate_sqlalchemy_table()
         
     @classmethod
     def init_set_metadata(cls, metadata):
         """
         Applies an instantiated sqlalchemy.MetaData() instance to __metadata__.metadata
         """
@@ -109,15 +109,14 @@
         update: bool = False
     ):
         """
         primary key is assumed to be first field, #TODO - add override later
         """
         if not alias:
             alias = {}
-        
         if not include:
             include = [f for f in cls.__fields__]
 
         primary_key = None
         for property, config in cls.schema()['properties'].items():
             if 'primary_key' in config:
                 if primary_key:
@@ -134,16 +133,16 @@
                 field_name = field.name
                 if field.name in alias:
                     field_name = alias[field.name]
                 model_fields.append({'name': field_name, 'type': field.type_, 'required': field.required})
 
         name = cls.__name__
         primary_key = model_fields[0]['name'] if not primary_key else primary_key
-        if not name in cls.__metadata__.tables or update:
-            
+        if name not in cls.__metadata__.tables or update:
+
             cls.__metadata__.tables[name] = {
                 'primary_key': primary_key,
                 'column_map': {},
                 'foreign_keys': {},
             }
 
         columns = []
@@ -203,15 +202,15 @@
                     column_type_config['column_type'](
                         *column_type_config['args'], 
                         **column_type_config['kwargs']
                     ),
                     primary_key = field['name'] == primary_key
                 )
             )
-        
+
         return columns
     
     @classmethod
     def normalize(cls, results: list):
         """
         ensure results of db querries are dict before parsing
         """
@@ -272,60 +271,58 @@
         for cond, value in where.items():
             # check if cond is a foreign key, handle pulling foreign references matching query
             if cond in cls.__metadata__.tables[cls.__name__]['foreign_keys']:
                 foreign_column_name = cls.__metadata__.tables[cls.__name__]['foreign_keys'][cond]
                 foreign_primary_key = cls.__metadata__.tables[value.__class__.__name__]['primary_key']
                 conditions.append(table.c[foreign_column_name]==getattr(value, foreign_primary_key))
                 continue
-            if not cond in table.c:
+            if cond not in table.c:
                 raise Exception(f"{cond} is not a valid column in {table}")
             query_value = value
-            
+
             serialized = cls.__metadata__.tables[cls.__name__]['column_map'][cond][2]
 
             if serialized:
                 query_value = dumps(value)
 
             conditions.append(table.c[cond] == query_value)
             values.append(query_value)
         for condition in conditions:
             query = query.where(condition)
         return query, tuple(values)
 
     @classmethod
     def get_table(cls):
-        if not cls.__name__ in cls.__metadata__.tables:
+        if cls.__name__ not in cls.__metadata__.tables:
             cls.generate_sqlalchemy_table()
 
         return cls.__metadata__.tables[cls.__name__]['table']
 
     @classmethod
     async def exists(cls,
         **column_values: dict
     ) -> bool:
 
         table = cls.get_table()
         primary_key = cls.__metadata__.tables[cls.__name__]['primary_key']
 
         for k in column_values:
-            if not k in table.c:
+            if k not in table.c:
                 raise Exception(f"{k} is not a valid column in  {table} ")
-        
-        
+
+
         sel = select([table.c[primary_key]])
 
         sel, values = cls.where(sel, column_values)
 
         database = cls.__metadata__.database
 
         results = await database.fetch(sel, cls.__name__, values)
 
-        if results:
-            return True
-        return False
+        return bool(results)
         
     @classmethod
     async def select(cls,
         *selection,
         where: Optional[Union[dict, None]] = None,
         alias: Optional[dict] = None,
     ) -> List[dict]:
@@ -456,29 +453,29 @@
         table_name = self.__class__.__name__
         primary_key = self.__metadata__.tables[table_name]['primary_key']
 
         if not to_update:
             to_update = self.dict()
             del to_update[primary_key]
 
-        where_ = dict(*where if where else {})
+        where_ = dict(*where or {})
         if not where_:
             where_ = {primary_key: getattr(self, primary_key)}
 
         table = self.__metadata__.tables[self.__class__.__name__]['table']
         for column in to_update.copy():
             if column in self.__metadata__.tables[table_name]['foreign_keys']:
                 del to_update[column] # = foreign_pk_value
                 continue
             if column not in table.c:
                 raise Exception(f"{column} is not a valid column in {table}")
-        
+
         query, _ = self.where(table.update(), where_)
         query = query.values(**to_update)
-        
+
         to_update = await self.serialize(to_update)
 
         await self.__metadata__.database.execute(query, to_update)
 
             
     async def delete(self):
         table_name = self.__class__.__name__
@@ -499,15 +496,15 @@
             query, values
         )
 
     @classmethod
     async def get(cls, **p_key):
         for k in p_key:
             primary_key = cls.__metadata__.tables[cls.__name__]['primary_key']
-            if not k == cls.__metadata__.tables[cls.__name__]['primary_key']:
+            if k != cls.__metadata__.tables[cls.__name__]['primary_key']:
                 raise f"Expected primary key {primary_key}=<value>"
         result = await cls.select('*', where={**p_key})
         return result[0] if result else None
 
     @classmethod
     async def create(cls, **column_args):
         new_obj = cls(**column_args)
```

## Comparing `pydbantic-0.0.8.dist-info/LICENSE` & `pydbantic-0.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pydbantic-0.0.8.dist-info/METADATA` & `pydbantic-0.0.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydbantic
-Version: 0.0.8
+Version: 0.0.9
 Summary: 'db' within pydantic - A single model for shaping, creating, accessing, storing data within a Database
 Home-page: https://github.com/codemation/pydbantic
 Author: Joshua Jamison
 Author-email: joshjamison1@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

