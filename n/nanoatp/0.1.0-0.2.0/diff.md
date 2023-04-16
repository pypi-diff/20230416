# Comparing `tmp/nanoatp-0.1.0.tar.gz` & `tmp/nanoatp-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanoatp-0.1.0.tar", max compression
+gzip compressed data, was "nanoatp-0.2.0.tar", max compression
```

## Comparing `nanoatp-0.1.0.tar` & `nanoatp-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1067 2023-02-24 19:04:39.038224 nanoatp-0.1.0/LICENSE
--rw-r--r--   0        0        0     1783 2023-04-12 18:39:23.726736 nanoatp-0.1.0/README.md
--rw-r--r--   0        0        0      212 2023-04-12 09:40:00.254184 nanoatp-0.1.0/nanoatp/__init__.py
--rw-r--r--   0        0        0     4117 2023-04-12 18:41:26.813824 nanoatp-0.1.0/nanoatp/nanoatp.py
--rw-r--r--   0        0        0      581 2023-04-11 18:47:08.891565 nanoatp-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2565 1970-01-01 00:00:00.000000 nanoatp-0.1.0/setup.py
--rw-r--r--   0        0        0     2259 1970-01-01 00:00:00.000000 nanoatp-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-02-24 19:04:39.038224 nanoatp-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2482 2023-04-16 10:06:15.513807 nanoatp-0.2.0/README.md
+-rw-r--r--   0        0        0      234 2023-04-16 10:06:15.517638 nanoatp-0.2.0/nanoatp/__init__.py
+-rw-r--r--   0        0        0     7820 2023-04-16 10:06:15.518718 nanoatp-0.2.0/nanoatp/nanoatp.py
+-rw-r--r--   0        0        0      486 2023-04-16 09:51:16.540716 nanoatp-0.2.0/nanoatp/richtext.py
+-rw-r--r--   0        0        0      581 2023-04-16 10:06:15.519574 nanoatp-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3293 1970-01-01 00:00:00.000000 nanoatp-0.2.0/setup.py
+-rw-r--r--   0        0        0     2958 1970-01-01 00:00:00.000000 nanoatp-0.2.0/PKG-INFO
```

### Comparing `nanoatp-0.1.0/LICENSE` & `nanoatp-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nanoatp-0.1.0/README.md` & `nanoatp-0.2.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -11,48 +11,77 @@
 ```
 
 Then in your application:
 
 ```python
 from nanoatp import BskyAgent
 
-agent = new BskyAgent("https://bsky.social")
+agent = BskyAgent("https://bsky.social")
 ```
 
 ## Usage
 
 ### Session management
 
 Log into a server using these APIs. You'll need an active session for most methods.
 
 ```python
 from nanoatp import BskyAgent
 
-agent = new BskyAgent("https://bsky.social")
+agent = BskyAgent("https://bsky.social")
 
 agent.login('alice@mail.com', 'hunter2')
 
 # if you don't specify credentials, ATP_IDENTIFIER and ATP_PASSWORD environment variables will be used
 # agent.login()
 ```
 
 ### API calls
 
 The agent includes methods for many common operations, including:
 
 ```python
 # Feeds and content
+agent.getPost(repo, rkey, cid)
 agent.post(record)
-agent.uploadBlob(data, contentType)
-agent.uploadImage(path, alt, contentType)
+agent.deletePost(postUri)
+agent.uploadBlob(data, encoding)
+agent.uploadImage(path, alt, encoding)  # wrapper for uploadBlob
 
 # Session management
 agent.login(identifier, password)
 ```
 
+For example, to post a record, reply to it, and upload an image:
+
+```python
+from nanoatp import BskyAgent
+
+agent = BskyAgent("https://bsky.social")
+session = agent.login()
+
+record = {"text": "Hello, world! 0"}
+r = agent.post(record)
+root = r
+parent = r
+
+record = {"text": "Hello, world! 1", "reply": {"root": root, "parent": parent}}
+r = agent.post(record)
+parent = r
+
+image = agent.uploadImage("favicon-16x16.png", "image/png")
+embed = {"$type": "app.bsky.embed.images#main", "images": [image]}
+record = {
+    "text": "Hello, world! 2",
+    "reply": {"root": root, "parent": parent},
+    "embed": embed
+}
+agent.post(record)
+```
+
 ## Advanced
 
 ### Advanced API calls
 
 The methods above are convenience wrappers. It covers most but not all available methods.
 
 The AT Protocol identifies methods and records with reverse-DNS names. You can use them on the agent as well:
```

### Comparing `nanoatp-0.1.0/pyproject.toml` & `nanoatp-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nanoatp"
-version = "0.1.0"
+version = "0.2.0"
 description = "nano implementation of the AT Protocol (Authenticated Transfer Protocol)"
 authors = ["Susumu OTA <1632335+susumuota@users.noreply.github.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9.16"
 requests = "^2.28.2"
```

### Comparing `nanoatp-0.1.0/setup.py` & `nanoatp-0.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['requests>=2.28.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'nanoatp',
-    'version': '0.1.0',
+    'version': '0.2.0',
     'description': 'nano implementation of the AT Protocol (Authenticated Transfer Protocol)',
-    'long_description': '# nanoatp\n\nA nano implementation of the AT Protocol (Authenticated Transfer Protocol).\n\n## Getting started\n\nFirst install the package:\n\n```bash\npip install nanoatp\n```\n\nThen in your application:\n\n```python\nfrom nanoatp import BskyAgent\n\nagent = new BskyAgent("https://bsky.social")\n```\n\n## Usage\n\n### Session management\n\nLog into a server using these APIs. You\'ll need an active session for most methods.\n\n```python\nfrom nanoatp import BskyAgent\n\nagent = new BskyAgent("https://bsky.social")\n\nagent.login(\'alice@mail.com\', \'hunter2\')\n\n# if you don\'t specify credentials, ATP_IDENTIFIER and ATP_PASSWORD environment variables will be used\n# agent.login()\n```\n\n### API calls\n\nThe agent includes methods for many common operations, including:\n\n```python\n# Feeds and content\nagent.post(record)\nagent.uploadBlob(data, contentType)\nagent.uploadImage(path, alt, contentType)\n\n# Session management\nagent.login(identifier, password)\n```\n\n## Advanced\n\n### Advanced API calls\n\nThe methods above are convenience wrappers. It covers most but not all available methods.\n\nThe AT Protocol identifies methods and records with reverse-DNS names. You can use them on the agent as well:\n\n```python\nres1 = agent.createRecord(\n    agent.session["did"],  # repo\n    "app.bsky.feed.post",  # collection\n    {\n        "$type": "app.bsky.feed.post",  # record\n        "text": "Hello, world!",\n        "createdAt": datetime.datetime.now(datetime.timezone.utc).isoformat().replace("+00:00", "Z")\n    }\n)\n```\n\n## Development\n\n```bash\nexport ATP_IDENTIFIER="foo.bsky.social"\nexport ATP_PASSWORD="password"\npoetry install\npoetry run pytest -s     # run pytest once\npoetry run -- ptw -- -s  # run pytest and watch for changes\n```\n\n## License\n\nMIT License. See [LICENSE](LICENSE) for details.\n\n## Author\n\nSusumu Ota\n',
+    'long_description': '# nanoatp\n\nA nano implementation of the AT Protocol (Authenticated Transfer Protocol).\n\n## Getting started\n\nFirst install the package:\n\n```bash\npip install nanoatp\n```\n\nThen in your application:\n\n```python\nfrom nanoatp import BskyAgent\n\nagent = BskyAgent("https://bsky.social")\n```\n\n## Usage\n\n### Session management\n\nLog into a server using these APIs. You\'ll need an active session for most methods.\n\n```python\nfrom nanoatp import BskyAgent\n\nagent = BskyAgent("https://bsky.social")\n\nagent.login(\'alice@mail.com\', \'hunter2\')\n\n# if you don\'t specify credentials, ATP_IDENTIFIER and ATP_PASSWORD environment variables will be used\n# agent.login()\n```\n\n### API calls\n\nThe agent includes methods for many common operations, including:\n\n```python\n# Feeds and content\nagent.getPost(repo, rkey, cid)\nagent.post(record)\nagent.deletePost(postUri)\nagent.uploadBlob(data, encoding)\nagent.uploadImage(path, alt, encoding)  # wrapper for uploadBlob\n\n# Session management\nagent.login(identifier, password)\n```\n\nFor example, to post a record, reply to it, and upload an image:\n\n```python\nfrom nanoatp import BskyAgent\n\nagent = BskyAgent("https://bsky.social")\nsession = agent.login()\n\nrecord = {"text": "Hello, world! 0"}\nr = agent.post(record)\nroot = r\nparent = r\n\nrecord = {"text": "Hello, world! 1", "reply": {"root": root, "parent": parent}}\nr = agent.post(record)\nparent = r\n\nimage = agent.uploadImage("favicon-16x16.png", "image/png")\nembed = {"$type": "app.bsky.embed.images#main", "images": [image]}\nrecord = {\n    "text": "Hello, world! 2",\n    "reply": {"root": root, "parent": parent},\n    "embed": embed\n}\nagent.post(record)\n```\n\n## Advanced\n\n### Advanced API calls\n\nThe methods above are convenience wrappers. It covers most but not all available methods.\n\nThe AT Protocol identifies methods and records with reverse-DNS names. You can use them on the agent as well:\n\n```python\nres1 = agent.createRecord(\n    agent.session["did"],  # repo\n    "app.bsky.feed.post",  # collection\n    {\n        "$type": "app.bsky.feed.post",  # record\n        "text": "Hello, world!",\n        "createdAt": datetime.datetime.now(datetime.timezone.utc).isoformat().replace("+00:00", "Z")\n    }\n)\n```\n\n## Development\n\n```bash\nexport ATP_IDENTIFIER="foo.bsky.social"\nexport ATP_PASSWORD="password"\npoetry install\npoetry run pytest -s     # run pytest once\npoetry run -- ptw -- -s  # run pytest and watch for changes\n```\n\n## License\n\nMIT License. See [LICENSE](LICENSE) for details.\n\n## Author\n\nSusumu Ota\n',
     'author': 'Susumu OTA',
     'author_email': '1632335+susumuota@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `nanoatp-0.1.0/PKG-INFO` & `nanoatp-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanoatp
-Version: 0.1.0
+Version: 0.2.0
 Summary: nano implementation of the AT Protocol (Authenticated Transfer Protocol)
 Author: Susumu OTA
 Author-email: 1632335+susumuota@users.noreply.github.com
 Requires-Python: >=3.9.16,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -24,48 +24,77 @@
 ```
 
 Then in your application:
 
 ```python
 from nanoatp import BskyAgent
 
-agent = new BskyAgent("https://bsky.social")
+agent = BskyAgent("https://bsky.social")
 ```
 
 ## Usage
 
 ### Session management
 
 Log into a server using these APIs. You'll need an active session for most methods.
 
 ```python
 from nanoatp import BskyAgent
 
-agent = new BskyAgent("https://bsky.social")
+agent = BskyAgent("https://bsky.social")
 
 agent.login('alice@mail.com', 'hunter2')
 
 # if you don't specify credentials, ATP_IDENTIFIER and ATP_PASSWORD environment variables will be used
 # agent.login()
 ```
 
 ### API calls
 
 The agent includes methods for many common operations, including:
 
 ```python
 # Feeds and content
+agent.getPost(repo, rkey, cid)
 agent.post(record)
-agent.uploadBlob(data, contentType)
-agent.uploadImage(path, alt, contentType)
+agent.deletePost(postUri)
+agent.uploadBlob(data, encoding)
+agent.uploadImage(path, alt, encoding)  # wrapper for uploadBlob
 
 # Session management
 agent.login(identifier, password)
 ```
 
+For example, to post a record, reply to it, and upload an image:
+
+```python
+from nanoatp import BskyAgent
+
+agent = BskyAgent("https://bsky.social")
+session = agent.login()
+
+record = {"text": "Hello, world! 0"}
+r = agent.post(record)
+root = r
+parent = r
+
+record = {"text": "Hello, world! 1", "reply": {"root": root, "parent": parent}}
+r = agent.post(record)
+parent = r
+
+image = agent.uploadImage("favicon-16x16.png", "image/png")
+embed = {"$type": "app.bsky.embed.images#main", "images": [image]}
+record = {
+    "text": "Hello, world! 2",
+    "reply": {"root": root, "parent": parent},
+    "embed": embed
+}
+agent.post(record)
+```
+
 ## Advanced
 
 ### Advanced API calls
 
 The methods above are convenience wrappers. It covers most but not all available methods.
 
 The AT Protocol identifies methods and records with reverse-DNS names. You can use them on the agent as well:
```

