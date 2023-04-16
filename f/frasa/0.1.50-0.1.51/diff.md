# Comparing `tmp/frasa-0.1.50.tar.gz` & `tmp/frasa-0.1.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frasa-0.1.50.tar", last modified: Sun Apr 16 13:07:18 2023, max compression
+gzip compressed data, was "frasa-0.1.51.tar", last modified: Sun Apr 16 13:41:13 2023, max compression
```

## Comparing `frasa-0.1.50.tar` & `frasa-0.1.51.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 13:07:18.208314 frasa-0.1.50/
--rw-r--r--   0 novay      (501) staff       (20)     1074 2023-04-12 07:34:01.000000 frasa-0.1.50/LICENSE
--rw-r--r--   0 novay      (501) staff       (20)      648 2023-04-16 12:56:55.000000 frasa-0.1.50/MANIFEST.in
--rw-r--r--   0 novay      (501) staff       (20)     1323 2023-04-16 13:07:18.208145 frasa-0.1.50/PKG-INFO
--rw-r--r--   0 novay      (501) staff       (20)      613 2023-04-15 21:07:37.000000 frasa-0.1.50/README.md
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 13:07:18.172729 frasa-0.1.50/frasa/
--rw-r--r--   0 novay      (501) staff       (20)      651 2023-04-16 13:07:08.000000 frasa-0.1.50/frasa/__init__.py
--rw-r--r--   0 novay      (501) staff       (20)      364 2023-04-15 12:25:54.000000 frasa-0.1.50/frasa/base.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 13:07:18.173711 frasa-0.1.50/frasa/datasets/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:13.000000 frasa-0.1.50/frasa/datasets/__init__.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 13:07:18.173850 frasa-0.1.50/frasa/datasets/corpus/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:21.000000 frasa-0.1.50/frasa/datasets/corpus/__init__.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 13:07:18.173974 frasa-0.1.50/frasa/datasets/corpus/bahasa/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:27.000000 frasa-0.1.50/frasa/datasets/corpus/bahasa/__init__.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 13:07:18.174229 frasa-0.1.50/frasa/datasets/corpus/indonesia/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:26.000000 frasa-0.1.50/frasa/datasets/corpus/indonesia/__init__.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 13:07:18.192358 frasa-0.1.50/frasa/datasets/corpus/indonesia/lemma/
--rw-r--r--   0 novay      (501) staff       (20)      377 2023-04-15 21:44:57.000000 frasa-0.1.50/frasa/datasets/corpus/indonesia/lemma/clitics.txt
--rw-r--r--   0 novay      (501) staff       (20) 19937523 2023-04-04 17:44:44.000000 frasa-0.1.50/frasa/datasets/corpus/indonesia/lemma/dict.json
--rw-r--r--   0 novay      (501) staff       (20)   236286 2023-04-04 17:43:21.000000 frasa-0.1.50/frasa/datasets/corpus/indonesia/lemma/root.txt
--rw-r--r--   0 novay      (501) staff       (20)    10520 2023-04-15 22:25:42.000000 frasa-0.1.50/frasa/datasets/corpus/indonesia/stopword.txt
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 13:07:18.199979 frasa-0.1.50/frasa/datasets/corpus/sensor/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:24.000000 frasa-0.1.50/frasa/datasets/corpus/sensor/__init__.py
--rw-r--r--   0 novay      (501) staff       (20)    71076 2023-04-14 16:22:53.000000 frasa-0.1.50/frasa/datasets/corpus/sensor/alphabetic_unicode.json
--rw-r--r--   0 novay      (501) staff       (20)      118 2023-04-15 23:06:01.000000 frasa-0.1.50/frasa/datasets/corpus/sensor/sensor-aturan.csv
--rw-r--r--   0 novay      (501) staff       (20)     7997 2023-04-15 23:06:01.000000 frasa-0.1.50/frasa/datasets/corpus/sensor/sensor-kata.csv
--rw-r--r--   0 novay      (501) staff       (20)      112 2023-04-15 23:06:01.000000 frasa-0.1.50/frasa/datasets/corpus/sensor/sensor-pengganti.csv
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 13:07:18.200278 frasa-0.1.50/frasa/datasets/corpus/tweets/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:23.000000 frasa-0.1.50/frasa/datasets/corpus/tweets/__init__.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 13:07:18.200546 frasa-0.1.50/frasa/datasets/models/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:51:39.000000 frasa-0.1.50/frasa/datasets/models/__init__.py
--rw-r--r--   0 novay      (501) staff       (20)   121561 2023-04-15 23:49:13.000000 frasa-0.1.50/frasa/datasets/models/frasa-gender.pickle
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 13:07:18.201233 frasa-0.1.50/frasa/deteksi/
--rw-r--r--   0 novay      (501) staff       (20)      865 2023-04-16 00:07:31.000000 frasa-0.1.50/frasa/deteksi/__init__.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 13:07:18.201634 frasa-0.1.50/frasa/deteksi/bahasa/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-12 09:15:48.000000 frasa-0.1.50/frasa/deteksi/bahasa/__init__.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 13:07:18.201765 frasa-0.1.50/frasa/deteksi/bahasa/data/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:46.000000 frasa-0.1.50/frasa/deteksi/bahasa/data/__init__.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 13:07:18.202706 frasa-0.1.50/frasa/deteksi/gender/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-15 23:39:09.000000 frasa-0.1.50/frasa/deteksi/gender/__init__.py
--rw-r--r--   0 novay      (501) staff       (20)     2772 2023-04-15 23:45:25.000000 frasa-0.1.50/frasa/deteksi/gender/classify.py
--rw-r--r--   0 novay      (501) staff       (20)      992 2023-04-16 00:06:23.000000 frasa-0.1.50/frasa/deteksi/gender/gender.py
--rw-r--r--   0 novay      (501) staff       (20)      747 2023-04-15 23:49:34.000000 frasa-0.1.50/frasa/deteksi/gender/utils.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 13:07:18.204158 frasa-0.1.50/frasa/deteksi/plagiat/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-15 23:14:54.000000 frasa-0.1.50/frasa/deteksi/plagiat/__init__.py
--rw-r--r--   0 novay      (501) staff       (20)     1363 2023-04-16 09:16:31.000000 frasa-0.1.50/frasa/deteksi/plagiat/cosine.py
--rw-r--r--   0 novay      (501) staff       (20)      911 2023-04-16 09:14:51.000000 frasa-0.1.50/frasa/deteksi/plagiat/jaccard.py
--rw-r--r--   0 novay      (501) staff       (20)     4247 2023-04-16 11:45:48.000000 frasa-0.1.50/frasa/deteksi/plagiat/plagiat.py
--rw-r--r--   0 novay      (501) staff       (20)     1176 2023-04-16 01:06:12.000000 frasa-0.1.50/frasa/deteksi/plagiat/rabin_karp.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 13:07:18.205374 frasa-0.1.50/frasa/preprocess/
--rw-r--r--   0 novay      (501) staff       (20)      186 2023-04-15 22:29:50.000000 frasa-0.1.50/frasa/preprocess/__init__.py
--rw-r--r--   0 novay      (501) staff       (20)     8758 2023-04-15 21:37:48.000000 frasa-0.1.50/frasa/preprocess/lemma.py
--rw-r--r--   0 novay      (501) staff       (20)      850 2023-04-15 22:28:40.000000 frasa-0.1.50/frasa/preprocess/stopword.py
--rw-r--r--   0 novay      (501) staff       (20)     9368 2023-04-15 22:35:39.000000 frasa-0.1.50/frasa/preprocess/token.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 13:07:18.206592 frasa-0.1.50/frasa/scrap/
--rw-r--r--   0 novay      (501) staff       (20)       88 2023-04-15 12:14:39.000000 frasa-0.1.50/frasa/scrap/__init__.py
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-15 16:58:09.000000 frasa-0.1.50/frasa/scrap/cnn.py
--rw-r--r--   0 novay      (501) staff       (20)     7911 2023-04-15 23:07:39.000000 frasa-0.1.50/frasa/scrap/detiknews.py
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-15 16:58:14.000000 frasa-0.1.50/frasa/scrap/liputan6.py
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-15 16:58:30.000000 frasa-0.1.50/frasa/scrap/tribun.py
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-15 16:58:21.000000 frasa-0.1.50/frasa/scrap/viva.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 13:07:18.207771 frasa-0.1.50/frasa/sensor/
--rw-r--r--   0 novay      (501) staff       (20)       76 2023-04-15 23:12:29.000000 frasa-0.1.50/frasa/sensor/__init__.py
--rw-r--r--   0 novay      (501) staff       (20)      428 2023-04-15 23:10:24.000000 frasa-0.1.50/frasa/sensor/constants.py
--rw-r--r--   0 novay      (501) staff       (20)     9267 2023-04-15 23:12:36.000000 frasa-0.1.50/frasa/sensor/sensor.py
--rw-r--r--   0 novay      (501) staff       (20)     1584 2023-04-15 23:10:52.000000 frasa-0.1.50/frasa/sensor/utils.py
--rw-r--r--   0 novay      (501) staff       (20)     2364 2023-04-14 16:23:34.000000 frasa-0.1.50/frasa/sensor/variasi.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 13:07:18.173549 frasa-0.1.50/frasa.egg-info/
--rw-r--r--   0 novay      (501) staff       (20)     1323 2023-04-16 13:07:18.000000 frasa-0.1.50/frasa.egg-info/PKG-INFO
--rw-r--r--   0 novay      (501) staff       (20)     1631 2023-04-16 13:07:18.000000 frasa-0.1.50/frasa.egg-info/SOURCES.txt
--rw-r--r--   0 novay      (501) staff       (20)        1 2023-04-16 13:07:18.000000 frasa-0.1.50/frasa.egg-info/dependency_links.txt
--rw-r--r--   0 novay      (501) staff       (20)       12 2023-04-16 13:07:18.000000 frasa-0.1.50/frasa.egg-info/top_level.txt
--rw-r--r--   0 novay      (501) staff       (20)       38 2023-04-16 13:07:18.208371 frasa-0.1.50/setup.cfg
--rw-r--r--   0 novay      (501) staff       (20)     1345 2023-04-16 13:07:01.000000 frasa-0.1.50/setup.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 13:41:13.429207 frasa-0.1.51/
+-rw-r--r--   0 novay      (501) staff       (20)     1074 2023-04-12 07:34:01.000000 frasa-0.1.51/LICENSE
+-rw-r--r--   0 novay      (501) staff       (20)      648 2023-04-16 12:56:55.000000 frasa-0.1.51/MANIFEST.in
+-rw-r--r--   0 novay      (501) staff       (20)     1323 2023-04-16 13:41:13.429053 frasa-0.1.51/PKG-INFO
+-rw-r--r--   0 novay      (501) staff       (20)      613 2023-04-15 21:07:37.000000 frasa-0.1.51/README.md
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 13:41:13.411032 frasa-0.1.51/frasa/
+-rw-r--r--   0 novay      (501) staff       (20)      677 2023-04-16 13:41:08.000000 frasa-0.1.51/frasa/__init__.py
+-rw-r--r--   0 novay      (501) staff       (20)      364 2023-04-15 12:25:54.000000 frasa-0.1.51/frasa/base.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 13:41:13.412106 frasa-0.1.51/frasa/datasets/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:13.000000 frasa-0.1.51/frasa/datasets/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 13:41:13.412237 frasa-0.1.51/frasa/datasets/corpus/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:21.000000 frasa-0.1.51/frasa/datasets/corpus/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 13:41:13.412347 frasa-0.1.51/frasa/datasets/corpus/bahasa/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:27.000000 frasa-0.1.51/frasa/datasets/corpus/bahasa/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 13:41:13.412609 frasa-0.1.51/frasa/datasets/corpus/indonesia/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:26.000000 frasa-0.1.51/frasa/datasets/corpus/indonesia/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 13:41:13.423785 frasa-0.1.51/frasa/datasets/corpus/indonesia/lemma/
+-rw-r--r--   0 novay      (501) staff       (20)      377 2023-04-15 21:44:57.000000 frasa-0.1.51/frasa/datasets/corpus/indonesia/lemma/clitics.txt
+-rw-r--r--   0 novay      (501) staff       (20) 19937523 2023-04-04 17:44:44.000000 frasa-0.1.51/frasa/datasets/corpus/indonesia/lemma/dict.json
+-rw-r--r--   0 novay      (501) staff       (20)   236286 2023-04-04 17:43:21.000000 frasa-0.1.51/frasa/datasets/corpus/indonesia/lemma/root.txt
+-rw-r--r--   0 novay      (501) staff       (20)    10520 2023-04-15 22:25:42.000000 frasa-0.1.51/frasa/datasets/corpus/indonesia/stopword.txt
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 13:41:13.424732 frasa-0.1.51/frasa/datasets/corpus/sensor/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:24.000000 frasa-0.1.51/frasa/datasets/corpus/sensor/__init__.py
+-rw-r--r--   0 novay      (501) staff       (20)    71076 2023-04-14 16:22:53.000000 frasa-0.1.51/frasa/datasets/corpus/sensor/alphabetic_unicode.json
+-rw-r--r--   0 novay      (501) staff       (20)      118 2023-04-15 23:06:01.000000 frasa-0.1.51/frasa/datasets/corpus/sensor/sensor-aturan.csv
+-rw-r--r--   0 novay      (501) staff       (20)     7997 2023-04-15 23:06:01.000000 frasa-0.1.51/frasa/datasets/corpus/sensor/sensor-kata.csv
+-rw-r--r--   0 novay      (501) staff       (20)      112 2023-04-15 23:06:01.000000 frasa-0.1.51/frasa/datasets/corpus/sensor/sensor-pengganti.csv
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 13:41:13.424873 frasa-0.1.51/frasa/datasets/corpus/tweets/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:23.000000 frasa-0.1.51/frasa/datasets/corpus/tweets/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 13:41:13.425103 frasa-0.1.51/frasa/datasets/models/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:51:39.000000 frasa-0.1.51/frasa/datasets/models/__init__.py
+-rw-r--r--   0 novay      (501) staff       (20)   121561 2023-04-15 23:49:13.000000 frasa-0.1.51/frasa/datasets/models/frasa-gender.pickle
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 13:41:13.425313 frasa-0.1.51/frasa/deteksi/
+-rw-r--r--   0 novay      (501) staff       (20)      865 2023-04-16 00:07:31.000000 frasa-0.1.51/frasa/deteksi/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 13:41:13.425452 frasa-0.1.51/frasa/deteksi/bahasa/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-12 09:15:48.000000 frasa-0.1.51/frasa/deteksi/bahasa/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 13:41:13.425568 frasa-0.1.51/frasa/deteksi/bahasa/data/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:46.000000 frasa-0.1.51/frasa/deteksi/bahasa/data/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 13:41:13.426092 frasa-0.1.51/frasa/deteksi/gender/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-15 23:39:09.000000 frasa-0.1.51/frasa/deteksi/gender/__init__.py
+-rw-r--r--   0 novay      (501) staff       (20)     2772 2023-04-15 23:45:25.000000 frasa-0.1.51/frasa/deteksi/gender/classify.py
+-rw-r--r--   0 novay      (501) staff       (20)      992 2023-04-16 00:06:23.000000 frasa-0.1.51/frasa/deteksi/gender/gender.py
+-rw-r--r--   0 novay      (501) staff       (20)      747 2023-04-15 23:49:34.000000 frasa-0.1.51/frasa/deteksi/gender/utils.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 13:41:13.426801 frasa-0.1.51/frasa/deteksi/plagiat/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-15 23:14:54.000000 frasa-0.1.51/frasa/deteksi/plagiat/__init__.py
+-rw-r--r--   0 novay      (501) staff       (20)     1363 2023-04-16 09:16:31.000000 frasa-0.1.51/frasa/deteksi/plagiat/cosine.py
+-rw-r--r--   0 novay      (501) staff       (20)      911 2023-04-16 09:14:51.000000 frasa-0.1.51/frasa/deteksi/plagiat/jaccard.py
+-rw-r--r--   0 novay      (501) staff       (20)     4247 2023-04-16 11:45:48.000000 frasa-0.1.51/frasa/deteksi/plagiat/plagiat.py
+-rw-r--r--   0 novay      (501) staff       (20)     1176 2023-04-16 01:06:12.000000 frasa-0.1.51/frasa/deteksi/plagiat/rabin_karp.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 13:41:13.427383 frasa-0.1.51/frasa/preprocess/
+-rw-r--r--   0 novay      (501) staff       (20)      186 2023-04-15 22:29:50.000000 frasa-0.1.51/frasa/preprocess/__init__.py
+-rw-r--r--   0 novay      (501) staff       (20)     8758 2023-04-15 21:37:48.000000 frasa-0.1.51/frasa/preprocess/lemma.py
+-rw-r--r--   0 novay      (501) staff       (20)      850 2023-04-15 22:28:40.000000 frasa-0.1.51/frasa/preprocess/stopword.py
+-rw-r--r--   0 novay      (501) staff       (20)     9372 2023-04-16 13:15:30.000000 frasa-0.1.51/frasa/preprocess/token.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 13:41:13.428164 frasa-0.1.51/frasa/scrap/
+-rw-r--r--   0 novay      (501) staff       (20)       88 2023-04-15 12:14:39.000000 frasa-0.1.51/frasa/scrap/__init__.py
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-15 16:58:09.000000 frasa-0.1.51/frasa/scrap/cnn.py
+-rw-r--r--   0 novay      (501) staff       (20)     7911 2023-04-15 23:07:39.000000 frasa-0.1.51/frasa/scrap/detiknews.py
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-15 16:58:14.000000 frasa-0.1.51/frasa/scrap/liputan6.py
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-15 16:58:30.000000 frasa-0.1.51/frasa/scrap/tribun.py
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-15 16:58:21.000000 frasa-0.1.51/frasa/scrap/viva.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 13:41:13.428803 frasa-0.1.51/frasa/sensor/
+-rw-r--r--   0 novay      (501) staff       (20)       76 2023-04-15 23:12:29.000000 frasa-0.1.51/frasa/sensor/__init__.py
+-rw-r--r--   0 novay      (501) staff       (20)      428 2023-04-15 23:10:24.000000 frasa-0.1.51/frasa/sensor/constants.py
+-rw-r--r--   0 novay      (501) staff       (20)     9267 2023-04-15 23:12:36.000000 frasa-0.1.51/frasa/sensor/sensor.py
+-rw-r--r--   0 novay      (501) staff       (20)     1584 2023-04-15 23:10:52.000000 frasa-0.1.51/frasa/sensor/utils.py
+-rw-r--r--   0 novay      (501) staff       (20)     2364 2023-04-14 16:23:34.000000 frasa-0.1.51/frasa/sensor/variasi.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 13:41:13.411933 frasa-0.1.51/frasa.egg-info/
+-rw-r--r--   0 novay      (501) staff       (20)     1323 2023-04-16 13:41:13.000000 frasa-0.1.51/frasa.egg-info/PKG-INFO
+-rw-r--r--   0 novay      (501) staff       (20)     1631 2023-04-16 13:41:13.000000 frasa-0.1.51/frasa.egg-info/SOURCES.txt
+-rw-r--r--   0 novay      (501) staff       (20)        1 2023-04-16 13:41:13.000000 frasa-0.1.51/frasa.egg-info/dependency_links.txt
+-rw-r--r--   0 novay      (501) staff       (20)       12 2023-04-16 13:41:13.000000 frasa-0.1.51/frasa.egg-info/top_level.txt
+-rw-r--r--   0 novay      (501) staff       (20)       38 2023-04-16 13:41:13.429260 frasa-0.1.51/setup.cfg
+-rw-r--r--   0 novay      (501) staff       (20)     1345 2023-04-16 13:41:03.000000 frasa-0.1.51/setup.py
```

### Comparing `frasa-0.1.50/LICENSE` & `frasa-0.1.51/LICENSE`

 * *Files identical despite different names*

### Comparing `frasa-0.1.50/MANIFEST.in` & `frasa-0.1.51/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `frasa-0.1.50/PKG-INFO` & `frasa-0.1.51/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frasa
-Version: 0.1.50
+Version: 0.1.51
 Summary: Koleksi NLP Pribadi untuk Bahasa Indonesia.
 Home-page: https://github.com/novay/frasa
 Author: Novianto Rahmadi
 Author-email: novay@btekno.id
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `frasa-0.1.50/README.md` & `frasa-0.1.51/README.md`

 * *Files identical despite different names*

### Comparing `frasa-0.1.50/frasa/__init__.py` & `frasa-0.1.51/frasa/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,17 +9,18 @@
 
 Kunjungi http://frasa.id untuk informasi selengkapnya.
 """
 
 import os
 
 __name__ = "frasa"
-__version__ = "0.1.50"
+__version__ = "0.1.51"
 __license__ = 'MIT'
 __author__ = 'Novianto Rahmadi'
 
 PACKAGE_DIR = os.path.dirname(os.path.abspath(__file__))
 DATASET_DIR = PACKAGE_DIR + '/datasets/corpus'
 MODELS_DIR = PACKAGE_DIR + '/datasets/models'
 
 from .base import *
-from .sensor import *
+from .sensor import *
+from .preprocess import *
```

### Comparing `frasa-0.1.50/frasa/datasets/corpus/indonesia/lemma/dict.json` & `frasa-0.1.51/frasa/datasets/corpus/indonesia/lemma/dict.json`

 * *Files identical despite different names*

### Comparing `frasa-0.1.50/frasa/datasets/corpus/indonesia/lemma/root.txt` & `frasa-0.1.51/frasa/datasets/corpus/indonesia/lemma/root.txt`

 * *Files identical despite different names*

### Comparing `frasa-0.1.50/frasa/datasets/corpus/indonesia/stopword.txt` & `frasa-0.1.51/frasa/datasets/corpus/indonesia/stopword.txt`

 * *Files identical despite different names*

### Comparing `frasa-0.1.50/frasa/datasets/corpus/sensor/alphabetic_unicode.json` & `frasa-0.1.51/frasa/datasets/corpus/sensor/alphabetic_unicode.json`

 * *Files identical despite different names*

### Comparing `frasa-0.1.50/frasa/datasets/corpus/sensor/sensor-kata.csv` & `frasa-0.1.51/frasa/datasets/corpus/sensor/sensor-kata.csv`

 * *Files identical despite different names*

### Comparing `frasa-0.1.50/frasa/datasets/models/frasa-gender.pickle` & `frasa-0.1.51/frasa/datasets/models/frasa-gender.pickle`

 * *Files identical despite different names*

### Comparing `frasa-0.1.50/frasa/deteksi/__init__.py` & `frasa-0.1.51/frasa/deteksi/__init__.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.50/frasa/deteksi/gender/classify.py` & `frasa-0.1.51/frasa/deteksi/gender/classify.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.50/frasa/deteksi/gender/gender.py` & `frasa-0.1.51/frasa/deteksi/gender/gender.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.50/frasa/deteksi/gender/utils.py` & `frasa-0.1.51/frasa/deteksi/gender/utils.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.50/frasa/deteksi/plagiat/cosine.py` & `frasa-0.1.51/frasa/deteksi/plagiat/cosine.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.50/frasa/deteksi/plagiat/jaccard.py` & `frasa-0.1.51/frasa/deteksi/plagiat/jaccard.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.50/frasa/deteksi/plagiat/plagiat.py` & `frasa-0.1.51/frasa/deteksi/plagiat/plagiat.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.50/frasa/deteksi/plagiat/rabin_karp.py` & `frasa-0.1.51/frasa/deteksi/plagiat/rabin_karp.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.50/frasa/preprocess/lemma.py` & `frasa-0.1.51/frasa/preprocess/lemma.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.50/frasa/preprocess/stopword.py` & `frasa-0.1.51/frasa/preprocess/stopword.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.50/frasa/preprocess/token.py` & `frasa-0.1.51/frasa/preprocess/token.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import os
 import re
 from frasa import PACKAGE_DIR
-from frasa.preprocess import lemma
+from .lemma import Lemmatisasi
 
 class Token:
     def __init__(self):
         self.current_dir = PACKAGE_DIR + '/datasets/corpus/indonesia'
         
         self.start_url = ["www.", "http"]
         self.end_url = [".com", ".id", ".io", ".html", ".org", ".net"]
         self.inside_punct = ['!', '&', '(', ')', '*', '?', ',', '.', '<', '>', '/', ':', ';',
                              '[', ']', '\\', '^', '`', '{', '}', '|', '~', '"', '“', "'"]
         self.outside_punct = self.inside_punct + ["-", "_"]
         
-        self.lemma = lemma
+        self.lemma = Lemmatisasi()
         clitics_file = os.path.join(self.current_dir, "lemma", "clitics.txt")
         with open(clitics_file) as f:
             self.non_clitics = set(f.read().splitlines())
 
     def convert_non_ascii(self, text):
         text = re.sub("\u2014|\u2013", "-", text)
         text = re.sub("\u2018|\u2019", "'", text)
```

### Comparing `frasa-0.1.50/frasa/scrap/detiknews.py` & `frasa-0.1.51/frasa/scrap/detiknews.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.50/frasa/sensor/sensor.py` & `frasa-0.1.51/frasa/sensor/sensor.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.50/frasa/sensor/utils.py` & `frasa-0.1.51/frasa/sensor/utils.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.50/frasa/sensor/variasi.py` & `frasa-0.1.51/frasa/sensor/variasi.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.50/frasa.egg-info/PKG-INFO` & `frasa-0.1.51/frasa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frasa
-Version: 0.1.50
+Version: 0.1.51
 Summary: Koleksi NLP Pribadi untuk Bahasa Indonesia.
 Home-page: https://github.com/novay/frasa
 Author: Novianto Rahmadi
 Author-email: novay@btekno.id
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `frasa-0.1.50/frasa.egg-info/SOURCES.txt` & `frasa-0.1.51/frasa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `frasa-0.1.50/setup.py` & `frasa-0.1.51/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 HERE = path.abspath(path.dirname(__file__))
 
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
     
 setup(
     name="frasa",
-    version="0.1.50",
+    version="0.1.51",
     description="Koleksi NLP Pribadi untuk Bahasa Indonesia.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/novay/frasa",
     author="Novianto Rahmadi",
     author_email="novay@btekno.id",
     license="MIT",
```

