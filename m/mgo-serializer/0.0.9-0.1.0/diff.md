# Comparing `tmp/mgo_serializer-0.0.9.tar.gz` & `tmp/mgo_serializer-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mgo_serializer-0.0.9.tar", last modified: Mon Apr 18 07:45:28 2022, max compression
+gzip compressed data, was "mgo_serializer-0.1.0.tar", last modified: Sun Apr 16 09:32:41 2023, max compression
```

## Comparing `mgo_serializer-0.0.9.tar` & `mgo_serializer-0.1.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 mosydev   (1000) mosydev   (1000)        0 2022-04-18 07:45:28.971658 mgo_serializer-0.0.9/
--rw-r--r--   0 mosydev   (1000) mosydev   (1000)      420 2022-04-18 07:45:28.971658 mgo_serializer-0.0.9/PKG-INFO
--rwxrwxrwx   0 mosydev   (1000) mosydev   (1000)      146 2022-04-06 08:39:36.000000 mgo_serializer-0.0.9/README.md
-drwxr-xr-x   0 mosydev   (1000) mosydev   (1000)        0 2022-04-18 07:45:28.964991 mgo_serializer-0.0.9/common/
--rw-r--r--   0 mosydev   (1000) mosydev   (1000)        0 2022-04-10 11:10:32.000000 mgo_serializer-0.0.9/common/__init__.py
-drwxr-xr-x   0 mosydev   (1000) mosydev   (1000)        0 2022-04-18 07:45:28.964991 mgo_serializer-0.0.9/common/api/
--rw-r--r--   0 mosydev   (1000) mosydev   (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.0.9/common/api/__init__.py
-drwxr-xr-x   0 mosydev   (1000) mosydev   (1000)        0 2022-04-18 07:45:28.964991 mgo_serializer-0.0.9/common/api/services/
--rw-r--r--   0 mosydev   (1000) mosydev   (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.0.9/common/api/services/__init__.py
-drwxr-xr-x   0 mosydev   (1000) mosydev   (1000)        0 2022-04-18 07:45:28.964991 mgo_serializer-0.0.9/common/api/services/account/
--rw-r--r--   0 mosydev   (1000) mosydev   (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.0.9/common/api/services/account/__init__.py
--rw-r--r--   0 mosydev   (1000) mosydev   (1000)    32911 2022-04-10 11:11:53.000000 mgo_serializer-0.0.9/common/api/services/account/account_pb2.py
--rw-r--r--   0 mosydev   (1000) mosydev   (1000)   114804 2022-04-10 11:11:53.000000 mgo_serializer-0.0.9/common/api/services/account/account_pb2_grpc.py
-drwxr-xr-x   0 mosydev   (1000) mosydev   (1000)        0 2022-04-18 07:45:28.964991 mgo_serializer-0.0.9/common/api/services/common/
--rw-r--r--   0 mosydev   (1000) mosydev   (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.0.9/common/api/services/common/__init__.py
--rw-r--r--   0 mosydev   (1000) mosydev   (1000)     9632 2022-04-10 11:11:53.000000 mgo_serializer-0.0.9/common/api/services/common/common_pb2.py
--rw-r--r--   0 mosydev   (1000) mosydev   (1000)      159 2022-04-10 11:11:53.000000 mgo_serializer-0.0.9/common/api/services/common/common_pb2_grpc.py
-drwxr-xr-x   0 mosydev   (1000) mosydev   (1000)        0 2022-04-18 07:45:28.964991 mgo_serializer-0.0.9/common/api/services/discussion/
--rw-r--r--   0 mosydev   (1000) mosydev   (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.0.9/common/api/services/discussion/__init__.py
--rw-r--r--   0 mosydev   (1000) mosydev   (1000)     5389 2022-04-10 11:11:53.000000 mgo_serializer-0.0.9/common/api/services/discussion/discussion_pb2.py
--rw-r--r--   0 mosydev   (1000) mosydev   (1000)    19113 2022-04-10 11:11:53.000000 mgo_serializer-0.0.9/common/api/services/discussion/discussion_pb2_grpc.py
-drwxr-xr-x   0 mosydev   (1000) mosydev   (1000)        0 2022-04-18 07:45:28.968324 mgo_serializer-0.0.9/common/api/services/explore/
--rw-r--r--   0 mosydev   (1000) mosydev   (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.0.9/common/api/services/explore/__init__.py
--rw-r--r--   0 mosydev   (1000) mosydev   (1000)     3100 2022-04-10 11:11:53.000000 mgo_serializer-0.0.9/common/api/services/explore/explore_pb2.py
--rw-r--r--   0 mosydev   (1000) mosydev   (1000)     6027 2022-04-10 11:11:53.000000 mgo_serializer-0.0.9/common/api/services/explore/explore_pb2_grpc.py
-drwxr-xr-x   0 mosydev   (1000) mosydev   (1000)        0 2022-04-18 07:45:28.968324 mgo_serializer-0.0.9/common/api/services/hashtag/
--rw-r--r--   0 mosydev   (1000) mosydev   (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.0.9/common/api/services/hashtag/__init__.py
--rw-r--r--   0 mosydev   (1000) mosydev   (1000)     6160 2022-04-10 11:11:53.000000 mgo_serializer-0.0.9/common/api/services/hashtag/hashtag_pb2.py
--rw-r--r--   0 mosydev   (1000) mosydev   (1000)    14342 2022-04-10 11:11:53.000000 mgo_serializer-0.0.9/common/api/services/hashtag/hashtag_pb2_grpc.py
-drwxr-xr-x   0 mosydev   (1000) mosydev   (1000)        0 2022-04-18 07:45:28.968324 mgo_serializer-0.0.9/common/api/services/history/
--rw-r--r--   0 mosydev   (1000) mosydev   (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.0.9/common/api/services/history/__init__.py
--rw-r--r--   0 mosydev   (1000) mosydev   (1000)     4696 2022-04-10 11:11:53.000000 mgo_serializer-0.0.9/common/api/services/history/history_pb2.py
--rw-r--r--   0 mosydev   (1000) mosydev   (1000)     5873 2022-04-10 11:11:53.000000 mgo_serializer-0.0.9/common/api/services/history/history_pb2_grpc.py
-drwxr-xr-x   0 mosydev   (1000) mosydev   (1000)        0 2022-04-18 07:45:28.968324 mgo_serializer-0.0.9/common/api/services/mention/
--rw-r--r--   0 mosydev   (1000) mosydev   (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.0.9/common/api/services/mention/__init__.py
--rw-r--r--   0 mosydev   (1000) mosydev   (1000)     2302 2022-04-10 11:11:53.000000 mgo_serializer-0.0.9/common/api/services/mention/mention_pb2.py
--rw-r--r--   0 mosydev   (1000) mosydev   (1000)     6322 2022-04-10 11:11:53.000000 mgo_serializer-0.0.9/common/api/services/mention/mention_pb2_grpc.py
-drwxr-xr-x   0 mosydev   (1000) mosydev   (1000)        0 2022-04-18 07:45:28.968324 mgo_serializer-0.0.9/common/api/services/post/
--rw-r--r--   0 mosydev   (1000) mosydev   (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.0.9/common/api/services/post/__init__.py
--rw-r--r--   0 mosydev   (1000) mosydev   (1000)    11421 2022-04-10 11:11:53.000000 mgo_serializer-0.0.9/common/api/services/post/post_pb2.py
--rw-r--r--   0 mosydev   (1000) mosydev   (1000)    39890 2022-04-10 11:11:53.000000 mgo_serializer-0.0.9/common/api/services/post/post_pb2_grpc.py
-drwxr-xr-x   0 mosydev   (1000) mosydev   (1000)        0 2022-04-18 07:45:28.968324 mgo_serializer-0.0.9/common/api/services/product/
--rw-r--r--   0 mosydev   (1000) mosydev   (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.0.9/common/api/services/product/__init__.py
--rw-r--r--   0 mosydev   (1000) mosydev   (1000)    32899 2022-04-10 11:11:53.000000 mgo_serializer-0.0.9/common/api/services/product/product_pb2.py
--rw-r--r--   0 mosydev   (1000) mosydev   (1000)    86544 2022-04-10 11:11:53.000000 mgo_serializer-0.0.9/common/api/services/product/product_pb2_grpc.py
-drwxr-xr-x   0 mosydev   (1000) mosydev   (1000)        0 2022-04-18 07:45:28.968324 mgo_serializer-0.0.9/common/api/services/shop/
--rw-r--r--   0 mosydev   (1000) mosydev   (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.0.9/common/api/services/shop/__init__.py
--rw-r--r--   0 mosydev   (1000) mosydev   (1000)    45403 2022-04-10 11:11:53.000000 mgo_serializer-0.0.9/common/api/services/shop/shop_pb2.py
--rw-r--r--   0 mosydev   (1000) mosydev   (1000)    74160 2022-04-10 11:11:53.000000 mgo_serializer-0.0.9/common/api/services/shop/shop_pb2_grpc.py
-drwxr-xr-x   0 mosydev   (1000) mosydev   (1000)        0 2022-04-18 07:45:28.971658 mgo_serializer-0.0.9/common/api/services/stats/
--rw-r--r--   0 mosydev   (1000) mosydev   (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.0.9/common/api/services/stats/__init__.py
--rw-r--r--   0 mosydev   (1000) mosydev   (1000)     4291 2022-04-10 11:11:53.000000 mgo_serializer-0.0.9/common/api/services/stats/stats_pb2.py
--rw-r--r--   0 mosydev   (1000) mosydev   (1000)     9050 2022-04-10 11:11:53.000000 mgo_serializer-0.0.9/common/api/services/stats/stats_pb2_grpc.py
-drwxr-xr-x   0 mosydev   (1000) mosydev   (1000)        0 2022-04-18 07:45:28.971658 mgo_serializer-0.0.9/common/api/services/story/
--rw-r--r--   0 mosydev   (1000) mosydev   (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.0.9/common/api/services/story/__init__.py
--rw-r--r--   0 mosydev   (1000) mosydev   (1000)     7304 2022-04-10 11:11:53.000000 mgo_serializer-0.0.9/common/api/services/story/story_pb2.py
--rw-r--r--   0 mosydev   (1000) mosydev   (1000)    15700 2022-04-10 11:11:53.000000 mgo_serializer-0.0.9/common/api/services/story/story_pb2_grpc.py
-drwxr-xr-x   0 mosydev   (1000) mosydev   (1000)        0 2022-04-18 07:45:28.971658 mgo_serializer-0.0.9/mgo_serializer/
--rwxrwxrwx   0 mosydev   (1000) mosydev   (1000)      104 2022-04-06 08:10:46.000000 mgo_serializer-0.0.9/mgo_serializer/__init__.py
--rwxrwxrwx   0 mosydev   (1000) mosydev   (1000)      105 2022-04-13 13:25:29.000000 mgo_serializer-0.0.9/mgo_serializer/exceptions.py
--rwxrwxrwx   0 mosydev   (1000) mosydev   (1000)    16239 2022-04-18 07:40:08.000000 mgo_serializer-0.0.9/mgo_serializer/fields.py
--rwxrwxrwx   0 mosydev   (1000) mosydev   (1000)     4894 2022-04-09 12:15:08.000000 mgo_serializer-0.0.9/mgo_serializer/helpers.py
--rwxrwxrwx   0 mosydev   (1000) mosydev   (1000)     1498 2022-04-06 08:02:56.000000 mgo_serializer-0.0.9/mgo_serializer/meta.py
--rwxrwxrwx   0 mosydev   (1000) mosydev   (1000)    12734 2022-04-18 07:41:35.000000 mgo_serializer-0.0.9/mgo_serializer/serializer.py
--rwxrwxrwx   0 mosydev   (1000) mosydev   (1000)      837 2022-04-06 08:02:56.000000 mgo_serializer-0.0.9/mgo_serializer/utils.py
-drwxr-xr-x   0 mosydev   (1000) mosydev   (1000)        0 2022-04-18 07:45:28.971658 mgo_serializer-0.0.9/mgo_serializer.egg-info/
--rw-r--r--   0 mosydev   (1000) mosydev   (1000)      420 2022-04-18 07:45:28.000000 mgo_serializer-0.0.9/mgo_serializer.egg-info/PKG-INFO
--rw-r--r--   0 mosydev   (1000) mosydev   (1000)     1969 2022-04-18 07:45:28.000000 mgo_serializer-0.0.9/mgo_serializer.egg-info/SOURCES.txt
--rw-r--r--   0 mosydev   (1000) mosydev   (1000)        1 2022-04-18 07:45:28.000000 mgo_serializer-0.0.9/mgo_serializer.egg-info/dependency_links.txt
--rw-r--r--   0 mosydev   (1000) mosydev   (1000)       22 2022-04-18 07:45:28.000000 mgo_serializer-0.0.9/mgo_serializer.egg-info/top_level.txt
--rwxrwxrwx   0 mosydev   (1000) mosydev   (1000)       79 2022-04-18 07:45:28.971658 mgo_serializer-0.0.9/setup.cfg
--rwxrwxrwx   0 mosydev   (1000) mosydev   (1000)      528 2022-04-18 07:45:07.000000 mgo_serializer-0.0.9/setup.py
+drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-16 09:32:41.033725 mgo_serializer-0.1.0/
+-rw-r--r--   0 hydra     (1000) hydra     (1000)      392 2023-04-16 09:32:41.033725 mgo_serializer-0.1.0/PKG-INFO
+-rwxrwxrwx   0 hydra     (1000) hydra     (1000)      146 2022-04-06 08:39:36.000000 mgo_serializer-0.1.0/README.md
+drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-16 09:32:41.030392 mgo_serializer-0.1.0/common/
+-rw-r--r--   0 hydra     (1000) hydra     (1000)        0 2022-04-10 11:10:32.000000 mgo_serializer-0.1.0/common/__init__.py
+drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-16 09:32:41.030392 mgo_serializer-0.1.0/common/api/
+-rw-r--r--   0 hydra     (1000) hydra     (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.1.0/common/api/__init__.py
+drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-16 09:32:41.030392 mgo_serializer-0.1.0/common/api/services/
+-rw-r--r--   0 hydra     (1000) hydra     (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.1.0/common/api/services/__init__.py
+drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-16 09:32:41.030392 mgo_serializer-0.1.0/common/api/services/account/
+-rw-r--r--   0 hydra     (1000) hydra     (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.1.0/common/api/services/account/__init__.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)    32911 2022-04-10 11:11:53.000000 mgo_serializer-0.1.0/common/api/services/account/account_pb2.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)   114804 2022-04-10 11:11:53.000000 mgo_serializer-0.1.0/common/api/services/account/account_pb2_grpc.py
+drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-16 09:32:41.030392 mgo_serializer-0.1.0/common/api/services/common/
+-rw-r--r--   0 hydra     (1000) hydra     (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.1.0/common/api/services/common/__init__.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)     9632 2022-04-10 11:11:53.000000 mgo_serializer-0.1.0/common/api/services/common/common_pb2.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)      159 2022-04-10 11:11:53.000000 mgo_serializer-0.1.0/common/api/services/common/common_pb2_grpc.py
+drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-16 09:32:41.030392 mgo_serializer-0.1.0/common/api/services/discussion/
+-rw-r--r--   0 hydra     (1000) hydra     (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.1.0/common/api/services/discussion/__init__.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)     5389 2022-04-10 11:11:53.000000 mgo_serializer-0.1.0/common/api/services/discussion/discussion_pb2.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)    19113 2022-04-10 11:11:53.000000 mgo_serializer-0.1.0/common/api/services/discussion/discussion_pb2_grpc.py
+drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-16 09:32:41.030392 mgo_serializer-0.1.0/common/api/services/explore/
+-rw-r--r--   0 hydra     (1000) hydra     (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.1.0/common/api/services/explore/__init__.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)     3100 2022-04-10 11:11:53.000000 mgo_serializer-0.1.0/common/api/services/explore/explore_pb2.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)     6027 2022-04-10 11:11:53.000000 mgo_serializer-0.1.0/common/api/services/explore/explore_pb2_grpc.py
+drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-16 09:32:41.030392 mgo_serializer-0.1.0/common/api/services/hashtag/
+-rw-r--r--   0 hydra     (1000) hydra     (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.1.0/common/api/services/hashtag/__init__.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)     6160 2022-04-10 11:11:53.000000 mgo_serializer-0.1.0/common/api/services/hashtag/hashtag_pb2.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)    14342 2022-04-10 11:11:53.000000 mgo_serializer-0.1.0/common/api/services/hashtag/hashtag_pb2_grpc.py
+drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-16 09:32:41.030392 mgo_serializer-0.1.0/common/api/services/history/
+-rw-r--r--   0 hydra     (1000) hydra     (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.1.0/common/api/services/history/__init__.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)     4696 2022-04-10 11:11:53.000000 mgo_serializer-0.1.0/common/api/services/history/history_pb2.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)     5873 2022-04-10 11:11:53.000000 mgo_serializer-0.1.0/common/api/services/history/history_pb2_grpc.py
+drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-16 09:32:41.030392 mgo_serializer-0.1.0/common/api/services/mention/
+-rw-r--r--   0 hydra     (1000) hydra     (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.1.0/common/api/services/mention/__init__.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)     2302 2022-04-10 11:11:53.000000 mgo_serializer-0.1.0/common/api/services/mention/mention_pb2.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)     6322 2022-04-10 11:11:53.000000 mgo_serializer-0.1.0/common/api/services/mention/mention_pb2_grpc.py
+drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-16 09:32:41.030392 mgo_serializer-0.1.0/common/api/services/post/
+-rw-r--r--   0 hydra     (1000) hydra     (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.1.0/common/api/services/post/__init__.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)    11421 2022-04-10 11:11:53.000000 mgo_serializer-0.1.0/common/api/services/post/post_pb2.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)    39890 2022-04-10 11:11:53.000000 mgo_serializer-0.1.0/common/api/services/post/post_pb2_grpc.py
+drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-16 09:32:41.030392 mgo_serializer-0.1.0/common/api/services/product/
+-rw-r--r--   0 hydra     (1000) hydra     (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.1.0/common/api/services/product/__init__.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)    32899 2022-04-10 11:11:53.000000 mgo_serializer-0.1.0/common/api/services/product/product_pb2.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)    86544 2022-04-10 11:11:53.000000 mgo_serializer-0.1.0/common/api/services/product/product_pb2_grpc.py
+drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-16 09:32:41.033725 mgo_serializer-0.1.0/common/api/services/shop/
+-rw-r--r--   0 hydra     (1000) hydra     (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.1.0/common/api/services/shop/__init__.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)    45403 2022-04-10 11:11:53.000000 mgo_serializer-0.1.0/common/api/services/shop/shop_pb2.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)    74160 2022-04-10 11:11:53.000000 mgo_serializer-0.1.0/common/api/services/shop/shop_pb2_grpc.py
+drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-16 09:32:41.033725 mgo_serializer-0.1.0/common/api/services/stats/
+-rw-r--r--   0 hydra     (1000) hydra     (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.1.0/common/api/services/stats/__init__.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)     4291 2022-04-10 11:11:53.000000 mgo_serializer-0.1.0/common/api/services/stats/stats_pb2.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)     9050 2022-04-10 11:11:53.000000 mgo_serializer-0.1.0/common/api/services/stats/stats_pb2_grpc.py
+drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-16 09:32:41.033725 mgo_serializer-0.1.0/common/api/services/story/
+-rw-r--r--   0 hydra     (1000) hydra     (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.1.0/common/api/services/story/__init__.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)     7304 2022-04-10 11:11:53.000000 mgo_serializer-0.1.0/common/api/services/story/story_pb2.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)    15700 2022-04-10 11:11:53.000000 mgo_serializer-0.1.0/common/api/services/story/story_pb2_grpc.py
+drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-16 09:32:41.033725 mgo_serializer-0.1.0/mgo_serializer/
+-rwxrwxrwx   0 hydra     (1000) hydra     (1000)      104 2022-04-06 08:10:46.000000 mgo_serializer-0.1.0/mgo_serializer/__init__.py
+-rwxrwxrwx   0 hydra     (1000) hydra     (1000)      105 2022-04-13 13:25:29.000000 mgo_serializer-0.1.0/mgo_serializer/exceptions.py
+-rwxrwxrwx   0 hydra     (1000) hydra     (1000)    15874 2022-05-10 10:16:22.000000 mgo_serializer-0.1.0/mgo_serializer/fields.py
+-rwxrwxrwx   0 hydra     (1000) hydra     (1000)     4894 2022-05-11 09:53:09.000000 mgo_serializer-0.1.0/mgo_serializer/helpers.py
+-rwxrwxrwx   0 hydra     (1000) hydra     (1000)     1498 2022-04-06 08:02:56.000000 mgo_serializer-0.1.0/mgo_serializer/meta.py
+-rwxrwxrwx   0 hydra     (1000) hydra     (1000)    14670 2023-04-16 09:31:11.000000 mgo_serializer-0.1.0/mgo_serializer/serializer.py
+-rwxrwxrwx   0 hydra     (1000) hydra     (1000)      837 2022-04-06 08:02:56.000000 mgo_serializer-0.1.0/mgo_serializer/utils.py
+drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-16 09:32:41.033725 mgo_serializer-0.1.0/mgo_serializer.egg-info/
+-rw-r--r--   0 hydra     (1000) hydra     (1000)      392 2023-04-16 09:32:40.000000 mgo_serializer-0.1.0/mgo_serializer.egg-info/PKG-INFO
+-rw-r--r--   0 hydra     (1000) hydra     (1000)     1969 2023-04-16 09:32:41.000000 mgo_serializer-0.1.0/mgo_serializer.egg-info/SOURCES.txt
+-rw-r--r--   0 hydra     (1000) hydra     (1000)        1 2023-04-16 09:32:40.000000 mgo_serializer-0.1.0/mgo_serializer.egg-info/dependency_links.txt
+-rw-r--r--   0 hydra     (1000) hydra     (1000)       22 2023-04-16 09:32:40.000000 mgo_serializer-0.1.0/mgo_serializer.egg-info/top_level.txt
+-rwxrwxrwx   0 hydra     (1000) hydra     (1000)       79 2023-04-16 09:32:41.033725 mgo_serializer-0.1.0/setup.cfg
+-rwxrwxrwx   0 hydra     (1000) hydra     (1000)      528 2023-04-16 09:32:06.000000 mgo_serializer-0.1.0/setup.py
```

### Comparing `mgo_serializer-0.0.9/common/api/services/account/account_pb2.py` & `mgo_serializer-0.1.0/common/api/services/account/account_pb2.py`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.0.9/common/api/services/account/account_pb2_grpc.py` & `mgo_serializer-0.1.0/common/api/services/account/account_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.0.9/common/api/services/common/common_pb2.py` & `mgo_serializer-0.1.0/common/api/services/common/common_pb2.py`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.0.9/common/api/services/discussion/discussion_pb2.py` & `mgo_serializer-0.1.0/common/api/services/discussion/discussion_pb2.py`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.0.9/common/api/services/discussion/discussion_pb2_grpc.py` & `mgo_serializer-0.1.0/common/api/services/discussion/discussion_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.0.9/common/api/services/explore/explore_pb2.py` & `mgo_serializer-0.1.0/common/api/services/explore/explore_pb2.py`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.0.9/common/api/services/explore/explore_pb2_grpc.py` & `mgo_serializer-0.1.0/common/api/services/explore/explore_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.0.9/common/api/services/hashtag/hashtag_pb2.py` & `mgo_serializer-0.1.0/common/api/services/hashtag/hashtag_pb2.py`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.0.9/common/api/services/hashtag/hashtag_pb2_grpc.py` & `mgo_serializer-0.1.0/common/api/services/hashtag/hashtag_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.0.9/common/api/services/history/history_pb2.py` & `mgo_serializer-0.1.0/common/api/services/history/history_pb2.py`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.0.9/common/api/services/history/history_pb2_grpc.py` & `mgo_serializer-0.1.0/common/api/services/history/history_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.0.9/common/api/services/mention/mention_pb2.py` & `mgo_serializer-0.1.0/common/api/services/mention/mention_pb2.py`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.0.9/common/api/services/mention/mention_pb2_grpc.py` & `mgo_serializer-0.1.0/common/api/services/mention/mention_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.0.9/common/api/services/post/post_pb2.py` & `mgo_serializer-0.1.0/common/api/services/post/post_pb2.py`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.0.9/common/api/services/post/post_pb2_grpc.py` & `mgo_serializer-0.1.0/common/api/services/post/post_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.0.9/common/api/services/product/product_pb2.py` & `mgo_serializer-0.1.0/common/api/services/product/product_pb2.py`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.0.9/common/api/services/product/product_pb2_grpc.py` & `mgo_serializer-0.1.0/common/api/services/product/product_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.0.9/common/api/services/shop/shop_pb2.py` & `mgo_serializer-0.1.0/common/api/services/shop/shop_pb2.py`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.0.9/common/api/services/shop/shop_pb2_grpc.py` & `mgo_serializer-0.1.0/common/api/services/shop/shop_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.0.9/common/api/services/stats/stats_pb2.py` & `mgo_serializer-0.1.0/common/api/services/stats/stats_pb2.py`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.0.9/common/api/services/stats/stats_pb2_grpc.py` & `mgo_serializer-0.1.0/common/api/services/stats/stats_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.0.9/common/api/services/story/story_pb2.py` & `mgo_serializer-0.1.0/common/api/services/story/story_pb2.py`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.0.9/common/api/services/story/story_pb2_grpc.py` & `mgo_serializer-0.1.0/common/api/services/story/story_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.0.9/mgo_serializer/fields.py` & `mgo_serializer-0.1.0/mgo_serializer/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,25 +104,26 @@
 class BaseField(object):
     _auto_creation_counter = 0
 
     ALLOWED_TYPES = None
 
     initial = None
 
-    def __init__(self, initial=Empty, proto_field=None, default=None, data_field=None, custom=False, context=None):
+    def __init__(self, initial=Empty, proto_field=None, default=None, primary_key=None, custom=False, context=None, db_only=False):
         # Increase the auto creation counter
         self._auto_creation_counter = BaseField._auto_creation_counter
         BaseField._auto_creation_counter += 1
 
         self.initial = self.initial if (initial is Empty) else initial
         self.proto_field = proto_field
         self.default = default
         self.custom = custom
-        self.data_field = data_field
-        self.context = context
+        self.primary_key = primary_key
+        self.db_only = db_only
+        self.context = {} if context is None else context
 
         # These are set up by `.bind()` when the field is added to a serializer.
         self.field_name = None
         self.parent = None
         self.source = None
         self.attributes = None
 
@@ -153,16 +154,14 @@
 
         # convert the dictionary to mapping to make it easier to work with
         dictionary = DictMapper(dictionary) if isinstance(dictionary, dict) else dictionary
 
         if isinstance(dictionary, dict):
             if '_id' in dictionary:
                 dictionary['id'] = dictionary.pop('_id')
-            if self.data_field:
-                dictionary[self.field_name] = dictionary.pop(self.data_field)
 
         if self.custom:
             fill_method = getattr(instance, f'get_custom_{self.field_name}', None)
             return fill_method(dictionary) if fill_method else None
 
         return dictionary[self.field_name] if self.field_name in dictionary and not self.custom else Empty
 
@@ -231,26 +230,14 @@
 
     def __new__(cls, *args, **kwargs):
         instance = super().__new__(cls)
         instance._args = args
         instance._kwargs = kwargs
         return instance
 
-    def create(self, validated_data):
-        model_class = self.Meta.model
-
-        ids = ['id', 'pk', '_id']
-        for id_field in ids:
-            validated_data.pop(id_field, None)
-
-        return model_class.objects.create(**validated_data)
-
-    def save(self):
-        return self.create(self.validated_data)
-
 
 class BooleanField(BaseField):
     TRUE_VALUES = ['t', 'T', 'true', 'True', 'TRUE', '1', 1, True]
     FALSE_VALUES = ['f', 'F', 'false', 'False', 'FALSE', '0', 0, False]
     NULL_VALUES = ['n', 'N', 'null', 'Null', 'NULL', '', None]
 
     def to_internal_value(self, data):
```

### Comparing `mgo_serializer-0.0.9/mgo_serializer/helpers.py` & `mgo_serializer-0.1.0/mgo_serializer/helpers.py`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.0.9/mgo_serializer/meta.py` & `mgo_serializer-0.1.0/mgo_serializer/meta.py`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.0.9/mgo_serializer/serializer.py` & `mgo_serializer-0.1.0/mgo_serializer/serializer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import copy
 import re
 from functools import cached_property
 
 from google.protobuf.json_format import ParseDict, MessageToDict  # noqa
-from google.protobuf.message import Message # noqa
+from google.protobuf.message import Message  # noqa
 
-from mgo_serializer.fields import BaseField, Empty, set_value
 from mgo_serializer.exceptions import ValidationError
+from mgo_serializer.fields import BaseField, Empty, set_value
 from mgo_serializer.helpers import BindingDict, ReturnList, ReturnDict, NestedBoundField, BoundField
 from mgo_serializer.meta import SerializerMetaclass
 
 
 def mongo_to_protobuf(data, schema):
     """
     Convert data to protobuf.
@@ -47,16 +47,14 @@
     def __init__(self, instance=None, data=Empty, **kwargs):
         self.instance = instance
 
         if isinstance(self.instance, Message):
             self.instance = proto_to_dict(self.instance)
         elif isinstance(self.instance, list) and any(isinstance(item, Message) for item in self.instance):
             self.instance = [proto_to_dict(item) for item in self.instance]
-        else:
-            self.instance = copy.deepcopy(self.instance)
 
         if data is not Empty:
             if isinstance(data, list) and any(isinstance(item, Message) for item in data):
                 self.initial_data = [proto_to_dict(item) for item in data]
             elif isinstance(data, list) and not any(isinstance(item, Message) for item in data):
                 self.initial_data = data
             elif isinstance(data, Message):
@@ -97,14 +95,51 @@
 
     def to_representation(self, value):
         raise NotImplementedError('.to_representation() must be implemented.')
 
     def to_protobuf(self, data):
         raise NotImplementedError('.to_protobuf() must be implemented.')
 
+    def create(self, validated_data):
+        raise NotImplementedError('.create() must be implemented.')
+
+    def update(self, instance, validated_data):
+        raise NotImplementedError('.update() must be implemented.')
+
+    def pre_serialize(self, data):
+        """
+        Hook for pre serialization.
+        """
+        return data
+
+    def save(self, **kwargs):
+        assert hasattr(self, '_errors'), (
+            'You must call `.is_valid()` before calling `.save()`.'
+        )
+
+        assert not self.errors, (
+            'You cannot call `.save()` on a serializer with invalid data.'
+        )
+
+        validated_data = {**self.validated_data, **kwargs}
+
+        primary_keys = [
+            field.field_name for field in self.fields.values()
+            if field.primary_key and validated_data[field.field_name] is not None
+        ]
+
+        # check if primary key is provided
+        if not primary_keys:
+            self.instance = self.create(validated_data)
+        else:
+            primary_key_values = {key: validated_data[key] for key in primary_keys}
+            self.instance = self.update(primary_key_values, validated_data)
+
+        return self.instance
+
     def is_valid(self, raise_exception=False):
         """
         Validates the data.
         """
         if not hasattr(self, '_validated_data'):
             try:
                 self._validated_data = self.to_internal_value(self.initial_data)
@@ -160,21 +195,24 @@
         if hasattr(self, 'child') and not self.child.pb:
             raise AttributeError(
                 'Protobuf is not defined in {!r} serializer. '
                 'You can define it in MetaClass with `schema` key.'.format(self.child.__class__.__name__)
             )
 
         protobuf_list = []
-        self._protobuf = self.data
+        # run pre serialization hook
+        self._protobuf = getattr(
+            self.child, 'pre_serialize'
+        )(self.data) if hasattr(self, 'child') else getattr(self, 'pre_serialize')(self.data)
+
         if isinstance(self._protobuf, list):
             for item in self._protobuf:
                 protobuf_list.append(self.to_protobuf(item))
         else:
             return self.to_protobuf(self._protobuf)
-
         return protobuf_list
 
     @property
     def errors(self):
         if not hasattr(self, '_errors'):
             msg = 'You must call `.is_valid()` before accessing `.errors`.'
             raise AssertionError(msg)
@@ -207,14 +245,18 @@
             return self.to_representation(self.initial_data)
         return []
 
     def to_internal_value(self, data):
         ret = []
         errors = []
         for item in data:
+            if self.child.context == 'self' and isinstance(self.parent.context, dict):
+                self.child.context = self.parent.context
+            else:
+                self.child.context = self.context
             try:
                 validated = self.child.run_validation(item)
             except ValidationError as exc:
                 errors.append(exc.detail)
             else:
                 ret.append(validated)
                 errors.append({})
@@ -226,14 +268,20 @@
 
     def to_representation(self, data):
         return [self.child.to_representation(item) for item in data]
 
     def to_protobuf(self, data):
         return self.child.to_protobuf(data)
 
+    def create(self, validated_data):
+        return [self.child.create(data) for data in validated_data]
+
+    def pre_serialize(self, data):
+        return data
+
     @staticmethod
     def validate(attrs):
         return attrs
 
     def run_validation(self, data=Empty):
         """
         We override the default `run_validation`, making it transparent to the user.
@@ -342,14 +390,16 @@
 
         return ret
 
     def to_representation(self, instance):
         ret = {}
         fields = self._readable_fields
         for field in fields:
+            if field.db_only:
+                continue
             attribute = field.get_attribute(instance)
             key = field.proto_field if field.proto_field else field.field_name
             if attribute is None:
                 ret[key] = None
             else:
                 ret[key] = field.to_representation(attribute)
         return ret
@@ -367,16 +417,22 @@
         field = self.fields[key]
         value = self.data.get(key)
         error = self.errors.get(key) if hasattr(self, '_errors') else None
         if isinstance(field, Serializer):
             return NestedBoundField(field, value, error)
         return BoundField(field, value, error)
 
-    # Include a backlink to the serializer class on return objects.
-    # Allows renderers such as HTMLFormRenderer to get the full field info.
+    def create(self, validated_data):
+        model_class = self.meta.model
+        return model_class.objects.create(**validated_data)
+
+    def update(self, instance, validated_data):
+        model = self.meta.model.objects.get(id=instance['id'])
+        model.update(**validated_data)
+        return model
 
     @property
     def data(self):
         ret = super().data
         return ReturnDict(ret, serializer=self)
 
     @property
```

### Comparing `mgo_serializer-0.0.9/mgo_serializer/utils.py` & `mgo_serializer-0.1.0/mgo_serializer/utils.py`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.0.9/mgo_serializer.egg-info/SOURCES.txt` & `mgo_serializer-0.1.0/mgo_serializer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.0.9/setup.py` & `mgo_serializer-0.1.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="mgo_serializer",
-    version="0.0.9",
+    version="0.1.0",
     author='MosyDev',
     author_email='mostafa.uwsgi@gmail.com',
     description='A MongoEngine Serializer to serialize objects from JSON/BSON to JSON and gRPC',
     url='https://github.com/its0x4d/mgo_serializer',
     packages=setuptools.find_packages(),
     license='GPLv3',
     classifiers=[
```

