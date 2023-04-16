# Comparing `tmp/paella-0.0.1.dev0-py3-none-any.whl.zip` & `tmp/paella-0.0.1.dev1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,21 @@
-Zip file size: 1149 bytes, number of entries: 4
--rw-rw-r--  2.0 unx      446 b- defN 23-Apr-16 16:10 paella-0.0.1.dev0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-16 16:10 paella-0.0.1.dev0.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-Apr-16 16:10 paella-0.0.1.dev0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      312 b- defN 23-Apr-16 16:10 paella-0.0.1.dev0.dist-info/RECORD
-4 files, 857 bytes uncompressed, 535 bytes compressed:  37.6%
+Zip file size: 26128 bytes, number of entries: 19
+-rw-rw-r--  2.0 unx        0 b- defN 23-Apr-16 16:29 paella/__init__.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Apr-16 16:29 paella/parallel/__init__.py
+-rw-rw-r--  2.0 unx    11576 b- defN 23-Apr-16 16:03 paella/parallel/modules.py
+-rw-rw-r--  2.0 unx     9289 b- defN 23-Apr-16 16:03 paella/parallel/train.py
+-rw-rw-r--  2.0 unx     6034 b- defN 23-Apr-16 16:03 paella/parallel/utils.py
+-rw-rw-r--  2.0 unx     5234 b- defN 23-Apr-16 16:03 paella/parallel/vqgan.py
+-rw-rw-r--  2.0 unx      689 b- defN 23-Apr-16 16:03 paella/parallel/run/run.sh
+-rw-rw-r--  2.0 unx        0 b- defN 23-Apr-16 16:29 paella/single/__init__.py
+-rw-rw-r--  2.0 unx    11454 b- defN 23-Apr-16 16:03 paella/single/modules.py
+-rw-rw-r--  2.0 unx     2975 b- defN 23-Apr-16 16:03 paella/single/train.py
+-rw-rw-r--  2.0 unx     2231 b- defN 23-Apr-16 16:03 paella/single/utils.py
+-rw-rw-r--  2.0 unx     5305 b- defN 23-Apr-16 16:03 paella/single/vqgan.py
+-rw-rw-r--  2.0 unx     2428 b- defN 23-Apr-16 16:03 paella/utils/alter_attention.py
+-rw-rw-r--  2.0 unx    11994 b- defN 23-Apr-16 16:03 paella/utils/modules.py
+-rw-rw-r--  2.0 unx     1071 b- defN 23-Apr-16 16:31 paella-0.0.1.dev1.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     6033 b- defN 23-Apr-16 16:31 paella-0.0.1.dev1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-16 16:31 paella-0.0.1.dev1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Apr-16 16:31 paella-0.0.1.dev1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1534 b- defN 23-Apr-16 16:31 paella-0.0.1.dev1.dist-info/RECORD
+19 files, 77946 bytes uncompressed, 23628 bytes compressed:  69.7%
```

## zipnote {}

```diff
@@ -1,13 +1,58 @@
-Filename: paella-0.0.1.dev0.dist-info/METADATA
+Filename: paella/__init__.py
 Comment: 
 
-Filename: paella-0.0.1.dev0.dist-info/WHEEL
+Filename: paella/parallel/__init__.py
 Comment: 
 
-Filename: paella-0.0.1.dev0.dist-info/top_level.txt
+Filename: paella/parallel/modules.py
 Comment: 
 
-Filename: paella-0.0.1.dev0.dist-info/RECORD
+Filename: paella/parallel/train.py
+Comment: 
+
+Filename: paella/parallel/utils.py
+Comment: 
+
+Filename: paella/parallel/vqgan.py
+Comment: 
+
+Filename: paella/parallel/run/run.sh
+Comment: 
+
+Filename: paella/single/__init__.py
+Comment: 
+
+Filename: paella/single/modules.py
+Comment: 
+
+Filename: paella/single/train.py
+Comment: 
+
+Filename: paella/single/utils.py
+Comment: 
+
+Filename: paella/single/vqgan.py
+Comment: 
+
+Filename: paella/utils/alter_attention.py
+Comment: 
+
+Filename: paella/utils/modules.py
+Comment: 
+
+Filename: paella-0.0.1.dev1.dist-info/LICENSE
+Comment: 
+
+Filename: paella-0.0.1.dev1.dist-info/METADATA
+Comment: 
+
+Filename: paella-0.0.1.dev1.dist-info/WHEEL
+Comment: 
+
+Filename: paella-0.0.1.dev1.dist-info/top_level.txt
+Comment: 
+
+Filename: paella-0.0.1.dev1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

