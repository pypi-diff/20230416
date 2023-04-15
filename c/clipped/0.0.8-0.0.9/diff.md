# Comparing `tmp/clipped-0.0.8.tar.gz` & `tmp/clipped-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clipped-0.0.8.tar", last modified: Sat Apr 15 22:57:40 2023, max compression
+gzip compressed data, was "clipped-0.0.9.tar", last modified: Sat Apr 15 23:04:54 2023, max compression
```

## Comparing `clipped-0.0.8.tar` & `clipped-0.0.9.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-15 22:57:40.821213 clipped-0.0.8/
--rw-r--r--   0 mourad     (501) staff       (20)      174 2023-04-15 22:56:44.000000 clipped-0.0.8/MANIFEST.in
--rw-r--r--   0 mourad     (501) staff       (20)     2012 2023-04-15 22:57:40.821303 clipped-0.0.8/PKG-INFO
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-15 22:57:40.810866 clipped-0.0.8/clipped/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/__init__.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-15 22:57:40.812946 clipped-0.0.8/clipped/config/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/config/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)       91 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/config/constants.py
--rw-r--r--   0 mourad     (501) staff       (20)       40 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/config/exceptions.py
--rw-r--r--   0 mourad     (501) staff       (20)     4022 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/config/manager.py
--rw-r--r--   0 mourad     (501) staff       (20)     6199 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/config/parser.py
--rw-r--r--   0 mourad     (501) staff       (20)      527 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/config/patch_strategy.py
--rw-r--r--   0 mourad     (501) staff       (20)    14929 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/config/schema.py
--rw-r--r--   0 mourad     (501) staff       (20)     8856 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/config/spec.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-15 22:57:40.813722 clipped-0.0.8/clipped/decorators/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/decorators/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)      646 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/decorators/cached_property.py
--rw-r--r--   0 mourad     (501) staff       (20)     4355 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/decorators/deprecation.py
--rw-r--r--   0 mourad     (501) staff       (20)     1923 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/decorators/memoization.py
--rw-r--r--   0 mourad     (501) staff       (20)     2686 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/decorators/signals.py
--rw-r--r--   0 mourad     (501) staff       (20)     6224 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/formatting.py
--rw-r--r--   0 mourad     (501) staff       (20)      824 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/manager_interface.py
--rw-r--r--   0 mourad     (501) staff       (20)      203 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/pkg.py
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/py.typed
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-15 22:57:40.815480 clipped-0.0.8/clipped/types/
--rw-r--r--   0 mourad     (501) staff       (20)     3748 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/types/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     1298 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/types/docker_image.py
--rw-r--r--   0 mourad     (501) staff       (20)     1889 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/types/email.py
--rw-r--r--   0 mourad     (501) staff       (20)     1033 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/types/gcs.py
--rw-r--r--   0 mourad     (501) staff       (20)      693 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/types/lists.py
--rw-r--r--   0 mourad     (501) staff       (20)      158 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/types/numbers.py
--rw-r--r--   0 mourad     (501) staff       (20)     1142 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/types/ref_or_obj.py
--rw-r--r--   0 mourad     (501) staff       (20)     1019 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/types/s3.py
--rw-r--r--   0 mourad     (501) staff       (20)     1265 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/types/uri.py
--rw-r--r--   0 mourad     (501) staff       (20)      683 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/types/uuids.py
--rw-r--r--   0 mourad     (501) staff       (20)     3179 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/types/wasb.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-15 22:57:40.821075 clipped-0.0.8/clipped/utils/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     1004 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/bools.py
--rw-r--r--   0 mourad     (501) staff       (20)      143 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/click.py
--rw-r--r--   0 mourad     (501) staff       (20)      665 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/cmd.py
--rw-r--r--   0 mourad     (501) staff       (20)      570 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/coroutine.py
--rw-r--r--   0 mourad     (501) staff       (20)      755 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/csv.py
--rw-r--r--   0 mourad     (501) staff       (20)     7568 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/dates.py
--rw-r--r--   0 mourad     (501) staff       (20)     3354 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/dicts.py
--rw-r--r--   0 mourad     (501) staff       (20)      496 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/encoding.py
--rw-r--r--   0 mourad     (501) staff       (20)     1093 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/enums.py
--rw-r--r--   0 mourad     (501) staff       (20)     2001 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/env.py
--rw-r--r--   0 mourad     (501) staff       (20)     4737 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/git.py
--rw-r--r--   0 mourad     (501) staff       (20)     1827 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/hashing.py
--rw-r--r--   0 mourad     (501) staff       (20)     1175 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/http.py
--rw-r--r--   0 mourad     (501) staff       (20)     3363 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/humanize.py
--rw-r--r--   0 mourad     (501) staff       (20)     1327 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/imports.py
--rw-r--r--   0 mourad     (501) staff       (20)     1695 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/indentation.py
--rw-r--r--   0 mourad     (501) staff       (20)      287 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/json.py
--rw-r--r--   0 mourad     (501) staff       (20)     1170 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/lists.py
--rw-r--r--   0 mourad     (501) staff       (20)      113 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/logging.py
--rw-r--r--   0 mourad     (501) staff       (20)     1280 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/np.py
--rw-r--r--   0 mourad     (501) staff       (20)     8484 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/paths.py
--rw-r--r--   0 mourad     (501) staff       (20)      674 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/query_params.py
--rw-r--r--   0 mourad     (501) staff       (20)     1134 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/requests.py
--rw-r--r--   0 mourad     (501) staff       (20)     1041 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/responses.py
--rw-r--r--   0 mourad     (501) staff       (20)      559 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/sanitizers.py
--rw-r--r--   0 mourad     (501) staff       (20)      676 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/serialization.py
--rw-r--r--   0 mourad     (501) staff       (20)     2674 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/strings.py
--rw-r--r--   0 mourad     (501) staff       (20)     1115 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/tz.py
--rw-r--r--   0 mourad     (501) staff       (20)     4040 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/units.py
--rw-r--r--   0 mourad     (501) staff       (20)      269 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/urls.py
--rw-r--r--   0 mourad     (501) staff       (20)      614 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/validation.py
--rw-r--r--   0 mourad     (501) staff       (20)     1128 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/versions.py
--rw-r--r--   0 mourad     (501) staff       (20)     1068 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/workers.py
--rw-r--r--   0 mourad     (501) staff       (20)      546 2023-04-15 22:56:44.000000 clipped-0.0.8/clipped/utils/yaml.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-15 22:57:40.811588 clipped-0.0.8/clipped.egg-info/
--rw-r--r--   0 mourad     (501) staff       (20)     2012 2023-04-15 22:57:40.000000 clipped-0.0.8/clipped.egg-info/PKG-INFO
--rw-r--r--   0 mourad     (501) staff       (20)     1796 2023-04-15 22:57:40.000000 clipped-0.0.8/clipped.egg-info/SOURCES.txt
--rw-r--r--   0 mourad     (501) staff       (20)        1 2023-04-15 22:57:40.000000 clipped-0.0.8/clipped.egg-info/dependency_links.txt
--rw-r--r--   0 mourad     (501) staff       (20)        8 2023-04-15 22:57:40.000000 clipped-0.0.8/clipped.egg-info/top_level.txt
--rw-r--r--   0 mourad     (501) staff       (20)     1033 2023-04-15 22:57:40.821791 clipped-0.0.8/setup.cfg
--rw-r--r--   0 mourad     (501) staff       (20)     2345 2023-04-15 22:56:44.000000 clipped-0.0.8/setup.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-15 23:04:54.406301 clipped-0.0.9/
+-rw-r--r--   0 mourad     (501) staff       (20)      174 2023-04-15 23:00:45.000000 clipped-0.0.9/MANIFEST.in
+-rw-r--r--   0 mourad     (501) staff       (20)     2012 2023-04-15 23:04:54.406403 clipped-0.0.9/PKG-INFO
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-15 23:04:54.396034 clipped-0.0.9/clipped/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/__init__.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-15 23:04:54.398054 clipped-0.0.9/clipped/config/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/config/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)       91 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/config/constants.py
+-rw-r--r--   0 mourad     (501) staff       (20)       40 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/config/exceptions.py
+-rw-r--r--   0 mourad     (501) staff       (20)     4022 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/config/manager.py
+-rw-r--r--   0 mourad     (501) staff       (20)     6136 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/config/parser.py
+-rw-r--r--   0 mourad     (501) staff       (20)      527 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/config/patch_strategy.py
+-rw-r--r--   0 mourad     (501) staff       (20)    14929 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/config/schema.py
+-rw-r--r--   0 mourad     (501) staff       (20)     8856 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/config/spec.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-15 23:04:54.398941 clipped-0.0.9/clipped/decorators/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/decorators/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)      646 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/decorators/cached_property.py
+-rw-r--r--   0 mourad     (501) staff       (20)     4355 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/decorators/deprecation.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1923 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/decorators/memoization.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2686 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/decorators/signals.py
+-rw-r--r--   0 mourad     (501) staff       (20)     6224 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/formatting.py
+-rw-r--r--   0 mourad     (501) staff       (20)      824 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/manager_interface.py
+-rw-r--r--   0 mourad     (501) staff       (20)      203 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/pkg.py
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/py.typed
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-15 23:04:54.400740 clipped-0.0.9/clipped/types/
+-rw-r--r--   0 mourad     (501) staff       (20)     3748 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/types/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1298 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/types/docker_image.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1889 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/types/email.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1033 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/types/gcs.py
+-rw-r--r--   0 mourad     (501) staff       (20)      693 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/types/lists.py
+-rw-r--r--   0 mourad     (501) staff       (20)      158 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/types/numbers.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1142 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/types/ref_or_obj.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1019 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/types/s3.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1265 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/types/uri.py
+-rw-r--r--   0 mourad     (501) staff       (20)      683 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/types/uuids.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3179 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/types/wasb.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-15 23:04:54.406151 clipped-0.0.9/clipped/utils/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/utils/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1004 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/utils/bools.py
+-rw-r--r--   0 mourad     (501) staff       (20)      143 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/utils/click.py
+-rw-r--r--   0 mourad     (501) staff       (20)      665 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/utils/cmd.py
+-rw-r--r--   0 mourad     (501) staff       (20)      570 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/utils/coroutine.py
+-rw-r--r--   0 mourad     (501) staff       (20)      755 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/utils/csv.py
+-rw-r--r--   0 mourad     (501) staff       (20)     7568 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/utils/dates.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3354 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/utils/dicts.py
+-rw-r--r--   0 mourad     (501) staff       (20)      496 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/utils/encoding.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1093 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/utils/enums.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2001 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/utils/env.py
+-rw-r--r--   0 mourad     (501) staff       (20)     4737 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/utils/git.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1827 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/utils/hashing.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1175 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/utils/http.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3363 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/utils/humanize.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1327 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/utils/imports.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1695 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/utils/indentation.py
+-rw-r--r--   0 mourad     (501) staff       (20)      287 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/utils/json.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1170 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/utils/lists.py
+-rw-r--r--   0 mourad     (501) staff       (20)      113 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/utils/logging.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1280 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/utils/np.py
+-rw-r--r--   0 mourad     (501) staff       (20)     8484 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/utils/paths.py
+-rw-r--r--   0 mourad     (501) staff       (20)      674 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/utils/query_params.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1134 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/utils/requests.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1041 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/utils/responses.py
+-rw-r--r--   0 mourad     (501) staff       (20)      559 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/utils/sanitizers.py
+-rw-r--r--   0 mourad     (501) staff       (20)      676 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/utils/serialization.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2674 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/utils/strings.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1115 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/utils/tz.py
+-rw-r--r--   0 mourad     (501) staff       (20)     4040 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/utils/units.py
+-rw-r--r--   0 mourad     (501) staff       (20)      269 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/utils/urls.py
+-rw-r--r--   0 mourad     (501) staff       (20)      614 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/utils/validation.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1128 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/utils/versions.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1068 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/utils/workers.py
+-rw-r--r--   0 mourad     (501) staff       (20)      546 2023-04-15 23:00:45.000000 clipped-0.0.9/clipped/utils/yaml.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-15 23:04:54.396755 clipped-0.0.9/clipped.egg-info/
+-rw-r--r--   0 mourad     (501) staff       (20)     2012 2023-04-15 23:04:54.000000 clipped-0.0.9/clipped.egg-info/PKG-INFO
+-rw-r--r--   0 mourad     (501) staff       (20)     1796 2023-04-15 23:04:54.000000 clipped-0.0.9/clipped.egg-info/SOURCES.txt
+-rw-r--r--   0 mourad     (501) staff       (20)        1 2023-04-15 23:04:54.000000 clipped-0.0.9/clipped.egg-info/dependency_links.txt
+-rw-r--r--   0 mourad     (501) staff       (20)        8 2023-04-15 23:04:54.000000 clipped-0.0.9/clipped.egg-info/top_level.txt
+-rw-r--r--   0 mourad     (501) staff       (20)     1033 2023-04-15 23:04:54.406890 clipped-0.0.9/setup.cfg
+-rw-r--r--   0 mourad     (501) staff       (20)     2345 2023-04-15 23:00:45.000000 clipped-0.0.9/setup.py
```

### Comparing `clipped-0.0.8/PKG-INFO` & `clipped-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipped
-Version: 0.0.8
+Version: 0.0.9
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
-Metadata-Version: 2.1 Name: clipped Version: 0.0.8 Summary: Common shortcuts
+Metadata-Version: 2.1 Name: clipped Version: 0.0.9 Summary: Common shortcuts
 and utils. Home-page: https://github.com/mmourafiq/clipped Author: Mourad
 Mourafiq Author-email: mourad.mourafiq@gmail.com Maintainer: Mourad Mourafiq
 Maintainer-email: mourad.mourafiq@gmail.com License: Apache 2.0 Keywords:
 cli,configuration,utils,setup Platform: any Classifier: Intended Audience ::
 Information Technology Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Science/Research Classifier: Operating System :: OS Independent Classifier:
```

### Comparing `clipped-0.0.8/clipped/config/manager.py` & `clipped-0.0.9/clipped/config/manager.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.8/clipped/config/parser.py` & `clipped-0.0.9/clipped/config/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 import logging
 
-from typing import Any, Callable, List, Optional, Type, TypeVar, TYPE_CHECKING
+from typing import Any, Callable, List, Optional, Type, TypeVar
 
 import orjson
 
 from pydantic import PydanticTypeError, PydanticValueError, StrBytes, ValidationError
-from pydantic.parse import load_str_bytes
+from pydantic.parse import load_str_bytes, Protocol
 from pydantic.tools import NameFactory, _get_parsing_type
 
 from clipped.config.constants import NO_VALUE_FOUND
 from clipped.config.exceptions import SchemaError
 from clipped.decorators.memoization import memoize, memoize_method
 
-if TYPE_CHECKING:
-    from pydantic.parse import Protocol
 
 _logger = logging.getLogger("clipped.parser")
 
 T = TypeVar("T")
 
 
 class Parser:
```

### Comparing `clipped-0.0.8/clipped/config/patch_strategy.py` & `clipped-0.0.9/clipped/config/patch_strategy.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.8/clipped/config/schema.py` & `clipped-0.0.9/clipped/config/schema.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.8/clipped/config/spec.py` & `clipped-0.0.9/clipped/config/spec.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.8/clipped/decorators/cached_property.py` & `clipped-0.0.9/clipped/decorators/cached_property.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.8/clipped/decorators/deprecation.py` & `clipped-0.0.9/clipped/decorators/deprecation.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.8/clipped/decorators/memoization.py` & `clipped-0.0.9/clipped/decorators/memoization.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.8/clipped/decorators/signals.py` & `clipped-0.0.9/clipped/decorators/signals.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.8/clipped/formatting.py` & `clipped-0.0.9/clipped/formatting.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.8/clipped/manager_interface.py` & `clipped-0.0.9/clipped/manager_interface.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.8/clipped/types/__init__.py` & `clipped-0.0.9/clipped/types/__init__.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.8/clipped/types/docker_image.py` & `clipped-0.0.9/clipped/types/docker_image.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.8/clipped/types/email.py` & `clipped-0.0.9/clipped/types/email.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.8/clipped/types/gcs.py` & `clipped-0.0.9/clipped/types/gcs.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.8/clipped/types/lists.py` & `clipped-0.0.9/clipped/types/lists.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.8/clipped/types/ref_or_obj.py` & `clipped-0.0.9/clipped/types/ref_or_obj.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.8/clipped/types/s3.py` & `clipped-0.0.9/clipped/types/s3.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.8/clipped/types/uri.py` & `clipped-0.0.9/clipped/types/uri.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.8/clipped/types/uuids.py` & `clipped-0.0.9/clipped/types/uuids.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.8/clipped/types/wasb.py` & `clipped-0.0.9/clipped/types/wasb.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.8/clipped/utils/bools.py` & `clipped-0.0.9/clipped/utils/bools.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.8/clipped/utils/cmd.py` & `clipped-0.0.9/clipped/utils/cmd.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.8/clipped/utils/coroutine.py` & `clipped-0.0.9/clipped/utils/coroutine.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.8/clipped/utils/csv.py` & `clipped-0.0.9/clipped/utils/csv.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.8/clipped/utils/dates.py` & `clipped-0.0.9/clipped/utils/dates.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.8/clipped/utils/dicts.py` & `clipped-0.0.9/clipped/utils/dicts.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.8/clipped/utils/enums.py` & `clipped-0.0.9/clipped/utils/enums.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.8/clipped/utils/env.py` & `clipped-0.0.9/clipped/utils/env.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.8/clipped/utils/git.py` & `clipped-0.0.9/clipped/utils/git.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.8/clipped/utils/hashing.py` & `clipped-0.0.9/clipped/utils/hashing.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.8/clipped/utils/http.py` & `clipped-0.0.9/clipped/utils/http.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.8/clipped/utils/humanize.py` & `clipped-0.0.9/clipped/utils/humanize.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.8/clipped/utils/imports.py` & `clipped-0.0.9/clipped/utils/imports.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.8/clipped/utils/indentation.py` & `clipped-0.0.9/clipped/utils/indentation.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.8/clipped/utils/lists.py` & `clipped-0.0.9/clipped/utils/lists.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.8/clipped/utils/np.py` & `clipped-0.0.9/clipped/utils/np.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.8/clipped/utils/paths.py` & `clipped-0.0.9/clipped/utils/paths.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.8/clipped/utils/query_params.py` & `clipped-0.0.9/clipped/utils/query_params.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.8/clipped/utils/requests.py` & `clipped-0.0.9/clipped/utils/requests.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.8/clipped/utils/responses.py` & `clipped-0.0.9/clipped/utils/responses.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.8/clipped/utils/sanitizers.py` & `clipped-0.0.9/clipped/utils/sanitizers.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.8/clipped/utils/serialization.py` & `clipped-0.0.9/clipped/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.8/clipped/utils/strings.py` & `clipped-0.0.9/clipped/utils/strings.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.8/clipped/utils/tz.py` & `clipped-0.0.9/clipped/utils/tz.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.8/clipped/utils/units.py` & `clipped-0.0.9/clipped/utils/units.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.8/clipped/utils/validation.py` & `clipped-0.0.9/clipped/utils/validation.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.8/clipped/utils/versions.py` & `clipped-0.0.9/clipped/utils/versions.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.8/clipped/utils/workers.py` & `clipped-0.0.9/clipped/utils/workers.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.8/clipped/utils/yaml.py` & `clipped-0.0.9/clipped/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.8/clipped.egg-info/PKG-INFO` & `clipped-0.0.9/clipped.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipped
-Version: 0.0.8
+Version: 0.0.9
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
-Metadata-Version: 2.1 Name: clipped Version: 0.0.8 Summary: Common shortcuts
+Metadata-Version: 2.1 Name: clipped Version: 0.0.9 Summary: Common shortcuts
 and utils. Home-page: https://github.com/mmourafiq/clipped Author: Mourad
 Mourafiq Author-email: mourad.mourafiq@gmail.com Maintainer: Mourad Mourafiq
 Maintainer-email: mourad.mourafiq@gmail.com License: Apache 2.0 Keywords:
 cli,configuration,utils,setup Platform: any Classifier: Intended Audience ::
 Information Technology Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Science/Research Classifier: Operating System :: OS Independent Classifier:
```

### Comparing `clipped-0.0.8/clipped.egg-info/SOURCES.txt` & `clipped-0.0.9/clipped.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clipped-0.0.8/setup.cfg` & `clipped-0.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `clipped-0.0.8/setup.py` & `clipped-0.0.9/setup.py`

 * *Files identical despite different names*

