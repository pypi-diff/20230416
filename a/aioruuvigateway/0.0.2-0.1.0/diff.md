# Comparing `tmp/aioruuvigateway-0.0.2.tar.gz` & `tmp/aioruuvigateway-0.1.0.tar.gz`

## Comparing `aioruuvigateway-0.0.2.tar` & `aioruuvigateway-0.1.0.tar`

### file list

```diff
@@ -1,29 +1,28 @@
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 aioruuvigateway-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 aioruuvigateway-0.0.2/setup.cfg
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 aioruuvigateway-0.0.2/.github/workflows/build.yml
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 aioruuvigateway-0.0.2/.github/workflows/pre-commit.yml
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 aioruuvigateway-0.0.2/.github/workflows/test.yml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 aioruuvigateway-0.0.2/.idea/.gitignore
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 aioruuvigateway-0.0.2/.idea/aioruuvigateway.iml
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 aioruuvigateway-0.0.2/.idea/encodings.xml
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 aioruuvigateway-0.0.2/.idea/misc.xml
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 aioruuvigateway-0.0.2/.idea/modules.xml
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 aioruuvigateway-0.0.2/.idea/vcs.xml
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 aioruuvigateway-0.0.2/.idea/workspace.xml
--rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 aioruuvigateway-0.0.2/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 aioruuvigateway-0.0.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 aioruuvigateway-0.0.2/aioruuvigateway/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aioruuvigateway-0.0.2/aioruuvigateway/__init__.py
--rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 aioruuvigateway-0.0.2/aioruuvigateway/__main__.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 aioruuvigateway-0.0.2/aioruuvigateway/api.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 aioruuvigateway-0.0.2/aioruuvigateway/excs.py
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 aioruuvigateway-0.0.2/aioruuvigateway/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aioruuvigateway-0.0.2/aioruuvigateway/py.typed
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 aioruuvigateway-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 aioruuvigateway-0.0.2/tests/example.json
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 aioruuvigateway-0.0.2/tests/test_library.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 aioruuvigateway-0.0.2/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 aioruuvigateway-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 aioruuvigateway-0.0.2/README.md
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 aioruuvigateway-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 aioruuvigateway-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 aioruuvigateway-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 aioruuvigateway-0.1.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 aioruuvigateway-0.1.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 aioruuvigateway-0.1.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 aioruuvigateway-0.1.0/.idea/.gitignore
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 aioruuvigateway-0.1.0/.idea/aioruuvigateway.iml
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 aioruuvigateway-0.1.0/.idea/encodings.xml
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 aioruuvigateway-0.1.0/.idea/misc.xml
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 aioruuvigateway-0.1.0/.idea/modules.xml
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 aioruuvigateway-0.1.0/.idea/vcs.xml
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 aioruuvigateway-0.1.0/.idea/workspace.xml
+-rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 aioruuvigateway-0.1.0/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 aioruuvigateway-0.1.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 aioruuvigateway-0.1.0/aioruuvigateway/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aioruuvigateway-0.1.0/aioruuvigateway/__init__.py
+-rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 aioruuvigateway-0.1.0/aioruuvigateway/__main__.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 aioruuvigateway-0.1.0/aioruuvigateway/api.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 aioruuvigateway-0.1.0/aioruuvigateway/excs.py
+-rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 aioruuvigateway-0.1.0/aioruuvigateway/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aioruuvigateway-0.1.0/aioruuvigateway/py.typed
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 aioruuvigateway-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 aioruuvigateway-0.1.0/tests/example.json
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 aioruuvigateway-0.1.0/tests/test_library.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 aioruuvigateway-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 aioruuvigateway-0.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 aioruuvigateway-0.1.0/README.md
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 aioruuvigateway-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 aioruuvigateway-0.1.0/PKG-INFO
```

### Comparing `aioruuvigateway-0.0.2/.github/workflows/test.yml` & `aioruuvigateway-0.1.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `aioruuvigateway-0.0.2/.idea/workspace.xml` & `aioruuvigateway-0.1.0/.idea/workspace.xml`

 * *Files 4% similar despite different names*

#### Comparing `aioruuvigateway-0.0.2/.idea/workspace.xml` & `aioruuvigateway-0.1.0/.idea/workspace.xml`

```diff
@@ -1,9 +1,12 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
+  <component name="AutoImportSettings">
+    <option name="autoReloadType" value="SELECTIVE"/>
+  </component>
   <component name="ChangeListManager">
     <list default="true" id="7644242b-eab8-4a37-99a7-f5ecda1aa54f" name="Changes" comment="">
       <change beforePath="$PROJECT_DIR$/.github/workflows/test.yml" beforeDir="false" afterPath="$PROJECT_DIR$/.github/workflows/test.yml" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/aioruuvigateway/models.py" beforeDir="false" afterPath="$PROJECT_DIR$/aioruuvigateway/models.py" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
@@ -23,28 +26,30 @@
   </component>
   <component name="PropertiesComponent"><![CDATA[{
   "keyToString": {
     "RunOnceActivity.OpenProjectViewOnStart": "true",
     "RunOnceActivity.ShowReadmeOnStart": "true",
     "WebServerToolWindowFactoryState": "false",
     "node.js.detected.package.eslint": "true",
+    "node.js.detected.package.tslint": "true",
     "node.js.selected.package.eslint": "(autodetect)",
+    "node.js.selected.package.tslint": "(autodetect)",
     "nodejs_package_manager_path": "npm",
     "vue.rearranger.settings.migration": "true"
   }
 }]]></component>
   <component name="SpellCheckerSettings" RuntimeDictionaries="0" Folders="0" CustomDictionaries="0" DefaultDictionary="application-level" UseSingleDictionary="true" transferred="true"/>
   <component name="TaskManager">
     <task active="true" id="Default" summary="Default task">
       <changelist id="7644242b-eab8-4a37-99a7-f5ecda1aa54f" name="Changes" comment=""/>
       <created>1672535772919</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1672535772919</updated>
-      <workItem from="1672535777826" duration="26000"/>
+      <workItem from="1672535777826" duration="537000"/>
     </task>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
 </project>
```

### Comparing `aioruuvigateway-0.0.2/.idea/inspectionProfiles/Project_Default.xml` & `aioruuvigateway-0.1.0/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `aioruuvigateway-0.0.2/aioruuvigateway/__main__.py` & `aioruuvigateway-0.1.0/aioruuvigateway/__main__.py`

 * *Files identical despite different names*

### Comparing `aioruuvigateway-0.0.2/aioruuvigateway/api.py` & `aioruuvigateway-0.1.0/aioruuvigateway/api.py`

 * *Files identical despite different names*

### Comparing `aioruuvigateway-0.0.2/aioruuvigateway/models.py` & `aioruuvigateway-0.1.0/aioruuvigateway/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,25 +16,36 @@
 
 @dataclasses.dataclass()
 class TagData(TimestampConversionMixin):
     mac: str  # AA:BB:CC:DD:EE:FF
     rssi: int
     timestamp: int
     data: bytes
+    age_seconds: int | None = None
 
     def parse_announcement(self) -> BLEGAPAdvertisement:
         return parse_advertisement_data([self.data])
 
     @classmethod
-    def from_gateway_history_json_tag(cls, mac: str, data: dict) -> TagData:
+    def from_gateway_history_json_tag(
+        cls,
+        mac: str,
+        data: dict,
+        response_timestamp: int | None,
+    ) -> TagData:
+        tag_timestamp = int(data["timestamp"])
+        age_seconds = (
+            (response_timestamp - tag_timestamp) if response_timestamp else None
+        )
         return cls(
             mac=mac,
             rssi=int(data["rssi"]),
-            timestamp=int(data["timestamp"]),
+            timestamp=tag_timestamp,
             data=bytes.fromhex(data["data"]),
+            age_seconds=age_seconds,
         )
 
 
 @dataclasses.dataclass()
 class HistoryResponse(TimestampConversionMixin):
     timestamp: int
     gw_mac: str
@@ -44,17 +55,22 @@
     @property
     def gw_mac_suffix(self) -> str:
         return self.gw_mac[-5:].upper()
 
     @classmethod
     def from_gateway_history_json(cls, data: dict) -> HistoryResponse:
         data = data["data"]
+        response_timestamp = int(data["timestamp"])
         tags = [
-            TagData.from_gateway_history_json_tag(mac=mac, data=tag_data)
+            TagData.from_gateway_history_json_tag(
+                mac=mac,
+                data=tag_data,
+                response_timestamp=response_timestamp,
+            )
             for mac, tag_data in data.get("tags", {}).items()
         ]
         return HistoryResponse(
-            timestamp=int(data["timestamp"]),
+            timestamp=response_timestamp,
             gw_mac=data["gw_mac"],
             coordinates=data.get("coordinates", ""),
             tags=tags,
         )
```

### Comparing `aioruuvigateway-0.0.2/tests/example.json` & `aioruuvigateway-0.1.0/tests/example.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9875%*

 * *Differences: {"'data'": "{'tags': {'E0:50:40:30:20:A0': OrderedDict([('rssi', -87), ('timestamp', "*

 * *           "'1672395002'), ('data', '07FF4C0012020000')])}}"}*

```diff
@@ -18,12 +18,17 @@
                 "rssi": -59,
                 "timestamp": "1672395020"
             },
             "BB:BB:BB:BB:CA:08": {
                 "data": "0201061BFF9904050F4845C0C0EC03200284FFBC9976876268BBBBBBBBCA08",
                 "rssi": -65,
                 "timestamp": "1672395021"
+            },
+            "E0:50:40:30:20:A0": {
+                "data": "07FF4C0012020000",
+                "rssi": -87,
+                "timestamp": "1672395002"
             }
         },
         "timestamp": "1672395021"
     }
 }
```

### Comparing `aioruuvigateway-0.0.2/tests/test_library.py` & `aioruuvigateway-0.1.0/tests/test_library.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,21 +23,22 @@
             host="192.168.1.202",
             bearer_token="bear, a scary bear",
         )
     assert history.gw_mac_suffix == "EE:FF"
     manufacturers = Counter()
     for tag in history.tags:
         assert tag.datetime.year == 2022
+        assert tag.age_seconds in {0, 1, 19}
         ann = tag.parse_announcement()
-        print(ann)
+        print(tag, ann)
         manufacturers.update(ann.manufacturer_data.keys())
     assert manufacturers == {
         0x0499: 2,  # Two Ruuvitags
         0x012D: 1,  # One Sony
-        0x004C: 1,  # One Apple
+        0x004C: 2,  # Two Apples
     }
 
 
 @pytest.mark.asyncio
 async def test_auth(httpx_mock):
     httpx_mock.add_response(
         url="http://192.168.1.202/history",
```

### Comparing `aioruuvigateway-0.0.2/LICENSE.txt` & `aioruuvigateway-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aioruuvigateway-0.0.2/README.md` & `aioruuvigateway-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `aioruuvigateway-0.0.2/pyproject.toml` & `aioruuvigateway-0.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -20,23 +20,23 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
-  "bluetooth-data-tools~=0.3.1",
+  "bluetooth-data-tools>=0.3.1",
   "httpx>=0.23.0",
 ]
 dynamic = ["version"]
 
 [project.urls]
-Documentation = "https://github.com/unknown/aioruuvigateway#readme"
-Issues = "https://github.com/unknown/aioruuvigateway/issues"
-Source = "https://github.com/unknown/aioruuvigateway"
+Documentation = "https://github.com/akx/aioruuvigateway#readme"
+Issues = "https://github.com/akx/aioruuvigateway/issues"
+Source = "https://github.com/akx/aioruuvigateway"
 
 [tool.hatch.version]
 path = "aioruuvigateway/__about__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
   "pytest",
@@ -62,7 +62,26 @@
 [tool.coverage.report]
 exclude_lines = [
   "no cov",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
   "raise NotImplementedError",
 ]
+
+[tool.ruff]
+target-version = "py37"
+ignore = ["SIM105"]
+line-length = 88
+select = [
+    "C9",
+    "E",
+    "F",
+    "SIM",
+    "TID",
+    "W",
+]
+
+[tool.ruff.mccabe]
+max-complexity = 10
+
+[tool.ruff.flake8-tidy-imports]
+ban-relative-imports = "all"
```

### Comparing `aioruuvigateway-0.0.2/PKG-INFO` & `aioruuvigateway-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: aioruuvigateway
-Version: 0.0.2
-Project-URL: Documentation, https://github.com/unknown/aioruuvigateway#readme
-Project-URL: Issues, https://github.com/unknown/aioruuvigateway/issues
-Project-URL: Source, https://github.com/unknown/aioruuvigateway
+Version: 0.1.0
+Project-URL: Documentation, https://github.com/akx/aioruuvigateway#readme
+Project-URL: Issues, https://github.com/akx/aioruuvigateway/issues
+Project-URL: Source, https://github.com/akx/aioruuvigateway
 Author-email: Aarni Koskela <akx@iki.fi>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
-Requires-Dist: bluetooth-data-tools~=0.3.1
+Requires-Dist: bluetooth-data-tools>=0.3.1
 Requires-Dist: httpx>=0.23.0
 Description-Content-Type: text/markdown
 
 # aioruuvigateway
 
 An asyncio-native library for requesting data from a Ruuvi Gateway.
```

