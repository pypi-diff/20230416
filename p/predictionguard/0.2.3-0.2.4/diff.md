# Comparing `tmp/predictionguard-0.2.3.tar.gz` & `tmp/predictionguard-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "predictionguard-0.2.3.tar", last modified: Tue Mar  7 12:23:15 2023, max compression
+gzip compressed data, was "predictionguard-0.2.4.tar", last modified: Sun Apr 16 20:41:57 2023, max compression
```

## Comparing `predictionguard-0.2.3.tar` & `predictionguard-0.2.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1083 2022-12-30 13:34:31.843283 predictionguard-0.2.3/LICENSE
--rw-r--r--   0        0        0     1878 2023-02-17 23:59:20.007675 predictionguard-0.2.3/README.md
--rw-r--r--   0        0        0     3256 2023-02-19 21:56:15.644765 predictionguard-0.2.3/examples/sentiment.ipynb
--rw-r--r--   0        0        0      104 2023-03-07 12:22:34.771836 predictionguard-0.2.3/predictionguard/__init__.py
--rw-r--r--   0        0        0    10321 2023-03-07 12:22:25.855905 predictionguard-0.2.3/predictionguard/client.py
--rw-r--r--   0        0        0      425 2023-02-19 23:10:58.422073 predictionguard-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     2191 1970-01-01 00:00:00.000000 predictionguard-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1083 2022-12-30 13:34:31.843283 predictionguard-0.2.4/LICENSE
+-rw-r--r--   0        0        0     1878 2023-02-17 23:59:20.007675 predictionguard-0.2.4/README.md
+-rw-r--r--   0        0        0     3256 2023-02-19 21:56:15.644765 predictionguard-0.2.4/examples/sentiment.ipynb
+-rw-r--r--   0        0        0      104 2023-04-16 20:40:32.564410 predictionguard-0.2.4/predictionguard/__init__.py
+-rw-r--r--   0        0        0    10823 2023-04-16 20:40:10.523874 predictionguard-0.2.4/predictionguard/client.py
+-rw-r--r--   0        0        0      425 2023-02-19 23:10:58.422073 predictionguard-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     2191 1970-01-01 00:00:00.000000 predictionguard-0.2.4/PKG-INFO
```

### Comparing `predictionguard-0.2.3/LICENSE` & `predictionguard-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `predictionguard-0.2.3/README.md` & `predictionguard-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `predictionguard-0.2.3/examples/sentiment.ipynb` & `predictionguard-0.2.4/examples/sentiment.ipynb`

 * *Files identical despite different names*

### Comparing `predictionguard-0.2.3/predictionguard/client.py` & `predictionguard-0.2.4/predictionguard/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -144,15 +144,20 @@
                         "Updated At",
                         "Failure Rate",
                         "GPUs",
                     ],
                 )
             )
         else:
-            raise ValueError("Could not list proxies. Please try again.")
+            err = ""
+            try:
+                err = response.json()["error"]
+            except:
+                pass
+            raise ValueError("Could not list proxies. " + err)
 
     def create_proxy(self, task: str, name: str, examples: list, wait: bool = True):
         """
         Create a new proxy.
         Args:
            * task (str): The task to create the proxy for.
            * name (str): The name of the proxy.
@@ -259,15 +264,20 @@
         params = {"name": name}
         response = requests.request("DELETE", url + "/proxy", headers=headers, params=params)
 
         # If the request was successful, print the proxy info.
         if response.status_code == 200:
             print("Proxy deleted successfully!")
         else:
-            raise ValueError("Could not delete proxy. Please try again.")
+            err = ""
+            try:
+                err = response.json()["error"]
+            except:
+                pass
+            raise ValueError("Could not delete proxy. " + err)
 
     def predict(self, name: str, data: dict):
         """
         Make a prediction using a proxy.
         Args:
            * name (str): The name of the proxy to make the prediction with.
            * data (dict): A input sample to submit for inference.
@@ -282,8 +292,15 @@
         )
 
         # If the request was successful, print the proxies.
         if response.status_code == 200:
             prediction = response.json()
             return prediction
         else:
-            raise ValueError("Could not make prediction. Please try again.")
+            # Check if there is a json body in the response. Read that in,
+            # print out the error field in the json body, and raise an exception.
+            err = ""
+            try:
+                err = response.json()["error"]
+            except:
+                pass
+            raise ValueError("Could not make prediction. " + err)
```

### Comparing `predictionguard-0.2.3/PKG-INFO` & `predictionguard-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: predictionguard
-Version: 0.2.3
+Version: 0.2.4
 Summary: AI models are irrelevant. Use Prediction Guard.
 Author-email: Daniel Whitenack <dan@predictionguard.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Project-URL: Home, https://predictionguard.com
 
 # Prediction Guard - Python Client
```

