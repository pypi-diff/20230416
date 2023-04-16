# Comparing `tmp/python_frank_energie-3.0.0a2.tar.gz` & `tmp/python_frank_energie-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_frank_energie-3.0.0a2.tar", max compression
+gzip compressed data, was "python_frank_energie-3.1.0.tar", max compression
```

## Comparing `python_frank_energie-3.0.0a2.tar` & `python_frank_energie-3.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11346 2023-03-31 20:23:15.208961 python_frank_energie-3.0.0a2/LICENSE
--rw-r--r--   0        0        0      325 2023-03-31 20:23:15.208961 python_frank_energie-3.0.0a2/README.md
--rw-r--r--   0        0        0     2340 2023-03-31 20:23:35.157119 python_frank_energie-3.0.0a2/pyproject.toml
--rw-r--r--   0        0        0      175 2023-03-31 20:23:15.208961 python_frank_energie-3.0.0a2/python_frank_energie/__init__.py
--rw-r--r--   0        0        0      257 2023-03-31 20:23:15.208961 python_frank_energie-3.0.0a2/python_frank_energie/exceptions.py
--rw-r--r--   0        0        0     5080 2023-03-31 20:23:15.208961 python_frank_energie-3.0.0a2/python_frank_energie/frank_energie.py
--rw-r--r--   0        0        0     5763 2023-03-31 20:23:15.208961 python_frank_energie-3.0.0a2/python_frank_energie/models.py
--rw-r--r--   0        0        0     1219 1970-01-01 00:00:00.000000 python_frank_energie-3.0.0a2/PKG-INFO
+-rw-r--r--   0        0        0    11346 2023-04-16 12:06:31.436265 python_frank_energie-3.1.0/LICENSE
+-rw-r--r--   0        0        0      325 2023-04-16 12:06:31.436265 python_frank_energie-3.1.0/README.md
+-rw-r--r--   0        0        0     2332 2023-04-16 12:06:56.724124 python_frank_energie-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0      175 2023-04-16 12:06:31.436265 python_frank_energie-3.1.0/python_frank_energie/__init__.py
+-rw-r--r--   0        0        0      332 2023-04-16 12:06:31.440265 python_frank_energie-3.1.0/python_frank_energie/exceptions.py
+-rw-r--r--   0        0        0     5975 2023-04-16 12:06:31.440265 python_frank_energie-3.1.0/python_frank_energie/frank_energie.py
+-rw-r--r--   0        0        0     6766 2023-04-16 12:06:31.440265 python_frank_energie-3.1.0/python_frank_energie/models.py
+-rw-r--r--   0        0        0     1217 1970-01-01 00:00:00.000000 python_frank_energie-3.1.0/PKG-INFO
```

### Comparing `python_frank_energie-3.0.0a2/LICENSE` & `python_frank_energie-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_frank_energie-3.0.0a2/pyproject.toml` & `python_frank_energie-3.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-frank-energie"
-version = "3.0.0-alpha-2"
+version = "3.1.0"
 description = "Asynchronous Python client for the Frank Energie"
 authors = ["DCSBL"]
 maintainers = ["DCSBL"]
 license = "Apache License 2.0"
 readme = "README.md"
 homepage = "https://github.com/dcsbl/python-frank-energie"
 repository = "https://github.com/dcsbl/python-frank-energie"
@@ -27,15 +27,15 @@
 flake8 = "^4.0.1"
 flake8-docstrings = "^1.5.0"
 isort = "^5.11.4"
 pre-commit = "^3.1.1"
 pre-commit-hooks = "^4.4.0"
 pylint = "^2.15.10"
 pytest = "^7.2.1"
-pytest-asyncio = "^0.20.3"
+pytest-asyncio = "^0.21.0"
 pytest-cov = "^4.0.0"
 yamllint = "^1.29.0"
 pyupgrade = "^3.3.1"
 flake8-simplify = "^0.19.3"
 vulture = "^2.7"
 flake8-bandit = "^3.0.0"
 flake8-bugbear = "^23.3.12"
```

### Comparing `python_frank_energie-3.0.0a2/python_frank_energie/frank_energie.py` & `python_frank_energie-3.1.0/python_frank_energie/frank_energie.py`

 * *Files 12% similar despite different names*

```diff
@@ -58,14 +58,34 @@
             "operationName": "Login",
             "variables": {"email": username, "password": password},
         }
 
         self._auth = Authentication.from_dict(await self._query(query))
         return self._auth
 
+    async def renewToken(self, authToken: str, refreshToken: str) -> str:
+        query = {
+            "query": """
+                mutation RenewToken($authToken: String!, $refreshToken: String!) {
+                    renewToken(authToken: $authToken, refreshToken: $refreshToken) {
+                        authToken
+                        refreshToken
+                    }
+                }
+            """,
+            "operationName": "RenewToken",
+            "variables": {"authToken": authToken, "refreshToken": refreshToken},
+        }
+
+        json = await self._query(query)
+        print(json)
+
+        self._auth = Authentication.from_dict(json)
+        return self._auth
+
     async def monthSummary(self) -> MonthSummary:
 
         if self._auth is None:
             raise AuthRequiredException
 
         query = {
             "query": """
@@ -139,14 +159,22 @@
         return (
             PriceData(
                 response["data"]["marketPricesElectricity"] if response["data"] else {}
             ),
             PriceData(response["data"]["marketPricesGas"] if response["data"] else {}),
         )
 
+    @property
+    def is_authenticated(self) -> bool:
+        """Return if client is authenticated.
+
+        Does not actually check if the token is valid.
+        """
+        return self._auth is not None
+
     async def close(self) -> None:
         """Close client session."""
         if self._session and self._close_session:
             await self._session.close()
 
     async def __aenter__(self) -> FrankEnergie:
         """Async enter.
```

### Comparing `python_frank_energie-3.0.0a2/python_frank_energie/models.py` & `python_frank_energie-3.1.0/python_frank_energie/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,42 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from datetime import datetime, timedelta, timezone
 
 from dateutil import parser
 
-from .exceptions import AuthException
+from .exceptions import AuthException, RequestException
 
 
 @dataclass
 class Authentication:
+    """Authentication data.
+
+    authToken: The token to use for authenticated requests.
+    refreshToken: The token to use to renew the authToken.
+    """
 
     authToken: str
     refreshToken: str
 
     @staticmethod
     def from_dict(data: dict[str, str]) -> Authentication:
+        """Parse the response from the login or renewToken mutation."""
 
         if errors := data.get("errors"):
             raise AuthException(errors[0]["message"])
 
-        payload = data.get("data").get("login")
-        if payload is None:
+        login_payload = data.get("data", {}).get("login")
+        renew_payload = data.get("data", {}).get("renewToken")
+        if not login_payload and not renew_payload:
             raise AuthException("Unexpected response")
 
+        payload = login_payload or renew_payload
+
         return Authentication(
             authToken=payload.get("authToken"),
             refreshToken=payload.get("refreshToken"),
         )
 
 
 @dataclass
@@ -38,19 +47,19 @@
     advancedPaymentAmount: float
     hasCO2Compensation: bool
 
     @staticmethod
     def from_dict(data: dict[str, str]) -> Authentication:
 
         if errors := data.get("errors"):
-            raise AuthException(errors[0]["message"])
+            raise RequestException(errors[0]["message"])
 
-        payload = data.get("data").get("me")
-        if payload is None:
-            raise AuthException("Unexpected response")
+        payload = data.get("data", {}).get("me")
+        if not payload:
+            raise RequestException("Unexpected response")
 
         return User(
             connectionsStatus=payload.get("connectionsStatus"),
             firstMeterReadingDate=payload.get("firstMeterReadingDate"),
             lastMeterReadingDate=payload.get("lastMeterReadingDate"),
             advancedPaymentAmount=payload.get("advancedPaymentAmount"),
             hasCO2Compensation=payload.get("hasCO2Compensation"),
@@ -63,19 +72,19 @@
     expectedCostsUntilLastMeterReadingDate: float
     lastMeterReadingDate: str
 
     @staticmethod
     def from_dict(data: dict[str, str]) -> Authentication:
 
         if errors := data.get("errors"):
-            raise AuthException(errors[0]["message"])
+            raise RequestException(errors[0]["message"])
 
-        payload = data.get("data").get("monthSummary")
-        if payload is None:
-            raise AuthException("Unexpected response")
+        payload = data.get("data", {}).get("monthSummary")
+        if not payload:
+            raise RequestException("Unexpected response")
 
         return MonthSummary(
             actualCostsUntilLastMeterReadingDate=payload.get(
                 "actualCostsUntilLastMeterReadingDate"
             ),
             expectedCostsUntilLastMeterReadingDate=payload.get(
                 "expectedCostsUntilLastMeterReadingDate"
@@ -183,7 +192,28 @@
 
     def asdict(self, attr) -> dict:
         """Return a dict that can be used as entity attribute data."""
         return [
             {"from": e.date_from, "till": e.date_till, "price": getattr(e, attr)}
             for e in self.price_data
         ]
+
+
+@dataclass
+class MarketPrices:
+
+    marketPricesElectricity: PriceData
+    marketPricesGas: PriceData
+
+    @staticmethod
+    def from_dict(data: dict[str, str]) -> MarketPrices:
+        if errors := data.get("errors"):
+            raise RequestException(errors[0]["message"])
+
+        payload = data.get("data", {})
+        if not payload:
+            raise RequestException("Unexpected response")
+
+        return MarketPrices(
+            marketPricesElectricity=PriceData(payload.get("marketPricesElectricity")),
+            marketPricesGas=PriceData(payload.get("marketPricesGas")),
+        )
```

### Comparing `python_frank_energie-3.0.0a2/PKG-INFO` & `python_frank_energie-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-frank-energie
-Version: 3.0.0a2
+Version: 3.1.0
 Summary: Asynchronous Python client for the Frank Energie
 Home-page: https://github.com/dcsbl/python-frank-energie
 License: Apache-2.0
 Author: DCSBL
 Maintainer: DCSBL
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

