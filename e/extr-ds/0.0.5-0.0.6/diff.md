# Comparing `tmp/extr-ds-0.0.5.tar.gz` & `tmp/extr-ds-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extr-ds-0.0.5.tar", last modified: Sat Apr 15 13:15:49 2023, max compression
+gzip compressed data, was "extr-ds-0.0.6.tar", last modified: Sun Apr 16 19:36:44 2023, max compression
```

## Comparing `extr-ds-0.0.5.tar` & `extr-ds-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 13:15:48.968478 extr-ds-0.0.5/
--rw-rw-rw-   0        0        0     2645 2023-04-15 13:15:48.963504 extr-ds-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1786 2023-04-14 20:27:48.000000 extr-ds-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-04-15 13:15:48.978852 extr-ds-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      607 2023-04-15 13:15:11.000000 extr-ds-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-15 13:15:48.558726 extr-ds-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-04-15 13:15:48.848479 extr-ds-0.0.5/src/extr_ds/
--rw-rw-rw-   0        0        0       27 2023-04-15 12:51:37.000000 extr-ds-0.0.5/src/extr_ds/__init__.py
--rw-rw-rw-   0        0        0     1602 2023-04-15 13:14:58.000000 extr-ds-0.0.5/src/extr_ds/labelers.py
--rw-rw-rw-   0        0        0      938 2023-04-15 12:50:19.000000 extr-ds-0.0.5/src/extr_ds/models.py
--rw-rw-rw-   0        0        0      939 2023-04-13 12:37:43.000000 extr-ds-0.0.5/src/extr_ds/tokenizer.py
--rw-rw-rw-   0        0        0     1561 2023-04-15 12:51:08.000000 extr-ds-0.0.5/src/extr_ds/validators.py
-drwxrwxrwx   0        0        0        0 2023-04-15 13:15:48.954479 extr-ds-0.0.5/src/extr_ds.egg-info/
--rw-rw-rw-   0        0        0     2645 2023-04-15 13:15:47.000000 extr-ds-0.0.5/src/extr_ds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      313 2023-04-15 13:15:47.000000 extr-ds-0.0.5/src/extr_ds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 13:15:47.000000 extr-ds-0.0.5/src/extr_ds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-15 13:15:47.000000 extr-ds-0.0.5/src/extr_ds.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-15 13:15:47.000000 extr-ds-0.0.5/src/extr_ds.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 19:36:44.257335 extr-ds-0.0.6/
+-rw-rw-rw-   0        0        0     3883 2023-04-16 19:36:44.250979 extr-ds-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2728 2023-04-16 19:30:04.000000 extr-ds-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-16 19:36:44.263367 extr-ds-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      607 2023-04-16 19:36:23.000000 extr-ds-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 19:36:44.056114 extr-ds-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-04-16 19:36:44.103126 extr-ds-0.0.6/src/extr_ds/
+-rw-rw-rw-   0        0        0       27 2023-04-15 12:51:37.000000 extr-ds-0.0.6/src/extr_ds/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 19:36:44.246066 extr-ds-0.0.6/src/extr_ds/labelers/
+-rw-rw-rw-   0        0        0       68 2023-04-16 10:14:54.000000 extr-ds-0.0.6/src/extr_ds/labelers/__init__.py
+-rw-rw-rw-   0        0        0     1604 2023-04-16 09:37:06.000000 extr-ds-0.0.6/src/extr_ds/labelers/iob.py
+-rw-rw-rw-   0        0        0     3879 2023-04-16 19:35:58.000000 extr-ds-0.0.6/src/extr_ds/labelers/relation.py
+-rw-rw-rw-   0        0        0     1145 2023-04-16 10:21:54.000000 extr-ds-0.0.6/src/extr_ds/models.py
+-rw-rw-rw-   0        0        0     1059 2023-04-16 18:37:33.000000 extr-ds-0.0.6/src/extr_ds/tokenizer.py
+-rw-rw-rw-   0        0        0     1561 2023-04-15 12:51:08.000000 extr-ds-0.0.6/src/extr_ds/validators.py
+drwxrwxrwx   0        0        0        0 2023-04-16 19:36:44.225006 extr-ds-0.0.6/src/extr_ds.egg-info/
+-rw-rw-rw-   0        0        0     3883 2023-04-16 19:36:43.000000 extr-ds-0.0.6/src/extr_ds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2023-04-16 19:36:43.000000 extr-ds-0.0.6/src/extr_ds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 19:36:43.000000 extr-ds-0.0.6/src/extr_ds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-16 19:36:43.000000 extr-ds-0.0.6/src/extr_ds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-16 19:36:43.000000 extr-ds-0.0.6/src/extr_ds.egg-info/top_level.txt
```

### Comparing `extr-ds-0.0.5/PKG-INFO` & `extr-ds-0.0.6/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,75 +1,103 @@
-Metadata-Version: 2.1
-Name: extr-ds
-Version: 0.0.5
-Summary: Library to quickly build basic datasets for Named Entity Recognition (NER) and Relation Extraction (RE) Machine Learning tasks.
-Home-page: https://github.com/dpasse/extr-ds
-License: UNKNOWN
-Description: # extr-ds
-        > Library to quickly build basic datasets for Named Entity Recognition (NER) and Relation Extraction (RE) Machine Learning tasks.
-        
-        <br />
-        
-        ## Install
-        
-        ```
-        pip install extr-ds
-        ```
-        
-        ## Example
-        
-        ```python
-        text = 'Ted Johnson is a pitcher. Ted went to my school.'
-        ```
-        
-        ### 1. Label Entities for Named-Entity Recognition Task (NER)
-        
-        ```python
-        from extr import RegEx, RegExLabel, EntityExtactor
-        from extr_ds import IOB
-        
-        entity_extractor = EntityExtactor([
-            RegExLabel('PERSON', [
-                RegEx([r'(ted\s+johnson|ted)'], re.IGNORECASE)
-            ]),
-            RegExLabel('POSITION', [
-                RegEx([r'pitcher'], re.IGNORECASE)
-            ]),
-        ])
-        
-        sentence_tokenizer = ## 3rd party tokenizer ##
-        labels = IOB(sentence_tokenizer, entity_extractor).label(text)
-        
-        ## labels ==  [
-        ##     <Label tokens=..., labels=['B-PERSON', 'I-PERSON', 'O', 'O', 'B-POSITION', 'O']>,
-        ##     <Label tokens=..., labels=['B-PERSON', 'O', 'O', 'O', 'O', 'O']>
-        ## ]
-        ```
-        
-        ### 2. Find and define the type of difference between labels
-        
-        ```python
-        from extr_ds.validators import check_for_differences
-        
-        differences_in_labels = check_for_differences(
-            ['B-PERSON', 'I-PERSON', 'O', 'O', 'B-POSITION', 'O'],
-            ['B-PERSON', 'O', 'O', 'O', 'B-POSITION', 'O']
-        )
-        
-        ## differences_in_labels.has_diffs == True
-        ## differences_in_labels.diffs_between_labels == [
-        ##      <Difference index=1, diff_type=DifferenceTypes.S2_MISSING>
-        ## ]
-        
-        differences_in_labels = check_for_differences(
-            ['B-PERSON', 'I-PERSON', 'O', 'O', 'B-POSITION', 'O'],
-            ['B-PERSON', 'B-PERSON', 'O', 'O', 'B-POSITION', 'O']
-        )
-        
-        ## differences_in_labels.has_diffs == True
-        ## differences_in_labels.diffs_between_labels == [
-        ##      <Difference index=1, diff_type=DifferenceTypes.MISMATCH>
-        ## ]
-        ```
-        
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
+# extr-ds
+> Library to quickly build basic datasets for Named Entity Recognition (NER) and Relation Extraction (RE) Machine Learning tasks.
+
+<br />
+
+## Install
+
+```
+pip install extr-ds
+```
+
+## Example
+
+```python
+text = 'Ted Johnson is a pitcher. Ted went to my school.'
+```
+
+### 1. Label Entities for Named-Entity Recognition Task (NER)
+
+```python
+from extr import RegEx, RegExLabel, EntityExtactor
+from extr_ds import IOB
+
+entity_extractor = EntityExtactor([
+    RegExLabel('PERSON', [
+        RegEx([r'(ted\s+johnson|ted)'], re.IGNORECASE)
+    ]),
+    RegExLabel('POSITION', [
+        RegEx([r'pitcher'], re.IGNORECASE)
+    ]),
+])
+
+sentence_tokenizer = ## 3rd party tokenizer ##
+labels = IOB(sentence_tokenizer, entity_extractor).label(text)
+
+## labels ==  [
+##     <Label tokens=..., labels=['B-PERSON', 'I-PERSON', 'O', 'O', 'B-POSITION', 'O']>,
+##     <Label tokens=..., labels=['B-PERSON', 'O', 'O', 'O', 'O', 'O']>
+## ]
+```
+
+### 2. Annotate for Relation Extraction Task (RE)
+
+```python
+from extr import RegExRelationLabelBuilder, RelationExtractor
+from extr_ds.labelers import RelationClassification
+
+person_to_position_relationship = RegExRelationLabelBuilder('is_a') \
+    .add_e1_to_e2(
+        'PERSON',
+        [
+            r'\s+is\s+a\s+',
+        ],
+        'POSITION'
+    ) \
+    .build()
+
+labeler = RelationClassification(
+    sentence_tokenizer,
+    EntityExtractor([
+        RegExLabel('PERSON', [
+            RegEx([r'(ted johnson|bob)'], re.IGNORECASE)
+        ]),
+        RegExLabel('POSITION', [
+            RegEx([r'pitcher'], re.IGNORECASE)
+        ]),
+    ]),
+    RelationExtractor([person_to_position_relationship]),
+    [('PERSON', 'POSITION', 'NO_RELATION')],
+)
+
+labels = labeler.label(text)
+
+## labels == [
+##    <RelationLabel sentence="<e1>Ted Johnson</e1> is a <e2>pitcher</e2>." label="is_a">
+## ]
+```
+
+### 3. Find and define the type of difference between labels
+
+```python
+from extr_ds.validators import check_for_differences
+
+differences_in_labels = check_for_differences(
+    ['B-PERSON', 'I-PERSON', 'O', 'O', 'B-POSITION', 'O'],
+    ['B-PERSON', 'O', 'O', 'O', 'B-POSITION', 'O']
+)
+
+## differences_in_labels.has_diffs == True
+## differences_in_labels.diffs_between_labels == [
+##      <Difference index=1, diff_type=DifferenceTypes.S2_MISSING>
+## ]
+
+differences_in_labels = check_for_differences(
+    ['B-PERSON', 'I-PERSON', 'O', 'O', 'B-POSITION', 'O'],
+    ['B-PERSON', 'B-PERSON', 'O', 'O', 'B-POSITION', 'O']
+)
+
+## differences_in_labels.has_diffs == True
+## differences_in_labels.diffs_between_labels == [
+##      <Difference index=1, diff_type=DifferenceTypes.MISMATCH>
+## ]
+```
```

### Comparing `extr-ds-0.0.5/setup.py` & `extr-ds-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name='extr-ds',
-    version='0.0.5',
+    version='0.0.6',
     keywords='',
     description='Library to quickly build basic datasets for Named Entity Recognition (NER) and Relation Extraction (RE) Machine Learning tasks.',
     packages=setuptools.find_packages('src'),
     package_dir={'': 'src'},
     install_requires=[
-        'extr==0.0.6'
+        'extr==0.0.7'
     ],
     url='https://github.com/dpasse/extr-ds',
     long_description=long_description,
     long_description_content_type='text/markdown',
 )
```

### Comparing `extr-ds-0.0.5/src/extr_ds/labelers.py` & `extr-ds-0.0.6/src/extr_ds/labelers/iob.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import List, Callable, Generator, Iterator, cast
 from extr import Entity, EntityExtractor
-from .models import TokenGroup, Label
-from .tokenizer import tokenizer
+from ..models import TokenGroup, Label
+from ..tokenizer import tokenizer
 
 
 class IOB():
     def __init__(self, sentence_tokenizer: Callable[[str], List[List[str]]], entity_extractor: EntityExtractor) -> None:
         self._sentence_tokenizer = sentence_tokenizer
         self._entity_extractor = entity_extractor
```

### Comparing `extr-ds-0.0.5/src/extr_ds/models.py` & `extr-ds-0.0.6/src/extr_ds/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,16 +22,25 @@
 
     def __repr__(self) -> str:
         return f'<Token text="{self.text}", location={repr(self.location)}, order={self.order}>'
 
 @dataclass(frozen=True)
 class TokenGroup(ILocation):
     location: Location
+    sentence: str
     tokens: List[Token]
 
 @dataclass
 class Label:
     tokens: List[Token]
     labels: List[str]
 
     def __repr__(self) -> str:
         return f'<Label tokens={self.tokens}, labels={self.labels}>'
+
+@dataclass
+class RelationLabel:
+    sentence: str
+    label: str
+
+    def __repr__(self) -> str:
+        return f'<RelationLabel sentence="{self.sentence}" label="{self.label}">'
```

### Comparing `extr-ds-0.0.5/src/extr_ds/tokenizer.py` & `extr-ds-0.0.6/src/extr_ds/tokenizer.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,8 +21,14 @@
                 Token(term, Location(offset + start, offset + end), counter)
             )
 
             cache = cache[end:]
             offset += end
             counter += 1
 
-        yield TokenGroup(Location(sentence_start, offset), tokens_in_sentence)
+        sentence_text = text[sentence_start:offset]
+
+        yield TokenGroup(
+            Location(sentence_start, offset),
+            sentence_text,
+            tokens_in_sentence
+        )
```

### Comparing `extr-ds-0.0.5/src/extr_ds/validators.py` & `extr-ds-0.0.6/src/extr_ds/validators.py`

 * *Files identical despite different names*

### Comparing `extr-ds-0.0.5/src/extr_ds.egg-info/PKG-INFO` & `extr-ds-0.0.6/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extr-ds
-Version: 0.0.5
+Version: 0.0.6
 Summary: Library to quickly build basic datasets for Named Entity Recognition (NER) and Relation Extraction (RE) Machine Learning tasks.
 Home-page: https://github.com/dpasse/extr-ds
 License: UNKNOWN
 Description: # extr-ds
         > Library to quickly build basic datasets for Named Entity Recognition (NER) and Relation Extraction (RE) Machine Learning tasks.
         
         <br />
@@ -41,15 +41,52 @@
         
         ## labels ==  [
         ##     <Label tokens=..., labels=['B-PERSON', 'I-PERSON', 'O', 'O', 'B-POSITION', 'O']>,
         ##     <Label tokens=..., labels=['B-PERSON', 'O', 'O', 'O', 'O', 'O']>
         ## ]
         ```
         
-        ### 2. Find and define the type of difference between labels
+        ### 2. Annotate for Relation Extraction Task (RE)
+        
+        ```python
+        from extr import RegExRelationLabelBuilder, RelationExtractor
+        from extr_ds.labelers import RelationClassification
+        
+        person_to_position_relationship = RegExRelationLabelBuilder('is_a') \
+            .add_e1_to_e2(
+                'PERSON',
+                [
+                    r'\s+is\s+a\s+',
+                ],
+                'POSITION'
+            ) \
+            .build()
+        
+        labeler = RelationClassification(
+            sentence_tokenizer,
+            EntityExtractor([
+                RegExLabel('PERSON', [
+                    RegEx([r'(ted johnson|bob)'], re.IGNORECASE)
+                ]),
+                RegExLabel('POSITION', [
+                    RegEx([r'pitcher'], re.IGNORECASE)
+                ]),
+            ]),
+            RelationExtractor([person_to_position_relationship]),
+            [('PERSON', 'POSITION', 'NO_RELATION')],
+        )
+        
+        labels = labeler.label(text)
+        
+        ## labels == [
+        ##    <RelationLabel sentence="<e1>Ted Johnson</e1> is a <e2>pitcher</e2>." label="is_a">
+        ## ]
+        ```
+        
+        ### 3. Find and define the type of difference between labels
         
         ```python
         from extr_ds.validators import check_for_differences
         
         differences_in_labels = check_for_differences(
             ['B-PERSON', 'I-PERSON', 'O', 'O', 'B-POSITION', 'O'],
             ['B-PERSON', 'O', 'O', 'O', 'B-POSITION', 'O']
```

