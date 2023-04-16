# Comparing `tmp/pyquora-0.3.0.tar.gz` & `tmp/pyquora-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyquora-0.3.0.tar", last modified: Thu Sep  2 04:54:43 2021, max compression
+gzip compressed data, was "pyquora-0.4.1.tar", last modified: Sun Apr 16 09:25:40 2023, max compression
```

## Comparing `pyquora-0.3.0.tar` & `pyquora-0.4.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-02 04:54:43.864246 pyquora-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1076 2021-09-02 04:54:31.000000 pyquora-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       15 2021-09-02 04:54:31.000000 pyquora-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2445 2021-09-02 04:54:43.864246 pyquora-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1204 2021-09-02 04:54:31.000000 pyquora-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-02 04:54:43.864246 pyquora-0.3.0/pyquora.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2445 2021-09-02 04:54:43.000000 pyquora-0.3.0/pyquora.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      392 2021-09-02 04:54:43.000000 pyquora-0.3.0/pyquora.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-02 04:54:43.000000 pyquora-0.3.0/pyquora.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-09-02 04:54:43.000000 pyquora-0.3.0/pyquora.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-09-02 04:54:43.000000 pyquora-0.3.0/pyquora.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-02 04:54:43.864246 pyquora-0.3.0/quora/
--rw-r--r--   0 runner    (1001) docker     (121)      264 2021-09-02 04:54:31.000000 pyquora-0.3.0/quora/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-02 04:54:31.000000 pyquora-0.3.0/quora/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1095 2021-09-02 04:54:31.000000 pyquora-0.3.0/quora/_parsers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1249 2021-09-02 04:54:31.000000 pyquora-0.3.0/quora/answer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1006 2021-09-02 04:54:31.000000 pyquora-0.3.0/quora/cache.py
--rw-r--r--   0 runner    (1001) docker     (121)      743 2021-09-02 04:54:31.000000 pyquora-0.3.0/quora/content.py
--rw-r--r--   0 runner    (1001) docker     (121)      203 2021-09-02 04:54:31.000000 pyquora-0.3.0/quora/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2550 2021-09-02 04:54:31.000000 pyquora-0.3.0/quora/profile.py
--rw-r--r--   0 runner    (1001) docker     (121)      453 2021-09-02 04:54:31.000000 pyquora-0.3.0/quora/question.py
--rw-r--r--   0 runner    (1001) docker     (121)      691 2021-09-02 04:54:31.000000 pyquora-0.3.0/quora/sync.py
--rw-r--r--   0 runner    (1001) docker     (121)      692 2021-09-02 04:54:31.000000 pyquora-0.3.0/quora/topic.py
--rw-r--r--   0 runner    (1001) docker     (121)     2234 2021-09-02 04:54:31.000000 pyquora-0.3.0/quora/user.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-09-02 04:54:43.864246 pyquora-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1456 2021-09-02 04:54:31.000000 pyquora-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:25:40.021825 pyquora-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-16 09:25:27.000000 pyquora-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-16 09:25:27.000000 pyquora-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-16 09:25:40.021825 pyquora-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-16 09:25:27.000000 pyquora-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:25:40.021825 pyquora-0.4.1/pyquora.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-16 09:25:39.000000 pyquora-0.4.1/pyquora.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-16 09:25:39.000000 pyquora-0.4.1/pyquora.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 09:25:39.000000 pyquora-0.4.1/pyquora.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-16 09:25:39.000000 pyquora-0.4.1/pyquora.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-16 09:25:39.000000 pyquora-0.4.1/pyquora.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:25:40.021825 pyquora-0.4.1/quora/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-16 09:25:27.000000 pyquora-0.4.1/quora/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 09:25:27.000000 pyquora-0.4.1/quora/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-16 09:25:27.000000 pyquora-0.4.1/quora/_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-16 09:25:27.000000 pyquora-0.4.1/quora/answer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-16 09:25:27.000000 pyquora-0.4.1/quora/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-16 09:25:27.000000 pyquora-0.4.1/quora/content.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-16 09:25:27.000000 pyquora-0.4.1/quora/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-16 09:25:27.000000 pyquora-0.4.1/quora/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-16 09:25:27.000000 pyquora-0.4.1/quora/question.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-16 09:25:27.000000 pyquora-0.4.1/quora/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-16 09:25:27.000000 pyquora-0.4.1/quora/topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-04-16 09:25:27.000000 pyquora-0.4.1/quora/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 09:25:40.021825 pyquora-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-16 09:25:27.000000 pyquora-0.4.1/setup.py
```

### Comparing `pyquora-0.3.0/LICENSE` & `pyquora-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyquora-0.3.0/PKG-INFO` & `pyquora-0.4.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,62 +1,65 @@
 Metadata-Version: 2.1
 Name: pyquora
-Version: 0.3.0
+Version: 0.4.1
 Summary: Fetch profiles and data from Quora.
 Home-page: https://github.com/TheShubhendra/pyquora
 Author: Shubhendra Kushwaha
 Author-email: shubhendrakushwaha94@gmail.com
 License: MIT
-Description: # pyquora
-        
-        Fetches user profiles and data from Quora.
-        
-        ![GitHub](https://img.shields.io/github/license/TheShubhendra/pyquora)
-        ![PyPI - Downloads](https://img.shields.io/pypi/dm/pyquora)
-        
-        ![GitHub last commit](https://img.shields.io/github/last-commit/TheShubhendra/pyquora)
-        
-        ![Build Status](https://img.shields.io/github/workflow/status/TheShubhendra/pyquora/Python%20package)
-        ![Requires.io (branch)](https://img.shields.io/requires/github/TheShubhendra/pyquora/master)
-        ![GitHub repo size](https://img.shields.io/github/repo-size/TheShubhendra/pyquora)
-        ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyquora)
-        ![PyPI - Wheel](https://img.shields.io/pypi/wheel/pyquora)
-        ![PyPI](https://img.shields.io/pypi/v/pyquora)
-        [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
-        ![PyPI - Status](https://img.shields.io/pypi/status/pyquora)
-        ![PyPI - Format](https://img.shields.io/pypi/format/pyquora)
-        
-        
-        # installation
-        
-        `pip install pyquora`
-        
-        # Usage
-        
-        ```python
-        import asyncio
-        from quora import User
-        
-        async def main():
-            user = User(<Quora-Username>)
-            profile = await user.profile()
-            print(profile.followerCount)
-        asyncio.run(main())
-        
-        ```
 Keywords: scraper,quora
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: Free For Educational Use
 Classifier: License :: Free For Home Use
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# pyquora
+
+Fetches user profiles and data from Quora.
+
+![GitHub](https://img.shields.io/github/license/TheShubhendra/pyquora)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/pyquora)
+
+![GitHub last commit](https://img.shields.io/github/last-commit/TheShubhendra/pyquora)
+
+![Build Status](https://img.shields.io/github/workflow/status/TheShubhendra/pyquora/Python%20package)
+![Requires.io (branch)](https://img.shields.io/requires/github/TheShubhendra/pyquora/master)
+![GitHub repo size](https://img.shields.io/github/repo-size/TheShubhendra/pyquora)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyquora)
+![PyPI - Wheel](https://img.shields.io/pypi/wheel/pyquora)
+![PyPI](https://img.shields.io/pypi/v/pyquora)
+[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
+![PyPI - Status](https://img.shields.io/pypi/status/pyquora)
+![PyPI - Format](https://img.shields.io/pypi/format/pyquora)
+
+
+# installation
+
+`pip install pyquora`
+
+# Usage
+
+```python
+import asyncio
+from quora import User
+
+async def main():
+    user = User(<Quora-Username>)
+    profile = await user.profile()
+    print(profile.followerCount)
+asyncio.run(main())
+
+```
```

### Comparing `pyquora-0.3.0/README.md` & `pyquora-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pyquora-0.3.0/pyquora.egg-info/PKG-INFO` & `pyquora-0.4.1/pyquora.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,62 +1,65 @@
 Metadata-Version: 2.1
 Name: pyquora
-Version: 0.3.0
+Version: 0.4.1
 Summary: Fetch profiles and data from Quora.
 Home-page: https://github.com/TheShubhendra/pyquora
 Author: Shubhendra Kushwaha
 Author-email: shubhendrakushwaha94@gmail.com
 License: MIT
-Description: # pyquora
-        
-        Fetches user profiles and data from Quora.
-        
-        ![GitHub](https://img.shields.io/github/license/TheShubhendra/pyquora)
-        ![PyPI - Downloads](https://img.shields.io/pypi/dm/pyquora)
-        
-        ![GitHub last commit](https://img.shields.io/github/last-commit/TheShubhendra/pyquora)
-        
-        ![Build Status](https://img.shields.io/github/workflow/status/TheShubhendra/pyquora/Python%20package)
-        ![Requires.io (branch)](https://img.shields.io/requires/github/TheShubhendra/pyquora/master)
-        ![GitHub repo size](https://img.shields.io/github/repo-size/TheShubhendra/pyquora)
-        ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyquora)
-        ![PyPI - Wheel](https://img.shields.io/pypi/wheel/pyquora)
-        ![PyPI](https://img.shields.io/pypi/v/pyquora)
-        [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
-        ![PyPI - Status](https://img.shields.io/pypi/status/pyquora)
-        ![PyPI - Format](https://img.shields.io/pypi/format/pyquora)
-        
-        
-        # installation
-        
-        `pip install pyquora`
-        
-        # Usage
-        
-        ```python
-        import asyncio
-        from quora import User
-        
-        async def main():
-            user = User(<Quora-Username>)
-            profile = await user.profile()
-            print(profile.followerCount)
-        asyncio.run(main())
-        
-        ```
 Keywords: scraper,quora
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: Free For Educational Use
 Classifier: License :: Free For Home Use
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# pyquora
+
+Fetches user profiles and data from Quora.
+
+![GitHub](https://img.shields.io/github/license/TheShubhendra/pyquora)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/pyquora)
+
+![GitHub last commit](https://img.shields.io/github/last-commit/TheShubhendra/pyquora)
+
+![Build Status](https://img.shields.io/github/workflow/status/TheShubhendra/pyquora/Python%20package)
+![Requires.io (branch)](https://img.shields.io/requires/github/TheShubhendra/pyquora/master)
+![GitHub repo size](https://img.shields.io/github/repo-size/TheShubhendra/pyquora)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyquora)
+![PyPI - Wheel](https://img.shields.io/pypi/wheel/pyquora)
+![PyPI](https://img.shields.io/pypi/v/pyquora)
+[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
+![PyPI - Status](https://img.shields.io/pypi/status/pyquora)
+![PyPI - Format](https://img.shields.io/pypi/format/pyquora)
+
+
+# installation
+
+`pip install pyquora`
+
+# Usage
+
+```python
+import asyncio
+from quora import User
+
+async def main():
+    user = User(<Quora-Username>)
+    profile = await user.profile()
+    print(profile.followerCount)
+asyncio.run(main())
+
+```
```

### Comparing `pyquora-0.3.0/quora/_parsers.py` & `pyquora-0.4.1/quora/_parsers.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,34 +2,35 @@
 import json
 import re
 
 from quora.answer import Answer
 from quora.topic import Topic
 from .exceptions import ProfileNotFoundError
 
-
+# noqa: E501
 def parse_page(html_data, user):
     """Parse HTML and return JSON."""
     try:
-        data = re.findall(
-            r'window\.ansFrontendGlobals\.data\.inlineQueryResults\.results\[".*?"\] = ("{.*}");',  # noqa: E501
+        data = re.search(
+            r'window\.ansFrontendGlobals\.data\.inlineQueryResults\.results\[".*\]\.push\((?P<extracted_data>\".*\")\);',
             html_data,
-        )[-1]
+        )
+        data = data.group('extracted_data')
         data = json.loads(json.loads(data))
         return data["data"]["user"]
     except Exception as e:
-        user.logger.exception("Unable to Parse the profile")
+        # user.logger.warn("Unable to Parse the profile")
         raise ProfileNotFoundError(
             f"No profile\
 found with the username {user.username}."
         )
 
 
-def parse_answers(json_data, user):
+def parse_answers(json_data, user, language):
     """Parse JSON string of answers and return list of `Answer` object."""
     answers = json_data["recentPublicAndPinnedAnswersConnection"]["edges"]
-    return [Answer(ans["node"], user) for ans in answers]
+    return [Answer(ans["node"], user, language) for ans in answers]
 
 
-def parse_topics(json_data):
+def parse_topics(json_data, language):
     topics = json_data["expertiseTopicsConnection"]["edges"]
-    return [Topic(topic["node"]) for topic in topics]
+    return [Topic(topic["node"], language) for topic in topics]
```

### Comparing `pyquora-0.3.0/quora/answer.py` & `pyquora-0.4.1/quora/answer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """Answer class to represent a Quora answer."""
 from quora.content import Content
 from quora.question import Question
 
 
 class Answer:
-    def __init__(self, data_dict, user):
+    def __init__(self, data_dict, user, language="en"):
         """Constructs the `Answer` object."""
         self.id = data_dict.get("id")
         self.aid = data_dict.get("aid")
         self.isPinned = data_dict.get("isPinned")
         self.question = Question(data_dict.get("question"))
+        self.language = language
         self.url = "https://www.quora.com" + data_dict.get("permaUrl")
         self.content = Content(data_dict.get("content"))
         self.creationTime = data_dict.get("creationTime")
         self.updatedTime = data_dict.get("updatedTime")
         self.author = data_dict.get("author")
         self.user = user
         self.username = self.user.username
```

### Comparing `pyquora-0.3.0/quora/cache.py` & `pyquora-0.4.1/quora/cache.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,29 +2,31 @@
 
 logger = logging.getLogger(__name__)
 
 
 def cache(cache_exp=None):
     def decorator(func):
         async def _wrapper(user, *args, **kwargs):
-            key = f"pyquora_{func.__name__}_{user.username}"
+            key = f"pyquora_{func.__name__}_{user.username}_{kwargs.get('language','en')}"
             if user._cache is not None:
                 value = user._cache.get(key)
                 if value is not None:
                     logger.info(f"Using cache from {key}")
                     return value
             res = await func(user, *args, **kwargs)
             if user._cache is not None:
                 time = 0
                 if kwargs.get("cache_exp"):
                     time = kwargs.get("cache_exp")
                 elif user._cache_exp:
                     time = user._cache_exp
                 elif cache_exp:
                     time = cache_exp
+                if not isinstance(time, int):
+                    raise TypeError(f"cache expiry time should be in int. I got {time} instead.")
                 logger.info(f"Storing cache into {key} will expire in {time} seconds")
                 user._cache.set(key, res, time=time)
             return res
 
         return _wrapper
 
     return decorator
```

### Comparing `pyquora-0.3.0/quora/content.py` & `pyquora-0.4.1/quora/content.py`

 * *Files identical despite different names*

### Comparing `pyquora-0.3.0/quora/profile.py` & `pyquora-0.4.1/quora/profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Contains Profile class."""
 import json
 
 
 class Profile:
     """Represent the profile of a quora user."""
 
-    def __init__(self, user, data):
+    def __init__(self, user, data, language="en"):
         """Constructor for Profile."""
         self.user = user
         self.username = user.username
         self.id = data.get("id")
         self.uid = data.get("uid")
+        self.language = language
         self.profileImage = data.get("profileImageUrl")
         try:
             self.firstName = data["names"][0]["givenName"]
         except Exception:
             self.firstName = None
         try:
             self.lastName = data["names"][0]["familyName"]
```

### Comparing `pyquora-0.3.0/quora/sync.py` & `pyquora-0.4.1/quora/sync.py`

 * *Files identical despite different names*

### Comparing `pyquora-0.3.0/quora/topic.py` & `pyquora-0.4.1/quora/topic.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 class Topic:
     """Class to represent a topic."""
 
-    def __init__(self, json_data):
+    def __init__(self, json_data, language="en"):
         self.id = json_data.get("id")
         self.name = json_data.get("name")
         self.url = "https://www.quora.com" + json_data.get("url")
+        self.language = language
         self.photoUrl = json_data.get("photoUrl")
         self.followerCount = json_data.get("numFollowers")
         self.userAnswersCount = json_data.get("numPublicAnswersOfUser")
         # From August 2021 Quora started using dynamic loading of answers.
-        #self.userAnswersUrl = "https://www.quora.com" + json_data.get("userAnswersUrl")
+        # self.userAnswersUrl = "https://www.quora.com" + json_data.get("userAnswersUrl")
 
     def __str__(self):
         return self.name
 
     def __eq__(self, other):
         return self.id == other.id
```

### Comparing `pyquora-0.3.0/setup.py` & `pyquora-0.4.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         requirements = f.read()
     return requirements
 
 
 setup(
     name="pyquora",
     packages=find_packages(),
-    version="0.3.0",
+    version="0.4.1",
     license="MIT",
     description="""Fetch profiles and data from Quora.""",
     author="Shubhendra Kushwaha",
     author_email="shubhendrakushwaha94@gmail.com",
     url="https://github.com/TheShubhendra/pyquora",
     keywords=[
         "scraper",
@@ -40,10 +40,12 @@
         "License :: Free For Educational Use",
         "License :: Free For Home Use",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     python_requires=">=3.7",
 )
```

