# Comparing `tmp/openlake-0.5.dev1-py3-none-any.whl.zip` & `tmp/openlake-0.5.dev2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 15316 bytes, number of entries: 12
+Zip file size: 15352 bytes, number of entries: 12
 -rw-r--r--  2.0 unx     1832 b- defN 20-Feb-02 00:00 openlake/__init__.py
 -rw-r--r--  2.0 unx     1581 b- defN 20-Feb-02 00:00 openlake/cache.py
 -rw-r--r--  2.0 unx     1884 b- defN 20-Feb-02 00:00 openlake/fetcher.py
 -rw-r--r--  2.0 unx     2031 b- defN 20-Feb-02 00:00 openlake/parser.py
 -rw-r--r--  2.0 unx     3372 b- defN 20-Feb-02 00:00 openlake/provider/__init__.py
--rw-r--r--  2.0 unx     4782 b- defN 20-Feb-02 00:00 openlake/provider/kaggle.py
+-rw-r--r--  2.0 unx     4865 b- defN 20-Feb-02 00:00 openlake/provider/kaggle.py
 -rw-r--r--  2.0 unx     2213 b- defN 20-Feb-02 00:00 openlake/provider/sklearn.py
-?rw-r--r--  2.0 unx     3911 b- defN 20-Feb-02 00:00 openlake-0.5.dev1.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 openlake-0.5.dev1.dist-info/WHEEL
-?rw-r--r--  2.0 unx    11358 b- defN 20-Feb-02 00:00 openlake-0.5.dev1.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      122 b- defN 20-Feb-02 00:00 openlake-0.5.dev1.dist-info/licenses/NOTICE
-?rw-r--r--  2.0 unx      976 b- defN 20-Feb-02 00:00 openlake-0.5.dev1.dist-info/RECORD
-12 files, 34149 bytes uncompressed, 13686 bytes compressed:  59.9%
+?rw-r--r--  2.0 unx     3911 b- defN 20-Feb-02 00:00 openlake-0.5.dev2.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 openlake-0.5.dev2.dist-info/WHEEL
+?rw-r--r--  2.0 unx    11358 b- defN 20-Feb-02 00:00 openlake-0.5.dev2.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      122 b- defN 20-Feb-02 00:00 openlake-0.5.dev2.dist-info/licenses/NOTICE
+?rw-r--r--  2.0 unx      976 b- defN 20-Feb-02 00:00 openlake-0.5.dev2.dist-info/RECORD
+12 files, 34232 bytes uncompressed, 13722 bytes compressed:  59.9%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: openlake/provider/kaggle.py
 Comment: 
 
 Filename: openlake/provider/sklearn.py
 Comment: 
 
-Filename: openlake-0.5.dev1.dist-info/METADATA
+Filename: openlake-0.5.dev2.dist-info/METADATA
 Comment: 
 
-Filename: openlake-0.5.dev1.dist-info/WHEEL
+Filename: openlake-0.5.dev2.dist-info/WHEEL
 Comment: 
 
-Filename: openlake-0.5.dev1.dist-info/licenses/LICENSE
+Filename: openlake-0.5.dev2.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: openlake-0.5.dev1.dist-info/licenses/NOTICE
+Filename: openlake-0.5.dev2.dist-info/licenses/NOTICE
 Comment: 
 
-Filename: openlake-0.5.dev1.dist-info/RECORD
+Filename: openlake-0.5.dev2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## openlake/__init__.py

```diff
@@ -13,15 +13,15 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 """Openlake ForML feed."""
 
-__version__ = '0.5.dev1'
+__version__ = '0.5.dev2'
 
 import typing
 
 from forml.provider.feed import lazy
 
 from openlake.provider import kaggle, sklearn
```

## openlake/provider/kaggle.py

```diff
@@ -136,12 +136,16 @@
                 schema.Avazu.C20,
                 schema.Avazu.C21,
             ),
             'test.gz',
         ),  # Testset partition
         Partition(schema.Avazu.features, 'train.gz'),  # Trainset partition
     )
-    CSV_PARAMS = {'compression': 'gzip'}
+    CSV_PARAMS = {
+        'compression': 'gzip',
+        'parse_dates': ['hour'],
+        'date_format': '%y%m%d%H',
+    }
 
     @property
     def source(self) -> dsl.Source:
         return schema.Avazu
```

## Comparing `openlake-0.5.dev1.dist-info/METADATA` & `openlake-0.5.dev2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlake
-Version: 0.5.dev1
+Version: 0.5.dev2
 Summary: Public dataset feed.
 Project-URL: Source, https://github.com/formlio/openlake/
 Project-URL: Documentation, https://openlake.readthedocs.io/
 Project-URL: Issues, https://github.com/formlio/openlake/issues/
 Maintainer-email: ForML Development Team <info@forml.io>
 License: Apache License 2.0
 License-File: LICENSE
```

## Comparing `openlake-0.5.dev1.dist-info/licenses/LICENSE` & `openlake-0.5.dev2.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `openlake-0.5.dev1.dist-info/RECORD` & `openlake-0.5.dev2.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-openlake/__init__.py,sha256=rxWj134beJuVjbMAtm0jMs4-HWB3YvDp1N1XhsnIoc4,1832
+openlake/__init__.py,sha256=mkvSmssuBdv2xT8c06hp3G7sGsCbvZlXfChRM2InzzM,1832
 openlake/cache.py,sha256=Xt1pBtxdi27fz9K7ed1abRpp_XY9mOr1jim67bMnoLY,1581
 openlake/fetcher.py,sha256=bq7ETig2z-K85_t-dS4twu4IRj4cUuBYeX5vH-cWVh4,1884
 openlake/parser.py,sha256=D0b9Dk5qTYJ_p70TeP-YDtDdRRvyVotl0gJIeGh7_AM,2031
 openlake/provider/__init__.py,sha256=qD1n8Qf4dvc_itEL-WlBZdPUwMvSodEjeT-FojCfLiI,3372
-openlake/provider/kaggle.py,sha256=GNCb5x-C2O8QSylLlq6jlhipNhMHMV1XZ032AMGgp58,4782
+openlake/provider/kaggle.py,sha256=387uL4f2x81Dn2HXZ3_PVxwVkztexSq-VNDg4yUBXZw,4865
 openlake/provider/sklearn.py,sha256=JABZYL5RrIsFr_FVub8VX5-sTg7OKz6lQ_fIH_ogspU,2213
-openlake-0.5.dev1.dist-info/METADATA,sha256=Yij3v2Xr5f-JGHFu2V4moV5cHz8CU8mjeKIOY78AG_Q,3911
-openlake-0.5.dev1.dist-info/WHEEL,sha256=EI2JsGydwUL5GP9t6kzZv7G3HDPi7FuZDDf9In6amRM,87
-openlake-0.5.dev1.dist-info/licenses/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
-openlake-0.5.dev1.dist-info/licenses/NOTICE,sha256=xbb-byT8Cde4kQDdI0OTYPzVJQEG135aaEQjJqeDYJY,122
-openlake-0.5.dev1.dist-info/RECORD,,
+openlake-0.5.dev2.dist-info/METADATA,sha256=0TgTIP0E78BwngVNrYBSCJlbRQGIhof_wjvbeQhU7D0,3911
+openlake-0.5.dev2.dist-info/WHEEL,sha256=EI2JsGydwUL5GP9t6kzZv7G3HDPi7FuZDDf9In6amRM,87
+openlake-0.5.dev2.dist-info/licenses/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
+openlake-0.5.dev2.dist-info/licenses/NOTICE,sha256=uDVKzYIrESArI709R0OUcBXhlWpbzSSuCG47c9v3pVI,122
+openlake-0.5.dev2.dist-info/RECORD,,
```

