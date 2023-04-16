# Comparing `tmp/haki_crawler-0.3.tar.gz` & `tmp/haki_crawler-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haki_crawler-0.3.tar", last modified: Sun Apr 16 10:23:49 2023, max compression
+gzip compressed data, was "haki_crawler-0.4.tar", last modified: Sun Apr 16 10:34:57 2023, max compression
```

## Comparing `haki_crawler-0.3.tar` & `haki_crawler-0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-16 10:23:49.511977 haki_crawler-0.3/
--rw-r--r--   0 admin      (501) staff       (20)      616 2023-04-16 10:23:49.511525 haki_crawler-0.3/PKG-INFO
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-16 10:23:49.508553 haki_crawler-0.3/haki_crawler/
--rw-r--r--   0 admin      (501) staff       (20)        0 2023-04-16 10:09:24.000000 haki_crawler-0.3/haki_crawler/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     6103 2023-04-16 10:09:28.000000 haki_crawler-0.3/haki_crawler/sensortower.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-16 10:23:49.510869 haki_crawler-0.3/haki_crawler.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)      616 2023-04-16 10:23:49.000000 haki_crawler-0.3/haki_crawler.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      240 2023-04-16 10:23:49.000000 haki_crawler-0.3/haki_crawler.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2023-04-16 10:23:49.000000 haki_crawler-0.3/haki_crawler.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) staff       (20)        9 2023-04-16 10:23:49.000000 haki_crawler-0.3/haki_crawler.egg-info/requires.txt
--rw-r--r--   0 admin      (501) staff       (20)       13 2023-04-16 10:23:49.000000 haki_crawler-0.3/haki_crawler.egg-info/top_level.txt
--rw-r--r--   0 admin      (501) staff       (20)       38 2023-04-16 10:23:49.512155 haki_crawler-0.3/setup.cfg
--rw-r--r--   0 admin      (501) staff       (20)     1221 2023-04-16 10:23:09.000000 haki_crawler-0.3/setup.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-16 10:34:57.812462 haki_crawler-0.4/
+-rw-r--r--   0 admin      (501) staff       (20)      616 2023-04-16 10:34:57.812179 haki_crawler-0.4/PKG-INFO
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-16 10:34:57.809854 haki_crawler-0.4/haki_crawler/
+-rw-r--r--   0 admin      (501) staff       (20)        0 2023-04-16 10:09:24.000000 haki_crawler-0.4/haki_crawler/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     6115 2023-04-16 10:32:48.000000 haki_crawler-0.4/haki_crawler/sensortower.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-16 10:34:57.811756 haki_crawler-0.4/haki_crawler.egg-info/
+-rw-r--r--   0 admin      (501) staff       (20)      616 2023-04-16 10:34:57.000000 haki_crawler-0.4/haki_crawler.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)      240 2023-04-16 10:34:57.000000 haki_crawler-0.4/haki_crawler.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2023-04-16 10:34:57.000000 haki_crawler-0.4/haki_crawler.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) staff       (20)        9 2023-04-16 10:34:57.000000 haki_crawler-0.4/haki_crawler.egg-info/requires.txt
+-rw-r--r--   0 admin      (501) staff       (20)       13 2023-04-16 10:34:57.000000 haki_crawler-0.4/haki_crawler.egg-info/top_level.txt
+-rw-r--r--   0 admin      (501) staff       (20)       38 2023-04-16 10:34:57.812570 haki_crawler-0.4/setup.cfg
+-rw-r--r--   0 admin      (501) staff       (20)     1221 2023-04-16 10:32:58.000000 haki_crawler-0.4/setup.py
```

### Comparing `haki_crawler-0.3/PKG-INFO` & `haki_crawler-0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haki_crawler
-Version: 0.3
+Version: 0.4
 Summary: A short description of your package
 Home-page: https://example.com
 Author: namhn1495
 Author-email: namhn1495@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `haki_crawler-0.3/haki_crawler/sensortower.py` & `haki_crawler-0.4/haki_crawler/sensortower.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,14 +169,14 @@
     # Send the request to the API and return the response
     response = requests.request("GET", url, headers=headers, params=params)
     return response.json()
 
 
 # cookie = requests.get('http://localhost:3000/sensortower')
 # cookie = cookie.json()
-cookie = {
-    "session": "2e8e2b1cfd6d791d55b235e53066f7a3",
-    "device_id": "446def50-8494-487a-ab39-d8d965f014d2",
-}
+# cookie = {
+#     "session": "2e8e2b1cfd6d791d55b235e53066f7a3",
+#     "device_id": "446def50-8494-487a-ab39-d8d965f014d2",
+# }
 
-result = usages(cookie=cookie)
-print(json.dumps(result, indent=2))
+# result = usages(cookie=cookie)
+# print(json.dumps(result, indent=2))
```

### Comparing `haki_crawler-0.3/haki_crawler.egg-info/PKG-INFO` & `haki_crawler-0.4/haki_crawler.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haki-crawler
-Version: 0.3
+Version: 0.4
 Summary: A short description of your package
 Home-page: https://example.com
 Author: namhn1495
 Author-email: namhn1495@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `haki_crawler-0.3/setup.py` & `haki_crawler-0.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         shutil.rmtree(thu_muc)
         print(f"Đã xóa thư mục: {thu_muc}")
     else:
         print(f"Thư mục {thu_muc} không tồn tại")
 
 setup(
     name=LIB_NAME,
-    version="0.3",
+    version="0.4",
     packages=find_packages(),
     install_requires=[
         # Danh sách các gói phụ thuộc của gói này
         "requests",
     ],
     author="namhn1495",
     author_email="namhn1495@gmail.com",
```

