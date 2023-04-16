# Comparing `tmp/mypyllant-0.2.1.tar.gz` & `tmp/mypyllant-0.2.2.tar.gz`

## Comparing `mypyllant-0.2.1.tar` & `mypyllant-0.2.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 mypyllant-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0    45426 2020-02-02 00:00:00.000000 mypyllant-0.2.1/logo.png
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 mypyllant-0.2.1/requirements-dev.txt
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 mypyllant-0.2.1/setup.cfg
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 mypyllant-0.2.1/.github/workflows/build-test.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.2.1/src/myPyllant/__init__.py
--rw-r--r--   0        0        0    15560 2020-02-02 00:00:00.000000 mypyllant-0.2.1/src/myPyllant/api.py
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 mypyllant-0.2.1/src/myPyllant/const.py
--rwxr-xr-x   0        0        0     2672 2020-02-02 00:00:00.000000 mypyllant-0.2.1/src/myPyllant/export.py
--rw-r--r--   0        0        0     7731 2020-02-02 00:00:00.000000 mypyllant-0.2.1/src/myPyllant/models.py
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 mypyllant-0.2.1/src/myPyllant/sample.py
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 mypyllant-0.2.1/src/myPyllant/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.2.1/tests/__init__.py
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 mypyllant-0.2.1/tests/conftest.py
--rwxr-xr-x   0        0        0      784 2020-02-02 00:00:00.000000 mypyllant-0.2.1/tests/find_countries.py
--rw-r--r--   0        0        0     4727 2020-02-02 00:00:00.000000 mypyllant-0.2.1/tests/generate_test_data.py
--rw-r--r--   0        0        0     3484 2020-02-02 00:00:00.000000 mypyllant-0.2.1/tests/test_api.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 mypyllant-0.2.1/tests/test_countries.py
--rw-r--r--   0        0        0     4866 2020-02-02 00:00:00.000000 mypyllant-0.2.1/tests/test_generate_test_data.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 mypyllant-0.2.1/tests/json/064876fe84e6a872c97ac79ba1c2a7c71ff974ca/current_system.json
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 mypyllant-0.2.1/tests/json/064876fe84e6a872c97ac79ba1c2a7c71ff974ca/device_buckets.json
--rw-r--r--   0        0        0     6159 2020-02-02 00:00:00.000000 mypyllant-0.2.1/tests/json/064876fe84e6a872c97ac79ba1c2a7c71ff974ca/systems.json
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 mypyllant-0.2.1/tests/json/1cb8b8ad6bbd158eaca1527b3d5f852b8b473c0c/current_system.json
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 mypyllant-0.2.1/tests/json/1cb8b8ad6bbd158eaca1527b3d5f852b8b473c0c/device_buckets.json
--rw-r--r--   0        0        0     6354 2020-02-02 00:00:00.000000 mypyllant-0.2.1/tests/json/1cb8b8ad6bbd158eaca1527b3d5f852b8b473c0c/systems.json
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 mypyllant-0.2.1/tests/json/d121ac4dd73851053d557b1f8b6126bb1bf71a25/current_system.json
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 mypyllant-0.2.1/tests/json/d121ac4dd73851053d557b1f8b6126bb1bf71a25/device_buckets.json
--rw-r--r--   0        0        0     6400 2020-02-02 00:00:00.000000 mypyllant-0.2.1/tests/json/d121ac4dd73851053d557b1f8b6126bb1bf71a25/systems.json
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 mypyllant-0.2.1/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 mypyllant-0.2.1/LICENSE
--rw-r--r--   0        0        0     4404 2020-02-02 00:00:00.000000 mypyllant-0.2.1/README.md
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 mypyllant-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     5010 2020-02-02 00:00:00.000000 mypyllant-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 mypyllant-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    45426 2020-02-02 00:00:00.000000 mypyllant-0.2.2/logo.png
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 mypyllant-0.2.2/requirements-dev.txt
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 mypyllant-0.2.2/setup.cfg
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 mypyllant-0.2.2/.github/workflows/build-test.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.2.2/src/myPyllant/__init__.py
+-rw-r--r--   0        0        0    15667 2020-02-02 00:00:00.000000 mypyllant-0.2.2/src/myPyllant/api.py
+-rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 mypyllant-0.2.2/src/myPyllant/const.py
+-rwxr-xr-x   0        0        0     2687 2020-02-02 00:00:00.000000 mypyllant-0.2.2/src/myPyllant/export.py
+-rw-r--r--   0        0        0     7731 2020-02-02 00:00:00.000000 mypyllant-0.2.2/src/myPyllant/models.py
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 mypyllant-0.2.2/src/myPyllant/sample.py
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 mypyllant-0.2.2/src/myPyllant/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.2.2/tests/__init__.py
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 mypyllant-0.2.2/tests/conftest.py
+-rwxr-xr-x   0        0        0     1060 2020-02-02 00:00:00.000000 mypyllant-0.2.2/tests/find_countries.py
+-rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 mypyllant-0.2.2/tests/generate_test_data.py
+-rw-r--r--   0        0        0     3484 2020-02-02 00:00:00.000000 mypyllant-0.2.2/tests/test_api.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 mypyllant-0.2.2/tests/test_countries.py
+-rw-r--r--   0        0        0     4866 2020-02-02 00:00:00.000000 mypyllant-0.2.2/tests/test_generate_test_data.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 mypyllant-0.2.2/tests/json/064876fe84e6a872c97ac79ba1c2a7c71ff974ca/current_system.json
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 mypyllant-0.2.2/tests/json/064876fe84e6a872c97ac79ba1c2a7c71ff974ca/device_buckets.json
+-rw-r--r--   0        0        0     6159 2020-02-02 00:00:00.000000 mypyllant-0.2.2/tests/json/064876fe84e6a872c97ac79ba1c2a7c71ff974ca/systems.json
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 mypyllant-0.2.2/tests/json/1cb8b8ad6bbd158eaca1527b3d5f852b8b473c0c/current_system.json
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 mypyllant-0.2.2/tests/json/1cb8b8ad6bbd158eaca1527b3d5f852b8b473c0c/device_buckets.json
+-rw-r--r--   0        0        0     6354 2020-02-02 00:00:00.000000 mypyllant-0.2.2/tests/json/1cb8b8ad6bbd158eaca1527b3d5f852b8b473c0c/systems.json
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 mypyllant-0.2.2/tests/json/d121ac4dd73851053d557b1f8b6126bb1bf71a25/current_system.json
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 mypyllant-0.2.2/tests/json/d121ac4dd73851053d557b1f8b6126bb1bf71a25/device_buckets.json
+-rw-r--r--   0        0        0     6400 2020-02-02 00:00:00.000000 mypyllant-0.2.2/tests/json/d121ac4dd73851053d557b1f8b6126bb1bf71a25/systems.json
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 mypyllant-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 mypyllant-0.2.2/LICENSE
+-rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 mypyllant-0.2.2/README.md
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 mypyllant-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     5223 2020-02-02 00:00:00.000000 mypyllant-0.2.2/PKG-INFO
```

### Comparing `mypyllant-0.2.1/.pre-commit-config.yaml` & `mypyllant-0.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.1/logo.png` & `mypyllant-0.2.2/logo.png`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.1/setup.cfg` & `mypyllant-0.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.1/.github/workflows/build-test.yaml` & `mypyllant-0.2.2/.github/workflows/build-test.yaml`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.1/src/myPyllant/api.py` & `mypyllant-0.2.2/src/myPyllant/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,18 +62,22 @@
     username: str = None
     password: str = None
     aiohttp_session: aiohttp.ClientSession = None
     oauth_session: dict = {}
     oauth_session_expires: datetime.datetime | None = None
 
     def __init__(self, username: str, password: str, country: str, brand: str) -> None:
-        if country not in COUNTRIES.keys():
-            raise ValueError(f"Country must be one of {', '.join(COUNTRIES.keys())}")
         if brand not in BRANDS.keys():
-            raise ValueError(f"Brand must be one of {', '.join(BRANDS.keys())}")
+            raise ValueError(
+                f"Invalid brand, must be one of {', '.join(BRANDS.keys())}"
+            )
+        if country not in COUNTRIES[brand].keys():
+            raise ValueError(
+                f"Invalid country, {BRANDS[brand]} only supports {', '.join(COUNTRIES[brand].keys())}"
+            )
         self.username = username
         self.password = password
         self.country = country
         self.brand = brand
         trace_config = aiohttp.TraceConfig()
         trace_config.on_request_start.append(on_request_start)
         trace_config.on_request_end.append(on_request_end)
```

### Comparing `mypyllant-0.2.1/src/myPyllant/const.py` & `mypyllant-0.2.2/src/myPyllant/const.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,36 +7,53 @@
 )
 BRANDS = {
     "vaillant": "Vaillant",
     "sdbg": "Saunier Duval",
 }
 DEFAULT_BRAND = "vaillant"
 COUNTRIES = {
-    "austria": "Austria",
-    "belgium": "Belgium",
-    "bulgaria": "Bulgaria",
-    "croatia": "Croatia",
-    "czechrepublic": "Czechia",
-    "denmark": "Denmark",
-    "estonia": "Estonia",
-    "finland": "Finland",
-    "france": "France",
-    "germany": "Germany",
-    "greece": "Greece",
-    "hungary": "Hungary",
-    "italy": "Italy",
-    "latvia": "Latvia",
-    "lithuania": "Lithuania",
-    "netherlands": "Netherlands",
-    "norway": "Norway",
-    "poland": "Poland",
-    "portugal": "Portugal",
-    "romania": "Romania",
-    "serbia": "Serbia",
-    "slovakia": "Slovakia",
-    "slovenia": "Slovenia",
-    "spain": "Spain",
-    "sweden": "Sweden",
-    "switzerland": "Switzerland",
-    "unitedkingdom": "United Kingdom",
+    "vaillant": {
+        "austria": "Austria",
+        "belgium": "Belgium",
+        "bulgaria": "Bulgaria",
+        "croatia": "Croatia",
+        "czechrepublic": "Czechia",
+        "denmark": "Denmark",
+        "estonia": "Estonia",
+        "finland": "Finland",
+        "france": "France",
+        "germany": "Germany",
+        "greece": "Greece",
+        "hungary": "Hungary",
+        "italy": "Italy",
+        "latvia": "Latvia",
+        "lithuania": "Lithuania",
+        "netherlands": "Netherlands",
+        "norway": "Norway",
+        "poland": "Poland",
+        "portugal": "Portugal",
+        "romania": "Romania",
+        "serbia": "Serbia",
+        "slovakia": "Slovakia",
+        "slovenia": "Slovenia",
+        "spain": "Spain",
+        "sweden": "Sweden",
+        "switzerland": "Switzerland",
+        "unitedkingdom": "United Kingdom",
+    },
+    "sdbg": {
+        "austria": "Austria",
+        "czechrepublic": "Czechia",
+        "finland": "Finland",
+        "france": "France",
+        "greece": "Greece",
+        "hungary": "Hungary",
+        "italy": "Italy",
+        "lithuania": "Lithuania",
+        "poland": "Poland",
+        "portugal": "Portugal",
+        "romania": "Romania",
+        "slovakia": "Slovakia",
+        "spain": "Spain",
+    },
 }
 DEFAULT_QUICK_VETO_DURATION = 3
```

### Comparing `mypyllant-0.2.1/src/myPyllant/export.py` & `mypyllant-0.2.2/src/myPyllant/export.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 parser = argparse.ArgumentParser(description="Export data from myVaillant API.")
 parser.add_argument("user", help="Username (email address) for the myVaillant app")
 parser.add_argument("password", help="Password for the myVaillant app")
 parser.add_argument(
     "country",
     help="Country your account is registered in, i.e. 'germany'",
-    choices=COUNTRIES.keys(),
+    choices=COUNTRIES[DEFAULT_BRAND].keys(),
 )
 parser.add_argument(
     "brand",
     help="Brand your account is registered in, i.e. 'vaillant'",
     default=DEFAULT_BRAND,
     choices=BRANDS.keys(),
 )
```

### Comparing `mypyllant-0.2.1/src/myPyllant/models.py` & `mypyllant-0.2.2/src/myPyllant/models.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.1/src/myPyllant/sample.py` & `mypyllant-0.2.2/src/myPyllant/sample.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 import argparse
 import asyncio
 from datetime import datetime, timedelta
 
-from custom_components.mypyllant.const import COUNTRIES
-
 from myPyllant.api import MyPyllantAPI
+from myPyllant.const import BRANDS, COUNTRIES, DEFAULT_BRAND
 
 parser = argparse.ArgumentParser(description="Export data from myVaillant API   .")
 parser.add_argument("user", help="Username (email address) for the myVaillant app")
 parser.add_argument("password", help="Password for the myVaillant app")
 parser.add_argument(
     "country",
     help="Country your account is registered in, i.e. 'germany'",
-    choices=COUNTRIES.keys(),
+    choices=COUNTRIES[DEFAULT_BRAND].keys(),
+)
+parser.add_argument(
+    "brand",
+    help="Brand your account is registered in, i.e. 'vaillant'",
+    default=DEFAULT_BRAND,
+    choices=BRANDS.keys(),
 )
 
 
-async def main(user, password, country):
-    async with MyPyllantAPI(user, password, country) as api:
+async def main(user, password, country, brand):
+    async with MyPyllantAPI(user, password, country, brand) as api:
         async for system in api.get_systems():
             print(await api.set_holiday(system, datetime.now()))
             print(
                 await (
                     await api.set_holiday(
                         system, datetime.now(), datetime.now() + timedelta(days=1)
                     )
@@ -38,8 +43,8 @@
             print(await api.set_set_back_temperature(system.zones[0], 15.5))
             print(await api.quick_veto_zone_temperature(system.zones[0], 21, 5))
             print(await api.cancel_quick_veto_zone_temperature(system.zones[0]))
 
 
 if __name__ == "__main__":
     args = parser.parse_args()
-    asyncio.run(main(args.user, args.password, args.country))
+    asyncio.run(main(args.user, args.password, args.country, args.brand))
```

### Comparing `mypyllant-0.2.1/src/myPyllant/utils.py` & `mypyllant-0.2.2/src/myPyllant/utils.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.1/tests/conftest.py` & `mypyllant-0.2.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.1/tests/generate_test_data.py` & `mypyllant-0.2.2/tests/generate_test_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     description="Generates test data necessary to run integration tests."
 )
 parser.add_argument("user", help="Username (email address) for the myVaillant app")
 parser.add_argument("password", help="Password for the myVaillant app")
 parser.add_argument(
     "country",
     help="Country your account is registered in, i.e. 'germany'",
-    choices=COUNTRIES.keys(),
+    choices=COUNTRIES[DEFAULT_BRAND].keys(),
 )
 parser.add_argument(
     "brand",
     help="Brand your account is registered in, i.e. 'vaillant'",
     default=DEFAULT_BRAND,
     choices=BRANDS.keys(),
 )
```

### Comparing `mypyllant-0.2.1/tests/test_api.py` & `mypyllant-0.2.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.1/tests/test_generate_test_data.py` & `mypyllant-0.2.2/tests/test_generate_test_data.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.1/tests/json/064876fe84e6a872c97ac79ba1c2a7c71ff974ca/current_system.json` & `mypyllant-0.2.2/tests/json/064876fe84e6a872c97ac79ba1c2a7c71ff974ca/current_system.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.1/tests/json/064876fe84e6a872c97ac79ba1c2a7c71ff974ca/systems.json` & `mypyllant-0.2.2/tests/json/064876fe84e6a872c97ac79ba1c2a7c71ff974ca/systems.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.1/tests/json/1cb8b8ad6bbd158eaca1527b3d5f852b8b473c0c/current_system.json` & `mypyllant-0.2.2/tests/json/1cb8b8ad6bbd158eaca1527b3d5f852b8b473c0c/current_system.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.1/tests/json/1cb8b8ad6bbd158eaca1527b3d5f852b8b473c0c/systems.json` & `mypyllant-0.2.2/tests/json/1cb8b8ad6bbd158eaca1527b3d5f852b8b473c0c/systems.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.1/tests/json/d121ac4dd73851053d557b1f8b6126bb1bf71a25/current_system.json` & `mypyllant-0.2.2/tests/json/d121ac4dd73851053d557b1f8b6126bb1bf71a25/current_system.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.1/tests/json/d121ac4dd73851053d557b1f8b6126bb1bf71a25/systems.json` & `mypyllant-0.2.2/tests/json/d121ac4dd73851053d557b1f8b6126bb1bf71a25/systems.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.1/.gitignore` & `mypyllant-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.1/LICENSE` & `mypyllant-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.1/README.md` & `mypyllant-0.2.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,56 +1,61 @@
 # myPyllant
 
 [![PyPI](https://img.shields.io/pypi/v/myPyllant)](https://pypi.org/project/myPyllant/)
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/signalkraft/myPyllant/build-test.yaml)
 
-A Python library to interact with the API behind the myVAILLANT app, needs at least Python 3.10.
+A Python library to interact with the API behind the myVAILLANT app ((and branded versions of it, such as the MiGo app from Saunier Duval). Needs at least Python 3.10.
 
-Not affiliated with Vaillant, the developers take no responsibility for anything that happens to your Vaillant devices because of this library.
+Not affiliated with Vaillant, the developers take no responsibility for anything that happens to your devices because of this library.
 
 ![myPyllant](https://raw.githubusercontent.com/signalkraft/myPyllant/main/logo.png)
 
 ## Install and Test
 
 > **Warning**
 > 
 > You need at least Python 3.10
 
 ```shell
 pip install myPyllant
-python3 -m myPyllant.export user password country
+python3 -m myPyllant.export user password country brand
 # See python3 -m myPyllant.export -h for more options and a list of countries
 ```
 
 The `--data` argument exports historical data of the devices in your system.
 Without this keyword, information about your system will be exported as JSON.
 
 ## Usage
 
 ```python
 import argparse
 import asyncio
 from datetime import datetime, timedelta
 
-from custom_components.mypyllant.const import COUNTRIES
-
 from myPyllant.api import MyPyllantAPI
+from myPyllant.const import BRANDS, COUNTRIES, DEFAULT_BRAND
 
 parser = argparse.ArgumentParser(description="Export data from myVaillant API   .")
 parser.add_argument("user", help="Username (email address) for the myVaillant app")
 parser.add_argument("password", help="Password for the myVaillant app")
 parser.add_argument(
     "country",
     help="Country your account is registered in, i.e. 'germany'",
-    choices=COUNTRIES.keys(),
+    choices=COUNTRIES[DEFAULT_BRAND].keys(),
+)
+parser.add_argument(
+    "brand",
+    help="Brand your account is registered in, i.e. 'vaillant'",
+    default=DEFAULT_BRAND,
+    choices=BRANDS.keys(),
 )
 
 
-async def main(user, password, country):
-    async with MyPyllantAPI(user, password, country) as api:
+async def main(user, password, country, brand):
+    async with MyPyllantAPI(user, password, country, brand) as api:
         async for system in api.get_systems():
             print(await api.set_holiday(system, datetime.now()))
             print(
                 await (
                     await api.set_holiday(
                         system, datetime.now(), datetime.now() + timedelta(days=1)
                     )
@@ -67,22 +72,21 @@
             print(await api.set_set_back_temperature(system.zones[0], 15.5))
             print(await api.quick_veto_zone_temperature(system.zones[0], 21, 5))
             print(await api.cancel_quick_veto_zone_temperature(system.zones[0]))
 
 
 if __name__ == "__main__":
     args = parser.parse_args()
-    asyncio.run(main(args.user, args.password, args.country))
+    asyncio.run(main(args.user, args.password, args.country, args.brand))
 
 ```
 
 ### Tested Configurations
 
-* Vaillant aroTHERM plus heatpump, sensoCOMFORT VRC 720, sensoNET VR 921
-* [VMW 23CS/1-5 C (N-ES) ecoTEC plus](https://github.com/signalkraft/myPyllant/pull/6)
+See https://github.com/signalkraft/mypyllant-component/blob/main/README.md#tested-setups
 
 ## Contributing
 
 > **Warning**
 > 
 > You need at least Python 3.10
 
@@ -94,29 +98,29 @@
 pip install -r requirements-dev.txt
 pre-commit install
 pytest
 ```
 
 ### Supporting new Countries
 
-The myVAILLANT app uses Keycloak and OIDC for authentication, with a realm for each country.
+The myVAILLANT app uses Keycloak and OIDC for authentication, with a realm for each country and brand.
 There is a script to check which countries are supported:
 
 ```shell
 python3 tests/find_countries.py
 ```
 
 Copy the resulting dictionary into [src/myPyllant/const.py](src/myPyllant/const.py)
 
 ### Contributing Test Data
 
 Because the myVAILLANT API isn't documented, you can help the development of this library by contributing test data:
 
 ```shell
-python3 tests/generate_test_data.py username password country
+python3 tests/generate_test_data.py username password country brand
 ```
 
 Create a fork of this repository and create a PR with the newly created folder in `test/json`.
 
 ## Notes
 
 * Auth is loosely based on https://github.com/TA2k/ioBroker.vaillant
```

### Comparing `mypyllant-0.2.1/pyproject.toml` & `mypyllant-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.1/PKG-INFO` & `mypyllant-0.2.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myPyllant
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Python library to interact with the API behind the myVAILLANT app
 Project-URL: Homepage, https://github.com/signalkraft/myPyllant
 Project-URL: Bug Tracker, https://github.com/signalkraft/myPyllant/issues
 Author-email: Philipp <pd@signalkraft.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,58 +15,63 @@
 Description-Content-Type: text/markdown
 
 # myPyllant
 
 [![PyPI](https://img.shields.io/pypi/v/myPyllant)](https://pypi.org/project/myPyllant/)
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/signalkraft/myPyllant/build-test.yaml)
 
-A Python library to interact with the API behind the myVAILLANT app, needs at least Python 3.10.
+A Python library to interact with the API behind the myVAILLANT app ((and branded versions of it, such as the MiGo app from Saunier Duval). Needs at least Python 3.10.
 
-Not affiliated with Vaillant, the developers take no responsibility for anything that happens to your Vaillant devices because of this library.
+Not affiliated with Vaillant, the developers take no responsibility for anything that happens to your devices because of this library.
 
 ![myPyllant](https://raw.githubusercontent.com/signalkraft/myPyllant/main/logo.png)
 
 ## Install and Test
 
 > **Warning**
 > 
 > You need at least Python 3.10
 
 ```shell
 pip install myPyllant
-python3 -m myPyllant.export user password country
+python3 -m myPyllant.export user password country brand
 # See python3 -m myPyllant.export -h for more options and a list of countries
 ```
 
 The `--data` argument exports historical data of the devices in your system.
 Without this keyword, information about your system will be exported as JSON.
 
 ## Usage
 
 ```python
 import argparse
 import asyncio
 from datetime import datetime, timedelta
 
-from custom_components.mypyllant.const import COUNTRIES
-
 from myPyllant.api import MyPyllantAPI
+from myPyllant.const import BRANDS, COUNTRIES, DEFAULT_BRAND
 
 parser = argparse.ArgumentParser(description="Export data from myVaillant API   .")
 parser.add_argument("user", help="Username (email address) for the myVaillant app")
 parser.add_argument("password", help="Password for the myVaillant app")
 parser.add_argument(
     "country",
     help="Country your account is registered in, i.e. 'germany'",
-    choices=COUNTRIES.keys(),
+    choices=COUNTRIES[DEFAULT_BRAND].keys(),
+)
+parser.add_argument(
+    "brand",
+    help="Brand your account is registered in, i.e. 'vaillant'",
+    default=DEFAULT_BRAND,
+    choices=BRANDS.keys(),
 )
 
 
-async def main(user, password, country):
-    async with MyPyllantAPI(user, password, country) as api:
+async def main(user, password, country, brand):
+    async with MyPyllantAPI(user, password, country, brand) as api:
         async for system in api.get_systems():
             print(await api.set_holiday(system, datetime.now()))
             print(
                 await (
                     await api.set_holiday(
                         system, datetime.now(), datetime.now() + timedelta(days=1)
                     )
@@ -83,22 +88,21 @@
             print(await api.set_set_back_temperature(system.zones[0], 15.5))
             print(await api.quick_veto_zone_temperature(system.zones[0], 21, 5))
             print(await api.cancel_quick_veto_zone_temperature(system.zones[0]))
 
 
 if __name__ == "__main__":
     args = parser.parse_args()
-    asyncio.run(main(args.user, args.password, args.country))
+    asyncio.run(main(args.user, args.password, args.country, args.brand))
 
 ```
 
 ### Tested Configurations
 
-* Vaillant aroTHERM plus heatpump, sensoCOMFORT VRC 720, sensoNET VR 921
-* [VMW 23CS/1-5 C (N-ES) ecoTEC plus](https://github.com/signalkraft/myPyllant/pull/6)
+See https://github.com/signalkraft/mypyllant-component/blob/main/README.md#tested-setups
 
 ## Contributing
 
 > **Warning**
 > 
 > You need at least Python 3.10
 
@@ -110,29 +114,29 @@
 pip install -r requirements-dev.txt
 pre-commit install
 pytest
 ```
 
 ### Supporting new Countries
 
-The myVAILLANT app uses Keycloak and OIDC for authentication, with a realm for each country.
+The myVAILLANT app uses Keycloak and OIDC for authentication, with a realm for each country and brand.
 There is a script to check which countries are supported:
 
 ```shell
 python3 tests/find_countries.py
 ```
 
 Copy the resulting dictionary into [src/myPyllant/const.py](src/myPyllant/const.py)
 
 ### Contributing Test Data
 
 Because the myVAILLANT API isn't documented, you can help the development of this library by contributing test data:
 
 ```shell
-python3 tests/generate_test_data.py username password country
+python3 tests/generate_test_data.py username password country brand
 ```
 
 Create a fork of this repository and create a PR with the newly created folder in `test/json`.
 
 ## Notes
 
 * Auth is loosely based on https://github.com/TA2k/ioBroker.vaillant
```

