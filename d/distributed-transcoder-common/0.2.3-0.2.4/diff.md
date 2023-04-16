# Comparing `tmp/distributed-transcoder-common-0.2.3.tar.gz` & `tmp/distributed-transcoder-common-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "distributed-transcoder-common-0.2.3.tar", max compression
+gzip compressed data, was "distributed-transcoder-common-0.2.4.tar", max compression
```

## Comparing `distributed-transcoder-common-0.2.3.tar` & `distributed-transcoder-common-0.2.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       86 2023-04-04 05:32:08.748355 distributed-transcoder-common-0.2.3/distributed_transcoder_common/__init__.py
--rw-r--r--   0        0        0      416 2023-04-04 05:06:21.155583 distributed-transcoder-common-0.2.3/distributed_transcoder_common/message_types.py
--rw-r--r--   0        0        0     1742 2023-04-15 06:23:13.897558 distributed-transcoder-common-0.2.3/distributed_transcoder_common/models.py
--rw-r--r--   0        0        0      390 2023-04-15 06:23:45.593207 distributed-transcoder-common-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      695 2023-04-15 06:23:48.866363 distributed-transcoder-common-0.2.3/setup.py
--rw-r--r--   0        0        0      422 2023-04-15 06:23:48.866566 distributed-transcoder-common-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0       86 2023-04-04 05:32:08.748355 distributed-transcoder-common-0.2.4/distributed_transcoder_common/__init__.py
+-rw-r--r--   0        0        0      416 2023-04-04 05:06:21.155583 distributed-transcoder-common-0.2.4/distributed_transcoder_common/message_types.py
+-rw-r--r--   0        0        0     1907 2023-04-16 03:00:08.313542 distributed-transcoder-common-0.2.4/distributed_transcoder_common/models.py
+-rw-r--r--   0        0        0      390 2023-04-16 03:00:55.472977 distributed-transcoder-common-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      695 2023-04-16 03:00:59.864056 distributed-transcoder-common-0.2.4/setup.py
+-rw-r--r--   0        0        0      422 2023-04-16 03:00:59.864263 distributed-transcoder-common-0.2.4/PKG-INFO
```

### Comparing `distributed-transcoder-common-0.2.3/distributed_transcoder_common/models.py` & `distributed-transcoder-common-0.2.4/distributed_transcoder_common/models.py`

 * *Files 23% similar despite different names*

```diff
@@ -21,23 +21,29 @@
         ordering = ["name"]
 
     class PydanticMeta:
         exclude = ("jobs",)
 
 
 class Job(Model):
+    STATE_QUEUED = "queued"
+    STATE_IN_PROGRESS = "in-progress"
+    STATE_FINISHED = "finished"
+    STATE_FAILED = "failed"
+    STATE_CANCELLED = "cancelled"
+
     id = fields.UUIDField(pk=True)
     job_id = fields.CharField(max_length=50, unique=True)
     input_s3_path = fields.CharField(max_length=255)
     output_s3_path = fields.CharField(max_length=255)
     pipeline = fields.TextField()
     preset: fields.ForeignKeyNullableRelation[Preset] = fields.ForeignKeyField(
         "models.Preset", null=True
     )
-    state = fields.CharField(max_length=20, default="queued")
+    state = fields.CharField(max_length=20, default=STATE_QUEUED)
     error = fields.TextField(null=True)
     error_type = fields.CharField(max_length=50, null=True)
     created_at = fields.DatetimeField(auto_now_add=True)
     updated_at = fields.DatetimeField(auto_now=True)
 
     class Meta:
         ordering = ["-created_at"]
```

### Comparing `distributed-transcoder-common-0.2.3/setup.py` & `distributed-transcoder-common-0.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['tortoise-orm>=0.19.3,<0.20.0']
 
 setup_kwargs = {
     'name': 'distributed-transcoder-common',
-    'version': '0.2.3',
+    'version': '0.2.4',
     'description': 'A common library for for the distributed transcoder project',
     'long_description': None,
     'author': 'Eric Volpert',
     'author_email': 'ericvolp12@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

