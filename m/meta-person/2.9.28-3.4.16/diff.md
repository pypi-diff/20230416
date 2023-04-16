# Comparing `tmp/meta-person-2.9.28.tar.gz` & `tmp/meta-person-3.4.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/meta-person-2.9.28.tar", last modified: Sat Oct  8 08:52:43 2022, max compression
+gzip compressed data, was "dist/meta-person-3.4.16.tar", last modified: Sun Apr 16 07:34:28 2023, max compression
```

## Comparing `meta-person-2.9.28.tar` & `meta-person-3.4.16.tar`

### file list

```diff
@@ -1,35 +1,30 @@
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2022-10-08 08:52:43.000000 meta-person-2.9.28/
--rw-rw-r--   0 cash      (1000) cash      (1000)      283 2022-10-08 08:52:43.000000 meta-person-2.9.28/PKG-INFO
--rw-rw-r--   0 cash      (1000) cash      (1000)       36 2022-09-20 06:14:09.000000 meta-person-2.9.28/README.md
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2022-10-08 08:52:43.000000 meta-person-2.9.28/meta_person.egg-info/
--rw-rw-r--   0 cash      (1000) cash      (1000)      283 2022-10-08 08:52:43.000000 meta-person-2.9.28/meta_person.egg-info/PKG-INFO
--rw-rw-r--   0 cash      (1000) cash      (1000)      869 2022-10-08 08:52:43.000000 meta-person-2.9.28/meta_person.egg-info/SOURCES.txt
--rw-rw-r--   0 cash      (1000) cash      (1000)        1 2022-10-08 08:52:43.000000 meta-person-2.9.28/meta_person.egg-info/dependency_links.txt
--rw-rw-r--   0 cash      (1000) cash      (1000)       54 2022-10-08 08:52:43.000000 meta-person-2.9.28/meta_person.egg-info/requires.txt
--rw-rw-r--   0 cash      (1000) cash      (1000)       11 2022-10-08 08:52:43.000000 meta-person-2.9.28/meta_person.egg-info/top_level.txt
--rw-rw-r--   0 cash      (1000) cash      (1000)        1 2022-10-08 08:52:43.000000 meta-person-2.9.28/meta_person.egg-info/zip-safe
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2022-10-08 08:52:43.000000 meta-person-2.9.28/metaperson/
--rw-rw-r--   0 cash      (1000) cash      (1000)      130 2022-09-28 06:39:18.000000 meta-person-2.9.28/metaperson/__init__.py
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2022-10-08 08:52:43.000000 meta-person-2.9.28/metaperson/app/
--rw-rw-r--   0 cash      (1000) cash      (1000)      295 2022-09-28 06:39:18.000000 meta-person-2.9.28/metaperson/app/__init__.py
--rw-rw-r--   0 cash      (1000) cash      (1000)      360 2022-09-28 06:53:22.000000 meta-person-2.9.28/metaperson/app/hand_classification_trt.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     1192 2022-09-27 03:07:27.000000 meta-person-2.9.28/metaperson/app/hand_detection_onnx.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     1054 2022-09-28 06:52:46.000000 meta-person-2.9.28/metaperson/app/hand_detection_trt.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     1184 2022-09-20 06:09:06.000000 meta-person-2.9.28/metaperson/app/onnx_to_trt.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     1095 2022-09-28 06:58:57.000000 meta-person-2.9.28/metaperson/app/person_detection_trt.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     3293 2022-09-28 07:22:09.000000 meta-person-2.9.28/metaperson/app/person_tracker_trt.py
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2022-10-08 08:52:43.000000 meta-person-2.9.28/metaperson/model_zoo/
--rw-rw-r--   0 cash      (1000) cash      (1000)      123 2022-09-28 06:34:23.000000 meta-person-2.9.28/metaperson/model_zoo/__init__.py
--rw-rw-r--   0 cash      (1000) cash      (1000)      951 2021-12-04 09:05:10.000000 meta-person-2.9.28/metaperson/model_zoo/basetrack.py
--rw-rw-r--   0 cash      (1000) cash      (1000)    11832 2022-09-28 06:22:50.000000 meta-person-2.9.28/metaperson/model_zoo/byte_tracker.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     9521 2021-12-04 09:05:10.000000 meta-person-2.9.28/metaperson/model_zoo/kalman_filter.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     6222 2021-12-04 09:05:10.000000 meta-person-2.9.28/metaperson/model_zoo/matching.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     3247 2022-09-27 03:07:37.000000 meta-person-2.9.28/metaperson/model_zoo/onnx_predictor.py
--rw-rw-r--   0 cash      (1000) cash      (1000)    13946 2022-09-20 03:38:46.000000 meta-person-2.9.28/metaperson/model_zoo/trt_export.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     2206 2022-09-28 06:51:36.000000 meta-person-2.9.28/metaperson/model_zoo/trt_predictor.py
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2022-10-08 08:52:43.000000 meta-person-2.9.28/metaperson/utils/
--rw-rw-r--   0 cash      (1000) cash      (1000)       47 2022-09-20 03:43:16.000000 meta-person-2.9.28/metaperson/utils/__init__.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     7059 2022-09-08 08:47:40.000000 meta-person-2.9.28/metaperson/utils/image_batch.py
--rw-rw-r--   0 cash      (1000) cash      (1000)    14011 2022-10-05 13:20:02.000000 meta-person-2.9.28/metaperson/utils/utils.py
--rw-rw-r--   0 cash      (1000) cash      (1000)       38 2022-10-08 08:52:43.000000 meta-person-2.9.28/setup.cfg
--rw-rw-r--   0 cash      (1000) cash      (1000)      690 2022-10-08 08:52:20.000000 meta-person-2.9.28/setup.py
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-04-16 07:34:28.000000 meta-person-3.4.16/
+-rw-rw-r--   0 cash      (1000) cash      (1000)      281 2023-04-16 07:34:28.000000 meta-person-3.4.16/PKG-INFO
+-rw-rw-r--   0 cash      (1000) cash      (1000)       35 2021-11-29 11:46:57.000000 meta-person-3.4.16/README.md
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-04-16 07:34:28.000000 meta-person-3.4.16/meta_person.egg-info/
+-rw-rw-r--   0 cash      (1000) cash      (1000)      281 2023-04-16 07:34:28.000000 meta-person-3.4.16/meta_person.egg-info/PKG-INFO
+-rw-rw-r--   0 cash      (1000) cash      (1000)      670 2023-04-16 07:34:28.000000 meta-person-3.4.16/meta_person.egg-info/SOURCES.txt
+-rw-rw-r--   0 cash      (1000) cash      (1000)        1 2023-04-16 07:34:28.000000 meta-person-3.4.16/meta_person.egg-info/dependency_links.txt
+-rw-rw-r--   0 cash      (1000) cash      (1000)       57 2023-04-16 07:34:28.000000 meta-person-3.4.16/meta_person.egg-info/requires.txt
+-rw-rw-r--   0 cash      (1000) cash      (1000)       11 2023-04-16 07:34:28.000000 meta-person-3.4.16/meta_person.egg-info/top_level.txt
+-rw-rw-r--   0 cash      (1000) cash      (1000)        1 2023-04-16 07:34:28.000000 meta-person-3.4.16/meta_person.egg-info/zip-safe
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-04-16 07:34:28.000000 meta-person-3.4.16/metaperson/
+-rw-rw-r--   0 cash      (1000) cash      (1000)       79 2023-04-16 07:19:12.000000 meta-person-3.4.16/metaperson/__init__.py
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-04-16 07:34:28.000000 meta-person-3.4.16/metaperson/app/
+-rw-rw-r--   0 cash      (1000) cash      (1000)      183 2023-04-16 07:19:24.000000 meta-person-3.4.16/metaperson/app/__init__.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     1798 2021-12-10 18:12:55.000000 meta-person-3.4.16/metaperson/app/onnx_to_trt.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     3565 2023-04-11 04:05:00.000000 meta-person-3.4.16/metaperson/app/person_detection_trt.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     3355 2023-04-10 07:31:05.000000 meta-person-3.4.16/metaperson/app/person_recognition_trt.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     4239 2023-04-11 05:47:00.000000 meta-person-3.4.16/metaperson/app/person_reid_trt.py
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-04-16 07:34:28.000000 meta-person-3.4.16/metaperson/model_zoo/
+-rw-rw-r--   0 cash      (1000) cash      (1000)       38 2023-04-16 07:22:22.000000 meta-person-3.4.16/metaperson/model_zoo/__init__.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)      951 2021-12-04 09:05:10.000000 meta-person-3.4.16/metaperson/model_zoo/basetrack.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)    11898 2023-04-10 08:22:12.000000 meta-person-3.4.16/metaperson/model_zoo/byte_tracker.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     9500 2023-04-10 08:08:30.000000 meta-person-3.4.16/metaperson/model_zoo/kalman_filter.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     6134 2023-04-10 08:12:10.000000 meta-person-3.4.16/metaperson/model_zoo/matching.py
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-04-16 07:34:28.000000 meta-person-3.4.16/metaperson/utils/
+-rw-rw-r--   0 cash      (1000) cash      (1000)       40 2023-04-16 07:18:35.000000 meta-person-3.4.16/metaperson/utils/__init__.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     3509 2023-04-16 07:30:41.000000 meta-person-3.4.16/metaperson/utils/boxes.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     1371 2021-12-11 03:52:50.000000 meta-person-3.4.16/metaperson/utils/trt.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)       38 2023-04-16 07:34:28.000000 meta-person-3.4.16/setup.cfg
+-rw-rw-r--   0 cash      (1000) cash      (1000)      699 2023-04-16 07:32:54.000000 meta-person-3.4.16/setup.py
```

### Comparing `meta-person-2.9.28/meta_person.egg-info/SOURCES.txt` & `meta-person-3.4.16/meta_person.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -4,24 +4,19 @@
 meta_person.egg-info/SOURCES.txt
 meta_person.egg-info/dependency_links.txt
 meta_person.egg-info/requires.txt
 meta_person.egg-info/top_level.txt
 meta_person.egg-info/zip-safe
 metaperson/__init__.py
 metaperson/app/__init__.py
-metaperson/app/hand_classification_trt.py
-metaperson/app/hand_detection_onnx.py
-metaperson/app/hand_detection_trt.py
 metaperson/app/onnx_to_trt.py
 metaperson/app/person_detection_trt.py
-metaperson/app/person_tracker_trt.py
+metaperson/app/person_recognition_trt.py
+metaperson/app/person_reid_trt.py
 metaperson/model_zoo/__init__.py
 metaperson/model_zoo/basetrack.py
 metaperson/model_zoo/byte_tracker.py
 metaperson/model_zoo/kalman_filter.py
 metaperson/model_zoo/matching.py
-metaperson/model_zoo/onnx_predictor.py
-metaperson/model_zoo/trt_export.py
-metaperson/model_zoo/trt_predictor.py
 metaperson/utils/__init__.py
-metaperson/utils/image_batch.py
-metaperson/utils/utils.py
+metaperson/utils/boxes.py
+metaperson/utils/trt.py
```

### Comparing `meta-person-2.9.28/metaperson/app/person_tracker_trt.py` & `meta-person-3.4.16/metaperson/app/person_recognition_trt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import cv2, time
 from .person_detection_trt import PersonDetectionTrt
 from ..model_zoo import BYTETracker
 
 
 class PersonTrackerTrt:
     def __init__(self,
-                 model_file='models/yolov7.trt',
-                 score_thr=0.25,
-                 nms_thr=0.45,
+                 model_file='models/bytetrack_s_fp16.trt',
+                 score_thr=0.2,
+                 nms_thr=0.7,
                  track_thresh=0.5,
                  match_thresh=0.8,
                  track_buffer=30,
                  frame_rate=30,
                  person_detector=None):
         if person_detector is None:
-            self.detector = PersonDetectionTrt(trt_file=model_file, conf=score_thr, iou=nms_thr)
+            self.detector = PersonDetectionTrt(model_file, score_thr, nms_thr)
         else:
             self.detector = person_detector
         self.tracker = BYTETracker(track_thresh, match_thresh, track_buffer, frame_rate)
 
     def predict(self, image, min_box_area=10, aspect_ratio_thresh=1.6):
         img_info = image.shape[:2]
         results = []
@@ -40,26 +40,26 @@
             l, t, r, b = max(box[0], 0), max(box[1], 0), min(box[0] + box[2] - 1, w - 1), min(box[1] + box[3] - 1,
                                                                                               h - 1)
             cv2.rectangle(image, (l, t), (r, b), (255, 0, 255), 2)
             cv2.putText(image, 'id: %d, score: %.2f' % (result['id'], result['score']),
                         (l, max(t - 4, 0)), cv2.FONT_HERSHEY_PLAIN, 2, (0, 0, 255), thickness=2)
         return image
 
-    def predict_video(self, file_path=0, min_box_area=10):
+    def predict_video(self, file_path=0, min_box_area=10, aspect_ratio_thresh=1.6):
         cap = cv2.VideoCapture(file_path)
         frame_id = 0
         while True:
             ret, frame = cap.read()
             if ret:
                 s = time.time()
-                results = self.predict(frame, min_box_area)
+                results = self.predict(frame, min_box_area, aspect_ratio_thresh)
                 print("person nums: ", len(results), time.time() - s)
                 if len(results) > 0:
                     frame = self.show(frame, results)
-                    cv2.imwrite('images/results/' + str(frame_id) + '.jpg', frame)
+                    cv2.imwrite('/home/cash/WorkSpace/online_data/results/' + str(frame_id) + '.jpg', frame)
             else:
                 break
             frame_id += 1
 
 
 if __name__ == '__main__':
     import glob, time, os
```

### Comparing `meta-person-2.9.28/metaperson/model_zoo/basetrack.py` & `meta-person-3.4.16/metaperson/model_zoo/basetrack.py`

 * *Files identical despite different names*

### Comparing `meta-person-2.9.28/metaperson/model_zoo/byte_tracker.py` & `meta-person-3.4.16/metaperson/model_zoo/byte_tracker.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,17 +139,17 @@
 
 class BYTETracker(object):
     def __init__(self,
                  track_thresh=0.5,
                  match_thresh=0.8,
                  track_buffer=30,
                  frame_rate=30):
-        self.tracked_stracks = []
-        self.lost_stracks = []
-        self.removed_stracks = []
+        self.tracked_stracks = []  # type: list[STrack]
+        self.lost_stracks = []  # type: list[STrack]
+        self.removed_stracks = []  # type: list[STrack]
 
         self.frame_id = 0
         self.mot20 = False
         self.track_thresh = track_thresh
         self.det_thresh = track_thresh + 0.1
         self.match_thresh = match_thresh
         self.buffer_size = int(frame_rate / 30.0 * track_buffer)
```

### Comparing `meta-person-2.9.28/metaperson/model_zoo/kalman_filter.py` & `meta-person-3.4.16/metaperson/model_zoo/kalman_filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# vim: expandtab:ts=4:sw=4
 import numpy as np
 import scipy.linalg
 
 """
 Table for the 0.95 quantile of the chi-square distribution with N degrees of
 freedom (contains values for N=1, ..., 9). Taken from MATLAB/Octave's chi2inv
 function and used as Mahalanobis gating threshold.
@@ -110,15 +111,14 @@
         std_vel = [
             self._std_weight_velocity * mean[3],
             self._std_weight_velocity * mean[3],
             1e-5,
             self._std_weight_velocity * mean[3]]
         motion_cov = np.diag(np.square(np.r_[std_pos, std_vel]))
 
-        # mean = np.dot(self._motion_mat, mean)
         mean = np.dot(mean, self._motion_mat.T)
         covariance = np.linalg.multi_dot((
             self._motion_mat, covariance, self._motion_mat.T)) + motion_cov
 
         return mean, covariance
 
     def project(self, mean, covariance):
```

### Comparing `meta-person-2.9.28/metaperson/model_zoo/matching.py` & `meta-person-3.4.16/metaperson/model_zoo/matching.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import cv2
 import numpy as np
 import scipy
 import lap
 from scipy.spatial.distance import cdist
 
 from cython_bbox import bbox_overlaps as bbox_ious
 from .kalman_filter import chi2inv95
@@ -133,28 +132,28 @@
     return cost_matrix
 
 
 def gate_cost_matrix(kf, cost_matrix, tracks, detections, only_position=False):
     if cost_matrix.size == 0:
         return cost_matrix
     gating_dim = 2 if only_position else 4
-    gating_threshold = kalman_filter.chi2inv95[gating_dim]
+    gating_threshold = chi2inv95[gating_dim]
     measurements = np.asarray([det.to_xyah() for det in detections])
     for row, track in enumerate(tracks):
         gating_distance = kf.gating_distance(
             track.mean, track.covariance, measurements, only_position)
         cost_matrix[row, gating_distance > gating_threshold] = np.inf
     return cost_matrix
 
 
 def fuse_motion(kf, cost_matrix, tracks, detections, only_position=False, lambda_=0.98):
     if cost_matrix.size == 0:
         return cost_matrix
     gating_dim = 2 if only_position else 4
-    gating_threshold = kalman_filter.chi2inv95[gating_dim]
+    gating_threshold = chi2inv95[gating_dim]
     measurements = np.asarray([det.to_xyah() for det in detections])
     for row, track in enumerate(tracks):
         gating_distance = kf.gating_distance(
             track.mean, track.covariance, measurements, only_position, metric='maha')
         cost_matrix[row, gating_distance > gating_threshold] = np.inf
         cost_matrix[row] = lambda_ * cost_matrix[row] + (1 - lambda_) * gating_distance
     return cost_matrix
@@ -165,15 +164,14 @@
         return cost_matrix
     reid_sim = 1 - cost_matrix
     iou_dist = iou_distance(tracks, detections)
     iou_sim = 1 - iou_dist
     fuse_sim = reid_sim * (1 + iou_sim) / 2
     det_scores = np.array([det.score for det in detections])
     det_scores = np.expand_dims(det_scores, axis=0).repeat(cost_matrix.shape[0], axis=0)
-    # fuse_sim = fuse_sim * (1 + det_scores) / 2
     fuse_cost = 1 - fuse_sim
     return fuse_cost
 
 
 def fuse_score(cost_matrix, detections):
     if cost_matrix.size == 0:
         return cost_matrix
```

### Comparing `meta-person-2.9.28/metaperson/model_zoo/onnx_predictor.py` & `meta-person-3.4.16/metaperson/app/person_detection_trt.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,81 +1,89 @@
+import os
 import cv2
 import numpy as np
-import onnxruntime
-from ..utils import multiclass_nms
+import tensorrt as trt
+import pycuda.driver as cuda
+from ..utils import allocate_buffers, do_inference, preproc, demo_postprocess, multiclass_nms
 
 
-def letterbox(im, new_shape=(640, 640), color=(114, 114, 114), auto=True, scaleup=True, stride=32):
-    # Resize and pad image while meeting stride-multiple constraints
-    shape = im.shape[:2]  # current shape [height, width]
-    if isinstance(new_shape, int):
-        new_shape = (new_shape, new_shape)
-
-    # Scale ratio (new / old)
-    r = min(new_shape[0] / shape[0], new_shape[1] / shape[1])
-    if not scaleup:  # only scale down, do not scale up (for better val mAP)
-        r = min(r, 1.0)
-
-    # Compute padding
-    new_unpad = int(round(shape[1] * r)), int(round(shape[0] * r))
-    dw, dh = new_shape[1] - new_unpad[0], new_shape[0] - new_unpad[1]  # wh padding
-
-    if auto:  # minimum rectangle
-        dw, dh = np.mod(dw, stride), np.mod(dh, stride)  # wh padding
-
-    dw /= 2  # divide padding into 2 sides
-    dh /= 2
-
-    if shape[::-1] != new_unpad:  # resize
-        im = cv2.resize(im, new_unpad, interpolation=cv2.INTER_LINEAR)
-    top, bottom = int(round(dh - 0.1)), int(round(dh + 0.1))
-    left, right = int(round(dw - 0.1)), int(round(dw + 0.1))
-    im = cv2.copyMakeBorder(im, top, bottom, left, right, cv2.BORDER_CONSTANT, value=color)  # add border
-    return im, r, (dw, dh)
-
-
-class OnnxPredictor:
+class PersonDetectionTrt:
     def __init__(self,
-                 onnx_file='models/hand.onnx',
-                 input_shape=(640, 640),
-                 conf=0.1,
-                 iou=0.45,
-                 end2end=False,
-                 use_gpu=False):
-        self.input_shape = input_shape
-        self.conf = conf
-        self.iou = iou
-        self.end2end = end2end
-        self.n_classes = 1
-        self.class_names = ['hand']
-        providers = ['CUDAExecutionProvider', 'CPUExecutionProvider'] if use_gpu else ['CPUExecutionProvider']
-        self.session = onnxruntime.InferenceSession(onnx_file, providers=providers)
-        self.input_names = [i.name for i in self.session.get_inputs()]
-        self.output_names = [i.name for i in self.session.get_outputs()]
-
-    def detect(self, image):
-        img = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
-        img, ratio, dwdh = letterbox(img, auto=False)
-        img = img.transpose((2, 0, 1))
-        img = np.expand_dims(img, 0)
-        img = np.ascontiguousarray(img)
-        img = img.astype(np.float32) / 255
-
-        data = self.session.run(self.output_names, {self.input_names[0]: img})[0]
-
-        predictions = np.reshape(data, (1, -1, int(5 + self.n_classes)))[0]
-        dets = self.postprocess(predictions, ratio, dwdh, self.conf, self.iou)
-        return dets
-
-    @staticmethod
-    def postprocess(predictions, ratio, dwdh, score_thr, nms_thr):
+                 engine_file,
+                 score_thr=0.1,
+                 nms_thr=0.7,
+                 with_p6=False):
+        self.engine_file = engine_file
+        self.score_thr = score_thr
+        self.nms_thr = nms_thr
+        self.with_p6 = with_p6
+        self.rgb_means = (0.485, 0.456, 0.406)
+        self.std = (0.229, 0.224, 0.225)
+        cuda.init()
+        self._device_ctx = cuda.Device(0).make_context()
+        engine = self.get_model(engine_file)
+        self.input_shape = list(engine.get_binding_shape(engine[0]))
+        self.output_shape = list(engine.get_binding_shape(engine[-1]))
+        self.context = engine.create_execution_context()
+        self.inputs, self.outputs, self.bindings, self.stream = allocate_buffers(engine)
+
+    def get_model(self, engine_file):
+        if not os.path.exists(engine_file):
+            FileNotFoundError('Trt file not exist')
+
+        runtime = trt.Runtime(trt.Logger(trt.Logger.VERBOSE))
+        with open(engine_file, "rb") as f:
+            return runtime.deserialize_cuda_engine(f.read())
+
+    def predict(self, image):
+        image, ratio = preproc(image, self.input_shape[2:], self.rgb_means, self.std)
+        image = np.expand_dims(image, axis=0)
+        image_batch_ravel = image.ravel()
+        np.copyto(dst=self.inputs[0].host, src=image_batch_ravel)
+        self._device_ctx.push()
+        outputs = do_inference(context=self.context,
+                               bindings=self.bindings,
+                               inputs=self.inputs,
+                               outputs=self.outputs,
+                               stream=self.stream,
+                               batch_size=self.input_shape[0])
+        self._device_ctx.pop()
+        outputs = [output.reshape(self.output_shape) for output in outputs]
+        predictions = demo_postprocess(outputs[0], self.input_shape[2:], p6=self.with_p6)[0]
         boxes = predictions[:, :4]
         scores = predictions[:, 4:5] * predictions[:, 5:]
         boxes_xyxy = np.ones_like(boxes)
         boxes_xyxy[:, 0] = boxes[:, 0] - boxes[:, 2] / 2.
         boxes_xyxy[:, 1] = boxes[:, 1] - boxes[:, 3] / 2.
         boxes_xyxy[:, 2] = boxes[:, 0] + boxes[:, 2] / 2.
         boxes_xyxy[:, 3] = boxes[:, 1] + boxes[:, 3] / 2.
-        boxes_xyxy -= np.array(dwdh * 2)
         boxes_xyxy /= ratio
-        dets = multiclass_nms(boxes_xyxy, scores, nms_thr=nms_thr, score_thr=score_thr)
-        return dets
+        dets = multiclass_nms(boxes_xyxy, scores, nms_thr=self.nms_thr, score_thr=self.score_thr)
+        return dets[:, :-1] if dets is not None else None
+
+    def __del__(self):
+        del self.inputs
+        del self.outputs
+        del self.stream
+        self._device_ctx.pop()
+        self._device_ctx.detach()  # release device context
+
+    def show(self, image, results):
+        index = 1
+        for (box, score) in zip(list(results[:, :-1].astype(int)), list(results[:, -1])):
+            cv2.rectangle(image, (box[0], box[1]), (box[2], box[3]), (255, 0, 255), 2)
+            cv2.putText(image, 'id: %d, score: %.2f' % (index, score),
+                        (box[0], box[1] - 4), cv2.FONT_HERSHEY_PLAIN, 2, (0, 0, 255), thickness=2)
+            index += 1
+        return image
+
+
+if __name__ == '__main__':
+    import time
+
+    tp = PersonDetectionTrt(engine_file='bytetrack_s_fp16.trt')
+
+    img = cv2.imread("face.jpg")
+    s = time.time()
+    trt_out = tp.predict(img)
+    print("time: ", time.time() - s)
+    print(list(trt_out))
```

### Comparing `meta-person-2.9.28/setup.py` & `meta-person-3.4.16/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from setuptools import setup, find_packages
 
 requirements = [
     'opencv-python',
     'setuptools',
     'tensorrt',
-    'pycuda',
     'numpy',
-    'pillow',
+    'pycuda',
+    'scipy',
+    'lap',
 ]
 
-__version__ = 'V2.09.28'
+__version__ = 'V3.04.16'
 
 setup(
     name='meta-person',
     version=__version__,
     author='CachCheng',
     author_email='tkggpdc2007@163.com',
-    url='https://github.com/CachCheng/cvperson',
+    url='https://github.com/CachCheng/cvtrack',
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     description='Meta Person Toolkit',
     license='Apache-2.0',
     packages=find_packages(exclude=('docs', 'tests', 'scripts')),
     zip_safe=True,
     include_package_data=True,
```

