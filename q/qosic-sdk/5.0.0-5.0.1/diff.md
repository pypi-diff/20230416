# Comparing `tmp/qosic_sdk-5.0.0.tar.gz` & `tmp/qosic_sdk-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qosic_sdk-5.0.0.tar", max compression
+gzip compressed data, was "qosic_sdk-5.0.1.tar", max compression
```

## Comparing `qosic_sdk-5.0.0.tar` & `qosic_sdk-5.0.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     1070 2023-03-12 21:28:03.303354 qosic_sdk-5.0.0/LICENSE
--rw-r--r--   0        0        0     2689 2023-04-14 01:28:48.893584 qosic_sdk-5.0.0/README.rst
--rw-r--r--   0        0        0     1455 2023-04-14 01:32:48.475923 qosic_sdk-5.0.0/pyproject.toml
--rw-r--r--   0        0        0      239 2023-04-14 01:14:33.379707 qosic_sdk-5.0.0/qosic/__init__.py
--rw-r--r--   0        0        0     2324 2023-04-14 01:31:39.956112 qosic_sdk-5.0.0/qosic/client.py
--rw-r--r--   0        0        0      373 2023-04-14 00:58:28.576720 qosic_sdk-5.0.0/qosic/errors.py
--rw-r--r--   0        0        0      320 2023-03-12 21:28:03.304354 qosic_sdk-5.0.0/qosic/logger.py
--rw-r--r--   0        0        0        0 2023-04-14 01:15:19.899605 qosic_sdk-5.0.0/qosic/mobile_carriers/__init__.py
--rw-r--r--   0        0        0       60 2023-04-14 01:16:57.383390 qosic_sdk-5.0.0/qosic/mobile_carriers/bj/__init__.py
--rw-r--r--   0        0        0     1605 2023-04-14 01:27:02.658877 qosic_sdk-5.0.0/qosic/mobile_carriers/bj/moov.py
--rw-r--r--   0        0        0     3639 2023-04-14 01:26:12.206016 qosic_sdk-5.0.0/qosic/mobile_carriers/bj/mtn.py
--rw-r--r--   0        0        0     2103 2023-04-14 01:30:49.059252 qosic_sdk-5.0.0/qosic/mobile_carriers/utils.py
--rw-r--r--   0        0        0      424 2023-04-14 01:11:42.396009 qosic_sdk-5.0.0/qosic/protocols.py
--rw-r--r--   0        0        0        0 2023-03-12 21:28:03.304354 qosic_sdk-5.0.0/qosic/py.typed
--rw-r--r--   0        0        0     2036 2023-04-14 01:30:29.259307 qosic_sdk-5.0.0/qosic/utils.py
--rw-r--r--   0        0        0     3734 1970-01-01 00:00:00.000000 qosic_sdk-5.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-03-12 21:28:03.303354 qosic_sdk-5.0.1/LICENSE
+-rw-r--r--   0        0        0     2369 2023-04-16 09:37:55.342889 qosic_sdk-5.0.1/README.rst
+-rw-r--r--   0        0        0     1455 2023-04-16 07:23:44.930957 qosic_sdk-5.0.1/pyproject.toml
+-rw-r--r--   0        0        0      244 2023-04-16 07:23:44.941957 qosic_sdk-5.0.1/qosic/__init__.py
+-rw-r--r--   0        0        0     2349 2023-04-16 07:46:29.774705 qosic_sdk-5.0.1/qosic/client.py
+-rw-r--r--   0        0        0      373 2023-04-14 00:58:28.576720 qosic_sdk-5.0.1/qosic/errors.py
+-rw-r--r--   0        0        0      320 2023-03-12 21:28:03.304354 qosic_sdk-5.0.1/qosic/logger.py
+-rw-r--r--   0        0        0        0 2023-04-14 01:15:19.899605 qosic_sdk-5.0.1/qosic/mobile_carriers/__init__.py
+-rw-r--r--   0        0        0       60 2023-04-14 01:16:57.383390 qosic_sdk-5.0.1/qosic/mobile_carriers/bj/__init__.py
+-rw-r--r--   0        0        0     1595 2023-04-15 21:11:45.413318 qosic_sdk-5.0.1/qosic/mobile_carriers/bj/moov.py
+-rw-r--r--   0        0        0     3658 2023-04-16 07:09:23.575916 qosic_sdk-5.0.1/qosic/mobile_carriers/bj/mtn.py
+-rw-r--r--   0        0        0     1869 2023-04-16 07:12:13.535902 qosic_sdk-5.0.1/qosic/mobile_carriers/bj/mtn_.py
+-rw-r--r--   0        0        0     1724 2023-04-15 19:16:18.777977 qosic_sdk-5.0.1/qosic/mobile_carriers/utils.py
+-rw-r--r--   0        0        0     1369 2023-04-16 07:25:33.360774 qosic_sdk-5.0.1/qosic/protocols.py
+-rw-r--r--   0        0        0        0 2023-03-12 21:28:03.304354 qosic_sdk-5.0.1/qosic/py.typed
+-rw-r--r--   0        0        0     2421 2023-04-15 21:11:45.953317 qosic_sdk-5.0.1/qosic/utils.py
+-rw-r--r--   0        0        0     3414 1970-01-01 00:00:00.000000 qosic_sdk-5.0.1/PKG-INFO
```

### Comparing `qosic_sdk-5.0.0/LICENSE` & `qosic_sdk-5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qosic_sdk-5.0.0/README.rst` & `qosic_sdk-5.0.1/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -8,17 +8,14 @@
 
 .. image:: https://img.shields.io/pypi/v/qosic-sdk.svg
         :target: https://pypi.python.org/pypi/qosic-sdk
 
 .. image:: https://img.shields.io/pypi/pyversions/qosic-sdk
         :target: https://github.com/Tobi-De/qosic-sdk
 
-.. image:: https://api.travis-ci.com/Tobi-De/qosic-sdk.svg
-        :target: https://travis-ci.com/Tobi-De/qosic-sdk
-
 .. image:: https://readthedocs.org/projects/qosic-sdk/badge/?version=latest
         :target: https://qosic-sdk.readthedocs.io/en/latest/?version=latest
         :alt: Documentation Status
 
 .. image:: https://img.shields.io/badge/license-MIT-blue.svg
         :target: https://github.com/Tobi-De/qosic-sdk/blob/main/LICENSE
 
@@ -48,34 +45,30 @@
 
        pip install qosic-sdk
 
 .. code:: python3
 
 
        from dotenv import dotenv_values
-       from qosic import Client
-       from qosic.mobile_carriers import bj
+       from qosic import Client, bj
 
        config = dotenv_values(".env")
 
        moov_client_id = config.get("MOOV_CLIENT_ID")
        mtn_client_id = config.get("MTN_CLIENT_ID")
-       server_login = config.get("SERVER_LOGIN")
-       server_pass = config.get("SERVER_PASSWORD")
-       # This is just for test purpose, you should directly pass the phone number
-       phone = config.get("PHONE_NUMBER")
 
+       login = config.get("SERVER_LOGIN")
+       pass = config.get("SERVER_PASSWORD")
 
        def main():
-           client = Client(
-               login=server_login,
-               password=server_pass,
-               providers=[bj.MTN(id=mtn_client_id), bj.MOOV(id=moov_client_id)],
-           )
-           result = client.pay(phone=phone, amount=500, first_name="User", last_name="TEST")
+           phone = "229XXXXXXXX"
+           mobile_carriers = [bj.MTN(id=mtn_client_id), bj.MOOV(id=moov_client_id)]
+           client = Client(login=login, password=pass, mobile_carriers=mobile_carriers)
+
+           result = client.pay(phone=phone, amount=500)
            print(result)
            if result.success:
                print(f"Everything went fine")
 
            result = client.refund(reference=result.reference, phone=phone)
            print(result)
```

### Comparing `qosic_sdk-5.0.0/pyproject.toml` & `qosic_sdk-5.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qosic-sdk"
-version = "5.0.0"
+version = "5.0.1"
 description = "An unofficial python sdk for the QosIc platform."
 authors = ["Tobi-De <tobidegnon@protonmail.com>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/Tobi-De/qosic-sdk"
 homepage = "https://github.com/Tobi-De/qosic-sdk"
 keywords = ["python", "qosic-sdk", "qosic", "qos", "payment", "momo", "mobile money"]
```

### Comparing `qosic_sdk-5.0.0/qosic/client.py` & `qosic_sdk-5.0.1/qosic/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from .protocols import MobileCarrier
 from .utils import Result, guess_mobile_carrier_from, Payer, log_response, log_request
 
 
 @dataclass
 class Client:
     """The synchronous client that will be used to make the request to the QosIc api
-    :param mobile_carriers: The list of your mobile_carrier
+    :param mobile_carriers: The list of configured mobile carriers to use to communicate with the API.
     :param login: Your server authentication login/user
     :param password: Your server authentication password
     :param logger: Custom logger
     :param base_url: The QosIC server root domain if you ever need to change it
     """
 
     login: str
@@ -50,16 +50,16 @@
         self._http_client.close()
 
     def pay(
         self,
         *,
         phone: str,
         amount: int,
-        first_name: str | None = None,
-        last_name: str | None = None,
+        first_name: str = "",
+        last_name: str = "",
     ) -> Result:
         payer = Payer(
             phone=phone, amount=amount, first_name=first_name, last_name=last_name
         )
         mobile_carrier = guess_mobile_carrier_from(
             phone=phone, mobile_carriers=self.mobile_carriers
         )
```

### Comparing `qosic_sdk-5.0.0/qosic/mobile_carriers/bj/moov.py` & `qosic_sdk-5.0.1/qosic/mobile_carriers/bj/moov.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 from __future__ import annotations
 
 import httpx
 from dataclasses import dataclass, field
 
 from qosic.errors import FeatureNotImplementedError
 from qosic.mobile_carriers.utils import (
-    _generic_reference_factory,
-    _validate_reference_factory,
-    _req_body_from_payer,
-    _handle_common_errors,
-    _extract_json,
-    _resp_is_ok,
+    generic_reference_factory,
+    validate_reference_factory,
+    handle_common_errors,
+    get_json_from,
+    response_is_ok,
 )
 from ...utils import Payer, Result
 
 MOOV_PREFIXES = ["55", "60", "63", "64", "65", "68", "94", "95", "98", "99"]
 MOOV_PAYMENT_PATH = "/QosicBridge/user/requestpaymentmv"
 
 
 @dataclass(frozen=True)
 class MOOV:
     id: str
     allowed_prefixes: list[str] = field(default_factory=lambda: MOOV_PREFIXES)
-    reference_factory: callable = _generic_reference_factory
+    reference_factory: callable = generic_reference_factory
 
     def __post_init__(self):
-        _validate_reference_factory(self.reference_factory)
+        validate_reference_factory(self.reference_factory)
 
     def pay(self, client: httpx.Client, *, payer: Payer) -> Result:
-        body = _req_body_from_payer(self, payer)
+        body = payer.to_qos_compliant_payment_request_body(self)
         response = client.post(url=MOOV_PAYMENT_PATH, json=body)
-        _handle_common_errors(response, provider=self, payer=payer)
-        json_content = _extract_json(response)
-        ok = _resp_is_ok(response) and json_content["responsecode"] == "0"
+        handle_common_errors(response, provider=self, payer=payer)
+        json_content = get_json_from(response)
+        ok = response_is_ok(response) and json_content["responsecode"] == "0"
         status = Result.Status.CONFIRMED if ok else Result.Status.FAILED
         return Result(
             reference=body["transref"],
             mobile_carrier=self,
             status=status,
             response=response,
             phone=payer.phone,
```

### Comparing `qosic_sdk-5.0.0/qosic/mobile_carriers/bj/mtn.py` & `qosic_sdk-5.0.1/qosic/mobile_carriers/bj/mtn.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,20 +3,19 @@
 import contextlib
 
 import httpx
 import polling2
 from dataclasses import dataclass, field
 
 from qosic.mobile_carriers.utils import (
-    _generic_reference_factory,
-    _validate_reference_factory,
-    _req_body_from_payer,
-    _handle_common_errors,
-    _extract_json,
-    _resp_is_ok,
+    generic_reference_factory,
+    validate_reference_factory,
+    handle_common_errors,
+    get_json_from,
+    response_is_ok,
 )
 from ...utils import Payer, Result
 
 MTN_PAYMENT_PATH = "/QosicBridge/user/requestpayment"
 MTN_PAYMENT_STATUS_PATH = "/QosicBridge/user/gettransactionstatus"
 MTN_PREFIXES = ["51", "52", "53", "61", "62", "66", "67", "69", "90", "91", "96", "97"]
 MTN_REFUND_PATH = "/QosicBridge/user/refund"
@@ -25,31 +24,31 @@
 @dataclass(frozen=True)
 class MTN:
     id: str
     step: int = 10
     timeout: int = 60 * 2
     max_tries: int | None = None
     allowed_prefixes: list[str] = field(default_factory=lambda: MTN_PREFIXES)
-    reference_factory: callable = _generic_reference_factory
+    reference_factory: callable = generic_reference_factory
 
     def __post_init__(self):
-        _validate_reference_factory(self.reference_factory)
+        validate_reference_factory(self.reference_factory)
         assert 5 <= self.step <= 30, f"Step {self.step} must be between 5 and 30"
         assert (
             60 <= self.timeout <= 180
         ), f"Timeout {self.timeout}  must be between 60 and 180"
         if self.max_tries:
             assert (
                 self.max_tries * self.step <= self.timeout
             ), f"max_tries exceed timeout: {self.max_tries} * {self.step} > {self.timeout}"
 
     def pay(self, client: httpx.Client, *, payer: Payer) -> Result:
-        body = _req_body_from_payer(self, payer)
+        body = payer.to_qos_compliant_payment_request_body(self)
         response = client.post(url=MTN_PAYMENT_PATH, json=body)
-        _handle_common_errors(response, provider=self, payer=payer)
+        handle_common_errors(response, provider=self, payer=payer)
         res_dict = {
             "reference": body["transref"],
             "mobile_carrier": self,
             "status": Result.Status.FAILED,
             "response": response,
             "phone": payer.phone,
         }
@@ -67,28 +66,30 @@
         return Result(**res_dict)
 
     def _check_status(self, *, client: httpx.Client, reference: str) -> Result.Status:
         response = client.post(
             url=MTN_PAYMENT_STATUS_PATH,
             json={"clientid": self.id, "transref": reference},
         )
-        json_content = _extract_json(response)
-        if not _resp_is_ok(response) or json_content["responsecode"] is None:
+        json_content = get_json_from(response)
+        if not response_is_ok(response) or json_content["responsecode"] is None:
             raise MTNPaymentRejected()
-        if _resp_is_ok(response) and json_content["responsecode"] == "00":
+        if response_is_ok(response) and json_content["responsecode"] == "00":
             return Result.Status.CONFIRMED
         return Result.Status.FAILED
 
     def refund(self, client: httpx.Client, *, reference: str, phone: str) -> Result:
         response = client.post(
             url=MTN_REFUND_PATH,
             json={"clientid": self.id, "transref": reference},
         )
-        _handle_common_errors(response, provider=self)
-        ok = _resp_is_ok(response) and _extract_json(response)["responsecode"] == "00"
+        handle_common_errors(response, provider=self)
+        ok = (
+            response_is_ok(response) and get_json_from(response)["responsecode"] == "00"
+        )
         status = Result.Status.CONFIRMED if ok else Result.Status.FAILED
         return Result(
             reference=reference,
             mobile_carrier=self,
             status=status,
             response=response,
             phone=phone,
```

### Comparing `qosic_sdk-5.0.0/qosic/mobile_carriers/utils.py` & `qosic_sdk-5.0.1/qosic/mobile_carriers/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,30 +7,29 @@
 
 from qosic.errors import (
     InvalidCredentialsError,
     InvalidProviderIDError,
     UserAccountNotFoundError,
     ServerError,
 )
-from qosic.protocols import MobileCarrier
-from qosic.utils import Payer, get_random_string
+from qosic.utils import get_random_string
 
 
-def _generic_reference_factory(*args, **kwargs) -> str:
+def generic_reference_factory(*args, **kwargs) -> str:
     return get_random_string()
 
 
-def _extract_json(response: httpx.Response):
+def get_json_from(response: httpx.Response) -> dict:
     try:
         return response.json()
     except json.decoder.JSONDecodeError:
         return {"responsecode": None}
 
 
-def _handle_common_errors(response: httpx.Response, **kwargs) -> None:
+def handle_common_errors(response: httpx.Response, **kwargs) -> None:
     status: int = response.status_code  # noqa
     if codes.is_server_error(status):
         raise ServerError(
             "Qosic server if failing for some reason, active debug for more details."
         )
     provider = kwargs.get("provider")
     if provider and codes.NOT_FOUND == status:
@@ -42,27 +41,16 @@
     payer = kwargs.get("payer")
     if payer and codes.EXPECTATION_FAILED == status:
         raise UserAccountNotFoundError(
             f"A mobile money account was not found for {payer.phone}"
         )
 
 
-def _validate_reference_factory(func: callable) -> None:
+def validate_reference_factory(func: callable) -> None:
     ref = func()
     assert isinstance(ref, str), "Your factory function should return strings"
     assert len(ref) > 6, "Your factory function generate too short strings"
     assert len(ref) <= 16, "Your factory function generate too long strings"
 
 
-def _req_body_from_payer(provider: MobileCarrier, payer: Payer) -> dict:
-    return {
-        "clientid": provider.id,
-        "msisdn": payer.phone,
-        "amount": str(payer.amount),
-        "transref": provider.reference_factory(payer),
-        "firstname": payer.first_name or "",
-        "lastname": payer.last_name or "",
-    }
-
-
-def _resp_is_ok(response: httpx.Response):
+def response_is_ok(response: httpx.Response):
     return response.status_code == httpx.codes.OK
```

### Comparing `qosic_sdk-5.0.0/qosic/utils.py` & `qosic_sdk-5.0.1/qosic/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     *, phone: str, mobile_carriers: list[MobileCarrier]
 ) -> MobileCarrier:
     prefix = phone[3:5]
     for carrier in mobile_carriers:
         if prefix in carrier.allowed_prefixes:
             return carrier
     raise MobileCarrierNotFoundError(
-        f"A provider was not found for the given phone number: {phone}"
+        f"A mobile carrier was not found for the given phone number: {phone}"
     )
 
 
 @dataclass(frozen=True)
 class Result:
     """A helper class to summarize the responses from the server."""
 
@@ -64,15 +64,27 @@
         return self.status == self.Status.CONFIRMED
 
 
 @dataclass(frozen=True)
 class Payer:
     phone: str
     amount: int
-    first_name: str | None = None
-    last_name: str | None = None
+    first_name: str = ""
+    last_name: str = ""
 
     def __post_init__(self):
         if not re.fullmatch(r"\d{11}", self.phone):
             raise InvalidPhoneNumberError(
                 f"Invalid format for {self.phone}, ex: 229XXXXXXXX"
             )
+
+    def to_qos_compliant_payment_request_body(
+        self, mobile_carrier: MobileCarrier
+    ) -> dict:
+        return {
+            "clientid": mobile_carrier.id,
+            "msisdn": self.phone,
+            "amount": str(self.amount),
+            "transref": mobile_carrier.reference_factory(self),
+            "firstname": self.first_name,
+            "lastname": self.last_name,
+        }
```

### Comparing `qosic_sdk-5.0.0/PKG-INFO` & `qosic_sdk-5.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qosic-sdk
-Version: 5.0.0
+Version: 5.0.1
 Summary: An unofficial python sdk for the QosIc platform.
 Home-page: https://github.com/Tobi-De/qosic-sdk
 License: MIT
 Keywords: python,qosic-sdk,qosic,qos,payment,momo,mobile money
 Author: Tobi-De
 Author-email: tobidegnon@protonmail.com
 Requires-Python: >=3.8,<4.0
@@ -34,17 +34,14 @@
 
 .. image:: https://img.shields.io/pypi/v/qosic-sdk.svg
         :target: https://pypi.python.org/pypi/qosic-sdk
 
 .. image:: https://img.shields.io/pypi/pyversions/qosic-sdk
         :target: https://github.com/Tobi-De/qosic-sdk
 
-.. image:: https://api.travis-ci.com/Tobi-De/qosic-sdk.svg
-        :target: https://travis-ci.com/Tobi-De/qosic-sdk
-
 .. image:: https://readthedocs.org/projects/qosic-sdk/badge/?version=latest
         :target: https://qosic-sdk.readthedocs.io/en/latest/?version=latest
         :alt: Documentation Status
 
 .. image:: https://img.shields.io/badge/license-MIT-blue.svg
         :target: https://github.com/Tobi-De/qosic-sdk/blob/main/LICENSE
 
@@ -74,34 +71,30 @@
 
        pip install qosic-sdk
 
 .. code:: python3
 
 
        from dotenv import dotenv_values
-       from qosic import Client
-       from qosic.mobile_carriers import bj
+       from qosic import Client, bj
 
        config = dotenv_values(".env")
 
        moov_client_id = config.get("MOOV_CLIENT_ID")
        mtn_client_id = config.get("MTN_CLIENT_ID")
-       server_login = config.get("SERVER_LOGIN")
-       server_pass = config.get("SERVER_PASSWORD")
-       # This is just for test purpose, you should directly pass the phone number
-       phone = config.get("PHONE_NUMBER")
 
+       login = config.get("SERVER_LOGIN")
+       pass = config.get("SERVER_PASSWORD")
 
        def main():
-           client = Client(
-               login=server_login,
-               password=server_pass,
-               providers=[bj.MTN(id=mtn_client_id), bj.MOOV(id=moov_client_id)],
-           )
-           result = client.pay(phone=phone, amount=500, first_name="User", last_name="TEST")
+           phone = "229XXXXXXXX"
+           mobile_carriers = [bj.MTN(id=mtn_client_id), bj.MOOV(id=moov_client_id)]
+           client = Client(login=login, password=pass, mobile_carriers=mobile_carriers)
+
+           result = client.pay(phone=phone, amount=500)
            print(result)
            if result.success:
                print(f"Everything went fine")
 
            result = client.refund(reference=result.reference, phone=phone)
            print(result)
```

