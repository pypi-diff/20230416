# Comparing `tmp/fresco-3.1.0.tar.gz` & `tmp/fresco-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fresco-3.1.0.tar", last modified: Wed May  4 19:52:55 2022, max compression
+gzip compressed data, was "fresco-3.2.0.tar", last modified: Sun Apr 16 17:05:39 2023, max compression
```

## Comparing `fresco-3.1.0.tar` & `fresco-3.2.0.tar`

### file list

```diff
@@ -1,68 +1,69 @@
-drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2022-05-04 19:52:55.002662 fresco-3.1.0/
--rw-r--r--   0 oliver    (1001) wheel        (0)    19421 2022-05-04 19:49:20.000000 fresco-3.1.0/CHANGELOG.rst
--rw-r--r--   0 oliver    (1001) wheel        (0)    11358 2022-05-04 19:49:19.000000 fresco-3.1.0/LICENSE.txt
--rw-r--r--   0 oliver    (1001) wheel        (0)       50 2022-05-04 19:49:19.000000 fresco-3.1.0/MANIFEST.in
--rw-r--r--   0 oliver    (1001) wheel        (0)     1595 2022-05-04 19:52:55.002766 fresco-3.1.0/PKG-INFO
--rw-r--r--   0 oliver    (1001) wheel        (0)      822 2022-05-04 19:49:19.000000 fresco-3.1.0/README.rst
-drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2022-05-04 19:52:54.994399 fresco-3.1.0/fresco/
--rw-r--r--   0 oliver    (1001) wheel        (0)      917 2022-05-04 19:52:06.000000 fresco-3.1.0/fresco/__init__.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     7056 2022-05-04 19:49:19.000000 fresco-3.1.0/fresco/cookie.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    25662 2022-05-04 19:49:19.000000 fresco-3.1.0/fresco/core.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     3270 2022-05-04 19:49:19.000000 fresco-3.1.0/fresco/decorators.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     4410 2022-05-04 19:49:19.000000 fresco-3.1.0/fresco/exceptions.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     4172 2022-05-04 19:49:19.000000 fresco-3.1.0/fresco/middleware.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    13094 2022-05-04 19:49:19.000000 fresco-3.1.0/fresco/multidict.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    10272 2022-05-04 19:49:19.000000 fresco-3.1.0/fresco/options.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    26473 2022-05-04 19:49:19.000000 fresco-3.1.0/fresco/request.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     3339 2022-05-04 19:49:19.000000 fresco-3.1.0/fresco/requestcontext.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    38276 2022-05-04 19:49:19.000000 fresco-3.1.0/fresco/response.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    10176 2022-05-04 19:49:19.000000 fresco-3.1.0/fresco/routeargs.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    56619 2022-05-04 19:49:19.000000 fresco-3.1.0/fresco/routing.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     2513 2022-05-04 19:49:19.000000 fresco-3.1.0/fresco/static.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    10591 2022-05-04 19:49:19.000000 fresco-3.1.0/fresco/subrequests.py
-drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2022-05-04 19:52:54.998538 fresco-3.1.0/fresco/tests/
--rw-r--r--   0 oliver    (1001) wheel        (0)        0 2022-05-04 19:49:19.000000 fresco-3.1.0/fresco/tests/__init__.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     1747 2022-05-04 19:49:19.000000 fresco-3.1.0/fresco/tests/fixtures.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     2193 2022-05-04 19:49:19.000000 fresco-3.1.0/fresco/tests/test_cookie.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    33786 2022-05-04 19:49:19.000000 fresco-3.1.0/fresco/tests/test_core.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     1502 2022-05-04 19:49:19.000000 fresco-3.1.0/fresco/tests/test_decorators.py
--rw-r--r--   0 oliver    (1001) wheel        (0)      973 2022-05-04 19:49:19.000000 fresco-3.1.0/fresco/tests/test_exceptions.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     3141 2022-05-04 19:49:19.000000 fresco-3.1.0/fresco/tests/test_middleware.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     7579 2022-05-04 19:49:19.000000 fresco-3.1.0/fresco/tests/test_multidict.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     8605 2022-05-04 19:49:19.000000 fresco-3.1.0/fresco/tests/test_options.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    15931 2022-05-04 19:49:19.000000 fresco-3.1.0/fresco/tests/test_request.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     3116 2022-05-04 19:49:19.000000 fresco-3.1.0/fresco/tests/test_requestcontext.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     8940 2022-05-04 19:49:19.000000 fresco-3.1.0/fresco/tests/test_response.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     8167 2022-05-04 19:49:19.000000 fresco-3.1.0/fresco/tests/test_routeargs.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    36555 2022-05-04 19:49:19.000000 fresco-3.1.0/fresco/tests/test_routing.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     4673 2022-05-04 19:49:19.000000 fresco-3.1.0/fresco/tests/test_static.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     7128 2022-05-04 19:49:19.000000 fresco-3.1.0/fresco/tests/test_subrequests.py
-drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2022-05-04 19:52:54.999988 fresco-3.1.0/fresco/tests/util/
--rw-r--r--   0 oliver    (1001) wheel        (0)        0 2022-05-04 19:49:19.000000 fresco-3.1.0/fresco/tests/util/__init__.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    10570 2022-05-04 19:49:19.000000 fresco-3.1.0/fresco/tests/util/form_data.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     1117 2022-05-04 19:49:19.000000 fresco-3.1.0/fresco/tests/util/test_common.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    10765 2022-05-04 19:49:19.000000 fresco-3.1.0/fresco/tests/util/test_http.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     1492 2022-05-04 19:49:19.000000 fresco-3.1.0/fresco/tests/util/test_security.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     7689 2022-05-04 19:49:19.000000 fresco-3.1.0/fresco/tests/util/test_urls.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     3040 2022-05-04 19:49:19.000000 fresco-3.1.0/fresco/tests/util/test_wsgi.py
--rw-r--r--   0 oliver    (1001) wheel        (0)      347 2022-05-04 19:49:19.000000 fresco-3.1.0/fresco/typing.py
-drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2022-05-04 19:52:55.002478 fresco-3.1.0/fresco/util/
--rw-r--r--   0 oliver    (1001) wheel        (0)        7 2022-05-04 19:49:19.000000 fresco-3.1.0/fresco/util/__init__.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     1609 2022-05-04 19:49:19.000000 fresco-3.1.0/fresco/util/cache.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     1274 2022-05-04 19:49:19.000000 fresco-3.1.0/fresco/util/common.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     5483 2022-05-04 19:49:19.000000 fresco-3.1.0/fresco/util/contentencodings.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     1383 2022-05-04 19:49:19.000000 fresco-3.1.0/fresco/util/file.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    20940 2022-05-04 19:49:19.000000 fresco-3.1.0/fresco/util/http.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     1320 2022-05-04 19:49:19.000000 fresco-3.1.0/fresco/util/io.py
--rw-r--r--   0 oliver    (1001) wheel        (0)      370 2022-05-04 19:49:19.000000 fresco-3.1.0/fresco/util/object.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     1058 2022-05-04 19:49:19.000000 fresco-3.1.0/fresco/util/security.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     2309 2022-05-04 19:49:19.000000 fresco-3.1.0/fresco/util/textproc.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     9107 2022-05-04 19:49:19.000000 fresco-3.1.0/fresco/util/urls.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    12731 2022-05-04 19:49:19.000000 fresco-3.1.0/fresco/util/wsgi.py
-drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2022-05-04 19:52:54.995224 fresco-3.1.0/fresco.egg-info/
--rw-r--r--   0 oliver    (1001) wheel        (0)     1595 2022-05-04 19:52:54.000000 fresco-3.1.0/fresco.egg-info/PKG-INFO
--rw-r--r--   0 oliver    (1001) wheel        (0)     1460 2022-05-04 19:52:54.000000 fresco-3.1.0/fresco.egg-info/SOURCES.txt
--rw-r--r--   0 oliver    (1001) wheel        (0)        1 2022-05-04 19:52:54.000000 fresco-3.1.0/fresco.egg-info/dependency_links.txt
--rw-r--r--   0 oliver    (1001) wheel        (0)        7 2022-05-04 19:52:54.000000 fresco-3.1.0/fresco.egg-info/top_level.txt
--rw-r--r--   0 oliver    (1001) wheel        (0)      795 2022-05-04 19:52:55.003374 fresco-3.1.0/setup.cfg
--rw-r--r--   0 oliver    (1001) wheel        (0)      634 2022-05-04 19:49:19.000000 fresco-3.1.0/setup.py
+drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-04-16 17:05:39.020991 fresco-3.2.0/
+-rw-r--r--   0 oliver    (1001) wheel        (0)    20107 2023-04-16 17:02:23.000000 fresco-3.2.0/CHANGELOG.rst
+-rw-r--r--   0 oliver    (1001) wheel        (0)    11358 2023-04-16 17:02:22.000000 fresco-3.2.0/LICENSE.txt
+-rw-r--r--   0 oliver    (1001) wheel        (0)       50 2023-04-16 17:02:22.000000 fresco-3.2.0/MANIFEST.in
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1575 2023-04-16 17:05:39.021103 fresco-3.2.0/PKG-INFO
+-rw-r--r--   0 oliver    (1001) wheel        (0)      822 2023-04-16 17:02:22.000000 fresco-3.2.0/README.rst
+drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-04-16 17:05:39.012626 fresco-3.2.0/fresco/
+-rw-r--r--   0 oliver    (1001) wheel        (0)      917 2023-04-16 17:05:34.000000 fresco-3.2.0/fresco/__init__.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     7055 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/cookie.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    26509 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/core.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     3232 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/decorators.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     4410 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/exceptions.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     4171 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/middleware.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    13004 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/multidict.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    10272 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/options.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    27071 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/request.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     3339 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/requestcontext.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    37099 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/response.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    10176 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/routeargs.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    57738 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/routing.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     2513 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/static.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    11016 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/subrequests.py
+drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-04-16 17:05:39.016820 fresco-3.2.0/fresco/tests/
+-rw-r--r--   0 oliver    (1001) wheel        (0)        0 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/tests/__init__.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1871 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/tests/fixtures.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     2171 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/tests/test_cookie.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    34019 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/tests/test_core.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1480 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/tests/test_decorators.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)      973 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/tests/test_exceptions.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     3137 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/tests/test_middleware.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     7565 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/tests/test_multidict.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     8603 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/tests/test_options.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    16389 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/tests/test_request.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     3115 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/tests/test_requestcontext.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     8934 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/tests/test_response.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     8162 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/tests/test_routeargs.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    36812 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/tests/test_routing.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     4686 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/tests/test_static.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     7909 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/tests/test_subrequests.py
+drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-04-16 17:05:39.018308 fresco-3.2.0/fresco/tests/util/
+-rw-r--r--   0 oliver    (1001) wheel        (0)        0 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/tests/util/__init__.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    10570 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/tests/util/form_data.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1117 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/tests/util/test_common.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    10803 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/tests/util/test_http.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1492 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/tests/util/test_security.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     7643 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/tests/util/test_urls.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     3038 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/tests/util/test_wsgi.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)      106 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/types.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)      347 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/typing.py
+drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-04-16 17:05:39.020805 fresco-3.2.0/fresco/util/
+-rw-r--r--   0 oliver    (1001) wheel        (0)        7 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/util/__init__.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1609 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/util/cache.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1258 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/util/common.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     5484 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/util/contentencodings.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1383 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/util/file.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    22126 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/util/http.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1289 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/util/io.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)      370 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/util/object.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1058 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/util/security.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     2309 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/util/textproc.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     9195 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/util/urls.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    12970 2023-04-16 17:02:22.000000 fresco-3.2.0/fresco/util/wsgi.py
+drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-04-16 17:05:39.013444 fresco-3.2.0/fresco.egg-info/
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1575 2023-04-16 17:05:38.000000 fresco-3.2.0/fresco.egg-info/PKG-INFO
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1476 2023-04-16 17:05:38.000000 fresco-3.2.0/fresco.egg-info/SOURCES.txt
+-rw-r--r--   0 oliver    (1001) wheel        (0)        1 2023-04-16 17:05:38.000000 fresco-3.2.0/fresco.egg-info/dependency_links.txt
+-rw-r--r--   0 oliver    (1001) wheel        (0)        7 2023-04-16 17:05:38.000000 fresco-3.2.0/fresco.egg-info/top_level.txt
+-rw-r--r--   0 oliver    (1001) wheel        (0)      795 2023-04-16 17:05:39.021821 fresco-3.2.0/setup.cfg
+-rw-r--r--   0 oliver    (1001) wheel        (0)      634 2023-04-16 17:02:22.000000 fresco-3.2.0/setup.py
```

### Comparing `fresco-3.1.0/CHANGELOG.rst` & `fresco-3.2.0/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,25 @@
 Changelog
 =========
 
+
+3.2.0 (released 2023-04-16)
+---------------------------
+
+- Bugfix: fixed cases where the close methods of WSGI content iterators were
+  not called, notably when using subrequests
+- Bugfix: fix ``ResourceWarnings`` caused by unclosed temporary files
+- Added ``route_class`` argument to ``RouteCollection.route``
+- Modified ``RouteCollection.route_wsgi`` to allow it to take a string path to
+  the WSGI callable instead of the callable itself, making its signature more
+  consistent with ``RouteCollection.route``
+- Added ``fresco.process_request_once``
+- ``request.make_url`` and ``fresco.util.url.make_query`` now drop items from
+  the generated query string if the value is ``None``
+
 3.1.0 (released 2022-05-04)
 ---------------------------
 
 - Bugfix: passing URL paths to subrequests no longer raises an exception
 - Added an ``_env`` argument to ``fresco.subrequest.subrequest`` to allow custom
   WSGI environ keys to be passed to the subrequest
```

### Comparing `fresco-3.1.0/LICENSE.txt` & `fresco-3.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fresco-3.1.0/PKG-INFO` & `fresco-3.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: fresco
-Version: 3.1.0
+Version: 3.2.0
 Summary: A Web/WSGI micro-framework
 Home-page: https://ollycope.com/software/fresco/latest/
 Author: Oliver Cope
 Author-email: oliver@redgecko.org
 License: Apache
 Keywords: wsgi web www framework
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: PyPy
@@ -42,9 +41,7 @@
 
 
 Read the
 `fresco web framework documentation
 <https://ollycope.com/software/fresco/latest/>`_ for
 more about the framework, or
 visit the `source repo <https://sr.ht/~olly/fresco/>`_.
-
-
```

### Comparing `fresco-3.1.0/README.rst` & `fresco-3.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `fresco-3.1.0/fresco/__init__.py` & `fresco-3.2.0/fresco/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 #     Unless required by applicable law or agreed to in writing, software
 #     distributed under the License is distributed on an "AS IS" BASIS,
 #     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #     See the License for the specific language governing permissions and
 #     limitations under the License.
 #
-__version__ = "3.1.0"
+__version__ = "3.2.0"
 
 DEFAULT_CHARSET = "UTF-8"
 
 from .request import *  # noqa
 from .requestcontext import context  # noqa
 from .response import *  # noqa
 from .core import *  # noqa
```

### Comparing `fresco-3.1.0/fresco/cookie.py` & `fresco-3.2.0/fresco/cookie.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,15 +159,14 @@
                     returned
     """
     if not cookie_string:
         return []
     cookies = []
 
     for part in cookie_string.split(";"):
-
         try:
             k, v = part.strip().split("=", 1)
         except ValueError:
             continue
 
         if k[0] == "$":
             # An attribute (eg path or domain) pertaining to the most recently
```

### Comparing `fresco-3.1.0/fresco/core.py` & `fresco-3.2.0/fresco/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,21 +9,23 @@
 #     Unless required by applicable law or agreed to in writing, software
 #     distributed under the License is distributed on an "AS IS" BASIS,
 #     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #     See the License for the specific language governing permissions and
 #     limitations under the License.
 #
 from functools import partial
+from functools import wraps
 from typing import Callable
 from typing import Dict
 from typing import List
 from typing import Tuple
 from typing import Type
 from typing import Set
 from typing import Union
+import typing as t
 import contextlib
 import logging
 import sys
 import types
 
 from fresco.request import Request
 from fresco.response import Response
@@ -60,15 +62,14 @@
     #: A stdlib logger object, or None
     logger = None
 
     #: Class to use to instantiate request objects
     request_class = Request
 
     def __init__(self, *args, **kwargs):
-
         views = kwargs.pop("views", None)
         path = kwargs.pop("path", None)
         super(FrescoApp, self).__init__(*args, **kwargs)
 
         if views is not None:
             if path is None:
                 path = "/"
@@ -266,19 +267,15 @@
     def view(self, request=None) -> Response:
         request = request or context.request
         try:
             path = request.path_info
         except ResponseException as e:
             response = e.response
         else:
-            response = self.get_response(
-                request,
-                path,
-                request.method
-            )
+            response = self.get_response(request, path, request.method)
 
         for f in self.process_response_handlers:
             try:
                 r = f(request, response)
                 if r is not None:
                     response = r
             except Exception:
@@ -327,15 +324,14 @@
 
     def handle_exception(
         self, request, allow_reraise=True
     ) -> Union[
         Response,
         Tuple[Type[BaseException], BaseException, types.TracebackType],
     ]:
-
         exc_info = sys.exc_info()
         if exc_info[0] is None:
             raise AssertionError(
                 "handle_exception called " "when no exception is being handled"
             )
 
         have_error_handlers = self.process_exception_handlers or any(
@@ -446,36 +442,36 @@
             context_pop=context.pop,
         ):
             request = request_class(environ)
             context_push(request=request, app=frescoapp)
             iterator = None
             try:
                 iterator = wsgi_app(environ, start_response)
-                for item in iterator:
-                    yield item
+                yield from iterator
             except Exception:
                 exc_info = sys.exc_info()
                 try:
                     response = frescoapp.handle_exception(request)
                     if "400" <= response.status <= "599":
                         response = frescoapp.handle_http_error_response(
                             request, response
                         )
 
                     def exc_start_response(s, h, exc_info=exc_info):
                         return start_response(s, h, exc_info)
 
-                    for item in response(environ, exc_start_response):
-                        yield item
+                    yield from response(environ, exc_start_response)
                 finally:
                     del exc_info
             finally:
                 try:
                     if process_teardown_handlers:
                         call_process_teardown_handlers(request)
+                    for item in request.teardown_handlers:
+                        item()
                 finally:
                     try:
                         close = getattr(iterator, "close", None)
                         if close is not None:
                             close()
                     finally:
                         context_pop()
@@ -558,14 +554,35 @@
         """
         for func in self.process_teardown_handlers:
             try:
                 func(request)
             except Exception:
                 self.log_exception(request)
 
+    def process_request_once(
+        self, func: Callable[[Request], t.Optional[Response]]
+    ) -> Callable[[Request], t.Optional[Response]]:
+        """
+        Register a ``process_request`` hook function that is called only once
+
+        When running fresco with multiple worker threads/processes the hook
+        function will be called at most once per worker.
+        """
+
+        @self.process_request
+        @wraps(func)
+        def process_request_once(request: Request) -> t.Optional[Response]:
+            try:
+                self.process_request_handlers.remove(process_request_once)
+            except ValueError:
+                return None
+            return func(request)
+
+        return func
+
     def process_request(self, func):
         """
         Register a ``process_request`` hook function
         """
         self.process_request_handlers.append(func)
         return func
 
@@ -651,35 +668,39 @@
 
         def fake_start_response(status, headers, exc_info=None):
             return lambda s: None
 
         environ = make_environ(url, environ, wsgi_input, **kwargs)
         app = self.make_wsgi_app(wsgi_app=fake_app, use_middleware=middleware)
         result = app(environ, fake_start_response)
-        close = getattr(result, "close", lambda: None)
+        close = getattr(result, "close", None)
         content_iterator = iter(result)
-        next(content_iterator, None)
-        yield context
-        list(content_iterator)
-        close()
+        try:
+            next(content_iterator, None)
+            yield context
+            list(content_iterator)
+        finally:
+            if close is not None:
+                close()
 
     def requestcontext_with_payload(
         self, url="/", data=None, environ=None, files=None, multipart=False, **kwargs
     ):
-
         if files:
             multipart = True
 
         if multipart:
             wsgi_input, headers = encode_multipart(data, files)
             kwargs.update(headers)
         elif hasattr(data, "read"):
             wsgi_input = data.read()
         elif isinstance(data, bytes):
             wsgi_input = data
+        elif data is None:
+            wsgi_input = ""
         else:
             wsgi_input = make_query(data).encode("ascii")
 
         if "CONTENT_LENGTH" not in kwargs:
             kwargs["CONTENT_LENGTH"] = str(len(wsgi_input))
 
         return self.requestcontext(url, environ, wsgi_input=wsgi_input, **kwargs)
```

### Comparing `fresco-3.1.0/fresco/decorators.py` & `fresco-3.2.0/fresco/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,17 +75,15 @@
     """
     # Called as a decorator or decorator factory
     if data is _marker or callable(data):
 
         def json_response_decorator(func):
             @wraps(func)
             def json_response_decorated(*fa, **fkw):
-                return Response.json(
-                    func(*fa, **fkw), indent, separators, **kwargs
-                )
+                return Response.json(func(*fa, **fkw), indent, separators, **kwargs)
 
             return json_response_decorated
 
         # Called as a decorator factory (``@json_response()``)
         if data is _marker:
             return json_response_decorator
```

### Comparing `fresco-3.1.0/fresco/exceptions.py` & `fresco-3.2.0/fresco/exceptions.py`

 * *Files identical despite different names*

### Comparing `fresco-3.1.0/fresco/middleware.py` & `fresco-3.2.0/fresco/middleware.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,14 @@
             environ["SERVER_PORT"] = port
 
         if is_ssl:
             environ["wsgi.url_scheme"] = "https"
             environ["HTTPS"] = "on"
 
         try:
-
             forwards = environ["HTTP_X_FORWARDED_FOR"].split(", ") + [
                 env("REMOTE_ADDR", "")
             ]
         except KeyError:
             # No X-Forwarded-For header?
             return self.app(environ, start_response)
```

### Comparing `fresco-3.1.0/fresco/multidict.py` & `fresco-3.2.0/fresco/multidict.py`

 * *Files 0% similar despite different names*

```diff
@@ -346,33 +346,29 @@
 
                 >>> d = MultiDict([('name', 'eric'),\
                 ...                ('occupation', 'lumberjack')])
                 >>> d.update(mood='okay')
 
         """
         if len(args) > 1:
-            raise TypeError(
-                "expected at most 1 argument, got %d" % (1 + len(args),)
-            )
+            raise TypeError("expected at most 1 argument, got %d" % (1 + len(args),))
         if args:
             other = args[0]
         else:
             other = []
         return self._update(other, True, **kwargs)
 
     def extend(self, *args, **kwargs):
         """
         Extend the MultiDict with another MultiDict, regular dictionary or a
         iterable of ``(key, value)`` pairs. This is similar to :meth:`update`
         except that new keys are added to old keys.
         """
         if len(args) > 1:
-            raise TypeError(
-                "expected at most 1 argument, got %d", (1 + len(args),)
-            )
+            raise TypeError("expected at most 1 argument, got %d", (1 + len(args),))
         if args:
             other = args[0]
         else:
             other = []
         return self._update(other, False, **kwargs)
 
     def _update(self, *args, **kwargs):
@@ -394,17 +390,15 @@
             items = list(other)
 
         if kwargs:
             items += list(kwargs.items())
 
         if replace:
             replaced = {k for k, v in items if k in self._dict}
-            self._order = [
-                (k, v) for (k, v) in self._order if k not in replaced
-            ]
+            self._order = [(k, v) for (k, v) in self._order if k not in replaced]
             for key in replaced:
                 self._dict[key] = []
 
         for k, v in items:
             self._dict.setdefault(k, []).append(v)
             self._order.append((k, v))
```

### Comparing `fresco-3.1.0/fresco/options.py` & `fresco-3.2.0/fresco/options.py`

 * *Files identical despite different names*

### Comparing `fresco-3.1.0/fresco/request.py` & `fresco-3.2.0/fresco/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,24 +19,24 @@
 The :class:`Request` class models an incoming HTTP request, allowing access to
 HTTP headers and request data (eg query string or submitted form data).
 """
 from urllib.parse import ParseResult
 from urllib.parse import quote
 from urllib.parse import urlparse
 from urllib.parse import urlunparse
-from typing import Dict
-from typing import Optional
+import typing as t
 import datetime
 import json
 import posixpath
 import re
 
 from fresco import exceptions
 from fresco.cookie import parse_cookie_header
 from fresco.multidict import MultiDict
+from fresco.types import QuerySpec
 from fresco.util.http import FileUpload
 from fresco.util.http import get_body_bytes
 from fresco.util.http import get_content_type_info
 from fresco.util.http import parse_post
 from fresco.util.http import parse_querystring
 from fresco.util.urls import normpath
 from fresco.util.urls import make_query
@@ -79,28 +79,32 @@
     STATE_ENV_KEY = "fresco._request_state"
 
     #: WSGI key for the session variable. The default value is configured for
     #: use with `beaker <http://beaker.groovie.org/>`_
     SESSION_ENV_KEY = "beaker.session"
 
     #: The WSGI environ dict
-    environ: Dict
+    environ: t.Dict
 
     #: Encoding used to decode WSGI parameters, notably PATH_INFO and form data
     default_charset = fresco.DEFAULT_CHARSET
 
     #: The decoder class to use for JSON request payloads
     json_decoder_class = json.JSONDecoder
 
+    #: List of functions to be called at the end of this request's lifecycle
+    teardown_handlers: t.List[t.Callable]
+
     def __init__(self, environ):
         if self.STATE_ENV_KEY in environ:
             self.__dict__ = environ[self.STATE_ENV_KEY]
         else:
             environ[self.STATE_ENV_KEY] = self.__dict__
-        self.environ = environ
+            self.environ = environ
+            self.teardown_handlers = []
 
     def __str__(self):
         """
         Return a useful text representation of the request
         """
         return "<%s %s %s>" % (self.__class__.__name__, self.method, self.url)
 
@@ -130,24 +134,25 @@
 
         This will return the ``POST`` or ``PUT`` data when available, otherwise
         querystring (``GET``)  data. Querystring data is always available via
         the ``query`` property.
         """
         if self._form is None:
             if self.environ["REQUEST_METHOD"] in ("PUT", "POST"):
-                self._form = MultiDict(
-                    parse_post(
-                        self.environ,
-                        self.environ["wsgi.input"],
-                        self.charset,
-                        self.MAX_SIZE,
-                        self.MAX_MULTIPART_SIZE,
-                        ie_workaround=self.IE_CONTENT_DISPOSITION_WORKAROUND,
-                    )
+                items, close = parse_post(
+                    self.environ,
+                    self.environ["wsgi.input"],
+                    self.charset,
+                    self.MAX_SIZE,
+                    self.MAX_MULTIPART_SIZE,
+                    ie_workaround=self.IE_CONTENT_DISPOSITION_WORKAROUND,
                 )
+                if close:
+                    self.teardown_handlers.append(close)
+                self._form = MultiDict(items)
             else:
                 data = environ_to_str(self.environ.get("QUERY_STRING", ""))
                 self._form = MultiDict(parse_querystring(data, self.charset))
         return self._form
 
     @property
     def content_type_encoding(self):
@@ -466,15 +471,15 @@
         """
         try:
             return environ_to_str(self.environ["SCRIPT_NAME"], self.charset)
         except UnicodeDecodeError:
             raise exceptions.BadRequest
 
     @property
-    def query_string(self) -> Optional[str]:
+    def query_string(self) -> t.Optional[str]:
         """
         The QUERY_STRING value as a unicode string
         """
         return self.environ.get("QUERY_STRING")
 
     @property
     def referrer(self):
@@ -518,41 +523,41 @@
         """
         Return ``True`` if the request is served over a secure connection.
         """
         return self.environ["wsgi.url_scheme"] == "https"
 
     def make_url(
         self,
-        scheme=None,
-        netloc=None,
-        path=None,
-        parameters=None,
-        query=None,
-        query_add=None,
-        query_replace=None,
-        fragment=None,
-        SCRIPT_NAME=None,
-        PATH_INFO=None,
+        scheme: t.Optional[str] = None,
+        netloc: t.Optional[str] = None,
+        path: t.Optional[str] = None,
+        parameters: t.Optional[str] = None,
+        query: t.Union[None, str, QuerySpec] = None,
+        query_add: t.Union[None, str, QuerySpec] = None,
+        query_replace: t.Union[None, str, QuerySpec] = None,
+        fragment: t.Optional[str] = None,
+        SCRIPT_NAME: t.Optional[str] = None,
+        PATH_INFO: t.Optional[str] = None,
         **kwargs,
-    ):
-        r"""\
+    ) -> str:
+        r"""
         Make a new URL based on the current URL, replacing any of the six
         URL elements (scheme, netloc, path, parameters, query or fragment). The
         current request's query string is not included in the generated URL
         unless you explicitly pass it in.
 
         :param scheme:      The URL scheme, eg ``http`` or ``https``
         :param netloc:      The netloc portion of the URL, eg 'example.com:80'
         :param path:        The path portion of the URL, eg '/my/page.html'
         :param parameters:  RFC2396 path parameters (see also the stdlib
                             urlparse module)
         :param fragment:    The URL fragment
         :param query:       Query data, as a list of tuples, a dict or a string.
-                            Any query parameters present in the current url
-                            will be removed.
+                            If supplied, any query parameters present in the
+                            current request's url will be removed.
         :param query_add:   Query parameters to add. If the current url already
                             contains query parameters with the same name, these
                             will be supplemented with the new values.
         :param query_replace: Query parameters to replace. If the current url
                               already contains query parameters with the same
                               name, these will be replaced with the new values.
         :param PATH_INFO:   The PATH_INFO portion of the path. Overrides
@@ -631,14 +636,15 @@
         values in an existing query string. If either of these is specified
         then the current request's query string (or value of ``query``, if
         specified) will be extended with the given values.
         These arguments take a dict, a list of ``(key, value)`` tuples, or any
         other type convertable to a MultiDict.
         """
         parsed_url = self.parsed_url
+        querystr: t.Optional[str] = None
 
         if path is not None:
             path = quote(path, encoding=self.charset)
 
             if path[0] != "/":
                 path = posixpath.join(posixpath.dirname(parsed_url[2]), path)
                 path = posixpath.normpath(path)
@@ -672,25 +678,28 @@
 
             if query_replace is not None:
                 query_dict.update(query_replace)
 
             if kwargs:
                 query_dict.update(kwargs)
 
-            query = make_query(query_dict)
+            querystr = make_query(query_dict)
 
-        elif query is not None and not isinstance(query, str):
-            query = make_query(query)
+        elif query is not None:
+            if isinstance(query, str):
+                querystr = query
+            else:
+                querystr = make_query(query)
 
         url = (
             scheme if scheme is not None else parsed_url[0],
             netloc if netloc is not None else parsed_url[1],
             path if path is not None else parsed_url[2],
             parameters if parameters is not None else parsed_url[3],
-            query,
+            querystr,
             fragment,
         )
 
         return urlunparse(url)
 
     def resolve_url(self, url, relative="app"):
         """
```

### Comparing `fresco-3.1.0/fresco/requestcontext.py` & `fresco-3.2.0/fresco/requestcontext.py`

 * *Files identical despite different names*

### Comparing `fresco-3.1.0/fresco/response.py` & `fresco-3.2.0/fresco/response.py`

 * *Files 2% similar despite different names*

```diff
@@ -338,15 +338,15 @@
         status=None,
         headers=None,
         onclose=None,
         _nocontent=[],
         passthrough=False,
         content_iterator=None,
         make_headers=make_headers,
-        **kwargs
+        **kwargs,
     ):
         """
         Create a new Response object, modelling the HTTP status, headers and
         content of an HTTP response. Response instances are valid WSGI
         applications.
 
         :param content: The response content as an iterable object
@@ -402,31 +402,28 @@
         if headers or kwargs:
             headers = make_headers(headers, kwargs)
 
         # Ensure a content-type header is set if a content iterator has been
         # provided
         if content is not _nocontent:
             if not any(k == "Content-Type" for k, v in headers):
-                headers = [
-                    ("Content-Type", self.default_content_type)
-                ] + headers
+                headers = [("Content-Type", self.default_content_type)] + headers
 
         self.headers = headers
 
         # Now we've dealt with the headers (including Content-Type,
         # which the charset property will look for when deciding how to
         # encode strings) we can pull the content into an iterable.
         # We optimize for the common cases (byte string, unicode string,
         # list of byte strings, list of unicode strings), otherwise
         # we wrap the iterator in :func:`encoder`, which iterates the content
         # and tries to encode each item as a byte string. Note that this
         # code assumes that lists are homogeneous.
         self.content = content
         if content_iterator:
-            self.content = content
             self.content_iterator = content_iterator
         elif passthrough or content is _nocontent:
             self.content_iterator = content
         else:
             content_islist = isinstance(content, list)
             if content_islist:
                 if len(content) == 0:
@@ -438,17 +435,15 @@
                     self.content_iterator = (c.encode(charset) for c in content)
 
             elif isinstance(content, bytes):
                 self.content_iterator = [content]
             elif isinstance(content, str):
                 self.content_iterator = [content.encode(self.charset)]
             else:
-                self.content_iterator = _copy_close(
-                    content, encoder(content, self.charset)
-                )
+                self.content_iterator = encoder(content, self.charset)
 
     def __call__(self, environ, start_response, exc_info=None):
         """
         WSGI callable. Calls ``start_response`` with assigned headers and
         returns an iterator over ``content``.
         """
         start_response(self.status, self.headers, exc_info)
@@ -459,67 +454,68 @@
 
     def add_onclose(self, *funcs):
         """
         Add functions to be called as part of the response iterator's ``close``
         method.
         """
         return self.__class__(
-            self.content, self.status, self.headers, self.onclose + list(funcs)
+            self.content,
+            self.status,
+            self.headers,
+            self.onclose + list(funcs),
+            content_iterator=self.content_iterator,
         )
 
     @classmethod
     def from_wsgi(cls, wsgi_callable, environ, start_response):
         """
         Return a ``Response`` object constructed from the result of calling
         ``wsgi_callable`` with the given ``environ`` and ``start_response``
         arguments.
         """
         responder = StartResponseWrapper(start_response)
         content = wsgi_callable(environ, responder)
+        close = getattr(content, "close", None)
         if responder.buf.tell():
-            content = _copy_close(
-                content, chain(content, [responder.buf.getvalue()])
-            )
+            content = chain(content, [responder.buf.getvalue()])
 
         if not responder.called:
             # Iterator has not called start_response yet. Call next(content)
             # to force the application to call start_response
             try:
                 chunk = next(content)
             except StopIteration:
                 pass
             except Exception:
-                close = getattr(content, "close", None)
                 if close is not None:
                     close()
                 raise
             else:
-                content = _copy_close(content, chain([chunk], content))
+                content = chain([chunk], content)
         return cls(
             content,
             responder.status,
             headers=responder.headers,
             passthrough=True,
+            onclose=[close] if close is not None else [],
         )
 
     def get_headers(self, name):
         """\
         Return the list of headers set with the given name.
 
         Synopsis::
 
             >>> r = Response(set_cookie = ['cookie1', 'cookie2'])
             >>> r.get_headers('set-cookie')
             ['cookie1', 'cookie2']
 
         """
         return [
-            value
-            for header, value in self.headers
-            if header.lower() == name.lower()
+            value for header, value in self.headers if header.lower() == name.lower()
         ]
 
     def get_header(self, name, default=""):
         """\
         Return the concatenated values of the named header(s) or ``default`` if
         the header has not been set.
 
@@ -568,17 +564,15 @@
 
             >>> r = Response(content_type='text/plain')
             >>> r.headers
             [('Content-Type', 'text/plain')]
             >>> r.add_header('Cache-Control', 'no-cache').headers
             [('Content-Type', 'text/plain'), ('Cache-Control', 'no-cache')]
         """
-        return self.replace(
-            headers=(self.headers + [(make_header_name(name), value)])
-        )
+        return self.replace(headers=(self.headers + [(make_header_name(name), value)]))
 
     def add_headers(self, headers=[], **kwheaders):
         """\
         Return a new response object with the given additional headers.
 
         Synopsis::
 
@@ -586,17 +580,15 @@
             >>> r.headers
             [('Content-Type', 'text/plain')]
             >>> r.add_headers(
             ...     cache_control='no-cache',
             ... ).headers
             [('Content-Type', 'text/plain'), ('Cache-Control', 'no-cache')]
         """
-        return self.replace(
-            headers=make_headers(self.headers + headers, kwheaders)
-        )
+        return self.replace(headers=make_headers(self.headers + headers, kwheaders))
 
     def remove_headers(self, *headers):
         """\
         Return a new response object with the named headers removed.
 
         Synopsis::
 
@@ -676,17 +668,15 @@
         _vary_on: Set[str] = set(vary_on)
         newheaders = []
         for k, v in self.headers:
             if k.lower() == "vary":
                 _vary_on.update(s.strip() for s in v.split(","))
             else:
                 newheaders.append((k, v))
-        return self.replace(
-            headers=newheaders + [("Vary", ", ".join(_vary_on))]
-        )
+        return self.replace(headers=newheaders + [("Vary", ", ".join(_vary_on))])
 
     def replace(self, content=None, status=None, headers=None, **kwheaders):
         """\
         Return a new response object with any of content, status or headers
         changed.
 
         Synopsis::
@@ -713,17 +703,17 @@
             headers = self.headers
 
         if status is None:
             status = self.status
 
         if kwheaders:
             toremove = {make_header_name(k) for k in kwheaders}
-            headers = [
-                (k, v) for k, v in headers if k not in toremove
-            ] + make_headers([], kwheaders)
+            headers = [(k, v) for k, v in headers if k not in toremove] + make_headers(
+                [], kwheaders
+            )
 
         return self.__class__(
             content,
             status,
             headers,
             onclose=onclose,
             content_iterator=content_iterator,
@@ -817,15 +807,15 @@
         return cls(
             "<html>\n"
             "<body>\n"
             "<h1>401 Authorization Required</h1>\n"
             "</body>\n"
             "</html>",
             status=STATUS_UNAUTHORIZED,
-            www_authenticate=authenticate
+            www_authenticate=authenticate,
         )
 
     @classmethod
     def unauthorized_basic(cls, realm):
         """
         Return an HTTP unauthorized response (401) with a WWW-Authenticate
         header set for HTTP Basic authentication..
@@ -840,19 +830,15 @@
         Synopsis::
 
             >>> def view():
             ...     return Response.forbidden()
             ...
         """
         return cls(
-            "<html>\n"
-            "<body>\n"
-            "<h1>%s</h1>\n"
-            "</body>\n"
-            "</html>" % (message,),
+            "<html>\n<body>\n<h1>%s</h1>\n</body>\n</html>" % (message,),
             status=STATUS_FORBIDDEN,
         )
 
     @classmethod
     def bad_request(cls, request=None):
         """\
         Return an HTTP bad request response.
@@ -904,21 +890,15 @@
         Return an HTTP Payload Too Large response (413)::
 
             >>> response = Response.payload_too_large()
 
         """
         return cls(
             status=STATUS_PAYLOAD_TOO_LARGE,
-            content=[
-                "<html>"
-                "<body>"
-                "<h1>Payload Too Large</h1>"
-                "</body>"
-                "</html>"
-            ],
+            content=["<html><body><h1>Payload Too Large</h1></body></html>"],
         )
 
     request_entity_too_large = payload_too_large
 
     @classmethod
     def method_not_allowed(cls, valid_methods):
         """\
@@ -934,21 +914,15 @@
 
         :return: A :class:`fresco.response.Response` instance
         """
 
         return cls(
             status=STATUS_METHOD_NOT_ALLOWED,
             allow=",".join(valid_methods),
-            content=[
-                "<html>"
-                "<body>"
-                "<h1>Method not allowed</h1>"
-                "</body>"
-                "</html>"
-            ],
+            content=["<html><body><h1>Method not allowed</h1></body></html>"],
         )
 
     @classmethod
     def internal_server_error(cls):
         """\
         Return an HTTP internal server error response (500).
 
@@ -959,21 +933,15 @@
             ...
 
         :return: A :class:`fresco.response.Response` instance
         """
 
         return cls(
             status=STATUS_INTERNAL_SERVER_ERROR,
-            content=[
-                "<html>"
-                "<body>"
-                "<h1>Internal Server Error</h1>"
-                "</body>"
-                "</html>"
-            ],
+            content=["<html><body><h1>Internal Server Error</h1></body></html>"],
         )
 
     @classmethod
     def unrestricted_redirect(
         cls, location, request=None, status=STATUS_FOUND, **kwargs
     ):
         """\
@@ -1072,15 +1040,15 @@
     def redirect(
         cls,
         url,
         fallback=None,
         status=STATUS_FOUND,
         _is_safe_url=is_safe_url,
         allowed_hosts=frozenset(),
-        **kwargs
+        **kwargs,
     ):
         """
         Return an HTTP redirect reponse (30x). Will only redirect to the
         current host or hosts in the ``allowed_hosts`` list. A ``ValueError``
         will be raised if the URL is not permitted and no fallback is
         specified.
 
@@ -1100,17 +1068,15 @@
 
         The location argument is interpreted as for
         :meth:`~fresco.response.Response.unrestricted_redirect`
         """
         # Create the fallback redirect response always so that
         # changes to route names don't result in latent bugs
         if fallback:
-            fallback = Response.unrestricted_redirect(
-                fallback, status=status, **kwargs
-            )
+            fallback = Response.unrestricted_redirect(fallback, status=status, **kwargs)
         if callable(url) or "//" not in url:
             return cls.unrestricted_redirect(url, status=status, **kwargs)
 
         if url and _is_safe_url(url, allowed_hosts):
             return cls.unrestricted_redirect(url, status=status, **kwargs)
         if fallback:
             return fallback
@@ -1177,15 +1143,15 @@
         data,
         indent=None,
         separators=(",", ":"),
         content_type="application/json",
         status=None,
         headers=None,
         dumps=stdlib_json.dumps,
-        **kwargs
+        **kwargs,
     ):
         """
         Return an ``application/json`` response with the given data
         JSON serialized
 
         :param data: The data to json encode.
         :param indent: The indent level.
@@ -1220,28 +1186,7 @@
         output.append(line_break)
     output.append(line_break)
     output.extend(r.content_iterator)
     s = b"".join(output)
     if encoding:
         return s.decode(encoding)
     return s
-
-
-def _copy_close(src, dst, marker=object()):
-    """\
-    Copy the ``close`` attribute from ``src`` to ``dst``, which are assumed to
-    be iterators.
-
-    If it is not possible to copy the attribute over (eg for
-    ``itertools.chain``, which does not support the close attribute) an
-    instance of ``ClosingIterator`` is returned which will proxy calls to
-    ``close`` as necessary.
-    """
-
-    close = getattr(src, "close", marker)
-    if close is not marker:
-        try:
-            setattr(dst, "close", close)
-        except AttributeError:
-            return ClosingIterator(dst, close)
-
-    return dst
```

### Comparing `fresco-3.1.0/fresco/routeargs.py` & `fresco-3.2.0/fresco/routeargs.py`

 * *Files identical despite different names*

### Comparing `fresco-3.1.0/fresco/routing.py` & `fresco-3.2.0/fresco/routing.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,22 +21,21 @@
 from collections.abc import MutableSequence
 from importlib import import_module
 from functools import partial
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import List
-from typing import Iterator
-from typing import Iterable
 from typing import Mapping
 from typing import Optional
 from typing import Union
 from typing import Set
 from typing import Tuple
 from weakref import WeakKeyDictionary
+import typing as t
 
 from fresco.exceptions import ResponseException
 from fresco.response import Response
 from fresco.request import Request
 from fresco.requestcontext import context
 from fresco.routeargs import RouteArg
 from fresco.util.cache import make_cache
@@ -238,14 +237,16 @@
     should return ``None``.
 
     Pattern objects may also be able to take a tuple of
     ``(positional_arguments, keyword_arguments)`` and return a corresponding
     URL path.
     """
 
+    segments: t.List["PatternSegment"]
+
     def match(self, path):
         """
         Should return a tuple of ``(positional_arguments, keyword_arguments)``
         if the pattern matches the given URL path, or None if it does not
         match.
         """
         raise NotImplementedError
@@ -679,28 +680,27 @@
     )
 
     #: Always provide an positional ``request`` argument to views
     provide_request = False
 
     def __init__(
         self,
-        pattern,
+        pattern: t.Union[str, Pattern],
         methods=None,
         view=None,
         kwargs=None,
         args=None,
         name=None,
         predicate=None,
         decorators=None,
         filters=None,
         fallthrough_on=None,
         provide_request: Optional[bool] = None,
         **_kwargs,
     ):
-
         """
         :param pattern:     A string that can be compiled into a path pattern
         :param methods:     The list of HTTP methods the view is bound to
                             ('GET', 'POST', etc)
         :param view:        The view function.
         :param kwargs:      A dictionary of default keyword arguments to pass
                             to the view callable
@@ -768,15 +768,15 @@
         """
         method_view_map: Dict[str, Callable] = {}
         if methods:
             if isinstance(methods, str):
                 methods = [methods]
             else:
                 # Catch the common error of not providing a valid method
-                if not isinstance(methods, Iterable):
+                if not isinstance(methods, t.Iterable):
                     raise TypeError(
                         "HTTP methods must be specified as a string or iterable"
                     )
             for m in methods:
                 if m not in ALL_METHODS:
                     raise ValueError("{!r} is not a valid HTTP method".format(m))
             method_view_map.update((m, view) for m in methods)
@@ -1183,15 +1183,15 @@
                 if isinstance(item, Route):
                     self.add_route(item)
                 elif hasattr(item, "__routes__"):
                     for r in item.__routes__:
                         if r.instance is None:
                             r = r.bindto(item)
                         self.add_route(r)
-                elif isinstance(item, Iterable):
+                elif isinstance(item, t.Iterable):
                     for r in item:
                         self.add_route(r)
                 else:
                     raise TypeError(item)
         if cache:
             self.reinit_route_cache()
 
@@ -1203,15 +1203,15 @@
             for item in other:
                 result.add_route(item)
         return result
 
     def __radd__(self, other):
         if isinstance(other, Route):
             return RouteCollection([other]) + self
-        elif isinstance(other, Iterable):
+        elif isinstance(other, t.Iterable):
             return RouteCollection(other) + self
         raise TypeError("Cannot add %r to %r" % (other, self))
 
     def __iter__(self):
         return iter(self.__routes__)
 
     def __getitem__(self, index):
@@ -1241,15 +1241,14 @@
 
     def insert(self, position, item):
         self.__routes__.insert(position, item)
         if self._route_cache is not None:
             self.reinit_route_cache()
 
     def add_route(self, route):
-
         self.__routes__.append(route)
         if self._route_cache is not None:
             self.reinit_route_cache()
 
     def add_prefix(self, prefix):
         """
         Return a copy of the RouteCollection with the given path prepended to
@@ -1362,15 +1361,15 @@
     def _get_routes(self, key):
         method, path = key
         routes = ((r, r.match(path, method)) for r in self.__routes__)
         return [(r, t) for (r, t) in routes if t is not None]
 
     def get_route_traversals(
         self, path: str, method: Optional[str], request: Optional[Request] = None
-    ) -> Iterator[RouteTraversal]:
+    ) -> t.Iterator[RouteTraversal]:
         """
         Generate RouteTraversals for routes matching the given path and
         method::
 
             for rt in routecollection.get_route_traversals('/foo/bar', GET):
                 print("Route is", rt.route)
                 print("Arguments extracted from the path:", rt.args, rt.kwargs)
@@ -1478,105 +1477,144 @@
                             traversal_kwargs,
                         )
                     ],
                 )
 
     def get_routes(
         self, path: str, method: str, request: Optional[Request] = None
-    ) -> Iterable[RouteTraversal]:
+    ) -> t.Iterable[RouteTraversal]:
         warnings.warn(
             "RouteCollection.get_routes is deprecated and will be removed "
             "in a future version. Use get_route_traversals instead",
             DeprecationWarning,
         )
         return self.get_route_traversals(path, method, request)
 
-    def route(self, pattern, methods=None, view=None, *args, **kwargs):
+    def route(
+        self,
+        pattern: t.Union[str, Pattern],
+        methods: t.Optional[t.Union[str, t.Iterable[str]]] = None,
+        view: t.Optional[t.Union[str, t.Callable]] = None,
+        *args,
+        route_class: t.Optional[t.Type[Route]] = None,
+        **kwargs,
+    ):
         """
         Match a URL pattern to a view function. Can be used as a function
         decorator, in which case the ``view`` parameter should not be passed.
 
         :param pattern: A string that can be compiled into a path pattern
         :param methods: A list of HTTP methods the view is bound to
         :param view:    The view function. If not specified a function
                         decorator will be returned.
 
         Other parameters are as for the :class:`Route` constructor.
         """
         # Catch the common error of not providing a valid method
-        if methods and not isinstance(methods, Iterable):
+        if methods and not isinstance(methods, t.Iterable):
             raise TypeError("HTTP methods must be specified as a string or iterable")
 
         # Called as a decorator?
         if methods is not None and view is None:
 
             def route_decorator(func):
                 self.add_route(
                     self.route_class(pattern, methods, func, *args, **kwargs)
                 )
                 return func
 
             return route_decorator
 
-        route = self.route_class(pattern, methods, view, *args, **kwargs)
+        cls = route_class if route_class is not None else self.route_class
+        route = cls(pattern, methods, view, *args, **kwargs)
         self.add_route(route)
         return route
 
-    def route_wsgi(self, path, wsgiapp, rewrite_script_name=True, *args, **kwargs):
+    def route_wsgi(
+        self,
+        path: str,
+        wsgiapp: t.Union[t.Callable, str],
+        rewrite_script_name: bool = True,
+        *args,
+        **kwargs,
+    ):
         """
         Route requests to ``path`` to the given WSGI application
 
         :param path: the mount point for the app
-        :param wsgiapp: the WSGI callable
+        :param wsgiapp: the WSGI callable, or the path to a callable in the
+                        format ``myapp.module.do_wsgi``.
         :param rewrite_script_name: if ``True`` (the default),
                                     the mount point specified by ``path`` will
                                     be shifted off ``PATH_INFO`` and into the
                                     ``SCRIPT_NAME`` environ key.
         """
 
         def fake_start_response(status, headers, exc_info=None):
             return None
 
         if path.encode("ascii", "ignore").decode("ascii") == path:
             ws_path = path
         else:
             ws_path = None
 
+        resolved_wsgi_app = None
+
         def fresco_wsgi_view(
+            request,
             path=path,
             ws_path=ws_path,
-            context=context,
             rewrite_script_name=rewrite_script_name,
             fake_start_response=fake_start_response,
             make_response=Response.from_wsgi,
-            wsgiapp=wsgiapp,
         ):
-            request = context.request
+            nonlocal resolved_wsgi_app
             environ = request.environ
             ws_SCRIPT_NAME = environ["SCRIPT_NAME"]
             shift_script_name = rewrite_script_name and not (
                 path == "/" and ws_SCRIPT_NAME == ""
             )
             if shift_script_name:
                 if ws_path is None:
                     ws_path = path.encode(request.charset).decode("ISO-8859-1")
                 environ = environ.copy()
                 environ["SCRIPT_NAME"] = ws_SCRIPT_NAME + ws_path
                 environ["PATH_INFO"] = environ["PATH_INFO"][len(ws_path) :]
-            return make_response(wsgiapp, environ, fake_start_response)
 
-        return self.route_all(path, ALL_METHODS, fresco_wsgi_view, *args, **kwargs)
+            if resolved_wsgi_app is None:
+                if isinstance(wsgiapp, str):
+                    if "." in wsgiapp:
+                        mod_name, attr_name = wsgiapp.rsplit(".", 1)
+                        mod = import_module(mod_name)
+                        resolved_wsgi_app = getattr(mod, attr_name)
+                else:
+                    resolved_wsgi_app = wsgiapp
 
-    def route_all(self, path, *args, **kwargs):
-        """\
+            return make_response(resolved_wsgi_app, environ, fake_start_response)
+
+        return self.route_all(
+            path, ALL_METHODS, fresco_wsgi_view, route_class=RRoute, *args, **kwargs
+        )
+
+    def route_all(
+        self, path, methods=None, view=None, *args, route_class=None, **kwargs
+    ):
+        """
         Expose a view for all URLs starting with ``path``.
 
         :param path: the path prefix at which the view will be routed
         """
-        return self.route(MatchAllURLsPattern(path), *args, **kwargs)
+        return self.route(
+            MatchAllURLsPattern(path),
+            methods,
+            view,
+            route_class=route_class,
+            *args,
+            **kwargs,
+        )
 
     def include(self, path, views, fallthrough_on=None):
         """
         Include a view collection at the given path.
 
         The included view collection's url properties will be modified to
         generate the prefixed URLs.
```

### Comparing `fresco-3.1.0/fresco/static.py` & `fresco-3.2.0/fresco/static.py`

 * *Files identical despite different names*

### Comparing `fresco-3.1.0/fresco/subrequests.py` & `fresco-3.2.0/fresco/subrequests.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from itertools import chain
 from typing import Any
 from typing import Dict
 from typing import Tuple
 
 from fresco.core import context
 from fresco.request import Request
+from fresco.response import Response
 from fresco.routing import Route
 from fresco.routing import GET
 from fresco.routing import RouteArg
 from fresco.util.http import parse_header
+from fresco.util.wsgi import make_environ
 
 __all__ = ["subrequest", "subrequest_raw", "subrequest_bytes"]
 
 
 class Markup(str):
     def __html__(self):
         return self
@@ -98,78 +100,87 @@
     :param _env: Additional keys to merge into the subrequest's environ
                  (may only be used when ``_full`` is True)
 
     :param args: Additional positional arguments
 
     :param kwargs: Additional keyword arguments
     """
+    mode = kwargs.pop("_mode", "str")
+    if mode == "str":
+        return subrequest_str(view, *args, **kwargs)
+    elif mode == "bytes":
+        return subrequest_bytes(view, *args, **kwargs)
+    elif mode == "raw":
+        return subrequest_raw(view, *args, **kwargs)
+    else:
+        raise ValueError("Mode must be one of 'str', 'bytes', or 'raw'")
+
+
+def subrequest_str(view, *args, **kwargs) -> str:
+    """
+    Perform a subrequest and return the response content as a string.
+    See :func:`~fresco.subrequests.subrequest` for details
+    """
+    return response_to_str(subrequest_raw(view, *args, **kwargs))
+
+
+def subrequest_bytes(view, *args, **kwargs) -> bytes:
+    """
+    Perform a subrequest and return the response content as a byte string.
+    See :func:`~fresco.subrequests.subrequest` for details
+    """
+    return response_to_bytes(subrequest_raw(view, *args, **kwargs))
+
+
+def subrequest_raw(view, *args, **kwargs) -> Response:
+    """
+    Perform a subrequest and return the raw response object.
+    See :func:`~fresco.subrequests.subrequest` for details
+    """
 
     current_request = context.request
+    response = None
     full = kwargs.pop("_full", False)
     resolve = kwargs.pop("_resolve", False)
-    mode = kwargs.pop("_mode", "str")
     _env = kwargs.pop("_env", {})
     environ = current_request.environ.copy()
     del environ["PATH_INFO"]
     if "QUERY_STRING" in environ:
         del environ["QUERY_STRING"]
 
-    if full or (isinstance(view, str) and "/" in view):
-        del environ[current_request.STATE_ENV_KEY]
-        app = context.app
-        if full:
-            path = app.urlfor(view, *args, **kwargs)
-        else:
-            path = view
-        with app.requestcontext(path, environ) as c:
-            c.is_subrequest = True
+    app = context.app
+    context.push(**dict(context.currentcontext(), is_subrequest=True))
+    try:
+        if full or (isinstance(view, str) and "/" in view):
+            del environ[current_request.STATE_ENV_KEY]
+            if full:
+                path = app.urlfor(view, *args, **kwargs)
+            else:
+                path = view
+            environ = make_environ(path, environ, b"")
             if _env:
-                c.request.environ.update(_env)
-            response = app.view()
-
-    else:
-        assert not _env, "Use of _env invalid without _full"
-        context.push(**dict(context.currentcontext(), is_subrequest=True))
-        try:
+                environ.update(_env)
+            request = app.request_class(environ)
+            context["request"] = request
+            response = app.view(request)
+        else:
+            assert not _env, "Use of _env invalid without _full"
             if not callable(view) or resolve:
                 view, routed_args, routed_kwargs = resolve_viewspec(
                     view, *args, **kwargs
                 )
 
                 # Use args/kwargs extracted during route traversal,
                 args, kwargs = routed_args, routed_kwargs
 
             response = view(*args, **kwargs)
-        finally:
-            context.pop()
 
-    if mode == "str":
-        return response_to_str(response)
-    elif mode == "bytes":
-        return response_to_bytes(response)
-    elif mode == "raw":
         return response
-    else:
-        raise ValueError("Mode must be one of 'str', 'bytes', or 'raw'")
-
-
-def subrequest_bytes(*args, **kwargs):
-    """
-    Perform a subrequest and return the response content as a byte string.
-    See :func:`~fresco.subrequests.subrequest` for details
-    """
-    return subrequest(_mode="bytes", *args, **kwargs)
-
-
-def subrequest_raw(*args, **kwargs):
-    """
-    Perform a subrequest and return the raw response object.
-    See :func:`~fresco.subrequests.subrequest` for details
-    """
-    return subrequest(_mode="raw", *args, **kwargs)
+    finally:
+        context.pop()
 
 
 def response_to_str(response) -> str:
     ct, params = parse_header(response.get_header("Content-Type"))
     encoding = params.get("charset")
     try:
         # Check for the common case that response.content is already a
@@ -185,29 +196,27 @@
 
         # Anything else: decode the content iterator
         else:
             if not encoding:
                 raise ValueError("No content encoding specified")
             content = b"".join(response.content_iterator).decode(encoding)
     finally:
-        if response.onclose:
-            for f in response.onclose:
-                f()
+        for f in response.onclose:
+            f()
     if ct.startswith("text/html") or "xml" in ct.split(";")[0]:
         return Markup(content)
     return content
 
 
 def response_to_bytes(response):
     try:
         return b"".join(response.content_iterator)
     finally:
-        if response.onclose:
-            for f in response.onclose:
-                f()
+        for f in response.onclose:
+            f()
 
 
 def resolve_viewspec(viewspec, *args, **kwargs):
     """
     :param viewspec: a view name, a reference in the form
                      ``'package.module.viewfunction'``, or the view
                      callable itself.
```

### Comparing `fresco-3.1.0/fresco/tests/fixtures.py` & `fresco-3.2.0/fresco/tests/fixtures.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,7 +55,13 @@
         return Response([])
 
 
 def module_level_function():
     """
     A module level function
     """
+
+
+def wsgi_app(environ, start_response):
+    start_response("200 OK", [("Content-Type", "text/plain")])
+
+    return [b"ok"]
```

### Comparing `fresco-3.1.0/fresco/tests/test_cookie.py` & `fresco-3.2.0/fresco/tests/test_cookie.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,11 +51,9 @@
         """Cookie as both secure and httponly"""
         c = Cookie("key", "value", secure=True, httponly=True)
         assert str(c) == "key=value;Path=/;Secure;HttpOnly;SameSite=Lax"
 
     def test_dates_are_rfc_formatted(self):
         c = Cookie("a", "b", expires=datetime(2001, 1, 1, 12))
         assert "Expires=Mon, 01 Jan 2001 12:00:00 GMT;" in str(c)
-        c = Cookie(
-            "a", "b", expires=datetime(2001, 1, 1, 12, tzinfo=FakeTZInfo())
-        )
+        c = Cookie("a", "b", expires=datetime(2001, 1, 1, 12, tzinfo=FakeTZInfo()))
         assert "Expires=Mon, 01 Jan 2001 11:00:00 GMT;" in str(c)
```

### Comparing `fresco-3.1.0/fresco/tests/test_core.py` & `fresco-3.2.0/fresco/tests/test_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 
 class CustomException(Exception):
     pass
 
 
 class TestFrescoApp(object):
     def test_route_operates_as_a_decorator(self):
-
         app = FrescoApp()
 
         @app.route("/", GET)
         def view():
             return Response([b"ok"])
 
         with app.requestcontext("/"):
@@ -84,15 +83,14 @@
         with app.requestcontext("/post", REQUEST_METHOD="GET"):
             assert app.view().status_code == 405
 
         with app.requestcontext("/post", REQUEST_METHOD="POST"):
             assert app.view().status_code == 200
 
     def test_HEAD_request_delegated_to_GET_view(self):
-
         app = FrescoApp()
 
         @app.route("/", GET)
         def view():
             return Response([], x_original_view="GET")
 
         with app.requestcontext("/", REQUEST_METHOD="HEAD"):
@@ -151,94 +149,80 @@
         with app.requestcontext("/f/bar"):
             assert list(app.view().content_iterator) == [b"foo"]
 
         with app.requestcontext("/b/bar"):
             assert list(app.view().content_iterator) == [b"bar"]
 
     def test_wsgi_app_handles_response_exceptions(self):
-
         from fresco.exceptions import NotFound
 
         def view():
             raise NotFound()
 
         app = FrescoApp()
         app.route("/", GET, view)
 
         with app.requestcontext("/"):
             assert app.view().status_code == 404
 
     def test_route_wsgi_app(self):
         def wsgiapp(environ, start_response):
-
-            start_response(
-                "200 OK", [("Content-Type", "application/x-pachyderm")]
-            )
+            start_response("200 OK", [("Content-Type", "application/x-pachyderm")])
             return [b"pretty pink elephants"]
 
         app = FrescoApp()
         app.route_wsgi("/", wsgiapp)
 
         with app.requestcontext("/"):
-            assert list(app.view().content_iterator) == [
-                b"pretty pink elephants"
-            ]
-            assert (
-                app.view().get_header("Content-Type")
-                == "application/x-pachyderm"
-            )
+            assert list(app.view().content_iterator) == [b"pretty pink elephants"]
+            assert app.view().get_header("Content-Type") == "application/x-pachyderm"
 
     def test_get_methods_matches_on_path(self):
-
         app = FrescoApp()
         app.route("/1", POST, lambda: None)
         app.route("/1", PUT, lambda: None)
         app.route("/2", GET, lambda: None)
         app.route("/2", DELETE, lambda: None)
 
         with app.requestcontext() as c:
             assert app.get_methods(c.request, "/1") == set([POST, PUT])
 
         with app.requestcontext() as c:
             assert app.get_methods(c.request, "/2") == set([GET, DELETE])
 
     def test_get_methods_matches_on_predicate(self):
-
         p1 = Mock(return_value=True)
         p2 = Mock(return_value=False)
 
         app = FrescoApp()
         app.route("/", POST, lambda: None, predicate=p1)
         app.route("/", PUT, lambda: None, predicate=p2)
 
         with app.requestcontext("/") as c:
             assert app.get_methods(c.request, "/") == set([POST])
             assert p1.call_args_list == [call(c.request)]
             assert p2.call_args_list == [call(c.request)]
 
     def test_invalid_path_encoding_triggers_bad_request(self):
         app = FrescoApp()
-        with app.requestcontext(
-            PATH_INFO=fixtures.misquoted_wsgi_unicode_path
-        ):
+        with app.requestcontext(PATH_INFO=fixtures.misquoted_wsgi_unicode_path):
             assert app.view().status_code == 400
 
     def test_remove_middleware(self):
         app = FrescoApp()
         m1 = Mock()
         m2 = Mock()
         app.add_middleware(m1)
         app.add_middleware(m2)
         app.remove_middleware(m1)
         app(create_env(), Mock()).close()
         assert m1.call_count == 0
         assert m2.call_count == 1
 
     def test_insert_middleware(self):
-
         calls = []
 
         def middleware(app, name):
             def middleware(env, start_response):
                 calls.append(name)
                 return app(env, start_response)
 
@@ -254,15 +238,14 @@
             app.view()
 
         # Middleware is called from the outside-in, so the item inserted in
         # position 0 is last to be called
         assert calls == ["mercury", "venus", "earth"]
 
     def test_routing_falls_though_with_fallthrough_on(self):
-
         app = FrescoApp()
         app.route(
             "/",
             GET=lambda: Response(status="204 No Content"),
             fallthrough_on={204},
         )
         app.route("/", GET=lambda: Response(status="200 OK"))
@@ -306,14 +289,30 @@
         def process_request(request):
             return new_response
 
         with app.requestcontext("/"):
             assert app.view() is new_response
             assert view.call_count == 0
 
+    def test_process_request_once_only_called_once(self):
+        app = FrescoApp()
+        view = Mock(return_value=Response())
+        app.route("/", GET, view)
+        new_response = Response()
+
+        @app.process_request_once
+        def process_request(request):
+            return new_response
+
+        with app.requestcontext("/"):
+            assert app.view() is new_response
+            assert view.call_count == 0
+            assert app.view() is not new_response
+            assert view.call_count == 1
+
     def test_process_view_continues_on_none(self):
         app = FrescoApp()
         view = Mock(return_value=Response())
         app.route("/", GET, view)
 
         @app.process_view
         def process_view(request, v, args, kwargs):
@@ -482,39 +481,37 @@
         with app.requestcontext("/") as c:
             iterator = app(c.request.environ, Mock())
             iterator.close()
         with pytest.raises(Exception):
             app.process_teardown(Mock())
 
     def test_exception_in_process_hooks_do_not_stop_processing(self):
-
         for hook, view in [
             ("process_request", Response),
             ("process_view", Response),
             ("process_response", Response),
             ("process_exception", Mock(side_effect=CustomException())),
             ("process_http_error_response", Response.not_found),
             ("process_teardown", Response),
         ]:
             faulty_hook = Mock(side_effect=CustomException())
             process_teardown = Mock(return_value=None)
 
             app = FrescoApp()
-            app.route("/", GET, view)
+            app.route("/", GET, view)  # type: ignore
             getattr(app, hook)(faulty_hook)
             app.process_teardown(process_teardown)
 
             with app.requestcontext("/"):
                 app.view()
 
             assert faulty_hook.call_count == 1, hook
             assert process_teardown.call_count == 1
 
     def test_it_raises_exception_in_route_resolution(self):
-
         from fresco.routing import register_converter, StrConverter
 
         @register_converter("bugs")
         class Converter(StrConverter):
             def from_string(self, s):
                 raise AssertionError("Oops!")
 
@@ -542,15 +539,14 @@
 
         app.route("/", GET, self.exception_view)
         with app.requestcontext("/"):
             with pytest.raises(CustomException):
                 app.view()
 
     def test_it_reraises_if_no_500_error_handler_installed(self):
-
         app = FrescoApp()
         app.process_http_error_response(lambda req, res: None, 404)
 
         app.route("/", GET, self.exception_view)
         with app.requestcontext("/"):
             with pytest.raises(CustomException):
                 app.view()
@@ -662,15 +658,14 @@
             assert process_http_error_response.call_count == 1
             req, res = process_http_error_response.call_args[0]
             assert res.status_code == 500
 
 
 class TestIncludeApp(object):
     def test_it_routes_to_an_included_app(self):
-
         app = FrescoApp()
 
         @app.route("/", GET)
         def view():
             return Response([b"ok"])
 
         app2 = FrescoApp()
@@ -689,17 +684,15 @@
 
         app = FrescoApp()
         app.route("/", GET, view)
         app2 = FrescoApp()
         app2.include("/app1", app)
 
         with app2.requestcontext("/app1/"):
-            assert list(app2.view().content_iterator) == [
-                b"http://localhost/app1/"
-            ]
+            assert list(app2.view().content_iterator) == [b"http://localhost/app1/"]
 
 
 class TestTrailingSlashes(object):
     """\
     The general principle is that if a GET or HEAD request is received for a
     URL without a trailing slash and no match is found, the app will look for a
     URL with a trailing slash, and redirect the client if such a route exists.
@@ -720,37 +713,34 @@
         with app.requestcontext(""):
             assert app.view().status_code == 301
             assert app.view().get_header("location") == "http://localhost/"
 
 
 class TestViewCollection(object):
     def test_appdef(self):
-
         app = FrescoApp()
         app.include("/", fixtures.CBV("bananas!"))
         with app.requestcontext("/"):
             assert list(app.view().content_iterator) == [b"bananas!"]
 
     def test_appdef_url_generation(self):
-
         foo = fixtures.CBV("foo!")
         bar = fixtures.CBV("bar!")
         baz = fixtures.CBV("baz!")
 
         app = FrescoApp(views=foo)
         app.include("/bar", bar)
         app.include("/baz", baz)
 
         with app.requestcontext():
             assert urlfor(foo.index_html) == "http://localhost/"
             assert urlfor(bar.index_html) == "http://localhost/bar/"
             assert urlfor(baz.index_html) == "http://localhost/baz/"
 
     def test_instance_available_in_context(self):
-
         s = []
 
         class MyCBV(fixtures.CBV):
             def index_html(self):
                 from fresco import context
 
                 s.append(context.view_self)
@@ -788,27 +778,25 @@
         def middleware(environ, start_response):
             environ["sausages"] = 1
             return app(environ, start_response)
 
         return middleware
 
     def test_creates_isolated_context(self):
-
         app = FrescoApp()
         with app.requestcontext():
             context.request = "foo"
 
             with app.requestcontext():
                 context.request = "bar"
                 assert context.request == "bar"
 
             assert context.request == "foo"
 
     def test_parses_full_url(self):
-
         with FrescoApp().requestcontext("https://arthur@example.org:123/?x=y"):
             assert context.request.environ["HTTPS"] == "on"
             assert context.request.environ["REMOTE_USER"] == "arthur"
             assert context.request.environ["HTTP_HOST"] == "example.org:123"
             assert context.request.environ["SCRIPT_NAME"] == ""
             assert context.request.environ["PATH_INFO"] == "/"
             assert context.request.environ["QUERY_STRING"] == "x=y"
@@ -844,29 +832,26 @@
     def test_it_converts_wsgi_keys(self):
         # CONTENT_TYPE is both a WSGI core environ key and a standard request
         # header. The WSGI key must win.
         with FrescoApp().requestcontext(content_type="foo"):
             assert context.request.environ["CONTENT_TYPE"] == "foo"
 
     def test_it_invokes_middleware(self):
-
         app = FrescoApp()
         app.add_middleware(self._middleware)
         with app.requestcontext() as c:
             assert "sausages" in c.request.environ
 
     def test_it_skips_middleware(self):
-
         app = FrescoApp()
         app.add_middleware(self._middleware)
         with app.requestcontext(middleware=False) as c:
             assert "sausages" not in c.request.environ
 
     def test_it_closes_middleware(self):
-
         close = Mock()
 
         def middleware(app):
             def middleware(environ, start_response):
                 return ClosingIterator(app(environ, start_response), close)
 
             return middleware
@@ -896,15 +881,14 @@
 
         app = FrescoApp()
         app.add_middleware(middleware)
         with app.requestcontext():
             assert next(counter) == 1
 
     def test_it_calls_late_added_middleware(self):
-
         calls = []
 
         def middleware(app):
             calls.append("middleware initialized")
 
             def middleware(env, start_response):
                 calls.append("middleware called")
@@ -925,15 +909,14 @@
         # middleware included
         with app.requestcontext("/"):
             app.view()
 
         assert calls == ["middleware initialized", "middleware called"]
 
     def test_it_passes_a_valid_start_response_to_middleware(self):
-
         calls = []
 
         def middleware(app):
             def middleware(env, start_response):
                 calls.append("middleware called")
                 write = start_response("200 OK", [])
                 assert callable(write)
@@ -958,18 +941,15 @@
 
         setattr(fixtures, "aliased_view", view)
 
         app = FrescoApp()
         app.route("/", GET, view)
         with app.requestcontext():
             assert urlfor(view) == "http://localhost/"
-            assert (
-                urlfor("fresco.tests.fixtures.aliased_view")
-                == "http://localhost/"
-            )
+            assert urlfor("fresco.tests.fixtures.aliased_view") == "http://localhost/"
 
         delattr(fixtures, "aliased_view")
 
     def test_urlfor_with_view_function(self):
         def view():
             return Response()
 
@@ -981,17 +961,15 @@
     def test_urlfor_allows_script_name(self):
         def view():
             return Response()
 
         app = FrescoApp()
         app.route("/foo", GET, view)
         with app.requestcontext():
-            assert (
-                urlfor(view, _script_name="/abc") == "http://localhost/abc/foo"
-            )
+            assert urlfor(view, _script_name="/abc") == "http://localhost/abc/foo"
 
     def test_urlfor_with_string(self):
         app = FrescoApp()
         app.route("/myviewfunc", GET, fixtures.module_level_function)
         with app.requestcontext():
             assert (
                 urlfor("fresco.tests.fixtures.module_level_function")
@@ -1014,28 +992,25 @@
         app = FrescoApp()
         app.route("/1", GET, myviewfunc)
         app.route("/2", GET, myviewfunc)
         with app.requestcontext():
             assert urlfor(myviewfunc) == "http://localhost/1"
 
     def test_urlfor_with_class_based_view_spec(self):
-
         app = FrescoApp()
         app.include("/foo", fixtures.CBV("x"))
         with app.requestcontext():
             assert (
                 urlfor("fresco.tests.fixtures.CBV.index_html")
                 == "http://localhost/foo/"
             )
 
     def test_it_uses_values_from_path_defaults(self):
         app = FrescoApp()
-        app.route(
-            "/<test:int>", GET, lambda: None, name="test", test_default=1
-        )
+        app.route("/<test:int>", GET, lambda: None, name="test", test_default=1)
         with app.requestcontext():
             assert urlfor("test") == "http://localhost/1"
 
     def test_it_uses_callable_values_from_path_defaults(self):
         generate_value = Mock(return_value=1)
         app = FrescoApp()
         app.route(
@@ -1055,10 +1030,9 @@
 
         app = FrescoApp()
         app.route("/", GET, f)
         with app.requestcontext():
             assert urlfor(f, _query="a=1") == "http://localhost/?a=1"
             assert urlfor(f, _query={"a": "1"}) == "http://localhost/?a=1"
             assert (
-                urlfor(f, _query=[("a", "1"), ("a", 2)])
-                == "http://localhost/?a=1&a=2"
+                urlfor(f, _query=[("a", "1"), ("a", 2)]) == "http://localhost/?a=1&a=2"
             )
```

### Comparing `fresco-3.1.0/fresco/tests/test_decorators.py` & `fresco-3.2.0/fresco/tests/test_decorators.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,17 +14,15 @@
 #
 from fresco.decorators import json_response
 
 
 class TestJSONResponse(object):
     def test_it_allows_custom_formatting(self):
         r = json_response({"l": [1, 2, 3]}, indent=1, separators=(", ", ": "))
-        assert list(r.content_iterator) == [
-            b'{\n "l": [\n  1, \n  2, \n  3\n ]\n}'
-        ]
+        assert list(r.content_iterator) == [b'{\n "l": [\n  1, \n  2, \n  3\n ]\n}']
 
     def test_it_acts_as_a_filter(self):
         r = json_response({"l": [1, 2, 3]})
         assert list(r.content_iterator) == [b'{"l":[1,2,3]}']
         assert r.get_header("content-type") == "application/json"
 
     def test_it_acts_as_a_decorator(self):
```

### Comparing `fresco-3.1.0/fresco/tests/test_exceptions.py` & `fresco-3.2.0/fresco/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `fresco-3.1.0/fresco/tests/test_middleware.py` & `fresco-3.2.0/fresco/tests/test_middleware.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,47 +28,43 @@
             request = context.request
             return Response([request.url, request.environ["REMOTE_ADDR"]])
 
         app.add_middleware(XForwarded, *args, **kwargs)
         return app
 
     def test_forwards_x_forwarded_for(self):
-
         app = self.get_app()
         with app.requestcontext(
             "/", REMOTE_ADDR="127.0.0.1", HTTP_X_FORWARDED_FOR="1.2.3.4"
         ):
             url, addr = app.view().content_iterator
             assert addr == b"1.2.3.4"
 
     def test_forwards_x_forwarded_host(self):
-
         app = self.get_app()
         with app.requestcontext(
             "/",
             REMOTE_ADDR="127.0.0.1",
             HTTP_X_FORWARDED_HOST="frontendserver",
         ):
             url, addr = app.view().content_iterator
         assert url == b"http://frontendserver/"
 
     def test_forwards_x_forwarded_ssl(self):
-
         app = self.get_app()
         with app.requestcontext(
             "/",
             REMOTE_ADDR="127.0.0.1",
             HTTP_X_FORWARDED_SSL="on",
             HTTP_X_FORWARDED_HOST="localhost",
         ):
             url, addr = app.view().content_iterator
             assert url == b"https://localhost/"
 
     def test_forwards_x_forwarded_proto(self):
-
         app = self.get_app()
         with app.requestcontext(
             "/",
             REMOTE_ADDR="127.0.0.1",
             HTTP_X_FORWARDED_PROTO="https",
             HTTP_X_FORWARDED_HOST="localhost",
         ):
```

### Comparing `fresco-3.1.0/fresco/tests/test_multidict.py` & `fresco-3.2.0/fresco/tests/test_multidict.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,17 +14,15 @@
 #
 import pytest
 from fresco.multidict import MultiDict
 
 
 def is_consistent(multidict: MultiDict) -> bool:
     "Verify that the MultiDict has internal consistency"
-    dictallitems = sorted(
-        (k, v) for k, vs in multidict._dict.items() for v in vs
-    )
+    dictallitems = sorted((k, v) for k, vs in multidict._dict.items() for v in vs)
     orderallitems = sorted(multidict._order)
     return list(sorted(dictallitems)) == list(sorted(orderallitems))
 
 
 class TestMultDict(object):
     def test_getitem_returns_only_first(self):
         m = MultiDict([("a", 1), ("a", 2), ("b", 3)])
```

### Comparing `fresco-3.1.0/fresco/tests/test_options.py` & `fresco-3.2.0/fresco/tests/test_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,25 +62,23 @@
             pass
 
         options = Options()
         options.update_from_object(Foo(), True)
         assert "__module__" in options
 
     def test_options_update_from_file(self):
-
         with NamedTemporaryFile() as tmpfile:
             tmpfile.write(b"a = 1\nb = 2\n")
             tmpfile.flush()
 
             options = Options()
             options.update_from_file(tmpfile.name)
             assert options == {"a": 1, "b": 2}
 
     def test_options_update_from_file_has_dunder_file_global(self):
-
         with NamedTemporaryFile() as tmpfile:
             tmpfile.write(b"a = __file__")
             tmpfile.flush()
 
             options = Options()
             options.update_from_file(tmpfile.name)
             assert options == {"a": tmpfile.name}
```

### Comparing `fresco-3.1.0/fresco/tests/test_request.py` & `fresco-3.2.0/fresco/tests/test_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,20 +169,18 @@
             now = c.request.now
             assert now.tzinfo is datetime.timezone.utc
             assert now is c.request.now
 
 
 class TestPathEncoding(object):
     def test_url_is_quoted(self):
-
         with context(SCRIPT_NAME=fixtures.wsgi_unicode_path, PATH_INFO="") as c:
             assert c.request.url == "http://localhost" + fixtures.quoted_unicode_path
 
     def test_application_url_is_quoted(self):
-
         with context(SCRIPT_NAME=fixtures.wsgi_unicode_path, PATH_INFO="") as c:
             assert (
                 c.request.application_url
                 == "http://localhost" + fixtures.quoted_unicode_path
             )
 
     def test_parsed_url_is_quoted(self):
@@ -253,14 +251,25 @@
     def test_query_dict(self):
         with context() as c:
             self.assert_equal_with_query(
                 c.request.make_url(query={"a": 1, "b": "2 3"}),
                 "http://localhost/?a=1&b=2+3",
             )
 
+    def test_query_drops_items_with_None_value(self):
+        with context() as c:
+            self.assert_equal_with_query(
+                c.request.make_url(query={"a": 1, "b": None}),
+                "http://localhost/?a=1",
+            )
+            self.assert_equal_with_query(
+                c.request.make_url(query=[("a", 1), ("b", None)]),
+                "http://localhost/?a=1",
+            )
+
     def test_query_kwargs(self):
         with context() as c:
             self.assert_equal_with_query(
                 c.request.make_url(query={"a": 1}, b=2),
                 "http://localhost/?a=1&b=2",
             )
 
@@ -360,15 +369,14 @@
     def test_currentrequest_returns_None(self):
         from fresco import currentrequest
 
         assert currentrequest() is None
 
 
 class TestMultipart(object):
-
     filename = "test.txt"
     filedata = "123456\n"
     boundary = "---------------------------1234"
 
     post_data = (
         (
             "--{boundary}\r\n"
@@ -388,37 +396,36 @@
         "wsgi_input": post_data,
         "REQUEST_METHOD": "POST",
         "CONTENT_TYPE": "multipart/form-data; boundary=" + boundary,
         "CONTENT_LENGTH": str(len(post_data)),
     }
 
     def test_files_populated(self):
-
         with FrescoApp().requestcontext(**self.request_args) as c:
             request = c.request
 
-        assert len(request.files) == 1
-        assert "uploaded_file" in request.files
+            assert len(request.files) == 1
+            assert "uploaded_file" in request.files
 
     def test_file_content_available(self):
-
         with FrescoApp().requestcontext(**self.request_args) as c:
             request = c.request
 
-        b = BytesIO()
-        request.files["uploaded_file"].save(b)
+            b = BytesIO()
+            request.files["uploaded_file"].save(b)
         assert b.getvalue() == self.filedata.encode("latin1")
 
     def test_headers_available(self):
-
         with FrescoApp().requestcontext(**self.request_args) as c:
             request = c.request
 
-        assert request.files["uploaded_file"].headers["content-type"] == "text/plain"
-        assert request.files["uploaded_file"].filename == self.filename
+            assert (
+                request.files["uploaded_file"].headers["content-type"] == "text/plain"
+            )
+            assert request.files["uploaded_file"].filename == self.filename
 
     def test_quotes_in_input_names_are_decoded(self):
         """
         Field names in multipart form data must be decoded as RFC822
         quoted-strings
         """
         data = (
```

### Comparing `fresco-3.1.0/fresco/tests/test_requestcontext.py` & `fresco-3.2.0/fresco/tests/test_requestcontext.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,14 @@
         app = FrescoApp()
         app.route("/", GET, view)
 
         with app.requestcontext("/"):
             app.view()
 
     def test_context_returns_correct_request_for_each_app(self):
-
         from time import sleep
         from threading import Thread, current_thread
 
         threadcount = 3
         itercount = 200
         calls = []
```

### Comparing `fresco-3.1.0/fresco/tests/test_response.py` & `fresco-3.2.0/fresco/tests/test_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,37 +181,36 @@
     def test_delete_cookie(self):
         r = Response().delete_cookie(name="fruit")
         assert r.get_header("Set-Cookie") == (
             "fruit=;Expires=Thu, 01 Jan 1970 00:00:00 GMT;Max-Age=0;Path=/;SameSite=Lax"
         )
 
     def test_response_get_headers(self):
-
         r = Response(
             ["whoa nelly!"],
             content_type="text/plain",
             x_test_header=["1", "2"],
         )
         assert r.get_header("content-type") == "text/plain"
         assert r.get_header("x-test-header") == "1,2"
         assert r.get_header("X-Test-Header") == "1,2"
         assert r.get_header("x-does-not-exist", "boo!") == "boo!"
 
     def test_response_buffered_sets_content_length(self):
         r = Response(["whoa nelly!"]).buffered()
         assert r.get_header("content-length") == "11"
 
-        r = Response([u"whoa nélly!"]).buffered()
+        r = Response(["whoa nélly!"]).buffered()
         assert r.get_header("content-length") == "12"
 
     def test_it_encodes_a_unicode_string_according_to_content_type(self):
-        r = Response(u"café", content_type="text/plain; charset=utf-8")
-        assert list(r({}, Mock())) == [u"café".encode("utf-8")]
-        r = Response(u"café", content_type="text/plain; charset=latin-1")
-        assert list(r({}, Mock())) == [u"café".encode("latin-1")]
+        r = Response("café", content_type="text/plain; charset=utf-8")
+        assert list(r({}, Mock())) == ["café".encode("utf-8")]
+        r = Response("café", content_type="text/plain; charset=latin-1")
+        assert list(r({}, Mock())) == ["café".encode("latin-1")]
 
 
 class TestAddVary(object):
     def test_it_adds_a_vary_header(self):
         r = Response(content_type="text/plain").add_vary("Accept-Encoding")
         assert ("Vary", "Accept-Encoding") in r.headers
```

### Comparing `fresco-3.1.0/fresco/tests/test_routeargs.py` & `fresco-3.2.0/fresco/tests/test_routeargs.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,22 +20,20 @@
 from fresco.routing import GET
 from fresco.routing import POST
 from fresco.routing import Route
 
 
 class TestRouteArg(object):
     def test_routekwarg_configured(self):
-
         A = routeargs.RouteArg()
         route = Route("/", GET, lambda r: None, x=A)
         assert A.route is route
         assert A.name == "x"
 
     def test_routekwarg_value_passed(self):
-
         view = Mock(return_value=Response())
         routekwarg = Mock(spec=routeargs.RouteArg)
         routekwarg.return_value = "xyzzy"
 
         app = FrescoApp()
         app.route("/", GET, view, x=routekwarg)
         with app.requestcontext("/") as c:
@@ -158,26 +156,24 @@
             app.view()
             x = view.call_args[1]["x"]
             assert x is c.request
 
 
 class Test_routearg(object):
     def test_it_calls_func(object):
-
         view = Mock(return_value=Response())
         argfunc = Mock()
         app = FrescoApp()
         app.route("/", GET, view, x=routeargs.routearg(argfunc))
         with app.requestcontext("/"):
             app.view()
             assert argfunc.call_count == 1, argfunc.call_count
             assert view.call_args[1]["x"] is argfunc()
 
     def test_it_passes_additional_args(object):
-
         view = Mock(return_value=Response())
         argfunc = Mock()
         app = FrescoApp()
         app.route("/", GET, view, x=routeargs.routearg(argfunc, "x", y=42))
         with app.requestcontext("/") as c:
             app.view()
             assert argfunc.call_args == ((c.request, "x"), {"y": 42})
@@ -204,15 +200,14 @@
             "/", data=b'{"foo":"bar"}', CONTENT_TYPE="application/json"
         ):
             app.view()
             x = view.call_args[1]["x"]
             assert x == {"foo": "bar"}
 
     def test_it_returns_bad_request_on_invalid_payload(self):
-
         view = Mock(return_value=Response())
         app = FrescoApp()
         app.route("/", POST, view, x=routeargs.JSONPayload())
         with app.requestcontext_post(
             "/", data=b"invalid json!", CONTENT_TYPE="application/json"
         ):
             r = app.view()
```

### Comparing `fresco-3.1.0/fresco/tests/test_routing.py` & `fresco-3.2.0/fresco/tests/test_routing.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,14 @@
         assert method.__self__ is ob
     except AttributeError:
         assert method.im_self is ob
 
 
 class TestMethodDispatch(object):
     def test_route_is_dispatched_to_correct_method(self):
-
         getview = Mock(return_value=Response())
         postview = Mock(return_value=Response())
         app = FrescoApp()
         app.route("/", GET, getview)
         app.route("/", POST, postview)
 
         with app.requestcontext("/"):
@@ -66,15 +65,14 @@
             app.view()
             assert getview.call_count == 1
             assert postview.call_count == 1
 
 
 class TestRouteConstructor(object):
     def test_multiple_views_can_be_associated_with_a_route(self):
-
         app = FrescoApp()
         v1 = Mock(return_value=Response())
         v2 = Mock(return_value=Response())
         app.route("/", GET=v1, POST=v2)
 
         with app.requestcontext():
             app.view()
@@ -99,15 +97,14 @@
 
         with app.requestcontext_post():
             app.view()
             assert v1.call_count == 1
             assert v2.call_count == 1
 
     def test_it_catches_invalid_methods(self):
-
         # Route must be a string or an iterable
         with pytest.raises(TypeError):
             Route("/", object(), lambda: None)
 
         # Route must be a valid HTTP method
         with pytest.raises(ValueError):
             Route("/", "FOO", lambda: None)
@@ -158,15 +155,14 @@
         mock = Mock(return_value=None)
         app = FrescoApp([Route("/", GET=Response, foo="bar").before(mock)])
         with app.requestcontext("/"):
             app.view()
         assert mock.call_args_list == [call(foo="bar")]
 
     def test_it_applies_chained_hook_calls_in_order(self):
-
         mock = Mock(return_value=None)
 
         @Route.before(mock, 1)
         @Route.before(mock, 2)
         def view():
             return Response()
 
@@ -236,29 +232,27 @@
             return response.replace(
                 content=[b"".join(response.content_iterator) + b"!"]
             )
 
         return exclaim
 
     def test_decorator_is_applied(self):
-
         views = fixtures.CBV("test")
 
         app = FrescoApp()
         app.route("/decorated", GET, views.index_html, decorators=[self.exclaim])
         app.route("/plain", GET, views.index_html)
 
         with app.requestcontext("/decorated"):
             assert list(app.view().content_iterator) == [b"test!"]
 
         with app.requestcontext("/plain"):
             assert list(app.view().content_iterator) == [b"test"]
 
     def test_decorator_is_applied_with_wrap_method(self):
-
         views = fixtures.CBV("test")
 
         app = FrescoApp()
         app.route("/decorated", GET, views.index_html).wrap(self.exclaim)
         app.route("/plain", GET, views.index_html)
 
         with app.requestcontext("/decorated"):
@@ -284,15 +278,14 @@
         app.include("/a", A())
         with app.requestcontext("/"):
             assert list(app.view().content_iterator) == [b"test!"]
         with app.requestcontext("/a/"):
             assert list(app.view().content_iterator) == [b"test!"]
 
     def test_decorator_works_with_urlfor(self):
-
         views = fixtures.CBV("test")
         app = FrescoApp()
         app.route("/decorated", GET, views.index_html, decorators=[self.exclaim])
         with app.requestcontext():
             assert urlfor(views.index_html, _app=app) == "http://localhost/decorated"
 
     def test_using_wraps_with_viewspec_doesnt_raise_AttributeError(self):
@@ -369,46 +362,42 @@
         class A:
             __routes__ = [r2, r3]
 
         rc = RouteCollection([r1, A()])
         assert [r.name for r in rc] == ["1", "2", "3"]
 
     def test_get_routes_matches_on_method(self):
-
         r_get = Route("/", GET, None)
         r_post = Route("/", POST, None)
 
         rc = RouteCollection([r_post, r_get])
 
         assert [r.route for r in rc.get_route_traversals("/", GET)] == [r_get]
         assert [r.route for r in rc.get_route_traversals("/", POST)] == [r_post]
 
     def test_get_routes_matches_on_path(self):
-
         r1 = Route("/1", GET, None)
         r2 = Route("/2", GET, None)
 
         rc = RouteCollection([r1, r2])
 
         assert [r.route for r in rc.get_route_traversals("/1", GET)] == [r1]
         assert [r.route for r in rc.get_route_traversals("/2", GET)] == [r2]
 
     def test_get_routes_can_match_all_methods(self):
-
         r1 = Route("/1", GET, None)
         r2 = Route("/1", POST, None)
 
         rc = RouteCollection([r1, r2])
         assert [r.route for r in rc.get_route_traversals("/1", None)] == [
             r1,
             r2,
         ]
 
     def test_route_returns_traversal_information_on_nested_routes(self):
-
         a = RouteCollection()
         b = RouteCollection()
 
         a_route = Route("/harvey", GET, lambda: None)
         b_route = Route("/harvey", GET, lambda: None)
 
         a.add_route(a_route)
@@ -608,14 +597,21 @@
 
         test_wsgi_app("/prefix", "/prefix", "/prefix", "")
         test_wsgi_app("/prefix", "/prefix/", "/prefix", "/")
         test_wsgi_app("/", "/", "", "/")
         test_wsgi_app("/", "/foo", "", "/foo")
         test_wsgi_app("/prefix", "/prefix", "", "/prefix", rewrite_script_name=False)
 
+    def test_it_routes_to_a_wsgi_app_by_dotted_path(self):
+        app = FrescoApp()
+        app.route_wsgi("/", "fresco.tests.fixtures.wsgi_app")
+        with app.requestcontext("/"):
+            response = app.view()
+        assert list(response.content_iterator) == [b"ok"]
+
     def test_fallthrough_can_be_applied_to_collection(self):
         a = Route("/fee", GET=lambda: Response(status=204))
         a = Route("/fie", GET=lambda: Response(status=204))
         b = Route("/foe", GET=lambda: Response(status=204))
         rc = RouteCollection([a, b])
         rc = rc.fallthrough_on(["204"])
         assert all(r.fallthrough_statuses == {204} for r in rc.__routes__)
@@ -673,29 +669,27 @@
         app = FrescoApp()
         app.delegate("/foo", Views())
 
         with app.requestcontext("/foo/hello"):
             assert app.view().content == b"OK"
 
     def test_url_variables_are_passed(self):
-
         hello = Mock(return_value=Response())
 
         inner = FrescoApp()
         inner.route("/<i:str>", GET, hello)
 
         outer = FrescoApp()
         outer.delegate("/<o:str>", inner)
 
         with outer.requestcontext("/foo/bar"):
             outer.view()
             assert hello.call_args_list == [call(i="bar", o="foo")]
 
     def test_delegation_to_dynamic_routes(self):
-
         result = []
 
         class MyRoutes(object):
             __routes__ = [Route("/<inner:int>", GET, "view")]
 
             def __init__(self, **kwargs):
                 self.kwargs = kwargs
@@ -709,15 +703,14 @@
         with app.requestcontext("/one/2"):
             app.view()
             instance, inner_kwargs = result[0]
             assert instance.kwargs == {"outer": "one"}
             assert inner_kwargs == {"inner": 2}
 
     def test_dynamic_routes_are_never_shared(self):
-
         result = []
 
         class MyRoutes(object):
             __routes__ = [Route("", GET, "view")]
 
             def __init__(self, value):
                 self.value = value
@@ -744,27 +737,25 @@
         outer = FrescoApp()
         outer.delegate("/<o:str>", inner, name="delegation")
 
         with outer.requestcontext("/foo/bar"):
             assert outer.pathfor("delegation:inner-route", o="x", i="y") == "/x/y"
 
     def test_pathfor_with_dynamic_delegated_route(self):
-
         view = Mock(return_value=Response())
 
         def routecollectionfactory(*args, **kwargs):
             return RouteCollection([Route("/<i:str>", GET, view, name="inner-route")])
 
         rc = RouteCollection()
         rc.delegate("/<o:str>", routecollectionfactory, name="delegation", dynamic=True)
 
         assert rc.pathfor("delegation:inner-route", o="x", i="y") == "/x/y"
 
     def test_pathfor_with_dynamic_delegated_route_uses_default_args(self):
-
         view = Mock(return_value=Response())
 
         def routecollectionfactory(factoryarg1, factoryarg2):
             return RouteCollection([Route("/<i:str>", GET, view, name="inner-route")])
 
         rc = RouteCollection()
         rc.delegate(
@@ -775,15 +766,14 @@
             name="delegation",
             dynamic=True,
         )
 
         assert rc.pathfor("delegation:inner-route", i="y") == "/foo/bar/y"
 
     def test_urlfor_with_dynamic_delegated_route_and_view_self(self):
-
         result = []
 
         class MyRoutes(object):
             __routes__ = [Route("/<inner:int>/view", GET, "view")]
 
             def __init__(self, **kwargs):
                 self.kwargs = kwargs
@@ -810,15 +800,14 @@
 
         app = FrescoApp()
         app.delegate("/<a:str>", Routable, dynamic=True, name="x")
         with app.requestcontext("/two/2/view"):
             assert urlfor("x:y", a="a", b=1) == "http://localhost/a/1"
 
     def test_delegated_routes_can_be_included(self):
-
         view = Mock(return_value=Response())
 
         inner = RouteCollection([Route("/baz", GET, view)])
         middle = RouteCollection([DelegateRoute("/bar", inner)])
         outer = FrescoApp()
         outer.include("/foo", middle)
         with outer.requestcontext("/foo/bar/baz"):
@@ -985,15 +974,14 @@
         routes.route("/", GET, myview)
 
         assert list(routes.get_route_traversals("/", GET)) == [
             tms.InstanceOf(RouteTraversal, route=tms.InstanceOf(self.CustomRoute))
         ]
 
     def test_it_uses_route_class_in_decorator(self):
-
         routes = RouteCollection(route_class=self.CustomRoute)
 
         @routes.route("/", GET)
         def myview():
             pass
 
         assert list(routes.get_route_traversals("/", GET)) == [
@@ -1012,15 +1000,14 @@
 
         assert list(routes2.get_route_traversals("/incl/", GET)) == [
             tms.InstanceOf(RouteTraversal, route=tms.InstanceOf(self.CustomRoute))
         ]
 
 
 class TestRouteTraversal(object):
-
     routes = RouteCollection()
     inner = RouteCollection()
     inner2 = RouteCollection()
 
     view = object()
     inner2.route("/<i:int>", GET=view, name="c")
     inner.delegate("/<i:int>", inner2, name="b")
@@ -1029,15 +1016,14 @@
     def test_it_reconstructs_the_path(self):
         traversal = next(self.routes.get_route_traversals("/1/2/3", GET))
 
         # Do we get the original path back?
         assert traversal.build_path() == "/1/2/3"
 
     def test_it_modifies_the_path(self):
-
         traversal = next(self.routes.get_route_traversals("/1/2/3", GET))
 
         # Modify the traversal and check we get a modified path back
         assert traversal.replace("a", {"i": 0}).build_path() == "/0/2/3"
 
         assert traversal.replace("b", {"i": 0}).build_path() == "/1/0/3"
         assert traversal.replace("a:b", {"i": 0}).build_path() == "/1/0/3"
```

### Comparing `fresco-3.1.0/fresco/tests/test_static.py` & `fresco-3.2.0/fresco/tests/test_static.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,22 +22,21 @@
 from fresco import FrescoApp
 from fresco.static import serve_static_file
 from fresco.util.wsgi import ClosingIterator
 from fresco.util.wsgi import apply_request
 
 
 class TestServeStaticFile:
-    def setup(self):
-
+    def setup_method(self):
         fh, tmpname = mkstemp()
         self.tmpname = tmpname
         self.mtime = int(os.path.getmtime(self.tmpname))
         os.close(fh)
 
-    def teardown(self):
+    def teardown_method(self):
         os.unlink(self.tmpname)
 
     def parse_lmh(self, last_modified):
         return timegm(parsedate(last_modified))  # type: ignore
 
     def make_ims(self, since, tz=0):
         return {"HTTP_IF_MODIFIED_SINCE": formatdate(since, tz)}
```

### Comparing `fresco-3.1.0/fresco/tests/test_subrequests.py` & `fresco-3.2.0/fresco/tests/test_subrequests.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 # encoding: UTF-8
 from fresco.core import FrescoApp
 from fresco.routing import GET
 from fresco.routing import Route
 from fresco.requestcontext import context
 from fresco.response import Response
 from fresco.routeargs import GetArg, routearg
-from fresco.subrequests import subrequest, subrequest_raw, subrequest_bytes
+from fresco.subrequests import subrequest
+from fresco.subrequests import subrequest_bytes
+from fresco.subrequests import subrequest_raw
+from fresco.subrequests import subrequest_str
 
 from unittest.mock import Mock
 import typing as t
 import pytest
 
 
 class TestSubRequest(object):
@@ -124,15 +127,14 @@
         with app.requestcontext():
             assert (
                 subrequest("named collection:named view", a="foo", b="bar")
                 == "*foobar*"
             )
 
     def test_it_does_a_full_request(self):
-
         request_hook = Mock(return_value=None)
         view = Mock(return_value=Response())
 
         app = FrescoApp()
         app.route("/view", GET, view)
         app.process_request(request_hook)
         with app.requestcontext():
@@ -141,15 +143,14 @@
             assert request_hook.call_count == 0
 
             subrequest(view, _full=True)
             assert view.call_count == 2
             assert request_hook.call_count == 1
 
     def test_it_maintains_the_environ(self):
-
         subreq_environ = None
 
         def view():
             nonlocal subreq_environ
             subreq_environ = context.request.environ
             return Response()
 
@@ -158,15 +159,14 @@
 
         with app.requestcontext("/xyzzy") as c:
             original_environ = c.request.environ
             subrequest(view)
             assert subreq_environ is original_environ
 
     def test_it_passes_original_environ_values(self):
-
         subreq_environ = None
 
         def view():
             nonlocal subreq_environ
             subreq_environ = context.request.environ
             return Response()
 
@@ -193,15 +193,14 @@
             assert all(
                 subreq_environ[k] != environ_not_copied[k] for k in environ_not_copied
             )
             assert subreq_environ["PATH_INFO"] == "/view"
             assert subreq_environ["QUERY_STRING"] == "test"
 
     def test_it_merges_custom_environ_keys(self):
-
         subreq_environ: t.Optional[dict] = None
 
         def view():
             nonlocal subreq_environ
             subreq_environ = context.request.environ
             return Response()
 
@@ -210,7 +209,28 @@
 
         with app.requestcontext("/xyzzy") as c:
             original_environ = c.request.environ
             subrequest(view, _full=True, _env={"hey.there": True})
             assert subreq_environ is not None
             assert "hey.there" in subreq_environ
             assert "hey.there" not in original_environ
+
+    def test_it_exhausts_content_iterator_before_closing_response(self):
+        tracker = ["view inited"]
+
+        def view():
+            def responder():
+                tracker.append("responder started")
+                yield ",".join(tracker)
+
+            r = Response(responder())
+            r = r.add_onclose(lambda: tracker.append("response closed"))
+            return r
+
+        app = FrescoApp()
+        app.route("/", GET, view)
+
+        with app.requestcontext("/"):
+            result = subrequest_str(view, _full=True)
+        assert ",".join(tracker) == "view inited,responder started,response closed"
+
+        assert result == "view inited,responder started"
```

### Comparing `fresco-3.1.0/fresco/tests/util/form_data.py` & `fresco-3.2.0/fresco/tests/util/form_data.py`

 * *Files identical despite different names*

### Comparing `fresco-3.1.0/fresco/tests/util/test_common.py` & `fresco-3.2.0/fresco/tests/util/test_common.py`

 * *Files identical despite different names*

### Comparing `fresco-3.1.0/fresco/tests/util/test_http.py` & `fresco-3.2.0/fresco/tests/util/test_http.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 from fresco import FrescoApp
 from fresco import context
 from fresco import Response
 from fresco.exceptions import RequestParseError
 from fresco.routing import POST
 from fresco.util.http import FileUpload
+from fresco.util.http import PostParser
 from fresco.util.http import encode_multipart
 from fresco.util.http import parse_parameters
 from fresco.util.http import parse_post
 from fresco.util.http import parse_querystring
 
 from . import form_data
 
@@ -77,39 +78,37 @@
         for data in form_data.multipart_samples:
             io = BytesIO(data["data"])  # type: ignore
             io.seek(0)
             environ = {
                 "CONTENT_LENGTH": data["content_length"],
                 "CONTENT_TYPE": data["content_type"],
             }
-            parsed = sorted(list(parse_post(environ, io, "UTF-8")))
+            with PostParser(environ, io, "UTF-8") as parsed:
+                parsed = sorted(list(parsed))
 
-            assert [name for name, value in parsed] == [
-                "empty-text-input",
-                "file-upload",
-                "text-input-ascii",
-                "text-input-unicode",
-            ]
-
-            assert parsed[0] == ("empty-text-input", "")
-            assert parsed[2] == ("text-input-ascii", "abcdef")
-            assert parsed[3] == (
-                "text-input-unicode",
-                b"\xce\xb1\xce\xb2\xce\xb3\xce\xb4".decode("utf8"),
-            )
-
-            fieldname, fileupload = parsed[1]
-            assert isinstance(fileupload, FileUpload)
-            assert fieldname == "file-upload"
-            assert fileupload.filename == "test.data"
-            assert (
-                fileupload.headers["content-type"]
-                == "application/octet-stream"
-            )
-            assert fileupload.file.read() == form_data.FILE_UPLOAD_DATA
+                assert [name for name, value in parsed] == [
+                    "empty-text-input",
+                    "file-upload",
+                    "text-input-ascii",
+                    "text-input-unicode",
+                ]
+
+                assert parsed[0] == ("empty-text-input", "")
+                assert parsed[2] == ("text-input-ascii", "abcdef")
+                assert parsed[3] == (
+                    "text-input-unicode",
+                    b"\xce\xb1\xce\xb2\xce\xb3\xce\xb4".decode("utf8"),
+                )
+
+                fieldname, fileupload = parsed[1]
+                assert isinstance(fileupload, FileUpload)
+                assert fieldname == "file-upload"
+                assert fileupload.filename == "test.data"
+                assert fileupload.headers["content-type"] == "application/octet-stream"
+                assert fileupload.file.read() == form_data.FILE_UPLOAD_DATA
 
     def test_non_ascii_headers(self):
         """
         Ensure that headers containing non-ascii characters are handled.
         NB the stdlib email.parser module that we use for parsing replaces
         any 8-bit characters with the unicode replacement character.
         """
@@ -123,18 +122,18 @@
             b"----XXXXXX--\r\n"
         )
         environ = {
             "CONTENT_LENGTH": len(data),
             "CONTENT_TYPE": "multipart/form-data; boundary=--XXXXXX",
         }
         f = BytesIO(data)
-        parsed = list(parse_post(environ, f, "UTF-8"))
-        fieldname, fileupload = parsed[0]
-        assert isinstance(fileupload, FileUpload)
-        assert fileupload.filename == "caf\uFFFD\uFFFD.txt"
+        with PostParser(environ, f, "UTF-8") as parsed:
+            fieldname, fileupload = list(parsed)[0]
+            assert isinstance(fileupload, FileUpload)
+            assert fileupload.filename == "caf\uFFFD\uFFFD.txt"
 
     def test_malformed_headers_raise_exceptions(self):
         # Missing '=' in parameter
         data, env = self._make_env(
             b"Content-Disposition: form-data; name; \r\n\r\n" b"1234567890\r\n"
         )
         with pytest.raises(RequestParseError):
@@ -194,22 +193,19 @@
             request.MAX_SIZE = 100
             request.get("f1")
             return Response(["ok"])
 
         app = FrescoApp()
         app.route("/", POST, view)
 
-        with app.requestcontext_post(
-            "/", multipart=True, data=[("f1", "x" * 200)]
-        ):
+        with app.requestcontext_post("/", multipart=True, data=[("f1", "x" * 200)]):
             assert app.view().status == "413 Payload Too Large"
 
 
 class TestParseFormEncodedData(object):
-
     char_latin1 = b"\xa3"
     char_utf8 = b"\xc2\xa3"
     char = char_latin1.decode("latin1")
 
     assert char_latin1.decode("latin1") == char_utf8.decode("utf8") == char
 
     def test_formencoded_data_too_big(self):
@@ -251,64 +247,56 @@
             CONTENT_TYPE="application/x-www-form-urlencoded",
             wsgi_input=data,
         ):
             response = app.view()
             assert response.status == "400 Bad Request"
 
     def test_non_utf8_data_posted(self):
-
         data = b"char=" + quote(self.char_latin1).encode("ascii")
         env = {
             "REQUEST_METHOD": "POST",
             "CONTENT_LENGTH": str(len(data)),
             "wsgi.input": BytesIO(data),
         }
 
         with FrescoApp().requestcontext(environ=env) as c:
             request = c.request
             request.charset = "latin1"
             assert request.form["char"] == self.char
 
     def test_non_utf8_data_getted(self):
-
         data = "char=" + quote(self.char_latin1)
         env = {"REQUEST_METHOD": "GET", "QUERY_STRING": data}
 
         with FrescoApp().requestcontext(environ=env) as c:
             request = c.request
             request.charset = "latin1"
             assert request.query["char"] == self.char
 
 
 class TestEncodeMultipart(object):
     def test_it_encodes_a_data_dict(self):
         data, headers = encode_multipart([("foo", "bar baf")])
         data = data.getvalue()
-        assert (
-            b'Content-Disposition: form-data; name="foo"\r\n\r\nbar baf'
-            in data
-        )
+        assert b'Content-Disposition: form-data; name="foo"\r\n\r\nbar baf' in data
 
     def test_it_encodes_a_file_tuple(self):
-        data, headers = encode_multipart(
-            files=[("foo", "foo.txt", "ascii", "bar")]
-        )
+        data, headers = encode_multipart(files=[("foo", "foo.txt", "ascii", "bar")])
         data = data.getvalue()
         expected = (
             b"Content-Disposition: form-data; "
             b'name="foo"; filename="foo.txt"\r\n'
             b"Content-Type: ascii\r\n"
             b"\r\n"
             b"bar"
         )
         assert expected in data
 
 
 class TestParseParameters(object):
-
     token = st.text(
         alphabet="".join(
             chr(c) for c in range(33, 127) if chr(c) not in '()<>@,;:\\/[]?="'
         ),
         min_size=1,
     )
```

### Comparing `fresco-3.1.0/fresco/tests/util/test_security.py` & `fresco-3.2.0/fresco/tests/util/test_security.py`

 * *Files identical despite different names*

### Comparing `fresco-3.1.0/fresco/tests/util/test_urls.py` & `fresco-3.2.0/fresco/tests/util/test_urls.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,17 +42,15 @@
 
     def test_triple_dot_preserved(self):
         assert normpath("/.../") == "/.../"
 
     def test_combined_patterns(self):
         assert normpath("/..//../") == "/"
         assert normpath("/hello/.//dolly//") == "/hello/dolly/"
-        assert (
-            normpath("///hello/.//dolly//./..//.//sailor") == "/hello/sailor"
-        )
+        assert normpath("///hello/.//dolly//./..//.//sailor") == "/hello/sailor"
 
     def test_trailing_slash_preserved(self):
         assert normpath("/sliced/bread/") == "/sliced/bread/"
 
 
 class TestMakeQuery(object):
     def test_make_query(self):
@@ -63,17 +61,17 @@
     def test_make_query_unicode(self):
         assert (
             make_query(a=[alpha, beta, gamma], charset="utf8")
             == "a=%CE%B1&a=%CE%B2&a=%CE%B3"
         )
 
     def test_make_query_unicode_default_encoding(self):
-        assert make_query(
-            a=[alpha, beta, gamma], charset="utf8"
-        ) == make_query(a=[alpha, beta, gamma])
+        assert make_query(a=[alpha, beta, gamma], charset="utf8") == make_query(
+            a=[alpha, beta, gamma]
+        )
 
 
 class TestSafeURL(object):
     def test_it_loads_defaults_from_context(self):
         with FrescoApp().requestcontext(
             **{"wsgi.url_scheme": "https", "HTTP_HOST": "foo.example.org"}
         ):
@@ -93,17 +91,15 @@
             "//good.example.org/",
             "/path?next_url=http://bad.example.org/",
         ]
         for u in safe:
             assert is_safe_url(u, allowed_hosts={"good.example.org"}) is True
 
     def test_it_handles_port_numbers_correctly(self):
-        def test(
-            scheme, server_name="localhost", server_port="80", http_host=None
-        ):
+        def test(scheme, server_name="localhost", server_port="80", http_host=None):
             env = {
                 "SERVER_NAME": server_name,
                 "SERVER_PORT": server_port,
                 "wsgi.url_scheme": scheme,
                 "HTTP_HOST": http_host,
             }
```

### Comparing `fresco-3.1.0/fresco/tests/util/test_wsgi.py` & `fresco-3.2.0/fresco/tests/util/test_wsgi.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,14 @@
     StartResponseWrapper,
     getenv,
     setenv,
 )
 
 
 class Counter(object):
-
     value = 0
 
     def inc(self):
         self.value += 1
 
 
 def start_response(status, headers, exc_info=None):
@@ -92,15 +91,14 @@
             r = Response.from_wsgi(
                 wsgiapp, c.request.environ, lambda status, headers: None
             )
             assert b"".join(r.content) == b"catsatmat"
 
 
 class TestEnvironGetSet(object):
-
     wsgibytes = "ø".encode("UTF-8")
     wsgistr = wsgibytes.decode("ISO-8859-1")
 
     def test_getenv_returns_bytes(self):
         assert getenv({"x": self.wsgistr}, "x") == "ø".encode("UTF-8")
 
     def test_setenv_sets_str(self):
```

### Comparing `fresco-3.1.0/fresco/util/cache.py` & `fresco-3.2.0/fresco/util/cache.py`

 * *Files identical despite different names*

### Comparing `fresco-3.1.0/fresco/util/common.py` & `fresco-3.2.0/fresco/util/common.py`

 * *Files 16% similar despite different names*

```diff
@@ -33,13 +33,11 @@
 
 def fq_path(ob):
     """
     Return the fully qualified path of ``ob``, expected to be a function or
     method
     """
     name = (
-        getattr(ob, "__qualname__", None)
-        or getattr(ob, "__name__", None)
-        or repr(ob)
+        getattr(ob, "__qualname__", None) or getattr(ob, "__name__", None) or repr(ob)
     )
     module = getattr(ob, "__module__", None) or ""
     return "{}.{}".format(module, name)
```

### Comparing `fresco-3.1.0/fresco/util/contentencodings.py` & `fresco-3.2.0/fresco/util/contentencodings.py`

 * *Files 0% similar despite different names*

```diff
@@ -318,15 +318,15 @@
         methodcaller("lower"),
         methodcaller("upper"),
     ],
     [
         lambda s: s,
         methodcaller("replace", "-", "_"),
         methodcaller("replace", "_", "-"),
-    ]
+    ],
 ]
 
 ALLOWED_ENCODINGS = {
     functools.reduce(lambda x, fn: fn(x), fns, enc)
     for enc in ALLOWED_ENCODINGS
     for fns in itertools.product(*transforms)
 }
```

### Comparing `fresco-3.1.0/fresco/util/file.py` & `fresco-3.2.0/fresco/util/file.py`

 * *Files identical despite different names*

### Comparing `fresco-3.1.0/fresco/util/http.py` & `fresco-3.2.0/fresco/util/http.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 from typing import Dict
 from typing import Iterator
 from typing import Iterable
 from typing import List
 from typing import Tuple
 from typing import Callable
 from typing import Union
+from typing import Optional
+import typing as t
 from tempfile import SpooledTemporaryFile
 import os
 import re
 import io
 
 from urllib.parse import unquote_plus
 from shutil import copyfileobj
@@ -51,14 +53,16 @@
 MB = 1024 * KB
 
 #: Data chunk size to read from the input stream (wsgi.input)
 CHUNK_SIZE = min(io.DEFAULT_BUFFER_SIZE, 1024)
 
 ParsedContentType = namedtuple("ParsedContentType", "content_type encoding params")
 
+ParsedField = Union["FileUpload", str]
+
 token_pattern = r"[!#-\'*-.0-9A-Z\^-~]+"
 quotedstringparts_pattern = r'(?:(\\.)|([^"\\]+))'
 quotedstring_pattern = r'"(?:{})*"'.format(quotedstringparts_pattern)
 quotedstring_parser = re.compile(r"{}".format(quotedstringparts_pattern))
 
 parameter_parser = re.compile(
     r"\s*"
@@ -191,15 +195,15 @@
         value,
         parse_parameters(remaining.strip(), preserve_backslashes=preserve_backslashes),
     )
 
 
 def parse_querystring(
     data: str,
-    charset: str = None,
+    charset: Optional[str] = None,
     strict: bool = False,
     keep_blank_values: bool = True,
 ) -> List[Tuple[str, str]]:
     """
     Return ``(key, value)`` pairs from the given querystring::
 
         >>> list(parse_querystring('green%20eggs=ham;me=sam+i+am'))
@@ -241,20 +245,20 @@
         except UnicodeDecodeError:
             raise RequestParseError(f"Invalid {charset} character data")
     return result
 
 
 def parse_post(
     environ,
-    fp,
-    default_charset=None,
+    _io: t.IO[bytes],
+    default_charset: Optional[str] = None,
     max_size=16 * KB,
     max_multipart_size=2 * MB,
     ie_workaround=True,
-) -> Iterable[Tuple[str, Union["FileUpload", str]]]:
+) -> Tuple[Iterable[Tuple[str, ParsedField]], Optional[Callable]]:
     """\
     Parse the contents of an HTTP POST request, which may be either
     application/x-www-form-urlencoded or multipart/form-data encoded.
 
     Returned items are either tuples of (name, value) for simple string values
     or (name, FileUpload) for uploaded files.
 
@@ -275,19 +279,22 @@
 
     try:
         content_length = int(environ["CONTENT_LENGTH"])
     except (TypeError, ValueError, KeyError):
         raise MissingContentLength()
 
     try:
-        bytestream = io_iterator(fp, CHUNK_SIZE, maxlen=content_length)
+        bytestream = io_iterator(_io, CHUNK_SIZE, maxlen=content_length)
         if ct == "application/x-www-form-urlencoded":
             if content_length > max_size:
                 raise TooBig("Content Length exceeds permitted size")
-            return parse_querystring(b"".join(bytestream).decode("ASCII"), charset)
+            return (
+                parse_querystring(b"".join(bytestream).decode("ASCII"), charset),
+                None,
+            )
         else:
             if content_length > max_multipart_size:
                 raise TooBig("Content Length exceeds permitted size")
             try:
                 boundary = ct_params["boundary"]
             except KeyError:
                 raise RequestParseError(
@@ -300,14 +307,30 @@
                 max_size,
                 ie_workaround=ie_workaround,
             )
     except UnicodeDecodeError:
         raise RequestParseError("Payload contains non ascii data")
 
 
+class PostParser:
+    close: t.Optional[Callable] = None
+
+    def __init__(self, *args, **kwargs):
+        self.args = args
+        self.kwargs = kwargs
+
+    def __enter__(self):
+        items, self.close = parse_post(*self.args, **self.kwargs)
+        return items
+
+    def __exit__(self, exc_type, exc_value, exc_traceback):
+        if self.close:
+            self.close()
+
+
 def get_body_bytes(environ, max_size=16 * KB) -> bytes:
     """
     Read a single message body from environ['wsgi.input'], returning a bytes
     object.
     """
     try:
         content_length = int(environ["CONTENT_LENGTH"])
@@ -315,41 +338,34 @@
         raise MissingContentLength()
 
     if content_length > max_size:
         raise TooBig("Content Length exceeds permitted size")
     return b"".join(io_iterator(environ["wsgi.input"], maxlen=content_length))
 
 
-def parse_body(environ, fp, default_charset=None, max_size=16 * KB):
-    """
-    Parse the message
-        (payload as a byte string, content-type, encoding)
-    """
-    ct, charset, params = get_content_type_info(
-        environ.get("CONTENT_TYPE", "text/plain")
-    )
-
-
 class HTTPMessage(Message):
     """
     Represent HTTP request message headers
     """
 
 
 def parse_multipart(
     stream: ByteIterator, boundary, default_charset, max_size, ie_workaround=True
-) -> Iterator[Tuple[str, Union["FileUpload", str]]]:
+) -> Tuple[Iterable[Tuple[str, ParsedField]], Optional[Callable]]:
     """
-    Parse data encoded as ``multipart/form-data``. Generate tuples of::
+    Parse data encoded as ``multipart/form-data``.
+    Return an iterator over tuples of ` (<field-name>, <data>)``, and an
+    optional ``close`` function.
 
-        (<field-name>, <data>)
-
-    Where ``data`` will be a string in the case of a regular input field, or a
+    ``data`` will be a string in the case of a regular input field, or a
     ``FileUpload`` instance if a file was uploaded.
 
+    If a ``close`` function is returned, the caller must call it in order to
+    close any temporary files created at the end of the request lifecycle.
+
     :param stream: input stream from which to read data
     :param boundary: multipart boundary string, as specified by the
                      ``Content-Disposition`` header
     :param default_charset: character set to use for encoding, if not specified
                             by a content-type header. In practice web browsers
                             don't supply a content-type header so this needs to
                             contain a sensible value.
@@ -378,69 +394,90 @@
     if peek[2 : boundary_size + 2] != boundary:
         raise RequestParseError("Malformed POST data: expected boundary")
 
     if peek[boundary_size + 2 : boundary_size + 4] != b"\r\n":
         raise RequestParseError("Malformed POST data: expected CRLF")
 
     stream = chain([peek[boundary_size + 4 :]], stream)
+    open_files = set()
+    fields = []
 
-    while True:
-        headers, data, stream = _read_multipart_field(stream, boundary, max_size)
-        try:
-            _, params = parse_header(
-                headers["Content-Disposition"], ie_workaround=ie_workaround
-            )
-        except KeyError:
-            raise RequestParseError("Missing Content-Disposition header")
+    try:
+        while True:
+            headers, data, stream = _read_multipart_field(stream, boundary, max_size)
+            open_files.add(data)
+            try:
+                _, params = parse_header(
+                    headers["Content-Disposition"], ie_workaround=ie_workaround
+                )
+            except KeyError:
+                raise RequestParseError("Missing Content-Disposition header")
 
-        try:
-            name = params["name"]
-        except KeyError:
-            raise RequestParseError("Missing name in Content-Disposition header")
-
-        is_file_upload = "Content-Type" in headers and "filename" in params
-        if is_file_upload:
-            data.seek(0)
-            yield name, FileUpload(params["filename"], headers, data)
-        else:
-            charset = parse_header(headers.get("Content-Type", ""))[1].get(
-                "charset", default_charset
-            )
-            if data.tell() > max_size:
-                data.close()
-                raise TooBig("Data block exceeds maximum permitted size")
             try:
+                name = params["name"]
+            except KeyError:
+                raise RequestParseError("Missing name in Content-Disposition header")
+
+            is_file_upload = "Content-Type" in headers and "filename" in params
+            if is_file_upload:
                 data.seek(0)
-                yield name, data.read().decode(charset)
-            except UnicodeDecodeError:
-                raise RequestParseError(f"Invalid {charset} character data")
-
-        peek = next(stream)
-        if peek[:2] == b"\r\n":
-            stream = chain([peek[2:]], stream)
-        elif peek == b"--\r\n":
-            if next(stream, None) is None:
-                break
+                fu = FileUpload(params["filename"], headers, data)
+                fields.append((name, fu))
             else:
-                RequestParseError("Boundary not properly terminated")
-        else:
-            raise RequestParseError("Boundary not properly terminated")
+                charset = parse_header(headers.get("Content-Type", ""))[1].get(
+                    "charset", default_charset
+                )
+                if data.tell() > max_size:
+                    data.close()
+                    open_files.remove(data)
+                    raise TooBig("Data block exceeds maximum permitted size")
+                try:
+                    data.seek(0)
+                    fields.append((name, data.read().decode(charset)))
+                    data.close()
+                    open_files.remove(data)
+                except UnicodeDecodeError:
+                    raise RequestParseError(f"Invalid {charset} character data")
+
+            peek = next(stream)
+            if peek[:2] == b"\r\n":
+                stream = chain([peek[2:]], stream)
+            elif peek == b"--\r\n":
+                if next(stream, None) is None:
+                    break
+                else:
+                    RequestParseError("Boundary incorrectly terminated")
+            else:
+                raise RequestParseError("Boundary incorrectly terminated")
+    except Exception:
+        for f in open_files:
+            f.close()
+        raise
+
+    close: Optional[Callable] = None
+    if open_files:
+
+        def close():
+            for f in open_files:
+                f.close()
+
+    return fields, close
 
 
 def _read_multipart_field(
     stream: ByteIterator, boundary: bytes, max_size: int
 ) -> Tuple["HTTPMessage", SpooledTemporaryFile, ByteIterator]:
     """
     Read a single part from a multipart/form-data message and return a tuple of
     ``(headers, data, remainder)``.
 
     Iterator ``iostream`` must be positioned at the start of the header block
     for the field.
 
-    Return a tuple of ('<headers>', '<data>')
+    The caller must call ``data.close()`` after consuming the data.
 
     ``headers`` is an instance of ``email.message.Message``.
 
     ``data`` is an instance of ``tempfile.SpooledTemporaryFile``.
     """
     output = SpooledTemporaryFile(max_size)
     parser = BytesFeedParser(_factory=HTTPMessage)
@@ -524,15 +561,14 @@
 
 class FileUpload(object):
     """\
     Represent a file uploaded in an HTTP form submission
     """
 
     def __init__(self, filename, headers, fileob):
-
         self.filename = filename
         self.headers = headers
         self.file = fileob
 
         # UNC/Windows path
         if self.filename[:2] == "\\\\" or self.filename[1:3] == ":\\":
             self.filename = self.filename[self.filename.rfind("\\") + 1 :]
```

### Comparing `fresco-3.1.0/fresco/util/io.py` & `fresco-3.2.0/fresco/util/io.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,24 +13,23 @@
 #     limitations under the License.
 #
 #
 """
 Utilities for wrapping IO streams. These are used internally by
 fresco when parsing wsgi request input streams.
 """
-from io import IOBase
 from io import DEFAULT_BUFFER_SIZE
 
-from typing import Iterator
+import typing as t
 
 
-ByteIterator = Iterator[bytes]
+ByteIterator = t.Iterator[bytes]
 
 
-def io_iterator(fp: IOBase, size=DEFAULT_BUFFER_SIZE, maxlen=-1) -> ByteIterator:
+def io_iterator(fp: t.IO, size=DEFAULT_BUFFER_SIZE, maxlen=-1) -> ByteIterator:
     bytecount = 0
     if maxlen > 0:
         while True:
             r = fp.read(min(maxlen - bytecount, size))
             bytecount += len(r)
             if r == b"":
                 return
```

### Comparing `fresco-3.1.0/fresco/util/security.py` & `fresco-3.2.0/fresco/util/security.py`

 * *Files identical despite different names*

### Comparing `fresco-3.1.0/fresco/util/textproc.py` & `fresco-3.2.0/fresco/util/textproc.py`

 * *Files identical despite different names*

### Comparing `fresco-3.1.0/fresco/util/urls.py` & `fresco-3.2.0/fresco/util/urls.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,17 +21,19 @@
 from itertools import chain
 from typing import List
 from urllib.parse import quote_plus
 from urllib.parse import urlparse
 from urllib.parse import urlunparse
 import posixpath
 import re
+import typing as t
 
 import fresco
 from fresco.multidict import MultiDict
+from fresco.types import QuerySpec
 
 __all__ = "join_path", "url_join", "strip_trailing_slashes", "normpath"
 
 
 def join_path(a, b):
     """
     Join two URL path segments together.
@@ -89,17 +91,15 @@
     # Link is already absolute, return it unchanged
     if prel.scheme:
         return rel
 
     pbase = urlparse(base)
     path = pbase.path
     if prel.path:
-        path = normpath(
-            posixpath.join(posixpath.dirname(pbase.path), prel.path)
-        )
+        path = normpath(posixpath.join(posixpath.dirname(pbase.path), prel.path))
 
     return urlunparse(
         (
             pbase.scheme,
             pbase.netloc,
             path,
             prel.params,
@@ -166,15 +166,20 @@
             continue
 
         newpath_append(seg)
 
     return "/".join(newpath)
 
 
-def make_query(data=None, separator="&", charset=None, **kwargs):
+def make_query(
+    data: QuerySpec = [],
+    separator: str = "&",
+    charset: t.Optional[str] = None,
+    **kwargs,
+) -> str:
     """
     Return a query string formed from the given dictionary data.
 
     If no encoding is given, unicode values are encoded using the character set
     specified by ``fresco.DEFAULT_CHARSET``.
 
     Basic usage::
@@ -201,20 +206,19 @@
         'x=1'
 
     :param data: data for query string
     :param separator: separator used between each key value pair
     :param charset: encoding to be used for unicode values
     :rtype: str
     """
+    items: t.Iterable[t.Tuple[str, t.Any]]
     if isinstance(data, MultiDict):
         items = data.allitems()
     elif isinstance(data, Mapping):
         items = data.items()
-    elif data is None:
-        items = []
     else:
         items = data
     if kwargs:
         items = chain(items, kwargs.items())
 
     if charset is None:
         charset = fresco.DEFAULT_CHARSET
@@ -223,15 +227,15 @@
     append = pairs.append
     for k, v in items:
         if isinstance(v, (str, bytes)):
             append(f"{quote_plus(k, charset)}={quote_plus(v, charset)}")
         elif hasattr(v, "__iter__"):
             for v in v:
                 append(f"{quote_plus(k, charset)}={quote_plus(str(v), charset)}")
-        else:
+        elif v is not None:
             append(f"{quote_plus(k, charset)}={quote_plus(str(v), charset)}")
     return separator.join(pairs)
 
 
 def _qs_frag(key, value, charset=None):
     """\
     Return a fragment of a query string in the format 'key=value'::
@@ -311,17 +315,15 @@
                 allowed_hosts = {f"{server_name}:{server_port}"}
 
     parsed = urlparse(url)
     scheme = parsed.scheme
     netloc = parsed.netloc
     if ":" in netloc:
         host, port = netloc.split(":")
-        if (scheme == "http" and port == "80") or (
-            scheme == "https" and port == "443"
-        ):
+        if (scheme == "http" and port == "80") or (scheme == "https" and port == "443"):
             netloc = host
 
     return (
         (scheme in allowed_schemes and netloc in allowed_hosts)
         or (scheme == "" and netloc == "")
         or (scheme == "" and netloc in allowed_hosts)
     )
```

### Comparing `fresco-3.1.0/fresco/util/wsgi.py` & `fresco-3.2.0/fresco/util/wsgi.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,27 +12,31 @@
 #     See the License for the specific language governing permissions and
 #     limitations under the License.
 #
 """
 Utilities for interfacing with WSGI
 """
 
+import logging
 from functools import partial
 from io import BytesIO
 from urllib.parse import unquote
 from urllib.parse import urlparse
 from typing import List
 from typing import Optional
 from typing import Tuple
 import sys
 
 from fresco.typing import ExcInfoTuple
 from fresco.typing import HeadersList
 from fresco.typing import WSGICallable
 
+logger = logging.getLogger(__name__)
+
+
 __all__ = [
     "environ_to_str",
     "str_to_environ",
     "environ_to_bytes",
     "bytes_to_environ",
     "StartResponseWrapper",
     "ClosingIterator",
@@ -297,17 +301,22 @@
         """
         return self._next()
 
     def close(self):
         """
         Call all close functions listed in ``*close_funcs``.
         """
-        self._closed = True
         for func in self._close_funcs:
-            func()
+            try:
+                func()
+            except Exception:
+                logger.exception(
+                    "ContentIterator close function {func!r} raised an exception"
+                )
+        self._closed = True
 
     def __del__(self):
         """
         Emit a warning if the iterator is deleted without ``close`` having been
         called.
         """
         if not self._closed:
```

### Comparing `fresco-3.1.0/fresco.egg-info/PKG-INFO` & `fresco-3.2.0/fresco.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: fresco
-Version: 3.1.0
+Version: 3.2.0
 Summary: A Web/WSGI micro-framework
 Home-page: https://ollycope.com/software/fresco/latest/
 Author: Oliver Cope
 Author-email: oliver@redgecko.org
 License: Apache
 Keywords: wsgi web www framework
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: PyPy
@@ -42,9 +41,7 @@
 
 
 Read the
 `fresco web framework documentation
 <https://ollycope.com/software/fresco/latest/>`_ for
 more about the framework, or
 visit the `source repo <https://sr.ht/~olly/fresco/>`_.
-
-
```

### Comparing `fresco-3.1.0/fresco.egg-info/SOURCES.txt` & `fresco-3.2.0/fresco.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 fresco/request.py
 fresco/requestcontext.py
 fresco/response.py
 fresco/routeargs.py
 fresco/routing.py
 fresco/static.py
 fresco/subrequests.py
+fresco/types.py
 fresco/typing.py
 fresco.egg-info/PKG-INFO
 fresco.egg-info/SOURCES.txt
 fresco.egg-info/dependency_links.txt
 fresco.egg-info/top_level.txt
 fresco/tests/__init__.py
 fresco/tests/fixtures.py
```

### Comparing `fresco-3.1.0/setup.cfg` & `fresco-3.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `fresco-3.1.0/setup.py` & `fresco-3.2.0/setup.py`

 * *Files identical despite different names*

