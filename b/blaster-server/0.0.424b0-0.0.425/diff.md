# Comparing `tmp/blaster-server-0.0.424b0.tar.gz` & `tmp/blaster-server-0.0.425.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blaster-server-0.0.424b0.tar", last modified: Mon Apr  3 11:06:16 2023, max compression
+gzip compressed data, was "blaster-server-0.0.425.tar", last modified: Sun Apr 16 18:16:05 2023, max compression
```

## Comparing `blaster-server-0.0.424b0.tar` & `blaster-server-0.0.425.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-03 11:06:16.492416 blaster-server-0.0.424b0/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1061 2019-07-03 19:03:00.000000 blaster-server-0.0.424b0/LICENSE.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       38 2022-11-07 18:47:07.000000 blaster-server-0.0.424b0/MANIFEST.in
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      851 2023-04-03 11:06:16.492416 blaster-server-0.0.424b0/PKG-INFO
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     2620 2022-11-14 12:45:11.000000 blaster-server-0.0.424b0/README.md
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2021-10-05 11:27:02.000000 blaster-server-0.0.424b0/__init__.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-03 11:06:16.488416 blaster-server-0.0.424b0/blaster/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      875 2023-01-09 13:10:46.000000 blaster-server-0.0.424b0/blaster/__init__.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-03 11:06:16.488416 blaster-server-0.0.424b0/blaster/cloud/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       51 2022-11-09 17:29:08.000000 blaster-server-0.0.424b0/blaster/cloud/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3257 2022-12-03 12:42:35.000000 blaster-server-0.0.424b0/blaster/cloud/analytics.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-03 11:06:16.488416 blaster-server-0.0.424b0/blaster/cloud/aws/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       78 2019-07-03 19:03:00.000000 blaster-server-0.0.424b0/blaster/cloud/aws/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1371 2022-12-01 11:30:06.000000 blaster-server-0.0.424b0/blaster/cloud/aws/ses_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5230 2023-01-28 12:53:32.000000 blaster-server-0.0.424b0/blaster/cloud/push_tasks.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3729 2023-03-23 02:32:10.000000 blaster-server-0.0.424b0/blaster/cloud/storage.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3796 2023-03-06 12:38:58.000000 blaster-server-0.0.424b0/blaster/config.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3715 2023-01-28 12:57:17.000000 blaster-server-0.0.424b0/blaster/connection_pool.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       99 2020-11-22 14:37:38.000000 blaster-server-0.0.424b0/blaster/constants.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5290 2023-03-30 07:56:48.000000 blaster-server-0.0.424b0/blaster/logging.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    62562 2023-03-20 21:38:44.000000 blaster-server-0.0.424b0/blaster/mongo_orm.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    14954 2023-03-22 22:32:18.000000 blaster-server-0.0.424b0/blaster/schema.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    36521 2023-04-03 11:05:37.000000 blaster-server-0.0.424b0/blaster/server.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    46829 2023-04-03 00:57:53.000000 blaster-server-0.0.424b0/blaster/tools.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-03 11:06:16.488416 blaster-server-0.0.424b0/blaster/utils/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2019-07-03 19:03:00.000000 blaster-server-0.0.424b0/blaster/utils/__init__.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-03 11:06:16.488416 blaster-server-0.0.424b0/blaster/utils/data/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    53078 2022-11-08 15:22:07.000000 blaster-server-0.0.424b0/blaster/utils/data/countries.json
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)   119011 2022-12-01 10:20:50.000000 blaster-server-0.0.424b0/blaster/utils/data/mime_types.json
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     6824 2023-01-08 13:22:03.000000 blaster-server-0.0.424b0/blaster/utils/data_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1951 2023-01-07 12:42:21.000000 blaster-server-0.0.424b0/blaster/utils/events.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     4812 2023-03-30 16:36:26.000000 blaster-server-0.0.424b0/blaster/utils/fork.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1076 2023-02-21 07:52:48.000000 blaster-server-0.0.424b0/blaster/utils/lat_long_utils.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     5552 2023-02-01 17:01:50.000000 blaster-server-0.0.424b0/blaster/utils/phone_number_utils.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     6773 2020-12-14 07:56:42.000000 blaster-server-0.0.424b0/blaster/utils/xss_html.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-03 11:06:16.488416 blaster-server-0.0.424b0/blaster/websocket/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1022 2019-07-03 19:03:00.000000 blaster-server-0.0.424b0/blaster/websocket/__init__.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    12874 2019-07-03 19:03:00.000000 blaster-server-0.0.424b0/blaster/websocket/_abnf.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    11136 2022-01-06 11:42:20.000000 blaster-server-0.0.424b0/blaster/websocket/_app.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    16360 2019-07-03 19:03:00.000000 blaster-server-0.0.424b0/blaster/websocket/_core.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     2141 2019-07-03 19:03:00.000000 blaster-server-0.0.424b0/blaster/websocket/_exceptions.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     4793 2019-07-03 19:03:00.000000 blaster-server-0.0.424b0/blaster/websocket/_handshake.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     7288 2019-07-03 19:03:00.000000 blaster-server-0.0.424b0/blaster/websocket/_http.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1870 2019-07-03 19:03:00.000000 blaster-server-0.0.424b0/blaster/websocket/_logging.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     3623 2019-07-03 19:03:00.000000 blaster-server-0.0.424b0/blaster/websocket/_socket.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1550 2019-07-03 19:03:00.000000 blaster-server-0.0.424b0/blaster/websocket/_ssl_compat.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     3670 2019-07-03 19:03:00.000000 blaster-server-0.0.424b0/blaster/websocket/_url.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     3632 2019-07-03 19:03:00.000000 blaster-server-0.0.424b0/blaster/websocket/_utils.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    12758 2021-10-03 12:23:56.000000 blaster-server-0.0.424b0/blaster/websocket/server.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-03 11:06:16.488416 blaster-server-0.0.424b0/blaster/websocket/tests/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2019-07-03 19:03:00.000000 blaster-server-0.0.424b0/blaster/websocket/tests/__init__.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    26115 2019-07-03 19:03:00.000000 blaster-server-0.0.424b0/blaster/websocket/tests/test_websocket.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-03 11:06:16.488416 blaster-server-0.0.424b0/blaster_server.egg-info/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      851 2023-04-03 11:06:16.000000 blaster-server-0.0.424b0/blaster_server.egg-info/PKG-INFO
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1682 2023-04-03 11:06:16.000000 blaster-server-0.0.424b0/blaster_server.egg-info/SOURCES.txt
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        1 2023-04-03 11:06:16.000000 blaster-server-0.0.424b0/blaster_server.egg-info/dependency_links.txt
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      221 2023-04-03 11:06:16.000000 blaster-server-0.0.424b0/blaster_server.egg-info/requires.txt
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       41 2023-04-03 11:06:16.000000 blaster-server-0.0.424b0/blaster_server.egg-info/top_level.txt
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-03 11:06:16.492416 blaster-server-0.0.424b0/examples/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2019-07-03 19:03:00.000000 blaster-server-0.0.424b0/examples/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      266 2022-01-06 11:42:20.000000 blaster-server-0.0.424b0/examples/fast_api_test.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      636 2019-07-03 19:03:00.000000 blaster-server-0.0.424b0/examples/gevent_wsgi_test.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      233 2021-10-04 14:48:01.000000 blaster-server-0.0.424b0/examples/meinheld_flask.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1743 2022-06-17 17:10:40.000000 blaster-server-0.0.424b0/examples/mongo_ormexample.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2386 2022-11-14 12:13:43.000000 blaster-server-0.0.424b0/examples/simple_examples.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1088 2019-07-03 19:03:00.000000 blaster-server-0.0.424b0/examples/test_chat_room.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      614 2021-02-24 01:34:32.000000 blaster-server-0.0.424b0/examples/tornado_hello_world.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      791 2021-02-24 01:20:44.000000 blaster-server-0.0.424b0/examples/wheezy_hello.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       79 2023-04-03 11:06:16.492416 blaster-server-0.0.424b0/setup.cfg
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1560 2023-04-02 09:24:19.000000 blaster-server-0.0.424b0/setup.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-03 11:06:16.492416 blaster-server-0.0.424b0/test/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2022-07-26 21:35:40.000000 blaster-server-0.0.424b0/test/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6851 2023-01-07 00:03:08.000000 blaster-server-0.0.424b0/test/test_mongo_orm.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      503 2022-11-07 18:31:41.000000 blaster-server-0.0.424b0/test/test_schema.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     5457 2022-12-09 21:19:51.000000 blaster-server-0.0.424b0/test/test_tools.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      345 2022-11-08 15:22:13.000000 blaster-server-0.0.424b0/test/test_utils.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      615 2021-02-24 11:15:27.000000 blaster-server-0.0.424b0/test/timeit_snippets.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-16 18:16:05.846692 blaster-server-0.0.425/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1061 2019-07-03 19:03:00.000000 blaster-server-0.0.425/LICENSE.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       38 2022-11-07 18:47:07.000000 blaster-server-0.0.425/MANIFEST.in
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      849 2023-04-16 18:16:05.846692 blaster-server-0.0.425/PKG-INFO
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     2620 2022-11-14 12:45:11.000000 blaster-server-0.0.425/README.md
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2021-10-05 11:27:02.000000 blaster-server-0.0.425/__init__.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-16 18:16:05.842692 blaster-server-0.0.425/blaster/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      875 2023-01-09 13:10:46.000000 blaster-server-0.0.425/blaster/__init__.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-16 18:16:05.842692 blaster-server-0.0.425/blaster/cloud/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       51 2022-11-09 17:29:08.000000 blaster-server-0.0.425/blaster/cloud/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3257 2022-12-03 12:42:35.000000 blaster-server-0.0.425/blaster/cloud/analytics.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-16 18:16:05.842692 blaster-server-0.0.425/blaster/cloud/aws/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       78 2019-07-03 19:03:00.000000 blaster-server-0.0.425/blaster/cloud/aws/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1371 2022-12-01 11:30:06.000000 blaster-server-0.0.425/blaster/cloud/aws/ses_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5230 2023-01-28 12:53:32.000000 blaster-server-0.0.425/blaster/cloud/push_tasks.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3729 2023-03-23 02:32:10.000000 blaster-server-0.0.425/blaster/cloud/storage.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3796 2023-03-06 12:38:58.000000 blaster-server-0.0.425/blaster/config.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3715 2023-01-28 12:57:17.000000 blaster-server-0.0.425/blaster/connection_pool.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       99 2020-11-22 14:37:38.000000 blaster-server-0.0.425/blaster/constants.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5290 2023-03-30 07:56:48.000000 blaster-server-0.0.425/blaster/logging.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    62615 2023-04-15 22:13:28.000000 blaster-server-0.0.425/blaster/mongo_orm.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    14954 2023-03-22 22:32:18.000000 blaster-server-0.0.425/blaster/schema.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    36521 2023-04-03 11:05:37.000000 blaster-server-0.0.425/blaster/server.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    46829 2023-04-03 00:57:53.000000 blaster-server-0.0.425/blaster/tools.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-16 18:16:05.842692 blaster-server-0.0.425/blaster/utils/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2019-07-03 19:03:00.000000 blaster-server-0.0.425/blaster/utils/__init__.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-16 18:16:05.842692 blaster-server-0.0.425/blaster/utils/data/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    53078 2022-11-08 15:22:07.000000 blaster-server-0.0.425/blaster/utils/data/countries.json
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)   119011 2022-12-01 10:20:50.000000 blaster-server-0.0.425/blaster/utils/data/mime_types.json
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     7087 2023-04-16 18:10:42.000000 blaster-server-0.0.425/blaster/utils/data_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1951 2023-01-07 12:42:21.000000 blaster-server-0.0.425/blaster/utils/events.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     4812 2023-03-30 16:36:26.000000 blaster-server-0.0.425/blaster/utils/fork.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1076 2023-02-21 07:52:48.000000 blaster-server-0.0.425/blaster/utils/lat_long_utils.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     5552 2023-02-01 17:01:50.000000 blaster-server-0.0.425/blaster/utils/phone_number_utils.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     6773 2020-12-14 07:56:42.000000 blaster-server-0.0.425/blaster/utils/xss_html.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-16 18:16:05.842692 blaster-server-0.0.425/blaster/websocket/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1022 2019-07-03 19:03:00.000000 blaster-server-0.0.425/blaster/websocket/__init__.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    12874 2019-07-03 19:03:00.000000 blaster-server-0.0.425/blaster/websocket/_abnf.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    11136 2022-01-06 11:42:20.000000 blaster-server-0.0.425/blaster/websocket/_app.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    16360 2019-07-03 19:03:00.000000 blaster-server-0.0.425/blaster/websocket/_core.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     2141 2019-07-03 19:03:00.000000 blaster-server-0.0.425/blaster/websocket/_exceptions.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     4793 2019-07-03 19:03:00.000000 blaster-server-0.0.425/blaster/websocket/_handshake.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     7288 2019-07-03 19:03:00.000000 blaster-server-0.0.425/blaster/websocket/_http.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1870 2019-07-03 19:03:00.000000 blaster-server-0.0.425/blaster/websocket/_logging.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     3623 2019-07-03 19:03:00.000000 blaster-server-0.0.425/blaster/websocket/_socket.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1550 2019-07-03 19:03:00.000000 blaster-server-0.0.425/blaster/websocket/_ssl_compat.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     3670 2019-07-03 19:03:00.000000 blaster-server-0.0.425/blaster/websocket/_url.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     3632 2019-07-03 19:03:00.000000 blaster-server-0.0.425/blaster/websocket/_utils.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    12758 2021-10-03 12:23:56.000000 blaster-server-0.0.425/blaster/websocket/server.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-16 18:16:05.842692 blaster-server-0.0.425/blaster/websocket/tests/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2019-07-03 19:03:00.000000 blaster-server-0.0.425/blaster/websocket/tests/__init__.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    26115 2019-07-03 19:03:00.000000 blaster-server-0.0.425/blaster/websocket/tests/test_websocket.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-16 18:16:05.842692 blaster-server-0.0.425/blaster_server.egg-info/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      849 2023-04-16 18:16:05.000000 blaster-server-0.0.425/blaster_server.egg-info/PKG-INFO
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1682 2023-04-16 18:16:05.000000 blaster-server-0.0.425/blaster_server.egg-info/SOURCES.txt
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        1 2023-04-16 18:16:05.000000 blaster-server-0.0.425/blaster_server.egg-info/dependency_links.txt
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      221 2023-04-16 18:16:05.000000 blaster-server-0.0.425/blaster_server.egg-info/requires.txt
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       41 2023-04-16 18:16:05.000000 blaster-server-0.0.425/blaster_server.egg-info/top_level.txt
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-16 18:16:05.842692 blaster-server-0.0.425/examples/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2019-07-03 19:03:00.000000 blaster-server-0.0.425/examples/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      266 2022-01-06 11:42:20.000000 blaster-server-0.0.425/examples/fast_api_test.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      636 2019-07-03 19:03:00.000000 blaster-server-0.0.425/examples/gevent_wsgi_test.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      233 2021-10-04 14:48:01.000000 blaster-server-0.0.425/examples/meinheld_flask.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1743 2022-06-17 17:10:40.000000 blaster-server-0.0.425/examples/mongo_ormexample.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2386 2022-11-14 12:13:43.000000 blaster-server-0.0.425/examples/simple_examples.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1088 2019-07-03 19:03:00.000000 blaster-server-0.0.425/examples/test_chat_room.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      614 2021-02-24 01:34:32.000000 blaster-server-0.0.425/examples/tornado_hello_world.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      791 2021-02-24 01:20:44.000000 blaster-server-0.0.425/examples/wheezy_hello.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       79 2023-04-16 18:16:05.846692 blaster-server-0.0.425/setup.cfg
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1559 2023-04-16 17:58:45.000000 blaster-server-0.0.425/setup.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-16 18:16:05.846692 blaster-server-0.0.425/test/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2022-07-26 21:35:40.000000 blaster-server-0.0.425/test/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6851 2023-01-07 00:03:08.000000 blaster-server-0.0.425/test/test_mongo_orm.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      503 2022-11-07 18:31:41.000000 blaster-server-0.0.425/test/test_schema.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     5457 2022-12-09 21:19:51.000000 blaster-server-0.0.425/test/test_tools.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      791 2023-04-16 18:15:30.000000 blaster-server-0.0.425/test/test_utils.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      615 2021-02-24 11:15:27.000000 blaster-server-0.0.425/test/timeit_snippets.py
```

### Comparing `blaster-server-0.0.424b0/LICENSE.txt` & `blaster-server-0.0.425/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.424b0/PKG-INFO` & `blaster-server-0.0.425/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blaster-server
-Version: 0.0.424b0
+Version: 0.0.425
 Summary: Gevent based python server built from scratch for maximum performance
 Home-page: https://github.com/abhinavabcd/blaster
 Author: Abhinav Reddy
 Author-email: abhinavabcd@gmail.com
 License: MIT
 Download-URL: https://github.com/abhinavabcd/blaster/archive/v0.0337b.tar.gz
 Keywords: server,superfast,Like FastApi or Flask but 10x faster
```

### Comparing `blaster-server-0.0.424b0/README.md` & `blaster-server-0.0.425/README.md`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.424b0/blaster/__init__.py` & `blaster-server-0.0.425/blaster/__init__.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.424b0/blaster/cloud/analytics.py` & `blaster-server-0.0.425/blaster/cloud/analytics.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.424b0/blaster/cloud/aws/ses_utils.py` & `blaster-server-0.0.425/blaster/cloud/aws/ses_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.424b0/blaster/cloud/push_tasks.py` & `blaster-server-0.0.425/blaster/cloud/push_tasks.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.424b0/blaster/cloud/storage.py` & `blaster-server-0.0.425/blaster/cloud/storage.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.424b0/blaster/config.py` & `blaster-server-0.0.425/blaster/config.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.424b0/blaster/connection_pool.py` & `blaster-server-0.0.425/blaster/connection_pool.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.424b0/blaster/logging.py` & `blaster-server-0.0.425/blaster/logging.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.424b0/blaster/mongo_orm.py` & `blaster-server-0.0.425/blaster/mongo_orm.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,16 @@
 		super(MongoList, self).remove(item)
 		_pull = self._model_obj._other_query_updates.get("$pull")
 		if(_pull == None):
 			self._model_obj._other_query_updates["$pull"] = _pull = {}
 		value_to_remove = _pull.get(self.path, _OBJ_END_)
 		if(value_to_remove == _OBJ_END_):
 			_pull[self.path] = item  # first item to remove
-		else:
+		else: 
+			# if there are multiple items to remove, use $in
 			if(
 				isinstance(value_to_remove, dict)
 				and "$in" in value_to_remove
 			):
 				_pull[self.path]["$in"].append(item)
 			else:
 				_pull[self.path] = {"$in": [value_to_remove, item]}
```

### Comparing `blaster-server-0.0.424b0/blaster/schema.py` & `blaster-server-0.0.425/blaster/schema.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.424b0/blaster/server.py` & `blaster-server-0.0.425/blaster/server.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.424b0/blaster/tools.py` & `blaster-server-0.0.425/blaster/tools.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.424b0/blaster/utils/data/countries.json` & `blaster-server-0.0.425/blaster/utils/data/countries.json`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.424b0/blaster/utils/data/mime_types.json` & `blaster-server-0.0.425/blaster/utils/data/mime_types.json`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.424b0/blaster/utils/data_utils.py` & `blaster-server-0.0.425/blaster/utils/data_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -61,47 +61,55 @@
 		return val
 	return f * (val / f + 1)
 
 
 '''
 	return UNITS (current absolute app units value), CURRENCY_CODE, VALUE_IN_CURRENCY_CODE
 '''
-NUM_REGEX = re.compile(r'[+-.]?[0-9]+(?:\.[0-9]+)?')
+NUM_REGEX = re.compile(r'[+-.]?[0-9][0-9,]*(?:\.[0-9]+)?')
 def parse_currency_string(currency_str, default_currency_code=DEFAULT_CURRENCY_CODE, country_code=None):
 	val = NUM_REGEX.findall(currency_str)
 	if(not val):
 		return 0, default_currency_code, 0
 
-	val = val[0]
-	currency_code = currency_str.replace(val, "").strip().upper()
+	val_str = val[0]
+	currency_code = None
+	if(_curreny_code := currency_str.replace(val_str, " ").split()):
+		currency_code = _curreny_code[0].upper()
+	val = val_str.replace(",", "")  # remove commas
 	if(not currency_code):
 		if(country_code):
 			currency_code = COUNTRY_DATA[country_code]["currency_code"]
 
 	if(not currency_code or currency_code not in INR_EXCHANGE_RATE): # if invalid currency set to default
 		currency_code = default_currency_code
 
 	if(val[0] == "."):
 		val = "0." + val[1:].replace(".", "", 1)
 
-	val = float(val) # convert str to float
+	val = float(val)  # convert str to float
 	return int(val * 1000 * INR_EXCHANGE_RATE[currency_code]), currency_code, val
 
 
 def convert_currency(val, from_currency='APP_CURRENCY', to_currency='INR'):
 	# val / from_currency_inr_exchange -> inr  then multiply to_exchange rate 
-	return (val *  INR_EXCHANGE_RATE[to_currency.upper()]) / INR_EXCHANGE_RATE[from_currency.upper()]
+	return (val * INR_EXCHANGE_RATE[to_currency.upper()]) / INR_EXCHANGE_RATE[from_currency.upper()]
 
 
 # simply parse number , units
 def parse_string_to_units(full_str, default_unit="EUR"):
 	val = NUM_REGEX.findall(full_str)
 	if(not val):
 		return 0, default_unit
 
-	units_value = val[0]
-	units_code = full_str.replace(units_value, "").strip() or default_unit
+	val_str = val[0]
+	units_code = None
+	if(_units_code := full_str.replace(val_str, " ").split()):
+		units_code = _units_code[0]
+	units_code = units_code or default_unit
+
+	units_value = val_str.replace(",", "")  # remove any commas
 
 	if(units_value[0] == "."):
 		units_value = "0." + units_value[1:].replace(".", "", 1)
 
 	return float(units_value), units_code
```

### Comparing `blaster-server-0.0.424b0/blaster/utils/events.py` & `blaster-server-0.0.425/blaster/utils/events.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.424b0/blaster/utils/fork.py` & `blaster-server-0.0.425/blaster/utils/fork.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.424b0/blaster/utils/lat_long_utils.py` & `blaster-server-0.0.425/blaster/utils/lat_long_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.424b0/blaster/utils/phone_number_utils.py` & `blaster-server-0.0.425/blaster/utils/phone_number_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.424b0/blaster/utils/xss_html.py` & `blaster-server-0.0.425/blaster/utils/xss_html.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.424b0/blaster/websocket/__init__.py` & `blaster-server-0.0.425/blaster/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.424b0/blaster/websocket/_abnf.py` & `blaster-server-0.0.425/blaster/websocket/_abnf.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.424b0/blaster/websocket/_app.py` & `blaster-server-0.0.425/blaster/websocket/_app.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.424b0/blaster/websocket/_core.py` & `blaster-server-0.0.425/blaster/websocket/_core.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.424b0/blaster/websocket/_exceptions.py` & `blaster-server-0.0.425/blaster/websocket/_exceptions.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.424b0/blaster/websocket/_handshake.py` & `blaster-server-0.0.425/blaster/websocket/_handshake.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.424b0/blaster/websocket/_http.py` & `blaster-server-0.0.425/blaster/websocket/_http.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.424b0/blaster/websocket/_logging.py` & `blaster-server-0.0.425/blaster/websocket/_logging.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.424b0/blaster/websocket/_socket.py` & `blaster-server-0.0.425/blaster/websocket/_socket.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.424b0/blaster/websocket/_ssl_compat.py` & `blaster-server-0.0.425/blaster/websocket/_ssl_compat.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.424b0/blaster/websocket/_url.py` & `blaster-server-0.0.425/blaster/websocket/_url.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.424b0/blaster/websocket/_utils.py` & `blaster-server-0.0.425/blaster/websocket/_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.424b0/blaster/websocket/server.py` & `blaster-server-0.0.425/blaster/websocket/server.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.424b0/blaster/websocket/tests/test_websocket.py` & `blaster-server-0.0.425/blaster/websocket/tests/test_websocket.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.424b0/blaster_server.egg-info/PKG-INFO` & `blaster-server-0.0.425/blaster_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blaster-server
-Version: 0.0.424b0
+Version: 0.0.425
 Summary: Gevent based python server built from scratch for maximum performance
 Home-page: https://github.com/abhinavabcd/blaster
 Author: Abhinav Reddy
 Author-email: abhinavabcd@gmail.com
 License: MIT
 Download-URL: https://github.com/abhinavabcd/blaster/archive/v0.0337b.tar.gz
 Keywords: server,superfast,Like FastApi or Flask but 10x faster
```

### Comparing `blaster-server-0.0.424b0/blaster_server.egg-info/SOURCES.txt` & `blaster-server-0.0.425/blaster_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.424b0/examples/gevent_wsgi_test.py` & `blaster-server-0.0.425/examples/gevent_wsgi_test.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.424b0/examples/mongo_ormexample.py` & `blaster-server-0.0.425/examples/mongo_ormexample.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.424b0/examples/simple_examples.py` & `blaster-server-0.0.425/examples/simple_examples.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.424b0/examples/test_chat_room.py` & `blaster-server-0.0.425/examples/test_chat_room.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.424b0/examples/tornado_hello_world.py` & `blaster-server-0.0.425/examples/tornado_hello_world.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.424b0/examples/wheezy_hello.py` & `blaster-server-0.0.425/examples/wheezy_hello.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.424b0/setup.py` & `blaster-server-0.0.425/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
 	name='blaster-server',
 	packages=find_packages() + ["blaster/utils/data"],
-	version='0.0.424b',
+	version='0.0.425',
 	license='MIT',
 	description='Gevent based python server built from scratch for maximum performance',
 	author='Abhinav Reddy',                   # Type in your name
 	author_email='abhinavabcd@gmail.com',      # Type in your E-Mail
 	url='https://github.com/abhinavabcd/blaster',
 	download_url='https://github.com/abhinavabcd/blaster/archive/v0.0337b.tar.gz',
 	keywords=['server', 'superfast', 'Like FastApi or Flask but 10x faster'],
```

### Comparing `blaster-server-0.0.424b0/test/test_mongo_orm.py` & `blaster-server-0.0.425/test/test_mongo_orm.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.424b0/test/test_tools.py` & `blaster-server-0.0.425/test/test_tools.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.424b0/test/timeit_snippets.py` & `blaster-server-0.0.425/test/timeit_snippets.py`

 * *Files identical despite different names*

