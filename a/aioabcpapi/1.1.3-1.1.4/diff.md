# Comparing `tmp/aioabcpapi-1.1.3.tar.gz` & `tmp/aioabcpapi-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioabcpapi-1.1.3.tar", last modified: Wed Feb  1 21:08:56 2023, max compression
+gzip compressed data, was "aioabcpapi-1.1.4.tar", last modified: Sun Apr 16 16:41:09 2023, max compression
```

## Comparing `aioabcpapi-1.1.3.tar` & `aioabcpapi-1.1.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-02-01 21:08:56.966409 aioabcpapi-1.1.3/
--rw-rw-rw-   0        0        0     1085 2022-05-10 19:34:18.000000 aioabcpapi-1.1.3/LICENSE
--rw-rw-rw-   0        0        0     5341 2023-02-01 21:08:56.966409 aioabcpapi-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     4519 2022-11-22 13:00:19.000000 aioabcpapi-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-02-01 21:08:56.907394 aioabcpapi-1.1.3/aioabcpapi/
--rw-rw-rw-   0        0        0      584 2023-02-01 20:02:12.000000 aioabcpapi-1.1.3/aioabcpapi/__init__.py
--rw-rw-rw-   0        0        0      265 2022-07-27 23:21:17.000000 aioabcpapi-1.1.3/aioabcpapi/abcp.py
--rw-rw-rw-   0        0        0    18503 2023-02-01 20:24:12.000000 aioabcpapi-1.1.3/aioabcpapi/api.py
--rw-rw-rw-   0        0        0     4657 2022-12-13 07:04:54.000000 aioabcpapi-1.1.3/aioabcpapi/base.py
-drwxrwxrwx   0        0        0        0 2023-02-01 21:08:56.939402 aioabcpapi-1.1.3/aioabcpapi/cp/
--rw-rw-rw-   0        0        0        2 2022-07-27 23:21:17.000000 aioabcpapi-1.1.3/aioabcpapi/cp/__init__.py
--rw-rw-rw-   0        0        0   110789 2023-02-01 20:59:32.000000 aioabcpapi-1.1.3/aioabcpapi/cp/admin.py
--rw-rw-rw-   0        0        0      360 2022-07-28 02:02:14.000000 aioabcpapi-1.1.3/aioabcpapi/cp/base.py
--rw-rw-rw-   0        0        0    60152 2022-12-13 07:07:31.000000 aioabcpapi-1.1.3/aioabcpapi/cp/client.py
--rw-rw-rw-   0        0        0      485 2022-06-02 20:47:31.000000 aioabcpapi-1.1.3/aioabcpapi/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-02-01 21:08:56.949405 aioabcpapi-1.1.3/aioabcpapi/ts/
--rw-rw-rw-   0        0        0        0 2022-05-22 19:06:06.000000 aioabcpapi-1.1.3/aioabcpapi/ts/__init__.py
--rw-rw-rw-   0        0        0   107523 2022-12-13 06:57:01.000000 aioabcpapi-1.1.3/aioabcpapi/ts/admin.py
--rw-rw-rw-   0        0        0      368 2022-07-28 02:02:14.000000 aioabcpapi-1.1.3/aioabcpapi/ts/base.py
--rw-rw-rw-   0        0        0    44136 2022-12-13 07:00:25.000000 aioabcpapi-1.1.3/aioabcpapi/ts/client.py
-drwxrwxrwx   0        0        0        0 2023-02-01 21:08:56.953405 aioabcpapi-1.1.3/aioabcpapi/utils/
--rw-rw-rw-   0        0        0        2 2022-12-13 06:33:44.000000 aioabcpapi-1.1.3/aioabcpapi/utils/__init__.py
--rw-rw-rw-   0        0        0      805 2022-12-13 07:00:57.000000 aioabcpapi-1.1.3/aioabcpapi/utils/fields_checker.py
--rw-rw-rw-   0        0        0     8625 2023-02-01 20:59:52.000000 aioabcpapi-1.1.3/aioabcpapi/utils/payload.py
-drwxrwxrwx   0        0        0        0 2023-02-01 21:08:56.929399 aioabcpapi-1.1.3/aioabcpapi.egg-info/
--rw-rw-rw-   0        0        0     5341 2023-02-01 21:08:56.000000 aioabcpapi-1.1.3/aioabcpapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      894 2023-02-01 21:08:56.000000 aioabcpapi-1.1.3/aioabcpapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-01 21:08:56.000000 aioabcpapi-1.1.3/aioabcpapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2023-02-01 21:08:56.000000 aioabcpapi-1.1.3/aioabcpapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       56 2023-02-01 21:08:56.000000 aioabcpapi-1.1.3/aioabcpapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      206 2023-02-01 21:08:56.971411 aioabcpapi-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1333 2023-02-01 20:02:12.000000 aioabcpapi-1.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-01 21:08:56.964407 aioabcpapi-1.1.3/test/
--rw-rw-rw-   0        0        0    15807 2022-08-10 22:50:42.000000 aioabcpapi-1.1.3/test/test_payload.py
+drwxrwxrwx   0        0        0        0 2023-04-16 16:41:09.414548 aioabcpapi-1.1.4/
+-rw-rw-rw-   0        0        0     1085 2022-05-10 19:34:18.000000 aioabcpapi-1.1.4/LICENSE
+-rw-rw-rw-   0        0        0     5341 2023-04-16 16:41:09.414548 aioabcpapi-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4519 2022-11-22 13:00:19.000000 aioabcpapi-1.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-16 16:41:09.273688 aioabcpapi-1.1.4/aioabcpapi/
+-rw-rw-rw-   0        0        0      584 2023-04-16 16:40:20.000000 aioabcpapi-1.1.4/aioabcpapi/__init__.py
+-rw-rw-rw-   0        0        0      680 2023-04-11 17:25:28.000000 aioabcpapi-1.1.4/aioabcpapi/abcp.py
+-rw-rw-rw-   0        0        0    18863 2023-04-11 16:46:29.000000 aioabcpapi-1.1.4/aioabcpapi/api.py
+-rw-rw-rw-   0        0        0     4799 2023-04-11 17:25:28.000000 aioabcpapi-1.1.4/aioabcpapi/base.py
+drwxrwxrwx   0        0        0        0 2023-04-16 16:41:09.342685 aioabcpapi-1.1.4/aioabcpapi/cp/
+-rw-rw-rw-   0        0        0        2 2022-07-27 23:21:17.000000 aioabcpapi-1.1.4/aioabcpapi/cp/__init__.py
+-rw-rw-rw-   0        0        0   113231 2023-04-11 17:21:52.000000 aioabcpapi-1.1.4/aioabcpapi/cp/admin.py
+-rw-rw-rw-   0        0        0      767 2023-04-11 17:25:28.000000 aioabcpapi-1.1.4/aioabcpapi/cp/base.py
+-rw-rw-rw-   0        0        0    60152 2022-12-13 07:07:31.000000 aioabcpapi-1.1.4/aioabcpapi/cp/client.py
+-rw-rw-rw-   0        0        0      535 2023-03-24 12:28:09.000000 aioabcpapi-1.1.4/aioabcpapi/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-16 16:41:09.379550 aioabcpapi-1.1.4/aioabcpapi/ts/
+-rw-rw-rw-   0        0        0        0 2022-05-22 19:06:06.000000 aioabcpapi-1.1.4/aioabcpapi/ts/__init__.py
+-rw-rw-rw-   0        0        0   113383 2023-04-11 17:37:33.000000 aioabcpapi-1.1.4/aioabcpapi/ts/admin.py
+-rw-rw-rw-   0        0        0      784 2023-04-11 17:25:28.000000 aioabcpapi-1.1.4/aioabcpapi/ts/base.py
+-rw-rw-rw-   0        0        0    45010 2023-04-11 16:56:32.000000 aioabcpapi-1.1.4/aioabcpapi/ts/client.py
+drwxrwxrwx   0        0        0        0 2023-04-16 16:41:09.399548 aioabcpapi-1.1.4/aioabcpapi/utils/
+-rw-rw-rw-   0        0        0        2 2022-12-13 06:33:44.000000 aioabcpapi-1.1.4/aioabcpapi/utils/__init__.py
+-rw-rw-rw-   0        0        0      805 2022-12-13 07:00:57.000000 aioabcpapi-1.1.4/aioabcpapi/utils/fields_checker.py
+-rw-rw-rw-   0        0        0     9025 2023-04-11 17:30:01.000000 aioabcpapi-1.1.4/aioabcpapi/utils/payload.py
+drwxrwxrwx   0        0        0        0 2023-04-16 16:41:09.303685 aioabcpapi-1.1.4/aioabcpapi.egg-info/
+-rw-rw-rw-   0        0        0     5341 2023-04-16 16:41:08.000000 aioabcpapi-1.1.4/aioabcpapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      894 2023-04-16 16:41:09.000000 aioabcpapi-1.1.4/aioabcpapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 16:41:08.000000 aioabcpapi-1.1.4/aioabcpapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-04-16 16:41:08.000000 aioabcpapi-1.1.4/aioabcpapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       56 2023-04-16 16:41:08.000000 aioabcpapi-1.1.4/aioabcpapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      206 2023-04-16 16:41:09.416548 aioabcpapi-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1333 2023-04-16 16:40:20.000000 aioabcpapi-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 16:41:09.413549 aioabcpapi-1.1.4/test/
+-rw-rw-rw-   0        0        0    15807 2022-08-10 22:50:42.000000 aioabcpapi-1.1.4/test/test_payload.py
```

### Comparing `aioabcpapi-1.1.3/LICENSE` & `aioabcpapi-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aioabcpapi-1.1.3/PKG-INFO` & `aioabcpapi-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioabcpapi
-Version: 1.1.3
+Version: 1.1.4
 Summary: Async library for ABCP API
 Home-page: https://github.com/bl4ckm45k/aioabcpapi
 Author: bl4ckm45k
 Author-email: nonpowa@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `aioabcpapi-1.1.3/README.md` & `aioabcpapi-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `aioabcpapi-1.1.3/aioabcpapi/__init__.py` & `aioabcpapi-1.1.4/aioabcpapi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,9 +6,9 @@
                          AbcpParameterRequired, TeaPot)
 
 if sys.version_info < (3, 7):
     raise RuntimeError('Your Python version {0} is not supported, please install '
                        'Python 3.7+'.format('.'.join(map(str, sys.version_info[:3]))))
 
 __author__ = 'bl4ckm45k'
-__version__ = '1.1.3'
+__version__ = '1.1.4'
 __email__ = 'nonpowa@gmail.com'
```

### Comparing `aioabcpapi-1.1.3/aioabcpapi/api.py` & `aioabcpapi-1.1.4/aioabcpapi/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,20 +169,20 @@
             CREATE_USER: str = 'cp/user/new'
             GET_PROFILES: str = 'cp/users/profiles'
             EDIT_PROFILE: str = 'cp/users/profile'
 
             EDIT_USER: str = 'cp/user'
 
             GET_USER_SHIPMENT_ADDRESS: str = 'cp/user/shipmentAddresses'
-            GET_USER_SHIPMENT_ADDRESS_ZONES: str = '/cp/user/shipmentAddressZones'
-            GET_USER_SHIPMENT_ADDRESS_ZONE: str = '/cp/user/shipmentAddressZones/{}'
-            UPDATE_SHIPMENT_ZONES: str = '/cp/user/shipmentAddressZones'
-            CREATE_SHIPMENT_ZONE: str = '/cp/user/shipmentAddressZones/new'
-            UPDATE_SHIPMENT_ZONE: str = '/cp/user/shipmentAddressZones/{}/update'
-            DELETE_SHIPMENT_ZONE: str = '/cp/user/shipmentAddress/{}/delete'
+            GET_USER_SHIPMENT_ADDRESS_ZONES: str = 'cp/user/shipmentAddressZones'
+            GET_USER_SHIPMENT_ADDRESS_ZONE: str = 'cp/user/shipmentAddressZones/{}'
+            UPDATE_SHIPMENT_ZONES: str = 'cp/user/shipmentAddressZones'
+            CREATE_SHIPMENT_ZONE: str = 'cp/user/shipmentAddressZones/new'
+            UPDATE_SHIPMENT_ZONE: str = 'cp/user/shipmentAddressZones/{}/update'
+            DELETE_SHIPMENT_ZONE: str = 'cp/user/shipmentAddress/{}/delete'
             # Garage
             GET_USERS_CARS: str = 'cp/garage'
             SMS_SETTINGS: str = 'cp/user/smsSettings'
 
         @dataclass(frozen=True)
         class Staff:
             GET_STAFF: str = 'cp/managers'
@@ -336,30 +336,31 @@
             MASS_CANCEL: str = 'ts/positions/massCancel'
 
     class TsAdmin:
         @dataclass(frozen=True)
         class OrderPickings:
             FAST_GET_OUT: str = 'cp/ts/orderPickings/fastGetOut'
             GET: str = 'cp/ts/orderPickings/get'
-            GET_GOODS: str = '/cp/ts/orderPickings/getGoods'
-            CREATE_BY_OLD_POS: str = '/cp/ts/orderPickings/createByOldPos'
-            CHANGE_STATUS: str = '/cp/ts/orderPickings/changeStatus'
-            UPDATE: str = '/cp/ts/orderPickings/update'
-            DELETE_POSITION: str = '/cp/ts/orderPickings/deletePosition'
+            GET_GOODS: str = 'cp/ts/orderPickings/getGoods'
+            CREATE_BY_OLD_POS: str = 'cp/ts/orderPickings/createByOldPos'
+            CHANGE_STATUS: str = 'cp/ts/orderPickings/changeStatus'
+            UPDATE: str = 'cp/ts/orderPickings/update'
+            DELETE_POSITION: str = 'cp/ts/orderPickings/deletePosition'
 
         @dataclass(frozen=True)
         class CustomerComplaints:
             GET: str = 'cp/ts/customerComplaints/get'
-            GET_POSITIONS: str = '/cp/ts/customerComplaints/getPositions'
+            GET_POSITIONS: str = 'cp/ts/customerComplaints/getPositions'
             CREATE: str = 'cp/ts/customerComplaints/create'
             CREATE_POSITION: str = 'cp/ts/customerComplaints/createPosition'
             CREATE_POSITION_MULTIPLE: str = 'cp/ts/customerComplaints/createPositionMultiple'
             UPDATE_POSITION: str = 'cp/ts/customerComplaints/updatePosition'
             CHANGE_STATUS_POSITION: str = 'cp/ts/customerComplaints/changeStatusPosition'
             UPDATE: str = 'cp/ts/customerComplaints/update'
+            UPDATE_CUSTOM_FILE: str = 'cp/ts/customerComplaints/updateCustomFile'
 
         @dataclass(frozen=True)
         class DistributorOwners:
             DISTRIBUTOR_OWNERS: str = 'cp/ts/distributorOwners'
 
         @dataclass(frozen=True)
         class Orders:
@@ -428,14 +429,23 @@
 
         @dataclass(frozen=True)
         class TagsRelationships:
             LIST: str = 'cp/ts/tagsRelationships/list'
             CREATE: str = 'cp/ts/tagsRelationships/create'
             DELETE: str = 'cp/ts/tagsRelationships/delete'
 
+        @dataclass(frozen=True)
+        class Payments:
+            GET_LIST: str = 'cp/ts/payments/list'
+            CREATE: str = 'cp/ts/payments/create'
+
+        @dataclass(frozen=True)
+        class PaymentMethods:
+            METHODS_LIST: str = 'cp/ts/paymentMethods/list'
+
     class VinQu:
         pass
 
     class TecDoc:
         pass
```

### Comparing `aioabcpapi-1.1.3/aioabcpapi/base.py` & `aioabcpapi-1.1.4/aioabcpapi/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,30 +16,32 @@
 logger = logging.getLogger('base')
 
 
 class BaseAbcp:
 
     def __init__(
             self,
-            host: str = None,
-            login: str = None,
-            password: str = None,
+            host: str,
+            login: str,
+            password: str,
             loop: Optional[Union[asyncio.BaseEventLoop, asyncio.AbstractEventLoop]] = None,
             connections_limit: int = None,
             timeout: Optional[Union[int, float, aiohttp.ClientTimeout]] = None,
     ):
-        """ You can get API host name, login, password here: https://cp.abcp.ru/?page=allsettings&systemsettings&apiInformation
+        """Для получения доступа к API если вы являетесь администратором, перейдите в ПУ.
 
-        :param host: host name from ABCP
-        :type host: 'str'
-        :param login: login from ABCP
-        :type login: 'str'
-        :param password: password from ABCP
-        :type password: 'str' (md5 hash)
+        https://cp.abcp.ru/?page=allsettings&systemsettings&apiInformation
+
+        Если вы являетесь клиентом, запросите доступ у вашего менеджера.
+
+        :param host: Хост
+        :param login: Логин
+        :param password: MD5-пароль
         :raise: when host, login or password is invalid
+        :return: Объект класса
         """
 
         self._main_loop = loop
         # Authentication
 
         self._host = host
         self._login = login
@@ -62,15 +64,15 @@
     async def _get_new_session(self) -> aiohttp.ClientSession:
         return aiohttp.ClientSession(
             connector=self._connector_class(**self._connector_init),
             json_serialize=json.dumps
         )
 
     @property
-    def loop(self) -> Optional[asyncio.AbstractEventLoop]:
+    def _loop(self) -> Optional[asyncio.AbstractEventLoop]:
         return self._main_loop
 
     async def _get_session(self) -> Optional[aiohttp.ClientSession]:
         if self._session is None or self._session.closed:
             self._session = await self._get_new_session()
 
         if not self._session._loop.is_running():
@@ -89,22 +91,22 @@
     def __payload_check(self, payload):
         if isinstance(payload, dict):
             payload['userlogin'] = self._login
             payload['userpsw'] = self._password
         elif isinstance(payload, FormData):
             payload.add_field('userlogin', self._login)
             payload.add_field('userpsw', self._password)
-        if payload is None:
+        elif payload is None:
             payload = {'userlogin': self._login, 'userpsw': self._password}
         return payload
 
     async def _request(self, method: str,
                        payload: Union[Dict, FormData] = None, post: bool = False, **kwargs) -> Union[List, Dict, bool]:
         """
-        Make an _request to ABCP API
+        Make an request to ABCP API
 
         https://www.abcp.ru/wiki/API:Docs
 
         :param method: API method
         :type method: :obj:`str`
         :param payload: _request parameters
         :type payload: :obj:`dict`
```

### Comparing `aioabcpapi-1.1.3/aioabcpapi/cp/admin.py` & `aioabcpapi-1.1.4/aioabcpapi/cp/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,19 @@
 
 logging.basicConfig(level=logging.DEBUG)
 logger = logging.getLogger('Cp.Admin')
 
 
 class AdminApi(BaseAbcp):
     def __init__(self, *args):
+        """
+        Класс содержит методы административного интерфейса
+
+        https://www.abcp.ru/wiki/API.ABCP.Admin
+        """
         super().__init__(*args)
         self.orders = Orders(*args)
         self.finance = Finance(*args)
         self.users = Users(*args)
         self.staff = Staff(*args)
         self.statuses = Statuses(*args)
         self.distributors = Distributors(*args)
@@ -42,27 +47,29 @@
             numbers: Union[str, int, List] = None,
             internal_numbers: Optional[List] = None,
             status_code: Union[str, int, List] = None,
             office_id: Union[int, str] = None,
             distributor_order_id: Union[int, str] = None,
             is_canceled: Union[int, str] = None,
             distributor_id: Union[str, int, List] = None,
+            user_id: Union[int, str] = None,
             with_deleted: Union[str, bool] = None,
             format: Optional[str] = None,
             limit: Optional[int] = None,
             skip: Optional[int] = None,
             desc: Optional[bool] = None
 
     ):
         """Принимает в качестве параметров условия фильтрации заказов. Возвращает список заказов (в т.ч. список позиций заказа).
 
         Source: https://www.abcp.ru/wiki/API.ABCP.Admin#.D0.9F.D0.BE.D0.BB.D1.83.D1.87.D0.B5.D0.BD.D0.B8.D0.B5_.D1.81.D0.BF.D0.B8.D1.81.D0.BA.D0.B0_.D0.B7.D0.B0.D0.BA.D0.B0.D0.B7.D0.BE.D0.B2
 
 
 
+        :param user_id: Идентификатор клиента (покупателя). В результате вернутся все заказы, сделанные указанным клиентом.
         :param date_created_start: Начальная дата размещения заказа `str` в формате %Y-%m-%d %H:%M:%S  или datetime object
         :type date_created_start: `str` or `datetime`
         :param date_created_end: Конечная дата размещения заказа
         :type date_created_end: `str` or `datetime`
         :param date_updated_start: Начальная дата последнего обновления заказа в формате `str` в формате %Y-%m-%d %H:%M:%S  или datetime object
         :type date_updated_start: `str` or `datetime`
         :param date_updated_end: Конечная дата последнего обновления заказа в формате `str` в формате %Y-%m-%d %H:%M:%S  или datetime object
@@ -112,14 +119,16 @@
                 'Параметр "format" должен принимать одно из значений ["additional", "short", "count", "status_only", "p"]')
         if limit is not None and not 1 <= int(limit) <= 1000:
             raise AbcpAPIError(f'The limit must be more than {limit}')
         if isinstance(status_code, (int, str)):
             status_code = [status_code]
         if not isinstance(numbers, list) and numbers is not None:
             numbers = [numbers]
+        if isinstance(user_id, str) and not user_id.isdigit():
+            raise AbcpAPIError(f'Параметр user_id должен быть числом')
         payload = generate_payload(**locals())
 
         return await self._request(api.Methods.Admin.Orders.GET_ORDERS_LIST, payload)
 
     async def get_order(
             self,
             number: Union[int, str] = None,
@@ -802,14 +811,15 @@
             date_updated_start: Union[str, datetime] = None,
             date_updated_end: Union[str, datetime] = None,
             state: Union[str, int] = None,
             customer_status: Union[str, int] = None,
             customers_ids: Union[List, str, int] = None,
             market_type: Union[str, int] = None,
             phone: Union[str, int] = None,
+            enable_sms: Union[str, bool] = None,
             email: str = None,
             safe_mode: Union[str, int] = None,
             format: str = None,
             limit: Optional[int] = None,
             skip: Optional[int] = None,
             desc: Union[str, bool] = 'false'
     ):
@@ -833,14 +843,15 @@
         :type customer_status: int or str
         :param customers_ids: Массив идентификаторов покупателей
         :type customers_ids: List of str or int
         :param market_type: Тип регистрации. Значения:  1 - Розница 2 - Опт
         :type market_type: int or str
         :param phone: Номер телефона клиента
         :type phone: str 79998887766
+        :param enable_sms: Производится ли отпровка SMS клиенту
         :param email: E-mail клиента
         :type email: str
         :param safe_mode: "Безопасный режим" для клиентов не имеющих поддержки формата JSON.
                 Может принимать значения 0 или 1. При включении (1), адреса доставки в ответе будут возвращаться в виде
                 массива объектов с полями "id" и "name", а не как "ключ - значение".
         :type safe_mode: int or str
         :param format: 	Формат ответа. Доступные значения: p - заказы содержатся в поле items,
@@ -866,14 +877,16 @@
         if isinstance(date_updated_end, datetime):
             date_updated_end = f'{date_updated_end:%Y-%m-%d %H:%M:%S}'
 
         if isinstance(format, str) and format != 'p':
             raise AbcpWrongParameterError('The parameter "format" can only take the value "p" or None')
         if not isinstance(customers_ids, list) and customers_ids is not None:
             customers_ids = [customers_ids]
+        if isinstance(enable_sms, str) and (enable_sms != 'true' and enable_sms != 'false'):
+            raise AbcpAPIError('Параметр "enable_sms" должен быть булевым значением, либо строкой "true" или "false"')
         payload = generate_payload(**locals())
         return await self._request(api.Methods.Admin.Users.GET_USERS_LIST, payload)
 
     async def create(
             self,
             market_type: Union[str, int],
             name: str, password: str,
@@ -1026,15 +1039,15 @@
     async def edit(
             self,
             user_id: Union[str, int], business: Union[str, int] = None,
             email: str = None, name: str = None, second_name: str = None,
             surname: str = None, password: str = None,
             birth_date: Union[str, datetime] = None, city: str = None,
             mobile: Union[str, int] = None, icq: str = None,
-            skype: str = None, state: Union[str, int] = None,
+            skype: str = None, enable_sms: Union[bool, str] = None, state: Union[str, int] = None,
             profile_id: Union[int, str] = None, organization_name: str = None,
             organization_form: str = None, organization_official_name: str = None,
             inn: Union[str, int] = None, kpp: Union[str, int] = None, ogrn: Union[str, int] = None,
             bank_name: str = None, bik: Union[str, int] = None,
             correspondent_account: Union[str, int] = None, organization_account: Union[str, int] = None,
             delivery_address: Union[List[Dict], Dict] = None, baskets: Union[List[Dict], Dict] = None,
             baskets_delivery_address: Union[List[Dict], Dict] = None, comment: str = None,
@@ -1065,14 +1078,15 @@
         :param surname: Фамилия
         :param password: Необязательный параметр. Предназначен для изменения пароля пользователя
         :param birth_date:Дата рождения `str` в формате %Y-%m-%d  или datetime object
         :param city: Город
         :param mobile: Номер мобильного телефона
         :param icq:	ICQ UIN
         :param skype: Skype
+        :param enable_sms: Производится ли отпровка SMS клиенту
         :param state: Состояние аккаунта. Значения: от -1 до 2
         :param profile_id: Идентификатор профиля
         :param organization_name: Наименование организации
         :param organization_form: Правовая форма организации.
         :param organization_official_name: Наименование по регистрации (без правовой формы юр. лица)
         :param bank_name: Наименование банка
         :param bik: БИК банка
@@ -1095,14 +1109,16 @@
         :param pickup_state: Запрет самовывоза для клиента. 0 - запретить самовывоз, 1- разрешить самовывоз. Параметр актуален только если у вас на сайте включена опция: "Корзина: запрет самовывоза определенным клиентам".
         :return:
         """
         if isinstance(birth_date, datetime):
             birth_date = f'{birth_date:%Y-%m-%d}'
         if isinstance(pickup_state, bool):
             pickup_state = int(pickup_state)
+        if isinstance(enable_sms, str) and (enable_sms != 'true' and enable_sms != 'false'):
+            raise AbcpAPIError('Параметр "enable_sms" должен быть булевым значением, либо строкой "true" или "false"')
         payload = generate_payload(**locals())
         return await self._request(api.Methods.Admin.Users.EDIT_USER, payload, True)
 
     async def get_user_shipment_address(self, user_id: Union[int, str]):
         """
         Source: https://www.abcp.ru/wiki/API.ABCP.Admin#.D0.9F.D0.BE.D0.BB.D1.83.D1.87.D0.B5.D0.BD.D0.B8.D0.B5_.D1.81.D0.BF.D0.B8.D1.81.D0.BA.D0.B0_.D0.B0.D0.B4.D1.80.D0.B5.D1.81.D0.BE.D0.B2_.D0.B4.D0.BE.D1.81.D1.82.D0.B0.D0.B2.D0.BA.D0.B8
 
@@ -1217,32 +1233,38 @@
 
     async def update_manager(self, id: int, type_id: int = None,
                              first_name: str = None, last_name: str = None,
                              email: str = None, phone: str = None, mobile: str = None,
                              sip: Union[str, int] = None, comment: str = None, boss_id: int = None, office_id: int = None):
         """
 
-        :param id:
-        :param type_id:
-        :param first_name:
-        :param last_name:
-        :param email:
-        :param phone:
-        :param mobile:
-        :param SIP:
-        :param comment:
-        :param boss_id:
-        :param office_id:
+        Обновление данных сотрудника.
+
+        При изменении данных сотрудника необязательно передавать все параметры. Используйте в запросе только те данные, которые вы собираетесь изменить.
+
+        Source: https://www.abcp.ru/wiki/API.ABCP.Admin#.D0.9E.D0.B1.D0.BD.D0.BE.D0.B2.D0.BB.D0.B5.D0.BD.D0.B8.D0.B5_.D0.B4.D0.B0.D0.BD.D0.BD.D1.8B.D1.85_.D1.81.D0.BE.D1.82.D1.80.D1.83.D0.B4.D0.BD.D0.B8.D0.BA.D0.B0
+
+        :param id: Идентификатор сотрудника (обязательное поле)
+        :param type_id: Идентификатор должности сотрудника
+        :param first_name: Имя сотрудника
+        :param last_name: Фамилия сотрудника
+        :param email: Адрес ящика электронной почты
+        :param phone: Номер телефона
+        :param mobile: Номер мобильного телефона
+        :param sip: SIP номер
+        :param comment: Комментарий
+        :param boss_id: Идентификатор руководителя
+        :param office_id: Идентификатор офиса
         :return:
         """
         if isinstance(sip, str) and not sip.isdigit():
             raise AbcpWrongParameterError('Параметр "SIP" должен быть числом')
         payload = generate_payload(**locals())
         return await self._request(api.Methods.Admin.Staff.UPDATE_STAFF, payload, True)
-        pass
+
 
 class Statuses(BaseAbcp):
     async def get(self):
         """
         Source: https://www.abcp.ru/wiki/API.ABCP.Admin#.D0.9F.D0.BE.D0.BB.D1.83.D1.87.D0.B5.D0.BD.D0.B8.D0.B5_.D1.81.D0.BF.D0.B8.D1.81.D0.BA.D0.B0_.D1.81.D1.82.D0.B0.D1.82.D1.83.D1.81.D0.BE.D0.B2
         Возвращает список всех статусов позиций заказов.
         """
@@ -1564,15 +1586,15 @@
 
         if isinstance(article_only, bool):
             article_only = str(article_only).lower()
 
         if image_upload_mode == 1 and image_archive is None:
             raise AbcpWrongParameterError('Не передан архив с изображениями')
 
-        payload = generate_file_payload(exclude=['file', 'image_archive', 'catalog_id'], **locals())
+        payload = generate_file_payload(exclude=['file', 'image_archive', 'catalog_id'], max_size=100, **locals())
         return await self._request(api.Methods.Admin.UsersCatalog.UPLOAD.format(catalog_id), payload, True)
 
 
 class Payment(BaseAbcp):
     async def token(self, number: Union[str, int]):
         """
         Получение ссылки на оплату заказа
@@ -1594,8 +1616,8 @@
         :return:
         """
         if isinstance(client_id, str) and not client_id.isdigit():
             raise AbcpWrongParameterError('Параметр "client_id" должен быть числом')
         if isinstance(amount, str) and not amount.isdigit():
             raise AbcpWrongParameterError('Параметр "amount" должен быть числом')
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.Admin.Payment.TOP_BALANCE, payload)
+        return await self._request(api.Methods.Admin.Payment.TOP_BALANCE, payload)
```

### Comparing `aioabcpapi-1.1.3/aioabcpapi/cp/client.py` & `aioabcpapi-1.1.4/aioabcpapi/cp/client.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-1.1.3/aioabcpapi/ts/admin.py` & `aioabcpapi-1.1.4/aioabcpapi/ts/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import base64
 import logging
+import os
+from dataclasses import dataclass
 from datetime import datetime
-from typing import Union, List, Dict
+from typing import Union, List, Dict, Optional
 
 import pytz
 from pyrfc3339 import generate
 
 from .. import api
 from ..base import BaseAbcp
 from ..exceptions import AbcpWrongParameterError, AbcpParameterRequired
@@ -23,23 +25,25 @@
         self.distributor_owners = DistributorOwners(*args)
         self.orders = Orders(*args)
         self.cart = Cart(*args)
         self.positions = Positions(*args)
         self.good_receipts = GoodReceipts(*args)
         self.tags = Tags(*args)
         self.tags_relationships = TagsRelationships(*args)
+        self.payments = Payments(*args)
+        self.payment_methods = PaymentMethods(*args)
 
 
 class OrderPickings(BaseAbcp):
 
     async def fast_get_out(self, client_id: Union[str, int], supplier_id: Union[str, int],
                            positions: Union[List[Dict], Dict], distributor_id: Union[str, int] = None,
                            route_id: Union[str, int] = None, location_id: Union[str, int] = None,
                            order_picking_reseller_data: Dict = None,
-                           number: Union[str, int] = None, date: str = None,
+                           number: Union[str, int] = None, date: Union[datetime, str] = None,
                            ):
         """
         Операция быстрого создания заказа, приёмки, расхода
 
         Source: https://www.abcp.ru/wiki/API.TS.Admin#.D0.9E.D0.BF.D0.B5.D1.80.D0.B0.D1.86.D0.B8.D1.8F_.D0.B1.D1.8B.D1.81.D1.82.D1.80.D0.BE.D0.B3.D0.BE_.D1.81.D0.BE.D0.B7.D0.B4.D0.B0.D0.BD.D0.B8.D1.8F_.D0.B7.D0.B0.D0.BA.D0.B0.D0.B7.D0.B0.2C_.D0.BF.D1.80.D0.B8.D1.91.D0.BC.D0.BA.D0.B8.2C_.D1.80.D0.B0.D1.81.D1.85.D0.BE.D0.B4.D0.B0
 
 
@@ -227,15 +231,16 @@
 
     async def delete(self, id: int):
         payload = generate_payload(**locals())
         return await self._request(api.Methods.TsAdmin.OrderPickings.DELETE_POSITION, payload, True)
 
 
 class CustomerComplaints(BaseAbcp):
-    class FieldsChecker:
+    @dataclass
+    class _FieldsChecker:
         get_fields = ["orderPicking", "agreement", "tags", "posInfo"]
         get_positions_fields = ["item", "product", "location", "orderPickingInfo", "tags", "operationInfo",
                                 "supplierReturnPos"]
         update_fields = ["orderPicking", "agreement", "posInfo"]
 
     async def get(self, id: int = None, client_id: Union[int, str] = None, creator_id: Union[int, str] = None,
                   expert_id: Union[int, str] = None,
@@ -272,28 +277,28 @@
         if isinstance(date_end, datetime):
             date_end = generate(date_end.replace(tzinfo=pytz.utc))
         if isinstance(position_type, int) and (position_type < 1 or position_type > 3):
             raise AbcpWrongParameterError('position_type parameter must be between 1 and 3')
         if isinstance(position_statuses, list):
             position_statuses = ','.join(map(str, position_statuses))
         if fields is not None:
-            fields = check_fields(fields, self.FieldsChecker.get_fields)
+            fields = check_fields(fields, self._FieldsChecker.get_fields)
         payload = generate_payload(**locals())
         return await self._request(api.Methods.TsAdmin.CustomerComplaints.GET, payload)
 
     async def get_positions(self, op_id: Union[int, str] = None, order_picking_good_id: Union[int, str] = None,
                             order_picking_good_ids: Union[List, int] = None,
                             picking_ids: Union[List, int] = None,
                             old_co_position_ids: Union[List, int] = None,
                             client_id: Union[str, int] = None, old_item_id: Union[int, str] = None,
                             item_id: Union[int, str] = None,
                             tag_ids: Union[List, int] = None,
                             loc_id: Union[int, str] = None, status: int = None, type: int = None,
-                            date_start: str = None,
-                            date_end: str = None,
+                            date_start: Union[datetime, str] = None,
+                            date_end: Union[datetime, str] = None,
                             skip: int = None, limit: int = None,
                             sort: str = None, output: str = None,
                             fields: Union[List, str] = None):
         """
         Получение списка позиций операции возврата покупателя
 
         Source: https://www.abcp.ru/wiki/API.TS.Admin#.D0.9F.D0.BE.D0.BB.D1.83.D1.87.D0.B5.D0.BD.D0.B8.D0.B5_.D1.81.D0.BF.D0.B8.D1.81.D0.BA.D0.B0_.D0.BF.D0.BE.D0.B7.D0.B8.D1.86.D0.B8.D0.B9_.D0.BE.D0.BF.D0.B5.D1.80.D0.B0.D1.86.D0.B8.D0.B8_.D0.B2.D0.BE.D0.B7.D0.B2.D1.80.D0.B0.D1.82.D0.B0_.D0.BF.D0.BE.D0.BA.D1.83.D0.BF.D0.B0.D1.82.D0.B5.D0.BB.D1.8F
@@ -335,15 +340,15 @@
         if isinstance(tag_ids, list):
             tag_ids = ','.join(map(str, tag_ids))
         if isinstance(status, int) and not 1 <= status <= 8:
             raise AbcpWrongParameterError('Параметр "status" должен быть в диапазоне от 1 до 8')
         if isinstance(type, int) and not 1 <= type <= 3:
             raise AbcpWrongParameterError('Параметр "type" должен быть в диапазоне от 1 до 3')
         if fields is not None:
-            fields = check_fields(fields, self.FieldsChecker.get_positions_fields)
+            fields = check_fields(fields, self._FieldsChecker.get_positions_fields)
         payload = generate_payload(exclude=['old_item_id'], **locals())
         return await self._request(api.Methods.TsAdmin.CustomerComplaints.GET_POSITIONS, payload)
 
     async def create(self, order_picking_id: Union[str, int], positions: Union[List[Dict], Dict]):
         """
         Создание возврата покупателя
 
@@ -423,41 +428,66 @@
         """
         if not (1 <= status <= 8):
             raise AbcpWrongParameterError('Параметр "status" может принимать значения от 1 до 8')
         payload = generate_payload(**locals())
         return await self._request(api.Methods.TsAdmin.CustomerComplaints.CHANGE_STATUS_POSITION, payload, True)
 
     async def update(self, id: Union[str, int], number: int = None, expert_id: Union[int, str] = None,
-                     custom_complaint_file: str = None,
+                     custom_complaint_file: str = '',
                      fields: Union[List, str] = None):
         """
 
         :param id: [обязательный] идентификатор операции возврата покупателя
         :param number: [обязательный если не задан expert_id] уникальный номер операции
         :param expert_id: [обязательный если не задан number] идентификатор сотрудника-эксперта
-        :param custom_complaint_file: (Передавать путь к файлу) форма "Заявка на возврат", файл, передавать строкой в формате base64. Для удаления файла - указать пустую строку.
+        :param custom_complaint_file: (Передавать путь к файлу) форма "Заявка на возврат", файл, передавать строкой в формате base64. Если файл не передан, то будет удалён.
         :param fields: Расширенный формат вывода. Набор из следующих строк через запятую:
                         "orderPicking" - операция отгрузки, по которой создан возврат
                         "agreement" - договор, по которому выполнена отгрузка
                         "posInfo" - загрузка суммарной информации о позициях
         :return:
         """
-        if isinstance(custom_complaint_file, str):
+        if os.path.isfile(custom_complaint_file):
             with open(custom_complaint_file, "rb") as ccf:
                 encoded_string = base64.b64encode(ccf.read()).decode("utf-8")
             custom_complaint_file = f"{encoded_string}"
             del ccf
             del encoded_string
+        else:
+            raise TypeError('Неверно передан путь к файлу')
         if all(x is None for x in [number, expert_id]):
             raise AbcpParameterRequired('Один из параметров "number" или "expert_id" должен быть указан')
         if fields is not None:
-            fields = check_fields(fields, self.FieldsChecker.update_fields)
+            fields = check_fields(fields, self._FieldsChecker.update_fields)
         payload = generate_payload(**locals())
         return await self._request(api.Methods.TsAdmin.CustomerComplaints.UPDATE, payload, True)
 
+    async def update_custom_file(self, id: Union[int, str], custom_complaint_file: str = '',
+                                 fields: Union[List, str] = None):
+        """
+
+        :param id: идентификатор операции возврата покупателя
+        :param custom_complaint_file: (Передавать путь к файлу) форма "Заявка на возврат", файл, передавать строкой в формате base64. Если файл не передан, то будет удалён.
+        :param fields: [необязательный] Расширенный формат вывода
+        :return:
+        """
+        if os.path.isfile(custom_complaint_file):
+            with open(custom_complaint_file, "rb") as ccf:
+                encoded_string = base64.b64encode(ccf.read()).decode("utf-8")
+
+            custom_complaint_file = f"{encoded_string}"
+            del ccf
+            del encoded_string
+        else:
+            raise TypeError('Неверно передан путь к файлу')
+        if fields is not None:
+            fields = check_fields(fields, self._FieldsChecker.update_fields)
+        payload = generate_payload(**locals())
+        return await self._request(api.Methods.TsAdmin.CustomerComplaints.UPDATE_CUSTOM_FILE, payload, True)
+
 
 class DistributorOwners(BaseAbcp):
     async def distributor_owners(self, distributor_id: Union[str, int]):
         """
         Получение привязанного контрагента
 
         Source: https://www.abcp.ru/wiki/API.TS.Admin#.D0.9F.D0.BE.D0.BB.D1.83.D1.87.D0.B5.D0.BD.D0.B8.D0.B5_.D0.BF.D1.80.D0.B8.D0.B2.D1.8F.D0.B7.D0.B0.D0.BD.D0.BD.D0.BE.D0.B3.D0.BE_.D0.BA.D0.BE.D0.BD.D1.82.D1.80.D0.B0.D0.B3.D0.B5.D0.BD.D1.82.D0.B0
@@ -470,15 +500,15 @@
 
 
 class Orders(BaseAbcp):
     def __init__(self, *args):
         super().__init__(*args)
         self.messages = Messages(*args)
 
-    class FieldsChecker:
+    class _FieldsChecker:
         fields = ["deliveries", "agreement", "tags", "posInfo", "amounts"]
 
     async def create(self, client_id: Union[str, int], number: Union[int, str] = None,
                      agreement_id: Union[int, str] = None,
                      create_time: Union[datetime, str] = None, manager_id: Union[int, str] = None,
                      fields: Union[List, str] = None):
         """
@@ -493,29 +523,30 @@
         :param manager_id: Идентификатор сотрудника, ответственного за заказ
         :param fields: дополнительная информация ["agreement", "tags", "posInfo", "deliveries", "amounts"]
         :return:
         """
         if isinstance(create_time, datetime):
             create_time = generate(create_time.replace(tzinfo=pytz.utc))
         if fields is not None:
-            fields = check_fields(fields, self.FieldsChecker.fields)
+            fields = check_fields(fields, self._FieldsChecker.fields)
 
         payload = generate_payload(**locals())
         return await self._request(api.Methods.TsAdmin.Orders.CREATE, payload, True)
 
     async def create_by_cart(self, client_id: Union[str, int], agreement_id: Union[str, int],
                              positions: Union[List, int, str],
                              delivery_address: str, delivery_person: str, delivery_contact: str,
                              number: Union[int, str] = None,
-                             create_time: str = None, manager_id: Union[int, str] = None,
+                             create_time: Union[datetime, str] = None, manager_id: Union[int, str] = None,
                              delivery_method_id: Union[int, str] = None,
                              delivery_comment: str = None, delivery_employee_person: str = None,
                              delivery_employee_contact: str = None,
-                             delivery_reseller_comment: str = None, delivery_start_time: str = None,
-                             delivery_end_time: str = None,
+                             delivery_reseller_comment: str = None,
+                             delivery_start_time: Union[datetime, str] = None,
+                             delivery_end_time: Union[datetime, str] = None,
                              locale: str = None, fields: Union[List, str] = None
                              ):
         """
         Создание заказа по позициям корзины
 
         Source: https://www.abcp.ru/wiki/API.TS.Admin#.D0.A1.D0.BE.D0.B7.D0.B4.D0.B0.D0.BD.D0.B8.D0.B5_.D0.B7.D0.B0.D0.BA.D0.B0.D0.B7.D0.B0_.D0.BF.D0.BE_.D0.BF.D0.BE.D0.B7.D0.B8.D1.86.D0.B8.D1.8F.D0.BC_.D0.BA.D0.BE.D1.80.D0.B7.D0.B8.D0.BD.D1.8B
 
@@ -536,15 +567,15 @@
         :param delivery_start_time: время начала интервала доставки
         :param delivery_end_time: время конца интервала доставки
         :param locale: локаль для сохранения описаний товаров ru_RU
         :param fields: дополнительная информация ["agreement", "tags", "posInfo", "deliveries", "amounts"]
         :return:
         """
         if fields is not None:
-            fields = check_fields(fields, self.FieldsChecker.fields)
+            fields = check_fields(fields, self._FieldsChecker.fields)
         if isinstance(create_time, datetime):
             create_time = generate(create_time.replace(tzinfo=pytz.utc))
         if isinstance(delivery_start_time, datetime):
             delivery_start_time = generate(delivery_start_time.replace(tzinfo=pytz.utc))
         if isinstance(delivery_end_time, datetime):
             delivery_end_time = generate(delivery_end_time.replace(tzinfo=pytz.utc))
         if isinstance(positions, (int, str)):
@@ -558,17 +589,18 @@
         return await self._request(api.Methods.TsAdmin.Orders.CREATE_BY_CART, payload, True)
 
     async def orders_list(self, number: int = None,
                           agreement_id: Union[int, str] = None,
                           manager_id: Union[int, str] = None,
                           delivery_id: Union[int, str] = None,
                           message: str = None,
-                          date_start: str = None, date_end: str = None,
-                          update_date_start: str = None, update_date_end: str = None,
-                          deadline_date_start: str = None, deadline_date_end: str = None,
+                          date_start: Union[datetime, str] = None, date_end: Union[datetime, str] = None,
+                          update_date_start: Union[datetime, str] = None, update_date_end: Union[datetime, str] = None,
+                          deadline_date_start: Union[datetime, str] = None,
+                          deadline_date_end: Union[datetime, str] = None,
                           order_ids: Union[List, int] = None,
                           product_ids: Union[List, int] = None,
                           position_statuses: Union[List, int] = None,
                           skip: int = None,
                           limit: int = None):
         """
         Получение списка заказов
@@ -652,15 +684,15 @@
         :param client_id: Идентификатор клиента
         :param agreement_id: Идентификатор соглашения (договора)
         :param manager_id: Идентификатор сотрудника, ответственного за заказ
         :param fields: дополнительная информация ["agreement", "tags", "posInfo", "deliveries", "amounts"]
         :return:
         """
         if fields is not None:
-            fields = check_fields(fields, self.FieldsChecker.fields)
+            fields = check_fields(fields, self._FieldsChecker.fields)
         payload = generate_payload(**locals())
         return await self._request(api.Methods.TsAdmin.Orders.UPDATE, payload, True)
 
     async def merge(self, main_order_id: Union[str, int], merge_orders_ids: Union[List, str, int] = None,
                     fields: Union[List, str] = None):
         """
         Объединение заказов
@@ -671,15 +703,15 @@
         :param merge_orders_ids: массив, идентификаторы остальных заказов объединения
         :param fields: дополнительная информация
         :return:
         """
         if isinstance(merge_orders_ids, (int, str)):
             merge_orders_ids = [merge_orders_ids]
         if fields is not None:
-            fields = check_fields(fields, self.FieldsChecker.fields)
+            fields = check_fields(fields, self._FieldsChecker.fields)
         payload = generate_payload(**locals())
         return await self._request(api.Methods.TsAdmin.Orders.MERGE, payload, True)
 
     async def split(self, order_id: Union[str, int], position_ids: Union[List, str, int] = None,
                     fields: Union[List, str] = None):
 
         """
@@ -691,15 +723,15 @@
         :param position_ids: массив, идентификаторы отделяемых позиций заказа
         :param fields: дополнительная информация ["agreement", "tags", "posInfo", "deliveries", "amounts"]
         :return:
         """
         if isinstance(position_ids, (int, str)):
             position_ids = [position_ids]
         if fields is not None:
-            fields = check_fields(fields, self.FieldsChecker.fields)
+            fields = check_fields(fields, self._FieldsChecker.fields)
         payload = generate_payload(**locals())
         return await self._request(api.Methods.TsAdmin.Orders.SPLIT, payload, True)
 
     async def reprice(self, order_id: Union[str, int], new_sum: Union[float, int],
                       fields: Union[List, str] = None):
         """
         Изменение суммы заказа
@@ -708,15 +740,15 @@
 
         :param order_id: Идентификатор заказа клиента
         :param new_sum: новая сумма заказа
         :param fields: дополнительная информация ["agreement", "tags", "posInfo", "deliveries", "amounts"]
         :return:
         """
         if fields is not None:
-            fields = check_fields(fields, self.FieldsChecker.fields)
+            fields = check_fields(fields, self._FieldsChecker.fields)
         payload = generate_payload(**locals())
         return await self._request(api.Methods.TsAdmin.Orders.REPRICE, payload, True)
 
 
 class Messages(BaseAbcp):
     def __init__(self, *args):
         super().__init__(*args)
@@ -958,15 +990,15 @@
 
 
 class Positions(BaseAbcp):
     def __init__(self, *args):
         super().__init__(*args)
         self.messages = PositionsMessages(*args)
 
-    class FieldsChecker:
+    class _FieldsChecker:
         additional_info = ["reserv", "product", "orderPicking",
                            "customerComplaintPoses", "supplierOrder", "grPosition",
                            "order", "delivery", "tags", "unpaidAmount"]
         statuses = ["prepayment", "canceled", "new",
                     "supOrder", "supOrderCanceled", "reservation",
                     "orderPicking", "delivery", "finished"]
 
@@ -979,15 +1011,15 @@
         :param position_id: идентификатор позиции заказа
         :param additional_info: доп. информация позиции ["reserv", "product", "orderPicking",
                            "customerComplaintPoses", "supplierOrder", "grPosition",
                            "order", "delivery", "tags", "unpaidAmount"]
         :return:
         """
         if additional_info is not None:
-            additional_info = check_fields(additional_info, self.FieldsChecker.additional_info)
+            additional_info = check_fields(additional_info, self._FieldsChecker.additional_info)
 
         payload = generate_payload(**locals())
         return await self._request(api.Methods.TsAdmin.Positions.GET, payload)
 
     async def get_list(self, brand: str = None, message: str = None, agreement_id: Union[int, str] = None,
                        client_id: Union[int, str] = None,
                        manager_id: Union[int, str] = None,
@@ -1068,22 +1100,22 @@
             so_position_ids = [so_position_ids]
         if isinstance(route_ids, (int, str)):
             route_ids = [route_ids]
         if isinstance(distributor_ids, (int, str)):
             distributor_ids = [distributor_ids]
         if isinstance(ids, (int, str)):
             ids = [ids]
-        if isinstance(order_ids, (int, str)) :
+        if isinstance(order_ids, (int, str)):
             order_ids = [order_ids]
         if isinstance(statuses, str):
             statuses = [statuses]
         if isinstance(tag_ids, list):
             tag_ids = ','.join(map(str, tag_ids))
         if statuses is not None:
-            statuses = check_fields(statuses, self.FieldsChecker.statuses)
+            statuses = check_fields(statuses, self._FieldsChecker.statuses)
         payload = generate_payload(**locals())
         return await self._request(api.Methods.TsAdmin.Positions.GET_LIST, payload)
 
     async def create(self, order_id: Union[str, int], client_id: Union[str, int], route_id: Union[str, int],
                      distributor_id: Union[str, int], item_key: str,
                      quantity: Union[float, int], sell_price: Union[int, float],
                      brand: Union[str, int], number_fix: str, number: Union[int, str]):
@@ -1111,15 +1143,15 @@
     async def update(self, position_id: Union[str, int], route_id: Union[int, str] = None,
                      distributor_id: Union[int, str] = None,
                      quantity: Union[int, float] = None,
                      sell_price: Union[float, int] = None, cl_to_res_rate: Union[float, int] = None,
                      cl_sell_price: Union[float, int] = None,
                      price_data_sell_price: Union[float, int] = None,
                      prepayment_amount: Union[float, int] = None,
-                     deadline_time: str = None, deadline_time_max: str = None,
+                     deadline_time: Union[datetime, str] = None, deadline_time_max: Union[datetime, str] = None,
                      client_refusal: bool = None,
                      delivery_id: Union[int, str] = None,
                      status: str = None,
                      ):
         """
         Обновление позиции
 
@@ -1324,15 +1356,15 @@
 
     async def get(self, limit: int = None, skip: int = None,
                   output: str = None,
                   auto: str = None,
                   creator_id: Union[str, int] = None, worker_id: Union[str, int] = None,
                   agreement_id: str = None, statuses: Union[List, int] = None,
                   number: str = None,
-                  date_start: str = None, date_end: str = None,
+                  date_start: Union[datetime, str] = None, date_end: Union[datetime, str] = None,
                   sup_number: str = None):
         """
         Получение списка операций приёмки
 
         Source:
 
 
@@ -1664,13 +1696,85 @@
         if isinstance(tag_id, str) and not tag_id.isdigit():
             raise AbcpWrongParameterError('Параметр "tag_id" должен быть числом')
 
         if isinstance(object_id, str) and not object_id.isdigit():
             raise AbcpWrongParameterError('Параметр "object_id" должен быть числом')
 
         if isinstance(object_type, str) and object_type.isdigit():
-            if not 1 <= int(object_type) <= 13:
-                raise AbcpWrongParameterError('"object_type" must be in range 1-13')
+            object_type = int(object_type)
         if isinstance(object_type, int) and not 1 <= object_type <= 13:
             raise AbcpWrongParameterError('"object_type" must be in range 1-13')
         payload = generate_payload(**locals())
         return await self._request(api.Methods.TsAdmin.TagsRelationships.DELETE, payload, True)
+
+
+class Payments(BaseAbcp):
+    @dataclass(frozen=True)
+    class _Status:
+        status = ["new", "inProcess", "accepted", "rejected", "canceled"]
+
+    async def get_list(self,
+                       contractor_id: Union[str, int] = None, agreement_id: Union[str, int] = None,
+                       amount_start: Union[float, int, str] = None, amount_end: Union[float, int, str] = None,
+                       status: Union[List[str], str] = None,
+                       number: str = None,
+                       requisite_id: Union[str, int] = None,
+                       skip: int = None, limit: int = None,
+                       payment_type: Union[List[str], str] = None, payment_method_ids: Union[List[int], int] = None,
+                       date_start: Union[datetime, str] = None, date_end: Union[datetime, str] = None,
+                       fields: Union[List[str], str] = None):
+        if isinstance(date_start, datetime):
+            date_start = generate(date_start.replace(tzinfo=pytz.utc))
+        if isinstance(date_end, datetime):
+            date_end = generate(date_end.replace(tzinfo=pytz.utc))
+        if isinstance(status, list):
+            if any(x not in self._Status.status for x in status):
+                raise AbcpWrongParameterError(
+                    f'Неверный список статусов: {status} Допустимые статусы {self._Status.status}')
+            status = ','.join(status)
+        if isinstance(payment_method_ids, list):
+            payment_method_ids = ','.join(map(str, payment_method_ids))
+        if isinstance(payment_type, list):
+            payment_type = ','.join(payment_type)
+        payload = generate_payload(**locals())
+        return await self._request(api.Methods.TsAdmin.Payments.GET_LIST, payload)
+
+    async def create(self,
+                     payment_type: str, payment_method_id: int,
+                     agreement_id: int, author_id: int,
+                     amount: Union[float, int, str], date: Union[datetime, str],
+                     contractor_id: int = None, commission: Union[float, int] = None,
+                     comment: str = None, fields: Union[List[str], str] = None):
+        if isinstance(date, datetime):
+            date = generate(date.replace(tzinfo=pytz.utc))
+        if isinstance(fields, list):
+            fields = ','.join(fields)
+
+        payload = generate_payload(**locals())
+        return await self._request(api.Methods.TsAdmin.Payments.CREATE, payload)
+
+
+class PaymentMethods(BaseAbcp):
+    @dataclass(frozen=True)
+    class _Fields:
+        allow_change_param = ["yes", "no", "paymentInterfaceOnly", "editOnly"]
+
+    async def get_list(self,
+                       payment_type: Optional[str] = None,
+                       allow_change_payment: Optional[str] = None,
+                       state: Optional[str] = None):
+        """
+        Получение списка способов оплаты
+
+        Source: https://www.abcp.ru/wiki/API.TS.Admin#.D0.9F.D0.BE.D0.BB.D1.83.D1.87.D0.B5.D0.BD.D0.B8.D0.B5_.D1.81.D0.BF.D0.B8.D1.81.D0.BA.D0.B0_.D1.81.D0.BF.D0.BE.D1.81.D0.BE.D0.B1.D0.BE.D0.B2_.D0.BE.D0.BF.D0.BB.D0.B0.D1.82.D1.8B
+
+        :param payment_type: Тип оплаты
+        :param allow_change_payment: Вариант доступности изменения платежа
+        :param state: Состояние
+        :return:
+        """
+        if isinstance(allow_change_payment, str) and allow_change_payment not in self._Fields.allow_change_param:
+            raise AbcpWrongParameterError(f'Неверное значение параметра "allow_change_payment" {allow_change_payment}.'
+                                          f'Допустимые значения {self._Fields.allow_change_param}')
+
+        payload = generate_payload(**locals())
+        return await self._request(api.Methods.TsAdmin.PaymentMethods.METHODS_LIST, payload)
```

### Comparing `aioabcpapi-1.1.3/aioabcpapi/ts/client.py` & `aioabcpapi-1.1.4/aioabcpapi/ts/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -261,15 +261,15 @@
                             date_end: Union[str, datetime] = None,
                             type: Union[str, int] = None, skip: int = None, limit: int = None,
                             output: str = None, fields: Union[List, str] = None
                             ):
         """
         Получение списка позиций возврата покупателя
 
-        Source:
+        Source: https://www.abcp.ru/wiki/API.TS.Client#.D0.9F.D0.BE.D0.BB.D1.83.D1.87.D0.B5.D0.BD.D0.B8.D0.B5_.D1.81.D0.BF.D0.B8.D1.81.D0.BA.D0.B0_.D0.BF.D0.BE.D0.B7.D0.B8.D1.86.D0.B8.D0.B9_.D0.B2.D0.BE.D0.B7.D0.B2.D1.80.D0.B0.D1.82.D0.B0_.D0.BF.D0.BE.D0.BA.D1.83.D0.BF.D0.B0.D1.82.D0.B5.D0.BB.D1.8F
 
         :param op_id: идентификатор операции
         :param order_picking_good_id: идентификатор позиции отгрузки
         :param order_picking_good_ids: идентификаторы позиций расхода через запятую
         :param picking_ids:  идентификаторы операции расхода через запятую
         :param old_co_position_ids: Идентификаторы позиции заказа через запятую.
         :param old_item_id: идентификатор партии из отгрузки
@@ -278,15 +278,19 @@
         :param status:  статус позиции (1 - новый, 2 - в работе, 3 - отказ, 4 - подтверждён, 5 - выдано, 6 - аннулировано)
         :param date_start: Начальная дата диапазона поиска `str` в формате RFC3339 или datetime object
         :param date_end: Конечная дата диапазона поиска `str` в формате RFC3339 или datetime object
         :param type:тип возврата (1 - возврат, 2 - отказ, 3 - брак.)
         :param skip: количество операций в ответе, которое нужно пропустить
         :param limit: максимальное количество операций, которое должно быть возвращено в ответе. Максимально возможное значение 1000. Если не указан будет установлено максимально возможное значение.
         :param output:  формат вывода, 'e' - загрузка дополнительной информации (справочные товары)
-        :param fields: # TODO Check parameters contains only ['orderPickingInfo', 'product', 'operationInfo', 'supplierReturnPos]
+        :param fields: [необязательный] Загрузка дополнительной информации. Строка со следующими параметрами через запятую:
+                        product - товар из справочника
+                        orderPickingInfo - операция расхода; позиция расхода, связанная с возвратом; доступное для возврата количество
+                        operationInfo - информация об операции
+                        supplierReturnPos - связанный возврат поставщику (null, если такого нет)
         :return:
         """
         if isinstance(order_picking_good_ids, list):
             order_picking_good_ids = ','.join(map(str, order_picking_good_ids))
 
         if isinstance(picking_ids, list):
             picking_ids = ','.join(map(str, picking_ids))
```

### Comparing `aioabcpapi-1.1.3/aioabcpapi/utils/fields_checker.py` & `aioabcpapi-1.1.4/aioabcpapi/utils/fields_checker.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-1.1.3/aioabcpapi/utils/payload.py` & `aioabcpapi-1.1.4/aioabcpapi/utils/payload.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import logging
+import os
 from io import BufferedReader
 
 from aiohttp import FormData
 
+from aioabcpapi.exceptions import FileSizeExceeded
+
 DEFAULT_FILTER = ['self', 'cls', 'kwargs']
 logger = logging.getLogger('utils/payload')
 
 
 def get_pascal_case_key(key: str):
     return ''.join([*map(str.title, key.split('_'))])
 
@@ -188,29 +191,33 @@
                             data[f'positions[{z}][{key_z}]'] = value_z
                         else:
                             data[f'positions[{z}][positionParams][{key_z}]'] = value_z
     logger.debug(f'{data}')
     return data
 
 
-def generate_file_payload(exclude=None, **kwargs):
+def generate_file_payload(exclude=None, max_size: int = None, **kwargs):
     """
     Generate payload
     :param exclude:
+    :param max_size: Максимальный размер в Мб
     :param kwargs:
     :return: :obj:`aiohttp.FormData`
     """
     if exclude is None:
         exclude = []
     data = FormData()
     for key, value in kwargs.items():
         if key not in exclude + DEFAULT_FILTER and value is not None and not key.startswith('_'):
             data.add_field(get_camel_case_key(key), str(value))
         if key in exclude and key != '' and value is not None:
             if isinstance(value, BufferedReader):
                 data.add_field(get_camel_case_key(key), value, filename=value.name, content_type='multipart/form-data')
             if isinstance(value, str) and not value.isdigit():
                 with open(value, 'rb') as file:
+                    if max_size is not None:
+                        size = file.seek(0, os.SEEK_END)
+                        if (size / 1_048_576) > max_size: raise FileSizeExceeded('Файл не может быть больше 100 Мб')
                     data.add_field(get_camel_case_key(key), file, filename=file.name,
                                    content_type='multipart/form-data')
     logger.debug(f'{data}')
     return data
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aioabcpapi-1.1.3/aioabcpapi.egg-info/PKG-INFO` & `aioabcpapi-1.1.4/aioabcpapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioabcpapi
-Version: 1.1.3
+Version: 1.1.4
 Summary: Async library for ABCP API
 Home-page: https://github.com/bl4ckm45k/aioabcpapi
 Author: bl4ckm45k
 Author-email: nonpowa@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `aioabcpapi-1.1.3/aioabcpapi.egg-info/SOURCES.txt` & `aioabcpapi-1.1.4/aioabcpapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aioabcpapi-1.1.3/setup.py` & `aioabcpapi-1.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 if sys.version_info < (3, 7):
     raise RuntimeError('Your Python version {0} is not supported, please install '
                        'Python 3.7+'.format('.'.join(map(str, sys.version_info[:3]))))
 requirements = ["aiohttp>=3.8.3", "certifi>=2022.12.7", "ujson>=5.7.0", "pytz>=2022.7.1", "pyrfc3339"]
 
 setup(
     name='aioabcpapi',
-    version='1.1.3',
+    version='1.1.4',
     author='bl4ckm45k',
     author_email='nonpowa@gmail.com',
     description='Async library for ABCP API',
     long_description_content_type="text/markdown",
     url="https://github.com/bl4ckm45k/aioabcpapi",
     license="MIT",
     packages=['aioabcpapi', 'aioabcpapi/cp', 'aioabcpapi/ts', 'aioabcpapi/utils'],
```

### Comparing `aioabcpapi-1.1.3/test/test_payload.py` & `aioabcpapi-1.1.4/test/test_payload.py`

 * *Files identical despite different names*

