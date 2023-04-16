# Comparing `tmp/defisheye-1.2.0.tar.gz` & `tmp/defisheye-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "defisheye-1.2.0.tar", last modified: Sun Apr 16 03:26:57 2023, max compression
+gzip compressed data, was "defisheye-1.2.1.tar", last modified: Sun Apr 16 15:41:34 2023, max compression
```

## Comparing `defisheye-1.2.0.tar` & `defisheye-1.2.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 03:26:57.047714 defisheye-1.2.0/
--rw-rw-rw-   0        0        0     5967 2023-04-16 03:26:57.046614 defisheye-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     5661 2023-04-16 03:24:28.000000 defisheye-1.2.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-16 03:26:57.047714 defisheye-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1047 2023-04-16 02:43:59.000000 defisheye-1.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-16 03:26:57.005430 defisheye-1.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-16 03:26:57.017378 defisheye-1.2.0/src/defisheye/
--rw-rw-rw-   0        0        0      774 2023-04-15 12:41:29.000000 defisheye-1.2.0/src/defisheye/__init__.py
--rw-rw-rw-   0        0        0     4730 2023-04-16 01:29:23.000000 defisheye-1.2.0/src/defisheye/__main__.py
--rw-rw-rw-   0        0        0     5356 2023-04-15 12:41:29.000000 defisheye-1.2.0/src/defisheye/defisheye.py
--rw-rw-rw-   0        0        0     6772 2023-04-16 03:04:01.000000 defisheye-1.2.0/src/defisheye/defisheyeapp.py
-drwxrwxrwx   0        0        0        0 2023-04-16 03:26:57.045612 defisheye-1.2.0/src/defisheye/gui/
--rw-rw-rw-   0        0        0        0 2023-04-16 00:53:48.000000 defisheye-1.2.0/src/defisheye/gui/__init__.py
--rw-rw-rw-   0        0        0     1027 2023-04-16 02:05:08.000000 defisheye-1.2.0/src/defisheye/gui/camera.png
--rw-rw-rw-   0        0        0    11094 2023-04-16 01:04:31.000000 defisheye-1.2.0/src/defisheye/gui/edit-image.png
--rw-rw-rw-   0        0        0    17271 2023-04-16 01:13:09.000000 defisheye-1.2.0/src/defisheye/gui/image.png
--rw-rw-rw-   0        0        0     8421 2023-04-16 01:14:18.000000 defisheye-1.2.0/src/defisheye/gui/image200x200.png
--rw-rw-rw-   0        0        0    14302 2023-04-16 01:52:34.000000 defisheye-1.2.0/src/defisheye/gui/main.ui
--rw-rw-rw-   0        0        0     1038 2023-04-16 00:55:57.000000 defisheye-1.2.0/src/defisheye/gui/open-image.png
-drwxrwxrwx   0        0        0        0 2023-04-16 03:26:57.032382 defisheye-1.2.0/src/defisheye.egg-info/
--rw-rw-rw-   0        0        0     5967 2023-04-16 03:26:56.000000 defisheye-1.2.0/src/defisheye.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      565 2023-04-16 03:26:56.000000 defisheye-1.2.0/src/defisheye.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 03:26:56.000000 defisheye-1.2.0/src/defisheye.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       97 2023-04-16 03:26:56.000000 defisheye-1.2.0/src/defisheye.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       51 2023-04-16 03:26:56.000000 defisheye-1.2.0/src/defisheye.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-16 03:26:56.000000 defisheye-1.2.0/src/defisheye.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 15:41:34.298793 defisheye-1.2.1/
+-rw-rw-rw-   0        0        0     6387 2023-04-16 15:41:34.298793 defisheye-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6081 2023-04-16 15:37:57.000000 defisheye-1.2.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-16 15:41:34.298793 defisheye-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1047 2023-04-16 15:41:19.000000 defisheye-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 15:41:34.251050 defisheye-1.2.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-16 15:41:34.259357 defisheye-1.2.1/src/defisheye/
+-rw-rw-rw-   0        0        0      774 2023-04-15 12:41:29.000000 defisheye-1.2.1/src/defisheye/__init__.py
+-rw-rw-rw-   0        0        0     4730 2023-04-16 01:29:23.000000 defisheye-1.2.1/src/defisheye/__main__.py
+-rw-rw-rw-   0        0        0     5356 2023-04-15 12:41:29.000000 defisheye-1.2.1/src/defisheye/defisheye.py
+-rw-rw-rw-   0        0        0     6772 2023-04-16 03:04:01.000000 defisheye-1.2.1/src/defisheye/defisheyeapp.py
+drwxrwxrwx   0        0        0        0 2023-04-16 15:41:34.293745 defisheye-1.2.1/src/defisheye/gui/
+-rw-rw-rw-   0        0        0        0 2023-04-16 00:53:48.000000 defisheye-1.2.1/src/defisheye/gui/__init__.py
+-rw-rw-rw-   0        0        0     1027 2023-04-16 02:05:08.000000 defisheye-1.2.1/src/defisheye/gui/camera.png
+-rw-rw-rw-   0        0        0    11094 2023-04-16 01:04:31.000000 defisheye-1.2.1/src/defisheye/gui/edit-image.png
+-rw-rw-rw-   0        0        0    17271 2023-04-16 01:13:09.000000 defisheye-1.2.1/src/defisheye/gui/image.png
+-rw-rw-rw-   0        0        0     8421 2023-04-16 01:14:18.000000 defisheye-1.2.1/src/defisheye/gui/image200x200.png
+-rw-rw-rw-   0        0        0    14302 2023-04-16 01:52:34.000000 defisheye-1.2.1/src/defisheye/gui/main.ui
+-rw-rw-rw-   0        0        0     1038 2023-04-16 00:55:57.000000 defisheye-1.2.1/src/defisheye/gui/open-image.png
+drwxrwxrwx   0        0        0        0 2023-04-16 15:41:34.284425 defisheye-1.2.1/src/defisheye.egg-info/
+-rw-rw-rw-   0        0        0     6387 2023-04-16 15:41:34.000000 defisheye-1.2.1/src/defisheye.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      565 2023-04-16 15:41:34.000000 defisheye-1.2.1/src/defisheye.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 15:41:34.000000 defisheye-1.2.1/src/defisheye.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       97 2023-04-16 15:41:34.000000 defisheye-1.2.1/src/defisheye.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       51 2023-04-16 15:41:34.000000 defisheye-1.2.1/src/defisheye.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-16 15:41:34.000000 defisheye-1.2.1/src/defisheye.egg-info/top_level.txt
```

### Comparing `defisheye-1.2.0/PKG-INFO` & `defisheye-1.2.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: defisheye
-Version: 1.2.0
-Summary: Fast defisheye algorithm
-Home-page: https://github.com/duducosmos/defisheye
-Author: Eduardo S. Pereira
-Author-email: pereira.somoza@gmail.com
-License: Apache License 2.0
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-
 # Defisheye
 
 Fast Corrects for fisheye distortion in an image.
 
 Defisheye is designed to transform a fisheye image into a normal perspective
 view looking towards the center of the fisheye image.
 
@@ -157,36 +146,36 @@
 ANGLE is the clockwise positive rotation angle for the output perspective
 image relative to the orientation of the input fisheye image. Values are
 non-negative floats in range 0<=angle<360. The default is 0.
 
 ## Example
 
 Original
-![Original](./example/images/example3.jpg)
+![Original](https://raw.githubusercontent.com/duducosmos/defisheye/master/example/images/example3.jpg)
 
 pfov = 120
 
 Equal area  Circular
-![Equal Area](./example/images/out/example3_equalarea_circular_120.jpg)
+![Equal Area](https://raw.githubusercontent.com/duducosmos/defisheye/master/example/images/out/example3_equalarea_circular_120.jpg)
 
 Equal area Fullframe
-![Equal Area](./example/images/out/example3_equalarea_fullframe_120.jpg)
+![Equal Area](https://raw.githubusercontent.com/duducosmos/defisheye/master/example/images/out/example3_equalarea_fullframe_120.jpg)
 
 Linear  Circular
-![Equal Area](./example/images/out/example3_linear_circular_120.jpg)
+![Equal Area](https://raw.githubusercontent.com/duducosmos/defisheye/master/example/images/out/example3_linear_circular_120.jpg)
 
 Linear Fullframe
-![Equal Area](./example/images/out/example3_linear_fullframe_120.jpg)
+![Equal Area](https://raw.githubusercontent.com/duducosmos/defisheye/master/example/images/out/example3_linear_fullframe_120.jpg)
 
 
 orthographic  Circular
-![Equal Area](./example/images/out/example3_orthographic_circular_120.jpg)
+![Equal Area](https://raw.githubusercontent.com/duducosmos/defisheye/master/example/images/out/example3_orthographic_circular_120.jpg)
 
 Stereographic Circular
-![Equal Area](./example/images/out/example3_stereographic_circular_120.jpg)
+![Equal Area](https://raw.githubusercontent.com/duducosmos/defisheye/master/example/images/out/example3_stereographic_circular_120.jpg)
 
 
 ## Extra
 Developed by: E. S. Pereira.
 e-mail: pereira.somoza@gmail.com
 
 Based in the work of F. Weinhaus.
@@ -201,9 +190,7 @@
        http://www.apache.org/licenses/LICENSE-2.0
 
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
-
-
```

### Comparing `defisheye-1.2.0/README.md` & `defisheye-1.2.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: defisheye
+Version: 1.2.1
+Summary: Fast defisheye algorithm
+Home-page: https://github.com/duducosmos/defisheye
+Author: Eduardo S. Pereira
+Author-email: pereira.somoza@gmail.com
+License: Apache License 2.0
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+
 # Defisheye
 
 Fast Corrects for fisheye distortion in an image.
 
 Defisheye is designed to transform a fisheye image into a normal perspective
 view looking towards the center of the fisheye image.
 
@@ -146,36 +157,36 @@
 ANGLE is the clockwise positive rotation angle for the output perspective
 image relative to the orientation of the input fisheye image. Values are
 non-negative floats in range 0<=angle<360. The default is 0.
 
 ## Example
 
 Original
-![Original](./example/images/example3.jpg)
+![Original](https://raw.githubusercontent.com/duducosmos/defisheye/master/example/images/example3.jpg)
 
 pfov = 120
 
 Equal area  Circular
-![Equal Area](./example/images/out/example3_equalarea_circular_120.jpg)
+![Equal Area](https://raw.githubusercontent.com/duducosmos/defisheye/master/example/images/out/example3_equalarea_circular_120.jpg)
 
 Equal area Fullframe
-![Equal Area](./example/images/out/example3_equalarea_fullframe_120.jpg)
+![Equal Area](https://raw.githubusercontent.com/duducosmos/defisheye/master/example/images/out/example3_equalarea_fullframe_120.jpg)
 
 Linear  Circular
-![Equal Area](./example/images/out/example3_linear_circular_120.jpg)
+![Equal Area](https://raw.githubusercontent.com/duducosmos/defisheye/master/example/images/out/example3_linear_circular_120.jpg)
 
 Linear Fullframe
-![Equal Area](./example/images/out/example3_linear_fullframe_120.jpg)
+![Equal Area](https://raw.githubusercontent.com/duducosmos/defisheye/master/example/images/out/example3_linear_fullframe_120.jpg)
 
 
 orthographic  Circular
-![Equal Area](./example/images/out/example3_orthographic_circular_120.jpg)
+![Equal Area](https://raw.githubusercontent.com/duducosmos/defisheye/master/example/images/out/example3_orthographic_circular_120.jpg)
 
 Stereographic Circular
-![Equal Area](./example/images/out/example3_stereographic_circular_120.jpg)
+![Equal Area](https://raw.githubusercontent.com/duducosmos/defisheye/master/example/images/out/example3_stereographic_circular_120.jpg)
 
 
 ## Extra
 Developed by: E. S. Pereira.
 e-mail: pereira.somoza@gmail.com
 
 Based in the work of F. Weinhaus.
@@ -190,7 +201,9 @@
        http://www.apache.org/licenses/LICENSE-2.0
 
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
+
+
```

### Comparing `defisheye-1.2.0/setup.py` & `defisheye-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def read(filename):
     return open(os.path.join(os.path.dirname(__file__), filename)).read()
 
 
 setup(
     name="defisheye",
     license="Apache License 2.0",
-    version='1.2.0',
+    version='1.2.1',
     author='Eduardo S. Pereira',
     author_email='pereira.somoza@gmail.com',
     packages=find_packages("src"),
     package_dir={"": "src"},
     package_data={"": ["gui/*"]},
     description="Fast defisheye algorithm",
     long_description=read("README.md"),
```

### Comparing `defisheye-1.2.0/src/defisheye/__init__.py` & `defisheye-1.2.1/src/defisheye/__init__.py`

 * *Files identical despite different names*

### Comparing `defisheye-1.2.0/src/defisheye/__main__.py` & `defisheye-1.2.1/src/defisheye/__main__.py`

 * *Files identical despite different names*

### Comparing `defisheye-1.2.0/src/defisheye/defisheye.py` & `defisheye-1.2.1/src/defisheye/defisheye.py`

 * *Files identical despite different names*

### Comparing `defisheye-1.2.0/src/defisheye/defisheyeapp.py` & `defisheye-1.2.1/src/defisheye/defisheyeapp.py`

 * *Files identical despite different names*

### Comparing `defisheye-1.2.0/src/defisheye/gui/camera.png` & `defisheye-1.2.1/src/defisheye/gui/camera.png`

 * *Files identical despite different names*

### Comparing `defisheye-1.2.0/src/defisheye/gui/edit-image.png` & `defisheye-1.2.1/src/defisheye/gui/edit-image.png`

 * *Files identical despite different names*

### Comparing `defisheye-1.2.0/src/defisheye/gui/image.png` & `defisheye-1.2.1/src/defisheye/gui/image.png`

 * *Files identical despite different names*

### Comparing `defisheye-1.2.0/src/defisheye/gui/image200x200.png` & `defisheye-1.2.1/src/defisheye/gui/image200x200.png`

 * *Files identical despite different names*

### Comparing `defisheye-1.2.0/src/defisheye/gui/main.ui` & `defisheye-1.2.1/src/defisheye/gui/main.ui`

 * *Files identical despite different names*

### Comparing `defisheye-1.2.0/src/defisheye/gui/open-image.png` & `defisheye-1.2.1/src/defisheye/gui/open-image.png`

 * *Files identical despite different names*

### Comparing `defisheye-1.2.0/src/defisheye.egg-info/PKG-INFO` & `defisheye-1.2.1/src/defisheye.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: defisheye
-Version: 1.2.0
+Version: 1.2.1
 Summary: Fast defisheye algorithm
 Home-page: https://github.com/duducosmos/defisheye
 Author: Eduardo S. Pereira
 Author-email: pereira.somoza@gmail.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -157,36 +157,36 @@
 ANGLE is the clockwise positive rotation angle for the output perspective
 image relative to the orientation of the input fisheye image. Values are
 non-negative floats in range 0<=angle<360. The default is 0.
 
 ## Example
 
 Original
-![Original](./example/images/example3.jpg)
+![Original](https://raw.githubusercontent.com/duducosmos/defisheye/master/example/images/example3.jpg)
 
 pfov = 120
 
 Equal area  Circular
-![Equal Area](./example/images/out/example3_equalarea_circular_120.jpg)
+![Equal Area](https://raw.githubusercontent.com/duducosmos/defisheye/master/example/images/out/example3_equalarea_circular_120.jpg)
 
 Equal area Fullframe
-![Equal Area](./example/images/out/example3_equalarea_fullframe_120.jpg)
+![Equal Area](https://raw.githubusercontent.com/duducosmos/defisheye/master/example/images/out/example3_equalarea_fullframe_120.jpg)
 
 Linear  Circular
-![Equal Area](./example/images/out/example3_linear_circular_120.jpg)
+![Equal Area](https://raw.githubusercontent.com/duducosmos/defisheye/master/example/images/out/example3_linear_circular_120.jpg)
 
 Linear Fullframe
-![Equal Area](./example/images/out/example3_linear_fullframe_120.jpg)
+![Equal Area](https://raw.githubusercontent.com/duducosmos/defisheye/master/example/images/out/example3_linear_fullframe_120.jpg)
 
 
 orthographic  Circular
-![Equal Area](./example/images/out/example3_orthographic_circular_120.jpg)
+![Equal Area](https://raw.githubusercontent.com/duducosmos/defisheye/master/example/images/out/example3_orthographic_circular_120.jpg)
 
 Stereographic Circular
-![Equal Area](./example/images/out/example3_stereographic_circular_120.jpg)
+![Equal Area](https://raw.githubusercontent.com/duducosmos/defisheye/master/example/images/out/example3_stereographic_circular_120.jpg)
 
 
 ## Extra
 Developed by: E. S. Pereira.
 e-mail: pereira.somoza@gmail.com
 
 Based in the work of F. Weinhaus.
```

### Comparing `defisheye-1.2.0/src/defisheye.egg-info/SOURCES.txt` & `defisheye-1.2.1/src/defisheye.egg-info/SOURCES.txt`

 * *Files identical despite different names*

