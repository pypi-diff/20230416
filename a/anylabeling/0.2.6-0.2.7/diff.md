# Comparing `tmp/anylabeling-0.2.6.tar.gz` & `tmp/anylabeling-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anylabeling-0.2.6.tar", last modified: Sun Apr 16 09:02:24 2023, max compression
+gzip compressed data, was "anylabeling-0.2.7.tar", last modified: Sun Apr 16 18:19:32 2023, max compression
```

## Comparing `anylabeling-0.2.6.tar` & `anylabeling-0.2.7.tar`

### file list

```diff
@@ -1,145 +1,145 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:02:24.222624 anylabeling-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-16 09:02:15.000000 anylabeling-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-16 09:02:15.000000 anylabeling-0.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-04-16 09:02:24.222624 anylabeling-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-16 09:02:15.000000 anylabeling-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:02:24.206624 anylabeling-0.2.6/anylabeling/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/app_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:02:24.206624 anylabeling-0.2.6/anylabeling/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/configs/anylabeling_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:02:24.210624 anylabeling-0.2.6/anylabeling/configs/auto_labeling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/configs/auto_labeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/configs/auto_labeling/models.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/configs/auto_labeling/segment_anything_vit_b.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/configs/auto_labeling/segment_anything_vit_b_quant.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/configs/auto_labeling/segment_anything_vit_h_quant.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/configs/auto_labeling/segment_anything_vit_l.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/configs/auto_labeling/segment_anything_vit_l_quant.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/configs/auto_labeling/yolov5l.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/configs/auto_labeling/yolov5m.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/configs/auto_labeling/yolov5n.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/configs/auto_labeling/yolov5s.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/configs/auto_labeling/yolov5x.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/configs/auto_labeling/yolov8l.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/configs/auto_labeling/yolov8m.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/configs/auto_labeling/yolov8n.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/configs/auto_labeling/yolov8s.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/configs/auto_labeling/yolov8x.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:02:24.210624 anylabeling-0.2.6/anylabeling/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   477720 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/resources/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:02:24.210624 anylabeling-0.2.6/anylabeling/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:02:24.210624 anylabeling-0.2.6/anylabeling/services/auto_labeling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/services/auto_labeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/services/auto_labeling/lru_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/services/auto_labeling/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8822 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/services/auto_labeling/model_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/services/auto_labeling/segment_anything.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/services/auto_labeling/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/services/auto_labeling/yolov5.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/services/auto_labeling/yolov8.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:02:24.210624 anylabeling-0.2.6/anylabeling/views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:02:24.210624 anylabeling-0.2.6/anylabeling/views/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9583 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/common/toaster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:02:24.214624 anylabeling-0.2.6/anylabeling/views/labeling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:02:24.218624 anylabeling-0.2.6/anylabeling/views/labeling/icons/
--rw-r--r--   0 runner    (1001) docker     (123)    28068 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/brain.png
--rw-r--r--   0 runner    (1001) docker     (123)     6844 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/cancel.png
--rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/cartesian.png
--rw-r--r--   0 runner    (1001) docker     (123)    15818 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/circle.png
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/color-line.png
--rw-r--r--   0 runner    (1001) docker     (123)    23824 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/color.png
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/color_line.png
--rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/copy.png
--rw-r--r--   0 runner    (1001) docker     (123)     7842 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/delete.png
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/done.png
--rw-r--r--   0 runner    (1001) docker     (123)    22232 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/done.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15023 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/edit.png
--rw-r--r--   0 runner    (1001) docker     (123)     7718 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/expert.png
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/expert1.png
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/expert2.png
--rw-r--r--   0 runner    (1001) docker     (123)    37652 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/eye.png
--rw-r--r--   0 runner    (1001) docker     (123)     8059 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/feBlend-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/file.png
--rw-r--r--   0 runner    (1001) docker     (123)    17368 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/fit-width.png
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/fit-window.png
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/fit.png
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/format_createml.png
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/format_voc.png
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/format_yolo.png
--rw-r--r--   0 runner    (1001) docker     (123)    14479 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/help.png
--rw-r--r--   0 runner    (1001) docker     (123)    44771 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/labels.png
--rw-r--r--   0 runner    (1001) docker     (123)    36597 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/labels.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/line-strip.png
--rw-r--r--   0 runner    (1001) docker     (123)     9457 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/line.png
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/new.png
--rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/next.png
--rw-r--r--   0 runner    (1001) docker     (123)    26255 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/objects.png
--rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/open.png
--rw-r--r--   0 runner    (1001) docker     (123)    10572 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/paste.png
--rw-r--r--   0 runner    (1001) docker     (123)    13847 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/point.png
--rw-r--r--   0 runner    (1001) docker     (123)    14286 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/polygon.png
--rw-r--r--   0 runner    (1001) docker     (123)     7275 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/prev.png
--rw-r--r--   0 runner    (1001) docker     (123)    22460 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/quit.png
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/rectangle.png
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/resetall.png
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/save-as.png
--rw-r--r--   0 runner    (1001) docker     (123)     6118 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/save.png
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/undo-cross.png
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/undo.png
--rw-r--r--   0 runner    (1001) docker     (123)    18083 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/upload_brain.png
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/verify.png
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/zoom-in.png
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/zoom-out.png
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/zoom.png
--rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/label_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    92452 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/label_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/label_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    10828 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/shape.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:02:24.218624 anylabeling-0.2.6/anylabeling/views/labeling/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/utils/_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/utils/opencv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/utils/qt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/utils/shape.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:02:24.222624 anylabeling-0.2.6/anylabeling/views/labeling/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/widgets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:02:24.222624 anylabeling-0.2.6/anylabeling/views/labeling/widgets/auto_labeling/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/widgets/auto_labeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)    48612 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/widgets/canvas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/widgets/color_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/widgets/escapable_qlist_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/widgets/file_dialog_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/widgets/label_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/widgets/label_list_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/widgets/toolbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/widgets/zoom_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/mainwindow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:02:24.206624 anylabeling-0.2.6/anylabeling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-04-16 09:02:24.000000 anylabeling-0.2.6/anylabeling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-04-16 09:02:24.000000 anylabeling-0.2.6/anylabeling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 09:02:24.000000 anylabeling-0.2.6/anylabeling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-16 09:02:24.000000 anylabeling-0.2.6/anylabeling.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-16 09:02:24.000000 anylabeling-0.2.6/anylabeling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-16 09:02:24.000000 anylabeling-0.2.6/anylabeling.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-16 09:02:15.000000 anylabeling-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 09:02:24.222624 anylabeling-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-16 09:02:15.000000 anylabeling-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:19:32.862918 anylabeling-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-16 18:19:21.000000 anylabeling-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-16 18:19:21.000000 anylabeling-0.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-04-16 18:19:32.862918 anylabeling-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-16 18:19:21.000000 anylabeling-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:19:32.842918 anylabeling-0.2.7/anylabeling/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/app_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:19:32.846918 anylabeling-0.2.7/anylabeling/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/configs/anylabeling_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:19:32.850918 anylabeling-0.2.7/anylabeling/configs/auto_labeling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/configs/auto_labeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/configs/auto_labeling/models.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/configs/auto_labeling/segment_anything_vit_b.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/configs/auto_labeling/segment_anything_vit_b_quant.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/configs/auto_labeling/segment_anything_vit_h_quant.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/configs/auto_labeling/segment_anything_vit_l.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/configs/auto_labeling/segment_anything_vit_l_quant.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/configs/auto_labeling/yolov5l.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/configs/auto_labeling/yolov5m.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/configs/auto_labeling/yolov5n.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/configs/auto_labeling/yolov5s.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/configs/auto_labeling/yolov5x.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/configs/auto_labeling/yolov8l.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/configs/auto_labeling/yolov8m.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/configs/auto_labeling/yolov8n.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/configs/auto_labeling/yolov8s.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/configs/auto_labeling/yolov8x.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:19:32.850918 anylabeling-0.2.7/anylabeling/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   477720 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/resources/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:19:32.850918 anylabeling-0.2.7/anylabeling/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:19:32.850918 anylabeling-0.2.7/anylabeling/services/auto_labeling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/services/auto_labeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/services/auto_labeling/lru_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/services/auto_labeling/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/services/auto_labeling/model_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14919 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/services/auto_labeling/segment_anything.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/services/auto_labeling/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/services/auto_labeling/yolov5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/services/auto_labeling/yolov8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:19:32.850918 anylabeling-0.2.7/anylabeling/views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:19:32.854918 anylabeling-0.2.7/anylabeling/views/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9583 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/common/toaster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:19:32.854918 anylabeling-0.2.7/anylabeling/views/labeling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:19:32.862918 anylabeling-0.2.7/anylabeling/views/labeling/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)    28068 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/brain.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6844 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/cancel.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/cartesian.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15818 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/circle.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/color-line.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23824 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/color.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/color_line.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/copy.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7842 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/delete.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/done.png
+-rw-r--r--   0 runner    (1001) docker     (123)    22232 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/done.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15023 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/edit.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7718 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/expert.png
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/expert1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/expert2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    37652 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/eye.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8059 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/feBlend-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/file.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17368 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/fit-width.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/fit-window.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/fit.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/format_createml.png
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/format_voc.png
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/format_yolo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14479 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/help.png
+-rw-r--r--   0 runner    (1001) docker     (123)    44771 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/labels.png
+-rw-r--r--   0 runner    (1001) docker     (123)    36597 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/labels.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/line-strip.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9457 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/line.png
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/new.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/next.png
+-rw-r--r--   0 runner    (1001) docker     (123)    26255 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/objects.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/open.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10572 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/paste.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13847 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/point.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14286 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/polygon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7275 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/prev.png
+-rw-r--r--   0 runner    (1001) docker     (123)    22460 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/quit.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/rectangle.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/resetall.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/save-as.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6118 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/save.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/undo-cross.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/undo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18083 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/upload_brain.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/verify.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/zoom-in.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/zoom-out.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/icons/zoom.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/label_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93425 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/label_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/label_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10828 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:19:32.862918 anylabeling-0.2.7/anylabeling/views/labeling/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/utils/_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/utils/opencv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/utils/qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/utils/shape.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:19:32.862918 anylabeling-0.2.7/anylabeling/views/labeling/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/widgets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:19:32.862918 anylabeling-0.2.7/anylabeling/views/labeling/widgets/auto_labeling/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/widgets/auto_labeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48701 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/widgets/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/widgets/color_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/widgets/escapable_qlist_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/widgets/file_dialog_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/widgets/label_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/widgets/label_list_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/widgets/toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/labeling/widgets/zoom_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-16 18:19:21.000000 anylabeling-0.2.7/anylabeling/views/mainwindow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:19:32.846918 anylabeling-0.2.7/anylabeling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-04-16 18:19:32.000000 anylabeling-0.2.7/anylabeling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-04-16 18:19:32.000000 anylabeling-0.2.7/anylabeling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 18:19:32.000000 anylabeling-0.2.7/anylabeling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-16 18:19:32.000000 anylabeling-0.2.7/anylabeling.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-16 18:19:32.000000 anylabeling-0.2.7/anylabeling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-16 18:19:32.000000 anylabeling-0.2.7/anylabeling.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-16 18:19:21.000000 anylabeling-0.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 18:19:32.862918 anylabeling-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-16 18:19:21.000000 anylabeling-0.2.7/setup.py
```

### Comparing `anylabeling-0.2.6/LICENSE` & `anylabeling-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/PKG-INFO` & `anylabeling-0.2.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anylabeling
-Version: 0.2.6
+Version: 0.2.7
 Summary: Effortless data labeling with AI support
 Home-page: https://github.com/vietanhdev/anylabeling
 Author: Viet-Anh Nguyen
 Author-email: vietanh.dev@gmail.com
 License: GPLv3
 Keywords: Image Annotation,Machine Learning,Deep Learning
 Classifier: Intended Audience :: Developers
@@ -29,19 +29,19 @@
 ![](https://i.imgur.com/waxVImv.png)
 
 [![PyPI](https://img.shields.io/pypi/v/anylabeling)](https://pypi.org/project/anylabeling)
 [![license](https://img.shields.io/github/license/vietanhdev/anylabeling.svg)](https://github.com/vietanhdev/anylabeling/blob/master/LICENSE)
 [![open issues](https://isitmaintained.com/badge/open/vietanhdev/anylabeling.svg)](https://github.com/vietanhdev/anylabeling/issues)
 [![Pypi Downloads](https://pepy.tech/badge/anylabeling)](https://pypi.org/project/anylabeling/)
 
-<a href="https://www.youtube.com/watch?v=5iQSGL7ebXE">
+<a href="https://www.youtube.com/watch?v=xLVz-f6OeUY">
   <img alt="AnyLabeling" src="https://user-images.githubusercontent.com/18329471/232266520-1f52cd45-0776-479e-8a3c-4fef144c6b73.png"/>
 </a>
 
-- **Youtube Demo:** [https://www.youtube.com/watch?v=5iQSGL7ebXE](https://www.youtube.com/watch?v=5iQSGL7ebXE)
+- **Youtube Demo:** [https://www.youtube.com/watch?v=xLVz-f6OeUY](https://www.youtube.com/watch?v=xLVz-f6OeUY)
 - **Documentation:** [https://anylabeling.com](https://anylabeling.com)
 
 ## I. Install and run
 
 - Requirements: Python >= 3.8
 - Recommended: Miniconda/Anaconda <https://docs.conda.io/en/latest/miniconda.html>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: anylabeling Version: 0.2.6 Summary: Effortless data
+Metadata-Version: 2.1 Name: anylabeling Version: 0.2.7 Summary: Effortless data
 labeling with AI support Home-page: https://github.com/vietanhdev/anylabeling
 Author: Viet-Anh Nguyen Author-email: vietanh.dev@gmail.com License: GPLv3
 Keywords: Image Annotation,Machine Learning,Deep Learning Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
@@ -16,16 +16,16 @@
 ![](https://i.imgur.com/waxVImv.png) [![PyPI](https://img.shields.io/pypi/v/
 anylabeling)](https://pypi.org/project/anylabeling) [![license](https://
 img.shields.io/github/license/vietanhdev/anylabeling.svg)](https://github.com/
 vietanhdev/anylabeling/blob/master/LICENSE) [![open issues](https://
 isitmaintained.com/badge/open/vietanhdev/anylabeling.svg)](https://github.com/
 vietanhdev/anylabeling/issues) [![Pypi Downloads](https://pepy.tech/badge/
 anylabeling)](https://pypi.org/project/anylabeling/) [AnyLabeling] - **Youtube
-Demo:** [https://www.youtube.com/watch?v=5iQSGL7ebXE](https://www.youtube.com/
-watch?v=5iQSGL7ebXE) - **Documentation:** [https://anylabeling.com](https://
+Demo:** [https://www.youtube.com/watch?v=xLVz-f6OeUY](https://www.youtube.com/
+watch?v=xLVz-f6OeUY) - **Documentation:** [https://anylabeling.com](https://
 anylabeling.com) ## I. Install and run - Requirements: Python >= 3.8 -
 Recommended: Miniconda/Anaconda
 docs.conda.io/en/latest/miniconda.html> - Create environment: ```bash conda
 create -n anylabeling python=3.8 conda activate anylabeling ``` - **(For macOS
 only)** Install PyQt5 using Conda: ```bash conda install -c conda-forge
 pyqt==5.15.7 ``` - Install anylabeling: ```bash pip install anylabeling ``` -
 Run app: ```bash anylabeling ``` Or ```bash python -m anylabeling.app ``` ##
```

### Comparing `anylabeling-0.2.6/README.md` & `anylabeling-0.2.7/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 ![](https://i.imgur.com/waxVImv.png)
 
 [![PyPI](https://img.shields.io/pypi/v/anylabeling)](https://pypi.org/project/anylabeling)
 [![license](https://img.shields.io/github/license/vietanhdev/anylabeling.svg)](https://github.com/vietanhdev/anylabeling/blob/master/LICENSE)
 [![open issues](https://isitmaintained.com/badge/open/vietanhdev/anylabeling.svg)](https://github.com/vietanhdev/anylabeling/issues)
 [![Pypi Downloads](https://pepy.tech/badge/anylabeling)](https://pypi.org/project/anylabeling/)
 
-<a href="https://www.youtube.com/watch?v=5iQSGL7ebXE">
+<a href="https://www.youtube.com/watch?v=xLVz-f6OeUY">
   <img alt="AnyLabeling" src="https://user-images.githubusercontent.com/18329471/232266520-1f52cd45-0776-479e-8a3c-4fef144c6b73.png"/>
 </a>
 
-- **Youtube Demo:** [https://www.youtube.com/watch?v=5iQSGL7ebXE](https://www.youtube.com/watch?v=5iQSGL7ebXE)
+- **Youtube Demo:** [https://www.youtube.com/watch?v=xLVz-f6OeUY](https://www.youtube.com/watch?v=xLVz-f6OeUY)
 - **Documentation:** [https://anylabeling.com](https://anylabeling.com)
 
 ## I. Install and run
 
 - Requirements: Python >= 3.8
 - Recommended: Miniconda/Anaconda <https://docs.conda.io/en/latest/miniconda.html>
```

#### html2text {}

```diff
@@ -5,16 +5,16 @@
 ![](https://i.imgur.com/waxVImv.png) [![PyPI](https://img.shields.io/pypi/v/
 anylabeling)](https://pypi.org/project/anylabeling) [![license](https://
 img.shields.io/github/license/vietanhdev/anylabeling.svg)](https://github.com/
 vietanhdev/anylabeling/blob/master/LICENSE) [![open issues](https://
 isitmaintained.com/badge/open/vietanhdev/anylabeling.svg)](https://github.com/
 vietanhdev/anylabeling/issues) [![Pypi Downloads](https://pepy.tech/badge/
 anylabeling)](https://pypi.org/project/anylabeling/) [AnyLabeling] - **Youtube
-Demo:** [https://www.youtube.com/watch?v=5iQSGL7ebXE](https://www.youtube.com/
-watch?v=5iQSGL7ebXE) - **Documentation:** [https://anylabeling.com](https://
+Demo:** [https://www.youtube.com/watch?v=xLVz-f6OeUY](https://www.youtube.com/
+watch?v=xLVz-f6OeUY) - **Documentation:** [https://anylabeling.com](https://
 anylabeling.com) ## I. Install and run - Requirements: Python >= 3.8 -
 Recommended: Miniconda/Anaconda
 docs.conda.io/en/latest/miniconda.html> - Create environment: ```bash conda
 create -n anylabeling python=3.8 conda activate anylabeling ``` - **(For macOS
 only)** Install PyQt5 using Conda: ```bash conda install -c conda-forge
 pyqt==5.15.7 ``` - Install anylabeling: ```bash pip install anylabeling ``` -
 Run app: ```bash anylabeling ``` Or ```bash python -m anylabeling.app ``` ##
```

### Comparing `anylabeling-0.2.6/anylabeling/app.py` & `anylabeling-0.2.7/anylabeling/app.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/configs/anylabeling_config.yaml` & `anylabeling-0.2.7/anylabeling/configs/anylabeling_config.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/configs/auto_labeling/models.yaml` & `anylabeling-0.2.7/anylabeling/configs/auto_labeling/models.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/configs/auto_labeling/yolov5l.yaml` & `anylabeling-0.2.7/anylabeling/configs/auto_labeling/yolov5l.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/configs/auto_labeling/yolov5m.yaml` & `anylabeling-0.2.7/anylabeling/configs/auto_labeling/yolov5m.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/configs/auto_labeling/yolov5n.yaml` & `anylabeling-0.2.7/anylabeling/configs/auto_labeling/yolov5n.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/configs/auto_labeling/yolov5s.yaml` & `anylabeling-0.2.7/anylabeling/configs/auto_labeling/yolov5s.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/configs/auto_labeling/yolov5x.yaml` & `anylabeling-0.2.7/anylabeling/configs/auto_labeling/yolov5x.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/configs/auto_labeling/yolov8l.yaml` & `anylabeling-0.2.7/anylabeling/configs/auto_labeling/yolov8l.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/configs/auto_labeling/yolov8m.yaml` & `anylabeling-0.2.7/anylabeling/configs/auto_labeling/yolov8m.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/configs/auto_labeling/yolov8n.yaml` & `anylabeling-0.2.7/anylabeling/configs/auto_labeling/yolov8n.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/configs/auto_labeling/yolov8s.yaml` & `anylabeling-0.2.7/anylabeling/configs/auto_labeling/yolov8s.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/configs/auto_labeling/yolov8x.yaml` & `anylabeling-0.2.7/anylabeling/configs/auto_labeling/yolov8x.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/resources/resources.py` & `anylabeling-0.2.7/anylabeling/resources/resources.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/services/auto_labeling/lru_cache.py` & `anylabeling-0.2.7/anylabeling/services/auto_labeling/lru_cache.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/services/auto_labeling/model.py` & `anylabeling-0.2.7/anylabeling/services/auto_labeling/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,17 @@
 class Model:
     BASE_DOWNLOAD_URL = (
         "https://github.com/vietanhdev/anylabeling-assets/raw/main/"
     )
 
     class Meta:
         required_config_names = []
-        buttons = ["button_run"]
+        widgets = ["button_run"]
+        output_modes = ["rectangle"]
+        default_output_mode = "rectangle"
 
     def __init__(self, model_config, on_message) -> None:
         self.on_message = on_message
         # Load and check config
         if isinstance(model_config, str):
             if not os.path.isfile(model_config):
                 raise Exception(f"Config file not found: {model_config}")
@@ -35,20 +37,21 @@
             self.config = model_config
         else:
             raise Exception(f"Unknown config type: {type(model_config)}")
         self.check_missing_config(
             config_names=self.Meta.required_config_names,
             config=self.config,
         )
+        self.output_mode = self.Meta.default_output_mode
 
-    def get_required_buttons(self):
+    def get_required_widgets(self):
         """
-        Get required buttons for showing in UI
+        Get required widgets for showing in UI
         """
-        return self.Meta.buttons
+        return self.Meta.widgets
 
     def get_model_abs_path(self, model_path, model_folder_name):
         """
         Get model absolute path from config path or download from url
         """
         # Try getting model path from config folder
         model_abs_path = os.path.abspath(model_path)
@@ -133,15 +136,15 @@
         Check if config has all required config names
         """
         for name in config_names:
             if name not in config:
                 raise Exception(f"Missing config: {name}")
 
     @abstractmethod
-    def predict_shapes(self, image, image_path=None) -> AutoLabelingResult:
+    def predict_shapes(self, image, filename=None) -> AutoLabelingResult:
         """
         Predict image and return AnyLabeling shapes
         """
         raise NotImplementedError
 
     @abstractmethod
     def unload(self):
@@ -170,7 +173,13 @@
 
     def on_next_files_changed(self, next_files):
         """
         Handle next files changed. This function can preload next files
         and run inference to save time for user.
         """
         pass
+
+    def set_output_mode(self, mode):
+        """
+        Set output mode
+        """
+        self.output_mode = mode
```

### Comparing `anylabeling-0.2.6/anylabeling/services/auto_labeling/model_manager.py` & `anylabeling-0.2.7/anylabeling/services/auto_labeling/model_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,16 @@
     model_loaded = pyqtSignal(list)
     new_auto_labeling_result = pyqtSignal(AutoLabelingResult)
     auto_segmentation_model_selected = pyqtSignal()
     auto_segmentation_model_unselected = pyqtSignal()
     prediction_started = pyqtSignal()
     prediction_finished = pyqtSignal()
     request_next_files_requested = pyqtSignal()
+    output_modes_changed = pyqtSignal(list, str)
+
     model_configs = {}
 
     def __init__(self):
         super().__init__()
         self.model_infos = {}
         self.model_list_config = {}
 
@@ -58,21 +60,30 @@
         """Return model infos"""
         return self.model_infos
 
     def get_model_names(self):
         """Return model names"""
         return list(self.model_infos.keys())
 
+    def set_output_mode(self, mode):
+        """Set output mode"""
+        if self.loaded_model_info and self.loaded_model_info["model"]:
+            self.loaded_model_info["model"].set_output_mode(mode)
+
     @pyqtSlot()
     def on_model_download_finished(self):
         """Handle model download thread finished"""
         self.new_model_status.emit("Model loaded. Ready for labeling.")
         if self.loaded_model_info and self.loaded_model_info["model"]:
             self.model_loaded.emit(
-                self.loaded_model_info["model"].get_required_buttons()
+                self.loaded_model_info["model"].get_required_widgets()
+            )
+            self.output_modes_changed.emit(
+                self.loaded_model_info["model"].Meta.output_modes,
+                self.loaded_model_info["model"].Meta.default_output_mode,
             )
 
     def load_model(self, model_name):
         """Run model loading in a thread"""
         if (
             self.model_download_thread is not None
             and self.model_download_thread.isRunning()
```

### Comparing `anylabeling-0.2.6/anylabeling/services/auto_labeling/segment_anything.py` & `anylabeling-0.2.7/anylabeling/services/auto_labeling/segment_anything.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import os
+import sys
 from copy import deepcopy
 
 import cv2
 import numpy as np
 import onnxruntime
 from PyQt5 import QtCore
 from PyQt5.QtCore import QThread
@@ -24,21 +25,25 @@
         required_config_names = [
             "type",
             "name",
             "display_name",
             "encoder_model_path",
             "decoder_model_path",
         ]
-        buttons = [
+        widgets = [
+            "output_label",
+            "output_select_combobox",
             "button_add_point",
             "button_remove_point",
             "button_add_rect",
             "button_clear",
             "button_finish_object",
         ]
+        output_modes = ["polygon", "rectangle"]
+        default_output_mode = "polygon"
 
     def __init__(self, config_path, on_message) -> None:
         # Run the parent class's init method
         super().__init__(config_path, on_message)
         self.input_size = self.config["input_size"]
         self.max_width = self.config["max_width"]
         self.max_height = self.config["max_height"]
@@ -76,14 +81,15 @@
         # Cache for image embedding
         self.cache_size = 10
         self.preloaded_size = self.cache_size - 3
         self.image_embedding_cache = LRUCache(self.cache_size)
 
         # Pre-inference worker
         self.pre_inference_thread = None
+        self.pre_inference_worker = None
         self.stop_inference = False
 
     def set_auto_labeling_marks(self, marks):
         """Set auto labeling marks"""
         self.marks = marks
 
     def get_input_points(self, resized_ratio):
@@ -238,39 +244,75 @@
             approx = cv2.approxPolyDP(contour, epsilon, True)
             approx_contours.append(approx)
 
         # Remove small contours (area < 20% of average area)
         if len(approx_contours) > 1:
             areas = [cv2.contourArea(contour) for contour in approx_contours]
             avg_area = np.mean(areas)
-            approx_contours = [
+
+            filtered_approx_contours = [
                 contour
-                for contour, area in zip(approx_contours, areas, strict=False)
+                for contour, area in zip(approx_contours, areas)
                 if area > avg_area * 0.2
             ]
+            approx_contours = filtered_approx_contours
 
         # Contours to shapes
         shapes = []
-        for approx in approx_contours:
-            # Scale points
-            points = approx.reshape(-1, 2)
-            points[:, 0] = points[:, 0] / resized_ratio[0]
-            points[:, 1] = points[:, 1] / resized_ratio[1]
-            points = points.tolist()
-            if len(points) < 3:
-                continue
-            points.append(points[0])
+        if self.output_mode == "polygon":
+            for approx in approx_contours:
+                # Scale points
+                points = approx.reshape(-1, 2)
+                points[:, 0] = points[:, 0] / resized_ratio[0]
+                points[:, 1] = points[:, 1] / resized_ratio[1]
+                points = points.tolist()
+                if len(points) < 3:
+                    continue
+                points.append(points[0])
+
+                # Create shape
+                shape = Shape(flags={})
+                for point in points:
+                    point[0] = int(point[0])
+                    point[1] = int(point[1])
+                    shape.add_point(QtCore.QPointF(point[0], point[1]))
+                shape.shape_type = "polygon"
+                shape.closed = True
+                shape.fill_color = "#000000"
+                shape.line_color = "#000000"
+                shape.line_width = 1
+                shape.label = "AUTOLABEL_OBJECT"
+                shape.selected = False
+                shapes.append(shape)
+        elif self.output_mode == "rectangle":
+            x_min = 100000000
+            y_min = 100000000
+            x_max = 0
+            y_max = 0
+            for approx in approx_contours:
+                # Scale points
+                points = approx.reshape(-1, 2)
+                points[:, 0] = points[:, 0] / resized_ratio[0]
+                points[:, 1] = points[:, 1] / resized_ratio[1]
+                points = points.tolist()
+                if len(points) < 3:
+                    continue
+
+                # Get min/max
+                for point in points:
+                    x_min = min(x_min, point[0])
+                    y_min = min(y_min, point[1])
+                    x_max = max(x_max, point[0])
+                    y_max = max(y_max, point[1])
 
             # Create shape
             shape = Shape(flags={})
-            for point in points:
-                point[0] = int(point[0])
-                point[1] = int(point[1])
-                shape.add_point(QtCore.QPointF(point[0], point[1]))
-            shape.type = "polygon"
+            shape.add_point(QtCore.QPointF(x_min, y_min))
+            shape.add_point(QtCore.QPointF(x_max, y_max))
+            shape.shape_type = "rectangle"
             shape.closed = True
             shape.fill_color = "#000000"
             shape.line_color = "#000000"
             shape.line_width = 1
             shape.label = "AUTOLABEL_OBJECT"
             shape.selected = False
             shapes.append(shape)
@@ -313,16 +355,17 @@
             return AutoLabelingResult([], replace=False)
 
         result = AutoLabelingResult(shapes, replace=False)
         return result
 
     def unload(self):
         self.stop_inference = True
-        self.pre_inference_thread.quit()
-        self.pre_inference_thread.wait()
+        if self.pre_inference_thread:
+            self.pre_inference_thread.quit()
+            self.pre_inference_thread.wait()
         if self.encoder_session:
             self.encoder_session = None
         if self.decoder_session:
             self.decoder_session = None
 
     def preload_worker(self, files):
         """
```

### Comparing `anylabeling-0.2.6/anylabeling/services/auto_labeling/types.py` & `anylabeling-0.2.7/anylabeling/services/auto_labeling/types.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/services/auto_labeling/yolov5.py` & `anylabeling-0.2.7/anylabeling/services/auto_labeling/yolov5.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,17 @@
             "input_width",
             "input_height",
             "score_threshold",
             "nms_threshold",
             "confidence_threshold",
             "classes",
         ]
-        buttons = ["button_run"]
+        widgets = ["button_run"]
+        output_modes = ["rectangle"]
+        default_output_mode = "rectangle"
 
     def __init__(self, model_config, on_message) -> None:
         # Run the parent class's init method
         super().__init__(model_config, on_message)
 
         model_abs_path = self.get_model_abs_path(
             self.config["model_path"], self.config["name"]
```

### Comparing `anylabeling-0.2.6/anylabeling/services/auto_labeling/yolov8.py` & `anylabeling-0.2.7/anylabeling/services/auto_labeling/yolov8.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,17 @@
             "input_width",
             "input_height",
             "score_threshold",
             "nms_threshold",
             "confidence_threshold",
             "classes",
         ]
-        buttons = ["button_run"]
+        widgets = ["button_run"]
+        output_modes = ["rectangle"]
+        default_output_mode = "rectangle"
 
     def __init__(self, model_config, on_message) -> None:
         # Run the parent class's init method
         super().__init__(model_config, on_message)
 
         model_abs_path = self.get_model_abs_path(
             self.config["model_path"], self.config["name"]
```

### Comparing `anylabeling-0.2.6/anylabeling/views/common/toaster.py` & `anylabeling-0.2.7/anylabeling/views/common/toaster.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/__main__.py` & `anylabeling-0.2.7/anylabeling/views/labeling/__main__.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/config.py` & `anylabeling-0.2.7/anylabeling/views/labeling/config.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/icons/brain.png` & `anylabeling-0.2.7/anylabeling/views/labeling/icons/brain.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/icons/cancel.png` & `anylabeling-0.2.7/anylabeling/views/labeling/icons/cancel.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/icons/cartesian.png` & `anylabeling-0.2.7/anylabeling/views/labeling/icons/cartesian.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/icons/circle.png` & `anylabeling-0.2.7/anylabeling/views/labeling/icons/circle.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/icons/color-line.png` & `anylabeling-0.2.7/anylabeling/views/labeling/icons/color-line.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/icons/color.png` & `anylabeling-0.2.7/anylabeling/views/labeling/icons/color.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/icons/color_line.png` & `anylabeling-0.2.7/anylabeling/views/labeling/icons/color_line.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/icons/copy.png` & `anylabeling-0.2.7/anylabeling/views/labeling/icons/copy.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/icons/delete.png` & `anylabeling-0.2.7/anylabeling/views/labeling/icons/delete.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/icons/done.png` & `anylabeling-0.2.7/anylabeling/views/labeling/icons/done.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/icons/done.svg` & `anylabeling-0.2.7/anylabeling/views/labeling/icons/done.svg`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/icons/edit.png` & `anylabeling-0.2.7/anylabeling/views/labeling/icons/edit.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/icons/expert.png` & `anylabeling-0.2.7/anylabeling/views/labeling/icons/expert.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/icons/eye.png` & `anylabeling-0.2.7/anylabeling/views/labeling/icons/eye.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/icons/feBlend-icon.png` & `anylabeling-0.2.7/anylabeling/views/labeling/icons/feBlend-icon.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/icons/file.png` & `anylabeling-0.2.7/anylabeling/views/labeling/icons/file.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/icons/fit-width.png` & `anylabeling-0.2.7/anylabeling/views/labeling/icons/fit-width.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/icons/fit-window.png` & `anylabeling-0.2.7/anylabeling/views/labeling/icons/fit-window.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/icons/fit.png` & `anylabeling-0.2.7/anylabeling/views/labeling/icons/fit.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/icons/format_createml.png` & `anylabeling-0.2.7/anylabeling/views/labeling/icons/format_createml.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/icons/format_voc.png` & `anylabeling-0.2.7/anylabeling/views/labeling/icons/format_voc.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/icons/format_yolo.png` & `anylabeling-0.2.7/anylabeling/views/labeling/icons/format_yolo.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/icons/help.png` & `anylabeling-0.2.7/anylabeling/views/labeling/icons/help.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/icons/icon.png` & `anylabeling-0.2.7/anylabeling/views/labeling/icons/icon.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/icons/labels.png` & `anylabeling-0.2.7/anylabeling/views/labeling/icons/labels.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/icons/labels.svg` & `anylabeling-0.2.7/anylabeling/views/labeling/icons/labels.svg`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/icons/line-strip.png` & `anylabeling-0.2.7/anylabeling/views/labeling/icons/line-strip.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/icons/line.png` & `anylabeling-0.2.7/anylabeling/views/labeling/icons/line.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/icons/new.png` & `anylabeling-0.2.7/anylabeling/views/labeling/icons/new.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/icons/next.png` & `anylabeling-0.2.7/anylabeling/views/labeling/icons/next.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/icons/objects.png` & `anylabeling-0.2.7/anylabeling/views/labeling/icons/objects.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/icons/open.png` & `anylabeling-0.2.7/anylabeling/views/labeling/icons/open.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/icons/paste.png` & `anylabeling-0.2.7/anylabeling/views/labeling/icons/paste.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/icons/point.png` & `anylabeling-0.2.7/anylabeling/views/labeling/icons/point.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/icons/polygon.png` & `anylabeling-0.2.7/anylabeling/views/labeling/icons/polygon.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/icons/prev.png` & `anylabeling-0.2.7/anylabeling/views/labeling/icons/prev.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/icons/quit.png` & `anylabeling-0.2.7/anylabeling/views/labeling/icons/quit.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/icons/rectangle.png` & `anylabeling-0.2.7/anylabeling/views/labeling/icons/rectangle.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/icons/resetall.png` & `anylabeling-0.2.7/anylabeling/views/labeling/icons/resetall.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/icons/save-as.png` & `anylabeling-0.2.7/anylabeling/views/labeling/icons/save-as.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/icons/save.png` & `anylabeling-0.2.7/anylabeling/views/labeling/icons/save.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/icons/undo-cross.png` & `anylabeling-0.2.7/anylabeling/views/labeling/icons/undo-cross.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/icons/undo.png` & `anylabeling-0.2.7/anylabeling/views/labeling/icons/undo.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/icons/upload_brain.png` & `anylabeling-0.2.7/anylabeling/views/labeling/icons/upload_brain.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/icons/verify.png` & `anylabeling-0.2.7/anylabeling/views/labeling/icons/verify.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/icons/zoom-in.png` & `anylabeling-0.2.7/anylabeling/views/labeling/icons/zoom-in.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/icons/zoom-out.png` & `anylabeling-0.2.7/anylabeling/views/labeling/icons/zoom-out.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/icons/zoom.png` & `anylabeling-0.2.7/anylabeling/views/labeling/icons/zoom.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/label_file.py` & `anylabeling-0.2.7/anylabeling/views/labeling/label_file.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/label_widget.py` & `anylabeling-0.2.7/anylabeling/views/labeling/label_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -1175,14 +1175,16 @@
             disable_auto_labeling
             and self.auto_labeling_widget.auto_labeling_mode
             != AutoLabelingMode.NONE
         ):
             self.clear_auto_labeling_marks()
             self.auto_labeling_widget.set_auto_labeling_mode(None)
 
+        self.set_text_editing(False)
+
         self.canvas.set_editing(edit)
         self.canvas.create_mode = create_mode
         if edit:
             self.actions.create_mode.setEnabled(True)
             self.actions.create_rectangle_mode.setEnabled(True)
             self.actions.create_cirle_mode.setEnabled(True)
             self.actions.create_line_mode.setEnabled(True)
@@ -1230,21 +1232,24 @@
                 self.actions.create_cirle_mode.setEnabled(True)
                 self.actions.create_line_mode.setEnabled(True)
                 self.actions.create_point_mode.setEnabled(True)
                 self.actions.create_line_strip_mode.setEnabled(False)
             else:
                 raise ValueError(f"Unsupported create_mode: {create_mode}")
         self.actions.edit_mode.setEnabled(not edit)
+        self.label_instruction.setText(self.get_labeling_instruction())
 
     def set_edit_mode(self):
         # Disable auto labeling
         self.clear_auto_labeling_marks()
         self.auto_labeling_widget.set_auto_labeling_mode(None)
 
         self.toggle_draw_mode(True)
+        self.set_text_editing(True)
+        self.label_instruction.setText(self.get_labeling_instruction())
 
     def update_file_menu(self):
         current = self.filename
 
         def exists(filename):
             return osp.exists(str(filename))
 
@@ -1368,26 +1373,15 @@
             self.label_list.scroll_to_item(item)
         self._no_selection_slot = False
         n_selected = len(selected_shapes)
         self.actions.delete.setEnabled(n_selected)
         self.actions.duplicate.setEnabled(n_selected)
         self.actions.copy.setEnabled(n_selected)
         self.actions.edit.setEnabled(n_selected == 1)
-        if len(selected_shapes) == 1:
-            self.shape_text_label.setText("Object Text")
-            self.shape_text_edit.textChanged.disconnect()
-            self.shape_text_edit.setPlainText(selected_shapes[0].text)
-            self.shape_text_edit.textChanged.connect(self.shape_text_changed)
-        else:
-            self.shape_text_label.setText("Image Text")
-            self.shape_text_edit.textChanged.disconnect()
-            self.shape_text_edit.setPlainText(
-                self.other_data.get("image_text", "")
-            )
-            self.shape_text_edit.textChanged.connect(self.shape_text_changed)
+        self.set_text_editing(True)
 
     def add_label(self, shape):
         if shape.group_id is None:
             text = shape.label
         else:
             text = f"{shape.label} ({shape.group_id})"
         label_list_item = LabelListWidgetItem(text, shape)
@@ -1782,14 +1776,15 @@
         """Get the next files in the list."""
         if not self.image_list:
             return []
         filenames = []
         current_index = 0
         if filename is not None:
             current_index = self.image_list.index(filename)
+            filenames.append(filename)
         for _ in range(num_files):
             if current_index + 1 < len(self.image_list):
                 filenames.append(self.image_list[current_index + 1])
                 current_index += 1
             else:
                 filenames.append(self.image_list[-1])
                 break
@@ -2587,7 +2582,36 @@
 
         # Update shape colors
         for shape in self.canvas.shapes:
             self._update_shape_color(shape)
 
         if updated_shapes:
             self.set_dirty()
+
+    def set_text_editing(self, enable):
+        """Set text editing."""
+        if enable:
+            # Enable text editing and set shape text from selected shape
+            if len(self.canvas.selected_shapes) == 1:
+                self.shape_text_label.setText("Object Text")
+                self.shape_text_edit.textChanged.disconnect()
+                self.shape_text_edit.setPlainText(
+                    self.canvas.selected_shapes[0].text
+                )
+                self.shape_text_edit.textChanged.connect(
+                    self.shape_text_changed
+                )
+            else:
+                self.shape_text_label.setText("Image Text")
+                self.shape_text_edit.textChanged.disconnect()
+                self.shape_text_edit.setPlainText(
+                    self.other_data.get("image_text", "")
+                )
+                self.shape_text_edit.textChanged.connect(
+                    self.shape_text_changed
+                )
+        else:
+            self.shape_text_edit.setDisabled(True)
+            self.shape_text_label.setText("Switch to Edit mode to edit text")
+            self.shape_text_edit.textChanged.disconnect()
+            self.shape_text_edit.setPlainText("")
+            self.shape_text_edit.textChanged.connect(self.shape_text_changed)
```

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/label_wrapper.py` & `anylabeling-0.2.7/anylabeling/views/labeling/label_wrapper.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/logger.py` & `anylabeling-0.2.7/anylabeling/views/labeling/logger.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/shape.py` & `anylabeling-0.2.7/anylabeling/views/labeling/shape.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/testing.py` & `anylabeling-0.2.7/anylabeling/views/labeling/testing.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/utils/__init__.py` & `anylabeling-0.2.7/anylabeling/views/labeling/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/utils/_io.py` & `anylabeling-0.2.7/anylabeling/views/labeling/utils/_io.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/utils/image.py` & `anylabeling-0.2.7/anylabeling/views/labeling/utils/image.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/utils/qt.py` & `anylabeling-0.2.7/anylabeling/views/labeling/utils/qt.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/utils/shape.py` & `anylabeling-0.2.7/anylabeling/views/labeling/utils/shape.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py` & `anylabeling-0.2.7/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,42 +9,49 @@
 
 
 class AutoLabelingWidget(QWidget):
     new_model_selected = pyqtSignal(str)
     auto_segmentation_requested = pyqtSignal()
     auto_segmentation_disabled = pyqtSignal()
     auto_labeling_mode_changed = pyqtSignal(AutoLabelingMode)
-    undo_auto_labeling_action_requested = pyqtSignal()
     clear_auto_labeling_action_requested = pyqtSignal()
     finish_auto_labeling_object_action_requested = pyqtSignal()
 
     def __init__(self, parent):
         super().__init__()
         self.parent = parent
         current_dir = os.path.dirname(__file__)
         uic.loadUi(os.path.join(current_dir, "auto_labeling.ui"), self)
 
         self.model_manager = ModelManager()
         self.model_manager.new_model_status.connect(self.on_new_model_status)
         self.new_model_selected.connect(self.model_manager.load_model)
-        self.model_manager.model_loaded.connect(self.update_visible_buttons)
+        self.model_manager.model_loaded.connect(self.update_visible_widgets)
         self.model_manager.model_loaded.connect(
             self.enable_model_select_combobox
         )
         self.model_manager.new_auto_labeling_result.connect(
             lambda auto_labeling_result: self.parent.new_shapes_from_auto_labeling(
                 auto_labeling_result
             )
         )
         self.model_manager.auto_segmentation_model_selected.connect(
             self.auto_segmentation_requested
         )
         self.model_manager.auto_segmentation_model_unselected.connect(
             self.auto_segmentation_disabled
         )
+        self.model_manager.output_modes_changed.connect(
+            self.on_output_modes_changed
+        )
+        self.output_select_combobox.currentIndexChanged.connect(
+            lambda: self.model_manager.set_output_mode(
+                self.output_select_combobox.currentText()
+            )
+        )
 
         # Add models to combobox
         self.model_select_combobox.clear()
         self.model_select_combobox.addItem("No Model", userData=None)
         for model_info in self.model_manager.get_model_infos().values():
             self.model_select_combobox.addItem(
                 model_info["display_name"], userData=model_info["name"]
@@ -64,27 +71,24 @@
             )
         )
         self.button_add_rect.clicked.connect(
             lambda: self.set_auto_labeling_mode(
                 AutoLabelingMode.ADD, AutoLabelingMode.RECTANGLE
             )
         )
-        self.button_undo.clicked.connect(
-            self.undo_auto_labeling_action_requested
-        )
         self.button_clear.clicked.connect(
             self.clear_auto_labeling_action_requested
         )
         self.button_finish_object.clicked.connect(
             self.finish_auto_labeling_object_action_requested
         )
         self.button_finish_object.setShortcut("F")
 
-        # Hide labeling buttons by default
-        self.hide_labeling_buttons()
+        # Hide labeling widgets by default
+        self.hide_labeling_widgets()
 
         # Handle close button
         self.button_close.clicked.connect(self.unload_and_hide)
 
         # Handle model select combobox
         self.model_select_combobox.currentIndexChanged.connect(
             self.on_model_select_combobox_changed
@@ -105,15 +109,14 @@
             border: 1px solid #999999;
         """
         for button in [
             self.button_add_point,
             self.button_remove_point,
             self.button_add_rect,
             self.button_clear,
-            self.button_undo,
             self.button_finish_object,
         ]:
             button.setStyleSheet(style_sheet + "background-color: #ffffff;")
         if self.auto_labeling_mode == AutoLabelingMode.NONE:
             return
         if self.auto_labeling_mode.edit_mode == AutoLabelingMode.ADD:
             if self.auto_labeling_mode.shape_type == AutoLabelingMode.POINT:
@@ -156,40 +159,60 @@
     def on_new_model_status(self, status):
         self.model_status_label.setText(status)
 
     @pyqtSlot()
     def enable_model_select_combobox(self):
         self.model_select_combobox.setEnabled(True)
 
+    def on_output_modes_changed(self, output_modes, default_output_mode):
+        """Handle output modes changed"""
+        # Disconnect onIndexChanged signal to prevent triggering
+        # on model select combobox change
+        self.output_select_combobox.currentIndexChanged.disconnect()
+
+        self.output_select_combobox.clear()
+        for output_mode in output_modes:
+            self.output_select_combobox.addItem(output_mode)
+        self.output_select_combobox.setCurrentText(default_output_mode)
+
+        # Reconnect onIndexChanged signal
+        self.output_select_combobox.currentIndexChanged.connect(
+            lambda: self.model_manager.set_output_mode(
+                self.output_select_combobox.currentText()
+            )
+        )
+
     def on_model_select_combobox_changed(self, index):
+        """Handle model select combobox change"""
         model_name = self.model_select_combobox.itemData(index)
         # Disable combobox while loading model
         if model_name:
             self.model_select_combobox.setEnabled(False)
-        self.hide_labeling_buttons()
+        self.hide_labeling_widgets()
         self.new_model_selected.emit(model_name)
 
-    def update_visible_buttons(self, buttons):
-        """Update button status"""
-        for button in buttons:
-            getattr(self, button).show()
-
-    def hide_labeling_buttons(self):
-        """Hide labeling buttons by default"""
-        buttons = [
+    def update_visible_widgets(self, widgets):
+        """Update widget status"""
+        for widget in widgets:
+            getattr(self, widget).show()
+
+    def hide_labeling_widgets(self):
+        """Hide labeling widgets by default"""
+        widgets = [
+            "output_label",
+            "output_select_combobox",
             "button_run",
             "button_add_point",
             "button_remove_point",
             "button_add_rect",
-            "button_undo",
             "button_clear",
             "button_finish_object",
         ]
-        for button in buttons:
-            getattr(self, button).hide()
+        for widget in widgets:
+            getattr(self, widget).hide()
 
     def on_new_marks(self, marks):
         """Handle new marks"""
         self.model_manager.set_auto_labeling_marks(marks)
         self.run_prediction()
 
     def on_open(self):
```

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui` & `anylabeling-0.2.7/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui`

 * *Files 10% similar despite different names*

#### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui` & `anylabeling-0.2.7/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui`

```diff
@@ -2,15 +2,15 @@
 <ui version="4.0">
   <class>auto_labeling_form</class>
   <widget class="QWidget" name="auto_labeling_form">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
-        <width>1055</width>
+        <width>1205</width>
         <height>42</height>
       </rect>
     </property>
     <property name="sizePolicy">
       <sizepolicy hsizetype="Minimum" vsizetype="Minimum">
         <horstretch>0</horstretch>
         <verstretch>0</verstretch>
@@ -40,17 +40,17 @@
           <property name="spacing">
             <number>2</number>
           </property>
           <property name="topMargin">
             <number>0</number>
           </property>
           <item>
-            <widget class="QLabel" name="model">
+            <widget class="QLabel" name="model_label">
               <property name="text">
-                <string>Auto Labeling</string>
+                <string>Auto</string>
               </property>
             </widget>
           </item>
           <item>
             <widget class="QComboBox" name="model_select_combobox">
               <property name="enabled">
                 <bool>true</bool>
@@ -65,14 +65,35 @@
                 <property name="text">
                   <string>No Model</string>
                 </property>
               </item>
             </widget>
           </item>
           <item>
+            <widget class="QLabel" name="output_label">
+              <property name="text">
+                <string>Output</string>
+              </property>
+            </widget>
+          </item>
+          <item>
+            <widget class="QComboBox" name="output_select_combobox">
+              <item>
+                <property name="text">
+                  <string>polygon</string>
+                </property>
+              </item>
+              <item>
+                <property name="text">
+                  <string>rectangle</string>
+                </property>
+              </item>
+            </widget>
+          </item>
+          <item>
             <widget class="Line" name="line">
               <property name="orientation">
                 <enum>Qt::Vertical</enum>
               </property>
             </widget>
           </item>
           <item>
@@ -100,21 +121,14 @@
             <widget class="QPushButton" name="button_add_rect">
               <property name="text">
                 <string>+Rect</string>
               </property>
             </widget>
           </item>
           <item>
-            <widget class="QPushButton" name="button_undo">
-              <property name="text">
-                <string>Undo</string>
-              </property>
-            </widget>
-          </item>
-          <item>
             <widget class="QPushButton" name="button_clear">
               <property name="text">
                 <string>Clear</string>
               </property>
             </widget>
           </item>
           <item>
@@ -145,16 +159,34 @@
                   <height>0</height>
                 </size>
               </property>
             </spacer>
           </item>
           <item>
             <widget class="QPushButton" name="button_close">
-              <property name="text">
-                <string>Close</string>
+              <property name="sizePolicy">
+                <sizepolicy hsizetype="Minimum" vsizetype="Fixed">
+                  <horstretch>0</horstretch>
+                  <verstretch>0</verstretch>
+                </sizepolicy>
+              </property>
+              <property name="text">
+                <string/>
+              </property>
+              <property name="icon">
+                <iconset resource="../../../../resources/resources.qrc">
+                  <normaloff>:/images/images/cancel.png</normaloff>
+                  :/images/images/cancel.png
+                </iconset>
+              </property>
+              <property name="iconSize">
+                <size>
+                  <width>12</width>
+                  <height>12</height>
+                </size>
               </property>
             </widget>
           </item>
         </layout>
       </item>
     </layout>
   </widget>
```

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py` & `anylabeling-0.2.7/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/widgets/canvas.py` & `anylabeling-0.2.7/anylabeling/views/labeling/widgets/canvas.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,15 +216,18 @@
             self.auto_labeling_mode = AutoLabelingMode.NONE
             self.parent.toggle_draw_mode(
                 False, "rectangle", disable_auto_labeling=True
             )
 
     def get_mode(self):
         """Get current mode"""
-        if self.is_auto_labeling:
+        if (
+            self.is_auto_labeling
+            and self.auto_labeling_mode != AutoLabelingMode.NONE
+        ):
             return "Auto Labeling"
         if self.mode == self.CREATE:
             return "Drawing"
         elif self.mode == self.EDIT:
             return "Editing"
         else:
             return "Unknown"
```

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/widgets/color_dialog.py` & `anylabeling-0.2.7/anylabeling/views/labeling/widgets/color_dialog.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/widgets/file_dialog_preview.py` & `anylabeling-0.2.7/anylabeling/views/labeling/widgets/file_dialog_preview.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/widgets/label_dialog.py` & `anylabeling-0.2.7/anylabeling/views/labeling/widgets/label_dialog.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/widgets/label_list_widget.py` & `anylabeling-0.2.7/anylabeling/views/labeling/widgets/label_list_widget.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/widgets/toolbar.py` & `anylabeling-0.2.7/anylabeling/views/labeling/widgets/toolbar.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py` & `anylabeling-0.2.7/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/labeling/widgets/zoom_widget.py` & `anylabeling-0.2.7/anylabeling/views/labeling/widgets/zoom_widget.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling/views/mainwindow.py` & `anylabeling-0.2.7/anylabeling/views/mainwindow.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/anylabeling.egg-info/PKG-INFO` & `anylabeling-0.2.7/anylabeling.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anylabeling
-Version: 0.2.6
+Version: 0.2.7
 Summary: Effortless data labeling with AI support
 Home-page: https://github.com/vietanhdev/anylabeling
 Author: Viet-Anh Nguyen
 Author-email: vietanh.dev@gmail.com
 License: GPLv3
 Keywords: Image Annotation,Machine Learning,Deep Learning
 Classifier: Intended Audience :: Developers
@@ -29,19 +29,19 @@
 ![](https://i.imgur.com/waxVImv.png)
 
 [![PyPI](https://img.shields.io/pypi/v/anylabeling)](https://pypi.org/project/anylabeling)
 [![license](https://img.shields.io/github/license/vietanhdev/anylabeling.svg)](https://github.com/vietanhdev/anylabeling/blob/master/LICENSE)
 [![open issues](https://isitmaintained.com/badge/open/vietanhdev/anylabeling.svg)](https://github.com/vietanhdev/anylabeling/issues)
 [![Pypi Downloads](https://pepy.tech/badge/anylabeling)](https://pypi.org/project/anylabeling/)
 
-<a href="https://www.youtube.com/watch?v=5iQSGL7ebXE">
+<a href="https://www.youtube.com/watch?v=xLVz-f6OeUY">
   <img alt="AnyLabeling" src="https://user-images.githubusercontent.com/18329471/232266520-1f52cd45-0776-479e-8a3c-4fef144c6b73.png"/>
 </a>
 
-- **Youtube Demo:** [https://www.youtube.com/watch?v=5iQSGL7ebXE](https://www.youtube.com/watch?v=5iQSGL7ebXE)
+- **Youtube Demo:** [https://www.youtube.com/watch?v=xLVz-f6OeUY](https://www.youtube.com/watch?v=xLVz-f6OeUY)
 - **Documentation:** [https://anylabeling.com](https://anylabeling.com)
 
 ## I. Install and run
 
 - Requirements: Python >= 3.8
 - Recommended: Miniconda/Anaconda <https://docs.conda.io/en/latest/miniconda.html>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: anylabeling Version: 0.2.6 Summary: Effortless data
+Metadata-Version: 2.1 Name: anylabeling Version: 0.2.7 Summary: Effortless data
 labeling with AI support Home-page: https://github.com/vietanhdev/anylabeling
 Author: Viet-Anh Nguyen Author-email: vietanh.dev@gmail.com License: GPLv3
 Keywords: Image Annotation,Machine Learning,Deep Learning Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
@@ -16,16 +16,16 @@
 ![](https://i.imgur.com/waxVImv.png) [![PyPI](https://img.shields.io/pypi/v/
 anylabeling)](https://pypi.org/project/anylabeling) [![license](https://
 img.shields.io/github/license/vietanhdev/anylabeling.svg)](https://github.com/
 vietanhdev/anylabeling/blob/master/LICENSE) [![open issues](https://
 isitmaintained.com/badge/open/vietanhdev/anylabeling.svg)](https://github.com/
 vietanhdev/anylabeling/issues) [![Pypi Downloads](https://pepy.tech/badge/
 anylabeling)](https://pypi.org/project/anylabeling/) [AnyLabeling] - **Youtube
-Demo:** [https://www.youtube.com/watch?v=5iQSGL7ebXE](https://www.youtube.com/
-watch?v=5iQSGL7ebXE) - **Documentation:** [https://anylabeling.com](https://
+Demo:** [https://www.youtube.com/watch?v=xLVz-f6OeUY](https://www.youtube.com/
+watch?v=xLVz-f6OeUY) - **Documentation:** [https://anylabeling.com](https://
 anylabeling.com) ## I. Install and run - Requirements: Python >= 3.8 -
 Recommended: Miniconda/Anaconda
 docs.conda.io/en/latest/miniconda.html> - Create environment: ```bash conda
 create -n anylabeling python=3.8 conda activate anylabeling ``` - **(For macOS
 only)** Install PyQt5 using Conda: ```bash conda install -c conda-forge
 pyqt==5.15.7 ``` - Install anylabeling: ```bash pip install anylabeling ``` -
 Run app: ```bash anylabeling ``` Or ```bash python -m anylabeling.app ``` ##
```

### Comparing `anylabeling-0.2.6/anylabeling.egg-info/SOURCES.txt` & `anylabeling-0.2.7/anylabeling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.6/setup.py` & `anylabeling-0.2.7/setup.py`

 * *Files identical despite different names*

