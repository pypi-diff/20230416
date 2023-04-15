# Comparing `tmp/clipped-0.0.7.tar.gz` & `tmp/clipped-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clipped-0.0.7.tar", last modified: Sat Apr 15 22:49:42 2023, max compression
+gzip compressed data, was "clipped-0.0.8.tar", last modified: Sat Apr 15 22:57:40 2023, max compression
```

## Comparing `clipped-0.0.7.tar` & `clipped-0.0.8.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-15 22:49:42.692404 clipped-0.0.7/
--rw-r--r--   0 mourad     (501) staff       (20)      174 2023-04-15 22:49:06.000000 clipped-0.0.7/MANIFEST.in
--rw-r--r--   0 mourad     (501) staff       (20)     2012 2023-04-15 22:49:42.692516 clipped-0.0.7/PKG-INFO
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-15 22:49:42.682006 clipped-0.0.7/clipped/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/__init__.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-15 22:49:42.683992 clipped-0.0.7/clipped/config/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/config/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)       91 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/config/constants.py
--rw-r--r--   0 mourad     (501) staff       (20)       40 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/config/exceptions.py
--rw-r--r--   0 mourad     (501) staff       (20)     4022 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/config/manager.py
--rw-r--r--   0 mourad     (501) staff       (20)     6135 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/config/parser.py
--rw-r--r--   0 mourad     (501) staff       (20)      527 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/config/patch_strategy.py
--rw-r--r--   0 mourad     (501) staff       (20)    14929 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/config/schema.py
--rw-r--r--   0 mourad     (501) staff       (20)     8856 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/config/spec.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-15 22:49:42.684789 clipped-0.0.7/clipped/decorators/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/decorators/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)      646 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/decorators/cached_property.py
--rw-r--r--   0 mourad     (501) staff       (20)     4355 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/decorators/deprecation.py
--rw-r--r--   0 mourad     (501) staff       (20)     1923 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/decorators/memoization.py
--rw-r--r--   0 mourad     (501) staff       (20)     2686 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/decorators/signals.py
--rw-r--r--   0 mourad     (501) staff       (20)     6224 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/formatting.py
--rw-r--r--   0 mourad     (501) staff       (20)      824 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/manager_interface.py
--rw-r--r--   0 mourad     (501) staff       (20)      203 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/pkg.py
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/py.typed
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-15 22:49:42.686509 clipped-0.0.7/clipped/types/
--rw-r--r--   0 mourad     (501) staff       (20)     3868 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/types/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     1298 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/types/docker_image.py
--rw-r--r--   0 mourad     (501) staff       (20)     1889 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/types/email.py
--rw-r--r--   0 mourad     (501) staff       (20)     1081 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/types/gcs.py
--rw-r--r--   0 mourad     (501) staff       (20)      693 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/types/lists.py
--rw-r--r--   0 mourad     (501) staff       (20)      158 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/types/numbers.py
--rw-r--r--   0 mourad     (501) staff       (20)     1142 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/types/ref_or_obj.py
--rw-r--r--   0 mourad     (501) staff       (20)     1065 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/types/s3.py
--rw-r--r--   0 mourad     (501) staff       (20)     1265 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/types/uri.py
--rw-r--r--   0 mourad     (501) staff       (20)      683 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/types/uuids.py
--rw-r--r--   0 mourad     (501) staff       (20)     3229 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/types/wasb.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-15 22:49:42.692242 clipped-0.0.7/clipped/utils/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     1004 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/bools.py
--rw-r--r--   0 mourad     (501) staff       (20)      143 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/click.py
--rw-r--r--   0 mourad     (501) staff       (20)      665 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/cmd.py
--rw-r--r--   0 mourad     (501) staff       (20)      570 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/coroutine.py
--rw-r--r--   0 mourad     (501) staff       (20)      755 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/csv.py
--rw-r--r--   0 mourad     (501) staff       (20)     7568 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/dates.py
--rw-r--r--   0 mourad     (501) staff       (20)     3354 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/dicts.py
--rw-r--r--   0 mourad     (501) staff       (20)      496 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/encoding.py
--rw-r--r--   0 mourad     (501) staff       (20)     1093 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/enums.py
--rw-r--r--   0 mourad     (501) staff       (20)     2001 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/env.py
--rw-r--r--   0 mourad     (501) staff       (20)     4737 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/git.py
--rw-r--r--   0 mourad     (501) staff       (20)     1827 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/hashing.py
--rw-r--r--   0 mourad     (501) staff       (20)     1175 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/http.py
--rw-r--r--   0 mourad     (501) staff       (20)     3363 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/humanize.py
--rw-r--r--   0 mourad     (501) staff       (20)     1327 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/imports.py
--rw-r--r--   0 mourad     (501) staff       (20)     1695 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/indentation.py
--rw-r--r--   0 mourad     (501) staff       (20)      287 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/json.py
--rw-r--r--   0 mourad     (501) staff       (20)     1170 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/lists.py
--rw-r--r--   0 mourad     (501) staff       (20)      113 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/logging.py
--rw-r--r--   0 mourad     (501) staff       (20)     1280 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/np.py
--rw-r--r--   0 mourad     (501) staff       (20)     8484 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/paths.py
--rw-r--r--   0 mourad     (501) staff       (20)      674 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/query_params.py
--rw-r--r--   0 mourad     (501) staff       (20)     1134 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/requests.py
--rw-r--r--   0 mourad     (501) staff       (20)     1041 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/responses.py
--rw-r--r--   0 mourad     (501) staff       (20)      559 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/sanitizers.py
--rw-r--r--   0 mourad     (501) staff       (20)      676 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/serialization.py
--rw-r--r--   0 mourad     (501) staff       (20)     2674 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/strings.py
--rw-r--r--   0 mourad     (501) staff       (20)     1115 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/tz.py
--rw-r--r--   0 mourad     (501) staff       (20)     4040 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/units.py
--rw-r--r--   0 mourad     (501) staff       (20)      269 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/urls.py
--rw-r--r--   0 mourad     (501) staff       (20)      614 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/validation.py
--rw-r--r--   0 mourad     (501) staff       (20)     1128 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/versions.py
--rw-r--r--   0 mourad     (501) staff       (20)     1068 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/workers.py
--rw-r--r--   0 mourad     (501) staff       (20)      546 2023-04-15 22:49:06.000000 clipped-0.0.7/clipped/utils/yaml.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-15 22:49:42.682648 clipped-0.0.7/clipped.egg-info/
--rw-r--r--   0 mourad     (501) staff       (20)     2012 2023-04-15 22:49:42.000000 clipped-0.0.7/clipped.egg-info/PKG-INFO
--rw-r--r--   0 mourad     (501) staff       (20)     1796 2023-04-15 22:49:42.000000 clipped-0.0.7/clipped.egg-info/SOURCES.txt
--rw-r--r--   0 mourad     (501) staff       (20)        1 2023-04-15 22:49:42.000000 clipped-0.0.7/clipped.egg-info/dependency_links.txt
--rw-r--r--   0 mourad     (501) staff       (20)        8 2023-04-15 22:49:42.000000 clipped-0.0.7/clipped.egg-info/top_level.txt
--rw-r--r--   0 mourad     (501) staff       (20)     1033 2023-04-15 22:49:42.693029 clipped-0.0.7/setup.cfg
--rw-r--r--   0 mourad     (501) staff       (20)     2345 2023-04-15 22:49:06.000000 clipped-0.0.7/setup.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-15 22:57:40.821213 clipped-0.0.8/
+-rw-r--r--   0 mourad     (501) staff       (20)      174 2023-04-15 22:56:44.000000 clipped-0.0.8/MANIFEST.in
+-rw-r--r--   0 mourad     (501) staff       (20)     2012 2023-04-15 22:57:40.821303 clipped-0.0.8/PKG-INFO
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-15 22:57:40.810866 clipped-0.0.8/clipped/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/__init__.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-15 22:57:40.812946 clipped-0.0.8/clipped/config/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/config/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)       91 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/config/constants.py
+-rw-r--r--   0 mourad     (501) staff       (20)       40 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/config/exceptions.py
+-rw-r--r--   0 mourad     (501) staff       (20)     4022 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/config/manager.py
+-rw-r--r--   0 mourad     (501) staff       (20)     6199 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/config/parser.py
+-rw-r--r--   0 mourad     (501) staff       (20)      527 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/config/patch_strategy.py
+-rw-r--r--   0 mourad     (501) staff       (20)    14929 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/config/schema.py
+-rw-r--r--   0 mourad     (501) staff       (20)     8856 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/config/spec.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-15 22:57:40.813722 clipped-0.0.8/clipped/decorators/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/decorators/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)      646 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/decorators/cached_property.py
+-rw-r--r--   0 mourad     (501) staff       (20)     4355 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/decorators/deprecation.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1923 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/decorators/memoization.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2686 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/decorators/signals.py
+-rw-r--r--   0 mourad     (501) staff       (20)     6224 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/formatting.py
+-rw-r--r--   0 mourad     (501) staff       (20)      824 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/manager_interface.py
+-rw-r--r--   0 mourad     (501) staff       (20)      203 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/pkg.py
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/py.typed
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-15 22:57:40.815480 clipped-0.0.8/clipped/types/
+-rw-r--r--   0 mourad     (501) staff       (20)     3748 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/types/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1298 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/types/docker_image.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1889 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/types/email.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1033 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/types/gcs.py
+-rw-r--r--   0 mourad     (501) staff       (20)      693 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/types/lists.py
+-rw-r--r--   0 mourad     (501) staff       (20)      158 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/types/numbers.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1142 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/types/ref_or_obj.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1019 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/types/s3.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1265 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/types/uri.py
+-rw-r--r--   0 mourad     (501) staff       (20)      683 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/types/uuids.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3179 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/types/wasb.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-15 22:57:40.821075 clipped-0.0.8/clipped/utils/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1004 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/bools.py
+-rw-r--r--   0 mourad     (501) staff       (20)      143 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/click.py
+-rw-r--r--   0 mourad     (501) staff       (20)      665 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/cmd.py
+-rw-r--r--   0 mourad     (501) staff       (20)      570 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/coroutine.py
+-rw-r--r--   0 mourad     (501) staff       (20)      755 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/csv.py
+-rw-r--r--   0 mourad     (501) staff       (20)     7568 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/dates.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3354 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/dicts.py
+-rw-r--r--   0 mourad     (501) staff       (20)      496 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/encoding.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1093 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/enums.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2001 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/env.py
+-rw-r--r--   0 mourad     (501) staff       (20)     4737 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/git.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1827 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/hashing.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1175 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/http.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3363 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/humanize.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1327 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/imports.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1695 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/indentation.py
+-rw-r--r--   0 mourad     (501) staff       (20)      287 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/json.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1170 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/lists.py
+-rw-r--r--   0 mourad     (501) staff       (20)      113 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/logging.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1280 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/np.py
+-rw-r--r--   0 mourad     (501) staff       (20)     8484 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/paths.py
+-rw-r--r--   0 mourad     (501) staff       (20)      674 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/query_params.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1134 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/requests.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1041 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/responses.py
+-rw-r--r--   0 mourad     (501) staff       (20)      559 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/sanitizers.py
+-rw-r--r--   0 mourad     (501) staff       (20)      676 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/serialization.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2674 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/strings.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1115 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/tz.py
+-rw-r--r--   0 mourad     (501) staff       (20)     4040 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/units.py
+-rw-r--r--   0 mourad     (501) staff       (20)      269 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/urls.py
+-rw-r--r--   0 mourad     (501) staff       (20)      614 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/validation.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1128 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/versions.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1068 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/workers.py
+-rw-r--r--   0 mourad     (501) staff       (20)      546 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/yaml.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-15 22:57:40.811588 clipped-0.0.8/clipped.egg-info/
+-rw-r--r--   0 mourad     (501) staff       (20)     2012 2023-04-15 22:57:40.000000 clipped-0.0.8/clipped.egg-info/PKG-INFO
+-rw-r--r--   0 mourad     (501) staff       (20)     1796 2023-04-15 22:57:40.000000 clipped-0.0.8/clipped.egg-info/SOURCES.txt
+-rw-r--r--   0 mourad     (501) staff       (20)        1 2023-04-15 22:57:40.000000 clipped-0.0.8/clipped.egg-info/dependency_links.txt
+-rw-r--r--   0 mourad     (501) staff       (20)        8 2023-04-15 22:57:40.000000 clipped-0.0.8/clipped.egg-info/top_level.txt
+-rw-r--r--   0 mourad     (501) staff       (20)     1033 2023-04-15 22:57:40.821791 clipped-0.0.8/setup.cfg
+-rw-r--r--   0 mourad     (501) staff       (20)     2345 2023-04-15 22:56:44.000000 clipped-0.0.8/setup.py
```

### Comparing `clipped-0.0.7/PKG-INFO` & `clipped-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipped
-Version: 0.0.7
+Version: 0.0.8
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
-Metadata-Version: 2.1 Name: clipped Version: 0.0.7 Summary: Common shortcuts
+Metadata-Version: 2.1 Name: clipped Version: 0.0.8 Summary: Common shortcuts
 and utils. Home-page: https://github.com/mmourafiq/clipped Author: Mourad
 Mourafiq Author-email: mourad.mourafiq@gmail.com Maintainer: Mourad Mourafiq
 Maintainer-email: mourad.mourafiq@gmail.com License: Apache 2.0 Keywords:
 cli,configuration,utils,setup Platform: any Classifier: Intended Audience ::
 Information Technology Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Science/Research Classifier: Operating System :: OS Independent Classifier:
```

### Comparing `clipped-0.0.7/clipped/config/manager.py` & `clipped-0.0.8/clipped/config/manager.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.7/clipped/config/parser.py` & `clipped-0.0.8/clipped/config/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import logging
 
-from typing import Any, Callable, List, Optional, Protocol, Type, TypeVar
+from typing import Any, Callable, List, Optional, Type, TypeVar, TYPE_CHECKING
 
 import orjson
 
 from pydantic import PydanticTypeError, PydanticValueError, StrBytes, ValidationError
 from pydantic.parse import load_str_bytes
 from pydantic.tools import NameFactory, _get_parsing_type
 
 from clipped.config.constants import NO_VALUE_FOUND
 from clipped.config.exceptions import SchemaError
 from clipped.decorators.memoization import memoize, memoize_method
 
+if TYPE_CHECKING:
+    from pydantic.parse import Protocol
+
 _logger = logging.getLogger("clipped.parser")
 
 T = TypeVar("T")
 
 
 class Parser:
     _SCHEMA_EXCEPTION = SchemaError
```

### Comparing `clipped-0.0.7/clipped/config/patch_strategy.py` & `clipped-0.0.8/clipped/config/patch_strategy.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.7/clipped/config/schema.py` & `clipped-0.0.8/clipped/config/schema.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.7/clipped/config/spec.py` & `clipped-0.0.8/clipped/config/spec.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.7/clipped/decorators/cached_property.py` & `clipped-0.0.8/clipped/decorators/cached_property.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.7/clipped/decorators/deprecation.py` & `clipped-0.0.8/clipped/decorators/deprecation.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.7/clipped/decorators/memoization.py` & `clipped-0.0.8/clipped/decorators/memoization.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.7/clipped/decorators/signals.py` & `clipped-0.0.8/clipped/decorators/signals.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.7/clipped/formatting.py` & `clipped-0.0.8/clipped/formatting.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.7/clipped/manager_interface.py` & `clipped-0.0.8/clipped/manager_interface.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.7/clipped/types/__init__.py` & `clipped-0.0.8/clipped/types/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,21 +52,15 @@
 
 URI = "uri"
 AUTH = "auth"
 LIST = "list"
 GCS = "gcs"
 S3 = "s3"
 WASB = "wasb"
-DOCKERFILE = "dockerfile"
-FILE = "file"
-TENSORBOARD = "tensorboard"
-GIT = "git"
 IMAGE = "image"
-EVENT = "event"
-ARTIFACTS = "artifacts"
 PATH = "path"
 METRIC = "metric"
 METADATA = "metadata"
 DATE = "date"
 DATETIME = "datetime"
 UUID = "uuid"
 EMAIL = "email"
```

### Comparing `clipped-0.0.7/clipped/types/docker_image.py` & `clipped-0.0.8/clipped/types/docker_image.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.7/clipped/types/email.py` & `clipped-0.0.8/clipped/types/email.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.7/clipped/types/gcs.py` & `clipped-0.0.8/clipped/types/gcs.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,11 +30,7 @@
 
     def to_param(self):
         return str(self)
 
     @property
     def structured(self):
         return dict(bucket=self.host, blob=self.path.strip("/"))
-
-
-# Backwards compatibility
-V1GcsType = GcsPath
```

### Comparing `clipped-0.0.7/clipped/types/lists.py` & `clipped-0.0.8/clipped/types/lists.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.7/clipped/types/ref_or_obj.py` & `clipped-0.0.8/clipped/types/ref_or_obj.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.7/clipped/types/s3.py` & `clipped-0.0.8/clipped/types/s3.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,11 +30,7 @@
 
     def to_param(self):
         return str(self)
 
     @property
     def structured(self):
         return dict(bucket=self.host, key=self.path.strip("/"))
-
-
-# Backwards compatibility
-V1S3Type = S3Path
```

### Comparing `clipped-0.0.7/clipped/types/uri.py` & `clipped-0.0.8/clipped/types/uri.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.7/clipped/types/uuids.py` & `clipped-0.0.8/clipped/types/uuids.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.7/clipped/types/wasb.py` & `clipped-0.0.8/clipped/types/wasb.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,11 +86,7 @@
         return self._validate(self.to_param())
 
     def get_container_path(self):
         structured = self.structured
         if structured.get("path"):
             return f"{structured['container']}/{structured['path']}"
         return structured["container"]
-
-
-# Backwards compatibility
-V1WasbType = WasbPath
```

### Comparing `clipped-0.0.7/clipped/utils/bools.py` & `clipped-0.0.8/clipped/utils/bools.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.7/clipped/utils/cmd.py` & `clipped-0.0.8/clipped/utils/cmd.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.7/clipped/utils/coroutine.py` & `clipped-0.0.8/clipped/utils/coroutine.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.7/clipped/utils/csv.py` & `clipped-0.0.8/clipped/utils/csv.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.7/clipped/utils/dates.py` & `clipped-0.0.8/clipped/utils/dates.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.7/clipped/utils/dicts.py` & `clipped-0.0.8/clipped/utils/dicts.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.7/clipped/utils/enums.py` & `clipped-0.0.8/clipped/utils/enums.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.7/clipped/utils/env.py` & `clipped-0.0.8/clipped/utils/env.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.7/clipped/utils/git.py` & `clipped-0.0.8/clipped/utils/git.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.7/clipped/utils/hashing.py` & `clipped-0.0.8/clipped/utils/hashing.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.7/clipped/utils/http.py` & `clipped-0.0.8/clipped/utils/http.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.7/clipped/utils/humanize.py` & `clipped-0.0.8/clipped/utils/humanize.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.7/clipped/utils/imports.py` & `clipped-0.0.8/clipped/utils/imports.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.7/clipped/utils/indentation.py` & `clipped-0.0.8/clipped/utils/indentation.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.7/clipped/utils/lists.py` & `clipped-0.0.8/clipped/utils/lists.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.7/clipped/utils/np.py` & `clipped-0.0.8/clipped/utils/np.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.7/clipped/utils/paths.py` & `clipped-0.0.8/clipped/utils/paths.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.7/clipped/utils/query_params.py` & `clipped-0.0.8/clipped/utils/query_params.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.7/clipped/utils/requests.py` & `clipped-0.0.8/clipped/utils/requests.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.7/clipped/utils/responses.py` & `clipped-0.0.8/clipped/utils/responses.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.7/clipped/utils/sanitizers.py` & `clipped-0.0.8/clipped/utils/sanitizers.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.7/clipped/utils/serialization.py` & `clipped-0.0.8/clipped/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.7/clipped/utils/strings.py` & `clipped-0.0.8/clipped/utils/strings.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.7/clipped/utils/tz.py` & `clipped-0.0.8/clipped/utils/tz.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.7/clipped/utils/units.py` & `clipped-0.0.8/clipped/utils/units.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.7/clipped/utils/validation.py` & `clipped-0.0.8/clipped/utils/validation.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.7/clipped/utils/versions.py` & `clipped-0.0.8/clipped/utils/versions.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.7/clipped/utils/workers.py` & `clipped-0.0.8/clipped/utils/workers.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.7/clipped/utils/yaml.py` & `clipped-0.0.8/clipped/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.7/clipped.egg-info/PKG-INFO` & `clipped-0.0.8/clipped.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipped
-Version: 0.0.7
+Version: 0.0.8
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
-Metadata-Version: 2.1 Name: clipped Version: 0.0.7 Summary: Common shortcuts
+Metadata-Version: 2.1 Name: clipped Version: 0.0.8 Summary: Common shortcuts
 and utils. Home-page: https://github.com/mmourafiq/clipped Author: Mourad
 Mourafiq Author-email: mourad.mourafiq@gmail.com Maintainer: Mourad Mourafiq
 Maintainer-email: mourad.mourafiq@gmail.com License: Apache 2.0 Keywords:
 cli,configuration,utils,setup Platform: any Classifier: Intended Audience ::
 Information Technology Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Science/Research Classifier: Operating System :: OS Independent Classifier:
```

### Comparing `clipped-0.0.7/clipped.egg-info/SOURCES.txt` & `clipped-0.0.8/clipped.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clipped-0.0.7/setup.cfg` & `clipped-0.0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `clipped-0.0.7/setup.py` & `clipped-0.0.8/setup.py`

 * *Files identical despite different names*

