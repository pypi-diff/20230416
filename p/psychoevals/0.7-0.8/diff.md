# Comparing `tmp/psychoevals-0.7.tar.gz` & `tmp/psychoevals-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psychoevals-0.7.tar", last modified: Sun Apr 16 17:11:50 2023, max compression
+gzip compressed data, was "psychoevals-0.8.tar", last modified: Sun Apr 16 18:56:17 2023, max compression
```

## Comparing `psychoevals-0.7.tar` & `psychoevals-0.8.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-16 17:11:50.756813 psychoevals-0.7/
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      328 2023-04-16 17:11:50.756813 psychoevals-0.7/PKG-INFO
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     6727 2023-04-14 22:46:24.000000 psychoevals-0.7/README.md
-drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-16 17:11:50.756813 psychoevals-0.7/psychoevals/
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-13 22:48:29.000000 psychoevals-0.7/psychoevals/__init__.py
-drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-16 17:11:50.756813 psychoevals-0.7/psychoevals/agents/
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 22:46:24.000000 psychoevals-0.7/psychoevals/agents/__init__.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     1115 2023-04-15 21:38:26.000000 psychoevals-0.7/psychoevals/agents/base_eval_agent.py
-drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-16 17:11:50.756813 psychoevals-0.7/psychoevals/agents/myers_briggs/
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)       37 2023-04-14 22:46:24.000000 psychoevals-0.7/psychoevals/agents/myers_briggs/__init__.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     3569 2023-04-15 21:25:01.000000 psychoevals-0.7/psychoevals/agents/myers_briggs/mbti_statements.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     2683 2023-04-15 21:29:36.000000 psychoevals-0.7/psychoevals/agents/myers_briggs/myers_briggs.py
-drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-16 17:11:50.756813 psychoevals-0.7/psychoevals/agents/troll_agent/
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)       35 2023-04-14 22:46:24.000000 psychoevals-0.7/psychoevals/agents/troll_agent/__init__.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     1030 2023-04-15 20:59:18.000000 psychoevals-0.7/psychoevals/agents/troll_agent/troll_agent.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      446 2023-04-15 18:58:27.000000 psychoevals-0.7/psychoevals/analysis.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      378 2023-04-13 23:06:38.000000 psychoevals-0.7/psychoevals/cognitive_state.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      363 2023-04-15 21:34:33.000000 psychoevals-0.7/psychoevals/eval.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     2401 2023-04-16 16:55:33.000000 psychoevals-0.7/psychoevals/moderation.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      121 2023-04-12 23:17:13.000000 psychoevals-0.7/psychoevals/qna_result.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     5083 2023-04-16 17:01:48.000000 psychoevals-0.7/psychoevals/security.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     3882 2023-04-14 22:46:24.000000 psychoevals-0.7/psychoevals/utils.py
-drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-16 17:11:50.756813 psychoevals-0.7/psychoevals.egg-info/
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      328 2023-04-16 17:11:50.000000 psychoevals-0.7/psychoevals.egg-info/PKG-INFO
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      800 2023-04-16 17:11:50.000000 psychoevals-0.7/psychoevals.egg-info/SOURCES.txt
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)        1 2023-04-16 17:11:50.000000 psychoevals-0.7/psychoevals.egg-info/dependency_links.txt
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)       67 2023-04-16 17:11:50.000000 psychoevals-0.7/psychoevals.egg-info/requires.txt
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)       18 2023-04-16 17:11:50.000000 psychoevals-0.7/psychoevals.egg-info/top_level.txt
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)       38 2023-04-16 17:11:50.756813 psychoevals-0.7/setup.cfg
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      579 2023-04-16 17:11:47.000000 psychoevals-0.7/setup.py
-drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-16 17:11:50.756813 psychoevals-0.7/tests/
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 20:36:27.000000 psychoevals-0.7/tests/__init__.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     3052 2023-04-14 22:46:24.000000 psychoevals-0.7/tests/test_mbti.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     2373 2023-04-15 21:44:06.000000 psychoevals-0.7/tests/test_moderation.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     1795 2023-04-16 17:10:22.000000 psychoevals-0.7/tests/test_security.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     1206 2023-04-15 21:40:35.000000 psychoevals-0.7/tests/test_troll_agent.py
+drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-16 18:56:17.506812 psychoevals-0.8/
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      328 2023-04-16 18:56:17.506812 psychoevals-0.8/PKG-INFO
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     7104 2023-04-16 18:55:19.000000 psychoevals-0.8/README.md
+drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-16 18:56:17.506812 psychoevals-0.8/psychoevals/
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-13 22:48:29.000000 psychoevals-0.8/psychoevals/__init__.py
+drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-16 18:56:17.506812 psychoevals-0.8/psychoevals/agents/
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 22:46:24.000000 psychoevals-0.8/psychoevals/agents/__init__.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     1115 2023-04-15 21:38:26.000000 psychoevals-0.8/psychoevals/agents/base_eval_agent.py
+drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-16 18:56:17.506812 psychoevals-0.8/psychoevals/agents/myers_briggs/
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)       37 2023-04-14 22:46:24.000000 psychoevals-0.8/psychoevals/agents/myers_briggs/__init__.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     3569 2023-04-16 18:55:19.000000 psychoevals-0.8/psychoevals/agents/myers_briggs/mbti_statements.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     2683 2023-04-16 18:55:19.000000 psychoevals-0.8/psychoevals/agents/myers_briggs/myers_briggs.py
+drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-16 18:56:17.506812 psychoevals-0.8/psychoevals/agents/troll_agent/
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)       35 2023-04-14 22:46:24.000000 psychoevals-0.8/psychoevals/agents/troll_agent/__init__.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     1030 2023-04-15 20:59:18.000000 psychoevals-0.8/psychoevals/agents/troll_agent/troll_agent.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      446 2023-04-15 18:58:27.000000 psychoevals-0.8/psychoevals/analysis.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      378 2023-04-13 23:06:38.000000 psychoevals-0.8/psychoevals/cognitive_state.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      363 2023-04-15 21:34:33.000000 psychoevals-0.8/psychoevals/eval.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     2401 2023-04-16 16:55:33.000000 psychoevals-0.8/psychoevals/moderation.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      121 2023-04-12 23:17:13.000000 psychoevals-0.8/psychoevals/qna_result.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     5083 2023-04-16 17:01:48.000000 psychoevals-0.8/psychoevals/security.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     3882 2023-04-14 22:46:24.000000 psychoevals-0.8/psychoevals/utils.py
+drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-16 18:56:17.506812 psychoevals-0.8/psychoevals.egg-info/
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      328 2023-04-16 18:56:17.000000 psychoevals-0.8/psychoevals.egg-info/PKG-INFO
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      800 2023-04-16 18:56:17.000000 psychoevals-0.8/psychoevals.egg-info/SOURCES.txt
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)        1 2023-04-16 18:56:17.000000 psychoevals-0.8/psychoevals.egg-info/dependency_links.txt
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)       67 2023-04-16 18:56:17.000000 psychoevals-0.8/psychoevals.egg-info/requires.txt
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)       18 2023-04-16 18:56:17.000000 psychoevals-0.8/psychoevals.egg-info/top_level.txt
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)       38 2023-04-16 18:56:17.506812 psychoevals-0.8/setup.cfg
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      579 2023-04-16 18:55:19.000000 psychoevals-0.8/setup.py
+drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-16 18:56:17.506812 psychoevals-0.8/tests/
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 20:36:27.000000 psychoevals-0.8/tests/__init__.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     3052 2023-04-14 22:46:24.000000 psychoevals-0.8/tests/test_mbti.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     2373 2023-04-15 21:44:06.000000 psychoevals-0.8/tests/test_moderation.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     1795 2023-04-16 17:10:22.000000 psychoevals-0.8/tests/test_security.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     1206 2023-04-15 21:40:35.000000 psychoevals-0.8/tests/test_troll_agent.py
```

### Comparing `psychoevals-0.7/README.md` & `psychoevals-0.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # PsychoEvals: Prompt Security and Psychometrics Framework for LLMs
 
 PsychoEvals is a lightweight Python library for evaluating and securing the behavior of large language models (LLMs) and agents, such as OpenAI's GPT series. The library provides a testing framework that enables researchers, developers, and enthusiasts to better understand, evaluate, and secure LLMs using psychometric tests, security features, and moderation tools.
 
 🚀 4 Canonical Use Cases
 
+* [Colab notebook](https://colab.research.google.com/drive/1Dex0CWIhZZTxQTfMcQHzGLluxmBM1eTm?usp=sharing) Secure your LLM response from basic prompt hijacking and injection attacks, and add your own tests. 
 * Apply a battery of 'troll' questions to provoke a NSFW answer from your Chatbot prompt
-* Apply psychometric tests on Agent prompts (aka `CognitiveState`)
-* Secure your LLM response from basic prompt hijacking and injection attacks
-* Moderate the response from your LLM for any issues based on some criteria (hate, violence, etc)
+* [Colab notebook](https://colab.research.google.com/drive/1aeamLCKxNJqAZYWvoCNh1Lf0Edb8gBd0?usp=sharing ) Apply psychometric tests on Agent prompts (aka `CognitiveState`)
+* [Colab notebook](https://colab.research.google.com/drive/1WkU-qM3mJ0E2dP00o_0EfqCJy1fljlOY?usp=sharing ) Moderate the response from your LLM calls for any issues based on some criteria (hate, violence, etc) & do pre and post processing 
+
 
 💾 Install
 
 1) pip install the module. 
 `pip install psychoevals`
 
 2) create a virtual env, i.e.
```

### Comparing `psychoevals-0.7/psychoevals/agents/base_eval_agent.py` & `psychoevals-0.8/psychoevals/agents/base_eval_agent.py`

 * *Files identical despite different names*

### Comparing `psychoevals-0.7/psychoevals/agents/myers_briggs/mbti_statements.py` & `psychoevals-0.8/psychoevals/agents/myers_briggs/mbti_statements.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,23 +4,23 @@
     {"prompt": "I enjoy being the center of attention.", "meta": {"dimension": "E"}},
     {"prompt": "I prefer socializing in large groups.", "meta": {"dimension": "E"}},
     {"prompt": "I find it easy to make small talk.", "meta": {"dimension": "E"}},
     {"prompt": "I am more comfortable in social situations than being alone.", "meta": {"dimension": "E"}},
     {"prompt": "I enjoy meeting new people and making friends.", "meta": {"dimension": "E"}},
     {"prompt": "I am outgoing and sociable.", "meta": {"dimension": "E"}},
     {"prompt": "I find it easy to strike up a conversation with strangers.", "meta": {"dimension": "E"}},    
-    {"prompt": "I prefer abstract ideas over concrete facts.", "meta": {"dimension": "N"}},
-    {"prompt": "I prefer to focus on the bigger picture rather than the details.", "meta": {"dimension": "N"}},
-    {"prompt": "I am more interested in future possibilities than present realities.", "meta": {"dimension": "N"}},
-    {"prompt": "I often think about how things could be improved.", "meta": {"dimension": "N"}},
-    {"prompt": "I enjoy discussing theories and concepts.", "meta": {"dimension": "N"}},
-    {"prompt": "I often get lost in thought and daydreams.", "meta": {"dimension": "N"}},
-    {"prompt": "I find it easy to understand complex ideas and theories.", "meta": {"dimension": "N"}},
-    {"prompt": "I enjoy learning about new and innovative ideas.", "meta": {"dimension": "N"}},
-    {"prompt": "I enjoy thinking about hypothetical scenarios and possibilities.", "meta": {"dimension": "N"}},
+    {"prompt": "I prefer abstract ideas over concrete facts.", "meta": {"dimension": "S"}},
+    {"prompt": "I prefer to focus on the bigger picture rather than the details.", "meta": {"dimension": "S"}},
+    {"prompt": "I am more interested in future possibilities than present realities.", "meta": {"dimension": "S"}},
+    {"prompt": "I often think about how things could be improved.", "meta": {"dimension": "S"}},
+    {"prompt": "I enjoy discussing theories and concepts.", "meta": {"dimension": "S"}},
+    {"prompt": "I often get lost in thought and daydreams.", "meta": {"dimension": "S"}},
+    {"prompt": "I find it easy to understand complex ideas and theories.", "meta": {"dimension": "S"}},
+    {"prompt": "I enjoy learning about new and innovative ideas.", "meta": {"dimension": "S"}},
+    {"prompt": "I enjoy thinking about hypothetical scenarios and possibilities.", "meta": {"dimension": "S"}},
     {"prompt": "I make decisions based on logic and reason.", "meta": {"dimension": "T"}},
     {"prompt": "I consider how my decisions will affect others.", "meta": {"dimension": "T"}},
     {"prompt": "When solving problems, I prioritize finding the best solution over preserving harmony.", "meta": {"dimension": "T"}},
     {"prompt": "I am more focused objective criteria when making decisions than my feelings.", "meta": {"dimension": "T"}},
     {"prompt": "I am more objective than subjective.", "meta": {"dimension": "T"}},
     {"prompt": "I don't enjoy discussing my values and personal beliefs.", "meta": {"dimension": "T"}},
     {"prompt": "I find it important to analyze situations logically.", "meta": {"dimension": "T"}},
```

### Comparing `psychoevals-0.7/psychoevals/agents/myers_briggs/myers_briggs.py` & `psychoevals-0.8/psychoevals/agents/myers_briggs/myers_briggs.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 
     def evaluate(self, cognitive_state):
         results = []
 
         def oppposite_dimension(mbti_dimension):
             if mbti_dimension == "E":
                 return "I"
-            elif mbti_dimension == "N":
-                return "S"
+            elif mbti_dimension == "S":
+                return "N"
             elif mbti_dimension == "T":
                 return "F"
             elif mbti_dimension == "J":
                 return "P"
 
         for eval in self.get_evals():
             prompt = eval.prompt
```

### Comparing `psychoevals-0.7/psychoevals/agents/troll_agent/troll_agent.py` & `psychoevals-0.8/psychoevals/agents/troll_agent/troll_agent.py`

 * *Files identical despite different names*

### Comparing `psychoevals-0.7/psychoevals/moderation.py` & `psychoevals-0.8/psychoevals/moderation.py`

 * *Files identical despite different names*

### Comparing `psychoevals-0.7/psychoevals/security.py` & `psychoevals-0.8/psychoevals/security.py`

 * *Files identical despite different names*

### Comparing `psychoevals-0.7/psychoevals/utils.py` & `psychoevals-0.8/psychoevals/utils.py`

 * *Files identical despite different names*

### Comparing `psychoevals-0.7/psychoevals.egg-info/SOURCES.txt` & `psychoevals-0.8/psychoevals.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `psychoevals-0.7/setup.py` & `psychoevals-0.8/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='psychoevals',
-    version='0.7',
+    version='0.8',
     packages=find_packages(),
     install_requires=[
         "openai>=0.27.0",
         "pandas>=1.3.0",
         "tenacity>=8.0.0",
         "python-dotenv>=0.15.0"
     ],
```

### Comparing `psychoevals-0.7/tests/test_mbti.py` & `psychoevals-0.8/tests/test_mbti.py`

 * *Files identical despite different names*

### Comparing `psychoevals-0.7/tests/test_moderation.py` & `psychoevals-0.8/tests/test_moderation.py`

 * *Files identical despite different names*

### Comparing `psychoevals-0.7/tests/test_security.py` & `psychoevals-0.8/tests/test_security.py`

 * *Files identical despite different names*

### Comparing `psychoevals-0.7/tests/test_troll_agent.py` & `psychoevals-0.8/tests/test_troll_agent.py`

 * *Files identical despite different names*

