# Comparing `tmp/haki_crawler-0.4.tar.gz` & `tmp/haki_crawler-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haki_crawler-0.4.tar", last modified: Sun Apr 16 10:34:57 2023, max compression
+gzip compressed data, was "haki_crawler-0.5.tar", last modified: Sun Apr 16 11:00:49 2023, max compression
```

## Comparing `haki_crawler-0.4.tar` & `haki_crawler-0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-16 10:34:57.812462 haki_crawler-0.4/
--rw-r--r--   0 admin      (501) staff       (20)      616 2023-04-16 10:34:57.812179 haki_crawler-0.4/PKG-INFO
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-16 10:34:57.809854 haki_crawler-0.4/haki_crawler/
--rw-r--r--   0 admin      (501) staff       (20)        0 2023-04-16 10:09:24.000000 haki_crawler-0.4/haki_crawler/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     6115 2023-04-16 10:32:48.000000 haki_crawler-0.4/haki_crawler/sensortower.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-16 10:34:57.811756 haki_crawler-0.4/haki_crawler.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)      616 2023-04-16 10:34:57.000000 haki_crawler-0.4/haki_crawler.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      240 2023-04-16 10:34:57.000000 haki_crawler-0.4/haki_crawler.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2023-04-16 10:34:57.000000 haki_crawler-0.4/haki_crawler.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) staff       (20)        9 2023-04-16 10:34:57.000000 haki_crawler-0.4/haki_crawler.egg-info/requires.txt
--rw-r--r--   0 admin      (501) staff       (20)       13 2023-04-16 10:34:57.000000 haki_crawler-0.4/haki_crawler.egg-info/top_level.txt
--rw-r--r--   0 admin      (501) staff       (20)       38 2023-04-16 10:34:57.812570 haki_crawler-0.4/setup.cfg
--rw-r--r--   0 admin      (501) staff       (20)     1221 2023-04-16 10:32:58.000000 haki_crawler-0.4/setup.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-16 11:00:49.582330 haki_crawler-0.5/
+-rw-r--r--   0 admin      (501) staff       (20)      616 2023-04-16 11:00:49.582074 haki_crawler-0.5/PKG-INFO
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-16 11:00:49.579192 haki_crawler-0.5/haki_crawler/
+-rw-r--r--   0 admin      (501) staff       (20)        0 2023-04-16 10:09:24.000000 haki_crawler-0.5/haki_crawler/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     7737 2023-04-16 11:00:30.000000 haki_crawler-0.5/haki_crawler/sensortower.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-16 11:00:49.581553 haki_crawler-0.5/haki_crawler.egg-info/
+-rw-r--r--   0 admin      (501) staff       (20)      616 2023-04-16 11:00:49.000000 haki_crawler-0.5/haki_crawler.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)      240 2023-04-16 11:00:49.000000 haki_crawler-0.5/haki_crawler.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2023-04-16 11:00:49.000000 haki_crawler-0.5/haki_crawler.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) staff       (20)        9 2023-04-16 11:00:49.000000 haki_crawler-0.5/haki_crawler.egg-info/requires.txt
+-rw-r--r--   0 admin      (501) staff       (20)       13 2023-04-16 11:00:49.000000 haki_crawler-0.5/haki_crawler.egg-info/top_level.txt
+-rw-r--r--   0 admin      (501) staff       (20)       38 2023-04-16 11:00:49.582422 haki_crawler-0.5/setup.cfg
+-rw-r--r--   0 admin      (501) staff       (20)     1221 2023-04-16 11:00:41.000000 haki_crawler-0.5/setup.py
```

### Comparing `haki_crawler-0.4/PKG-INFO` & `haki_crawler-0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haki_crawler
-Version: 0.4
+Version: 0.5
 Summary: A short description of your package
 Home-page: https://example.com
 Author: namhn1495
 Author-email: namhn1495@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `haki_crawler-0.4/haki_crawler/sensortower.py` & `haki_crawler-0.5/haki_crawler/sensortower.py`

 * *Files 13% similar despite different names*

```diff
@@ -167,16 +167,61 @@
     url = f"https://api.sensortower.com/v1/android/usage/{usage_type}"
 
     # Send the request to the API and return the response
     response = requests.request("GET", url, headers=headers, params=params)
     return response.json()
 
 
-# cookie = requests.get('http://localhost:3000/sensortower')
-# cookie = cookie.json()
-# cookie = {
-#     "session": "2e8e2b1cfd6d791d55b235e53066f7a3",
-#     "device_id": "446def50-8494-487a-ab39-d8d965f014d2",
-# }
+def advanced_search(cookie, custom_filter_id, term, limit=250, country='US', auth_token='your_auth_token'):
+    """
+    This function performs an advanced search on the Sensor Tower website.
 
-# result = usages(cookie=cookie)
-# print(json.dumps(result, indent=2))
+    Args:
+    - cookie (str): The value of the 'session' cookie needed to authenticate the request.
+    - custom_filter_id (str): The ID of the custom filter to use for the search.
+    - term (str): The search term to use for the search.
+    - limit (int): The maximum number of results to return. Defaults to 250.
+
+    Returns:
+    - response (requests.Response): A response object containing the data retrieved from the search.
+    """
+
+    # Extract session and device_id from the cookie
+    session = cookie['session']
+    device_id = cookie['device_id']
+
+    # Set the URL and parameters for the request
+    url = "https://app.sensortower.com/advanced_search"
+    params = {
+        'country': country,
+        'auth_token': auth_token,
+        'device_type': 'android',
+        'entity_type': 'app',
+        'os': 'android',
+        'search_fields[]': ['name', 'short_description'],
+        'custom_fields_filter_id': custom_filter_id,
+        'term': term,
+        'limit': limit
+    }
+
+    # Set the headers for the request
+    headers = {
+        'Cookie': f'session={session}; device_id={device_id}'
+    }
+
+    # Send the request to the Sensor Tower website and return the response
+    response = requests.request("GET", url, headers=headers, params=params)
+    return response.json()
+
+
+if __name__ == "__main__":
+    # cookie = requests.get('http://localhost:3000/sensortower')
+    # cookie = cookie.json()
+
+    cookie = {
+        "session": "2e8e2b1cfd6d791d55b235e53066f7a3",
+        "device_id": "446def50-8494-487a-ab39-d8d965f014d2",
+    }
+
+    result = advanced_search(
+        cookie=cookie, custom_filter_id="643bd16ee1714cfff1654c97", term="voice changer")
+    print(json.dumps(result, indent=2))
```

### Comparing `haki_crawler-0.4/haki_crawler.egg-info/PKG-INFO` & `haki_crawler-0.5/haki_crawler.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haki-crawler
-Version: 0.4
+Version: 0.5
 Summary: A short description of your package
 Home-page: https://example.com
 Author: namhn1495
 Author-email: namhn1495@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `haki_crawler-0.4/setup.py` & `haki_crawler-0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         shutil.rmtree(thu_muc)
         print(f"Đã xóa thư mục: {thu_muc}")
     else:
         print(f"Thư mục {thu_muc} không tồn tại")
 
 setup(
     name=LIB_NAME,
-    version="0.4",
+    version="0.5",
     packages=find_packages(),
     install_requires=[
         # Danh sách các gói phụ thuộc của gói này
         "requests",
     ],
     author="namhn1495",
     author_email="namhn1495@gmail.com",
```

