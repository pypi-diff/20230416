# Comparing `tmp/gameyamlspiderandgenerator-1.0.0.tar.gz` & `tmp/gameyamlspiderandgenerator-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gameyamlspiderandgenerator-1.0.0.tar", max compression
+gzip compressed data, was "gameyamlspiderandgenerator-1.1.0.tar", max compression
```

## Comparing `gameyamlspiderandgenerator-1.0.0.tar` & `gameyamlspiderandgenerator-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rwxr-xr-x   0        0        0     1069 2022-12-30 03:55:28.534848 gameyamlspiderandgenerator-1.0.0/LICENSE
--rwxr-xr-x   0        0        0      809 2023-04-13 11:43:35.714655 gameyamlspiderandgenerator-1.0.0/README.md
--rwxr-xr-x   0        0        0      610 2023-04-13 11:36:40.137059 gameyamlspiderandgenerator-1.0.0/gameyamlspiderandgenerator/__init__.py
--rwxr-xr-x   0        0        0      980 2023-04-13 11:25:54.309363 gameyamlspiderandgenerator-1.0.0/gameyamlspiderandgenerator/__main__.py
--rwxr-xr-x   0        0        0      753 2023-02-09 08:13:15.170526 gameyamlspiderandgenerator-1.0.0/gameyamlspiderandgenerator/exception.py
--rwxr-xr-x   0        0        0       52 2023-01-22 05:16:08.901166 gameyamlspiderandgenerator-1.0.0/gameyamlspiderandgenerator/hook/__init__.py
--rwxr-xr-x   0        0        0      194 2023-01-22 05:16:08.901422 gameyamlspiderandgenerator-1.0.0/gameyamlspiderandgenerator/hook/_base.py
--rwxr-xr-x   0        0        0     2441 2023-04-13 11:25:54.310342 gameyamlspiderandgenerator-1.0.0/gameyamlspiderandgenerator/hook/search.py
--rwxr-xr-x   0        0        0       56 2023-01-22 05:16:08.902312 gameyamlspiderandgenerator-1.0.0/gameyamlspiderandgenerator/plugin/__init__.py
--rwxr-xr-x   0        0        0     2406 2023-01-22 05:16:08.902831 gameyamlspiderandgenerator-1.0.0/gameyamlspiderandgenerator/plugin/_base.py
--rwxr-xr-x   0        0        0     5469 2023-04-13 11:43:31.880195 gameyamlspiderandgenerator-1.0.0/gameyamlspiderandgenerator/plugin/itchio.py
--rwxr-xr-x   0        0        0     7593 2023-04-13 11:36:38.489756 gameyamlspiderandgenerator-1.0.0/gameyamlspiderandgenerator/plugin/steam.py
--rwxr-xr-x   0        0        0        0 2023-01-22 05:16:08.913666 gameyamlspiderandgenerator-1.0.0/gameyamlspiderandgenerator/util/__init__.py
--rwxr-xr-x   0        0        0      889 2023-04-13 11:25:54.313431 gameyamlspiderandgenerator-1.0.0/gameyamlspiderandgenerator/util/config.py
--rwxr-xr-x   0        0        0      812 2023-01-22 05:16:08.914586 gameyamlspiderandgenerator-1.0.0/gameyamlspiderandgenerator/util/fgi.py
--rwxr-xr-x   0        0        0     1611 2023-04-13 11:36:39.905737 gameyamlspiderandgenerator-1.0.0/gameyamlspiderandgenerator/util/fgi_yaml.py
--rwxr-xr-x   0        0        0     1956 2023-04-13 11:25:54.315122 gameyamlspiderandgenerator-1.0.0/gameyamlspiderandgenerator/util/plugin_manager.py
--rwxr-xr-x   0        0        0     2635 2023-04-13 11:36:40.039218 gameyamlspiderandgenerator-1.0.0/gameyamlspiderandgenerator/util/spider.py
--rwxr-xr-x   0        0        0      617 2023-04-13 11:43:47.612358 gameyamlspiderandgenerator-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1790 1970-01-01 00:00:00.000000 gameyamlspiderandgenerator-1.0.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1069 2023-04-14 04:39:09.582935 gameyamlspiderandgenerator-1.1.0/LICENSE
+-rwxr-xr-x   0        0        0      809 2023-04-14 04:39:09.583123 gameyamlspiderandgenerator-1.1.0/README.md
+-rwxr-xr-x   0        0        0      610 2023-04-14 04:39:09.583410 gameyamlspiderandgenerator-1.1.0/gameyamlspiderandgenerator/__init__.py
+-rwxr-xr-x   0        0        0      980 2023-04-14 04:39:09.583612 gameyamlspiderandgenerator-1.1.0/gameyamlspiderandgenerator/__main__.py
+-rwxr-xr-x   0        0        0      753 2023-04-14 04:39:09.583800 gameyamlspiderandgenerator-1.1.0/gameyamlspiderandgenerator/exception.py
+-rwxr-xr-x   0        0        0       52 2023-04-14 04:39:09.584087 gameyamlspiderandgenerator-1.1.0/gameyamlspiderandgenerator/hook/__init__.py
+-rwxr-xr-x   0        0        0      194 2023-04-14 04:39:09.584282 gameyamlspiderandgenerator-1.1.0/gameyamlspiderandgenerator/hook/_base.py
+-rwxr-xr-x   0        0        0     2365 2023-04-16 02:41:59.202807 gameyamlspiderandgenerator-1.1.0/gameyamlspiderandgenerator/hook/search.py
+-rwxr-xr-x   0        0        0       56 2023-04-14 04:39:09.584827 gameyamlspiderandgenerator-1.1.0/gameyamlspiderandgenerator/plugin/__init__.py
+-rwxr-xr-x   0        0        0     2406 2023-04-14 04:39:09.585063 gameyamlspiderandgenerator-1.1.0/gameyamlspiderandgenerator/plugin/_base.py
+-rwxr-xr-x   0        0        0     6406 2023-04-16 03:52:20.134307 gameyamlspiderandgenerator-1.1.0/gameyamlspiderandgenerator/plugin/itchio.py
+-rwxr-xr-x   0        0        0     7531 2023-04-16 03:03:23.223332 gameyamlspiderandgenerator-1.1.0/gameyamlspiderandgenerator/plugin/steam.py
+-rwxr-xr-x   0        0        0        0 2023-04-14 04:39:09.585883 gameyamlspiderandgenerator-1.1.0/gameyamlspiderandgenerator/util/__init__.py
+-rwxr-xr-x   0        0        0     1026 2023-04-16 02:34:35.477228 gameyamlspiderandgenerator-1.1.0/gameyamlspiderandgenerator/util/config.py
+-rwxr-xr-x   0        0        0     1187 2023-04-16 02:34:35.339573 gameyamlspiderandgenerator-1.1.0/gameyamlspiderandgenerator/util/fgi.py
+-rwxr-xr-x   0        0        0     1706 2023-04-16 02:46:20.126317 gameyamlspiderandgenerator-1.1.0/gameyamlspiderandgenerator/util/fgi_yaml.py
+-rwxr-xr-x   0        0        0     1944 2023-04-16 02:40:43.137333 gameyamlspiderandgenerator-1.1.0/gameyamlspiderandgenerator/util/plugin_manager.py
+-rwxr-xr-x   0        0        0     2611 2023-04-16 02:40:42.901945 gameyamlspiderandgenerator-1.1.0/gameyamlspiderandgenerator/util/spider.py
+-rwxr-xr-x   0        0        0      617 2023-04-16 03:53:49.412367 gameyamlspiderandgenerator-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1790 1970-01-01 00:00:00.000000 gameyamlspiderandgenerator-1.1.0/PKG-INFO
```

### Comparing `gameyamlspiderandgenerator-1.0.0/LICENSE` & `gameyamlspiderandgenerator-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.0.0/README.md` & `gameyamlspiderandgenerator-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.0.0/gameyamlspiderandgenerator/__init__.py` & `gameyamlspiderandgenerator-1.1.0/gameyamlspiderandgenerator/__init__.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.0.0/gameyamlspiderandgenerator/__main__.py` & `gameyamlspiderandgenerator-1.1.0/gameyamlspiderandgenerator/__main__.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.0.0/gameyamlspiderandgenerator/exception.py` & `gameyamlspiderandgenerator-1.1.0/gameyamlspiderandgenerator/exception.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.0.0/gameyamlspiderandgenerator/hook/search.py` & `gameyamlspiderandgenerator-1.1.0/gameyamlspiderandgenerator/hook/search.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from re import sub
-from typing import AnyStr
 from urllib.parse import quote_plus
 
 from bs4 import BeautifulSoup
 from loguru import logger
 
 from ..hook import BaseHook
 from ..util.config import config
 from ..util.spider import get_json, get_text
 
 print(config, type(config))
 
 
 class Search(BaseHook):
     @staticmethod
-    def name_filter(s: AnyStr, rep: AnyStr = ""):
+    def name_filter(s: str, rep: str = ""):
         return sub("[^A-z]", rep, s.lower())
 
     def __init__(self, name: str) -> None:
         logger.info(f"init {name}")
         self.pure = self.name_filter(name)
         self.encode = quote_plus(self.name_filter(name, " "))
 
@@ -59,17 +58,15 @@
 
     def search_all(self) -> list:
         func_list = [
             self.__getattribute__(i)
             for i in (list(filter(lambda x: "__" not in x, self.__dir__())))
         ]
         func_list = filter(
-            lambda x: callable(x)
-                      and x.__name__.startswith("search")
-                      and x.__name__ != "search_all",
+            lambda x: callable(x) and x.__name__.startswith("search") and x.__name__ != "search_all",
             func_list,
         )
         for ii in func_list:
             logger.info(ii.__name__, ii())
         return [ii.__name__ for ii in func_list if ii()]
 
     def setup(self, data: dict):
```

### Comparing `gameyamlspiderandgenerator-1.0.0/gameyamlspiderandgenerator/plugin/_base.py` & `gameyamlspiderandgenerator-1.1.0/gameyamlspiderandgenerator/plugin/_base.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.0.0/gameyamlspiderandgenerator/plugin/itchio.py` & `gameyamlspiderandgenerator-1.1.0/gameyamlspiderandgenerator/plugin/itchio.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import itertools
 import re
 from contextlib import suppress
 from json import loads
 from re import match, sub
-from typing import AnyStr, List
-
 from bs4 import BeautifulSoup
 from html2text import html2text
 from langcodes import find
 
 from ._base import BasePlugin
 from ..util.fgi import fgi_dict
 from ..util.fgi_yaml import YamlData, pss_dedent
@@ -19,15 +17,15 @@
     _VERIFY_PATTERN = re.compile(r"https?://.+\.itch\.io/.+")
 
     @staticmethod
     def remove_query(s: str):
         s = re.sub(r"\?t=\d{6,12}", "", s)
         return s.replace("![]", "![img]")
 
-    def __init__(self, link: AnyStr) -> None:
+    def __init__(self, link: str) -> None:
         self.data_html = get_text(link)
         self.soup = BeautifulSoup(self.data_html, "html.parser")
         self.data = [
             ii
             for ii in [
                 loads(i.text)
                 for i in self.soup.find_all(
@@ -49,18 +47,16 @@
             else None
         )
 
     def get_name(self):
         return self.data["name"]
 
     def get_screenshots(self):
-        return [
-            i.attrs["src"]
-            for i in self.soup.find_all("img", attrs={"class": "screenshot"})
-        ]
+        temp = self.soup.select_one("div.columns > div.right_col.column > div.screenshot_list").select('a')
+        return [i.attrs['href'] for i in temp]
 
     def get_desc(self):
         return pss_dedent(self.remove_query(html2text(
             str(self.soup.select_one("div.formatted_description.user_formatted")),
             bodywidth=0,
         )).strip())
 
@@ -72,19 +68,19 @@
             "Android": "android",
             "HTML5": "web",
             "iOS": "ios",
         }
         platforms = self.more_info["Platforms"][0].split(",")
         return [repl[i.strip()] for i in platforms]
 
-    def get_authors(self) -> List[dict]:
+    def get_authors(self) -> list[dict]:
         temp = self.more_info["Author"]
         return [{"name": i, "role": "developer"} for i in temp]
 
-    def get_tags(self) -> List[str]:
+    def get_tags(self) -> list[str]:
         temp = self.more_info["Genre"] if "Genre" in self.more_info else []
         temp1 = self.more_info["Made with"] if "Made with" in self.more_info else []
         temp2 = self.more_info["Tags"]
         return [i.strip() for i in (temp2 + temp1 + temp)]
 
     def get_misc_tags(self):
         repl = {
@@ -107,21 +103,21 @@
         }
 
         ret = []
         for i, value in repl.items():
             ret.extend(value for ii in self.tag if i in ii)
         return list(set(ret))
 
-    def get_langs(self) -> List[str]:
+    def get_langs(self) -> list[str]:
         temp = self.more_info["Languages"] if "Languages" in self.more_info else ["English"]
         return list(set(find(i).language for i in temp))
 
-    def get_links(self) -> List[dict]:
+    def get_links(self) -> list[dict]:
         link = [i.attrs["href"] for i in self.soup.select("a[href]")]
-        data = list(list(set(link)))
+        data = list(set(link))
         return [
             {"name": p["prefix"], "uri": sub(p["match"], p["replace"], i)}
             for i, p in itertools.product(data, fgi_dict)
             if match(p["match"], i)
         ]
 
     def get_more_info(self):
@@ -161,8 +157,37 @@
             "links": self.get_links(),
             "thumbnail": self.get_thumbnail(),
             "screenshots": self.get_screenshots()  # + self.get_video(),
         }
         return YamlData(ret)
 
     def get_type_tag(self):
-        pass
+        repl = {
+            "Visual Novel": "visual-nove",
+            "Real time strategy": "Real time strategy",
+            "Strategy": "strategy",
+            "Casual": "casual",
+            "Adventure": "adventure",
+            "Board Game": "board",
+            "Action": "action",
+            "Fantasy": "fantasy",
+            "Fighting": "fighting",
+            "Music": "music",
+            "Shooter": "shooter",
+            "Puzzle": "puzzle",
+            "RPG": "role-playing",
+            "MMORPG": "mmorpg",
+            "Dating Sim": "dating-sim",
+            "Roguelike": "roguelike",
+            "Sports": "Sports",
+            "Bara": "bara",
+            "Yuri": "yuri",
+            "Gore": "gore",
+            "Comedy": "comedy",
+            "tragedy": "tragedy",
+            "Horror": "horror"
+        }
+
+        ret = []
+        for i, value in repl.items():
+            ret.extend(value for ii in self.tag if i in ii)
+        return list(set(ret))
```

### Comparing `gameyamlspiderandgenerator-1.0.0/gameyamlspiderandgenerator/plugin/steam.py` & `gameyamlspiderandgenerator-1.1.0/gameyamlspiderandgenerator/plugin/steam.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import re
-from typing import AnyStr, List, SupportsInt
 from urllib.parse import parse_qs, urlparse
 
 from bs4 import BeautifulSoup
 from html2text import html2text
 from langcodes import find
 
 from ._base import BasePlugin
@@ -12,26 +11,26 @@
 from ..util.spider import get_json, get_text
 
 
 class Steam(BasePlugin):
     _VERIFY_PATTERN = re.compile(r"https?://store\.steampowered\.com/app/\d+/.+/?.+")
 
     @staticmethod
-    def get_steam_id(link: AnyStr) -> SupportsInt:
+    def get_steam_id(link: str) -> int:
         return int(urlparse(link).path.split("/")[2])
 
     def get_name(self):
         return self.data[str(self.id)]["data"]["name"]
 
     @staticmethod
     def remove_query(s: str):
         s = re.sub(r"\?t=\d{6,12}", "", s)
         return s.replace("![]", "![img]")
 
-    def __init__(self, link: AnyStr) -> None:
+    def __init__(self, link: str) -> None:
         self.id = self.get_steam_id(link)
         self.data = get_json(
             f"https://store.steampowered.com/api/appdetails?appids={self.id}&cc=us&l=english"
         )
         self.data_html = get_text(link)
         self.soup = BeautifulSoup(self.data_html, "html.parser")
         self.name = self.get_name()
@@ -53,15 +52,15 @@
             },
             "links": self.get_links(),
             "thumbnail": self.get_thumbnail(),
             "screenshots": self.get_screenshots() + self.get_video(),  # type: ignore
         }
         return YamlData(ret)
 
-    def get_langs(self) -> List[str]:
+    def get_langs(self) -> list[str]:
         temp = self.data[str(self.id)]["data"]["supported_languages"].split(",")
         return list({find(i).language for i in temp})
 
     def get_desc(self):
         return pss_dedent(
             self.remove_query(
                 (
@@ -74,15 +73,15 @@
         )
 
     def get_brief_desc(self):
         return pss_dedent(
             html2text(self.data[str(self.id)]["data"]["short_description"], bodywidth=0)
         )
 
-    def get_authors(self) -> List[dict]:
+    def get_authors(self) -> list[dict]:
         temp = self.data[str(self.id)]["data"]
         developers = [{"name": i, "role": "developer"} for i in temp["developers"]]
         publishers = [{"name": i, "role": "publisher"} for i in temp["publishers"]]
         return developers + publishers
 
     def get_platforms(self):
         temp = self.data[str(self.id)]["data"]["platforms"]
@@ -113,15 +112,15 @@
         }
 
         ret = []
         for i, value in repl.items():
             ret.extend(value for ii in self.tag if i in ii)
         return list(set(ret))
 
-    def get_tags(self) -> List[dict]:
+    def get_tags(self) -> list[dict]:
         pass
 
     def get_misc_tags(self):
         repl = {
             "3D": "3d",
             "Pixel": "pixel-art",
             "Multiplayer": "multiplayer",
@@ -177,16 +176,16 @@
                     {"mime": "video/webm", "uri": video_webm[i]},
                     {"mime": "video/mp4", "uri": video_mp4[i]},
                 ],
             }
             for i in range(len(video_webm))
         ]
 
-    def get_links(self) -> List[dict]:
-        def remove_query_string(x: AnyStr):
+    def get_links(self) -> list[dict]:
+        def remove_query_string(x: str):
             return parse_qs(urlparse(x).query)["url"][0] if "linkfilter" in x else x  # type: ignore
 
         temp1 = self.soup.body.find(
             "div",
             attrs={"id": "game_area_description", "class": "game_area_description"},
         )
         temp3 = self.soup.body.find("div", attrs={"style": "padding-top: 14px;"})
```

### Comparing `gameyamlspiderandgenerator-1.0.0/gameyamlspiderandgenerator/util/fgi_yaml.py` & `gameyamlspiderandgenerator-1.1.0/gameyamlspiderandgenerator/util/fgi_yaml.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,18 +40,20 @@
 class YamlData:
     raw_dict: dict
 
     def __init__(self, raw_data: dict):
         self.raw_dict = raw_data
 
     def __str__(self):
-        return dump_to_yaml(self.raw_dict)
+        return dump_to_yaml({**self.raw_dict, "thumbnail": 'thumbnail.png'})
 
     def __bytes__(self):
         from ..util.spider import get_bytes
         _io = BytesIO()
         img = get_bytes(self.raw_dict["thumbnail"])
         zip_data = zipfile.ZipFile(_io, 'w', zipfile.ZIP_STORED)
         zip_data.writestr('thumbnail.png', process_thumbnail(img))
-        zip_data.writestr(self.raw_dict['name'] + ".yaml", dump_to_yaml(self.raw_dict))
+
+        zip_data.writestr(self.raw_dict['name'] + ".yaml",
+                          dump_to_yaml({**self.raw_dict, "thumbnail": 'thumbnail.png'}))
         zip_data.close()
         return _io.getvalue()
```

### Comparing `gameyamlspiderandgenerator-1.0.0/gameyamlspiderandgenerator/util/plugin_manager.py` & `gameyamlspiderandgenerator-1.1.0/gameyamlspiderandgenerator/util/plugin_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import importlib
-from typing import Dict, Literal, Type, Union, List
+from typing import Literal, Type, Union
 
 from loguru import logger
 
 from ..hook import BaseHook
 from ..plugin import BasePlugin
 from ..util.config import config
 
 
 class Package:
-    plugin: Dict[str, BasePlugin] = {}
-    hook: Dict[str, BaseHook] = {}
-    log: List[str] = []
+    plugin: dict[str, BasePlugin] = {}
+    hook: dict[str, BaseHook] = {}
+    log: list[str] = []
 
     def __init__(self):
         self.load_plugins()
         self.load_hooks()
 
     def __getitem__(self, item):
         # Compatibility with the old version
```

### Comparing `gameyamlspiderandgenerator-1.0.0/gameyamlspiderandgenerator/util/spider.py` & `gameyamlspiderandgenerator-1.1.0/gameyamlspiderandgenerator/util/spider.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from typing import Dict
 
 import requests
 from requests import JSONDecodeError
 
 from ..exception import (
     CommunicateWithServerFailed,
     InvalidResponse,
@@ -89,15 +88,15 @@
         return self.response.status_code
 
     @property
     def bytes(self):
         return self.response.content
 
 
-def get_json(url: str) -> Dict:
+def get_json(url: str) -> dict:
     with GetResponse(url) as resp:
         return resp.json
 
 
 def get_text(url: str) -> str:
     with GetResponse(url) as resp:
         return resp.text
```

### Comparing `gameyamlspiderandgenerator-1.0.0/pyproject.toml` & `gameyamlspiderandgenerator-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gameyamlspiderandgenerator"
-version = "1.0.0"
+version = "1.1.0"
 description = ""
 authors = ["kaesinol"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `gameyamlspiderandgenerator-1.0.0/PKG-INFO` & `gameyamlspiderandgenerator-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gameyamlspiderandgenerator
-Version: 1.0.0
+Version: 1.1.0
 Summary: 
 License: MIT
 Author: kaesinol
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

