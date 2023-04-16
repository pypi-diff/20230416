# Comparing `tmp/pygedcom-0.2.0.tar.gz` & `tmp/pygedcom-0.2.1.tar.gz`

## Comparing `pygedcom-0.2.0.tar` & `pygedcom-0.2.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.2.0/__init__.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 pygedcom-0.2.0/main.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 pygedcom-0.2.0/requirements.txt
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 pygedcom-0.2.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 pygedcom-0.2.0/.github/workflows/test_and_doc.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pygedcom-0.2.0/docs/Makefile
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 pygedcom-0.2.0/docs/conf.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 pygedcom-0.2.0/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 pygedcom-0.2.0/docs/make.bat
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 pygedcom-0.2.0/docs/sources/export.rst
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 pygedcom-0.2.0/docs/sources/gedcomElement.rst
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 pygedcom-0.2.0/docs/sources/gedcomParser.rst
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 pygedcom-0.2.0/docs/sources/gedcomRootElement.rst
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 pygedcom-0.2.0/docs/sources/gedcomSubElement.rst
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 pygedcom-0.2.0/docs/sources/getting_started.rst
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 pygedcom-0.2.0/docs/sources/parsing.rst
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pygedcom-0.2.0/src/pygedcom/__init__.py
--rw-r--r--   0        0        0    21792 2020-02-02 00:00:00.000000 pygedcom-0.2.0/src/pygedcom/gedcom_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.2.0/src/pygedcom/elements/__init__.py
--rw-r--r--   0        0        0     6562 2020-02-02 00:00:00.000000 pygedcom-0.2.0/src/pygedcom/elements/element.py
--rw-r--r--   0        0        0    70880 2020-02-02 00:00:00.000000 pygedcom-0.2.0/src/pygedcom/elements/mapping.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.2.0/src/pygedcom/elements/rootElements/__init__.py
--rw-r--r--   0        0        0     7258 2020-02-02 00:00:00.000000 pygedcom-0.2.0/src/pygedcom/elements/rootElements/family.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 pygedcom-0.2.0/src/pygedcom/elements/rootElements/head.py
--rw-r--r--   0        0        0     6983 2020-02-02 00:00:00.000000 pygedcom-0.2.0/src/pygedcom/elements/rootElements/individual.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 pygedcom-0.2.0/src/pygedcom/elements/rootElements/note.py
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 pygedcom-0.2.0/src/pygedcom/elements/rootElements/object.py
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 pygedcom-0.2.0/src/pygedcom/elements/rootElements/repository.py
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 pygedcom-0.2.0/src/pygedcom/elements/rootElements/rootElement.py
--rw-r--r--   0        0        0     4858 2020-02-02 00:00:00.000000 pygedcom-0.2.0/src/pygedcom/elements/rootElements/source.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 pygedcom-0.2.0/src/pygedcom/elements/rootElements/submitter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.2.0/src/pygedcom/elements/subElements/__init__.py
--rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 pygedcom-0.2.0/src/pygedcom/elements/subElements/commonEvent.py
--rw-r--r--   0        0        0     6574 2020-02-02 00:00:00.000000 pygedcom-0.2.0/src/pygedcom/elements/subElements/date.py
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 pygedcom-0.2.0/src/pygedcom/elements/subElements/map.py
--rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 pygedcom-0.2.0/src/pygedcom/elements/subElements/place.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.2.0/test/__init__.py
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 pygedcom-0.2.0/test/test_add_elements.py
--rw-r--r--   0        0        0     5429 2020-02-02 00:00:00.000000 pygedcom-0.2.0/test/test_export.py
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 pygedcom-0.2.0/test/test_parse.py
--rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 pygedcom-0.2.0/test/test_remove_element.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 pygedcom-0.2.0/test/test_set_prop.py
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 pygedcom-0.2.0/test/test_verify.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pygedcom-0.2.0/test/samples/00_simple_individual_record.ged
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 pygedcom-0.2.0/test/samples/01_simple_family_record.ged
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 pygedcom-0.2.0/test/samples/02_simple_source_record.ged
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 pygedcom-0.2.0/test/samples/03_simple_repository_record.ged
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pygedcom-0.2.0/test/samples/04_simple_date_formats.ged
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pygedcom-0.2.0/test/samples/05_all_date_modifiers.ged
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pygedcom-0.2.0/test/samples/10_invalid_level.ged
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 pygedcom-0.2.0/test/samples/20_complex_sample.ged
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 pygedcom-0.2.0/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 pygedcom-0.2.0/LICENSE
--rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 pygedcom-0.2.0/README.md
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 pygedcom-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3683 2020-02-02 00:00:00.000000 pygedcom-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.2.1/__init__.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 pygedcom-0.2.1/main.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 pygedcom-0.2.1/requirements.txt
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 pygedcom-0.2.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 pygedcom-0.2.1/.github/workflows/test_and_doc.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pygedcom-0.2.1/docs/Makefile
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 pygedcom-0.2.1/docs/conf.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 pygedcom-0.2.1/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 pygedcom-0.2.1/docs/make.bat
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 pygedcom-0.2.1/docs/sources/export.rst
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 pygedcom-0.2.1/docs/sources/gedcomElement.rst
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 pygedcom-0.2.1/docs/sources/gedcomParser.rst
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 pygedcom-0.2.1/docs/sources/gedcomRootElement.rst
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 pygedcom-0.2.1/docs/sources/gedcomSubElement.rst
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 pygedcom-0.2.1/docs/sources/getting_started.rst
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 pygedcom-0.2.1/docs/sources/parsing.rst
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pygedcom-0.2.1/src/pygedcom/__init__.py
+-rw-r--r--   0        0        0    21792 2020-02-02 00:00:00.000000 pygedcom-0.2.1/src/pygedcom/gedcom_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.2.1/src/pygedcom/elements/__init__.py
+-rw-r--r--   0        0        0     6562 2020-02-02 00:00:00.000000 pygedcom-0.2.1/src/pygedcom/elements/element.py
+-rw-r--r--   0        0        0    70880 2020-02-02 00:00:00.000000 pygedcom-0.2.1/src/pygedcom/elements/mapping.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.2.1/src/pygedcom/elements/rootElements/__init__.py
+-rw-r--r--   0        0        0     7279 2020-02-02 00:00:00.000000 pygedcom-0.2.1/src/pygedcom/elements/rootElements/family.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 pygedcom-0.2.1/src/pygedcom/elements/rootElements/head.py
+-rw-r--r--   0        0        0     6983 2020-02-02 00:00:00.000000 pygedcom-0.2.1/src/pygedcom/elements/rootElements/individual.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 pygedcom-0.2.1/src/pygedcom/elements/rootElements/note.py
+-rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 pygedcom-0.2.1/src/pygedcom/elements/rootElements/object.py
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 pygedcom-0.2.1/src/pygedcom/elements/rootElements/repository.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 pygedcom-0.2.1/src/pygedcom/elements/rootElements/rootElement.py
+-rw-r--r--   0        0        0     4858 2020-02-02 00:00:00.000000 pygedcom-0.2.1/src/pygedcom/elements/rootElements/source.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 pygedcom-0.2.1/src/pygedcom/elements/rootElements/submitter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.2.1/src/pygedcom/elements/subElements/__init__.py
+-rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 pygedcom-0.2.1/src/pygedcom/elements/subElements/commonEvent.py
+-rw-r--r--   0        0        0     6574 2020-02-02 00:00:00.000000 pygedcom-0.2.1/src/pygedcom/elements/subElements/date.py
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 pygedcom-0.2.1/src/pygedcom/elements/subElements/map.py
+-rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 pygedcom-0.2.1/src/pygedcom/elements/subElements/place.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygedcom-0.2.1/test/__init__.py
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 pygedcom-0.2.1/test/test_add_elements.py
+-rw-r--r--   0        0        0     5429 2020-02-02 00:00:00.000000 pygedcom-0.2.1/test/test_export.py
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 pygedcom-0.2.1/test/test_parse.py
+-rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 pygedcom-0.2.1/test/test_remove_element.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 pygedcom-0.2.1/test/test_set_prop.py
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 pygedcom-0.2.1/test/test_verify.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pygedcom-0.2.1/test/samples/00_simple_individual_record.ged
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 pygedcom-0.2.1/test/samples/01_simple_family_record.ged
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 pygedcom-0.2.1/test/samples/02_simple_source_record.ged
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 pygedcom-0.2.1/test/samples/03_simple_repository_record.ged
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pygedcom-0.2.1/test/samples/04_simple_date_formats.ged
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pygedcom-0.2.1/test/samples/05_all_date_modifiers.ged
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pygedcom-0.2.1/test/samples/10_invalid_level.ged
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 pygedcom-0.2.1/test/samples/20_complex_sample.ged
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 pygedcom-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 pygedcom-0.2.1/LICENSE
+-rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 pygedcom-0.2.1/README.md
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 pygedcom-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3681 2020-02-02 00:00:00.000000 pygedcom-0.2.1/PKG-INFO
```

### Comparing `pygedcom-0.2.0/requirements.txt` & `pygedcom-0.2.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `pygedcom-0.2.0/.github/workflows/python-publish.yml` & `pygedcom-0.2.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pygedcom-0.2.0/.github/workflows/test_and_doc.yml` & `pygedcom-0.2.1/.github/workflows/test_and_doc.yml`

 * *Files identical despite different names*

### Comparing `pygedcom-0.2.0/docs/Makefile` & `pygedcom-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pygedcom-0.2.0/docs/conf.py` & `pygedcom-0.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.2.0/docs/index.rst` & `pygedcom-0.2.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pygedcom-0.2.0/docs/make.bat` & `pygedcom-0.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pygedcom-0.2.0/docs/sources/export.rst` & `pygedcom-0.2.1/docs/sources/export.rst`

 * *Files identical despite different names*

### Comparing `pygedcom-0.2.0/docs/sources/gedcomRootElement.rst` & `pygedcom-0.2.1/docs/sources/gedcomRootElement.rst`

 * *Files identical despite different names*

### Comparing `pygedcom-0.2.0/docs/sources/getting_started.rst` & `pygedcom-0.2.1/docs/sources/getting_started.rst`

 * *Files identical despite different names*

### Comparing `pygedcom-0.2.0/docs/sources/parsing.rst` & `pygedcom-0.2.1/docs/sources/parsing.rst`

 * *Files identical despite different names*

### Comparing `pygedcom-0.2.0/src/pygedcom/gedcom_parser.py` & `pygedcom-0.2.1/src/pygedcom/gedcom_parser.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.2.0/src/pygedcom/elements/element.py` & `pygedcom-0.2.1/src/pygedcom/elements/element.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.2.0/src/pygedcom/elements/mapping.json` & `pygedcom-0.2.1/src/pygedcom/elements/mapping.json`

 * *Files identical despite different names*

### Comparing `pygedcom-0.2.0/src/pygedcom/elements/rootElements/family.py` & `pygedcom-0.2.1/src/pygedcom/elements/rootElements/family.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         """
         if self.find_sub_element("MARR") != []:
             marriage = self.find_sub_element("MARR")[0]
             marriage.__class__ = GedcomCommonEvent
             marriage.init_properties()
             return marriage
         else:
-            return None
+            return GedcomCommonEvent.empty()
 
     def __find_husband(self) -> str:
         """Find the husband of the family.
 
         :return: The husband of the family.
         :rtype: str
         """
```

### Comparing `pygedcom-0.2.0/src/pygedcom/elements/rootElements/head.py` & `pygedcom-0.2.1/src/pygedcom/elements/rootElements/head.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.2.0/src/pygedcom/elements/rootElements/individual.py` & `pygedcom-0.2.1/src/pygedcom/elements/rootElements/individual.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.2.0/src/pygedcom/elements/rootElements/note.py` & `pygedcom-0.2.1/src/pygedcom/elements/rootElements/note.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.2.0/src/pygedcom/elements/rootElements/object.py` & `pygedcom-0.2.1/src/pygedcom/elements/rootElements/object.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.2.0/src/pygedcom/elements/rootElements/repository.py` & `pygedcom-0.2.1/src/pygedcom/elements/rootElements/repository.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.2.0/src/pygedcom/elements/rootElements/rootElement.py` & `pygedcom-0.2.1/src/pygedcom/elements/rootElements/rootElement.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.2.0/src/pygedcom/elements/rootElements/source.py` & `pygedcom-0.2.1/src/pygedcom/elements/rootElements/source.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.2.0/src/pygedcom/elements/rootElements/submitter.py` & `pygedcom-0.2.1/src/pygedcom/elements/rootElements/submitter.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.2.0/src/pygedcom/elements/subElements/commonEvent.py` & `pygedcom-0.2.1/src/pygedcom/elements/subElements/commonEvent.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.2.0/src/pygedcom/elements/subElements/date.py` & `pygedcom-0.2.1/src/pygedcom/elements/subElements/date.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.2.0/src/pygedcom/elements/subElements/map.py` & `pygedcom-0.2.1/src/pygedcom/elements/subElements/map.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.2.0/src/pygedcom/elements/subElements/place.py` & `pygedcom-0.2.1/src/pygedcom/elements/subElements/place.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.2.0/test/test_add_elements.py` & `pygedcom-0.2.1/test/test_add_elements.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.2.0/test/test_export.py` & `pygedcom-0.2.1/test/test_export.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.2.0/test/test_parse.py` & `pygedcom-0.2.1/test/test_parse.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.2.0/test/test_remove_element.py` & `pygedcom-0.2.1/test/test_remove_element.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.2.0/test/test_set_prop.py` & `pygedcom-0.2.1/test/test_set_prop.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.2.0/test/test_verify.py` & `pygedcom-0.2.1/test/test_verify.py`

 * *Files identical despite different names*

### Comparing `pygedcom-0.2.0/test/samples/20_complex_sample.ged` & `pygedcom-0.2.1/test/samples/20_complex_sample.ged`

 * *Files identical despite different names*

### Comparing `pygedcom-0.2.0/.gitignore` & `pygedcom-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pygedcom-0.2.0/LICENSE` & `pygedcom-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pygedcom-0.2.0/README.md` & `pygedcom-0.2.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 You can check the parsing statistics to ensure that you've parsed the file correctly:
 
 
 ```python
 print(parser.get_stats())
 ```
 
-It's a good practice to verify your GEDCOM file before parsing it. You can do this with the following command:
+It's good practice to verify your GEDCOM file before parsing it. You can do this with the following command:
 
 
 ```python
 check = parser.verify()
 if check.status == 'ok':
     print("Your GEDCOM file is valid")
 else:
```

### Comparing `pygedcom-0.2.0/pyproject.toml` & `pygedcom-0.2.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pygedcom"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
     { name="Theo Petit", email="theo.p83@gmail.com" },
 ]
 description = "A gedcom utility library"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pygedcom-0.2.0/PKG-INFO` & `pygedcom-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygedcom
-Version: 0.2.0
+Version: 0.2.1
 Summary: A gedcom utility library
 Project-URL: Homepage, https://github.com/topetit/pygedcom
 Project-URL: Bug Tracker, https://github.com/topetit/pygedcom/issues
 Author-email: Theo Petit <theo.p83@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -46,15 +46,15 @@
 You can check the parsing statistics to ensure that you've parsed the file correctly:
 
 
 ```python
 print(parser.get_stats())
 ```
 
-It's a good practice to verify your GEDCOM file before parsing it. You can do this with the following command:
+It's good practice to verify your GEDCOM file before parsing it. You can do this with the following command:
 
 
 ```python
 check = parser.verify()
 if check.status == 'ok':
     print("Your GEDCOM file is valid")
 else:
```

