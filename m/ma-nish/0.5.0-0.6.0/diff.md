# Comparing `tmp/ma-nish-0.5.0.tar.gz` & `tmp/ma-nish-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ma-nish-0.5.0.tar", last modified: Sat Jan 14 17:51:15 2023, max compression
+gzip compressed data, was "ma-nish-0.6.0.tar", last modified: Sun Apr 16 15:26:55 2023, max compression
```

## Comparing `ma-nish-0.5.0.tar` & `ma-nish-0.6.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 17:51:15.000000 ma-nish-0.5.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 17:51:15.000000 ma-nish-0.5.0/ma_nish.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13624 2023-01-14 17:51:14.000000 ma-nish-0.5.0/ma_nish.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      290 2023-01-14 17:51:14.000000 ma-nish-0.5.0/ma_nish.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-14 17:51:14.000000 ma-nish-0.5.0/ma_nish.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      112 2023-01-14 17:51:14.000000 ma-nish-0.5.0/ma_nish.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-01-14 17:51:14.000000 ma-nish-0.5.0/ma_nish.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 17:51:15.000000 ma-nish-0.5.0/manish/
--rw-r--r--   0 root         (0) root         (0)    37215 2023-01-01 14:15:48.000000 ma-nish-0.5.0/manish/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1050 2023-01-01 14:22:08.000000 ma-nish-0.5.0/manish/button.py
--rw-r--r--   0 root         (0) root         (0)     2196 2023-01-01 14:22:03.000000 ma-nish-0.5.0/manish/contact.py
--rw-r--r--   0 root         (0) root         (0)     1193 2023-01-01 14:16:59.000000 ma-nish-0.5.0/manish/helpers.py
--rw-r--r--   0 root         (0) root         (0)      997 2023-01-01 14:21:32.000000 ma-nish-0.5.0/manish/location.py
--rw-r--r--   0 root         (0) root         (0)     1616 2023-01-01 14:18:02.000000 ma-nish-0.5.0/manish/template.py
--rw-r--r--   0 root         (0) root         (0)     1068 2022-11-27 13:18:25.000000 ma-nish-0.5.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)    13102 2023-01-14 17:45:26.000000 ma-nish-0.5.0/README.md
--rw-r--r--   0 root         (0) root         (0)     1089 2023-01-14 17:50:59.000000 ma-nish-0.5.0/setup.py
--rw-r--r--   0 root         (0) root         (0)    13624 2023-01-14 17:51:15.000000 ma-nish-0.5.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-14 17:51:15.000000 ma-nish-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:26:55.386890 ma-nish-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-16 15:26:41.000000 ma-nish-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13605 2023-04-16 15:26:55.386890 ma-nish-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13103 2023-04-16 15:26:41.000000 ma-nish-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:26:55.386890 ma-nish-0.6.0/ma_nish.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13605 2023-04-16 15:26:55.000000 ma-nish-0.6.0/ma_nish.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-16 15:26:55.000000 ma-nish-0.6.0/ma_nish.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 15:26:55.000000 ma-nish-0.6.0/ma_nish.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-16 15:26:55.000000 ma-nish-0.6.0/ma_nish.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-16 15:26:55.000000 ma-nish-0.6.0/ma_nish.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:26:55.386890 ma-nish-0.6.0/manish/
+-rw-r--r--   0 runner    (1001) docker     (123)    37823 2023-04-16 15:26:41.000000 ma-nish-0.6.0/manish/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-16 15:26:41.000000 ma-nish-0.6.0/manish/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-16 15:26:41.000000 ma-nish-0.6.0/manish/contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-16 15:26:41.000000 ma-nish-0.6.0/manish/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-16 15:26:41.000000 ma-nish-0.6.0/manish/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-16 15:26:41.000000 ma-nish-0.6.0/manish/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 15:26:55.386890 ma-nish-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-16 15:26:41.000000 ma-nish-0.6.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ma-nish-0.5.0/ma_nish.egg-info/PKG-INFO` & `ma-nish-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: ma-nish
-Version: 0.5.0
+Version: 0.6.0
 Summary: manish is an unofficial python wrapper for Whatsapp cloud api
 Home-page: https://github.com/t0mer/ma-nish
+Download-URL: https://pypi.org/project/ma-nish/
 Author: Tomer Klein
 Author-email: tomer.klein@gmail.com
 License: MIT
-Download-URL: https://pypi.org/project/ma-nish/
 Project-URL: Documentation, https://github.com/t0mer/ma-nish
 Project-URL: Source, https://github.com/t0mer/ma-nish
 Keywords: meta,ma-nish,facebook,whatsapp
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # manish
 WhatsApp has now opened up its API so you no longer have to go through a partner to send and receive WhatsApp messages!
 MaNish is an Unofficial python wrapper to [WhatsApp Cloud API](https://developers.facebook.com/docs/whatsapp/cloud-api)
 
@@ -72,15 +71,15 @@
 pip3 install --upgrade ma-nish
 ```
 
 
 ## Setting up the environment
 ### Set Up Meta App
 
-First you’ll need to follow the (instructions on this page)[https://developers.facebook.com/docs/whatsapp/cloud-api/get-started] to:
+First you’ll need to follow the [instructions on this page](https://developers.facebook.com/docs/whatsapp/cloud-api/get-started) to:
 
 * Register as a Meta Developer
 * Enable two-factor authentication for your account
 * Create a Meta App – you need to create a Business App for WhatsApp
 
 Once you’ve done that, go to your app and set up the WhatsApp product.
 
@@ -340,8 +339,7 @@
 >>>             delivery = manish.get_delivery(data)
 >>>             if delivery:
 >>>                 logger.info(f"Message : {delivery}")
 >>>             else:
 >>>                 logger.info("No new message")
 >>>     return "ok"
 ```
-
```

### Comparing `ma-nish-0.5.0/manish/__init__.py` & `ma-nish-0.6.0/manish/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -791,14 +791,32 @@
                 if "audio" in data["messages"][0]:
                     return data["messages"][0]["audio"]
             return None
         except Exception as e:
             logger.error("aw snap something went wrong: " + str(e))
             return None
 
+
+    def get_mobile(self, data: Dict[Any, Any]) -> Union[str, None]:
+        """
+        Extracts the mobile number of the sender from the data received from the webhook.
+        Args:
+            data[dict]: The data received from the webhook
+        Returns:
+            str: The mobile number of the sender
+        Example:
+            >>> from whatsapp import WhatsApp
+            >>> manish = MaNish(token, phone_number_id)
+            >>> mobile = manish.get_mobile(data)
+        """
+        data = self.preprocess(data)
+        if "contacts" in data:
+            return data["contacts"][0]["wa_id"]
+
+
     def get_video(self, data):
         """
         Extracts the video of the sender from the data received from the webhook.
         Args:
             data[dict]: The data received from the webhook
         Returns:
             dict: Dictionary containing the video details sent by the sender
```

### Comparing `ma-nish-0.5.0/manish/button.py` & `ma-nish-0.6.0/manish/button.py`

 * *Files identical despite different names*

### Comparing `ma-nish-0.5.0/manish/contact.py` & `ma-nish-0.6.0/manish/contact.py`

 * *Files identical despite different names*

### Comparing `ma-nish-0.5.0/manish/helpers.py` & `ma-nish-0.6.0/manish/helpers.py`

 * *Files identical despite different names*

### Comparing `ma-nish-0.5.0/manish/location.py` & `ma-nish-0.6.0/manish/location.py`

 * *Files identical despite different names*

### Comparing `ma-nish-0.5.0/manish/template.py` & `ma-nish-0.6.0/manish/template.py`

 * *Files identical despite different names*

### Comparing `ma-nish-0.5.0/LICENSE` & `ma-nish-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ma-nish-0.5.0/README.md` & `ma-nish-0.6.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 pip3 install --upgrade ma-nish
 ```
 
 
 ## Setting up the environment
 ### Set Up Meta App
 
-First you’ll need to follow the (instructions on this page)[https://developers.facebook.com/docs/whatsapp/cloud-api/get-started] to:
+First you’ll need to follow the [instructions on this page](https://developers.facebook.com/docs/whatsapp/cloud-api/get-started) to:
 
 * Register as a Meta Developer
 * Enable two-factor authentication for your account
 * Create a Meta App – you need to create a Business App for WhatsApp
 
 Once you’ve done that, go to your app and set up the WhatsApp product.
 
@@ -323,8 +323,8 @@
 >>>         else:
 >>>             delivery = manish.get_delivery(data)
 >>>             if delivery:
 >>>                 logger.info(f"Message : {delivery}")
 >>>             else:
 >>>                 logger.info("No new message")
 >>>     return "ok"
-```
+```
```

### Comparing `ma-nish-0.5.0/setup.py` & `ma-nish-0.6.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open("README.md", "r", encoding="UTF-8") as f:
      readme = f.read()
 
 
 setup_args = dict(
     name='ma-nish',
-    version='0.5.0',
+    version='0.6.0',
     description='manish is an unofficial python wrapper for Whatsapp cloud api',
     long_description_content_type="text/markdown",
     long_description=readme,
     license='MIT',
     packages=find_packages(),
     author='Tomer Klein',
     author_email='tomer.klein@gmail.com',
```

### Comparing `ma-nish-0.5.0/PKG-INFO` & `ma-nish-0.6.0/ma_nish.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: ma-nish
-Version: 0.5.0
+Version: 0.6.0
 Summary: manish is an unofficial python wrapper for Whatsapp cloud api
 Home-page: https://github.com/t0mer/ma-nish
+Download-URL: https://pypi.org/project/ma-nish/
 Author: Tomer Klein
 Author-email: tomer.klein@gmail.com
 License: MIT
-Download-URL: https://pypi.org/project/ma-nish/
 Project-URL: Documentation, https://github.com/t0mer/ma-nish
 Project-URL: Source, https://github.com/t0mer/ma-nish
 Keywords: meta,ma-nish,facebook,whatsapp
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # manish
 WhatsApp has now opened up its API so you no longer have to go through a partner to send and receive WhatsApp messages!
 MaNish is an Unofficial python wrapper to [WhatsApp Cloud API](https://developers.facebook.com/docs/whatsapp/cloud-api)
 
@@ -72,15 +71,15 @@
 pip3 install --upgrade ma-nish
 ```
 
 
 ## Setting up the environment
 ### Set Up Meta App
 
-First you’ll need to follow the (instructions on this page)[https://developers.facebook.com/docs/whatsapp/cloud-api/get-started] to:
+First you’ll need to follow the [instructions on this page](https://developers.facebook.com/docs/whatsapp/cloud-api/get-started) to:
 
 * Register as a Meta Developer
 * Enable two-factor authentication for your account
 * Create a Meta App – you need to create a Business App for WhatsApp
 
 Once you’ve done that, go to your app and set up the WhatsApp product.
 
@@ -340,8 +339,7 @@
 >>>             delivery = manish.get_delivery(data)
 >>>             if delivery:
 >>>                 logger.info(f"Message : {delivery}")
 >>>             else:
 >>>                 logger.info("No new message")
 >>>     return "ok"
 ```
-
```

