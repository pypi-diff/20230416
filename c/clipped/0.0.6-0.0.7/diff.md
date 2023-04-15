# Comparing `tmp/clipped-0.0.6.tar.gz` & `tmp/clipped-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clipped-0.0.6.tar", last modified: Thu Apr 13 08:14:35 2023, max compression
+gzip compressed data, was "clipped-0.0.7.tar", last modified: Sat Apr 15 22:49:42 2023, max compression
```

## Comparing `clipped-0.0.6.tar` & `clipped-0.0.7.tar`

### file list

```diff
@@ -1,58 +1,79 @@
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-13 08:14:35.493667 clipped-0.0.6/
--rw-r--r--   0 mourad     (501) staff       (20)      174 2023-04-13 08:13:58.000000 clipped-0.0.6/MANIFEST.in
--rw-r--r--   0 mourad     (501) staff       (20)     2012 2023-04-13 08:14:35.493773 clipped-0.0.6/PKG-INFO
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-13 08:14:35.486666 clipped-0.0.6/clipped/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-13 08:13:58.000000 clipped-0.0.6/clipped/__init__.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-13 08:14:35.488190 clipped-0.0.6/clipped/decorators/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-13 08:13:58.000000 clipped-0.0.6/clipped/decorators/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)      646 2023-04-13 08:13:58.000000 clipped-0.0.6/clipped/decorators/cached_property.py
--rw-r--r--   0 mourad     (501) staff       (20)     4355 2023-04-13 08:13:58.000000 clipped-0.0.6/clipped/decorators/deprecation.py
--rw-r--r--   0 mourad     (501) staff       (20)     1923 2023-04-13 08:13:58.000000 clipped-0.0.6/clipped/decorators/memoization.py
--rw-r--r--   0 mourad     (501) staff       (20)     2686 2023-04-13 08:13:58.000000 clipped-0.0.6/clipped/decorators/signals.py
--rw-r--r--   0 mourad     (501) staff       (20)     6224 2023-04-13 08:13:58.000000 clipped-0.0.6/clipped/formatting.py
--rw-r--r--   0 mourad     (501) staff       (20)      824 2023-04-13 08:13:58.000000 clipped-0.0.6/clipped/manager_interface.py
--rw-r--r--   0 mourad     (501) staff       (20)      203 2023-04-13 08:13:58.000000 clipped-0.0.6/clipped/pkg.py
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-13 08:13:58.000000 clipped-0.0.6/clipped/py.typed
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-13 08:14:35.493524 clipped-0.0.6/clipped/utils/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-13 08:13:58.000000 clipped-0.0.6/clipped/utils/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     1004 2023-04-13 08:13:58.000000 clipped-0.0.6/clipped/utils/bools.py
--rw-r--r--   0 mourad     (501) staff       (20)      143 2023-04-13 08:13:58.000000 clipped-0.0.6/clipped/utils/click.py
--rw-r--r--   0 mourad     (501) staff       (20)      665 2023-04-13 08:13:58.000000 clipped-0.0.6/clipped/utils/cmd.py
--rw-r--r--   0 mourad     (501) staff       (20)      570 2023-04-13 08:13:58.000000 clipped-0.0.6/clipped/utils/coroutine.py
--rw-r--r--   0 mourad     (501) staff       (20)      755 2023-04-13 08:13:58.000000 clipped-0.0.6/clipped/utils/csv.py
--rw-r--r--   0 mourad     (501) staff       (20)     7568 2023-04-13 08:13:58.000000 clipped-0.0.6/clipped/utils/dates.py
--rw-r--r--   0 mourad     (501) staff       (20)     3354 2023-04-13 08:13:58.000000 clipped-0.0.6/clipped/utils/dicts.py
--rw-r--r--   0 mourad     (501) staff       (20)      496 2023-04-13 08:13:58.000000 clipped-0.0.6/clipped/utils/encoding.py
--rw-r--r--   0 mourad     (501) staff       (20)     1093 2023-04-13 08:13:58.000000 clipped-0.0.6/clipped/utils/enums.py
--rw-r--r--   0 mourad     (501) staff       (20)     2001 2023-04-13 08:13:58.000000 clipped-0.0.6/clipped/utils/env.py
--rw-r--r--   0 mourad     (501) staff       (20)     4737 2023-04-13 08:13:58.000000 clipped-0.0.6/clipped/utils/git.py
--rw-r--r--   0 mourad     (501) staff       (20)     1827 2023-04-13 08:13:58.000000 clipped-0.0.6/clipped/utils/hashing.py
--rw-r--r--   0 mourad     (501) staff       (20)     1175 2023-04-13 08:13:58.000000 clipped-0.0.6/clipped/utils/http.py
--rw-r--r--   0 mourad     (501) staff       (20)     3363 2023-04-13 08:13:58.000000 clipped-0.0.6/clipped/utils/humanize.py
--rw-r--r--   0 mourad     (501) staff       (20)     1327 2023-04-13 08:13:58.000000 clipped-0.0.6/clipped/utils/imports.py
--rw-r--r--   0 mourad     (501) staff       (20)     1695 2023-04-13 08:13:58.000000 clipped-0.0.6/clipped/utils/indentation.py
--rw-r--r--   0 mourad     (501) staff       (20)      287 2023-04-13 08:13:58.000000 clipped-0.0.6/clipped/utils/json.py
--rw-r--r--   0 mourad     (501) staff       (20)      894 2023-04-13 08:13:58.000000 clipped-0.0.6/clipped/utils/lists.py
--rw-r--r--   0 mourad     (501) staff       (20)      113 2023-04-13 08:13:58.000000 clipped-0.0.6/clipped/utils/logging.py
--rw-r--r--   0 mourad     (501) staff       (20)     1280 2023-04-13 08:13:58.000000 clipped-0.0.6/clipped/utils/np.py
--rw-r--r--   0 mourad     (501) staff       (20)     8484 2023-04-13 08:13:58.000000 clipped-0.0.6/clipped/utils/paths.py
--rw-r--r--   0 mourad     (501) staff       (20)      674 2023-04-13 08:13:58.000000 clipped-0.0.6/clipped/utils/query_params.py
--rw-r--r--   0 mourad     (501) staff       (20)     1134 2023-04-13 08:13:58.000000 clipped-0.0.6/clipped/utils/requests.py
--rw-r--r--   0 mourad     (501) staff       (20)     1041 2023-04-13 08:13:58.000000 clipped-0.0.6/clipped/utils/responses.py
--rw-r--r--   0 mourad     (501) staff       (20)      559 2023-04-13 08:13:58.000000 clipped-0.0.6/clipped/utils/sanitizers.py
--rw-r--r--   0 mourad     (501) staff       (20)      676 2023-04-13 08:13:58.000000 clipped-0.0.6/clipped/utils/serialization.py
--rw-r--r--   0 mourad     (501) staff       (20)     2339 2023-04-13 08:13:58.000000 clipped-0.0.6/clipped/utils/strings.py
--rw-r--r--   0 mourad     (501) staff       (20)     1115 2023-04-13 08:13:58.000000 clipped-0.0.6/clipped/utils/tz.py
--rw-r--r--   0 mourad     (501) staff       (20)     4040 2023-04-13 08:13:58.000000 clipped-0.0.6/clipped/utils/units.py
--rw-r--r--   0 mourad     (501) staff       (20)      269 2023-04-13 08:13:58.000000 clipped-0.0.6/clipped/utils/urls.py
--rw-r--r--   0 mourad     (501) staff       (20)      614 2023-04-13 08:13:58.000000 clipped-0.0.6/clipped/utils/validation.py
--rw-r--r--   0 mourad     (501) staff       (20)     1128 2023-04-13 08:13:58.000000 clipped-0.0.6/clipped/utils/versions.py
--rw-r--r--   0 mourad     (501) staff       (20)     1068 2023-04-13 08:13:58.000000 clipped-0.0.6/clipped/utils/workers.py
--rw-r--r--   0 mourad     (501) staff       (20)      546 2023-04-13 08:13:58.000000 clipped-0.0.6/clipped/utils/yaml.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-13 08:14:35.487321 clipped-0.0.6/clipped.egg-info/
--rw-r--r--   0 mourad     (501) staff       (20)     2012 2023-04-13 08:14:35.000000 clipped-0.0.6/clipped.egg-info/PKG-INFO
--rw-r--r--   0 mourad     (501) staff       (20)     1318 2023-04-13 08:14:35.000000 clipped-0.0.6/clipped.egg-info/SOURCES.txt
--rw-r--r--   0 mourad     (501) staff       (20)        1 2023-04-13 08:14:35.000000 clipped-0.0.6/clipped.egg-info/dependency_links.txt
--rw-r--r--   0 mourad     (501) staff       (20)        8 2023-04-13 08:14:35.000000 clipped-0.0.6/clipped.egg-info/top_level.txt
--rw-r--r--   0 mourad     (501) staff       (20)     1033 2023-04-13 08:14:35.494289 clipped-0.0.6/setup.cfg
--rw-r--r--   0 mourad     (501) staff       (20)     2345 2023-04-13 08:13:58.000000 clipped-0.0.6/setup.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-15 22:49:42.692404 clipped-0.0.7/
+-rw-r--r--   0 mourad     (501) staff       (20)      174 2023-04-15 22:49:06.000000 clipped-0.0.7/MANIFEST.in
+-rw-r--r--   0 mourad     (501) staff       (20)     2012 2023-04-15 22:49:42.692516 clipped-0.0.7/PKG-INFO
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-15 22:49:42.682006 clipped-0.0.7/clipped/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/__init__.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-15 22:49:42.683992 clipped-0.0.7/clipped/config/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/config/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)       91 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/config/constants.py
+-rw-r--r--   0 mourad     (501) staff       (20)       40 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/config/exceptions.py
+-rw-r--r--   0 mourad     (501) staff       (20)     4022 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/config/manager.py
+-rw-r--r--   0 mourad     (501) staff       (20)     6135 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/config/parser.py
+-rw-r--r--   0 mourad     (501) staff       (20)      527 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/config/patch_strategy.py
+-rw-r--r--   0 mourad     (501) staff       (20)    14929 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/config/schema.py
+-rw-r--r--   0 mourad     (501) staff       (20)     8856 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/config/spec.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-15 22:49:42.684789 clipped-0.0.7/clipped/decorators/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/decorators/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)      646 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/decorators/cached_property.py
+-rw-r--r--   0 mourad     (501) staff       (20)     4355 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/decorators/deprecation.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1923 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/decorators/memoization.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2686 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/decorators/signals.py
+-rw-r--r--   0 mourad     (501) staff       (20)     6224 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/formatting.py
+-rw-r--r--   0 mourad     (501) staff       (20)      824 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/manager_interface.py
+-rw-r--r--   0 mourad     (501) staff       (20)      203 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/pkg.py
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/py.typed
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-15 22:49:42.686509 clipped-0.0.7/clipped/types/
+-rw-r--r--   0 mourad     (501) staff       (20)     3868 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/types/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1298 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/types/docker_image.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1889 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/types/email.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1081 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/types/gcs.py
+-rw-r--r--   0 mourad     (501) staff       (20)      693 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/types/lists.py
+-rw-r--r--   0 mourad     (501) staff       (20)      158 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/types/numbers.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1142 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/types/ref_or_obj.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1065 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/types/s3.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1265 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/types/uri.py
+-rw-r--r--   0 mourad     (501) staff       (20)      683 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/types/uuids.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3229 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/types/wasb.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-15 22:49:42.692242 clipped-0.0.7/clipped/utils/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1004 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/bools.py
+-rw-r--r--   0 mourad     (501) staff       (20)      143 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/click.py
+-rw-r--r--   0 mourad     (501) staff       (20)      665 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/cmd.py
+-rw-r--r--   0 mourad     (501) staff       (20)      570 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/coroutine.py
+-rw-r--r--   0 mourad     (501) staff       (20)      755 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/csv.py
+-rw-r--r--   0 mourad     (501) staff       (20)     7568 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/dates.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3354 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/dicts.py
+-rw-r--r--   0 mourad     (501) staff       (20)      496 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/encoding.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1093 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/enums.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2001 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/env.py
+-rw-r--r--   0 mourad     (501) staff       (20)     4737 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/git.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1827 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/hashing.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1175 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/http.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3363 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/humanize.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1327 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/imports.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1695 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/indentation.py
+-rw-r--r--   0 mourad     (501) staff       (20)      287 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/json.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1170 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/lists.py
+-rw-r--r--   0 mourad     (501) staff       (20)      113 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/logging.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1280 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/np.py
+-rw-r--r--   0 mourad     (501) staff       (20)     8484 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/paths.py
+-rw-r--r--   0 mourad     (501) staff       (20)      674 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/query_params.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1134 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/requests.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1041 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/responses.py
+-rw-r--r--   0 mourad     (501) staff       (20)      559 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/sanitizers.py
+-rw-r--r--   0 mourad     (501) staff       (20)      676 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/serialization.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2674 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/strings.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1115 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/tz.py
+-rw-r--r--   0 mourad     (501) staff       (20)     4040 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/units.py
+-rw-r--r--   0 mourad     (501) staff       (20)      269 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/urls.py
+-rw-r--r--   0 mourad     (501) staff       (20)      614 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/validation.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1128 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/versions.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1068 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/workers.py
+-rw-r--r--   0 mourad     (501) staff       (20)      546 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/yaml.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-15 22:49:42.682648 clipped-0.0.7/clipped.egg-info/
+-rw-r--r--   0 mourad     (501) staff       (20)     2012 2023-04-15 22:49:42.000000 clipped-0.0.7/clipped.egg-info/PKG-INFO
+-rw-r--r--   0 mourad     (501) staff       (20)     1796 2023-04-15 22:49:42.000000 clipped-0.0.7/clipped.egg-info/SOURCES.txt
+-rw-r--r--   0 mourad     (501) staff       (20)        1 2023-04-15 22:49:42.000000 clipped-0.0.7/clipped.egg-info/dependency_links.txt
+-rw-r--r--   0 mourad     (501) staff       (20)        8 2023-04-15 22:49:42.000000 clipped-0.0.7/clipped.egg-info/top_level.txt
+-rw-r--r--   0 mourad     (501) staff       (20)     1033 2023-04-15 22:49:42.693029 clipped-0.0.7/setup.cfg
+-rw-r--r--   0 mourad     (501) staff       (20)     2345 2023-04-15 22:49:06.000000 clipped-0.0.7/setup.py
```

### Comparing `clipped-0.0.6/PKG-INFO` & `clipped-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipped
-Version: 0.0.6
+Version: 0.0.7
 Summary: Common shortcuts and utils.
 Home-page: https://github.com/mmourafiq/clipped
 Author: Mourad Mourafiq
 Author-email: mourad.mourafiq@gmail.com
 Maintainer: Mourad Mourafiq
 Maintainer-email: mourad.mourafiq@gmail.com
 License: Apache 2.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: clipped Version: 0.0.6 Summary: Common shortcuts
+Metadata-Version: 2.1 Name: clipped Version: 0.0.7 Summary: Common shortcuts
 and utils. Home-page: https://github.com/mmourafiq/clipped Author: Mourad
 Mourafiq Author-email: mourad.mourafiq@gmail.com Maintainer: Mourad Mourafiq
 Maintainer-email: mourad.mourafiq@gmail.com License: Apache 2.0 Keywords:
 cli,configuration,utils,setup Platform: any Classifier: Intended Audience ::
 Information Technology Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Science/Research Classifier: Operating System :: OS Independent Classifier:
```

### Comparing `clipped-0.0.6/clipped/decorators/cached_property.py` & `clipped-0.0.7/clipped/decorators/cached_property.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.6/clipped/decorators/deprecation.py` & `clipped-0.0.7/clipped/decorators/deprecation.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.6/clipped/decorators/memoization.py` & `clipped-0.0.7/clipped/decorators/memoization.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.6/clipped/decorators/signals.py` & `clipped-0.0.7/clipped/decorators/signals.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.6/clipped/formatting.py` & `clipped-0.0.7/clipped/formatting.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.6/clipped/manager_interface.py` & `clipped-0.0.7/clipped/manager_interface.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.6/clipped/utils/bools.py` & `clipped-0.0.7/clipped/utils/bools.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.6/clipped/utils/cmd.py` & `clipped-0.0.7/clipped/utils/cmd.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.6/clipped/utils/coroutine.py` & `clipped-0.0.7/clipped/utils/coroutine.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.6/clipped/utils/csv.py` & `clipped-0.0.7/clipped/utils/csv.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.6/clipped/utils/dates.py` & `clipped-0.0.7/clipped/utils/dates.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.6/clipped/utils/dicts.py` & `clipped-0.0.7/clipped/utils/dicts.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.6/clipped/utils/enums.py` & `clipped-0.0.7/clipped/utils/enums.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.6/clipped/utils/env.py` & `clipped-0.0.7/clipped/utils/env.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.6/clipped/utils/git.py` & `clipped-0.0.7/clipped/utils/git.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.6/clipped/utils/hashing.py` & `clipped-0.0.7/clipped/utils/hashing.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.6/clipped/utils/http.py` & `clipped-0.0.7/clipped/utils/http.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.6/clipped/utils/humanize.py` & `clipped-0.0.7/clipped/utils/humanize.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.6/clipped/utils/imports.py` & `clipped-0.0.7/clipped/utils/imports.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.6/clipped/utils/indentation.py` & `clipped-0.0.7/clipped/utils/indentation.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.6/clipped/utils/lists.py` & `clipped-0.0.7/clipped/utils/lists.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     np = None
 
 
 def to_list(
     value: Any,
     check_none: bool = False,
     check_dict: bool = False,
+    check_str: bool = False,
     to_unique: bool = False,
 ) -> List:
     def _to_unique(v):
         try:
             return list(dict.fromkeys(v))
         except Exception as e:
             logging.debug("Could not return unique value for list. Error %s", e)
@@ -27,8 +28,17 @@
     if isinstance(value, (list, tuple, set)):
         return _to_unique(value) if to_unique else list(value)
     if np and isinstance(value, np.ndarray):
         value = value.tolist()
         return _to_unique(value) if to_unique else value
     if check_dict and isinstance(value, Mapping):
         return list(value.items())
+
+    if check_str and np and isinstance(value, str):
+        parts = value.split(",")
+        results = []
+        for part in parts:
+            part = part.strip()
+            if part:
+                results.append(part)
+        return results
     return [value]
```

### Comparing `clipped-0.0.6/clipped/utils/np.py` & `clipped-0.0.7/clipped/utils/np.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.6/clipped/utils/paths.py` & `clipped-0.0.7/clipped/utils/paths.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.6/clipped/utils/query_params.py` & `clipped-0.0.7/clipped/utils/query_params.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.6/clipped/utils/requests.py` & `clipped-0.0.7/clipped/utils/requests.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.6/clipped/utils/responses.py` & `clipped-0.0.7/clipped/utils/responses.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.6/clipped/utils/sanitizers.py` & `clipped-0.0.7/clipped/utils/sanitizers.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.6/clipped/utils/serialization.py` & `clipped-0.0.7/clipped/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.6/clipped/utils/strings.py` & `clipped-0.0.7/clipped/utils/strings.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import datetime
 import re
 import unicodedata
 
+from collections.abc import Mapping
 from decimal import Decimal
 from typing import Any, Callable
 
+from clipped.utils.json import orjson_dumps
+
 
 def strip_spaces(value: str, sep=None, join=True):
     """Cleans trailing whitespaces and replaces also multiple whitespaces with a single space."""
     value = value.strip()
     value = [v.strip() for v in value.split(sep)]
     join_sep = sep or " "
     return join_sep.join(value) if join else value
@@ -79,7 +82,17 @@
     return next(parts) + "".join(i.title() for i in parts)
 
 
 def to_snake_case(camel_str: str):
     regex1 = re.compile(r"([A-Z]+)([A-Z][a-z])")
     regex2 = re.compile(r"([a-z\d])([A-Z])")
     return regex2.sub(r"\1_\2", regex1.sub(r"\1_\2", camel_str)).lower()
+
+
+def to_string(v: Any):
+    base_types = (int, float, Mapping, list, tuple, set)
+    if isinstance(v, base_types):
+        return orjson_dumps(v)
+    # Important to keep null to evaluate empty values
+    if v is None:
+        return v
+    return str(v)
```

### Comparing `clipped-0.0.6/clipped/utils/tz.py` & `clipped-0.0.7/clipped/utils/tz.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.6/clipped/utils/units.py` & `clipped-0.0.7/clipped/utils/units.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.6/clipped/utils/validation.py` & `clipped-0.0.7/clipped/utils/validation.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.6/clipped/utils/versions.py` & `clipped-0.0.7/clipped/utils/versions.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.6/clipped/utils/workers.py` & `clipped-0.0.7/clipped/utils/workers.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.6/clipped/utils/yaml.py` & `clipped-0.0.7/clipped/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.6/clipped.egg-info/PKG-INFO` & `clipped-0.0.7/clipped.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipped
-Version: 0.0.6
+Version: 0.0.7
 Summary: Common shortcuts and utils.
 Home-page: https://github.com/mmourafiq/clipped
 Author: Mourad Mourafiq
 Author-email: mourad.mourafiq@gmail.com
 Maintainer: Mourad Mourafiq
 Maintainer-email: mourad.mourafiq@gmail.com
 License: Apache 2.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: clipped Version: 0.0.6 Summary: Common shortcuts
+Metadata-Version: 2.1 Name: clipped Version: 0.0.7 Summary: Common shortcuts
 and utils. Home-page: https://github.com/mmourafiq/clipped Author: Mourad
 Mourafiq Author-email: mourad.mourafiq@gmail.com Maintainer: Mourad Mourafiq
 Maintainer-email: mourad.mourafiq@gmail.com License: Apache 2.0 Keywords:
 cli,configuration,utils,setup Platform: any Classifier: Intended Audience ::
 Information Technology Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Science/Research Classifier: Operating System :: OS Independent Classifier:
```

### Comparing `clipped-0.0.6/setup.cfg` & `clipped-0.0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `clipped-0.0.6/setup.py` & `clipped-0.0.7/setup.py`

 * *Files identical despite different names*

