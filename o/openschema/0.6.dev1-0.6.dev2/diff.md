# Comparing `tmp/openschema-0.6.dev1-py3-none-any.whl.zip` & `tmp/openschema-0.6.dev2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 14645 bytes, number of entries: 12
+Zip file size: 14655 bytes, number of entries: 12
 -rw-r--r--  2.0 unx      836 b- defN 20-Feb-02 00:00 openschema/__init__.py
 -rw-r--r--  2.0 unx      944 b- defN 20-Feb-02 00:00 openschema/kaggle/__init__.py
--rw-r--r--  2.0 unx     3067 b- defN 20-Feb-02 00:00 openschema/kaggle/_avazu.py
+-rw-r--r--  2.0 unx     3069 b- defN 20-Feb-02 00:00 openschema/kaggle/_avazu.py
 -rw-r--r--  2.0 unx     2732 b- defN 20-Feb-02 00:00 openschema/kaggle/_titanic.py
 -rw-r--r--  2.0 unx     1010 b- defN 20-Feb-02 00:00 openschema/sklearn/__init__.py
 -rw-r--r--  2.0 unx     6768 b- defN 20-Feb-02 00:00 openschema/sklearn/_breast_cancer.py
 -rw-r--r--  2.0 unx     2458 b- defN 20-Feb-02 00:00 openschema/sklearn/_iris.py
-?rw-r--r--  2.0 unx     3783 b- defN 20-Feb-02 00:00 openschema-0.6.dev1.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 openschema-0.6.dev1.dist-info/WHEEL
-?rw-r--r--  2.0 unx    11358 b- defN 20-Feb-02 00:00 openschema-0.6.dev1.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      124 b- defN 20-Feb-02 00:00 openschema-0.6.dev1.dist-info/licenses/NOTICE
-?rw-r--r--  2.0 unx     1026 b- defN 20-Feb-02 00:00 openschema-0.6.dev1.dist-info/RECORD
-12 files, 34193 bytes uncompressed, 12911 bytes compressed:  62.2%
+?rw-r--r--  2.0 unx     3783 b- defN 20-Feb-02 00:00 openschema-0.6.dev2.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 openschema-0.6.dev2.dist-info/WHEEL
+?rw-r--r--  2.0 unx    11358 b- defN 20-Feb-02 00:00 openschema-0.6.dev2.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      124 b- defN 20-Feb-02 00:00 openschema-0.6.dev2.dist-info/licenses/NOTICE
+?rw-r--r--  2.0 unx     1026 b- defN 20-Feb-02 00:00 openschema-0.6.dev2.dist-info/RECORD
+12 files, 34195 bytes uncompressed, 12921 bytes compressed:  62.2%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: openschema/sklearn/_breast_cancer.py
 Comment: 
 
 Filename: openschema/sklearn/_iris.py
 Comment: 
 
-Filename: openschema-0.6.dev1.dist-info/METADATA
+Filename: openschema-0.6.dev2.dist-info/METADATA
 Comment: 
 
-Filename: openschema-0.6.dev1.dist-info/WHEEL
+Filename: openschema-0.6.dev2.dist-info/WHEEL
 Comment: 
 
-Filename: openschema-0.6.dev1.dist-info/licenses/LICENSE
+Filename: openschema-0.6.dev2.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: openschema-0.6.dev1.dist-info/licenses/NOTICE
+Filename: openschema-0.6.dev2.dist-info/licenses/NOTICE
 Comment: 
 
-Filename: openschema-0.6.dev1.dist-info/RECORD
+Filename: openschema-0.6.dev2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## openschema/__init__.py

```diff
@@ -15,8 +15,8 @@
 # specific language governing permissions and limitations
 # under the License.
 
 """
 Schema catalog.
 """
 
-__version__ = '0.6.dev1'
+__version__ = '0.6.dev2'
```

## openschema/kaggle/_avazu.py

```diff
@@ -35,15 +35,15 @@
     """Click/non-click.
 
     :Values:
         * ``0`` = Non-click
         * ``1`` = Click
     """
 
-    hour = dsl.Field(dsl.Integer())
+    hour = dsl.Field(dsl.Timestamp())
     """Ad request hour.
 
     Format is ``YYMMDDHH``, so ``14091123`` means *23:00* on *Sept. 11, 2014 UTC*.
     """
 
     C1 = dsl.Field(dsl.Integer())
     """Anonymized categorical variable 1."""
```

## Comparing `openschema-0.6.dev1.dist-info/METADATA` & `openschema-0.6.dev2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openschema
-Version: 0.6.dev1
+Version: 0.6.dev2
 Summary: Programmatic catalog of public dataset schemas.
 Project-URL: Source, https://github.com/formlio/openschema/
 Project-URL: Documentation, https://openschema.readthedocs.io/
 Project-URL: Issues, https://github.com/formlio/openschema/issues/
 Maintainer-email: ForML Development Team <info@forml.io>
 License: Apache License 2.0
 License-File: LICENSE
```

## Comparing `openschema-0.6.dev1.dist-info/licenses/LICENSE` & `openschema-0.6.dev2.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `openschema-0.6.dev1.dist-info/RECORD` & `openschema-0.6.dev2.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-openschema/__init__.py,sha256=fyar--jNiw0TPXVc4o3pFSZmX_xJvilAlc8rkeAhQcw,836
+openschema/__init__.py,sha256=Ezl6y_9ZPtUy4YcEQcq39h_dY3jeLfXT4LQJwtTTQAM,836
 openschema/kaggle/__init__.py,sha256=wGr9J5JWX7EZvJNrAW9zcD0vEFBKQ8O4ZbIzG5xHQbs,944
-openschema/kaggle/_avazu.py,sha256=QjI6YUQEzoxeHj-zXx2hJofs7KonHPpWQY5j-khAC3w,3067
+openschema/kaggle/_avazu.py,sha256=qpfGqM2LiwxV4rGm-HpIYCp8Kq15Qpr0KQSy4F2XYXo,3069
 openschema/kaggle/_titanic.py,sha256=d43oRYDq-VXvEpqnaZe9ugUEvT_UPNBArq2gjZi-zBE,2732
 openschema/sklearn/__init__.py,sha256=NVfnTf6KWexY35GPauRsquV2EDJqutQR4yiaFRkUeGU,1010
 openschema/sklearn/_breast_cancer.py,sha256=20GHdNMBiFRrXfyRD7JZqmI8mHGwh59XVVuc7v9NSSU,6768
 openschema/sklearn/_iris.py,sha256=7tzpnlR1aB2mlRGtNjGkKmASi3NXpg86ew3NZHTN7eQ,2458
-openschema-0.6.dev1.dist-info/METADATA,sha256=zN1YAyDsN68eJ_TFZGnJ9cjb9lvfCXt1_Qdl_IvS6p8,3783
-openschema-0.6.dev1.dist-info/WHEEL,sha256=EI2JsGydwUL5GP9t6kzZv7G3HDPi7FuZDDf9In6amRM,87
-openschema-0.6.dev1.dist-info/licenses/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
-openschema-0.6.dev1.dist-info/licenses/NOTICE,sha256=T6XsijfZh4z6h1yyQg-V8-6B5wRvdcFgOOf-dRrPRoE,124
-openschema-0.6.dev1.dist-info/RECORD,,
+openschema-0.6.dev2.dist-info/METADATA,sha256=kR3X2VchZA4ABVp0utwBzp3XFtt0hntswmiyTfjKiuk,3783
+openschema-0.6.dev2.dist-info/WHEEL,sha256=EI2JsGydwUL5GP9t6kzZv7G3HDPi7FuZDDf9In6amRM,87
+openschema-0.6.dev2.dist-info/licenses/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
+openschema-0.6.dev2.dist-info/licenses/NOTICE,sha256=LkiT-HMsWyvE11_z5QKraPAcXF594t0-X4qK5DPWihs,124
+openschema-0.6.dev2.dist-info/RECORD,,
```

