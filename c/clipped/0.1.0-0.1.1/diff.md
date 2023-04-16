# Comparing `tmp/clipped-0.1.0.tar.gz` & `tmp/clipped-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clipped-0.1.0.tar", last modified: Sun Apr 16 09:39:49 2023, max compression
+gzip compressed data, was "clipped-0.1.1.tar", last modified: Sun Apr 16 10:41:37 2023, max compression
```

## Comparing `clipped-0.1.0.tar` & `clipped-0.1.1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-16 09:39:49.932514 clipped-0.1.0/
--rw-r--r--   0 mourad     (501) staff       (20)      174 2023-04-16 09:39:00.000000 clipped-0.1.0/MANIFEST.in
--rw-r--r--   0 mourad     (501) staff       (20)     2012 2023-04-16 09:39:49.932597 clipped-0.1.0/PKG-INFO
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-16 09:39:49.924147 clipped-0.1.0/clipped/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/__init__.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-16 09:39:49.925712 clipped-0.1.0/clipped/config/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/config/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)       91 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/config/constants.py
--rw-r--r--   0 mourad     (501) staff       (20)       40 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/config/exceptions.py
--rw-r--r--   0 mourad     (501) staff       (20)     4022 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/config/manager.py
--rw-r--r--   0 mourad     (501) staff       (20)     6136 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/config/parser.py
--rw-r--r--   0 mourad     (501) staff       (20)      527 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/config/patch_strategy.py
--rw-r--r--   0 mourad     (501) staff       (20)    14929 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/config/schema.py
--rw-r--r--   0 mourad     (501) staff       (20)     8856 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/config/spec.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-16 09:39:49.926338 clipped-0.1.0/clipped/decorators/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/decorators/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)      646 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/decorators/cached_property.py
--rw-r--r--   0 mourad     (501) staff       (20)     4355 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/decorators/deprecation.py
--rw-r--r--   0 mourad     (501) staff       (20)     1923 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/decorators/memoization.py
--rw-r--r--   0 mourad     (501) staff       (20)     2686 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/decorators/signals.py
--rw-r--r--   0 mourad     (501) staff       (20)     6224 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/formatting.py
--rw-r--r--   0 mourad     (501) staff       (20)      824 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/manager_interface.py
--rw-r--r--   0 mourad     (501) staff       (20)      203 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/pkg.py
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/py.typed
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-16 09:39:49.927736 clipped-0.1.0/clipped/types/
--rw-r--r--   0 mourad     (501) staff       (20)     3748 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/types/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     1298 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/types/docker_image.py
--rw-r--r--   0 mourad     (501) staff       (20)     1889 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/types/email.py
--rw-r--r--   0 mourad     (501) staff       (20)     1033 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/types/gcs.py
--rw-r--r--   0 mourad     (501) staff       (20)      693 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/types/lists.py
--rw-r--r--   0 mourad     (501) staff       (20)      158 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/types/numbers.py
--rw-r--r--   0 mourad     (501) staff       (20)     1142 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/types/ref_or_obj.py
--rw-r--r--   0 mourad     (501) staff       (20)     1019 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/types/s3.py
--rw-r--r--   0 mourad     (501) staff       (20)     1265 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/types/uri.py
--rw-r--r--   0 mourad     (501) staff       (20)      683 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/types/uuids.py
--rw-r--r--   0 mourad     (501) staff       (20)     3179 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/types/wasb.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-16 09:39:49.932385 clipped-0.1.0/clipped/utils/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/utils/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     1004 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/utils/bools.py
--rw-r--r--   0 mourad     (501) staff       (20)      143 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/utils/click.py
--rw-r--r--   0 mourad     (501) staff       (20)      665 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/utils/cmd.py
--rw-r--r--   0 mourad     (501) staff       (20)      570 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/utils/coroutine.py
--rw-r--r--   0 mourad     (501) staff       (20)      755 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/utils/csv.py
--rw-r--r--   0 mourad     (501) staff       (20)     7568 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/utils/dates.py
--rw-r--r--   0 mourad     (501) staff       (20)     3354 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/utils/dicts.py
--rw-r--r--   0 mourad     (501) staff       (20)      496 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/utils/encoding.py
--rw-r--r--   0 mourad     (501) staff       (20)     1093 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/utils/enums.py
--rw-r--r--   0 mourad     (501) staff       (20)     2001 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/utils/env.py
--rw-r--r--   0 mourad     (501) staff       (20)     4737 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/utils/git.py
--rw-r--r--   0 mourad     (501) staff       (20)     1827 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/utils/hashing.py
--rw-r--r--   0 mourad     (501) staff       (20)     1175 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/utils/http.py
--rw-r--r--   0 mourad     (501) staff       (20)     3363 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/utils/humanize.py
--rw-r--r--   0 mourad     (501) staff       (20)     1327 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/utils/imports.py
--rw-r--r--   0 mourad     (501) staff       (20)     1695 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/utils/indentation.py
--rw-r--r--   0 mourad     (501) staff       (20)      287 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/utils/json.py
--rw-r--r--   0 mourad     (501) staff       (20)     1163 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/utils/lists.py
--rw-r--r--   0 mourad     (501) staff       (20)      113 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/utils/logging.py
--rw-r--r--   0 mourad     (501) staff       (20)     1280 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/utils/np.py
--rw-r--r--   0 mourad     (501) staff       (20)     8484 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/utils/paths.py
--rw-r--r--   0 mourad     (501) staff       (20)      674 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/utils/query_params.py
--rw-r--r--   0 mourad     (501) staff       (20)     1134 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/utils/requests.py
--rw-r--r--   0 mourad     (501) staff       (20)     1041 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/utils/responses.py
--rw-r--r--   0 mourad     (501) staff       (20)      559 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/utils/sanitizers.py
--rw-r--r--   0 mourad     (501) staff       (20)      676 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/utils/serialization.py
--rw-r--r--   0 mourad     (501) staff       (20)     2674 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/utils/strings.py
--rw-r--r--   0 mourad     (501) staff       (20)     1115 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/utils/tz.py
--rw-r--r--   0 mourad     (501) staff       (20)     4040 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/utils/units.py
--rw-r--r--   0 mourad     (501) staff       (20)      269 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/utils/urls.py
--rw-r--r--   0 mourad     (501) staff       (20)      614 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/utils/validation.py
--rw-r--r--   0 mourad     (501) staff       (20)     1128 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/utils/versions.py
--rw-r--r--   0 mourad     (501) staff       (20)     1068 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/utils/workers.py
--rw-r--r--   0 mourad     (501) staff       (20)      546 2023-04-16 09:39:00.000000 clipped-0.1.0/clipped/utils/yaml.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-16 09:39:49.924637 clipped-0.1.0/clipped.egg-info/
--rw-r--r--   0 mourad     (501) staff       (20)     2012 2023-04-16 09:39:49.000000 clipped-0.1.0/clipped.egg-info/PKG-INFO
--rw-r--r--   0 mourad     (501) staff       (20)     1796 2023-04-16 09:39:49.000000 clipped-0.1.0/clipped.egg-info/SOURCES.txt
--rw-r--r--   0 mourad     (501) staff       (20)        1 2023-04-16 09:39:49.000000 clipped-0.1.0/clipped.egg-info/dependency_links.txt
--rw-r--r--   0 mourad     (501) staff       (20)        8 2023-04-16 09:39:49.000000 clipped-0.1.0/clipped.egg-info/top_level.txt
--rw-r--r--   0 mourad     (501) staff       (20)     1033 2023-04-16 09:39:49.933025 clipped-0.1.0/setup.cfg
--rw-r--r--   0 mourad     (501) staff       (20)     2345 2023-04-16 09:39:00.000000 clipped-0.1.0/setup.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-16 10:41:37.724623 clipped-0.1.1/
+-rw-r--r--   0 mourad     (501) staff       (20)      174 2023-04-16 10:40:33.000000 clipped-0.1.1/MANIFEST.in
+-rw-r--r--   0 mourad     (501) staff       (20)     2012 2023-04-16 10:41:37.724722 clipped-0.1.1/PKG-INFO
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-16 10:41:37.714692 clipped-0.1.1/clipped/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/__init__.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-16 10:41:37.716468 clipped-0.1.1/clipped/config/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/config/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)       91 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/config/constants.py
+-rw-r--r--   0 mourad     (501) staff       (20)       40 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/config/exceptions.py
+-rw-r--r--   0 mourad     (501) staff       (20)     4022 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/config/manager.py
+-rw-r--r--   0 mourad     (501) staff       (20)     6164 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/config/parser.py
+-rw-r--r--   0 mourad     (501) staff       (20)      527 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/config/patch_strategy.py
+-rw-r--r--   0 mourad     (501) staff       (20)    14928 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/config/schema.py
+-rw-r--r--   0 mourad     (501) staff       (20)     8892 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/config/spec.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-16 10:41:37.717209 clipped-0.1.1/clipped/decorators/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/decorators/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)      646 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/decorators/cached_property.py
+-rw-r--r--   0 mourad     (501) staff       (20)     4355 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/decorators/deprecation.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1923 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/decorators/memoization.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2686 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/decorators/signals.py
+-rw-r--r--   0 mourad     (501) staff       (20)     6256 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/formatting.py
+-rw-r--r--   0 mourad     (501) staff       (20)      824 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/manager_interface.py
+-rw-r--r--   0 mourad     (501) staff       (20)      203 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/pkg.py
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/py.typed
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-16 10:41:37.718868 clipped-0.1.1/clipped/types/
+-rw-r--r--   0 mourad     (501) staff       (20)     3748 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/types/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1298 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/types/docker_image.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1889 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/types/email.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1033 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/types/gcs.py
+-rw-r--r--   0 mourad     (501) staff       (20)      693 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/types/lists.py
+-rw-r--r--   0 mourad     (501) staff       (20)      158 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/types/numbers.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1142 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/types/ref_or_obj.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1019 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/types/s3.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1265 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/types/uri.py
+-rw-r--r--   0 mourad     (501) staff       (20)      683 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/types/uuids.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3179 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/types/wasb.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-16 10:41:37.724471 clipped-0.1.1/clipped/utils/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1004 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/bools.py
+-rw-r--r--   0 mourad     (501) staff       (20)      143 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/click.py
+-rw-r--r--   0 mourad     (501) staff       (20)      665 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/cmd.py
+-rw-r--r--   0 mourad     (501) staff       (20)      570 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/coroutine.py
+-rw-r--r--   0 mourad     (501) staff       (20)      755 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/csv.py
+-rw-r--r--   0 mourad     (501) staff       (20)     7568 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/dates.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3354 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/dicts.py
+-rw-r--r--   0 mourad     (501) staff       (20)      496 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/encoding.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1093 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/enums.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2001 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/env.py
+-rw-r--r--   0 mourad     (501) staff       (20)     4737 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/git.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1827 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/hashing.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1175 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/http.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3363 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/humanize.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1327 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/imports.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1695 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/indentation.py
+-rw-r--r--   0 mourad     (501) staff       (20)      420 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/json.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1163 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/lists.py
+-rw-r--r--   0 mourad     (501) staff       (20)      113 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/logging.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1280 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/np.py
+-rw-r--r--   0 mourad     (501) staff       (20)     8484 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/paths.py
+-rw-r--r--   0 mourad     (501) staff       (20)      674 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/query_params.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1134 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/requests.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1041 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/responses.py
+-rw-r--r--   0 mourad     (501) staff       (20)      595 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/sanitizers.py
+-rw-r--r--   0 mourad     (501) staff       (20)      676 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/serialization.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2674 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/strings.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1115 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/tz.py
+-rw-r--r--   0 mourad     (501) staff       (20)     4040 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/units.py
+-rw-r--r--   0 mourad     (501) staff       (20)      269 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/urls.py
+-rw-r--r--   0 mourad     (501) staff       (20)      614 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/validation.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1128 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/versions.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1068 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/workers.py
+-rw-r--r--   0 mourad     (501) staff       (20)      546 2023-04-16 10:40:33.000000 clipped-0.1.1/clipped/utils/yaml.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-16 10:41:37.715278 clipped-0.1.1/clipped.egg-info/
+-rw-r--r--   0 mourad     (501) staff       (20)     2012 2023-04-16 10:41:37.000000 clipped-0.1.1/clipped.egg-info/PKG-INFO
+-rw-r--r--   0 mourad     (501) staff       (20)     1796 2023-04-16 10:41:37.000000 clipped-0.1.1/clipped.egg-info/SOURCES.txt
+-rw-r--r--   0 mourad     (501) staff       (20)        1 2023-04-16 10:41:37.000000 clipped-0.1.1/clipped.egg-info/dependency_links.txt
+-rw-r--r--   0 mourad     (501) staff       (20)        8 2023-04-16 10:41:37.000000 clipped-0.1.1/clipped.egg-info/top_level.txt
+-rw-r--r--   0 mourad     (501) staff       (20)     1033 2023-04-16 10:41:37.725202 clipped-0.1.1/setup.cfg
+-rw-r--r--   0 mourad     (501) staff       (20)     2345 2023-04-16 10:40:33.000000 clipped-0.1.1/setup.py
```

### Comparing `clipped-0.1.0/PKG-INFO` & `clipped-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipped
-Version: 0.1.0
+Version: 0.1.1
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
-Metadata-Version: 2.1 Name: clipped Version: 0.1.0 Summary: Common shortcuts
+Metadata-Version: 2.1 Name: clipped Version: 0.1.1 Summary: Common shortcuts
 and utils. Home-page: https://github.com/mmourafiq/clipped Author: Mourad
 Mourafiq Author-email: mourad.mourafiq@gmail.com Maintainer: Mourad Mourafiq
 Maintainer-email: mourad.mourafiq@gmail.com License: Apache 2.0 Keywords:
 cli,configuration,utils,setup Platform: any Classifier: Intended Audience ::
 Information Technology Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Science/Research Classifier: Operating System :: OS Independent Classifier:
```

### Comparing `clipped-0.1.0/clipped/config/manager.py` & `clipped-0.1.1/clipped/config/manager.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.0/clipped/config/parser.py` & `clipped-0.1.1/clipped/config/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 import logging
 
 from typing import Any, Callable, List, Optional, Type, TypeVar
 
-import orjson
-
 from pydantic import PydanticTypeError, PydanticValueError, StrBytes, ValidationError
-from pydantic.parse import load_str_bytes, Protocol
+from pydantic.parse import Protocol, load_str_bytes
 from pydantic.tools import NameFactory, _get_parsing_type
 
 from clipped.config.constants import NO_VALUE_FOUND
 from clipped.config.exceptions import SchemaError
 from clipped.decorators.memoization import memoize, memoize_method
-
+from clipped.utils.json import orjson_loads
 
 _logger = logging.getLogger("clipped.parser")
 
 T = TypeVar("T")
 
 
 class Parser:
@@ -56,15 +54,15 @@
         type_: Type[T],
         b: StrBytes,
         *,
         content_type: str = None,
         encoding: str = "utf8",
         proto: Protocol = None,
         allow_pickle: bool = False,
-        json_loads: Callable[[str], Any] = orjson.loads,
+        json_loads: Callable[[str], Any] = orjson_loads,
         type_name: Optional[NameFactory] = None,
     ) -> T:
         obj = load_str_bytes(
             b,
             proto=proto,
             content_type=content_type,
             encoding=encoding,
@@ -110,15 +108,15 @@
                     "No value was provided for the non optional key `{}`.".format(key)
                 )
             return default
 
         try:
             if cls.is_loadable(target_type) and isinstance(value, str):
                 new_value = cls.parse_raw_as(
-                    target_type, value, json_loads=orjson.loads
+                    target_type, value, json_loads=orjson_loads
                 )
             else:
                 new_value = cls.parse_obj_as(target_type, value)
             cls._check_options(key=key, value=new_value, options=options)
             return new_value
         except (
             TypeError,
```

### Comparing `clipped-0.1.0/clipped/config/patch_strategy.py` & `clipped-0.1.1/clipped/config/patch_strategy.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.0/clipped/config/schema.py` & `clipped-0.1.1/clipped/config/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 import functools
 import os
 import pprint
 
 from collections.abc import Mapping
 from typing import Any, Callable, Dict, List, Optional, Union
 
-import orjson
-
 from pydantic import BaseModel, Extra
 
 from clipped.config.exceptions import SchemaError
 from clipped.config.patch_strategy import PatchStrategy
 from clipped.config.spec import ConfigSpec
 from clipped.utils.dicts import deep_update
 from clipped.utils.humanize import humanize_timesince
-from clipped.utils.json import orjson_dumps
+from clipped.utils.json import orjson_dumps, orjson_loads
 from clipped.utils.strings import to_camel_case
 from clipped.utils.units import to_percentage, to_unit_memory
 
 
 class BaseSchemaModel(BaseModel):
     _IDENTIFIER: Optional[str] = None
     _DEFAULT_INCLUDE_ATTRIBUTES = []
@@ -399,15 +397,15 @@
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         arbitrary_types_allowed = True
         use_enum_values = True
         extra = Extra.forbid
         json_dumps: Callable[..., str] = orjson_dumps
-        json_loads = orjson.loads
+        json_loads = orjson_loads
 
 
 def to_partial(cls):
     class NewCls(cls):
         _PARTIAL = True
 
     NewCls.__name__ = f"Partial{cls.__name__}"
```

### Comparing `clipped-0.1.0/clipped/config/spec.py` & `clipped-0.1.1/clipped/config/spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-import json
 import os
 import sys
 import yaml
 
 from collections.abc import Mapping
 from requests import HTTPError
 from typing import Any, Dict
 from yaml.parser import ParserError
 from yaml.scanner import ScannerError
 
 from clipped.config.exceptions import SchemaError
 from clipped.utils.dicts import deep_update
+from clipped.utils.json import orjson_loads
 from clipped.utils.lists import to_list
 
 
 class ConfigSpec:
     _SCHEMA_EXCEPTION = SchemaError
 
     def __init__(
@@ -235,17 +235,17 @@
                 "Received non valid yaml: `%s`.\n" "Yaml error %s" % (f_path, e)
             ) from e
 
     @classmethod
     def read_from_json(cls, f_path, is_stream=False):
         if is_stream:
             try:
-                return json.loads(f_path)
+                return orjson_loads(f_path)
             except ValueError as e:
                 raise cls._SCHEMA_EXCEPTION("Json error: %s" % e) from e
         try:
             with open(f_path) as f:
-                return json.loads(f.read())
+                return orjson_loads(f.read())
         except ValueError as e:
             raise cls._SCHEMA_EXCEPTION(
                 "Received non valid json: `%s`.\n" "Json error %s" % (f_path, e)
             ) from e
```

### Comparing `clipped-0.1.0/clipped/decorators/cached_property.py` & `clipped-0.1.1/clipped/decorators/cached_property.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.0/clipped/decorators/deprecation.py` & `clipped-0.1.1/clipped/decorators/deprecation.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.0/clipped/decorators/memoization.py` & `clipped-0.1.1/clipped/decorators/memoization.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.0/clipped/decorators/signals.py` & `clipped-0.1.1/clipped/decorators/signals.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.0/clipped/formatting.py` & `clipped-0.1.1/clipped/formatting.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import json
 import sys
 import yaml
 
 from typing import Dict, List, Optional, Union
 
 import click
 
@@ -21,14 +20,15 @@
     TransferSpeedColumn,
 )
 from rich.syntax import Syntax
 from rich.table import Column, Table
 from rich.theme import Theme
 
 from clipped.utils.humanize import humanize_attrs
+from clipped.utils.json import orjson_dumps, orjson_loads, orjson_pprint_option
 from clipped.utils.lists import to_list
 from clipped.utils.units import to_unit_memory
 
 
 class Printer:
     COLORS = ["yellow", "blue", "magenta", "green", "cyan", "red", "white"]
     console = Console(
@@ -66,15 +66,15 @@
     @staticmethod
     def get_table(*args, **kwargs):
         return Table(*[Column(header=h, no_wrap=True) for h in args], **kwargs)
 
     @staticmethod
     def pprint(value):
         """Prints as formatted JSON"""
-        click.echo(json.dumps(value, sort_keys=True, indent=4, separators=(",", ": ")))
+        click.echo(orjson_dumps(value, option=orjson_pprint_option))
 
     @classmethod
     def print_md(cls, md: str):
         cls.console.print(Markdown(md))
 
     @classmethod
     def print_text(cls, value: str):
@@ -88,16 +88,16 @@
         value = yaml.safe_dump(value, sort_keys=True, indent=2)
         syntax = Syntax(value, "yaml", theme="dracula", line_numbers=False)
         cls.console.print(syntax)
 
     @classmethod
     def print_json(cls, value: any):
         if isinstance(value, str):
-            value = json.loads(value)
-        value = json.dumps(value, sort_keys=True, indent=4, separators=(",", ": "))
+            value = orjson_loads(value)
+        value = orjson_dumps(value, option=orjson_pprint_option)
         syntax = Syntax(value, "json", theme="dracula", line_numbers=False)
         cls.console.print(syntax)
 
     @classmethod
     def print(cls, text: str):
         cls.console.print(text)
```

### Comparing `clipped-0.1.0/clipped/manager_interface.py` & `clipped-0.1.1/clipped/manager_interface.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.0/clipped/types/__init__.py` & `clipped-0.1.1/clipped/types/__init__.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.0/clipped/types/docker_image.py` & `clipped-0.1.1/clipped/types/docker_image.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.0/clipped/types/email.py` & `clipped-0.1.1/clipped/types/email.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.0/clipped/types/gcs.py` & `clipped-0.1.1/clipped/types/gcs.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.0/clipped/types/lists.py` & `clipped-0.1.1/clipped/types/lists.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.0/clipped/types/ref_or_obj.py` & `clipped-0.1.1/clipped/types/ref_or_obj.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.0/clipped/types/s3.py` & `clipped-0.1.1/clipped/types/s3.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.0/clipped/types/uri.py` & `clipped-0.1.1/clipped/types/uri.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.0/clipped/types/uuids.py` & `clipped-0.1.1/clipped/types/uuids.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.0/clipped/types/wasb.py` & `clipped-0.1.1/clipped/types/wasb.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.0/clipped/utils/bools.py` & `clipped-0.1.1/clipped/utils/bools.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.0/clipped/utils/cmd.py` & `clipped-0.1.1/clipped/utils/cmd.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.0/clipped/utils/coroutine.py` & `clipped-0.1.1/clipped/utils/coroutine.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.0/clipped/utils/csv.py` & `clipped-0.1.1/clipped/utils/csv.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.0/clipped/utils/dates.py` & `clipped-0.1.1/clipped/utils/dates.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.0/clipped/utils/dicts.py` & `clipped-0.1.1/clipped/utils/dicts.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.0/clipped/utils/enums.py` & `clipped-0.1.1/clipped/utils/enums.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.0/clipped/utils/env.py` & `clipped-0.1.1/clipped/utils/env.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.0/clipped/utils/git.py` & `clipped-0.1.1/clipped/utils/git.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.0/clipped/utils/hashing.py` & `clipped-0.1.1/clipped/utils/hashing.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.0/clipped/utils/http.py` & `clipped-0.1.1/clipped/utils/http.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.0/clipped/utils/humanize.py` & `clipped-0.1.1/clipped/utils/humanize.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.0/clipped/utils/imports.py` & `clipped-0.1.1/clipped/utils/imports.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.0/clipped/utils/indentation.py` & `clipped-0.1.1/clipped/utils/indentation.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.0/clipped/utils/lists.py` & `clipped-0.1.1/clipped/utils/lists.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.0/clipped/utils/np.py` & `clipped-0.1.1/clipped/utils/np.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.0/clipped/utils/paths.py` & `clipped-0.1.1/clipped/utils/paths.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.0/clipped/utils/query_params.py` & `clipped-0.1.1/clipped/utils/query_params.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.0/clipped/utils/requests.py` & `clipped-0.1.1/clipped/utils/requests.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.0/clipped/utils/responses.py` & `clipped-0.1.1/clipped/utils/responses.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.0/clipped/utils/sanitizers.py` & `clipped-0.1.1/clipped/utils/sanitizers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-import json
-
 from collections.abc import Mapping
 from typing import Dict
 
+from clipped.utils.json import orjson_dumps
+
 
 def sanitize_value(d: Dict, handle_dict: bool = False):
     if isinstance(d, str):
         return d
     if not isinstance(d, Mapping):
-        return json.dumps(d)
+        return orjson_dumps(d)
     if not handle_dict:
-        return json.dumps(d)
+        return orjson_dumps(d)
     return {d_k: sanitize_value(d_v, handle_dict=True) for d_k, d_v in d.items()}
 
 
 def sanitize_string_dict(d: Dict[str, str] = None):
     if isinstance(d, Mapping):
         return {d_k: sanitize_value(d_v, handle_dict=False) for d_k, d_v in d.items()}
     return d
```

### Comparing `clipped-0.1.0/clipped/utils/serialization.py` & `clipped-0.1.1/clipped/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.0/clipped/utils/strings.py` & `clipped-0.1.1/clipped/utils/strings.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.0/clipped/utils/tz.py` & `clipped-0.1.1/clipped/utils/tz.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.0/clipped/utils/units.py` & `clipped-0.1.1/clipped/utils/units.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.0/clipped/utils/validation.py` & `clipped-0.1.1/clipped/utils/validation.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.0/clipped/utils/versions.py` & `clipped-0.1.1/clipped/utils/versions.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.0/clipped/utils/workers.py` & `clipped-0.1.1/clipped/utils/workers.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.0/clipped/utils/yaml.py` & `clipped-0.1.1/clipped/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `clipped-0.1.0/clipped.egg-info/PKG-INFO` & `clipped-0.1.1/clipped.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipped
-Version: 0.1.0
+Version: 0.1.1
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
-Metadata-Version: 2.1 Name: clipped Version: 0.1.0 Summary: Common shortcuts
+Metadata-Version: 2.1 Name: clipped Version: 0.1.1 Summary: Common shortcuts
 and utils. Home-page: https://github.com/mmourafiq/clipped Author: Mourad
 Mourafiq Author-email: mourad.mourafiq@gmail.com Maintainer: Mourad Mourafiq
 Maintainer-email: mourad.mourafiq@gmail.com License: Apache 2.0 Keywords:
 cli,configuration,utils,setup Platform: any Classifier: Intended Audience ::
 Information Technology Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Science/Research Classifier: Operating System :: OS Independent Classifier:
```

### Comparing `clipped-0.1.0/clipped.egg-info/SOURCES.txt` & `clipped-0.1.1/clipped.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clipped-0.1.0/setup.cfg` & `clipped-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `clipped-0.1.0/setup.py` & `clipped-0.1.1/setup.py`

 * *Files identical despite different names*

