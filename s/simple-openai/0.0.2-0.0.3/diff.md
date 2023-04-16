# Comparing `tmp/simple-openai-0.0.2.tar.gz` & `tmp/simple-openai-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-openai-0.0.2.tar", last modified: Sun Apr 16 14:42:40 2023, max compression
+gzip compressed data, was "simple-openai-0.0.3.tar", last modified: Sun Apr 16 14:46:41 2023, max compression
```

## Comparing `simple-openai-0.0.2.tar` & `simple-openai-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-16 14:42:40.476346 simple-openai-0.0.2/
--rw-r--r--   0 steve      (501) staff       (20)    11357 2023-04-15 11:09:16.000000 simple-openai-0.0.2/LICENSE
--rw-r--r--   0 steve      (501) staff       (20)    14318 2023-04-16 14:42:40.475932 simple-openai-0.0.2/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)      421 2023-04-16 14:41:39.000000 simple-openai-0.0.2/README.md
--rw-r--r--   0 steve      (501) staff       (20)     1179 2023-04-16 14:42:15.000000 simple-openai-0.0.2/pyproject.toml
--rw-r--r--   0 steve      (501) staff       (20)       38 2023-04-16 14:42:40.476414 simple-openai-0.0.2/setup.cfg
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-16 14:42:40.471809 simple-openai-0.0.2/src/
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-16 14:42:40.473628 simple-openai-0.0.2/src/simple_openai/
--rw-r--r--   0 steve      (501) staff       (20)      223 2023-04-16 13:49:41.000000 simple-openai-0.0.2/src/simple_openai/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)     6571 2023-04-16 13:37:12.000000 simple-openai-0.0.2/src/simple_openai/async_simple_openai.py
--rw-r--r--   0 steve      (501) staff       (20)      184 2023-04-16 13:51:48.000000 simple-openai-0.0.2/src/simple_openai/constants.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-16 14:42:40.474717 simple-openai-0.0.2/src/simple_openai/models/
--rw-r--r--   0 steve      (501) staff       (20)      883 2023-04-15 16:43:05.000000 simple-openai-0.0.2/src/simple_openai/models/open_ai_models.py
--rw-r--r--   0 steve      (501) staff       (20)      672 2023-04-16 13:21:37.000000 simple-openai-0.0.2/src/simple_openai/responses.py
--rw-r--r--   0 steve      (501) staff       (20)     5924 2023-04-16 13:48:53.000000 simple-openai-0.0.2/src/simple_openai/simple_openai.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-16 14:42:40.474577 simple-openai-0.0.2/src/simple_openai.egg-info/
--rw-r--r--   0 steve      (501) staff       (20)    14318 2023-04-16 14:42:40.000000 simple-openai-0.0.2/src/simple_openai.egg-info/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)      506 2023-04-16 14:42:40.000000 simple-openai-0.0.2/src/simple_openai.egg-info/SOURCES.txt
--rw-r--r--   0 steve      (501) staff       (20)        1 2023-04-16 14:42:40.000000 simple-openai-0.0.2/src/simple_openai.egg-info/dependency_links.txt
--rw-r--r--   0 steve      (501) staff       (20)       89 2023-04-16 14:42:40.000000 simple-openai-0.0.2/src/simple_openai.egg-info/requires.txt
--rw-r--r--   0 steve      (501) staff       (20)       14 2023-04-16 14:42:40.000000 simple-openai-0.0.2/src/simple_openai.egg-info/top_level.txt
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-16 14:42:40.475413 simple-openai-0.0.2/tests/
--rw-r--r--   0 steve      (501) staff       (20)     1579 2023-04-16 13:13:06.000000 simple-openai-0.0.2/tests/test_AsyncSimpleOpenai.py
--rw-r--r--   0 steve      (501) staff       (20)     1461 2023-04-16 13:51:21.000000 simple-openai-0.0.2/tests/test_SimpleOpenai.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-16 14:46:41.851611 simple-openai-0.0.3/
+-rw-r--r--   0 steve      (501) staff       (20)    11357 2023-04-15 11:09:16.000000 simple-openai-0.0.3/LICENSE
+-rw-r--r--   0 steve      (501) staff       (20)    16494 2023-04-16 14:46:41.851392 simple-openai-0.0.3/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)     2597 2023-04-16 14:45:45.000000 simple-openai-0.0.3/README.md
+-rw-r--r--   0 steve      (501) staff       (20)     1179 2023-04-16 14:46:16.000000 simple-openai-0.0.3/pyproject.toml
+-rw-r--r--   0 steve      (501) staff       (20)       38 2023-04-16 14:46:41.851653 simple-openai-0.0.3/setup.cfg
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-16 14:46:41.847591 simple-openai-0.0.3/src/
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-16 14:46:41.849437 simple-openai-0.0.3/src/simple_openai/
+-rw-r--r--   0 steve      (501) staff       (20)      223 2023-04-16 13:49:41.000000 simple-openai-0.0.3/src/simple_openai/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)     6571 2023-04-16 13:37:12.000000 simple-openai-0.0.3/src/simple_openai/async_simple_openai.py
+-rw-r--r--   0 steve      (501) staff       (20)      184 2023-04-16 13:51:48.000000 simple-openai-0.0.3/src/simple_openai/constants.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-16 14:46:41.850500 simple-openai-0.0.3/src/simple_openai/models/
+-rw-r--r--   0 steve      (501) staff       (20)      883 2023-04-15 16:43:05.000000 simple-openai-0.0.3/src/simple_openai/models/open_ai_models.py
+-rw-r--r--   0 steve      (501) staff       (20)      672 2023-04-16 13:21:37.000000 simple-openai-0.0.3/src/simple_openai/responses.py
+-rw-r--r--   0 steve      (501) staff       (20)     5924 2023-04-16 13:48:53.000000 simple-openai-0.0.3/src/simple_openai/simple_openai.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-16 14:46:41.850371 simple-openai-0.0.3/src/simple_openai.egg-info/
+-rw-r--r--   0 steve      (501) staff       (20)    16494 2023-04-16 14:46:41.000000 simple-openai-0.0.3/src/simple_openai.egg-info/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)      506 2023-04-16 14:46:41.000000 simple-openai-0.0.3/src/simple_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 steve      (501) staff       (20)        1 2023-04-16 14:46:41.000000 simple-openai-0.0.3/src/simple_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 steve      (501) staff       (20)       89 2023-04-16 14:46:41.000000 simple-openai-0.0.3/src/simple_openai.egg-info/requires.txt
+-rw-r--r--   0 steve      (501) staff       (20)       14 2023-04-16 14:46:41.000000 simple-openai-0.0.3/src/simple_openai.egg-info/top_level.txt
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-16 14:46:41.851036 simple-openai-0.0.3/tests/
+-rw-r--r--   0 steve      (501) staff       (20)     1579 2023-04-16 13:13:06.000000 simple-openai-0.0.3/tests/test_AsyncSimpleOpenai.py
+-rw-r--r--   0 steve      (501) staff       (20)     1461 2023-04-16 13:51:21.000000 simple-openai-0.0.3/tests/test_SimpleOpenai.py
```

### Comparing `simple-openai-0.0.2/LICENSE` & `simple-openai-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `simple-openai-0.0.2/PKG-INFO` & `simple-openai-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-openai
-Version: 0.0.2
+Version: 0.0.3
 Summary: Simple OpenAI API wrapper
 Author-email: Stephen Schleising <stephen@schleising.net>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -230,10 +230,86 @@
 
 ## Installation
 
 ```bash
 pip install simple-openai
 ```
 
+## Usage
+
+### Calling the API
+
+For the synchronous version, you can use the following code:
+
+    from simple_openai import SimpleOpenai
+
+    def main():
+        # Create the client
+        client = SimpleOpenai(api_key)
+
+        # Create tasks for the chat response and the image response
+        result = client.get_chat_response("Hello, how are you?")
+
+        # Print the result
+        if result.success:
+            # Print the message
+            print(f'Success: {result.message}')
+        else:
+            # Print the error
+            print(f'Error: {result.message}')
+
+        result = client.get_image_url("A cat")
+
+        # Print the result
+        if result.success:
+            # Print the message
+            print(f'Success: {result.message}')
+        else:
+            # Print the error
+            print(f'Error: {result.message}')
+
+    if __name__ == "__main__":
+        # Run the main function
+        main()
+
+For the asynchronous version, you can use the following code:
+
+    from simple_openai import AsyncSimpleOpenai
+    import asyncio
+
+    async def main():
+        # Create the client
+        client = AsyncSimpleOpenai(api_key)
+
+        # Create tasks for the chat response and the image response
+        tasks = [
+            client.get_chat_response("Hello, how are you?"),
+            client.get_image_url("A cat"),
+        ]
+
+        # Wait for the tasks to complete
+        for task in asyncio.as_completed(tasks):
+            # Get the result
+            result = await task
+
+            # Print the result
+            if result.success:
+                # Print the message
+                print(f'Success: {result.message}')
+            else:
+                # Print the error
+                print(f'Error: {result.message}')
+
+    if __name__ == "__main__":
+        # Run the main function
+        asyncio.run(main())
+
+### Output
+
+The output of the functions is a [SimpleOpenaiResponse](/simple_openai/responses/#src.simple_openai.responses.SimpleOpenaiResponse) object, which contains the following properties:
+
+- `success` - A boolean indicating whether the request was successful or not.
+- `message` - The message returned by the API.
+
 ## Documentation
 
 The documentation is available on [GitHub](https://schleising.github.io/simple-openai/)
```

### Comparing `simple-openai-0.0.2/pyproject.toml` & `simple-openai-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "simple-openai"
-version = "0.0.2"
+version = "0.0.3"
 description = "Simple OpenAI API wrapper"
 readme = "README.md"
 authors = [{ name = "Stephen Schleising", email = "stephen@schleising.net" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
```

### Comparing `simple-openai-0.0.2/src/simple_openai/async_simple_openai.py` & `simple-openai-0.0.3/src/simple_openai/async_simple_openai.py`

 * *Files identical despite different names*

### Comparing `simple-openai-0.0.2/src/simple_openai/models/open_ai_models.py` & `simple-openai-0.0.3/src/simple_openai/models/open_ai_models.py`

 * *Files identical despite different names*

### Comparing `simple-openai-0.0.2/src/simple_openai/responses.py` & `simple-openai-0.0.3/src/simple_openai/responses.py`

 * *Files identical despite different names*

### Comparing `simple-openai-0.0.2/src/simple_openai/simple_openai.py` & `simple-openai-0.0.3/src/simple_openai/simple_openai.py`

 * *Files identical despite different names*

### Comparing `simple-openai-0.0.2/src/simple_openai.egg-info/PKG-INFO` & `simple-openai-0.0.3/src/simple_openai.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-openai
-Version: 0.0.2
+Version: 0.0.3
 Summary: Simple OpenAI API wrapper
 Author-email: Stephen Schleising <stephen@schleising.net>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -230,10 +230,86 @@
 
 ## Installation
 
 ```bash
 pip install simple-openai
 ```
 
+## Usage
+
+### Calling the API
+
+For the synchronous version, you can use the following code:
+
+    from simple_openai import SimpleOpenai
+
+    def main():
+        # Create the client
+        client = SimpleOpenai(api_key)
+
+        # Create tasks for the chat response and the image response
+        result = client.get_chat_response("Hello, how are you?")
+
+        # Print the result
+        if result.success:
+            # Print the message
+            print(f'Success: {result.message}')
+        else:
+            # Print the error
+            print(f'Error: {result.message}')
+
+        result = client.get_image_url("A cat")
+
+        # Print the result
+        if result.success:
+            # Print the message
+            print(f'Success: {result.message}')
+        else:
+            # Print the error
+            print(f'Error: {result.message}')
+
+    if __name__ == "__main__":
+        # Run the main function
+        main()
+
+For the asynchronous version, you can use the following code:
+
+    from simple_openai import AsyncSimpleOpenai
+    import asyncio
+
+    async def main():
+        # Create the client
+        client = AsyncSimpleOpenai(api_key)
+
+        # Create tasks for the chat response and the image response
+        tasks = [
+            client.get_chat_response("Hello, how are you?"),
+            client.get_image_url("A cat"),
+        ]
+
+        # Wait for the tasks to complete
+        for task in asyncio.as_completed(tasks):
+            # Get the result
+            result = await task
+
+            # Print the result
+            if result.success:
+                # Print the message
+                print(f'Success: {result.message}')
+            else:
+                # Print the error
+                print(f'Error: {result.message}')
+
+    if __name__ == "__main__":
+        # Run the main function
+        asyncio.run(main())
+
+### Output
+
+The output of the functions is a [SimpleOpenaiResponse](/simple_openai/responses/#src.simple_openai.responses.SimpleOpenaiResponse) object, which contains the following properties:
+
+- `success` - A boolean indicating whether the request was successful or not.
+- `message` - The message returned by the API.
+
 ## Documentation
 
 The documentation is available on [GitHub](https://schleising.github.io/simple-openai/)
```

### Comparing `simple-openai-0.0.2/tests/test_AsyncSimpleOpenai.py` & `simple-openai-0.0.3/tests/test_AsyncSimpleOpenai.py`

 * *Files identical despite different names*

### Comparing `simple-openai-0.0.2/tests/test_SimpleOpenai.py` & `simple-openai-0.0.3/tests/test_SimpleOpenai.py`

 * *Files identical despite different names*

