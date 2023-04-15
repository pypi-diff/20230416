# Comparing `tmp/gitmate-0.0.2.tar.gz` & `tmp/gitmate-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitmate-0.0.2.tar", max compression
+gzip compressed data, was "gitmate-0.0.3.tar", max compression
```

## Comparing `gitmate-0.0.2.tar` & `gitmate-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1055 2023-04-01 22:33:36.993810 gitmate-0.0.2/README.md
--rw-r--r--   0        0        0       22 2023-04-01 22:33:51.870482 gitmate-0.0.2/gitmate/__init__.py
--rw-r--r--   0        0        0       36 2023-03-21 22:18:31.321034 gitmate-0.0.2/gitmate/__main__.py
--rw-r--r--   0        0        0     3642 2023-04-01 22:17:44.634506 gitmate-0.0.2/gitmate/main.py
--rw-r--r--   0        0        0     2713 2023-04-01 22:39:31.398213 gitmate-0.0.2/gitmate/models.py
--rw-r--r--   0        0        0     1611 2023-04-01 22:38:00.895672 gitmate-0.0.2/gitmate/utils.py
--rw-r--r--   0        0        0      534 2023-04-01 22:19:05.692485 gitmate-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1600 1970-01-01 00:00:00.000000 gitmate-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-04-01 22:33:36.993810 gitmate-0.0.3/README.md
+-rw-r--r--   0        0        0       22 2023-04-15 23:00:26.637625 gitmate-0.0.3/gitmate/__init__.py
+-rw-r--r--   0        0        0       36 2023-03-21 22:18:31.321034 gitmate-0.0.3/gitmate/__main__.py
+-rw-r--r--   0        0        0     3687 2023-04-15 22:51:52.221186 gitmate-0.0.3/gitmate/main.py
+-rw-r--r--   0        0        0     2713 2023-04-01 22:39:31.398213 gitmate-0.0.3/gitmate/models.py
+-rw-r--r--   0        0        0     1611 2023-04-01 22:38:00.895672 gitmate-0.0.3/gitmate/utils.py
+-rw-r--r--   0        0        0      534 2023-04-15 23:01:11.459098 gitmate-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1600 1970-01-01 00:00:00.000000 gitmate-0.0.3/PKG-INFO
```

### Comparing `gitmate-0.0.2/README.md` & `gitmate-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `gitmate-0.0.2/gitmate/main.py` & `gitmate-0.0.3/gitmate/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 
 @app.command()
 def verify():
     """Used to verify OpenAI API Key and Model name."""
     creds = get_creds(MODEL_OPTIONS)
     if isinstance(creds, dict):
         console.print(creds["error"], style="bold red")
+        return
 
     with Halo(text="Verifying", spinner="dots"):
         openai_key, model_name = creds
         response = predict("Who are you?", 5, openai_key, model_name)
 
     if "error" in response:
         console.print(response["error"]["message"], style="bold red")
@@ -65,14 +66,15 @@
 
 @app.command()
 def commit():
     """Create a commit and auto-generates a commit message."""
     creds = get_creds(MODEL_OPTIONS)
     if isinstance(creds, dict):
         console.print(creds["error"], style="bold red")
+        return
 
     openai_key, model_name = creds
     diff = subprocess.run(["git", "diff", "--cached"], capture_output=True, text=True)
     diff = diff.stdout[:4097]
 
     if not diff:
         console.print(
@@ -93,14 +95,15 @@
 
     if not cli_installed:
         return
 
     creds = get_creds(MODEL_OPTIONS)
     if isinstance(creds, dict):
         console.print(creds["error"], style="bold red")
+        return
 
     openai_key, model_name = creds
     commit_messages = subprocess.run(
         ["git", "log", "main..", "--pretty=format:%s", "--reverse"], capture_output=True, text=True
     )
     commit_messages = commit_messages.stdout
```

### Comparing `gitmate-0.0.2/gitmate/models.py` & `gitmate-0.0.3/gitmate/models.py`

 * *Files identical despite different names*

### Comparing `gitmate-0.0.2/gitmate/utils.py` & `gitmate-0.0.3/gitmate/utils.py`

 * *Files identical despite different names*

### Comparing `gitmate-0.0.2/pyproject.toml` & `gitmate-0.0.3/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gitmate"
-version = "0.0.2"
+version = "0.0.3"
 description = ""
 authors = ["Rohit Gupta <rohitgr1998@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 gitmate = "gitmate.main:app"
```

### Comparing `gitmate-0.0.2/PKG-INFO` & `gitmate-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitmate
-Version: 0.0.2
+Version: 0.0.3
 Summary: 
 Author: Rohit Gupta
 Author-email: rohitgr1998@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

