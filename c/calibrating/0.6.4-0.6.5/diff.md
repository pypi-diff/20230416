# Comparing `tmp/calibrating-0.6.4.tar.gz` & `tmp/calibrating-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/calibrating-0.6.4.tar", last modified: Fri Apr 14 07:58:52 2023, max compression
+gzip compressed data, was "dist/calibrating-0.6.5.tar", last modified: Sun Apr 16 15:29:30 2023, max compression
```

## Comparing `calibrating-0.6.4.tar` & `calibrating-0.6.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2023-04-14 07:58:52.000000 calibrating-0.6.4/
--rw-rw-r--   0 dl        (1000) dl        (1000)       35 2021-08-19 08:36:59.000000 calibrating-0.6.4/MANIFEST.in
--rw-rw-r--   0 dl        (1000) dl        (1000)      647 2023-04-14 07:58:52.000000 calibrating-0.6.4/PKG-INFO
--rw-rw-r--   0 dl        (1000) dl        (1000)     5544 2023-01-11 07:48:52.000000 calibrating-0.6.4/README.md
-drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2023-04-14 07:58:52.000000 calibrating-0.6.4/calibrating/
--rw-rw-r--   0 dl        (1000) dl        (1000)      643 2023-04-14 07:58:23.000000 calibrating-0.6.4/calibrating/__info__.py
--rw-rw-r--   0 dl        (1000) dl        (1000)      249 2022-12-22 13:24:45.000000 calibrating-0.6.4/calibrating/__init__.py
--rw-rw-r--   0 dl        (1000) dl        (1000)    18329 2023-04-14 05:58:51.000000 calibrating-0.6.4/calibrating/boards.py
--rw-rw-r--   0 dl        (1000) dl        (1000)    21801 2023-04-14 05:38:18.000000 calibrating-0.6.4/calibrating/camera.py
--rw-rw-r--   0 dl        (1000) dl        (1000)     1521 2022-12-22 17:59:18.000000 calibrating-0.6.4/calibrating/feature_libs.py
--rw-rw-r--   0 dl        (1000) dl        (1000)     4730 2023-02-07 10:00:28.000000 calibrating-0.6.4/calibrating/multi_boards.py
--rw-rw-r--   0 dl        (1000) dl        (1000)     3200 2022-12-22 13:14:32.000000 calibrating-0.6.4/calibrating/reconstruction.py
--rw-rw-r--   0 dl        (1000) dl        (1000)    21305 2023-04-13 11:51:43.000000 calibrating-0.6.4/calibrating/stereo.py
--rw-rw-r--   0 dl        (1000) dl        (1000)    25439 2023-04-14 05:50:57.000000 calibrating-0.6.4/calibrating/utils.py
-drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2023-04-14 07:58:52.000000 calibrating-0.6.4/calibrating.egg-info/
--rw-rw-r--   0 dl        (1000) dl        (1000)      647 2023-04-14 07:58:52.000000 calibrating-0.6.4/calibrating.egg-info/PKG-INFO
--rw-rw-r--   0 dl        (1000) dl        (1000)      442 2023-04-14 07:58:52.000000 calibrating-0.6.4/calibrating.egg-info/SOURCES.txt
--rw-rw-r--   0 dl        (1000) dl        (1000)        1 2023-04-14 07:58:52.000000 calibrating-0.6.4/calibrating.egg-info/dependency_links.txt
--rw-rw-r--   0 dl        (1000) dl        (1000)       54 2023-04-14 07:58:52.000000 calibrating-0.6.4/calibrating.egg-info/requires.txt
--rw-rw-r--   0 dl        (1000) dl        (1000)       12 2023-04-14 07:58:52.000000 calibrating-0.6.4/calibrating.egg-info/top_level.txt
--rw-rw-r--   0 dl        (1000) dl        (1000)       54 2022-09-30 10:04:15.000000 calibrating-0.6.4/requirements.txt
--rw-rw-r--   0 dl        (1000) dl        (1000)       38 2023-04-14 07:58:52.000000 calibrating-0.6.4/setup.cfg
--rw-rw-r--   0 dl        (1000) dl        (1000)      853 2021-08-19 08:44:30.000000 calibrating-0.6.4/setup.py
+drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2023-04-16 15:29:30.000000 calibrating-0.6.5/
+-rw-rw-r--   0 dl        (1000) dl        (1000)       35 2021-08-19 08:36:59.000000 calibrating-0.6.5/MANIFEST.in
+-rw-rw-r--   0 dl        (1000) dl        (1000)      647 2023-04-16 15:29:30.000000 calibrating-0.6.5/PKG-INFO
+-rw-rw-r--   0 dl        (1000) dl        (1000)     5544 2023-01-11 07:48:52.000000 calibrating-0.6.5/README.md
+drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2023-04-16 15:29:30.000000 calibrating-0.6.5/calibrating/
+-rw-rw-r--   0 dl        (1000) dl        (1000)      643 2023-04-16 15:28:31.000000 calibrating-0.6.5/calibrating/__info__.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)      249 2022-12-22 13:24:45.000000 calibrating-0.6.5/calibrating/__init__.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)    18323 2023-04-16 15:28:48.000000 calibrating-0.6.5/calibrating/boards.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)    21801 2023-04-14 05:38:18.000000 calibrating-0.6.5/calibrating/camera.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)     1521 2022-12-22 17:59:18.000000 calibrating-0.6.5/calibrating/feature_libs.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)     4730 2023-02-07 10:00:28.000000 calibrating-0.6.5/calibrating/multi_boards.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)     3200 2022-12-22 13:14:32.000000 calibrating-0.6.5/calibrating/reconstruction.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)    21305 2023-04-13 11:51:43.000000 calibrating-0.6.5/calibrating/stereo.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)    25439 2023-04-16 14:55:01.000000 calibrating-0.6.5/calibrating/utils.py
+drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2023-04-16 15:29:30.000000 calibrating-0.6.5/calibrating.egg-info/
+-rw-rw-r--   0 dl        (1000) dl        (1000)      647 2023-04-16 15:29:30.000000 calibrating-0.6.5/calibrating.egg-info/PKG-INFO
+-rw-rw-r--   0 dl        (1000) dl        (1000)      442 2023-04-16 15:29:30.000000 calibrating-0.6.5/calibrating.egg-info/SOURCES.txt
+-rw-rw-r--   0 dl        (1000) dl        (1000)        1 2023-04-16 15:29:30.000000 calibrating-0.6.5/calibrating.egg-info/dependency_links.txt
+-rw-rw-r--   0 dl        (1000) dl        (1000)       57 2023-04-16 15:29:30.000000 calibrating-0.6.5/calibrating.egg-info/requires.txt
+-rw-rw-r--   0 dl        (1000) dl        (1000)       12 2023-04-16 15:29:30.000000 calibrating-0.6.5/calibrating.egg-info/top_level.txt
+-rw-rw-r--   0 dl        (1000) dl        (1000)       57 2023-04-16 15:27:46.000000 calibrating-0.6.5/requirements.txt
+-rw-rw-r--   0 dl        (1000) dl        (1000)       38 2023-04-16 15:29:30.000000 calibrating-0.6.5/setup.cfg
+-rw-rw-r--   0 dl        (1000) dl        (1000)      853 2021-08-19 08:44:30.000000 calibrating-0.6.5/setup.py
```

### Comparing `calibrating-0.6.4/PKG-INFO` & `calibrating-0.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calibrating
-Version: 0.6.4
+Version: 0.6.5
 Summary: Calibrate camera's intrinsic/extristric, and build stereo depth camera with OpenCV python.
 Home-page: https://github.com/DIYer22/calibrating
 Author: DIYer22
 Author-email: ylxx@live.com
 License: UNKNOWN
 Description: Calibrate camera's intrinsic/extristric, and build stereo depth camera with OpenCV python.
 Platform: UNKNOWN
```

### Comparing `calibrating-0.6.4/README.md` & `calibrating-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `calibrating-0.6.4/calibrating/__info__.py` & `calibrating-0.6.5/calibrating/__info__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.6.4"
+__version__ = "0.6.5"
 __description__ = "Calibrate camera's intrinsic/extristric, and build stereo depth camera with OpenCV python."
 __license__ = "MIT"
 __author__ = "DIYer22"
 __author_email__ = "ylxx@live.com"
 __maintainer__ = "DIYer22"
 __maintainer_email__ = "ylxx@live.com"
 __github_username__ = "DIYer22"
```

### Comparing `calibrating-0.6.4/calibrating/boards.py` & `calibrating-0.6.5/calibrating/boards.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         self.calibration_img_info = info
         self.calibration_img_name = "xx mm, h*w.png"
         return self
 
     def __str__(self):
         if hasattr(self, "init_kwargs"):
             return str(self.init_kwargs)
-        return object.__str__(self)
+        return f"Instance of {type(self).__name__}"
 
     __repr__ = __str__
 
     @staticmethod
     def set_origin_to_center(points):
         if isinstance(points, dict):
             center = np.mean(utils.convert_points_for_cv2(points), 0, keepdims=True)
@@ -289,23 +289,22 @@
         )
         self.square_xy = square_xy
         if aruco_dict_tag is None:
             aruco_dict_tag = cv2.aruco.DICT_4X4_250
 
         self.aruco_dict_tag = aruco_dict_tag
         self.aruco_dictionary = get_aruco_dictionary_with_start(aruco_dict_tag)
-        self.board = cv2.aruco.CharucoBoard_create(
-            square_xy[0],
-            square_xy[1],
+        self.board = cv2.aruco.CharucoBoard(
+            square_xy,
             square_size_mm / 1000.0,
             marker_size_mm / 1000.0,
             self.aruco_dictionary,
         )
         self.object_points = {
-            id: xyz[None] for id, xyz in enumerate(self.board.chessboardCorners)
+            id: xyz[None] for id, xyz in enumerate(self.board.getChessboardCorners())
         }
         if self.init_kwargs.get("using_marker_corner"):
             self.object_points.update(
                 {
                     -1 - marker_id: marker_corners
                     for marker_id, marker_corners in enumerate(self.board.objPoints)
                 }
@@ -386,15 +385,15 @@
             marker_size_mm=size_mm * 0.75,
             aruco_dict_tag=aruco_dict_tag,
             invert_color=invert_color,
         )
 
         self = cls(**init_kwargs)
         self.calibration_img = cv2.cvtColor(
-            self.board.draw(hw[::-1]), cv2.COLOR_GRAY2RGB
+            self.board.generateImage(hw[::-1]), cv2.COLOR_GRAY2RGB
         )
         if invert_color:
             self.calibration_img = 255 - self.calibration_img
         self.calibration_img_info = dict(hw=hw, ppi=ppi, **init_kwargs)
         self.calibration_img_name = (
             f"charuco_square_x{square_xy[0]}y{square_xy[1]}_size{size_mm}mm.png"
         )
```

### Comparing `calibrating-0.6.4/calibrating/camera.py` & `calibrating-0.6.5/calibrating/camera.py`

 * *Files identical despite different names*

### Comparing `calibrating-0.6.4/calibrating/feature_libs.py` & `calibrating-0.6.5/calibrating/feature_libs.py`

 * *Files identical despite different names*

### Comparing `calibrating-0.6.4/calibrating/multi_boards.py` & `calibrating-0.6.5/calibrating/multi_boards.py`

 * *Files identical despite different names*

### Comparing `calibrating-0.6.4/calibrating/reconstruction.py` & `calibrating-0.6.5/calibrating/reconstruction.py`

 * *Files identical despite different names*

### Comparing `calibrating-0.6.4/calibrating/stereo.py` & `calibrating-0.6.5/calibrating/stereo.py`

 * *Files identical despite different names*

### Comparing `calibrating-0.6.4/calibrating/utils.py` & `calibrating-0.6.5/calibrating/utils.py`

 * *Files identical despite different names*

### Comparing `calibrating-0.6.4/calibrating.egg-info/PKG-INFO` & `calibrating-0.6.5/calibrating.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calibrating
-Version: 0.6.4
+Version: 0.6.5
 Summary: Calibrate camera's intrinsic/extristric, and build stereo depth camera with OpenCV python.
 Home-page: https://github.com/DIYer22/calibrating
 Author: DIYer22
 Author-email: ylxx@live.com
 License: UNKNOWN
 Description: Calibrate camera's intrinsic/extristric, and build stereo depth camera with OpenCV python.
 Platform: UNKNOWN
```

### Comparing `calibrating-0.6.4/setup.py` & `calibrating-0.6.5/setup.py`

 * *Files identical despite different names*

