# Comparing `tmp/EuclidSearchPackage-0.5.1.tar.gz` & `tmp/EuclidSearchPackage-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EuclidSearchPackage-0.5.1.tar", last modified: Tue Apr  4 16:44:48 2023, max compression
+gzip compressed data, was "EuclidSearchPackage-0.6.0.tar", last modified: Sun Apr 16 06:41:16 2023, max compression
```

## Comparing `EuclidSearchPackage-0.5.1.tar` & `EuclidSearchPackage-0.6.0.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-04-04 16:44:48.644781 EuclidSearchPackage-0.5.1/
--rw-rw-rw-   0        0        0     1080 2023-03-27 14:41:42.000000 EuclidSearchPackage-0.5.1/LICENSE
--rw-rw-rw-   0        0        0     3229 2023-04-04 16:44:48.643787 EuclidSearchPackage-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     1533 2023-03-29 05:49:21.000000 EuclidSearchPackage-0.5.1/README.md
--rw-rw-rw-   0        0        0      648 2023-04-04 16:44:32.000000 EuclidSearchPackage-0.5.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-04 16:44:48.644781 EuclidSearchPackage-0.5.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-04 16:44:48.512232 EuclidSearchPackage-0.5.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-04 16:44:48.515164 EuclidSearchPackage-0.5.1/src/EuclidSearchPackage/
-drwxrwxrwx   0        0        0        0 2023-04-04 16:44:48.536827 EuclidSearchPackage-0.5.1/src/EuclidSearchPackage/Demo/
--rw-rw-rw-   0        0        0     4554 2023-04-04 16:26:05.000000 EuclidSearchPackage-0.5.1/src/EuclidSearchPackage/Demo/WeiboClassV2.py
--rw-rw-rw-   0        0        0     3900 2023-04-04 16:41:51.000000 EuclidSearchPackage-0.5.1/src/EuclidSearchPackage/Demo/WeiboClassV3.py
--rw-rw-rw-   0        0        0      191 2023-03-29 05:37:33.000000 EuclidSearchPackage-0.5.1/src/EuclidSearchPackage/Demo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-04 16:44:48.596256 EuclidSearchPackage-0.5.1/src/EuclidSearchPackage/Utils/
--rw-rw-rw-   0        0        0     3006 2023-03-26 11:02:38.000000 EuclidSearchPackage-0.5.1/src/EuclidSearchPackage/Utils/EuclidDataTools.py
--rw-rw-rw-   0        0        0      602 2023-03-28 04:46:40.000000 EuclidSearchPackage-0.5.1/src/EuclidSearchPackage/Utils/EuclidDataTools_test.py
--rw-rw-rw-   0        0        0      378 2023-02-09 15:28:21.000000 EuclidSearchPackage-0.5.1/src/EuclidSearchPackage/Utils/MongoClient.py
--rw-rw-rw-   0        0        0      834 2023-02-10 08:51:16.000000 EuclidSearchPackage-0.5.1/src/EuclidSearchPackage/Utils/Set_header.py
--rw-rw-rw-   0        0        0      410 2023-03-28 04:46:40.000000 EuclidSearchPackage-0.5.1/src/EuclidSearchPackage/Utils/Utils.py
--rw-rw-rw-   0        0        0      220 2023-03-28 08:19:33.000000 EuclidSearchPackage-0.5.1/src/EuclidSearchPackage/Utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-04 16:44:48.638714 EuclidSearchPackage-0.5.1/src/EuclidSearchPackage/WeiboSearch/
--rw-rw-rw-   0        0        0     1138 2023-03-28 04:29:56.000000 EuclidSearchPackage-0.5.1/src/EuclidSearchPackage/WeiboSearch/Get_item_url_list.py
--rw-rw-rw-   0        0        0     1158 2023-03-29 05:39:33.000000 EuclidSearchPackage-0.5.1/src/EuclidSearchPackage/WeiboSearch/Get_longTextContent.py
--rw-rw-rw-   0        0        0     2410 2023-04-04 16:22:05.000000 EuclidSearchPackage-0.5.1/src/EuclidSearchPackage/WeiboSearch/Get_single_weibo_data.py
--rw-rw-rw-   0        0        0     5073 2023-03-28 04:40:36.000000 EuclidSearchPackage-0.5.1/src/EuclidSearchPackage/WeiboSearch/Get_single_weibo_details.py
--rw-rw-rw-   0        0        0     3105 2023-03-28 04:33:56.000000 EuclidSearchPackage-0.5.1/src/EuclidSearchPackage/WeiboSearch/Get_user_all_weibo.py
--rw-rw-rw-   0        0        0     1024 2023-03-28 04:08:25.000000 EuclidSearchPackage-0.5.1/src/EuclidSearchPackage/WeiboSearch/Get_user_info.py
--rw-rw-rw-   0        0        0      501 2023-03-28 04:29:00.000000 EuclidSearchPackage-0.5.1/src/EuclidSearchPackage/WeiboSearch/Set_cookie.py
--rw-rw-rw-   0        0        0      640 2023-04-04 16:22:05.000000 EuclidSearchPackage-0.5.1/src/EuclidSearchPackage/WeiboSearch/__init__.py
--rw-rw-rw-   0        0        0      223 2023-03-29 05:37:33.000000 EuclidSearchPackage-0.5.1/src/EuclidSearchPackage/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-04 16:44:48.534805 EuclidSearchPackage-0.5.1/src/EuclidSearchPackage.egg-info/
--rw-rw-rw-   0        0        0     3229 2023-04-04 16:44:48.000000 EuclidSearchPackage-0.5.1/src/EuclidSearchPackage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1148 2023-04-04 16:44:48.000000 EuclidSearchPackage-0.5.1/src/EuclidSearchPackage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-04 16:44:48.000000 EuclidSearchPackage-0.5.1/src/EuclidSearchPackage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-04-04 16:44:48.000000 EuclidSearchPackage-0.5.1/src/EuclidSearchPackage.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-04 16:44:48.642800 EuclidSearchPackage-0.5.1/src/Test/
--rw-rw-rw-   0        0        0      261 2023-04-04 16:30:47.000000 EuclidSearchPackage-0.5.1/src/Test/DemoTest.py
--rw-rw-rw-   0        0        0      679 2023-03-28 08:26:35.000000 EuclidSearchPackage-0.5.1/src/Test/Test.py
+drwxrwxrwx   0        0        0        0 2023-04-16 06:41:16.214428 EuclidSearchPackage-0.6.0/
+-rw-rw-rw-   0        0        0     1080 2023-03-27 14:41:42.000000 EuclidSearchPackage-0.6.0/LICENSE
+-rw-rw-rw-   0        0        0     3521 2023-04-16 06:41:16.214428 EuclidSearchPackage-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1825 2023-04-16 06:35:54.000000 EuclidSearchPackage-0.6.0/README.md
+-rw-rw-rw-   0        0        0      648 2023-04-16 06:40:21.000000 EuclidSearchPackage-0.6.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-16 06:41:16.214428 EuclidSearchPackage-0.6.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-16 06:41:16.192101 EuclidSearchPackage-0.6.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-16 06:41:16.195633 EuclidSearchPackage-0.6.0/src/EuclidSearchPackage/
+drwxrwxrwx   0        0        0        0 2023-04-16 06:41:16.201639 EuclidSearchPackage-0.6.0/src/EuclidSearchPackage/Demo/
+-rw-rw-rw-   0        0        0     8048 2023-04-16 06:33:00.000000 EuclidSearchPackage-0.6.0/src/EuclidSearchPackage/Demo/WeiboClassV1.py
+-rw-rw-rw-   0        0        0     4419 2023-04-16 06:33:00.000000 EuclidSearchPackage-0.6.0/src/EuclidSearchPackage/Demo/WeiboClassV2.py
+-rw-rw-rw-   0        0        0     3782 2023-04-16 06:33:00.000000 EuclidSearchPackage-0.6.0/src/EuclidSearchPackage/Demo/WeiboClassV3.py
+-rw-rw-rw-   0        0        0      231 2023-04-16 06:33:00.000000 EuclidSearchPackage-0.6.0/src/EuclidSearchPackage/Demo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 06:41:16.205640 EuclidSearchPackage-0.6.0/src/EuclidSearchPackage/Utils/
+-rw-rw-rw-   0        0        0     3006 2023-03-26 11:02:38.000000 EuclidSearchPackage-0.6.0/src/EuclidSearchPackage/Utils/EuclidDataTools.py
+-rw-rw-rw-   0        0        0      602 2023-03-28 04:46:40.000000 EuclidSearchPackage-0.6.0/src/EuclidSearchPackage/Utils/EuclidDataTools_test.py
+-rw-rw-rw-   0        0        0      378 2023-02-09 15:28:21.000000 EuclidSearchPackage-0.6.0/src/EuclidSearchPackage/Utils/MongoClient.py
+-rw-rw-rw-   0        0        0      834 2023-02-10 08:51:16.000000 EuclidSearchPackage-0.6.0/src/EuclidSearchPackage/Utils/Set_header.py
+-rw-rw-rw-   0        0        0      849 2023-04-16 06:23:45.000000 EuclidSearchPackage-0.6.0/src/EuclidSearchPackage/Utils/Utils.py
+-rw-rw-rw-   0        0        0      220 2023-03-28 08:19:33.000000 EuclidSearchPackage-0.6.0/src/EuclidSearchPackage/Utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 06:41:16.211640 EuclidSearchPackage-0.6.0/src/EuclidSearchPackage/WeiboSearch/
+-rw-rw-rw-   0        0        0     1138 2023-03-28 04:29:56.000000 EuclidSearchPackage-0.6.0/src/EuclidSearchPackage/WeiboSearch/Get_item_url_list.py
+-rw-rw-rw-   0        0        0     1158 2023-03-29 05:39:33.000000 EuclidSearchPackage-0.6.0/src/EuclidSearchPackage/WeiboSearch/Get_longTextContent.py
+-rw-rw-rw-   0        0        0     2410 2023-04-04 16:22:05.000000 EuclidSearchPackage-0.6.0/src/EuclidSearchPackage/WeiboSearch/Get_single_weibo_data.py
+-rw-rw-rw-   0        0        0     5073 2023-03-28 04:40:36.000000 EuclidSearchPackage-0.6.0/src/EuclidSearchPackage/WeiboSearch/Get_single_weibo_details.py
+-rw-rw-rw-   0        0        0     3105 2023-03-28 04:33:56.000000 EuclidSearchPackage-0.6.0/src/EuclidSearchPackage/WeiboSearch/Get_user_all_weibo.py
+-rw-rw-rw-   0        0        0     1024 2023-03-28 04:08:25.000000 EuclidSearchPackage-0.6.0/src/EuclidSearchPackage/WeiboSearch/Get_user_info.py
+-rw-rw-rw-   0        0        0      501 2023-03-28 04:29:00.000000 EuclidSearchPackage-0.6.0/src/EuclidSearchPackage/WeiboSearch/Set_cookie.py
+-rw-rw-rw-   0        0        0      640 2023-04-04 16:22:05.000000 EuclidSearchPackage-0.6.0/src/EuclidSearchPackage/WeiboSearch/__init__.py
+-rw-rw-rw-   0        0        0      255 2023-04-16 06:33:00.000000 EuclidSearchPackage-0.6.0/src/EuclidSearchPackage/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 06:41:16.198641 EuclidSearchPackage-0.6.0/src/EuclidSearchPackage.egg-info/
+-rw-rw-rw-   0        0        0     3521 2023-04-16 06:41:16.000000 EuclidSearchPackage-0.6.0/src/EuclidSearchPackage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1193 2023-04-16 06:41:16.000000 EuclidSearchPackage-0.6.0/src/EuclidSearchPackage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 06:41:16.000000 EuclidSearchPackage-0.6.0/src/EuclidSearchPackage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-04-16 06:41:16.000000 EuclidSearchPackage-0.6.0/src/EuclidSearchPackage.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 06:41:16.213640 EuclidSearchPackage-0.6.0/src/Test/
+-rw-rw-rw-   0        0        0      337 2023-04-16 06:33:00.000000 EuclidSearchPackage-0.6.0/src/Test/DemoTest.py
+-rw-rw-rw-   0        0        0      679 2023-03-28 08:26:35.000000 EuclidSearchPackage-0.6.0/src/Test/Test.py
```

### Comparing `EuclidSearchPackage-0.5.1/LICENSE` & `EuclidSearchPackage-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `EuclidSearchPackage-0.5.1/PKG-INFO` & `EuclidSearchPackage-0.6.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EuclidSearchPackage
-Version: 0.5.1
+Version: 0.6.0
 Summary: a package for search data from weibo, zhihu, guba and etc.
 Author-email: Euclid Jie <Ouweijie123@outlook.coom>
 License: MIT License
         
         Copyright (c) [2023] [Euclid-Jie]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -38,15 +38,26 @@
 ### 2、set cookie and import package
 
 ```python
 import EuclidSearchPackage as ESP
 ESP.Set_cookie('cookie.txt')  # 'cookie.txt' is your local cookie file path
 ```
 
-### 3、use `WeiboClassV3` to get data
+### 3、use `WeiboClassV1 ` to get data
+
+```python
+import src.EuclidSearchPackage as ESP
+ESP.Set_cookie('cookie.txt')
+timeBegin = '2023-03-01-0'
+timeEnd = '2023-03-10-0'
+demoClass = ESP.WeiboClassV1(Mongo=False)
+demoClass.main_get(['北师大', '珠海'], timeBegin, timeEnd)
+```
+
+### 4、use `WeiboClassV3` to get data
 
 compare to `WeiboClassV2`, `WeiboClassV3` use thread to get data more fast.
 
 ```python
 ESP.WeiboClassV3('北师大', Mongo=False, max_work_count=20, LongText=False).main('2023-03-11-00', '2023-03-27-21')
 ```
```

### Comparing `EuclidSearchPackage-0.5.1/README.md` & `EuclidSearchPackage-0.6.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -15,15 +15,26 @@
 ### 2、set cookie and import package
 
 ```python
 import EuclidSearchPackage as ESP
 ESP.Set_cookie('cookie.txt')  # 'cookie.txt' is your local cookie file path
 ```
 
-### 3、use `WeiboClassV3` to get data
+### 3、use `WeiboClassV1 ` to get data
+
+```python
+import src.EuclidSearchPackage as ESP
+ESP.Set_cookie('cookie.txt')
+timeBegin = '2023-03-01-0'
+timeEnd = '2023-03-10-0'
+demoClass = ESP.WeiboClassV1(Mongo=False)
+demoClass.main_get(['北师大', '珠海'], timeBegin, timeEnd)
+```
+
+### 4、use `WeiboClassV3` to get data
 
 compare to `WeiboClassV2`, `WeiboClassV3` use thread to get data more fast.
 
 ```python
 ESP.WeiboClassV3('北师大', Mongo=False, max_work_count=20, LongText=False).main('2023-03-11-00', '2023-03-27-21')
 ```
```

### Comparing `EuclidSearchPackage-0.5.1/pyproject.toml` & `EuclidSearchPackage-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "EuclidSearchPackage"
-version = "0.5.1"
+version = "0.6.0"
 authors = [
   { name="Euclid Jie", email="Ouweijie123@outlook.coom" },
 ]
 description = "a package for search data from weibo, zhihu, guba and etc."
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
```

### Comparing `EuclidSearchPackage-0.5.1/src/EuclidSearchPackage/Demo/WeiboClassV2.py` & `EuclidSearchPackage-0.6.0/src/EuclidSearchPackage/Demo/WeiboClassV2.py`

 * *Files 8% similar despite different names*

```diff
@@ -113,12 +113,7 @@
                 if NewEndTime >= tmpTime:
                     NewEndTime = tmpTime
                     BreakOrNot = False
             if BreakOrNot:
                 break
             print("\t >>> write blog url done")
         print(">>> get blog info done")
-
-
-if __name__ == '__main__':
-    self = WeiboClassV2('量化实习', Mongo=False)
-    self.main('2023-03-11-00', '2023-03-27-21')
```

### Comparing `EuclidSearchPackage-0.5.1/src/EuclidSearchPackage/Demo/WeiboClassV3.py` & `EuclidSearchPackage-0.6.0/src/EuclidSearchPackage/Demo/WeiboClassV3.py`

 * *Files 11% similar despite different names*

```diff
@@ -86,11 +86,7 @@
                     NewEndTime = tmpTime
                     BreakOrNot = False
             print("\t >>> write blog data done")
             if BreakOrNot:
                 break
 
         print("\n>>> get blog info done")
-
-
-if __name__ == '__main__':
-    WeiboClassV3('量化实习', Mongo=False).main('2023-02-11-00', '2023-03-27-21')
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `EuclidSearchPackage-0.5.1/src/EuclidSearchPackage/Utils/EuclidDataTools.py` & `EuclidSearchPackage-0.6.0/src/EuclidSearchPackage/Utils/EuclidDataTools.py`

 * *Files identical despite different names*

### Comparing `EuclidSearchPackage-0.5.1/src/EuclidSearchPackage/Utils/EuclidDataTools_test.py` & `EuclidSearchPackage-0.6.0/src/EuclidSearchPackage/Utils/EuclidDataTools_test.py`

 * *Files identical despite different names*

### Comparing `EuclidSearchPackage-0.5.1/src/EuclidSearchPackage/Utils/Set_header.py` & `EuclidSearchPackage-0.6.0/src/EuclidSearchPackage/Utils/Set_header.py`

 * *Files identical despite different names*

### Comparing `EuclidSearchPackage-0.5.1/src/EuclidSearchPackage/WeiboSearch/Get_item_url_list.py` & `EuclidSearchPackage-0.6.0/src/EuclidSearchPackage/WeiboSearch/Get_item_url_list.py`

 * *Files identical despite different names*

### Comparing `EuclidSearchPackage-0.5.1/src/EuclidSearchPackage/WeiboSearch/Get_longTextContent.py` & `EuclidSearchPackage-0.6.0/src/EuclidSearchPackage/WeiboSearch/Get_longTextContent.py`

 * *Files identical despite different names*

### Comparing `EuclidSearchPackage-0.5.1/src/EuclidSearchPackage/WeiboSearch/Get_single_weibo_data.py` & `EuclidSearchPackage-0.6.0/src/EuclidSearchPackage/WeiboSearch/Get_single_weibo_data.py`

 * *Files identical despite different names*

### Comparing `EuclidSearchPackage-0.5.1/src/EuclidSearchPackage/WeiboSearch/Get_single_weibo_details.py` & `EuclidSearchPackage-0.6.0/src/EuclidSearchPackage/WeiboSearch/Get_single_weibo_details.py`

 * *Files identical despite different names*

### Comparing `EuclidSearchPackage-0.5.1/src/EuclidSearchPackage/WeiboSearch/Get_user_all_weibo.py` & `EuclidSearchPackage-0.6.0/src/EuclidSearchPackage/WeiboSearch/Get_user_all_weibo.py`

 * *Files identical despite different names*

### Comparing `EuclidSearchPackage-0.5.1/src/EuclidSearchPackage/WeiboSearch/Get_user_info.py` & `EuclidSearchPackage-0.6.0/src/EuclidSearchPackage/WeiboSearch/Get_user_info.py`

 * *Files identical despite different names*

### Comparing `EuclidSearchPackage-0.5.1/src/EuclidSearchPackage/WeiboSearch/__init__.py` & `EuclidSearchPackage-0.6.0/src/EuclidSearchPackage/WeiboSearch/__init__.py`

 * *Files identical despite different names*

### Comparing `EuclidSearchPackage-0.5.1/src/EuclidSearchPackage.egg-info/PKG-INFO` & `EuclidSearchPackage-0.6.0/src/EuclidSearchPackage.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EuclidSearchPackage
-Version: 0.5.1
+Version: 0.6.0
 Summary: a package for search data from weibo, zhihu, guba and etc.
 Author-email: Euclid Jie <Ouweijie123@outlook.coom>
 License: MIT License
         
         Copyright (c) [2023] [Euclid-Jie]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -38,15 +38,26 @@
 ### 2、set cookie and import package
 
 ```python
 import EuclidSearchPackage as ESP
 ESP.Set_cookie('cookie.txt')  # 'cookie.txt' is your local cookie file path
 ```
 
-### 3、use `WeiboClassV3` to get data
+### 3、use `WeiboClassV1 ` to get data
+
+```python
+import src.EuclidSearchPackage as ESP
+ESP.Set_cookie('cookie.txt')
+timeBegin = '2023-03-01-0'
+timeEnd = '2023-03-10-0'
+demoClass = ESP.WeiboClassV1(Mongo=False)
+demoClass.main_get(['北师大', '珠海'], timeBegin, timeEnd)
+```
+
+### 4、use `WeiboClassV3` to get data
 
 compare to `WeiboClassV2`, `WeiboClassV3` use thread to get data more fast.
 
 ```python
 ESP.WeiboClassV3('北师大', Mongo=False, max_work_count=20, LongText=False).main('2023-03-11-00', '2023-03-27-21')
 ```
```

### Comparing `EuclidSearchPackage-0.5.1/src/EuclidSearchPackage.egg-info/SOURCES.txt` & `EuclidSearchPackage-0.6.0/src/EuclidSearchPackage.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 pyproject.toml
 src/EuclidSearchPackage/__init__.py
 src/EuclidSearchPackage.egg-info/PKG-INFO
 src/EuclidSearchPackage.egg-info/SOURCES.txt
 src/EuclidSearchPackage.egg-info/dependency_links.txt
 src/EuclidSearchPackage.egg-info/top_level.txt
+src/EuclidSearchPackage/Demo/WeiboClassV1.py
 src/EuclidSearchPackage/Demo/WeiboClassV2.py
 src/EuclidSearchPackage/Demo/WeiboClassV3.py
 src/EuclidSearchPackage/Demo/__init__.py
 src/EuclidSearchPackage/Utils/EuclidDataTools.py
 src/EuclidSearchPackage/Utils/EuclidDataTools_test.py
 src/EuclidSearchPackage/Utils/MongoClient.py
 src/EuclidSearchPackage/Utils/Set_header.py
```

### Comparing `EuclidSearchPackage-0.5.1/src/Test/Test.py` & `EuclidSearchPackage-0.6.0/src/Test/Test.py`

 * *Files identical despite different names*

