# Comparing `tmp/django_upload_to-0.2.0.tar.gz` & `tmp/django_upload_to-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_upload_to-0.2.0.tar", max compression
+gzip compressed data, was "django_upload_to-0.3.0.tar", max compression
```

## Comparing `django_upload_to-0.2.0.tar` & `django_upload_to-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1067 2023-04-16 00:50:05.387812 django_upload_to-0.2.0/LICENSE
--rw-r--r--   0        0        0     2957 2023-04-16 00:50:05.387812 django_upload_to-0.2.0/README.md
--rw-r--r--   0        0        0     1997 2023-04-16 00:50:05.387812 django_upload_to-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4502 2023-04-16 00:50:05.387812 django_upload_to-0.2.0/upload_to/__init__.py
--rw-r--r--   0        0        0     3785 1970-01-01 00:00:00.000000 django_upload_to-0.2.0/setup.py
--rw-r--r--   0        0        0     4704 1970-01-01 00:00:00.000000 django_upload_to-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-16 03:36:27.236923 django_upload_to-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3173 2023-04-16 03:36:27.236923 django_upload_to-0.3.0/README.md
+-rw-r--r--   0        0        0     2116 2023-04-16 03:36:27.236923 django_upload_to-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4502 2023-04-16 03:36:27.236923 django_upload_to-0.3.0/upload_to/__init__.py
+-rw-r--r--   0        0        0     4001 1970-01-01 00:00:00.000000 django_upload_to-0.3.0/setup.py
+-rw-r--r--   0        0        0     5014 1970-01-01 00:00:00.000000 django_upload_to-0.3.0/PKG-INFO
```

### Comparing `django_upload_to-0.2.0/LICENSE` & `django_upload_to-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_upload_to-0.2.0/README.md` & `django_upload_to-0.3.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -97,8 +97,14 @@
     filename = upload_to.uuid_filename(filename)
     path = upload_to.options_from_instance(instance)
     return upload_to.upload_to(path, filename)
 
 class MyProfile(models.Model):
     user = models.OneToOneField(...)
     avatar = models.FileField(upload_to=my_upload_generator)
-```
+```
+
+## Useful links
+
+1. [Documentation](https://valbertovc.github.io/django-upload-to/)
+2. [Changelog](https://github.com/valbertovc/django-upload-to/releases)
+3. [PyPi Page](https://pypi.org/project/django-upload-to/)
```

### Comparing `django_upload_to-0.2.0/pyproject.toml` & `django_upload_to-0.3.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "django-upload-to"
-version = "0.2.0"
+version = "0.3.0"
 description = "It generates dynamically a directory path and a file name for Django FileField"
 authors = ["Valberto Carneiro <valbertovc@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/valbertovc/django-upload-to"
 classifiers=[
     "Development Status :: 4 - Beta",
     "Framework :: Django :: 2",
@@ -34,26 +34,29 @@
     { include = "upload_to" }
 ]
 include = [
 "LICENSE",
 ]
 
 [tool.poetry.urls]
-"Homepage" = "https://github.com/valbertovc/django-upload-to"
+"Homepage" = "https://valbertovc.github.io/django-upload-to/"
 "Source" = "https://github.com/valbertovc/django-upload-to"
 "Bug Tracker" = "https://github.com/valbertovc/django-upload-to/issues"
+"Changelog" = "https://github.com/valbertovc/django-upload-to/releases"
 
 [tool.poetry.dependencies]
-python = "^3.7.0"
+python = ">=3.8,<4"
 Django = ">=2.2.0,>=3.0.0,>=4.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^2.15.0"
 tox = "^4.4.5"
 coverage = {extras = ["toml"], version = "^7.1.0"}
+mkdocs = "^1.4.2"
+mkdocs-material = "^9.1.6"
 
 [tool.pylint."MESSAGES CONTROL"]
 disable = [
     "missing-module-docstring",
     "missing-class-docstring",
     "missing-function-docstring",
     "import-error",
```

### Comparing `django_upload_to-0.2.0/upload_to/__init__.py` & `django_upload_to-0.3.0/upload_to/__init__.py`

 * *Files identical despite different names*

### Comparing `django_upload_to-0.2.0/setup.py` & `django_upload_to-0.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 {'': ['*']}
 
 install_requires = \
 ['Django>=4.0.0']
 
 setup_kwargs = {
     'name': 'django-upload-to',
-    'version': '0.2.0',
+    'version': '0.3.0',
     'description': 'It generates dynamically a directory path and a file name for Django FileField',
-    'long_description': '# django-upload-to\n\n[![codecov](https://codecov.io/github/valbertovc/django-upload-to/branch/main/graph/badge.svg?token=2R5S5GTS0X)](https://codecov.io/github/valbertovc/django-upload-to)\n\nIt generates dynamically a directory path and a secure file name for Django FileField.\n\nMain options:\n- Ready to use generators.\n- Generate secure file name without especial characters.\n- Generate file name using a uuid value.\n- Dynamically generate paths from the model instance.\n- Generate paths using Python datetime formats.\n\n## Get started\nInstall the django-upload-to in your virtual environment\n```bash\n$ pip install django-upload-to\n```\nImport it in your models file and add it as a `upload_to` argument in the `FileField` \n```python\n# my_app/models.py\nfrom upload_to import UploadTo\nfrom django.db import models\n\n\nclass MyModel(models.Model):\n    attachment = models.FileField(upload_to=UploadTo("attachments"))\n```\nThe path and file name generated will be like this:\n```text\n"attachments/the-file-name-uploaded.pdf"\n```\n\n## How to use the ready-to-use classes\n\nConsider the scenario below:\n```python\nimport upload_to\nfrom django.db import models\n\n\nclass MyUser(models.Model):\n    username = models.CharField(...)\n    avatar = models.FileField(upload_to=<generator>)\n\ninstance = MyUser(username=\'user@email.com\')\n```\nReplace the `<generator>` fragment by the generators as showed below:\n#### File in root folder\n```python\n>>> generator = upload_to.UploadTo()\n>>> generator(instance, "file.pdf")\n"file.pdf"\n\n```\n#### Define a folder structure\n```python\n>>> generator = upload_to.UploadTo(prefix=["files", "documents"])\n>>> generator(instance, "file.pdf")\n"files/documents/file.pdf"\n```\n#### Generate a folder name using datetime formats from Python\n```python\n>>> generator = upload_to.UploadTo(prefix=["pictures", "%Y"])\n>>> generator(instance, "file.png")\n"pictures/2023/file.png"\n```\n#### Replace the file name by an hexadecimal uuid value\n```python\n# 4. replace file name by a uuid value\n>>> generator = upload_to.UuidUploadTo()\n>>> generator(instance, "file.pdf")\n"b189dfdf25e640b2ba5c497472c20962.pdf"\n```\n#### Generate the folder path using the instance\'s attributes\n```python\n>>> generator = upload_to.AttrUploadTo(attrs=["username"])\n>>> generator(instance, "file.pdf")\n"useremailcom/file.pdf"\n```\n#### Generate the folder path using the app_label and the model_name from the instance\'s meta options\n```python\n>>> generator = upload_to.ModelUploadTo()\n>>> generator(instance, "file.pdf")\n"my_app/user/file.pdf"\n```\n\n## Customize your upload paths\n\n```python\n# my_app/models.py\nimport upload_to\nfrom django.db import models\n\n\ndef my_upload_generator(instance, filename):\n    filename = upload_to.uuid_filename(filename)\n    path = upload_to.options_from_instance(instance)\n    return upload_to.upload_to(path, filename)\n\nclass MyProfile(models.Model):\n    user = models.OneToOneField(...)\n    avatar = models.FileField(upload_to=my_upload_generator)\n```',
+    'long_description': '# django-upload-to\n\n[![codecov](https://codecov.io/github/valbertovc/django-upload-to/branch/main/graph/badge.svg?token=2R5S5GTS0X)](https://codecov.io/github/valbertovc/django-upload-to)\n\nIt generates dynamically a directory path and a secure file name for Django FileField.\n\nMain options:\n- Ready to use generators.\n- Generate secure file name without especial characters.\n- Generate file name using a uuid value.\n- Dynamically generate paths from the model instance.\n- Generate paths using Python datetime formats.\n\n## Get started\nInstall the django-upload-to in your virtual environment\n```bash\n$ pip install django-upload-to\n```\nImport it in your models file and add it as a `upload_to` argument in the `FileField` \n```python\n# my_app/models.py\nfrom upload_to import UploadTo\nfrom django.db import models\n\n\nclass MyModel(models.Model):\n    attachment = models.FileField(upload_to=UploadTo("attachments"))\n```\nThe path and file name generated will be like this:\n```text\n"attachments/the-file-name-uploaded.pdf"\n```\n\n## How to use the ready-to-use classes\n\nConsider the scenario below:\n```python\nimport upload_to\nfrom django.db import models\n\n\nclass MyUser(models.Model):\n    username = models.CharField(...)\n    avatar = models.FileField(upload_to=<generator>)\n\ninstance = MyUser(username=\'user@email.com\')\n```\nReplace the `<generator>` fragment by the generators as showed below:\n#### File in root folder\n```python\n>>> generator = upload_to.UploadTo()\n>>> generator(instance, "file.pdf")\n"file.pdf"\n\n```\n#### Define a folder structure\n```python\n>>> generator = upload_to.UploadTo(prefix=["files", "documents"])\n>>> generator(instance, "file.pdf")\n"files/documents/file.pdf"\n```\n#### Generate a folder name using datetime formats from Python\n```python\n>>> generator = upload_to.UploadTo(prefix=["pictures", "%Y"])\n>>> generator(instance, "file.png")\n"pictures/2023/file.png"\n```\n#### Replace the file name by an hexadecimal uuid value\n```python\n# 4. replace file name by a uuid value\n>>> generator = upload_to.UuidUploadTo()\n>>> generator(instance, "file.pdf")\n"b189dfdf25e640b2ba5c497472c20962.pdf"\n```\n#### Generate the folder path using the instance\'s attributes\n```python\n>>> generator = upload_to.AttrUploadTo(attrs=["username"])\n>>> generator(instance, "file.pdf")\n"useremailcom/file.pdf"\n```\n#### Generate the folder path using the app_label and the model_name from the instance\'s meta options\n```python\n>>> generator = upload_to.ModelUploadTo()\n>>> generator(instance, "file.pdf")\n"my_app/user/file.pdf"\n```\n\n## Customize your upload paths\n\n```python\n# my_app/models.py\nimport upload_to\nfrom django.db import models\n\n\ndef my_upload_generator(instance, filename):\n    filename = upload_to.uuid_filename(filename)\n    path = upload_to.options_from_instance(instance)\n    return upload_to.upload_to(path, filename)\n\nclass MyProfile(models.Model):\n    user = models.OneToOneField(...)\n    avatar = models.FileField(upload_to=my_upload_generator)\n```\n\n## Useful links\n\n1. [Documentation](https://valbertovc.github.io/django-upload-to/)\n2. [Changelog](https://github.com/valbertovc/django-upload-to/releases)\n3. [PyPi Page](https://pypi.org/project/django-upload-to/)',
     'author': 'Valberto Carneiro',
     'author_email': 'valbertovc@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/valbertovc/django-upload-to',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.7.0,<4.0.0',
+    'python_requires': '>=3.8,<4',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `django_upload_to-0.2.0/PKG-INFO` & `django_upload_to-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 Metadata-Version: 2.1
 Name: django-upload-to
-Version: 0.2.0
+Version: 0.3.0
 Summary: It generates dynamically a directory path and a file name for Django FileField
 Home-page: https://github.com/valbertovc/django-upload-to
 Keywords: django,file,media,upload
 Author: Valberto Carneiro
 Author-email: valbertovc@gmail.com
-Requires-Python: >=3.7.0,<4.0.0
+Requires-Python: >=3.8,<4
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django :: 2
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4
 Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Multimedia
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Dist: Django (>=4.0.0)
 Project-URL: Bug Tracker, https://github.com/valbertovc/django-upload-to/issues
+Project-URL: Changelog, https://github.com/valbertovc/django-upload-to/releases
+Project-URL: Homepage, https://valbertovc.github.io/django-upload-to/
 Project-URL: Repository, https://github.com/valbertovc/django-upload-to
 Project-URL: Source, https://github.com/valbertovc/django-upload-to
 Description-Content-Type: text/markdown
 
 # django-upload-to
 
 [![codecov](https://codecov.io/github/valbertovc/django-upload-to/branch/main/graph/badge.svg?token=2R5S5GTS0X)](https://codecov.io/github/valbertovc/django-upload-to)
@@ -137,7 +138,13 @@
     path = upload_to.options_from_instance(instance)
     return upload_to.upload_to(path, filename)
 
 class MyProfile(models.Model):
     user = models.OneToOneField(...)
     avatar = models.FileField(upload_to=my_upload_generator)
 ```
+
+## Useful links
+
+1. [Documentation](https://valbertovc.github.io/django-upload-to/)
+2. [Changelog](https://github.com/valbertovc/django-upload-to/releases)
+3. [PyPi Page](https://pypi.org/project/django-upload-to/)
```

