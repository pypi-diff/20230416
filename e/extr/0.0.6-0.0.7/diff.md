# Comparing `tmp/extr-0.0.6.tar.gz` & `tmp/extr-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extr-0.0.6.tar", last modified: Sat Apr 15 10:42:23 2023, max compression
+gzip compressed data, was "extr-0.0.7.tar", last modified: Sun Apr 16 18:50:49 2023, max compression
```

## Comparing `extr-0.0.6.tar` & `extr-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 10:42:23.587868 extr-0.0.6/
--rw-rw-rw-   0        0        0     2431 2023-04-15 10:42:23.584838 extr-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1580 2023-04-15 09:22:47.000000 extr-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-04-15 10:42:23.593986 extr-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      538 2023-04-15 10:41:45.000000 extr-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-15 10:42:23.174237 extr-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-04-15 10:42:23.363259 extr-0.0.6/src/extr/
--rw-rw-rw-   0        0        0      247 2023-04-13 10:55:50.000000 extr-0.0.6/src/extr/__init__.py
--rw-rw-rw-   0        0        0     1692 2023-04-13 10:18:22.000000 extr-0.0.6/src/extr/entities.py
--rw-rw-rw-   0        0        0      166 2023-04-12 10:31:30.000000 extr-0.0.6/src/extr/iterutils.py
--rw-rw-rw-   0        0        0     2261 2023-04-13 10:55:57.000000 extr-0.0.6/src/extr/models.py
--rw-rw-rw-   0        0        0     2510 2023-04-10 13:19:22.000000 extr-0.0.6/src/extr/regex.py
--rw-rw-rw-   0        0        0     1194 2023-04-12 10:32:54.000000 extr-0.0.6/src/extr/relations.py
-drwxrwxrwx   0        0        0        0 2023-04-15 10:42:23.579008 extr-0.0.6/src/extr.egg-info/
--rw-rw-rw-   0        0        0     2431 2023-04-15 10:42:22.000000 extr-0.0.6/src/extr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-04-15 10:42:23.000000 extr-0.0.6/src/extr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 10:42:22.000000 extr-0.0.6/src/extr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-04-15 10:42:22.000000 extr-0.0.6/src/extr.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 18:50:49.299183 extr-0.0.7/
+-rw-rw-rw-   0        0        0     2431 2023-04-16 18:50:49.299183 extr-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1580 2023-04-15 09:22:47.000000 extr-0.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-16 18:50:49.307184 extr-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      538 2023-04-16 18:50:30.000000 extr-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 18:50:49.061978 extr-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-04-16 18:50:49.122471 extr-0.0.7/src/extr/
+-rw-rw-rw-   0        0        0      247 2023-04-13 10:55:50.000000 extr-0.0.7/src/extr/__init__.py
+-rw-rw-rw-   0        0        0     1693 2023-04-16 18:19:36.000000 extr-0.0.7/src/extr/entities.py
+-rw-rw-rw-   0        0        0      166 2023-04-12 10:31:30.000000 extr-0.0.7/src/extr/iterutils.py
+-rw-rw-rw-   0        0        0     2263 2023-04-16 18:19:38.000000 extr-0.0.7/src/extr/models.py
+-rw-rw-rw-   0        0        0     2510 2023-04-10 13:19:22.000000 extr-0.0.7/src/extr/regex.py
+-rw-rw-rw-   0        0        0     1194 2023-04-12 10:32:54.000000 extr-0.0.7/src/extr/relations.py
+drwxrwxrwx   0        0        0        0 2023-04-16 18:50:49.291180 extr-0.0.7/src/extr.egg-info/
+-rw-rw-rw-   0        0        0     2431 2023-04-16 18:50:48.000000 extr-0.0.7/src/extr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-04-16 18:50:48.000000 extr-0.0.7/src/extr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 18:50:48.000000 extr-0.0.7/src/extr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-04-16 18:50:48.000000 extr-0.0.7/src/extr.egg-info/top_level.txt
```

### Comparing `extr-0.0.6/PKG-INFO` & `extr-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extr
-Version: 0.0.6
+Version: 0.0.7
 Summary: Named Entity Recognition (NER) and Relation Extraction (RE) library using Regular Expressions
 Home-page: https://github.com/dpasse/extr
 License: UNKNOWN
 Description: # Extr
         > Named Entity Recognition (NER) and Relation Extraction (RE) library using Regular Expressions
         
         <br />
```

### Comparing `extr-0.0.6/README.md` & `extr-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `extr-0.0.6/setup.py` & `extr-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name='extr',
-    version='0.0.6',
+    version='0.0.7',
     keywords='',
     description='Named Entity Recognition (NER) and Relation Extraction (RE) library using Regular Expressions',
     packages=setuptools.find_packages('src'),
     package_dir={'': 'src'},
     install_requires=[],
     url='https://github.com/dpasse/extr',
     long_description=long_description,
```

### Comparing `extr-0.0.6/src/extr/entities.py` & `extr-0.0.7/src/extr/entities.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,11 +40,11 @@
 class EntityAnnotator:
     def annotate(self, text: str, entities: List[Entity]) -> EntityAnnotationResults:
         def insert_entity(text: str, entity: Entity) -> str:
             return text[:entity.start] + str(entity) + text[entity.end:]
 
         annotated_text = text[:]
         for identifer, entity in enumerate(entities):
-            entity.identifer = identifer + 1
+            entity.identifier = identifer + 1
             annotated_text = insert_entity(annotated_text, entity)
 
         return EntityAnnotationResults(text, annotated_text, entities)
```

### Comparing `extr-0.0.6/src/extr/models.py` & `extr-0.0.7/src/extr/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,30 +42,30 @@
         return self.location.contains(other.location)
 
 @dataclass()
 class Entity(ILocation):
     label: str
     text: str
     location: Location
-    identifer: int = NOT_DEFINED_FLAG
+    identifier: int = NOT_DEFINED_FLAG
     attributes: Dict[str, Any] = field(default_factory=dict)
 
     @property
     def start(self) -> int:
         return self.location.start
 
     @property
     def end(self) -> int:
         return self.location.end
 
     def __repr__(self) -> str:
         return f'<Entity label="{self.label}" text="{self.text}" span={repr(self.location)}>'
 
     def __str__(self) -> str:
-        return f'##ENTITY_{self.label}_{self.identifer}##'
+        return f'##ENTITY_{self.label}_{self.identifier}##'
 
 @dataclass(frozen=True)
 class EntityAnnotationResults:
     original_text: str
     annotated_text: str
     entities: List[Entity]
```

### Comparing `extr-0.0.6/src/extr/regex.py` & `extr-0.0.7/src/extr/regex.py`

 * *Files identical despite different names*

### Comparing `extr-0.0.6/src/extr/relations.py` & `extr-0.0.7/src/extr/relations.py`

 * *Files identical despite different names*

### Comparing `extr-0.0.6/src/extr.egg-info/PKG-INFO` & `extr-0.0.7/src/extr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extr
-Version: 0.0.6
+Version: 0.0.7
 Summary: Named Entity Recognition (NER) and Relation Extraction (RE) library using Regular Expressions
 Home-page: https://github.com/dpasse/extr
 License: UNKNOWN
 Description: # Extr
         > Named Entity Recognition (NER) and Relation Extraction (RE) library using Regular Expressions
         
         <br />
```

