# Comparing `tmp/rasa-model-report-1.3.3.tar.gz` & `tmp/rasa-model-report-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rasa-model-report-1.3.3.tar", last modified: Thu Apr  6 16:03:09 2023, max compression
+gzip compressed data, was "rasa-model-report-1.3.4.tar", last modified: Sun Apr 16 21:48:00 2023, max compression
```

## Comparing `rasa-model-report-1.3.3.tar` & `rasa-model-report-1.3.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 bruno.justo  (1001) bruno.justo  (1001)        0 2023-04-06 16:03:09.029863 rasa-model-report-1.3.3/
--rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)    11357 2022-11-12 01:01:09.000000 rasa-model-report-1.3.3/LICENSE
--rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)     8523 2023-04-06 16:03:09.029863 rasa-model-report-1.3.3/PKG-INFO
--rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)     8129 2023-03-24 23:06:15.000000 rasa-model-report-1.3.3/README.md
-drwxrwxr-x   0 bruno.justo  (1001) bruno.justo  (1001)        0 2023-04-06 16:03:09.009863 rasa-model-report-1.3.3/rasa_model_report/
--rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)        0 2022-12-31 15:38:47.000000 rasa-model-report-1.3.3/rasa_model_report/__init__.py
-drwxrwxr-x   0 bruno.justo  (1001) bruno.justo  (1001)        0 2023-04-06 16:03:09.021864 rasa-model-report-1.3.3/rasa_model_report/controllers/
--rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)        0 2022-12-31 15:38:47.000000 rasa-model-report-1.3.3/rasa_model_report/controllers/__init__.py
--rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)     1157 2023-04-06 15:47:57.000000 rasa-model-report-1.3.3/rasa_model_report/controllers/controller.py
--rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)     1380 2022-12-31 15:38:47.000000 rasa-model-report-1.3.3/rasa_model_report/controllers/csv_controller.py
--rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)     7804 2023-02-27 00:24:02.000000 rasa-model-report-1.3.3/rasa_model_report/controllers/e2e_coverage_controller.py
--rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)    12196 2023-03-24 23:06:15.000000 rasa-model-report-1.3.3/rasa_model_report/controllers/json_controller.py
--rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)    23220 2023-04-06 15:47:57.000000 rasa-model-report-1.3.3/rasa_model_report/controllers/markdown_controller.py
--rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)     4616 2023-04-06 15:47:57.000000 rasa-model-report-1.3.3/rasa_model_report/controllers/model_report.py
--rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)     9116 2023-04-06 16:01:46.000000 rasa-model-report-1.3.3/rasa_model_report/controllers/nlu_controller.py
-drwxrwxr-x   0 bruno.justo  (1001) bruno.justo  (1001)        0 2023-04-06 16:03:09.025864 rasa-model-report-1.3.3/rasa_model_report/helpers/
--rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)        0 2022-12-31 15:38:47.000000 rasa-model-report-1.3.3/rasa_model_report/helpers/__init__.py
--rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)      204 2023-04-06 15:47:57.000000 rasa-model-report-1.3.3/rasa_model_report/helpers/constants.py
--rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)      247 2023-03-24 23:06:15.000000 rasa-model-report-1.3.3/rasa_model_report/helpers/type_aliases.py
--rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)     5885 2023-03-24 23:06:15.000000 rasa-model-report-1.3.3/rasa_model_report/helpers/utils.py
--rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)     3241 2023-04-06 15:47:57.000000 rasa-model-report-1.3.3/rasa_model_report/main.py
-drwxrwxr-x   0 bruno.justo  (1001) bruno.justo  (1001)        0 2023-04-06 16:03:09.013863 rasa-model-report-1.3.3/rasa_model_report.egg-info/
--rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)     8523 2023-04-06 16:03:08.000000 rasa-model-report-1.3.3/rasa_model_report.egg-info/PKG-INFO
--rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)     1132 2023-04-06 16:03:08.000000 rasa-model-report-1.3.3/rasa_model_report.egg-info/SOURCES.txt
--rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)        1 2023-04-06 16:03:08.000000 rasa-model-report-1.3.3/rasa_model_report.egg-info/dependency_links.txt
--rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)       66 2023-04-06 16:03:08.000000 rasa-model-report-1.3.3/rasa_model_report.egg-info/entry_points.txt
--rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)       35 2023-04-06 16:03:08.000000 rasa-model-report-1.3.3/rasa_model_report.egg-info/requires.txt
--rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)       18 2023-04-06 16:03:08.000000 rasa-model-report-1.3.3/rasa_model_report.egg-info/top_level.txt
--rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)      518 2023-04-06 16:03:09.029863 rasa-model-report-1.3.3/setup.cfg
--rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)      983 2023-04-06 16:02:52.000000 rasa-model-report-1.3.3/setup.py
-drwxrwxr-x   0 bruno.justo  (1001) bruno.justo  (1001)        0 2023-04-06 16:03:09.029863 rasa-model-report-1.3.3/tests/
--rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)      467 2023-02-26 23:52:26.000000 rasa-model-report-1.3.3/tests/test_controller.py
--rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)     1611 2022-12-31 15:38:47.000000 rasa-model-report-1.3.3/tests/test_csv_controller.py
--rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)     5900 2023-02-27 00:24:02.000000 rasa-model-report-1.3.3/tests/test_e2e_coverage_controller.py
--rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)     9082 2023-03-24 23:06:15.000000 rasa-model-report-1.3.3/tests/test_json_controller.py
--rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)     1294 2023-04-06 15:47:57.000000 rasa-model-report-1.3.3/tests/test_main.py
--rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)    13462 2023-04-06 15:47:57.000000 rasa-model-report-1.3.3/tests/test_markdown_controller.py
--rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)     2383 2023-04-06 15:47:57.000000 rasa-model-report-1.3.3/tests/test_model_report.py
--rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)     8143 2022-12-31 15:38:47.000000 rasa-model-report-1.3.3/tests/test_nlu_controller.py
--rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)     7652 2023-03-24 23:06:15.000000 rasa-model-report-1.3.3/tests/test_utils.py
+drwxrwxr-x   0 bruno.justo  (1001) bruno.justo  (1001)        0 2023-04-16 21:48:00.811050 rasa-model-report-1.3.4/
+-rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)    11357 2022-11-12 01:01:09.000000 rasa-model-report-1.3.4/LICENSE
+-rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)     8523 2023-04-16 21:48:00.811050 rasa-model-report-1.3.4/PKG-INFO
+-rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)     8129 2023-03-24 23:06:15.000000 rasa-model-report-1.3.4/README.md
+drwxrwxr-x   0 bruno.justo  (1001) bruno.justo  (1001)        0 2023-04-16 21:48:00.787050 rasa-model-report-1.3.4/rasa_model_report/
+-rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)        0 2023-04-14 19:07:12.000000 rasa-model-report-1.3.4/rasa_model_report/__init__.py
+drwxrwxr-x   0 bruno.justo  (1001) bruno.justo  (1001)        0 2023-04-16 21:48:00.799050 rasa-model-report-1.3.4/rasa_model_report/controllers/
+-rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)        0 2022-12-31 15:38:47.000000 rasa-model-report-1.3.4/rasa_model_report/controllers/__init__.py
+-rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)     1157 2023-04-14 19:07:12.000000 rasa-model-report-1.3.4/rasa_model_report/controllers/controller.py
+-rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)     1380 2022-12-31 15:38:47.000000 rasa-model-report-1.3.4/rasa_model_report/controllers/csv_controller.py
+-rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)     7754 2023-04-16 21:37:55.000000 rasa-model-report-1.3.4/rasa_model_report/controllers/e2e_coverage_controller.py
+-rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)    12196 2023-04-14 19:17:55.000000 rasa-model-report-1.3.4/rasa_model_report/controllers/json_controller.py
+-rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)    23241 2023-04-16 21:37:55.000000 rasa-model-report-1.3.4/rasa_model_report/controllers/markdown_controller.py
+-rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)     4616 2023-04-16 19:54:33.000000 rasa-model-report-1.3.4/rasa_model_report/controllers/model_report.py
+-rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)     9122 2023-04-16 21:37:55.000000 rasa-model-report-1.3.4/rasa_model_report/controllers/nlu_controller.py
+drwxrwxr-x   0 bruno.justo  (1001) bruno.justo  (1001)        0 2023-04-16 21:48:00.803050 rasa-model-report-1.3.4/rasa_model_report/helpers/
+-rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)        0 2022-12-31 15:38:47.000000 rasa-model-report-1.3.4/rasa_model_report/helpers/__init__.py
+-rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)      204 2023-04-14 19:07:12.000000 rasa-model-report-1.3.4/rasa_model_report/helpers/constants.py
+-rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)      247 2023-03-24 23:06:15.000000 rasa-model-report-1.3.4/rasa_model_report/helpers/type_aliases.py
+-rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)     5940 2023-04-16 21:37:55.000000 rasa-model-report-1.3.4/rasa_model_report/helpers/utils.py
+-rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)     3241 2023-04-14 19:07:12.000000 rasa-model-report-1.3.4/rasa_model_report/main.py
+drwxrwxr-x   0 bruno.justo  (1001) bruno.justo  (1001)        0 2023-04-16 21:48:00.791050 rasa-model-report-1.3.4/rasa_model_report.egg-info/
+-rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)     8523 2023-04-16 21:48:00.000000 rasa-model-report-1.3.4/rasa_model_report.egg-info/PKG-INFO
+-rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)     1132 2023-04-16 21:48:00.000000 rasa-model-report-1.3.4/rasa_model_report.egg-info/SOURCES.txt
+-rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)        1 2023-04-16 21:48:00.000000 rasa-model-report-1.3.4/rasa_model_report.egg-info/dependency_links.txt
+-rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)       66 2023-04-16 21:48:00.000000 rasa-model-report-1.3.4/rasa_model_report.egg-info/entry_points.txt
+-rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)       35 2023-04-16 21:48:00.000000 rasa-model-report-1.3.4/rasa_model_report.egg-info/requires.txt
+-rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)       18 2023-04-16 21:48:00.000000 rasa-model-report-1.3.4/rasa_model_report.egg-info/top_level.txt
+-rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)      518 2023-04-16 21:48:00.811050 rasa-model-report-1.3.4/setup.cfg
+-rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)      983 2023-04-16 21:47:44.000000 rasa-model-report-1.3.4/setup.py
+drwxrwxr-x   0 bruno.justo  (1001) bruno.justo  (1001)        0 2023-04-16 21:48:00.811050 rasa-model-report-1.3.4/tests/
+-rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)      467 2023-02-26 23:52:26.000000 rasa-model-report-1.3.4/tests/test_controller.py
+-rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)     1611 2022-12-31 15:38:47.000000 rasa-model-report-1.3.4/tests/test_csv_controller.py
+-rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)     6286 2023-04-16 21:37:55.000000 rasa-model-report-1.3.4/tests/test_e2e_coverage_controller.py
+-rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)     9082 2023-03-24 23:06:15.000000 rasa-model-report-1.3.4/tests/test_json_controller.py
+-rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)     1294 2023-04-16 19:58:51.000000 rasa-model-report-1.3.4/tests/test_main.py
+-rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)    13462 2023-04-14 19:07:12.000000 rasa-model-report-1.3.4/tests/test_markdown_controller.py
+-rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)     2383 2023-04-14 19:07:12.000000 rasa-model-report-1.3.4/tests/test_model_report.py
+-rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)     8143 2022-12-31 15:38:47.000000 rasa-model-report-1.3.4/tests/test_nlu_controller.py
+-rw-rw-r--   0 bruno.justo  (1001) bruno.justo  (1001)     7652 2023-04-16 18:39:22.000000 rasa-model-report-1.3.4/tests/test_utils.py
```

### Comparing `rasa-model-report-1.3.3/LICENSE` & `rasa-model-report-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rasa-model-report-1.3.3/PKG-INFO` & `rasa-model-report-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rasa-model-report
-Version: 1.3.3
+Version: 1.3.4
 Summary: Simple open-source Rasa command-line add-on that generates training model health reports for your projects.
 Home-page: https://github.com/brunohjs/rasa-model-report
 Author: Bruno Justo
 Author-email: brunohjs@gmail.com
 License: Apache 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `rasa-model-report-1.3.3/README.md` & `rasa-model-report-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `rasa-model-report-1.3.3/rasa_model_report/controllers/controller.py` & `rasa-model-report-1.3.4/rasa_model_report/controllers/controller.py`

 * *Files identical despite different names*

### Comparing `rasa-model-report-1.3.3/rasa_model_report/controllers/csv_controller.py` & `rasa-model-report-1.3.4/rasa_model_report/controllers/csv_controller.py`

 * *Files identical despite different names*

### Comparing `rasa-model-report-1.3.3/rasa_model_report/controllers/e2e_coverage_controller.py` & `rasa-model-report-1.3.4/rasa_model_report/controllers/e2e_coverage_controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,16 +75,16 @@
         self._actions = utils.list_diff(self._actions, self.get_utters_in_actions())
 
     def _generate(self) -> None:
         """
         Generate E2E tests coverage report string.
         """
         not_covered = {}
-        report_data = [self.json.extract_entity_from_string(item["name"]) for item in self.json.core]
-        for element in ["intents", "entities", "actions"]:
+        report_data = [item["name"] for item in self.json.core]
+        for element in ["intents", "actions"]:
             element_list = getattr(self, f"_{element}")
             not_covered[element] = {
                 "items": utils.list_diff(element_list, report_data)
             }
             not_covered[element]["rate"] = 0
             if element_list:
                 not_covered[element]["rate"] = 1 - len(not_covered[element]["items"]) / len(element_list)
```

### Comparing `rasa-model-report-1.3.3/rasa_model_report/controllers/json_controller.py` & `rasa-model-report-1.3.4/rasa_model_report/controllers/json_controller.py`

 * *Files identical despite different names*

### Comparing `rasa-model-report-1.3.3/rasa_model_report/controllers/markdown_controller.py` & `rasa-model-report-1.3.4/rasa_model_report/controllers/markdown_controller.py`

 * *Files 5% similar despite different names*

```diff
@@ -122,26 +122,27 @@
 
     def build_summary(self) -> str:
         """
         Build the report model summary.
 
         :return: Report model summary.
         """
-        text = "## Index\n"
-        text += " - [Overview](#overview)\n"
+        sections = [
+            " - [Overview](#overview)\n",
+            " - [Intents](#intents)\n",
+            " - [Entities](#entities)\n",
+            " - [Core](#core)\n",
+            " - [E2E Coverage](#e2e)\n"
+        ]
         if os.path.isfile(self.config_report_path):
-            text += " - [Config](#configs)\n"
-        text += " - [Intents](#intents)\n"
-        text += " - [Entities](#entities)\n"
+            sections.insert(1, " - [Config](#configs)\n")
         if self.nlu.is_connected():
-            text += " - [NLU](#nlu)\n"
-        text += " - [Core](#core)\n"
-        text += " - [E2E Coverage](#e2e)\n"
-        text += "\n"
-        return text
+            sections.insert(3, " - [NLU](#nlu)\n")
+
+        return f"## Index\n{''.join(sections)}\n"
 
     def build_table(self, data: List[Union[str, float]]) -> str:
         """
         Build a table in markdown format.
 
         :param data: List representing the table data.
         :return: Table in markdown format.
```

### Comparing `rasa-model-report-1.3.3/rasa_model_report/controllers/model_report.py` & `rasa-model-report-1.3.4/rasa_model_report/controllers/model_report.py`

 * *Files identical despite different names*

### Comparing `rasa-model-report-1.3.3/rasa_model_report/controllers/nlu_controller.py` & `rasa-model-report-1.3.4/rasa_model_report/controllers/nlu_controller.py`

 * *Files 5% similar despite different names*

```diff
@@ -170,18 +170,19 @@
     def _calculate_general_grade(self) -> Optional[float]:
         """
         Calculate the general grade value.
 
         :return: General grade value.
         """
         total_sentences = len(self._data)
-        if total_sentences:
-            total_problem_sentences = len(self._problem_sentences)
-            self._general_grade = 1 - total_problem_sentences / total_sentences
-            return self._general_grade
+        if not total_sentences:
+            return None
+        total_problem_sentences = len(self._problem_sentences)
+        self._general_grade = 1 - total_problem_sentences / total_sentences
+        return self._general_grade
 
     def request_nlu(self, text: str) -> type_aliases.nlu_payload:
         """
         Function that requests the NLU payload to the Rasa API.
 
         :param text: Sentence.
         :return: NLU payload.
@@ -200,16 +201,15 @@
     def _extract_sentences(text: str) -> List[str]:
         """
         Split and arrange sentences in a list.
 
         :param text: Sentences string file.
         :return: List of sentences.
         """
-        text = text.split("\n")
-        return [item[2:] for item in text if item != ""]
+        return [line.strip()[2:] for line in text.split("\n") if line.strip()]
 
     @staticmethod
     def remove_entities_from_text(text: str) -> str:
         """
         Remove Rasa entity syntax from text.
 
         :param text: Text with Rasa entity syntax.
```

### Comparing `rasa-model-report-1.3.3/rasa_model_report/helpers/utils.py` & `rasa-model-report-1.3.4/rasa_model_report/helpers/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,47 +14,46 @@
 from rasa_model_report.helpers import constants
 
 
 def format_date() -> str:
     """
     Format the current date to the format DD/MM/YY hh:mm:ss.
 
-    :return: Date string.
+    :return str: Date string.
     """
-    now = datetime.datetime.now()
-    return now.strftime("%d/%m/%y %H:%M:%S")
+    return datetime.datetime.now().strftime("%d/%m/%y %H:%M:%S")
 
 
 def convert_to_date(date: str) -> datetime.datetime:
     """
     Format string in the format DD/MM/YY hh:mm:ss to the datetime type.
 
     :param date: Date string.
-    :return: Datetime object.
+    :return datetime.datetime: Datetime object.
     """
     return datetime.datetime.strptime(date, "%d/%m/%y %H:%M:%S")
 
 
 def check(flag: bool) -> str:
     """
     Converts a boolean to an icon.
 
     :param flag: A boolean flag.
-    :return: A icon.
+    :return str: A icon.
     """
     return "✅" if flag else "❌"
 
 
 def get_color(value: float, scale: int = 1) -> str:
     """
     Returns a colored icon according to the value.
 
     :param value: Float value.
     :param scale: Scale that the value is on.
-    :return: A icon.
+    :return str: A icon.
     """
     if isinstance(value, (float, int)):
         if scale > 1:
             value /= scale
         if value >= 0.9:
             return "🟢"
         elif value >= 0.7:
@@ -69,15 +68,15 @@
 def change_scale(value: float, scale: int = 1, precision: int = 1) -> str:
     """
     Change the value scale and rounds it to display in string format.
 
     :param value: Value that will be changed to scale and rounds it.
     :param scale: Scale that will be applied.
     :param precision: Value precision.
-    :return: Value on the new scale and precision.
+    :return str: Value on the new scale and precision.
     """
     precision = precision if isinstance(precision, int) and 5 >= precision >= 0 else constants.GRADE_PRECISION
     if (
         isinstance(value, (float, int)) and
         isinstance(scale, (float, int)) and
         scale != 0
     ):
@@ -92,30 +91,28 @@
 
 
 def get_project_name(path: Optional[str] = None) -> str:
     """
     Returns the project folder's name.
 
     :param path: Project path. If not informed, the current path will be used.
-    :return: Project folder's name.
+    :return str: Project folder's name.
     """
-    if path:
-        return os.path.basename(path)
-    directory_path = os.getcwd()
+    directory_path = path or os.getcwd()
     return os.path.basename(directory_path)
 
 
 def request(url: str, method: str = "GET", json: dict = {}) -> Optional[requests.Response]:
     """
     Function that makes requests.
 
     :param url: URL.
     :param method: Request method (default: "GET").
     :param json: JSON body request (default: {}).
-    :return: Response object.
+    :return requests.Response: Response object.
     """
     response = None
     try:
         session = requests.Session()
         retries = Retry(total=2, backoff_factor=3)
         session.mount("http://", HTTPAdapter(max_retries=retries))
         response = session.request(method=method, url=url, json=json)
@@ -131,15 +128,15 @@
 
 def load_yaml_file(filename: str, error_flag: bool = True) -> Union[dict, list]:
     """
     Load data from YAML file.
 
     :param filename: YAML filename.
     :param error_flag: If True, an exception will be raised when the file isn't found (default: True).
-    :return: Data in list or dict format.
+    :return Union[dict, list]: Data in list or dict format.
     """
     if os.path.isfile(filename):
         file = open(filename, encoding="utf-8")
         data = safe_load(file)
         file.close()
         logging.info(f"{filename} file loaded successfully.")
         return data
@@ -155,26 +152,27 @@
 
 def list_diff(l1: List[str], l2: List[str]) -> List[str]:
     """
     Returns a list with the difference between l1 and l2 (l1 - l2).
 
     :param l1: First list.
     :param l2: Second list.
-    :return: Difference between l1 and l2.
+    :return list: Difference between l1 and l2.
     """
-    return [element for element in l1 if element not in l2]
+    set_l2 = set(l2)
+    return [element for element in l1 if element not in set_l2]
 
 
 def path_to(origin_path: str, destiny_path: str) -> str:
     """
     Return path to *destiny_path* from *origin_path*.
 
     :param origin_path: Origin path
     :param destiny_path: Destiny path
-    :return: Path to *destiny_path* from *origin_path*
+    :return str: Path to *destiny_path* from *origin_path*
     """
     undo_path = ""
     destiny_path = remove_duplicate_slashs(destiny_path)
     origin_path = remove_duplicate_slashs(origin_path)
     origin_path = origin_path[:-1] if origin_path[-1] == "/" else origin_path
     temp_path = origin_path
     while not destiny_path.startswith(temp_path):
@@ -191,10 +189,10 @@
 
 
 def remove_duplicate_slashs(text: str) -> str:
     """
     Remove duplicate slashs from string. Usually used in paths.
 
     :param text: Text string.
-    :return: Text without duplicate slashs.
+    :return str: Text without duplicate slashs.
     """
     return re.sub(r"\/+", "/", text)
```

### Comparing `rasa-model-report-1.3.3/rasa_model_report/main.py` & `rasa-model-report-1.3.4/rasa_model_report/main.py`

 * *Files identical despite different names*

### Comparing `rasa-model-report-1.3.3/rasa_model_report.egg-info/PKG-INFO` & `rasa-model-report-1.3.4/rasa_model_report.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rasa-model-report
-Version: 1.3.3
+Version: 1.3.4
 Summary: Simple open-source Rasa command-line add-on that generates training model health reports for your projects.
 Home-page: https://github.com/brunohjs/rasa-model-report
 Author: Bruno Justo
 Author-email: brunohjs@gmail.com
 License: Apache 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `rasa-model-report-1.3.3/rasa_model_report.egg-info/SOURCES.txt` & `rasa-model-report-1.3.4/rasa_model_report.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rasa-model-report-1.3.3/setup.cfg` & `rasa-model-report-1.3.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `rasa-model-report-1.3.3/setup.py` & `rasa-model-report-1.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="rasa-model-report",
-    version="1.3.3",
+    version="1.3.4",
     author="Bruno Justo",
     author_email="brunohjs@gmail.com",
     license="Apache 2.0",
     description="Simple open-source Rasa command-line add-on that "
                 "generates training model health reports for your projects.",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `rasa-model-report-1.3.3/tests/test_csv_controller.py` & `rasa-model-report-1.3.4/tests/test_csv_controller.py`

 * *Files identical despite different names*

### Comparing `rasa-model-report-1.3.3/tests/test_e2e_coverage_controller.py` & `rasa-model-report-1.3.4/tests/test_e2e_coverage_controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,15 +62,23 @@
 
 
 def test_generate_e2e_report_string():
     e2e_coverage_controller = pytest.e2e_coverage_controller
     e2e_coverage_controller._generate()
     assert e2e_coverage_controller._total_num_elements >= 0
     assert e2e_coverage_controller._total_num_not_covered >= 0
-    assert e2e_coverage_controller._total_rate >= 0
+    assert 1 >= e2e_coverage_controller._total_rate >= 0
+
+
+def test_generate_e2e_report_without_entities_section():
+    e2e_coverage_controller = pytest.e2e_coverage_controller
+    e2e_coverage_controller._generate()
+    assert "entities" not in e2e_coverage_controller.data
+    assert "intents" in e2e_coverage_controller.data
+    assert "actions" in e2e_coverage_controller.data
 
 
 def test_save_e2e_report_when_have_not_covered_items():
     e2e_coverage_controller = pytest.e2e_coverage_controller
     e2e_coverage_controller.save()
     assert os.path.isfile(f"{e2e_coverage_controller.results_path}/e2e_coverage_report.txt")
 
@@ -105,14 +113,15 @@
 
 
 def test_e2e_coverage_get_total_rate():
     e2e_coverage_controller = pytest.e2e_coverage_controller
     total_rate = e2e_coverage_controller.total_rate
     total_rate += 1
     assert e2e_coverage_controller.total_rate != total_rate
+    assert 1 >= e2e_coverage_controller._total_rate >= 0
     assert isinstance(e2e_coverage_controller.total_rate, float)
 
 
 def test_e2e_coverage_get_total_num_elements():
     e2e_coverage_controller = pytest.e2e_coverage_controller
     total_num_elements = e2e_coverage_controller.total_num_elements
     total_num_elements += 1
```

### Comparing `rasa-model-report-1.3.3/tests/test_json_controller.py` & `rasa-model-report-1.3.4/tests/test_json_controller.py`

 * *Files identical despite different names*

### Comparing `rasa-model-report-1.3.3/tests/test_main.py` & `rasa-model-report-1.3.4/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `rasa-model-report-1.3.3/tests/test_markdown_controller.py` & `rasa-model-report-1.3.4/tests/test_markdown_controller.py`

 * *Files identical despite different names*

### Comparing `rasa-model-report-1.3.3/tests/test_model_report.py` & `rasa-model-report-1.3.4/tests/test_model_report.py`

 * *Files identical despite different names*

### Comparing `rasa-model-report-1.3.3/tests/test_nlu_controller.py` & `rasa-model-report-1.3.4/tests/test_nlu_controller.py`

 * *Files identical despite different names*

### Comparing `rasa-model-report-1.3.3/tests/test_utils.py` & `rasa-model-report-1.3.4/tests/test_utils.py`

 * *Files identical despite different names*

