# Comparing `tmp/sj_tool-1.0.6-py3-none-any.whl.zip` & `tmp/sj_tool-1.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,29 +1,31 @@
-Zip file size: 12105 bytes, number of entries: 27
+Zip file size: 12950 bytes, number of entries: 29
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-14 09:37 sj_tool/__init__.py
 -rw-rw-rw-  2.0 fat      226 b- defN 23-Apr-10 10:09 sj_tool/decorator.py
 -rw-rw-rw-  2.0 fat      476 b- defN 23-Apr-01 13:00 sj_tool/email.py
 -rw-rw-rw-  2.0 fat      476 b- defN 23-Apr-01 13:00 sj_tool/email_sender.py
 -rw-rw-rw-  2.0 fat      155 b- defN 23-Mar-14 09:42 sj_tool/file.py
 -rw-rw-rw-  2.0 fat      313 b- defN 23-Apr-04 05:43 sj_tool/json.py
+-rw-rw-rw-  2.0 fat      335 b- defN 23-Apr-14 09:33 sj_tool/parallel.py
 -rw-rw-rw-  2.0 fat     2180 b- defN 23-Apr-10 10:28 sj_tool/scheduler.py
 -rw-rw-rw-  2.0 fat      245 b- defN 23-Apr-04 05:43 sj_tool/system.py
 -rw-rw-rw-  2.0 fat     1002 b- defN 23-Apr-10 10:05 sj_tool/util.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-14 09:40 sj_tool/db/__init__.py
 -rw-rw-rw-  2.0 fat     5626 b- defN 23-Apr-08 09:02 sj_tool/db/mongo.py
 -rw-rw-rw-  2.0 fat     1237 b- defN 23-Apr-08 08:39 sj_tool/db/mysql.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-27 08:29 sj_tool/fjsp/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-27 08:30 sj_tool/fjsp/entity/__init__.py
--rw-rw-rw-  2.0 fat      565 b- defN 23-Apr-09 06:28 sj_tool/fjsp/entity/changeover.py
+-rw-rw-rw-  2.0 fat      580 b- defN 23-Apr-15 09:09 sj_tool/fjsp/entity/changeover.py
+-rw-rw-rw-  2.0 fat      897 b- defN 23-Apr-10 09:07 sj_tool/fjsp/entity/fjsp_pool.py
 -rw-rw-rw-  2.0 fat      897 b- defN 23-Apr-10 09:07 sj_tool/fjsp/entity/global_pool.py
--rw-rw-rw-  2.0 fat      703 b- defN 23-Apr-09 09:06 sj_tool/fjsp/entity/job.py
+-rw-rw-rw-  2.0 fat      736 b- defN 23-Apr-15 11:54 sj_tool/fjsp/entity/job.py
 -rw-rw-rw-  2.0 fat      411 b- defN 23-Apr-09 05:22 sj_tool/fjsp/entity/machine.py
--rw-rw-rw-  2.0 fat      718 b- defN 23-Apr-09 03:28 sj_tool/fjsp/entity/operation.py
+-rw-rw-rw-  2.0 fat      829 b- defN 23-Apr-15 11:54 sj_tool/fjsp/entity/operation.py
 -rw-rw-rw-  2.0 fat      113 b- defN 23-Apr-09 09:02 sj_tool/fjsp/entity/product.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-30 02:45 sj_tool/logger/__init__.py
 -rw-rw-rw-  2.0 fat     1866 b- defN 23-Apr-08 12:57 sj_tool/logger/text_logger.py
 -rw-rw-rw-  2.0 fat     2718 b- defN 23-Apr-09 03:19 sj_tool/logger/visual_logger.py
--rw-rw-rw-  2.0 fat      492 b- defN 23-Apr-10 10:28 sj_tool-1.0.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-10 10:28 sj_tool-1.0.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-10 10:28 sj_tool-1.0.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     2126 b- defN 23-Apr-10 10:28 sj_tool-1.0.6.dist-info/RECORD
-27 files, 22645 bytes uncompressed, 8683 bytes compressed:  61.7%
+-rw-rw-rw-  2.0 fat      492 b- defN 23-Apr-15 11:54 sj_tool-1.0.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-15 11:54 sj_tool-1.0.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-15 11:54 sj_tool-1.0.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     2289 b- defN 23-Apr-15 11:54 sj_tool-1.0.7.dist-info/RECORD
+29 files, 24199 bytes uncompressed, 9274 bytes compressed:  61.7%
```

## zipnote {}

```diff
@@ -12,14 +12,17 @@
 
 Filename: sj_tool/file.py
 Comment: 
 
 Filename: sj_tool/json.py
 Comment: 
 
+Filename: sj_tool/parallel.py
+Comment: 
+
 Filename: sj_tool/scheduler.py
 Comment: 
 
 Filename: sj_tool/system.py
 Comment: 
 
 Filename: sj_tool/util.py
@@ -39,14 +42,17 @@
 
 Filename: sj_tool/fjsp/entity/__init__.py
 Comment: 
 
 Filename: sj_tool/fjsp/entity/changeover.py
 Comment: 
 
+Filename: sj_tool/fjsp/entity/fjsp_pool.py
+Comment: 
+
 Filename: sj_tool/fjsp/entity/global_pool.py
 Comment: 
 
 Filename: sj_tool/fjsp/entity/job.py
 Comment: 
 
 Filename: sj_tool/fjsp/entity/machine.py
@@ -63,20 +69,20 @@
 
 Filename: sj_tool/logger/text_logger.py
 Comment: 
 
 Filename: sj_tool/logger/visual_logger.py
 Comment: 
 
-Filename: sj_tool-1.0.6.dist-info/METADATA
+Filename: sj_tool-1.0.7.dist-info/METADATA
 Comment: 
 
-Filename: sj_tool-1.0.6.dist-info/WHEEL
+Filename: sj_tool-1.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: sj_tool-1.0.6.dist-info/top_level.txt
+Filename: sj_tool-1.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: sj_tool-1.0.6.dist-info/RECORD
+Filename: sj_tool-1.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sj_tool/fjsp/entity/changeover.py

```diff
@@ -1,15 +1,15 @@
 from typing import Dict
 
 
 class BasicOpInfo(object):
-    def __init__(self, op_type, name, machine_dict: Dict):
+    def __init__(self, op_type, name, machine_times: Dict[int, float]):
         self.op_type = op_type
         self.name = name
-        self.machine_dict = machine_dict
+        self.machine_times = machine_times
 
 
 class Changeover(object):
     def __init__(self):
         self.info = {}
 
     def add(self, pre_mtm, pre_op_type, cur_mtm, cur_op_type, processing_time):
```

## sj_tool/fjsp/entity/job.py

```diff
@@ -1,14 +1,16 @@
 from typing import Union
 
 import pandas as pd
 
 
 class BaseJob(object):
-    def __init__(self, job_id: Union[int, str], product_code, arrival_time: str, ots_time: str, demand: float):
+    def __init__(
+        self, job_id: Union[int, str], product_code: str, arrival_time: str, ots_time: str, demand: Union[int, float]
+    ):
         """
 
         :param job_id:
         :param product_code: 产品编码
         :param arrival_time: job到达时间，即最早可开始时间
         :param ots_time: 截止时间
         :param demand: 需求量
```

## sj_tool/fjsp/entity/operation.py

```diff
@@ -1,12 +1,18 @@
-from typing import List, Tuple, Dict
+from typing import List, Tuple, Dict, Union
 
 
 class BaseOperation:
-    def __init__(self, idx, job_id, op_type, machine_times: Dict[int, float] = None):
+    def __init__(
+        self,
+        idx: Union[int, str],
+        job_id: Union[int, str],
+        op_type: Union[int, str],
+        machine_times: Dict[int, float] = None,
+    ):
         """
 
         :param idx: 工序id
         :param job_id: 工单id
         :param op_type: 工序类型
         :param machine_times: 操作在不同机器上的所需时间列表，例：{1:2,2:2,3:4},
                 其中每个tuple的第一个元素表示机器id，第二个元素表示工序在对应机器上的单个所需时间
```

## Comparing `sj_tool-1.0.6.dist-info/RECORD` & `sj_tool-1.0.7.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 sj_tool/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sj_tool/decorator.py,sha256=nUTxQpiRjmV37SqojRz46vbYmV6N8-wbhF1tejJVeco,226
 sj_tool/email.py,sha256=qxNj5bQ31yzF1bi2XLIxJq5akw-vksZLOS9L5HdM5p8,476
 sj_tool/email_sender.py,sha256=qxNj5bQ31yzF1bi2XLIxJq5akw-vksZLOS9L5HdM5p8,476
 sj_tool/file.py,sha256=NsbZm_9UGni8CKoZEL9mMFwX7u2R2DXA-HtuUS1iaPw,155
 sj_tool/json.py,sha256=yG7paERY6nUtF51kz5ZXp396TKT-UgIyb0teAXeKD5Q,313
+sj_tool/parallel.py,sha256=ocC1AoHAZqSJToS-0o8DaxdANAsbJvRH-Y-wfmLt1PI,335
 sj_tool/scheduler.py,sha256=nSQm7feMCZ8SMeaOqQQ6KkFkwytWXHlMW1fVX7xHYU4,2180
 sj_tool/system.py,sha256=xQxxnAKZ8yW8LJZlw0MhpRyQ_p1LnqwlKnuwgiFdqgI,245
 sj_tool/util.py,sha256=oqnYmmzOa3dPRCNWSHDU_NziY7hODzi73A7xHQ6gcVw,1002
 sj_tool/db/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sj_tool/db/mongo.py,sha256=oUDrhYV_sOq8M9KNFK_QDExCWQ070T1nksp8XzGtDs4,5626
 sj_tool/db/mysql.py,sha256=o9tidq_q9TkDbJXUb6KTMf9O9cJMZeL3rCsADCmroBQ,1237
 sj_tool/fjsp/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sj_tool/fjsp/entity/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-sj_tool/fjsp/entity/changeover.py,sha256=ORGpGQ41ac0ztSqjf48k8Zm3mUl2LXSiupLeBL4rRXY,565
+sj_tool/fjsp/entity/changeover.py,sha256=MabGq1f5T-pUHOBRZdoqSfgqKqraA1CSNJn5Auiicn0,580
+sj_tool/fjsp/entity/fjsp_pool.py,sha256=9-pE3_NIZqVWDM0TrGosycMfzaE1iQov8mSZ3-LZEPo,897
 sj_tool/fjsp/entity/global_pool.py,sha256=9-pE3_NIZqVWDM0TrGosycMfzaE1iQov8mSZ3-LZEPo,897
-sj_tool/fjsp/entity/job.py,sha256=Jj5OGh1-X1LhIfy4WnkffeGL7S0StTUxOnNj0nqCbWA,703
+sj_tool/fjsp/entity/job.py,sha256=r4DGShXcv-K6rnKn5602-X2t6bs3yE1nfcAd3qIMe28,736
 sj_tool/fjsp/entity/machine.py,sha256=zBjVt5VYEuJlqA4yHzzEw9wlbVSAaJHlgj0lweSNaSw,411
-sj_tool/fjsp/entity/operation.py,sha256=_wI52FmRa80I_SvMm5fB0ZX4cQUAmhY3jtbUuN8dgsY,718
+sj_tool/fjsp/entity/operation.py,sha256=nJaMbjFyTJTGkjBg4yokXgwqldMkdbqs7psG-9d6nmo,829
 sj_tool/fjsp/entity/product.py,sha256=IzErQu-Hm0d8rSdWA3Z-HYaYBDmNUbyOMBumYc1dwuU,113
 sj_tool/logger/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sj_tool/logger/text_logger.py,sha256=hNPAxGVOsL46q-9cd-o-S7WV3CL52vlhD7HWKRAeh2Y,1866
 sj_tool/logger/visual_logger.py,sha256=AfKNWJpTb-Odm4gWUyVRXIykiXyvfrdAjukwugCD6os,2718
-sj_tool-1.0.6.dist-info/METADATA,sha256=fqz--AZEPyxo6ebGv7tTlXLOmAZIIIOi3O312CzyLxE,492
-sj_tool-1.0.6.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-sj_tool-1.0.6.dist-info/top_level.txt,sha256=U2pHVPt1Cmde1D9tGeZIoA5KUuo-Urt6Etd-qD5A_cA,8
-sj_tool-1.0.6.dist-info/RECORD,,
+sj_tool-1.0.7.dist-info/METADATA,sha256=D_uAxcooGUPy6Ua36yf8LijfaXymEosDbq0Pnp9tFsw,492
+sj_tool-1.0.7.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+sj_tool-1.0.7.dist-info/top_level.txt,sha256=U2pHVPt1Cmde1D9tGeZIoA5KUuo-Urt6Etd-qD5A_cA,8
+sj_tool-1.0.7.dist-info/RECORD,,
```

