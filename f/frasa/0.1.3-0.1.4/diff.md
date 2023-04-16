# Comparing `tmp/frasa-0.1.3.tar.gz` & `tmp/frasa-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frasa-0.1.3.tar", last modified: Sun Apr 16 12:50:37 2023, max compression
+gzip compressed data, was "frasa-0.1.4.tar", last modified: Sun Apr 16 12:57:11 2023, max compression
```

## Comparing `frasa-0.1.3.tar` & `frasa-0.1.4.tar`

### file list

```diff
@@ -1,70 +1,74 @@
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 12:50:37.527232 frasa-0.1.3/
--rw-r--r--   0 novay      (501) staff       (20)     1074 2023-04-12 07:34:01.000000 frasa-0.1.3/LICENSE
--rw-r--r--   0 novay      (501) staff       (20)      555 2023-04-15 23:14:00.000000 frasa-0.1.3/MANIFEST.in
--rw-r--r--   0 novay      (501) staff       (20)     1322 2023-04-16 12:50:37.527071 frasa-0.1.3/PKG-INFO
--rw-r--r--   0 novay      (501) staff       (20)      613 2023-04-15 21:07:37.000000 frasa-0.1.3/README.md
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 12:50:37.506165 frasa-0.1.3/frasa/
--rw-r--r--   0 novay      (501) staff       (20)      650 2023-04-16 12:50:01.000000 frasa-0.1.3/frasa/__init__.py
--rw-r--r--   0 novay      (501) staff       (20)      364 2023-04-15 12:25:54.000000 frasa-0.1.3/frasa/base.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 12:50:37.507347 frasa-0.1.3/frasa/datasets/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:13.000000 frasa-0.1.3/frasa/datasets/__init__.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 12:50:37.507476 frasa-0.1.3/frasa/datasets/corpus/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:21.000000 frasa-0.1.3/frasa/datasets/corpus/__init__.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 12:50:37.507593 frasa-0.1.3/frasa/datasets/corpus/bahasa/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:27.000000 frasa-0.1.3/frasa/datasets/corpus/bahasa/__init__.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 12:50:37.507833 frasa-0.1.3/frasa/datasets/corpus/indonesia/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:26.000000 frasa-0.1.3/frasa/datasets/corpus/indonesia/__init__.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 12:50:37.522202 frasa-0.1.3/frasa/datasets/corpus/indonesia/lemma/
--rw-r--r--   0 novay      (501) staff       (20)      377 2023-04-15 21:44:57.000000 frasa-0.1.3/frasa/datasets/corpus/indonesia/lemma/clitics.txt
--rw-r--r--   0 novay      (501) staff       (20) 19937523 2023-04-04 17:44:44.000000 frasa-0.1.3/frasa/datasets/corpus/indonesia/lemma/dict.json
--rw-r--r--   0 novay      (501) staff       (20)   236286 2023-04-04 17:43:21.000000 frasa-0.1.3/frasa/datasets/corpus/indonesia/lemma/root.txt
--rw-r--r--   0 novay      (501) staff       (20)    10520 2023-04-15 22:25:42.000000 frasa-0.1.3/frasa/datasets/corpus/indonesia/stopword.txt
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 12:50:37.522541 frasa-0.1.3/frasa/datasets/corpus/sensor/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:24.000000 frasa-0.1.3/frasa/datasets/corpus/sensor/__init__.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 12:50:37.522664 frasa-0.1.3/frasa/datasets/corpus/tweets/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:23.000000 frasa-0.1.3/frasa/datasets/corpus/tweets/__init__.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 12:50:37.522898 frasa-0.1.3/frasa/datasets/models/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:51:39.000000 frasa-0.1.3/frasa/datasets/models/__init__.py
--rw-r--r--   0 novay      (501) staff       (20)   121561 2023-04-15 23:49:13.000000 frasa-0.1.3/frasa/datasets/models/frasa-gender.pickle
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 12:50:37.523112 frasa-0.1.3/frasa/deteksi/
--rw-r--r--   0 novay      (501) staff       (20)      865 2023-04-16 00:07:31.000000 frasa-0.1.3/frasa/deteksi/__init__.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 12:50:37.523242 frasa-0.1.3/frasa/deteksi/bahasa/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-12 09:15:48.000000 frasa-0.1.3/frasa/deteksi/bahasa/__init__.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 12:50:37.523354 frasa-0.1.3/frasa/deteksi/bahasa/data/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:46.000000 frasa-0.1.3/frasa/deteksi/bahasa/data/__init__.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 12:50:37.523856 frasa-0.1.3/frasa/deteksi/gender/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-15 23:39:09.000000 frasa-0.1.3/frasa/deteksi/gender/__init__.py
--rw-r--r--   0 novay      (501) staff       (20)     2772 2023-04-15 23:45:25.000000 frasa-0.1.3/frasa/deteksi/gender/classify.py
--rw-r--r--   0 novay      (501) staff       (20)      992 2023-04-16 00:06:23.000000 frasa-0.1.3/frasa/deteksi/gender/gender.py
--rw-r--r--   0 novay      (501) staff       (20)      747 2023-04-15 23:49:34.000000 frasa-0.1.3/frasa/deteksi/gender/utils.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 12:50:37.524682 frasa-0.1.3/frasa/deteksi/plagiat/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-15 23:14:54.000000 frasa-0.1.3/frasa/deteksi/plagiat/__init__.py
--rw-r--r--   0 novay      (501) staff       (20)     1363 2023-04-16 09:16:31.000000 frasa-0.1.3/frasa/deteksi/plagiat/cosine.py
--rw-r--r--   0 novay      (501) staff       (20)      911 2023-04-16 09:14:51.000000 frasa-0.1.3/frasa/deteksi/plagiat/jaccard.py
--rw-r--r--   0 novay      (501) staff       (20)     4247 2023-04-16 11:45:48.000000 frasa-0.1.3/frasa/deteksi/plagiat/plagiat.py
--rw-r--r--   0 novay      (501) staff       (20)     1176 2023-04-16 01:06:12.000000 frasa-0.1.3/frasa/deteksi/plagiat/rabin_karp.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 12:50:37.525271 frasa-0.1.3/frasa/preprocess/
--rw-r--r--   0 novay      (501) staff       (20)      186 2023-04-15 22:29:50.000000 frasa-0.1.3/frasa/preprocess/__init__.py
--rw-r--r--   0 novay      (501) staff       (20)     8758 2023-04-15 21:37:48.000000 frasa-0.1.3/frasa/preprocess/lemma.py
--rw-r--r--   0 novay      (501) staff       (20)      850 2023-04-15 22:28:40.000000 frasa-0.1.3/frasa/preprocess/stopword.py
--rw-r--r--   0 novay      (501) staff       (20)     9368 2023-04-15 22:35:39.000000 frasa-0.1.3/frasa/preprocess/token.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 12:50:37.526168 frasa-0.1.3/frasa/scrap/
--rw-r--r--   0 novay      (501) staff       (20)       88 2023-04-15 12:14:39.000000 frasa-0.1.3/frasa/scrap/__init__.py
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-15 16:58:09.000000 frasa-0.1.3/frasa/scrap/cnn.py
--rw-r--r--   0 novay      (501) staff       (20)     7911 2023-04-15 23:07:39.000000 frasa-0.1.3/frasa/scrap/detiknews.py
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-15 16:58:14.000000 frasa-0.1.3/frasa/scrap/liputan6.py
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-15 16:58:30.000000 frasa-0.1.3/frasa/scrap/tribun.py
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-15 16:58:21.000000 frasa-0.1.3/frasa/scrap/viva.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 12:50:37.526839 frasa-0.1.3/frasa/sensor/
--rw-r--r--   0 novay      (501) staff       (20)       76 2023-04-15 23:12:29.000000 frasa-0.1.3/frasa/sensor/__init__.py
--rw-r--r--   0 novay      (501) staff       (20)      428 2023-04-15 23:10:24.000000 frasa-0.1.3/frasa/sensor/constants.py
--rw-r--r--   0 novay      (501) staff       (20)     9267 2023-04-15 23:12:36.000000 frasa-0.1.3/frasa/sensor/sensor.py
--rw-r--r--   0 novay      (501) staff       (20)     1584 2023-04-15 23:10:52.000000 frasa-0.1.3/frasa/sensor/utils.py
--rw-r--r--   0 novay      (501) staff       (20)     2364 2023-04-14 16:23:34.000000 frasa-0.1.3/frasa/sensor/variasi.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 12:50:37.507171 frasa-0.1.3/frasa.egg-info/
--rw-r--r--   0 novay      (501) staff       (20)     1322 2023-04-16 12:50:37.000000 frasa-0.1.3/frasa.egg-info/PKG-INFO
--rw-r--r--   0 novay      (501) staff       (20)     1436 2023-04-16 12:50:37.000000 frasa-0.1.3/frasa.egg-info/SOURCES.txt
--rw-r--r--   0 novay      (501) staff       (20)        1 2023-04-16 12:50:37.000000 frasa-0.1.3/frasa.egg-info/dependency_links.txt
--rw-r--r--   0 novay      (501) staff       (20)       12 2023-04-16 12:50:37.000000 frasa-0.1.3/frasa.egg-info/top_level.txt
--rw-r--r--   0 novay      (501) staff       (20)       38 2023-04-16 12:50:37.527282 frasa-0.1.3/setup.cfg
--rw-r--r--   0 novay      (501) staff       (20)     1127 2023-04-16 12:49:57.000000 frasa-0.1.3/setup.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 12:57:11.751974 frasa-0.1.4/
+-rw-r--r--   0 novay      (501) staff       (20)     1074 2023-04-12 07:34:01.000000 frasa-0.1.4/LICENSE
+-rw-r--r--   0 novay      (501) staff       (20)      648 2023-04-16 12:56:55.000000 frasa-0.1.4/MANIFEST.in
+-rw-r--r--   0 novay      (501) staff       (20)     1322 2023-04-16 12:57:11.751809 frasa-0.1.4/PKG-INFO
+-rw-r--r--   0 novay      (501) staff       (20)      613 2023-04-15 21:07:37.000000 frasa-0.1.4/README.md
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 12:57:11.717027 frasa-0.1.4/frasa/
+-rw-r--r--   0 novay      (501) staff       (20)      650 2023-04-16 12:57:08.000000 frasa-0.1.4/frasa/__init__.py
+-rw-r--r--   0 novay      (501) staff       (20)      364 2023-04-15 12:25:54.000000 frasa-0.1.4/frasa/base.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 12:57:11.717866 frasa-0.1.4/frasa/datasets/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:13.000000 frasa-0.1.4/frasa/datasets/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 12:57:11.717981 frasa-0.1.4/frasa/datasets/corpus/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:21.000000 frasa-0.1.4/frasa/datasets/corpus/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 12:57:11.718109 frasa-0.1.4/frasa/datasets/corpus/bahasa/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:27.000000 frasa-0.1.4/frasa/datasets/corpus/bahasa/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 12:57:11.718353 frasa-0.1.4/frasa/datasets/corpus/indonesia/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:26.000000 frasa-0.1.4/frasa/datasets/corpus/indonesia/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 12:57:11.736245 frasa-0.1.4/frasa/datasets/corpus/indonesia/lemma/
+-rw-r--r--   0 novay      (501) staff       (20)      377 2023-04-15 21:44:57.000000 frasa-0.1.4/frasa/datasets/corpus/indonesia/lemma/clitics.txt
+-rw-r--r--   0 novay      (501) staff       (20) 19937523 2023-04-04 17:44:44.000000 frasa-0.1.4/frasa/datasets/corpus/indonesia/lemma/dict.json
+-rw-r--r--   0 novay      (501) staff       (20)   236286 2023-04-04 17:43:21.000000 frasa-0.1.4/frasa/datasets/corpus/indonesia/lemma/root.txt
+-rw-r--r--   0 novay      (501) staff       (20)    10520 2023-04-15 22:25:42.000000 frasa-0.1.4/frasa/datasets/corpus/indonesia/stopword.txt
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 12:57:11.743636 frasa-0.1.4/frasa/datasets/corpus/sensor/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:24.000000 frasa-0.1.4/frasa/datasets/corpus/sensor/__init__.py
+-rw-r--r--   0 novay      (501) staff       (20)    71076 2023-04-14 16:22:53.000000 frasa-0.1.4/frasa/datasets/corpus/sensor/alphabetic_unicode.json
+-rw-r--r--   0 novay      (501) staff       (20)      118 2023-04-15 23:06:01.000000 frasa-0.1.4/frasa/datasets/corpus/sensor/sensor-aturan.csv
+-rw-r--r--   0 novay      (501) staff       (20)     7997 2023-04-15 23:06:01.000000 frasa-0.1.4/frasa/datasets/corpus/sensor/sensor-kata.csv
+-rw-r--r--   0 novay      (501) staff       (20)      112 2023-04-15 23:06:01.000000 frasa-0.1.4/frasa/datasets/corpus/sensor/sensor-pengganti.csv
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 12:57:11.743933 frasa-0.1.4/frasa/datasets/corpus/tweets/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:23.000000 frasa-0.1.4/frasa/datasets/corpus/tweets/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 12:57:11.744216 frasa-0.1.4/frasa/datasets/models/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:51:39.000000 frasa-0.1.4/frasa/datasets/models/__init__.py
+-rw-r--r--   0 novay      (501) staff       (20)   121561 2023-04-15 23:49:13.000000 frasa-0.1.4/frasa/datasets/models/frasa-gender.pickle
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 12:57:11.745006 frasa-0.1.4/frasa/deteksi/
+-rw-r--r--   0 novay      (501) staff       (20)      865 2023-04-16 00:07:31.000000 frasa-0.1.4/frasa/deteksi/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 12:57:11.745273 frasa-0.1.4/frasa/deteksi/bahasa/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-12 09:15:48.000000 frasa-0.1.4/frasa/deteksi/bahasa/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 12:57:11.745396 frasa-0.1.4/frasa/deteksi/bahasa/data/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:46.000000 frasa-0.1.4/frasa/deteksi/bahasa/data/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 12:57:11.746390 frasa-0.1.4/frasa/deteksi/gender/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-15 23:39:09.000000 frasa-0.1.4/frasa/deteksi/gender/__init__.py
+-rw-r--r--   0 novay      (501) staff       (20)     2772 2023-04-15 23:45:25.000000 frasa-0.1.4/frasa/deteksi/gender/classify.py
+-rw-r--r--   0 novay      (501) staff       (20)      992 2023-04-16 00:06:23.000000 frasa-0.1.4/frasa/deteksi/gender/gender.py
+-rw-r--r--   0 novay      (501) staff       (20)      747 2023-04-15 23:49:34.000000 frasa-0.1.4/frasa/deteksi/gender/utils.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 12:57:11.747761 frasa-0.1.4/frasa/deteksi/plagiat/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-15 23:14:54.000000 frasa-0.1.4/frasa/deteksi/plagiat/__init__.py
+-rw-r--r--   0 novay      (501) staff       (20)     1363 2023-04-16 09:16:31.000000 frasa-0.1.4/frasa/deteksi/plagiat/cosine.py
+-rw-r--r--   0 novay      (501) staff       (20)      911 2023-04-16 09:14:51.000000 frasa-0.1.4/frasa/deteksi/plagiat/jaccard.py
+-rw-r--r--   0 novay      (501) staff       (20)     4247 2023-04-16 11:45:48.000000 frasa-0.1.4/frasa/deteksi/plagiat/plagiat.py
+-rw-r--r--   0 novay      (501) staff       (20)     1176 2023-04-16 01:06:12.000000 frasa-0.1.4/frasa/deteksi/plagiat/rabin_karp.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 12:57:11.748926 frasa-0.1.4/frasa/preprocess/
+-rw-r--r--   0 novay      (501) staff       (20)      186 2023-04-15 22:29:50.000000 frasa-0.1.4/frasa/preprocess/__init__.py
+-rw-r--r--   0 novay      (501) staff       (20)     8758 2023-04-15 21:37:48.000000 frasa-0.1.4/frasa/preprocess/lemma.py
+-rw-r--r--   0 novay      (501) staff       (20)      850 2023-04-15 22:28:40.000000 frasa-0.1.4/frasa/preprocess/stopword.py
+-rw-r--r--   0 novay      (501) staff       (20)     9368 2023-04-15 22:35:39.000000 frasa-0.1.4/frasa/preprocess/token.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 12:57:11.750292 frasa-0.1.4/frasa/scrap/
+-rw-r--r--   0 novay      (501) staff       (20)       88 2023-04-15 12:14:39.000000 frasa-0.1.4/frasa/scrap/__init__.py
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-15 16:58:09.000000 frasa-0.1.4/frasa/scrap/cnn.py
+-rw-r--r--   0 novay      (501) staff       (20)     7911 2023-04-15 23:07:39.000000 frasa-0.1.4/frasa/scrap/detiknews.py
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-15 16:58:14.000000 frasa-0.1.4/frasa/scrap/liputan6.py
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-15 16:58:30.000000 frasa-0.1.4/frasa/scrap/tribun.py
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-15 16:58:21.000000 frasa-0.1.4/frasa/scrap/viva.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 12:57:11.751430 frasa-0.1.4/frasa/sensor/
+-rw-r--r--   0 novay      (501) staff       (20)       76 2023-04-15 23:12:29.000000 frasa-0.1.4/frasa/sensor/__init__.py
+-rw-r--r--   0 novay      (501) staff       (20)      428 2023-04-15 23:10:24.000000 frasa-0.1.4/frasa/sensor/constants.py
+-rw-r--r--   0 novay      (501) staff       (20)     9267 2023-04-15 23:12:36.000000 frasa-0.1.4/frasa/sensor/sensor.py
+-rw-r--r--   0 novay      (501) staff       (20)     1584 2023-04-15 23:10:52.000000 frasa-0.1.4/frasa/sensor/utils.py
+-rw-r--r--   0 novay      (501) staff       (20)     2364 2023-04-14 16:23:34.000000 frasa-0.1.4/frasa/sensor/variasi.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-16 12:57:11.717713 frasa-0.1.4/frasa.egg-info/
+-rw-r--r--   0 novay      (501) staff       (20)     1322 2023-04-16 12:57:11.000000 frasa-0.1.4/frasa.egg-info/PKG-INFO
+-rw-r--r--   0 novay      (501) staff       (20)     1631 2023-04-16 12:57:11.000000 frasa-0.1.4/frasa.egg-info/SOURCES.txt
+-rw-r--r--   0 novay      (501) staff       (20)        1 2023-04-16 12:57:11.000000 frasa-0.1.4/frasa.egg-info/dependency_links.txt
+-rw-r--r--   0 novay      (501) staff       (20)       12 2023-04-16 12:57:11.000000 frasa-0.1.4/frasa.egg-info/top_level.txt
+-rw-r--r--   0 novay      (501) staff       (20)       38 2023-04-16 12:57:11.752030 frasa-0.1.4/setup.cfg
+-rw-r--r--   0 novay      (501) staff       (20)     1127 2023-04-16 12:57:02.000000 frasa-0.1.4/setup.py
```

### Comparing `frasa-0.1.3/LICENSE` & `frasa-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `frasa-0.1.3/PKG-INFO` & `frasa-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frasa
-Version: 0.1.3
+Version: 0.1.4
 Summary: Koleksi NLP Pribadi untuk Bahasa Indonesia.
 Home-page: https://github.com/novay/frasa
 Author: Novianto Rahmadi
 Author-email: novay@btekno.id
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `frasa-0.1.3/README.md` & `frasa-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `frasa-0.1.3/frasa/__init__.py` & `frasa-0.1.4/frasa/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 Kunjungi http://frasa.id untuk informasi selengkapnya.
 """
 
 import os
 
 __name__ = "frasa"
-__version__ = "0.1.3"
+__version__ = "0.1.4"
 __license__ = 'MIT'
 __author__ = 'Novianto Rahmadi'
 
 PACKAGE_DIR = os.path.dirname(os.path.abspath(__file__))
 DATASET_DIR = PACKAGE_DIR + '/datasets/corpus'
 MODELS_DIR = PACKAGE_DIR + '/datasets/models'
```

### Comparing `frasa-0.1.3/frasa/datasets/corpus/indonesia/lemma/dict.json` & `frasa-0.1.4/frasa/datasets/corpus/indonesia/lemma/dict.json`

 * *Files identical despite different names*

### Comparing `frasa-0.1.3/frasa/datasets/corpus/indonesia/lemma/root.txt` & `frasa-0.1.4/frasa/datasets/corpus/indonesia/lemma/root.txt`

 * *Files identical despite different names*

### Comparing `frasa-0.1.3/frasa/datasets/corpus/indonesia/stopword.txt` & `frasa-0.1.4/frasa/datasets/corpus/indonesia/stopword.txt`

 * *Files identical despite different names*

### Comparing `frasa-0.1.3/frasa/datasets/models/frasa-gender.pickle` & `frasa-0.1.4/frasa/datasets/models/frasa-gender.pickle`

 * *Files identical despite different names*

### Comparing `frasa-0.1.3/frasa/deteksi/__init__.py` & `frasa-0.1.4/frasa/deteksi/__init__.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.3/frasa/deteksi/gender/classify.py` & `frasa-0.1.4/frasa/deteksi/gender/classify.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.3/frasa/deteksi/gender/gender.py` & `frasa-0.1.4/frasa/deteksi/gender/gender.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.3/frasa/deteksi/gender/utils.py` & `frasa-0.1.4/frasa/deteksi/gender/utils.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.3/frasa/deteksi/plagiat/cosine.py` & `frasa-0.1.4/frasa/deteksi/plagiat/cosine.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.3/frasa/deteksi/plagiat/jaccard.py` & `frasa-0.1.4/frasa/deteksi/plagiat/jaccard.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.3/frasa/deteksi/plagiat/plagiat.py` & `frasa-0.1.4/frasa/deteksi/plagiat/plagiat.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.3/frasa/deteksi/plagiat/rabin_karp.py` & `frasa-0.1.4/frasa/deteksi/plagiat/rabin_karp.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.3/frasa/preprocess/lemma.py` & `frasa-0.1.4/frasa/preprocess/lemma.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.3/frasa/preprocess/stopword.py` & `frasa-0.1.4/frasa/preprocess/stopword.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.3/frasa/preprocess/token.py` & `frasa-0.1.4/frasa/preprocess/token.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.3/frasa/scrap/detiknews.py` & `frasa-0.1.4/frasa/scrap/detiknews.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.3/frasa/sensor/sensor.py` & `frasa-0.1.4/frasa/sensor/sensor.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.3/frasa/sensor/utils.py` & `frasa-0.1.4/frasa/sensor/utils.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.3/frasa/sensor/variasi.py` & `frasa-0.1.4/frasa/sensor/variasi.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.3/frasa.egg-info/PKG-INFO` & `frasa-0.1.4/frasa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frasa
-Version: 0.1.3
+Version: 0.1.4
 Summary: Koleksi NLP Pribadi untuk Bahasa Indonesia.
 Home-page: https://github.com/novay/frasa
 Author: Novianto Rahmadi
 Author-email: novay@btekno.id
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `frasa-0.1.3/frasa.egg-info/SOURCES.txt` & `frasa-0.1.4/frasa.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,18 @@
 frasa/datasets/corpus/bahasa/__init__.py
 frasa/datasets/corpus/indonesia/__init__.py
 frasa/datasets/corpus/indonesia/stopword.txt
 frasa/datasets/corpus/indonesia/lemma/clitics.txt
 frasa/datasets/corpus/indonesia/lemma/dict.json
 frasa/datasets/corpus/indonesia/lemma/root.txt
 frasa/datasets/corpus/sensor/__init__.py
+frasa/datasets/corpus/sensor/alphabetic_unicode.json
+frasa/datasets/corpus/sensor/sensor-aturan.csv
+frasa/datasets/corpus/sensor/sensor-kata.csv
+frasa/datasets/corpus/sensor/sensor-pengganti.csv
 frasa/datasets/corpus/tweets/__init__.py
 frasa/datasets/models/__init__.py
 frasa/datasets/models/frasa-gender.pickle
 frasa/deteksi/__init__.py
 frasa/deteksi/bahasa/__init__.py
 frasa/deteksi/bahasa/data/__init__.py
 frasa/deteksi/gender/__init__.py
```

### Comparing `frasa-0.1.3/setup.py` & `frasa-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 HERE = path.abspath(path.dirname(__file__))
 
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
     
 setup(
     name="frasa",
-    version="0.1.3",
+    version="0.1.4",
     description="Koleksi NLP Pribadi untuk Bahasa Indonesia.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/novay/frasa",
     author="Novianto Rahmadi",
     author_email="novay@btekno.id",
     license="MIT",
```

