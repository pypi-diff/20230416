# Comparing `tmp/defisheye-1.1.0.tar.gz` & `tmp/defisheye-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "defisheye-1.1.0.tar", last modified: Sat Apr 15 14:07:59 2023, max compression
+gzip compressed data, was "defisheye-1.2.0.tar", last modified: Sun Apr 16 03:26:57 2023, max compression
```

## Comparing `defisheye-1.1.0.tar` & `defisheye-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 14:07:59.093201 defisheye-1.1.0/
--rw-rw-rw-   0        0        0     5776 2023-04-15 14:07:59.084847 defisheye-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     5470 2023-04-15 13:58:18.000000 defisheye-1.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-15 14:07:59.093201 defisheye-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      892 2023-04-15 13:47:38.000000 defisheye-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-15 14:07:59.035705 defisheye-1.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-15 14:07:59.046727 defisheye-1.1.0/src/defisheye/
--rw-rw-rw-   0        0        0      774 2023-04-15 12:41:29.000000 defisheye-1.1.0/src/defisheye/__init__.py
--rw-rw-rw-   0        0        0     4613 2023-04-15 13:49:19.000000 defisheye-1.1.0/src/defisheye/__main__.py
--rw-rw-rw-   0        0        0     5356 2023-04-15 12:41:29.000000 defisheye-1.1.0/src/defisheye/defisheye.py
-drwxrwxrwx   0        0        0        0 2023-04-15 14:07:59.084847 defisheye-1.1.0/src/defisheye.egg-info/
--rw-rw-rw-   0        0        0     5776 2023-04-15 14:07:58.000000 defisheye-1.1.0/src/defisheye.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      321 2023-04-15 14:07:58.000000 defisheye-1.1.0/src/defisheye.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 14:07:58.000000 defisheye-1.1.0/src/defisheye.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-04-15 14:07:58.000000 defisheye-1.1.0/src/defisheye.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       37 2023-04-15 14:07:58.000000 defisheye-1.1.0/src/defisheye.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-15 14:07:58.000000 defisheye-1.1.0/src/defisheye.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 03:26:57.047714 defisheye-1.2.0/
+-rw-rw-rw-   0        0        0     5967 2023-04-16 03:26:57.046614 defisheye-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5661 2023-04-16 03:24:28.000000 defisheye-1.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-16 03:26:57.047714 defisheye-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1047 2023-04-16 02:43:59.000000 defisheye-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 03:26:57.005430 defisheye-1.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-16 03:26:57.017378 defisheye-1.2.0/src/defisheye/
+-rw-rw-rw-   0        0        0      774 2023-04-15 12:41:29.000000 defisheye-1.2.0/src/defisheye/__init__.py
+-rw-rw-rw-   0        0        0     4730 2023-04-16 01:29:23.000000 defisheye-1.2.0/src/defisheye/__main__.py
+-rw-rw-rw-   0        0        0     5356 2023-04-15 12:41:29.000000 defisheye-1.2.0/src/defisheye/defisheye.py
+-rw-rw-rw-   0        0        0     6772 2023-04-16 03:04:01.000000 defisheye-1.2.0/src/defisheye/defisheyeapp.py
+drwxrwxrwx   0        0        0        0 2023-04-16 03:26:57.045612 defisheye-1.2.0/src/defisheye/gui/
+-rw-rw-rw-   0        0        0        0 2023-04-16 00:53:48.000000 defisheye-1.2.0/src/defisheye/gui/__init__.py
+-rw-rw-rw-   0        0        0     1027 2023-04-16 02:05:08.000000 defisheye-1.2.0/src/defisheye/gui/camera.png
+-rw-rw-rw-   0        0        0    11094 2023-04-16 01:04:31.000000 defisheye-1.2.0/src/defisheye/gui/edit-image.png
+-rw-rw-rw-   0        0        0    17271 2023-04-16 01:13:09.000000 defisheye-1.2.0/src/defisheye/gui/image.png
+-rw-rw-rw-   0        0        0     8421 2023-04-16 01:14:18.000000 defisheye-1.2.0/src/defisheye/gui/image200x200.png
+-rw-rw-rw-   0        0        0    14302 2023-04-16 01:52:34.000000 defisheye-1.2.0/src/defisheye/gui/main.ui
+-rw-rw-rw-   0        0        0     1038 2023-04-16 00:55:57.000000 defisheye-1.2.0/src/defisheye/gui/open-image.png
+drwxrwxrwx   0        0        0        0 2023-04-16 03:26:57.032382 defisheye-1.2.0/src/defisheye.egg-info/
+-rw-rw-rw-   0        0        0     5967 2023-04-16 03:26:56.000000 defisheye-1.2.0/src/defisheye.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      565 2023-04-16 03:26:56.000000 defisheye-1.2.0/src/defisheye.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 03:26:56.000000 defisheye-1.2.0/src/defisheye.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       97 2023-04-16 03:26:56.000000 defisheye-1.2.0/src/defisheye.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       51 2023-04-16 03:26:56.000000 defisheye-1.2.0/src/defisheye.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-16 03:26:56.000000 defisheye-1.2.0/src/defisheye.egg-info/top_level.txt
```

### Comparing `defisheye-1.1.0/PKG-INFO` & `defisheye-1.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: defisheye
-Version: 1.1.0
+Version: 1.2.0
 Summary: Fast defisheye algorithm
 Home-page: https://github.com/duducosmos/defisheye
 Author: Eduardo S. Pereira
 Author-email: pereira.somoza@gmail.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -40,14 +40,24 @@
 Process all image in a folder
 
 
 ```bash
 defisheye --images_folder example/images --save_dir example/Defisheye
 ```
 
+### Defisheye App
+
+The GUI version to analyse parameters 
+
+```bash
+defisheyeapp
+```
+
+![App](https://raw.githubusercontent.com/duducosmos/defisheye/master/example/defisheyeapp.png)
+
 
 ### Python Code
 
 ```python
 from defisheye import Defisheye
 
 dtype = 'linear'
```

### Comparing `defisheye-1.1.0/README.md` & `defisheye-1.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,24 @@
 Process all image in a folder
 
 
 ```bash
 defisheye --images_folder example/images --save_dir example/Defisheye
 ```
 
+### Defisheye App
+
+The GUI version to analyse parameters 
+
+```bash
+defisheyeapp
+```
+
+![App](https://raw.githubusercontent.com/duducosmos/defisheye/master/example/defisheyeapp.png)
+
 
 ### Python Code
 
 ```python
 from defisheye import Defisheye
 
 dtype = 'linear'
```

### Comparing `defisheye-1.1.0/setup.py` & `defisheye-1.2.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,24 +7,28 @@
 def read(filename):
     return open(os.path.join(os.path.dirname(__file__), filename)).read()
 
 
 setup(
     name="defisheye",
     license="Apache License 2.0",
-    version='1.1.0',
+    version='1.2.0',
     author='Eduardo S. Pereira',
     author_email='pereira.somoza@gmail.com',
     packages=find_packages("src"),
     package_dir={"": "src"},
+    package_data={"": ["gui/*"]},
     description="Fast defisheye algorithm",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     url="https://github.com/duducosmos/defisheye",
     install_requires=["numpy",
                       "opencv-python",
                       "argcomplete",
-                      'tqdm'
+                      'tqdm',
+                      'pygubu',
+                      'Pillow'
                       ],
     entry_points={"console_scripts": [
-        "defisheye = defisheye.__main__:main"]},
+        "defisheye = defisheye.__main__:main",
+        "defisheyeapp = defisheye.__main__:mainapp"]},
 )
```

### Comparing `defisheye-1.1.0/src/defisheye/__init__.py` & `defisheye-1.2.0/src/defisheye/__init__.py`

 * *Files identical despite different names*

### Comparing `defisheye-1.1.0/src/defisheye/__main__.py` & `defisheye-1.2.0/src/defisheye/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,14 +19,16 @@
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
 """
 import os
 import argparse
 from .defisheye import Defisheye
+from .defisheyeapp import DefisheyeApp
+
 import argcomplete
 from tqdm import tqdm
 
 
 __author__ = "Eduardo S. Pereira"
 __date__ = "02/2023"
 __version__ = "1.1.0"
@@ -53,14 +55,20 @@
         output_image = image_info[1]
         return process_image(input_image, output_image, **kwargs)
 
     for in_out_image in tqdm(list(to_process)):
         individual(in_out_image)
 
 
+def mainapp():
+    app = DefisheyeApp()
+    app.run()
+    return 0
+
+
 def main():
     parser = argparse.ArgumentParser(
         description="Defisheye algorithm")
 
     parser.add_argument("--image", type=str, default=None,
                         help="Input image to process")
```

### Comparing `defisheye-1.1.0/src/defisheye/defisheye.py` & `defisheye-1.2.0/src/defisheye/defisheye.py`

 * *Files identical despite different names*

### Comparing `defisheye-1.1.0/src/defisheye.egg-info/PKG-INFO` & `defisheye-1.2.0/src/defisheye.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: defisheye
-Version: 1.1.0
+Version: 1.2.0
 Summary: Fast defisheye algorithm
 Home-page: https://github.com/duducosmos/defisheye
 Author: Eduardo S. Pereira
 Author-email: pereira.somoza@gmail.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -40,14 +40,24 @@
 Process all image in a folder
 
 
 ```bash
 defisheye --images_folder example/images --save_dir example/Defisheye
 ```
 
+### Defisheye App
+
+The GUI version to analyse parameters 
+
+```bash
+defisheyeapp
+```
+
+![App](https://raw.githubusercontent.com/duducosmos/defisheye/master/example/defisheyeapp.png)
+
 
 ### Python Code
 
 ```python
 from defisheye import Defisheye
 
 dtype = 'linear'
```

