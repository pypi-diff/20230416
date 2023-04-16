# Comparing `tmp/mb_pytorch-1.0.202304151245-py3-none-any.whl.zip` & `tmp/mb_pytorch-1.0.202304160116-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
 Zip file size: 29617 bytes, number of entries: 36
--rw-rw-r--  2.0 unx     5492 b- defN 23-Apr-14 17:37 mb_pytorch/classification/training.py
+-rw-rw-r--  2.0 unx     5492 b- defN 23-Apr-16 01:15 mb_pytorch/classification/training.py
 -rw-rw-r--  2.0 unx       44 b- defN 23-Mar-16 11:39 mb_pytorch/dataloader/__init__.py
 -rw-rw-r--  2.0 unx    12157 b- defN 23-Apr-14 17:23 mb_pytorch/dataloader/loader.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Feb-23 13:56 mb_pytorch/metalearning/__init__.py
 -rw-rw-r--  2.0 unx     1385 b- defN 23-Mar-02 03:28 mb_pytorch/metalearning/meta_utils.py
 -rw-rw-r--  2.0 unx     1030 b- defN 23-Mar-15 02:58 mb_pytorch/metalearning/proto_dataloader.py
 -rw-rw-r--  2.0 unx     2861 b- defN 23-Mar-03 23:55 mb_pytorch/metalearning/prototypical.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Mar-31 19:54 mb_pytorch/models/__init__.py
@@ -25,14 +25,14 @@
 -rw-rw-r--  2.0 unx      257 b- defN 23-Mar-01 22:55 mb_pytorch/utils/dist.py
 -rw-rw-r--  2.0 unx     3391 b- defN 23-Apr-11 23:28 mb_pytorch/utils/extra_utils.py
 -rw-rw-r--  2.0 unx     7178 b- defN 23-Mar-15 02:58 mb_pytorch/utils/generate_emb.py
 -rw-rw-r--  2.0 unx     2582 b- defN 23-Apr-03 19:30 mb_pytorch/utils/losses.py
 -rw-rw-r--  2.0 unx     1199 b- defN 23-Apr-04 20:14 mb_pytorch/utils/metrics.py
 -rw-rw-r--  2.0 unx     6220 b- defN 23-Apr-13 20:59 mb_pytorch/utils/viewer.py
 -rw-rw-r--  2.0 unx      994 b- defN 23-Mar-06 13:11 mb_pytorch/utils/yaml_reader.py
--rwxrwxr-x  2.0 unx     1304 b- defN 23-Apr-15 12:45 mb_pytorch-1.0.202304151245.data/scripts/dataload_results.py
--rwxrwxr-x  2.0 unx      980 b- defN 23-Mar-15 02:59 mb_pytorch-1.0.202304151245.data/scripts/emb.py
--rw-rw-r--  2.0 unx      329 b- defN 23-Apr-15 12:45 mb_pytorch-1.0.202304151245.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-15 12:45 mb_pytorch-1.0.202304151245.dist-info/WHEEL
--rw-rw-r--  2.0 unx       11 b- defN 23-Apr-15 12:45 mb_pytorch-1.0.202304151245.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     3256 b- defN 23-Apr-15 12:45 mb_pytorch-1.0.202304151245.dist-info/RECORD
+-rwxrwxr-x  2.0 unx     1304 b- defN 23-Apr-16 01:16 mb_pytorch-1.0.202304160116.data/scripts/dataload_results.py
+-rwxrwxr-x  2.0 unx      980 b- defN 23-Mar-15 02:59 mb_pytorch-1.0.202304160116.data/scripts/emb.py
+-rw-rw-r--  2.0 unx      329 b- defN 23-Apr-16 01:16 mb_pytorch-1.0.202304160116.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-16 01:16 mb_pytorch-1.0.202304160116.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       11 b- defN 23-Apr-16 01:16 mb_pytorch-1.0.202304160116.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     3256 b- defN 23-Apr-16 01:16 mb_pytorch-1.0.202304160116.dist-info/RECORD
 36 files, 86368 bytes uncompressed, 24297 bytes compressed:  71.9%
```

## zipnote {}

```diff
@@ -84,26 +84,26 @@
 
 Filename: mb_pytorch/utils/viewer.py
 Comment: 
 
 Filename: mb_pytorch/utils/yaml_reader.py
 Comment: 
 
-Filename: mb_pytorch-1.0.202304151245.data/scripts/dataload_results.py
+Filename: mb_pytorch-1.0.202304160116.data/scripts/dataload_results.py
 Comment: 
 
-Filename: mb_pytorch-1.0.202304151245.data/scripts/emb.py
+Filename: mb_pytorch-1.0.202304160116.data/scripts/emb.py
 Comment: 
 
-Filename: mb_pytorch-1.0.202304151245.dist-info/METADATA
+Filename: mb_pytorch-1.0.202304160116.dist-info/METADATA
 Comment: 
 
-Filename: mb_pytorch-1.0.202304151245.dist-info/WHEEL
+Filename: mb_pytorch-1.0.202304160116.dist-info/WHEEL
 Comment: 
 
-Filename: mb_pytorch-1.0.202304151245.dist-info/top_level.txt
+Filename: mb_pytorch-1.0.202304160116.dist-info/top_level.txt
 Comment: 
 
-Filename: mb_pytorch-1.0.202304151245.dist-info/RECORD
+Filename: mb_pytorch-1.0.202304160116.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `mb_pytorch-1.0.202304151245.data/scripts/dataload_results.py` & `mb_pytorch-1.0.202304160116.data/scripts/dataload_results.py`

 * *Files identical despite different names*

## Comparing `mb_pytorch-1.0.202304151245.data/scripts/emb.py` & `mb_pytorch-1.0.202304160116.data/scripts/emb.py`

 * *Files identical despite different names*

## Comparing `mb_pytorch-1.0.202304151245.dist-info/RECORD` & `mb_pytorch-1.0.202304160116.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -24,13 +24,13 @@
 mb_pytorch/utils/dist.py,sha256=7-ZdntmiugRWYnT5wileo8mYTuV1dbjVl4ffJsfnfAw,257
 mb_pytorch/utils/extra_utils.py,sha256=-MaT-x3gwgEOVLpg-tWm5yLFtI0CxpV0QUlXx-rqu08,3391
 mb_pytorch/utils/generate_emb.py,sha256=2iK8wRIrYfaLpEgjdbFnDqGU5ux-1JhncQoeboW_6LQ,7178
 mb_pytorch/utils/losses.py,sha256=OLCPLkJH46IofSSVly2xdcklVv7Q5OFFEGtVrJcV7V0,2582
 mb_pytorch/utils/metrics.py,sha256=Kqmdu9llSjR8aRp3IVlmy6PqeQexf0ZXjTJUcEtvcfI,1199
 mb_pytorch/utils/viewer.py,sha256=tHdAPjUbGmrNgJQICc-8pLPc9VJB0Qr0JdeGtQMq4os,6220
 mb_pytorch/utils/yaml_reader.py,sha256=Azgr_5qttsH_BBVsCtfccFMvK6IEjTRYhd5qp4S5uzk,994
-mb_pytorch-1.0.202304151245.data/scripts/dataload_results.py,sha256=8IFAH7WX-nSJ7V532rr3Cl7R37v0jhSakw0JCd9dalE,1304
-mb_pytorch-1.0.202304151245.data/scripts/emb.py,sha256=5jSbTGNOhusDTvHZeaTwk4pmJa4HIdkRGd98s0L4Rl0,980
-mb_pytorch-1.0.202304151245.dist-info/METADATA,sha256=zVdDZLEIiN7Qhm3qWZThD0ywkoN1jiUkBbO0stwWAT0,329
-mb_pytorch-1.0.202304151245.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-mb_pytorch-1.0.202304151245.dist-info/top_level.txt,sha256=2m_aBiEfjq3pZM2NtYSlTqlgoQxH6WaK8_8SsRicIvg,11
-mb_pytorch-1.0.202304151245.dist-info/RECORD,,
+mb_pytorch-1.0.202304160116.data/scripts/dataload_results.py,sha256=8IFAH7WX-nSJ7V532rr3Cl7R37v0jhSakw0JCd9dalE,1304
+mb_pytorch-1.0.202304160116.data/scripts/emb.py,sha256=5jSbTGNOhusDTvHZeaTwk4pmJa4HIdkRGd98s0L4Rl0,980
+mb_pytorch-1.0.202304160116.dist-info/METADATA,sha256=fwsbZaLjPjKZRoupQVdktxbY28lZTccWMOKxuuokbBE,329
+mb_pytorch-1.0.202304160116.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+mb_pytorch-1.0.202304160116.dist-info/top_level.txt,sha256=2m_aBiEfjq3pZM2NtYSlTqlgoQxH6WaK8_8SsRicIvg,11
+mb_pytorch-1.0.202304160116.dist-info/RECORD,,
```

