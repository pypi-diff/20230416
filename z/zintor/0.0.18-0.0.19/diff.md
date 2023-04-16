# Comparing `tmp/zintor-0.0.18.tar.gz` & `tmp/zintor-0.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zintor-0.0.18.tar", last modified: Sat Apr 15 08:32:44 2023, max compression
+gzip compressed data, was "zintor-0.0.19.tar", last modified: Sun Apr 16 07:21:30 2023, max compression
```

## Comparing `zintor-0.0.18.tar` & `zintor-0.0.19.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 dzung     (1000) dzung     (1000)        0 2023-04-15 08:32:44.374474 zintor-0.0.18/
--rw-r--r--   0 dzung     (1000) dzung     (1000)      383 2023-04-15 08:32:44.374474 zintor-0.0.18/PKG-INFO
--rw-r--r--   0 dzung     (1000) dzung     (1000)       38 2023-04-15 08:32:44.374474 zintor-0.0.18/setup.cfg
--rw-r--r--   0 dzung     (1000) dzung     (1000)     1362 2023-04-15 08:32:40.000000 zintor-0.0.18/setup.py
-drwxr-xr-x   0 dzung     (1000) dzung     (1000)        0 2023-04-15 08:32:44.374474 zintor-0.0.18/zintor/
-drwxr-xr-x   0 dzung     (1000) dzung     (1000)        0 2023-04-15 08:32:44.374474 zintor-0.0.18/zintor/src/
-drwxr-xr-x   0 dzung     (1000) dzung     (1000)        0 2023-04-15 08:32:44.374474 zintor-0.0.18/zintor/src/zintor.egg-info/
--rw-r--r--   0 dzung     (1000) dzung     (1000)      383 2023-04-15 08:32:44.000000 zintor-0.0.18/zintor/src/zintor.egg-info/PKG-INFO
--rw-r--r--   0 dzung     (1000) dzung     (1000)      233 2023-04-15 08:32:44.000000 zintor-0.0.18/zintor/src/zintor.egg-info/SOURCES.txt
--rw-r--r--   0 dzung     (1000) dzung     (1000)        1 2023-04-15 08:32:44.000000 zintor-0.0.18/zintor/src/zintor.egg-info/dependency_links.txt
--rw-r--r--   0 dzung     (1000) dzung     (1000)       74 2023-04-15 08:32:44.000000 zintor-0.0.18/zintor/src/zintor.egg-info/requires.txt
--rw-r--r--   0 dzung     (1000) dzung     (1000)        7 2023-04-15 08:32:44.000000 zintor-0.0.18/zintor/src/zintor.egg-info/top_level.txt
--rw-r--r--   0 dzung     (1000) dzung     (1000)     3130 2023-04-15 08:25:00.000000 zintor-0.0.18/zintor/src/zintor.py
+drwxr-xr-x   0 dzung     (1000) dzung     (1000)        0 2023-04-16 07:21:30.114382 zintor-0.0.19/
+-rw-r--r--   0 dzung     (1000) dzung     (1000)      383 2023-04-16 07:21:30.114382 zintor-0.0.19/PKG-INFO
+-rw-r--r--   0 dzung     (1000) dzung     (1000)       38 2023-04-16 07:21:30.114382 zintor-0.0.19/setup.cfg
+-rw-r--r--   0 dzung     (1000) dzung     (1000)     1362 2023-04-16 07:21:14.000000 zintor-0.0.19/setup.py
+drwxr-xr-x   0 dzung     (1000) dzung     (1000)        0 2023-04-16 07:21:30.114382 zintor-0.0.19/zintor/
+drwxr-xr-x   0 dzung     (1000) dzung     (1000)        0 2023-04-16 07:21:30.114382 zintor-0.0.19/zintor/src/
+drwxr-xr-x   0 dzung     (1000) dzung     (1000)        0 2023-04-16 07:21:30.114382 zintor-0.0.19/zintor/src/zintor.egg-info/
+-rw-r--r--   0 dzung     (1000) dzung     (1000)      383 2023-04-16 07:21:30.000000 zintor-0.0.19/zintor/src/zintor.egg-info/PKG-INFO
+-rw-r--r--   0 dzung     (1000) dzung     (1000)      233 2023-04-16 07:21:30.000000 zintor-0.0.19/zintor/src/zintor.egg-info/SOURCES.txt
+-rw-r--r--   0 dzung     (1000) dzung     (1000)        1 2023-04-16 07:21:30.000000 zintor-0.0.19/zintor/src/zintor.egg-info/dependency_links.txt
+-rw-r--r--   0 dzung     (1000) dzung     (1000)       74 2023-04-16 07:21:30.000000 zintor-0.0.19/zintor/src/zintor.egg-info/requires.txt
+-rw-r--r--   0 dzung     (1000) dzung     (1000)        7 2023-04-16 07:21:30.000000 zintor-0.0.19/zintor/src/zintor.egg-info/top_level.txt
+-rw-r--r--   0 dzung     (1000) dzung     (1000)     3160 2023-04-16 07:20:56.000000 zintor-0.0.19/zintor/src/zintor.py
```

### Comparing `zintor-0.0.18/setup.py` & `zintor-0.0.19/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("readme.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="zintor",                             # This is the name of the package
-    version="0.0.18",                        # The initial release version
+    version="0.0.19",                        # The initial release version
     author="__Async__",                     # Full name of the author
     description="Python Admin Package",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `zintor-0.0.18/zintor/src/zintor.py` & `zintor-0.0.19/zintor/src/zintor.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,39 +43,39 @@
     pass
 
 class ImageView(ModelView):
     def _list_thumbnail(view, context, model, name):
         if not model.path:
             return ''
         return Markup('<img src="%s">' % url_for('static',
-                                                 filename=form.thumbgen_filename(model.path)))
+                                                 filename='upload/%s' % (form.thumbgen_filename(model.path))))
 
     column_formatters = {
         'path': _list_thumbnail
     }
 
     # Alternative way to contribute field is to override it completely.
     # In this case, Flask-Admin won't attempt to merge various parameters for the field.
     form_extra_fields = {
         'path': form.ImageUploadField(
             '画像',
-            base_path='static',
+            base_path='static/upload',
             allowed_extensions=('jpeg', 'jpg', 'png'),
             thumbnail_size=(100, 100, True),
             max_size=(2048, 2048, True),
             namegen=prefix_name,
         )
     }
     
 class ImageInlineModelForm(InlineFormAdmin):
     form_columns = ('id', 'path')
     form_extra_fields = {
         'path': form.ImageUploadField(
             '画像',
-            base_path='static',
+            base_path='static/upload',
             allowed_extensions=('jpeg', 'jpg', 'png'),
             thumbnail_size=(100, 100, True),
             max_size=(2048, 2048, True),
             namegen=prefix_name,
         )
     }
```

