# Comparing `tmp/openclimate-0.1.4.tar.gz` & `tmp/openclimate-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openclimate-0.1.4.tar", last modified: Sat Mar 25 22:27:37 2023, max compression
+gzip compressed data, was "openclimate-0.1.5.tar", last modified: Sun Apr 16 18:05:32 2023, max compression
```

## Comparing `openclimate-0.1.4.tar` & `openclimate-0.1.5.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwxr-xr-x   0 luke       (501) staff       (20)        0 2023-03-25 22:27:37.165833 openclimate-0.1.4/
--rw-r--r--   0 luke       (501) staff       (20)    11357 2023-01-20 23:37:55.000000 openclimate-0.1.4/LICENSE
--rw-r--r--   0 luke       (501) staff       (20)     5623 2023-03-25 22:27:37.165891 openclimate-0.1.4/PKG-INFO
--rw-r--r--   0 luke       (501) staff       (20)     4959 2023-03-22 16:03:41.000000 openclimate-0.1.4/README.md
--rw-r--r--   0 luke       (501) staff       (20)       95 2023-01-20 23:37:55.000000 openclimate-0.1.4/pyproject.toml
--rw-r--r--   0 luke       (501) staff       (20)      784 2023-03-25 22:27:37.166360 openclimate-0.1.4/setup.cfg
--rw-r--r--   0 luke       (501) staff       (20)       69 2023-01-20 23:37:55.000000 openclimate-0.1.4/setup.py
-drwxr-xr-x   0 luke       (501) staff       (20)        0 2023-03-25 22:27:37.161186 openclimate-0.1.4/src/
-drwxr-xr-x   0 luke       (501) staff       (20)        0 2023-03-25 22:27:37.164665 openclimate-0.1.4/src/openclimate/
--rw-r--r--   0 luke       (501) staff       (20)     4723 2023-03-25 20:49:38.000000 openclimate-0.1.4/src/openclimate/ActorOverview.py
--rw-r--r--   0 luke       (501) staff       (20)      414 2023-03-19 16:55:43.000000 openclimate-0.1.4/src/openclimate/Base.py
--rw-r--r--   0 luke       (501) staff       (20)     5511 2023-03-25 19:33:00.000000 openclimate-0.1.4/src/openclimate/Client.py
--rw-r--r--   0 luke       (501) staff       (20)     3285 2023-03-25 19:20:14.000000 openclimate-0.1.4/src/openclimate/Emissions.py
--rw-r--r--   0 luke       (501) staff       (20)     1924 2023-03-25 19:22:56.000000 openclimate-0.1.4/src/openclimate/GDP.py
--rw-r--r--   0 luke       (501) staff       (20)     1928 2023-03-25 19:27:29.000000 openclimate-0.1.4/src/openclimate/Population.py
--rw-r--r--   0 luke       (501) staff       (20)     3141 2023-03-19 16:56:07.000000 openclimate-0.1.4/src/openclimate/Search.py
--rw-r--r--   0 luke       (501) staff       (20)     2584 2023-03-25 22:25:31.000000 openclimate-0.1.4/src/openclimate/Targets.py
--rw-r--r--   0 luke       (501) staff       (20)       99 2023-03-19 16:56:31.000000 openclimate-0.1.4/src/openclimate/__init__.py
--rw-r--r--   0 luke       (501) staff       (20)     1925 2023-03-25 18:51:44.000000 openclimate-0.1.4/src/openclimate/utils.py
-drwxr-xr-x   0 luke       (501) staff       (20)        0 2023-03-25 22:27:37.165708 openclimate-0.1.4/src/openclimate.egg-info/
--rw-r--r--   0 luke       (501) staff       (20)     5623 2023-03-25 22:27:37.000000 openclimate-0.1.4/src/openclimate.egg-info/PKG-INFO
--rw-r--r--   0 luke       (501) staff       (20)      554 2023-03-25 22:27:37.000000 openclimate-0.1.4/src/openclimate.egg-info/SOURCES.txt
--rw-r--r--   0 luke       (501) staff       (20)        1 2023-03-25 22:27:37.000000 openclimate-0.1.4/src/openclimate.egg-info/dependency_links.txt
--rw-r--r--   0 luke       (501) staff       (20)        1 2023-03-19 18:05:55.000000 openclimate-0.1.4/src/openclimate.egg-info/not-zip-safe
--rw-r--r--   0 luke       (501) staff       (20)       25 2023-03-25 22:27:37.000000 openclimate-0.1.4/src/openclimate.egg-info/requires.txt
--rw-r--r--   0 luke       (501) staff       (20)       12 2023-03-25 22:27:37.000000 openclimate-0.1.4/src/openclimate.egg-info/top_level.txt
+drwxr-xr-x   0 luke       (501) staff       (20)        0 2023-04-16 18:05:32.441938 openclimate-0.1.5/
+-rw-r--r--   0 luke       (501) staff       (20)    11357 2023-01-20 23:37:55.000000 openclimate-0.1.5/LICENSE
+-rw-r--r--   0 luke       (501) staff       (20)     5757 2023-04-16 18:05:32.442016 openclimate-0.1.5/PKG-INFO
+-rw-r--r--   0 luke       (501) staff       (20)     5069 2023-04-01 23:16:43.000000 openclimate-0.1.5/README.md
+-rw-r--r--   0 luke       (501) staff       (20)      503 2023-04-01 20:53:58.000000 openclimate-0.1.5/pyproject.toml
+-rw-r--r--   0 luke       (501) staff       (20)      964 2023-04-16 18:05:32.442428 openclimate-0.1.5/setup.cfg
+-rw-r--r--   0 luke       (501) staff       (20)       69 2023-01-20 23:37:55.000000 openclimate-0.1.5/setup.py
+drwxr-xr-x   0 luke       (501) staff       (20)        0 2023-04-16 18:05:32.435912 openclimate-0.1.5/src/
+drwxr-xr-x   0 luke       (501) staff       (20)        0 2023-04-16 18:05:32.440284 openclimate-0.1.5/src/openclimate/
+-rw-r--r--   0 luke       (501) staff       (20)     4753 2023-04-15 01:24:55.000000 openclimate-0.1.5/src/openclimate/ActorOverview.py
+-rw-r--r--   0 luke       (501) staff       (20)      414 2023-03-19 16:55:43.000000 openclimate-0.1.5/src/openclimate/Base.py
+-rw-r--r--   0 luke       (501) staff       (20)     5462 2023-04-01 20:47:40.000000 openclimate-0.1.5/src/openclimate/Client.py
+-rw-r--r--   0 luke       (501) staff       (20)     3685 2023-04-02 21:50:27.000000 openclimate-0.1.5/src/openclimate/Emissions.py
+-rw-r--r--   0 luke       (501) staff       (20)     1925 2023-04-01 20:47:40.000000 openclimate-0.1.5/src/openclimate/GDP.py
+-rw-r--r--   0 luke       (501) staff       (20)     1929 2023-04-01 20:47:40.000000 openclimate-0.1.5/src/openclimate/Population.py
+-rw-r--r--   0 luke       (501) staff       (20)     3222 2023-04-01 20:47:40.000000 openclimate-0.1.5/src/openclimate/Search.py
+-rw-r--r--   0 luke       (501) staff       (20)     2662 2023-04-15 01:35:15.000000 openclimate-0.1.5/src/openclimate/Targets.py
+-rw-r--r--   0 luke       (501) staff       (20)     1285 2023-04-02 22:56:03.000000 openclimate-0.1.5/src/openclimate/Tools.py
+-rw-r--r--   0 luke       (501) staff       (20)      191 2023-04-02 21:48:07.000000 openclimate-0.1.5/src/openclimate/__init__.py
+-rw-r--r--   0 luke       (501) staff       (20)     1938 2023-04-02 22:29:08.000000 openclimate-0.1.5/src/openclimate/utils.py
+drwxr-xr-x   0 luke       (501) staff       (20)        0 2023-04-16 18:05:32.441482 openclimate-0.1.5/src/openclimate.egg-info/
+-rw-r--r--   0 luke       (501) staff       (20)     5757 2023-04-16 18:05:32.000000 openclimate-0.1.5/src/openclimate.egg-info/PKG-INFO
+-rw-r--r--   0 luke       (501) staff       (20)      600 2023-04-16 18:05:32.000000 openclimate-0.1.5/src/openclimate.egg-info/SOURCES.txt
+-rw-r--r--   0 luke       (501) staff       (20)        1 2023-04-16 18:05:32.000000 openclimate-0.1.5/src/openclimate.egg-info/dependency_links.txt
+-rw-r--r--   0 luke       (501) staff       (20)        1 2023-03-19 18:05:55.000000 openclimate-0.1.5/src/openclimate.egg-info/not-zip-safe
+-rw-r--r--   0 luke       (501) staff       (20)       98 2023-04-16 18:05:32.000000 openclimate-0.1.5/src/openclimate.egg-info/requires.txt
+-rw-r--r--   0 luke       (501) staff       (20)       12 2023-04-16 18:05:32.000000 openclimate-0.1.5/src/openclimate.egg-info/top_level.txt
+drwxr-xr-x   0 luke       (501) staff       (20)        0 2023-04-16 18:05:32.441648 openclimate-0.1.5/tests/
+-rw-r--r--   0 luke       (501) staff       (20)     1198 2023-04-01 23:13:03.000000 openclimate-0.1.5/tests/test_Client.py
```

### Comparing `openclimate-0.1.4/LICENSE` & `openclimate-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `openclimate-0.1.4/PKG-INFO` & `openclimate-0.1.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openclimate
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python client for OpenClimate API
 Home-page: https://github.com/Open-Earth-Foundation/OpenClimate-pyclient
 Author: Luke Gloege
 License: Apache
 Keywords: GHG,emissions,climate data
 Platform: unix
 Platform: linux
@@ -14,26 +14,28 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: testing
 License-File: LICENSE
 
 # OpenClimate-pyclient
 
+![Tests](https://github.com/Open-Earth-Foundation/OpenClimate-pyclient/actions/workflows/tests.yml/badge.svg)
 [![Documentation Status](https://readthedocs.org/projects/openclimate-pyclient/badge/?version=latest)](https://openclimate-pyclient.readthedocs.io/en/latest/?badge=latest)
 [![pypi](https://badgen.net/pypi/v/openclimate)](https://pypi.org/project/openclimate)
 [![Formatted with black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![Examples on binder](https://img.shields.io/badge/launch-binder-579ACA.svg?logo=data:image/png;base64,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)](https://mybinder.org/v2/gh/Open-Earth-Foundation/OpenClimate-pyclient/HEAD?urlpath=lab/tree/docs/notebooks/)
 [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/Open-Earth-Foundation/OpenClimate-pyclient/issues)
 
-OpenClimate Python Client is a Python 3.6+ package for the [OpenClimate API](https://github.com/Open-Earth-Foundation/OpenClimate/blob/develop/api/API.md). The goal of this package is to make emissions data and pledges more accessible.
+OpenClimate Python Client is a Python 3.8+ package for the [OpenClimate API](https://github.com/Open-Earth-Foundation/OpenClimate/blob/develop/api/API.md). The goal of this package is to make emissions data and pledges more accessible.
 
 # Installation
 ```
 pip install openclimate
 ```
 
 # Usage
```

### Comparing `openclimate-0.1.4/README.md` & `openclimate-0.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # OpenClimate-pyclient
 
+![Tests](https://github.com/Open-Earth-Foundation/OpenClimate-pyclient/actions/workflows/tests.yml/badge.svg)
 [![Documentation Status](https://readthedocs.org/projects/openclimate-pyclient/badge/?version=latest)](https://openclimate-pyclient.readthedocs.io/en/latest/?badge=latest)
 [![pypi](https://badgen.net/pypi/v/openclimate)](https://pypi.org/project/openclimate)
 [![Formatted with black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![Examples on binder](https://img.shields.io/badge/launch-binder-579ACA.svg?logo=data:image/png;base64,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)](https://mybinder.org/v2/gh/Open-Earth-Foundation/OpenClimate-pyclient/HEAD?urlpath=lab/tree/docs/notebooks/)
 [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/Open-Earth-Foundation/OpenClimate-pyclient/issues)
 
-OpenClimate Python Client is a Python 3.6+ package for the [OpenClimate API](https://github.com/Open-Earth-Foundation/OpenClimate/blob/develop/api/API.md). The goal of this package is to make emissions data and pledges more accessible.
+OpenClimate Python Client is a Python 3.8+ package for the [OpenClimate API](https://github.com/Open-Earth-Foundation/OpenClimate/blob/develop/api/API.md). The goal of this package is to make emissions data and pledges more accessible.
 
 # Installation
 ```
 pip install openclimate
 ```
 
 # Usage
```

### Comparing `openclimate-0.1.4/setup.cfg` & `openclimate-0.1.5/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = openclimate
-version = 0.1.4
+version = 0.1.5
 description = Python client for OpenClimate API
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Luke Gloege
 url = https://github.com/Open-Earth-Foundation/OpenClimate-pyclient
 keywords = GHG, emissions, climate data
 license = Apache
@@ -24,11 +24,25 @@
 	pandas>1.5
 	requests>2.28
 python_requires = >=3.8
 package_dir = 
 	=src
 zip_safe = no
 
+[options.extras_require]
+testing = 
+	pytest>=6.0
+	pytest-cov>=2.0
+	mypy>=0.910
+	flake8>=3.9
+	tox>=3.24
+
+[options.package_data]
+slapping = py.typed
+
+[flake8]
+max-line-length = 160
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `openclimate-0.1.4/src/openclimate/ActorOverview.py` & `openclimate-0.1.5/src/openclimate/ActorOverview.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import asyncio
 from dataclasses import dataclass
 import pandas as pd
 import requests
-from typing import List, Dict, Union, Tuple
+from typing import List, Union, Tuple, Optional
 import warnings
 
 from .utils import async_func
 from .Base import Base
 
 
 @dataclass
@@ -14,15 +14,15 @@
     """ActorOveriew API class
     get overview information of an actor
 
     Returns:
         object
     """
     @async_func
-    def _overview_single_actor(self, actor_id: str = None, ignore_warnings: bool = False) -> Dict:
+    def _overview_single_actor(self, actor_id: str, ignore_warnings: bool = False, *args, **kwargs):
         """retreive actor emissions
 
         Args:
             actor_id (str): code for actor your want to retrieve
             ignore_warnings (bool): ignore warning messages
 
         Returns:
@@ -37,15 +37,15 @@
         if data_list is None:
             warnings.warn(
                 f"ActorIDError: {actor_id} was not found", category=SyntaxWarning
             )
             return None
         return data_list
 
-    async def _overview_coros(self, actor_id: str = None, ignore_warnings: bool = False) -> Dict:
+    async def _overview_coros(self, actor_id: Union[str, List[str], Tuple[str]], ignore_warnings: bool = False, *args, **kwargs):
         """overview coroutines
 
         Args:
             actor_id (str): actor identifier. Defaults to None.
             ignore_warnings (bool): ignore warning messages
 
         Returns:
@@ -56,29 +56,29 @@
             asyncio.create_task(self._overview_single_actor(actor, ignore_warnings))
             for actor in actor_list
         ]
         results = await asyncio.gather(*tasks)
         return results
 
     def overview(
-        self, actor_id: Union[str, List[str], Tuple[str]] = None, ignore_warnings: bool = False
-    ) -> List[Dict]:
+        self, actor_id: Union[str, List[str], Tuple[str]], ignore_warnings: bool = False
+    ):
         """Retretive actor overview
 
         Args:
             actor_id (Union[str, List[str], Tuple[str]]): actor identifier. Defaults to None.
             ignore_warnings (bool): ignore warning messages
 
         Returns:
             List[Dict]: dictionary with actor overview
         """
         return asyncio.run(self._overview_coros(actor_id=actor_id, ignore_warnings=ignore_warnings))
 
     def parts(
-        self, actor_id: str = None, part_type: str = None, *args, **kwargs
+        self, actor_id: str, part_type: Optional[str] = None, *args, **kwargs
     ) -> pd.DataFrame:
         """Retreive actor parts (e.g. subnational, cities, ...)
 
         Args:
             actor_id (str): code for actor your want to retrieve
             part_type (str, optional): administrative level
 
@@ -114,15 +114,15 @@
             return None
         else:
             df = pd.DataFrame(data_list).sort_values(by=["type", "actor_id"])
             return df
 
     def country_codes(
         self,
-        like: str = None,
+        like: Optional[str] = None,
         case_sensitive: bool = False,
         regex: bool = True,
         *args,
         **kwargs,
     ) -> pd.DataFrame:
         """returns two-letter country codes
```

### Comparing `openclimate-0.1.4/src/openclimate/Client.py` & `openclimate-0.1.5/src/openclimate/Client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from dataclasses import dataclass
 import pandas as pd
-from typing import List, Dict, Union, Tuple
+from typing import Optional
 
 from .ActorOverview import ActorOverview
 from .Base import Base
 from .Emissions import Emissions
 from .GDP import GDP
 from .Population import Population
 from .Search import Search
@@ -33,78 +33,78 @@
     @property
     def jupyter(self):
         import nest_asyncio
 
         nest_asyncio.apply()
 
     def emissions(
-        self, actor_id: str = None, datasource_id: str = None, ignore_warnings: bool = False
+        self, actor_id: str, datasource_id: Optional[str] = None, ignore_warnings: bool = False
     ) -> pd.DataFrame:
         """retreive actor emissions
 
         Args:
             actor_id (str|List[str]): code for actor your want to retrieve
             datasource_id (str): code emissions dataset
             ignore_warnings (bool): ignore warning messages
 
         Returns:
             DataFrame: data for each emissions dataset
         """
         return Emissions().emissions(actor_id=actor_id, datasource_id=datasource_id, ignore_warnings=ignore_warnings)
 
-    def emissions_datasets(self, actor_id: str = None, ignore_warnings: bool = False) -> pd.DataFrame:
+    def emissions_datasets(self, actor_id: str, ignore_warnings: bool = False) -> pd.DataFrame:
         """retreive actor emissions datasets
 
         Args:
             actor_id (str): code for actor your want to retrieve
             ignore_warnings (bool): ignore warning messages
 
         Returns:
             DataFrame: data of emission datasets
         """
         return Emissions().datasets(actor_id=actor_id, ignore_warnings=ignore_warnings)
 
-    def targets(self, actor_id: str = None, ignore_warnings: bool = False) -> pd.DataFrame:
+    def targets(self, actor_id: str, ignore_warnings: bool = False) -> pd.DataFrame:
         """retreive actor targets
 
         Args:
             actor_id (str|List[str]): code for actor your want to retrieve
             ignore_warnings (bool): ignore warning messages
 
         Returns:
             DataFrame: dataframe of targets
         """
         return Targets().targets(actor_id=actor_id, ignore_warnings=ignore_warnings)
 
-    def population(self, actor_id: str = None, ignore_warnings: bool = False) -> pd.DataFrame:
+    def population(self, actor_id: str, ignore_warnings: bool = False) -> pd.DataFrame:
         """retreive actor population
 
         Args:
             actor_id (str|List[str]): code for actor your want to retrieve
             ignore_warnings (bool): ignore warning messages
 
         Returns:
             DataFrame: dataframe of population
         """
         return Population().population(actor_id=actor_id, ignore_warnings=ignore_warnings)
 
-    def gdp(self, actor_id: str = None, ignore_warnings: bool = False) -> pd.DataFrame:
+    def gdp(self, actor_id: str, ignore_warnings: bool = False) -> pd.DataFrame:
         """retreive actor GDP
 
         Args:
             actor_id (str|List[str]): code for actor your want to retrieve
             ignore_warnings (bool): ignore warning messages
 
         Returns:
             DataFrame: dataframe of GDP
         """
         return GDP().gdp(actor_id=actor_id, ignore_warnings=ignore_warnings)
 
     def parts(
-        self, actor_id: str = None, part_type: str = None, *args, **kwargs
+        self, actor_id: str, part_type: Optional[str] = None, *args, **kwargs
     ) -> pd.DataFrame:
         """retreive actor parts
 
         returns subnational, cities, companies, etc. within an actor_id
 
         Args:
             actor_id (str|List[str]): code for actor your want to retrieve
@@ -113,19 +113,19 @@
         Returns:
             DataFrame: dataframe of actors parts
         """
         return ActorOverview().parts(actor_id=actor_id, part_type=part_type)
 
     def search(
         self,
-        name: str = None,
-        identifier: str = None,
-        query: str = None,
-        language: str = None,
-        namespace: str = None,
+        name: Optional[str] = None,
+        identifier: Optional[str] = None,
+        query: Optional[str] = None,
+        language: Optional[str] = None,
+        namespace: Optional[str] = None,
         *args,
         **kwargs,
     ) -> pd.DataFrame:
         """search actor names and identifiers
 
         Args:
             query (str): full search of identifiers and names that include the search parameter
@@ -139,21 +139,19 @@
         """
         return Search().search(
             name=name,
             identifier=identifier,
             query=query,
             language=language,
             namespace=namespace,
-            *args,
-            **kwargs,
         )
 
     def country_codes(
         self,
-        like: str = None,
+        like: Optional[str] = None,
         case_sensitive: bool = False,
         regex: bool = True,
         *args,
         **kwargs,
     ) -> pd.DataFrame:
         """get country codes and filter using `like` regex phrases
 
@@ -164,11 +162,10 @@
 
         Returns:
             DataFrame: dataframe of country codes
         """
         return (
             ActorOverview()
             .country_codes(
-                like=like, case_sensitive=case_sensitive, regex=regex, *args, **kwargs
-            )
+                like=like, case_sensitive=case_sensitive, regex=regex)
             .reset_index(drop=True)
         )
```

### Comparing `openclimate-0.1.4/src/openclimate/Emissions.py` & `openclimate-0.1.5/src/openclimate/Emissions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from dataclasses import dataclass
 import pandas as pd
-from typing import List, Dict, Union, Tuple
+from typing import List, Dict, Union, Tuple, Any, Optional
 
 from .ActorOverview import ActorOverview
 from .Base import Base
 
 
 @dataclass
 class Emissions(Base):
-    def _get_emissions(self, overview: Dict = None) -> pd.DataFrame:
+    def _get_emissions(self, overview: Dict[Any, Any]) -> pd.DataFrame:
         """retreive emissions from overview dictionary
 
         Args:
             overview (Dict): dictionary of overview
 
         Returns:
             pd.DataFrame
@@ -31,47 +31,58 @@
             .assign(actor_id=overview["actor_id"])
             .drop(columns=["tags", "emissions_id"])
             .loc[:, columns]
         )
         return df_out.reset_index(drop=True)
 
     def datasets(
-        self, actor_id: Union[str, List[str], Tuple[str]] = None, ignore_warnings: bool = False
+        self,
+        actor_id: Union[str, List[str], Tuple[str]],
+        ignore_warnings: bool = False,
+        *args,
+        **kwargs,
     ) -> pd.DataFrame:
         """retreive emissions datasets for an actor
 
         Args:
             actor_id (Union[str, List[str], Tuple[str]], optional): actor code
             ignore_warnings (bool, optional): ignore warnings messages
 
         Returns:
             pd.DataFrame:
         """
-        overviews = ActorOverview().overview(actor_id=actor_id, ignore_warnings=ignore_warnings)
-        list_out = [
-            {
-                "actor_id": overview.get("actor_id"),
-                "datasource_id": datasource,
-                "name": data.get("name"),
-                "publisher": data.get("publisher"),
-                "published": data.get("published"),
-                "URL": data.get("URL"),
-            }
-            for overview in overviews
-            if overview
-            for datasource, data in overview.get("emissions").items()
-        ]
-        if list_out:
-            return pd.DataFrame(list_out)
-        return None
+        try:
+            actor_id = [actor_id] if isinstance(actor_id, str) else actor_id
+            overviews = ActorOverview().overview(
+                actor_id=actor_id, ignore_warnings=ignore_warnings
+            )
+        except Exception:
+            print(f"Something went wrong, check that {actor_id} is an actor")
+        else:
+            list_out = [
+                {
+                    "actor_id": overview.get("actor_id"),
+                    "datasource_id": datasource,
+                    "name": data.get("name"),
+                    "publisher": data.get("publisher"),
+                    "published": data.get("published"),
+                    "URL": data.get("URL"),
+                }
+                for overview in overviews
+                if overview
+                for datasource, data in overview.get("emissions").items()
+            ]
+            if list_out:
+                return pd.DataFrame(list_out)
+            return None
 
     def emissions(
         self,
-        actor_id: Union[str, List[str], Tuple[str]] = None,
-        datasource_id: str = None,
+        actor_id: Union[str, List[str], Tuple[str]],
+        datasource_id: Optional[str] = None,
         ignore_warnings: bool = False,
         *args,
         **kwargs,
     ) -> pd.DataFrame:
         """retrieve actor emissions
 
         Args:
@@ -80,15 +91,17 @@
             ignore_warnings (bool, optional): ignore warnings messages
 
         Returns:
             pd.DataFrame: _description_
         """
         try:
             actor_id = [actor_id] if isinstance(actor_id, str) else actor_id
-            overviews = ActorOverview().overview(actor_id=actor_id, ignore_warnings=ignore_warnings)
+            overviews = ActorOverview().overview(
+                actor_id=actor_id, ignore_warnings=ignore_warnings
+            )
         except Exception:
             print(f"Something went wrong, check that {actor_id} is an actor")
         else:
             df_list = [
                 self._get_emissions(overview) for overview in overviews if overview
             ]
             df = pd.concat(df_list)
```

### Comparing `openclimate-0.1.4/src/openclimate/GDP.py` & `openclimate-0.1.5/src/openclimate/GDP.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from dataclasses import dataclass
 import pandas as pd
-from typing import List, Dict, Union, Tuple
+from typing import List, Dict, Union, Tuple, Any
 
 from .utils import explode_dict_columns
 from .utils import filter_overviews
 
 from .ActorOverview import ActorOverview
 from .Base import Base
 
 
 @dataclass
 class GDP(Base):
-    def _get_gdp(self, overview: Dict = None) -> pd.DataFrame:
+    def _get_gdp(self, overview: Dict[Any, Any]) -> pd.DataFrame:
         """retreive GDP from overview dictionary
 
         Args:
             overview (Dict): dictionary of overview
 
         Returns:
             pd.DataFrame
@@ -31,15 +31,15 @@
             "datasource_name",
             "datasource_published",
             "datasource_URL",
         ]
         return explode_dict_columns(df).loc[:, columns].reset_index(drop=True)
 
     def gdp(
-        self, actor_id: Union[str, List[str], Tuple[str]] = None, ignore_warnings: bool = False, *args, **kwargs
+        self, actor_id: Union[str, List[str], Tuple[str]], ignore_warnings: bool = False, *args, **kwargs
     ) -> pd.DataFrame:
         """retreive actor GDP
 
         Args:
             actor_id (Union[str, List[str], Tuple[str]], optional): actor code
             ignore_warnings (bool): ignore warning messages
```

### Comparing `openclimate-0.1.4/src/openclimate/Population.py` & `openclimate-0.1.5/src/openclimate/Population.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from dataclasses import dataclass
 import pandas as pd
-from typing import List, Dict, Union, Tuple
+from typing import List, Dict, Union, Tuple, Any
 
 from .utils import explode_dict_columns
 from .utils import filter_overviews
 
 from .ActorOverview import ActorOverview
 from .Base import Base
 
 
 @dataclass
 class Population(Base):
-    def _get_population(self, overview: Dict = None) -> pd.DataFrame:
+    def _get_population(self, overview: Dict[Any, Any]) -> pd.DataFrame:
         """retreive population from overview dictionary
 
         Args:
             overview (Dict): dictionary of overview
 
         Returns:
             pd.DataFrame
@@ -31,15 +31,15 @@
             "datasource_name",
             "datasource_published",
             "datasource_URL",
         ]
         return explode_dict_columns(df).loc[:, columns].reset_index(drop=True)
 
     def population(
-        self, actor_id: Union[str, List[str], Tuple[str]] = None, ignore_warnings: bool = False, *args, **kwargs
+        self, actor_id: Union[str, List[str], Tuple[str]], ignore_warnings: bool = False, *args, **kwargs
     ) -> pd.DataFrame:
         """retreive actor population
 
         Args:
             actor_id (Union[str, List[str], Tuple[str]], optional): actor code
             ignore_warnings (bool): ignore warning messages
```

### Comparing `openclimate-0.1.4/src/openclimate/Search.py` & `openclimate-0.1.5/src/openclimate/Search.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from dataclasses import dataclass
 import pandas as pd
 import requests
-from typing import List, Dict, Union, Tuple
+from typing import Optional
 
 from .Base import Base
 
 
 @dataclass
 class Search(Base):
     def _search_endpoint(
         self,
-        name: str = None,
-        identifier: str = None,
-        query: str = None,
-        language: str = None,
-        namespace: str = None,
+        name: Optional[str] = None,
+        identifier: Optional[str] = None,
+        query: Optional[str] = None,
+        language: Optional[str] = None,
+        namespace: Optional[str] = None,
         *args,
         **kwargs,
     ) -> str:
         """retrieve search endpoint
 
         Args:
             query (str): full search of identifiers and names that include the search parameter
@@ -32,33 +32,33 @@
         """
         count = sum(1 for x in [query, identifier, name] if x is not None)
         if count != 1:
             raise ValueError(
                 "Exactly one of 'query', 'identifier' or 'name' must be passed as input"
             )
         if query:
-            return f"/search/actor?q=" + query
+            return f"/search/actor?q={query}"
         elif identifier:
-            endpoint = f"/search/actor?identifier=" + identifier
+            endpoint = f"/search/actor?identifier={identifier}"
             if namespace:
-                endpoint += "&namespace=" + namespace
+                endpoint += f"&namespace={namespace}"
             return endpoint
         else:
-            endpoint = f"/search/actor?name=" + name
+            endpoint = f"/search/actor?name={name}"
             if language:
-                endpoint += "&language=" + language
+                endpoint += f"&language={language}"
             return endpoint
 
     def search(
         self,
-        name: str = None,
-        identifier: str = None,
-        query: str = None,
-        language: str = None,
-        namespace: str = None,
+        name: Optional[str] = None,
+        identifier: Optional[str] = None,
+        query: Optional[str] = None,
+        language: Optional[str] = None,
+        namespace: Optional[str] = None,
         *args,
         **kwargs,
     ) -> pd.DataFrame:
         """search actors
 
         Args:
             query (str): full search of identifiers and names that include the search parameter
```

### Comparing `openclimate-0.1.4/src/openclimate/Targets.py` & `openclimate-0.1.5/src/openclimate/Targets.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from dataclasses import dataclass
 import pandas as pd
-from typing import List, Dict, Union, Tuple
+from typing import List, Dict, Union, Tuple, Any
 
 from .utils import explode_dict_columns
 from .utils import filter_overviews
 
 from .ActorOverview import ActorOverview
 from .Base import Base
 
 
 @dataclass
 class Targets(Base):
-    def _get_target(self, overview: Dict = None) -> pd.DataFrame:
+    def _get_target(self, overview: Dict[Any, Any]) -> pd.DataFrame:
         """retreive targets from overview dictionary
 
         Args:
             overview (Dict): dictionary of overview
 
         Returns:
             pd.DataFrame
         """
         data = overview["targets"]
 
         if data:
-            columns = [
+            columns_tmp = [
                 "actor_id",
                 "target_type",
                 "baseline_year",
                 "baseline_value",
                 "target_year",
                 "target_value",
                 "target_unit",
@@ -42,26 +42,28 @@
                 "initiative_URL",
             ]
             df = (
                 pd.DataFrame(data)
                 .sort_values(by=["target_year"])
                 .assign(actor_id=overview["actor_id"])
             )
+
+            columns = [col for col in columns_tmp if col in df.columns]
+
             return (
                 explode_dict_columns(df)
                 .loc[:, columns]
                 .rename({"initiative_initiative_id": "initiative_id"})
                 .reset_index(drop=True)
             )
 
         return None
 
-
     def targets(
-        self, actor_id: Union[str, List[str], Tuple[str]] = None, ignore_warnings: bool = False, *args, **kwargs
+        self, actor_id: Union[str, List[str], Tuple[str]], ignore_warnings: bool = False, *args, **kwargs
     ) -> pd.DataFrame:
         """retreive actor targets
 
         Args:
             actor_id (Union[str, List[str], Tuple[str]], optional): actor code
             ignore_warnings (bool): ignore warning messages
```

### Comparing `openclimate-0.1.4/src/openclimate/utils.py` & `openclimate-0.1.5/src/openclimate/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import asyncio
 from functools import wraps
 import pandas as pd
-from typing import List, Dict, Union, Tuple
+from typing import List, Dict, Any
 import warnings
 
+
 def explode_dict_columns(df: pd.DataFrame = None) -> pd.DataFrame:
     """expand rows with dictionaries into separate columns
 
     Args:
         df (pd.DataFrame): pandas dataframe. Defaults to None.
 
     Returns:
@@ -35,15 +36,16 @@
     @wraps(func)
     async def wrapper(*args, **kwargs):
         loop = asyncio.get_event_loop()
         return await loop.run_in_executor(None, func, *args, **kwargs)
 
     return wrapper
 
-def filter_overviews(overviews: List[Dict], key: str, ignore_warnings: bool = False) -> List[Dict]:
+
+def filter_overviews(overviews: List[Dict[Any, Any]], key: str, ignore_warnings: bool = False) -> List[Dict[Any, Any]]:
     """filter overviews if has data for key
 
     Args:
         overviews (List[Dict]): list of actor overviews
         ignore_warnings (bool): ignore warning messages
 
     Returns:
@@ -55,9 +57,8 @@
     for overview in overviews:
         if overview.get(key):
             filtered_overviews.append(overview)
         else:
             warnings.warn(
                 f"NoDataError: {overview.get('actor_id')} has no {key} data", category=UserWarning
             )
-
-    return filtered_overviews
+    return filtered_overviews
```

### Comparing `openclimate-0.1.4/src/openclimate.egg-info/PKG-INFO` & `openclimate-0.1.5/src/openclimate.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openclimate
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python client for OpenClimate API
 Home-page: https://github.com/Open-Earth-Foundation/OpenClimate-pyclient
 Author: Luke Gloege
 License: Apache
 Keywords: GHG,emissions,climate data
 Platform: unix
 Platform: linux
@@ -14,26 +14,28 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: testing
 License-File: LICENSE
 
 # OpenClimate-pyclient
 
+![Tests](https://github.com/Open-Earth-Foundation/OpenClimate-pyclient/actions/workflows/tests.yml/badge.svg)
 [![Documentation Status](https://readthedocs.org/projects/openclimate-pyclient/badge/?version=latest)](https://openclimate-pyclient.readthedocs.io/en/latest/?badge=latest)
 [![pypi](https://badgen.net/pypi/v/openclimate)](https://pypi.org/project/openclimate)
 [![Formatted with black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![Examples on binder](https://img.shields.io/badge/launch-binder-579ACA.svg?logo=data:image/png;base64,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)](https://mybinder.org/v2/gh/Open-Earth-Foundation/OpenClimate-pyclient/HEAD?urlpath=lab/tree/docs/notebooks/)
 [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/Open-Earth-Foundation/OpenClimate-pyclient/issues)
 
-OpenClimate Python Client is a Python 3.6+ package for the [OpenClimate API](https://github.com/Open-Earth-Foundation/OpenClimate/blob/develop/api/API.md). The goal of this package is to make emissions data and pledges more accessible.
+OpenClimate Python Client is a Python 3.8+ package for the [OpenClimate API](https://github.com/Open-Earth-Foundation/OpenClimate/blob/develop/api/API.md). The goal of this package is to make emissions data and pledges more accessible.
 
 # Installation
 ```
 pip install openclimate
 ```
 
 # Usage
```

### Comparing `openclimate-0.1.4/src/openclimate.egg-info/SOURCES.txt` & `openclimate-0.1.5/src/openclimate.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 src/openclimate/Base.py
 src/openclimate/Client.py
 src/openclimate/Emissions.py
 src/openclimate/GDP.py
 src/openclimate/Population.py
 src/openclimate/Search.py
 src/openclimate/Targets.py
+src/openclimate/Tools.py
 src/openclimate/__init__.py
 src/openclimate/utils.py
 src/openclimate.egg-info/PKG-INFO
 src/openclimate.egg-info/SOURCES.txt
 src/openclimate.egg-info/dependency_links.txt
 src/openclimate.egg-info/not-zip-safe
 src/openclimate.egg-info/requires.txt
-src/openclimate.egg-info/top_level.txt
+src/openclimate.egg-info/top_level.txt
+tests/test_Client.py
```

