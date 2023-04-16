# Comparing `tmp/anylabeling-0.2.4.tar.gz` & `tmp/anylabeling-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anylabeling-0.2.4.tar", last modified: Sat Apr 15 19:45:11 2023, max compression
+gzip compressed data, was "anylabeling-0.2.6.tar", last modified: Sun Apr 16 09:02:24 2023, max compression
```

## Comparing `anylabeling-0.2.4.tar` & `anylabeling-0.2.6.tar`

### file list

```diff
@@ -1,145 +1,145 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:45:11.464981 anylabeling-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-15 19:45:02.000000 anylabeling-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-15 19:45:02.000000 anylabeling-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-04-15 19:45:11.464981 anylabeling-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-04-15 19:45:02.000000 anylabeling-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:45:11.448981 anylabeling-0.2.4/anylabeling/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/app_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:45:11.448981 anylabeling-0.2.4/anylabeling/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/configs/anylabeling_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:45:11.448981 anylabeling-0.2.4/anylabeling/configs/auto_labeling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/configs/auto_labeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/configs/auto_labeling/models.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/configs/auto_labeling/segment_anything_vit_b.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/configs/auto_labeling/segment_anything_vit_b_quant.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/configs/auto_labeling/segment_anything_vit_h_quant.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/configs/auto_labeling/segment_anything_vit_l.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/configs/auto_labeling/segment_anything_vit_l_quant.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/configs/auto_labeling/yolov5l.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/configs/auto_labeling/yolov5m.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/configs/auto_labeling/yolov5n.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/configs/auto_labeling/yolov5s.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/configs/auto_labeling/yolov5x.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/configs/auto_labeling/yolov8l.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/configs/auto_labeling/yolov8m.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/configs/auto_labeling/yolov8n.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/configs/auto_labeling/yolov8s.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/configs/auto_labeling/yolov8x.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:45:11.448981 anylabeling-0.2.4/anylabeling/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   477720 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/resources/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:45:11.452981 anylabeling-0.2.4/anylabeling/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:45:11.452981 anylabeling-0.2.4/anylabeling/services/auto_labeling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/services/auto_labeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/services/auto_labeling/lru_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/services/auto_labeling/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8822 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/services/auto_labeling/model_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    12654 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/services/auto_labeling/segment_anything.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/services/auto_labeling/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/services/auto_labeling/yolov5.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/services/auto_labeling/yolov8.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:45:11.452981 anylabeling-0.2.4/anylabeling/views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:45:11.452981 anylabeling-0.2.4/anylabeling/views/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9583 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/common/toaster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:45:11.452981 anylabeling-0.2.4/anylabeling/views/labeling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:45:11.460981 anylabeling-0.2.4/anylabeling/views/labeling/icons/
--rw-r--r--   0 runner    (1001) docker     (123)    28068 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/brain.png
--rw-r--r--   0 runner    (1001) docker     (123)     6844 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/cancel.png
--rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/cartesian.png
--rw-r--r--   0 runner    (1001) docker     (123)    15818 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/circle.png
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/color-line.png
--rw-r--r--   0 runner    (1001) docker     (123)    23824 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/color.png
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/color_line.png
--rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/copy.png
--rw-r--r--   0 runner    (1001) docker     (123)     7842 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/delete.png
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/done.png
--rw-r--r--   0 runner    (1001) docker     (123)    22232 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/done.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15023 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/edit.png
--rw-r--r--   0 runner    (1001) docker     (123)     7718 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/expert.png
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/expert1.png
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/expert2.png
--rw-r--r--   0 runner    (1001) docker     (123)    37652 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/eye.png
--rw-r--r--   0 runner    (1001) docker     (123)     8059 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/feBlend-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/file.png
--rw-r--r--   0 runner    (1001) docker     (123)    17368 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/fit-width.png
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/fit-window.png
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/fit.png
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/format_createml.png
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/format_voc.png
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/format_yolo.png
--rw-r--r--   0 runner    (1001) docker     (123)    14479 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/help.png
--rw-r--r--   0 runner    (1001) docker     (123)    44771 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/labels.png
--rw-r--r--   0 runner    (1001) docker     (123)    36597 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/labels.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/line-strip.png
--rw-r--r--   0 runner    (1001) docker     (123)     9457 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/line.png
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/new.png
--rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/next.png
--rw-r--r--   0 runner    (1001) docker     (123)    26255 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/objects.png
--rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/open.png
--rw-r--r--   0 runner    (1001) docker     (123)    10572 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/paste.png
--rw-r--r--   0 runner    (1001) docker     (123)    13847 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/point.png
--rw-r--r--   0 runner    (1001) docker     (123)    14286 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/polygon.png
--rw-r--r--   0 runner    (1001) docker     (123)     7275 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/prev.png
--rw-r--r--   0 runner    (1001) docker     (123)    22460 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/quit.png
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/rectangle.png
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/resetall.png
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/save-as.png
--rw-r--r--   0 runner    (1001) docker     (123)     6118 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/save.png
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/undo-cross.png
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/undo.png
--rw-r--r--   0 runner    (1001) docker     (123)    18083 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/upload_brain.png
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/verify.png
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/zoom-in.png
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/zoom-out.png
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/icons/zoom.png
--rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/label_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    92452 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/label_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/label_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    10441 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/shape.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:45:11.460981 anylabeling-0.2.4/anylabeling/views/labeling/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/utils/_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/utils/opencv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/utils/qt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/utils/shape.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:45:11.464981 anylabeling-0.2.4/anylabeling/views/labeling/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/widgets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:45:11.464981 anylabeling-0.2.4/anylabeling/views/labeling/widgets/auto_labeling/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/widgets/auto_labeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)    48612 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/widgets/canvas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/widgets/color_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/widgets/escapable_qlist_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/widgets/file_dialog_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/widgets/label_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/widgets/label_list_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/widgets/toolbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/labeling/widgets/zoom_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-15 19:45:02.000000 anylabeling-0.2.4/anylabeling/views/mainwindow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:45:11.448981 anylabeling-0.2.4/anylabeling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-04-15 19:45:11.000000 anylabeling-0.2.4/anylabeling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-04-15 19:45:11.000000 anylabeling-0.2.4/anylabeling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 19:45:11.000000 anylabeling-0.2.4/anylabeling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-15 19:45:11.000000 anylabeling-0.2.4/anylabeling.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-15 19:45:11.000000 anylabeling-0.2.4/anylabeling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-15 19:45:11.000000 anylabeling-0.2.4/anylabeling.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-15 19:45:02.000000 anylabeling-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 19:45:11.464981 anylabeling-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-15 19:45:02.000000 anylabeling-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:02:24.222624 anylabeling-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-16 09:02:15.000000 anylabeling-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-16 09:02:15.000000 anylabeling-0.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-04-16 09:02:24.222624 anylabeling-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-16 09:02:15.000000 anylabeling-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:02:24.206624 anylabeling-0.2.6/anylabeling/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/app_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:02:24.206624 anylabeling-0.2.6/anylabeling/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/configs/anylabeling_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:02:24.210624 anylabeling-0.2.6/anylabeling/configs/auto_labeling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/configs/auto_labeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/configs/auto_labeling/models.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/configs/auto_labeling/segment_anything_vit_b.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/configs/auto_labeling/segment_anything_vit_b_quant.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/configs/auto_labeling/segment_anything_vit_h_quant.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/configs/auto_labeling/segment_anything_vit_l.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/configs/auto_labeling/segment_anything_vit_l_quant.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/configs/auto_labeling/yolov5l.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/configs/auto_labeling/yolov5m.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/configs/auto_labeling/yolov5n.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/configs/auto_labeling/yolov5s.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/configs/auto_labeling/yolov5x.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/configs/auto_labeling/yolov8l.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/configs/auto_labeling/yolov8m.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/configs/auto_labeling/yolov8n.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/configs/auto_labeling/yolov8s.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/configs/auto_labeling/yolov8x.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:02:24.210624 anylabeling-0.2.6/anylabeling/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   477720 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/resources/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:02:24.210624 anylabeling-0.2.6/anylabeling/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:02:24.210624 anylabeling-0.2.6/anylabeling/services/auto_labeling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/services/auto_labeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/services/auto_labeling/lru_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/services/auto_labeling/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8822 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/services/auto_labeling/model_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/services/auto_labeling/segment_anything.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/services/auto_labeling/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/services/auto_labeling/yolov5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/services/auto_labeling/yolov8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:02:24.210624 anylabeling-0.2.6/anylabeling/views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:02:24.210624 anylabeling-0.2.6/anylabeling/views/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9583 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/common/toaster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:02:24.214624 anylabeling-0.2.6/anylabeling/views/labeling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:02:24.218624 anylabeling-0.2.6/anylabeling/views/labeling/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)    28068 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/brain.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6844 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/cancel.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/cartesian.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15818 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/circle.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/color-line.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23824 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/color.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/color_line.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/copy.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7842 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/delete.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/done.png
+-rw-r--r--   0 runner    (1001) docker     (123)    22232 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/done.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15023 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/edit.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7718 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/expert.png
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/expert1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/expert2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    37652 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/eye.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8059 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/feBlend-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/file.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17368 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/fit-width.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/fit-window.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/fit.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/format_createml.png
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/format_voc.png
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/format_yolo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14479 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/help.png
+-rw-r--r--   0 runner    (1001) docker     (123)    44771 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/labels.png
+-rw-r--r--   0 runner    (1001) docker     (123)    36597 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/labels.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/line-strip.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9457 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/line.png
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/new.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/next.png
+-rw-r--r--   0 runner    (1001) docker     (123)    26255 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/objects.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/open.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10572 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/paste.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13847 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/point.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14286 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/polygon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7275 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/prev.png
+-rw-r--r--   0 runner    (1001) docker     (123)    22460 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/quit.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/rectangle.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/resetall.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/save-as.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6118 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/save.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/undo-cross.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/undo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18083 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/upload_brain.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/verify.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/zoom-in.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/zoom-out.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/icons/zoom.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/label_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92452 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/label_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/label_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10828 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:02:24.218624 anylabeling-0.2.6/anylabeling/views/labeling/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/utils/_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/utils/opencv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/utils/qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/utils/shape.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:02:24.222624 anylabeling-0.2.6/anylabeling/views/labeling/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/widgets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:02:24.222624 anylabeling-0.2.6/anylabeling/views/labeling/widgets/auto_labeling/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/widgets/auto_labeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48612 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/widgets/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/widgets/color_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/widgets/escapable_qlist_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/widgets/file_dialog_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/widgets/label_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/widgets/label_list_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/widgets/toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/labeling/widgets/zoom_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-16 09:02:15.000000 anylabeling-0.2.6/anylabeling/views/mainwindow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:02:24.206624 anylabeling-0.2.6/anylabeling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-04-16 09:02:24.000000 anylabeling-0.2.6/anylabeling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-04-16 09:02:24.000000 anylabeling-0.2.6/anylabeling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 09:02:24.000000 anylabeling-0.2.6/anylabeling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-16 09:02:24.000000 anylabeling-0.2.6/anylabeling.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-16 09:02:24.000000 anylabeling-0.2.6/anylabeling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-16 09:02:24.000000 anylabeling-0.2.6/anylabeling.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-16 09:02:15.000000 anylabeling-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 09:02:24.222624 anylabeling-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-16 09:02:15.000000 anylabeling-0.2.6/setup.py
```

### Comparing `anylabeling-0.2.4/LICENSE` & `anylabeling-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/PKG-INFO` & `anylabeling-0.2.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anylabeling
-Version: 0.2.4
+Version: 0.2.6
 Summary: Effortless data labeling with AI support
 Home-page: https://github.com/vietanhdev/anylabeling
 Author: Viet-Anh Nguyen
 Author-email: vietanh.dev@gmail.com
 License: GPLv3
 Keywords: Image Annotation,Machine Learning,Deep Learning
 Classifier: Intended Audience :: Developers
@@ -16,32 +16,33 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
-  <img style="width: 150px; max-width: 100%; height: auto; border-radius: 20px; overflow: hidden;" src="https://user-images.githubusercontent.com/18329471/232231236-6d6a1a79-22c9-4cbc-9132-c81cbc201265.png"/>
+  <img alt="AnyLabeling" style="width: 128px; max-width: 100%; height: auto;" src="https://user-images.githubusercontent.com/18329471/232250539-2b15b9ee-5593-41d0-ba22-e0442f314cce.png"/>
   <h1 align="center">🌟 AnyLabeling 🌟</h1>
   <p align="center">Effortless data labeling with AI support from <b>YOLO</b> and <b>Segment Anything</b>!<p>
   <p align="center"><b>AnyLabeling = LabelImg + Labelme + Improved UI + Auto-labeling</b><p>
 </p>
 
 ![](https://i.imgur.com/waxVImv.png)
 
 [![PyPI](https://img.shields.io/pypi/v/anylabeling)](https://pypi.org/project/anylabeling)
 [![license](https://img.shields.io/github/license/vietanhdev/anylabeling.svg)](https://github.com/vietanhdev/anylabeling/blob/master/LICENSE)
 [![open issues](https://isitmaintained.com/badge/open/vietanhdev/anylabeling.svg)](https://github.com/vietanhdev/anylabeling/issues)
 [![Pypi Downloads](https://pepy.tech/badge/anylabeling)](https://pypi.org/project/anylabeling/)
 
 <a href="https://www.youtube.com/watch?v=5iQSGL7ebXE">
-  <img alt="AnyLabeling" src="https://user-images.githubusercontent.com/18329471/231320488-2f8133bc-6b51-48f8-82a6-dd3b267f5156.png"/>
+  <img alt="AnyLabeling" src="https://user-images.githubusercontent.com/18329471/232266520-1f52cd45-0776-479e-8a3c-4fef144c6b73.png"/>
 </a>
 
-**Youtube Demo:** [https://www.youtube.com/watch?v=5iQSGL7ebXE](https://www.youtube.com/watch?v=5iQSGL7ebXE)
+- **Youtube Demo:** [https://www.youtube.com/watch?v=5iQSGL7ebXE](https://www.youtube.com/watch?v=5iQSGL7ebXE)
+- **Documentation:** [https://anylabeling.com](https://anylabeling.com)
 
 ## I. Install and run
 
 - Requirements: Python >= 3.8
 - Recommended: Miniconda/Anaconda <https://docs.conda.io/en/latest/miniconda.html>
 
 - Create environment:
```

#### html2text {}

```diff
@@ -1,32 +1,32 @@
-Metadata-Version: 2.1 Name: anylabeling Version: 0.2.4 Summary: Effortless data
+Metadata-Version: 2.1 Name: anylabeling Version: 0.2.6 Summary: Effortless data
 labeling with AI support Home-page: https://github.com/vietanhdev/anylabeling
 Author: Viet-Anh Nguyen Author-email: vietanh.dev@gmail.com License: GPLv3
 Keywords: Image Annotation,Machine Learning,Deep Learning Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3 :: Only Description-Content-Type: text/markdown
 License-File: LICENSE
- [https://user-images.githubusercontent.com/18329471/232231236-6d6a1a79-22c9-
-                          4cbc-9132-c81cbc201265.png]
+                                 [AnyLabeling]
                       ****** ð AnyLabeling ð ******
    Effortless data labeling with AI support from YOLO and Segment Anything!
         AnyLabeling = LabelImg + Labelme + Improved UI + Auto-labeling
 ![](https://i.imgur.com/waxVImv.png) [![PyPI](https://img.shields.io/pypi/v/
 anylabeling)](https://pypi.org/project/anylabeling) [![license](https://
 img.shields.io/github/license/vietanhdev/anylabeling.svg)](https://github.com/
 vietanhdev/anylabeling/blob/master/LICENSE) [![open issues](https://
 isitmaintained.com/badge/open/vietanhdev/anylabeling.svg)](https://github.com/
 vietanhdev/anylabeling/issues) [![Pypi Downloads](https://pepy.tech/badge/
-anylabeling)](https://pypi.org/project/anylabeling/) [AnyLabeling] **Youtube
+anylabeling)](https://pypi.org/project/anylabeling/) [AnyLabeling] - **Youtube
 Demo:** [https://www.youtube.com/watch?v=5iQSGL7ebXE](https://www.youtube.com/
-watch?v=5iQSGL7ebXE) ## I. Install and run - Requirements: Python >= 3.8 -
+watch?v=5iQSGL7ebXE) - **Documentation:** [https://anylabeling.com](https://
+anylabeling.com) ## I. Install and run - Requirements: Python >= 3.8 -
 Recommended: Miniconda/Anaconda
 docs.conda.io/en/latest/miniconda.html> - Create environment: ```bash conda
 create -n anylabeling python=3.8 conda activate anylabeling ``` - **(For macOS
 only)** Install PyQt5 using Conda: ```bash conda install -c conda-forge
 pyqt==5.15.7 ``` - Install anylabeling: ```bash pip install anylabeling ``` -
 Run app: ```bash anylabeling ``` Or ```bash python -m anylabeling.app ``` ##
 II. Development - Generate resources: ```bash pyrcc5 -o anylabeling/resources/
```

### Comparing `anylabeling-0.2.4/README.md` & `anylabeling-0.2.6/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 <p align="center">
-  <img style="width: 150px; max-width: 100%; height: auto; border-radius: 20px; overflow: hidden;" src="https://user-images.githubusercontent.com/18329471/232231236-6d6a1a79-22c9-4cbc-9132-c81cbc201265.png"/>
+  <img alt="AnyLabeling" style="width: 128px; max-width: 100%; height: auto;" src="https://user-images.githubusercontent.com/18329471/232250539-2b15b9ee-5593-41d0-ba22-e0442f314cce.png"/>
   <h1 align="center">🌟 AnyLabeling 🌟</h1>
   <p align="center">Effortless data labeling with AI support from <b>YOLO</b> and <b>Segment Anything</b>!<p>
   <p align="center"><b>AnyLabeling = LabelImg + Labelme + Improved UI + Auto-labeling</b><p>
 </p>
 
 ![](https://i.imgur.com/waxVImv.png)
 
 [![PyPI](https://img.shields.io/pypi/v/anylabeling)](https://pypi.org/project/anylabeling)
 [![license](https://img.shields.io/github/license/vietanhdev/anylabeling.svg)](https://github.com/vietanhdev/anylabeling/blob/master/LICENSE)
 [![open issues](https://isitmaintained.com/badge/open/vietanhdev/anylabeling.svg)](https://github.com/vietanhdev/anylabeling/issues)
 [![Pypi Downloads](https://pepy.tech/badge/anylabeling)](https://pypi.org/project/anylabeling/)
 
 <a href="https://www.youtube.com/watch?v=5iQSGL7ebXE">
-  <img alt="AnyLabeling" src="https://user-images.githubusercontent.com/18329471/231320488-2f8133bc-6b51-48f8-82a6-dd3b267f5156.png"/>
+  <img alt="AnyLabeling" src="https://user-images.githubusercontent.com/18329471/232266520-1f52cd45-0776-479e-8a3c-4fef144c6b73.png"/>
 </a>
 
-**Youtube Demo:** [https://www.youtube.com/watch?v=5iQSGL7ebXE](https://www.youtube.com/watch?v=5iQSGL7ebXE)
+- **Youtube Demo:** [https://www.youtube.com/watch?v=5iQSGL7ebXE](https://www.youtube.com/watch?v=5iQSGL7ebXE)
+- **Documentation:** [https://anylabeling.com](https://anylabeling.com)
 
 ## I. Install and run
 
 - Requirements: Python >= 3.8
 - Recommended: Miniconda/Anaconda <https://docs.conda.io/en/latest/miniconda.html>
 
 - Create environment:
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
- [https://user-images.githubusercontent.com/18329471/232231236-6d6a1a79-22c9-
-                          4cbc-9132-c81cbc201265.png]
+                                 [AnyLabeling]
                       ****** ð AnyLabeling ð ******
    Effortless data labeling with AI support from YOLO and Segment Anything!
         AnyLabeling = LabelImg + Labelme + Improved UI + Auto-labeling
 ![](https://i.imgur.com/waxVImv.png) [![PyPI](https://img.shields.io/pypi/v/
 anylabeling)](https://pypi.org/project/anylabeling) [![license](https://
 img.shields.io/github/license/vietanhdev/anylabeling.svg)](https://github.com/
 vietanhdev/anylabeling/blob/master/LICENSE) [![open issues](https://
 isitmaintained.com/badge/open/vietanhdev/anylabeling.svg)](https://github.com/
 vietanhdev/anylabeling/issues) [![Pypi Downloads](https://pepy.tech/badge/
-anylabeling)](https://pypi.org/project/anylabeling/) [AnyLabeling] **Youtube
+anylabeling)](https://pypi.org/project/anylabeling/) [AnyLabeling] - **Youtube
 Demo:** [https://www.youtube.com/watch?v=5iQSGL7ebXE](https://www.youtube.com/
-watch?v=5iQSGL7ebXE) ## I. Install and run - Requirements: Python >= 3.8 -
+watch?v=5iQSGL7ebXE) - **Documentation:** [https://anylabeling.com](https://
+anylabeling.com) ## I. Install and run - Requirements: Python >= 3.8 -
 Recommended: Miniconda/Anaconda
 docs.conda.io/en/latest/miniconda.html> - Create environment: ```bash conda
 create -n anylabeling python=3.8 conda activate anylabeling ``` - **(For macOS
 only)** Install PyQt5 using Conda: ```bash conda install -c conda-forge
 pyqt==5.15.7 ``` - Install anylabeling: ```bash pip install anylabeling ``` -
 Run app: ```bash anylabeling ``` Or ```bash python -m anylabeling.app ``` ##
 II. Development - Generate resources: ```bash pyrcc5 -o anylabeling/resources/
```

### Comparing `anylabeling-0.2.4/anylabeling/app.py` & `anylabeling-0.2.6/anylabeling/app.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/configs/anylabeling_config.yaml` & `anylabeling-0.2.6/anylabeling/configs/anylabeling_config.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/configs/auto_labeling/models.yaml` & `anylabeling-0.2.6/anylabeling/configs/auto_labeling/models.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/configs/auto_labeling/yolov5l.yaml` & `anylabeling-0.2.6/anylabeling/configs/auto_labeling/yolov5l.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/configs/auto_labeling/yolov5m.yaml` & `anylabeling-0.2.6/anylabeling/configs/auto_labeling/yolov5m.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/configs/auto_labeling/yolov5n.yaml` & `anylabeling-0.2.6/anylabeling/configs/auto_labeling/yolov5n.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/configs/auto_labeling/yolov5s.yaml` & `anylabeling-0.2.6/anylabeling/configs/auto_labeling/yolov5s.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/configs/auto_labeling/yolov5x.yaml` & `anylabeling-0.2.6/anylabeling/configs/auto_labeling/yolov5x.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/configs/auto_labeling/yolov8l.yaml` & `anylabeling-0.2.6/anylabeling/configs/auto_labeling/yolov8l.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/configs/auto_labeling/yolov8m.yaml` & `anylabeling-0.2.6/anylabeling/configs/auto_labeling/yolov8m.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/configs/auto_labeling/yolov8n.yaml` & `anylabeling-0.2.6/anylabeling/configs/auto_labeling/yolov8n.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/configs/auto_labeling/yolov8s.yaml` & `anylabeling-0.2.6/anylabeling/configs/auto_labeling/yolov8s.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/configs/auto_labeling/yolov8x.yaml` & `anylabeling-0.2.6/anylabeling/configs/auto_labeling/yolov8x.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/resources/resources.py` & `anylabeling-0.2.6/anylabeling/resources/resources.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/services/auto_labeling/lru_cache.py` & `anylabeling-0.2.6/anylabeling/services/auto_labeling/lru_cache.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/services/auto_labeling/model.py` & `anylabeling-0.2.6/anylabeling/services/auto_labeling/model.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/services/auto_labeling/model_manager.py` & `anylabeling-0.2.6/anylabeling/services/auto_labeling/model_manager.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/services/auto_labeling/segment_anything.py` & `anylabeling-0.2.6/anylabeling/services/auto_labeling/segment_anything.py`

 * *Files 7% similar despite different names*

```diff
@@ -221,26 +221,42 @@
         masks = masks.reshape(self.size_after_apply_max_width_height)
         return masks
 
     def post_process(self, masks, resized_ratio):
         """
         Post process masks
         """
-        shapes = []
         # Find contours
         contours, _ = cv2.findContours(
             masks.astype(np.uint8), cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_NONE
         )
+
+        # Refine contours
+        approx_contours = []
         for contour in contours:
             # Approximate contour
             epsilon = 0.001 * cv2.arcLength(contour, True)
             approx = cv2.approxPolyDP(contour, epsilon, True)
-            points = approx.reshape(-1, 2)
+            approx_contours.append(approx)
 
+        # Remove small contours (area < 20% of average area)
+        if len(approx_contours) > 1:
+            areas = [cv2.contourArea(contour) for contour in approx_contours]
+            avg_area = np.mean(areas)
+            approx_contours = [
+                contour
+                for contour, area in zip(approx_contours, areas, strict=False)
+                if area > avg_area * 0.2
+            ]
+
+        # Contours to shapes
+        shapes = []
+        for approx in approx_contours:
             # Scale points
+            points = approx.reshape(-1, 2)
             points[:, 0] = points[:, 0] / resized_ratio[0]
             points[:, 1] = points[:, 1] / resized_ratio[1]
             points = points.tolist()
             if len(points) < 3:
                 continue
             points.append(points[0])
```

### Comparing `anylabeling-0.2.4/anylabeling/services/auto_labeling/types.py` & `anylabeling-0.2.6/anylabeling/services/auto_labeling/types.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/services/auto_labeling/yolov5.py` & `anylabeling-0.2.6/anylabeling/services/auto_labeling/yolov5.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/services/auto_labeling/yolov8.py` & `anylabeling-0.2.6/anylabeling/services/auto_labeling/yolov8.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/common/toaster.py` & `anylabeling-0.2.6/anylabeling/views/common/toaster.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/__main__.py` & `anylabeling-0.2.6/anylabeling/views/labeling/__main__.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/config.py` & `anylabeling-0.2.6/anylabeling/views/labeling/config.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/icons/brain.png` & `anylabeling-0.2.6/anylabeling/views/labeling/icons/brain.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/icons/cancel.png` & `anylabeling-0.2.6/anylabeling/views/labeling/icons/cancel.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/icons/cartesian.png` & `anylabeling-0.2.6/anylabeling/views/labeling/icons/cartesian.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/icons/circle.png` & `anylabeling-0.2.6/anylabeling/views/labeling/icons/circle.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/icons/color-line.png` & `anylabeling-0.2.6/anylabeling/views/labeling/icons/color-line.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/icons/color.png` & `anylabeling-0.2.6/anylabeling/views/labeling/icons/color.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/icons/color_line.png` & `anylabeling-0.2.6/anylabeling/views/labeling/icons/color_line.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/icons/copy.png` & `anylabeling-0.2.6/anylabeling/views/labeling/icons/copy.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/icons/delete.png` & `anylabeling-0.2.6/anylabeling/views/labeling/icons/delete.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/icons/done.png` & `anylabeling-0.2.6/anylabeling/views/labeling/icons/done.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/icons/done.svg` & `anylabeling-0.2.6/anylabeling/views/labeling/icons/done.svg`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/icons/edit.png` & `anylabeling-0.2.6/anylabeling/views/labeling/icons/edit.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/icons/expert.png` & `anylabeling-0.2.6/anylabeling/views/labeling/icons/expert.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/icons/eye.png` & `anylabeling-0.2.6/anylabeling/views/labeling/icons/eye.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/icons/feBlend-icon.png` & `anylabeling-0.2.6/anylabeling/views/labeling/icons/feBlend-icon.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/icons/file.png` & `anylabeling-0.2.6/anylabeling/views/labeling/icons/file.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/icons/fit-width.png` & `anylabeling-0.2.6/anylabeling/views/labeling/icons/fit-width.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/icons/fit-window.png` & `anylabeling-0.2.6/anylabeling/views/labeling/icons/fit-window.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/icons/fit.png` & `anylabeling-0.2.6/anylabeling/views/labeling/icons/fit.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/icons/format_createml.png` & `anylabeling-0.2.6/anylabeling/views/labeling/icons/format_createml.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/icons/format_voc.png` & `anylabeling-0.2.6/anylabeling/views/labeling/icons/format_voc.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/icons/format_yolo.png` & `anylabeling-0.2.6/anylabeling/views/labeling/icons/format_yolo.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/icons/help.png` & `anylabeling-0.2.6/anylabeling/views/labeling/icons/help.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/icons/icon.png` & `anylabeling-0.2.6/anylabeling/views/labeling/icons/icon.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/icons/labels.png` & `anylabeling-0.2.6/anylabeling/views/labeling/icons/labels.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/icons/labels.svg` & `anylabeling-0.2.6/anylabeling/views/labeling/icons/labels.svg`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/icons/line-strip.png` & `anylabeling-0.2.6/anylabeling/views/labeling/icons/line-strip.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/icons/line.png` & `anylabeling-0.2.6/anylabeling/views/labeling/icons/line.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/icons/new.png` & `anylabeling-0.2.6/anylabeling/views/labeling/icons/new.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/icons/next.png` & `anylabeling-0.2.6/anylabeling/views/labeling/icons/next.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/icons/objects.png` & `anylabeling-0.2.6/anylabeling/views/labeling/icons/objects.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/icons/open.png` & `anylabeling-0.2.6/anylabeling/views/labeling/icons/open.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/icons/paste.png` & `anylabeling-0.2.6/anylabeling/views/labeling/icons/paste.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/icons/point.png` & `anylabeling-0.2.6/anylabeling/views/labeling/icons/point.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/icons/polygon.png` & `anylabeling-0.2.6/anylabeling/views/labeling/icons/polygon.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/icons/prev.png` & `anylabeling-0.2.6/anylabeling/views/labeling/icons/prev.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/icons/quit.png` & `anylabeling-0.2.6/anylabeling/views/labeling/icons/quit.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/icons/rectangle.png` & `anylabeling-0.2.6/anylabeling/views/labeling/icons/rectangle.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/icons/resetall.png` & `anylabeling-0.2.6/anylabeling/views/labeling/icons/resetall.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/icons/save-as.png` & `anylabeling-0.2.6/anylabeling/views/labeling/icons/save-as.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/icons/save.png` & `anylabeling-0.2.6/anylabeling/views/labeling/icons/save.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/icons/undo-cross.png` & `anylabeling-0.2.6/anylabeling/views/labeling/icons/undo-cross.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/icons/undo.png` & `anylabeling-0.2.6/anylabeling/views/labeling/icons/undo.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/icons/upload_brain.png` & `anylabeling-0.2.6/anylabeling/views/labeling/icons/upload_brain.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/icons/verify.png` & `anylabeling-0.2.6/anylabeling/views/labeling/icons/verify.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/icons/zoom-in.png` & `anylabeling-0.2.6/anylabeling/views/labeling/icons/zoom-in.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/icons/zoom-out.png` & `anylabeling-0.2.6/anylabeling/views/labeling/icons/zoom-out.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/icons/zoom.png` & `anylabeling-0.2.6/anylabeling/views/labeling/icons/zoom.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/label_file.py` & `anylabeling-0.2.6/anylabeling/views/labeling/label_file.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/label_widget.py` & `anylabeling-0.2.6/anylabeling/views/labeling/label_widget.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/label_wrapper.py` & `anylabeling-0.2.6/anylabeling/views/labeling/label_wrapper.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/logger.py` & `anylabeling-0.2.6/anylabeling/views/labeling/logger.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/shape.py` & `anylabeling-0.2.6/anylabeling/views/labeling/shape.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,16 +36,16 @@
     line_color = DEFAULT_LINE_COLOR
     fill_color = DEFAULT_FILL_COLOR
     select_line_color = DEFAULT_SELECT_LINE_COLOR
     select_fill_color = DEFAULT_SELECT_FILL_COLOR
     vertex_fill_color = DEFAULT_VERTEX_FILL_COLOR
     hvertex_fill_color = DEFAULT_HVERTEX_FILL_COLOR
     point_type = P_ROUND
-    point_size = 8
-    scale = 1.0
+    point_size = 4
+    scale = 1.5
 
     def __init__(
         self,
         label=None,
         text="",
         line_color=None,
         shape_type=None,
@@ -141,15 +141,15 @@
 
     def get_rect_from_line(self, pt1, pt2):
         """Get rectangle from diagonal line"""
         x1, y1 = pt1.x(), pt1.y()
         x2, y2 = pt2.x(), pt2.y()
         return QtCore.QRectF(x1, y1, x2 - x1, y2 - y1)
 
-    def paint(self, painter: QtGui.QPainter):
+    def paint(self, painter: QtGui.QPainter):  # noqa: max-complexity: 18
         """Paint shape using QPainter"""
         if self.points:
             color = (
                 self.select_line_color if self.selected else self.line_color
             )
             pen = QtGui.QPen(color)
             # Try using integer sizes for smoother drawing(?)
@@ -160,44 +160,52 @@
             vrtx_path = QtGui.QPainterPath()
 
             if self.shape_type == "rectangle":
                 assert len(self.points) in [1, 2]
                 if len(self.points) == 2:
                     rectangle = self.get_rect_from_line(*self.points)
                     line_path.addRect(rectangle)
-                for i in range(len(self.points)):
-                    self.draw_vertex(vrtx_path, i)
+                if self.selected:
+                    for i in range(len(self.points)):
+                        self.draw_vertex(vrtx_path, i)
             elif self.shape_type == "circle":
                 assert len(self.points) in [1, 2]
                 if len(self.points) == 2:
                     rectangle = self.get_circle_rect_from_line(self.points)
                     line_path.addEllipse(rectangle)
-                for i in range(len(self.points)):
-                    self.draw_vertex(vrtx_path, i)
+                if self.selected:
+                    for i in range(len(self.points)):
+                        self.draw_vertex(vrtx_path, i)
             elif self.shape_type == "linestrip":
                 line_path.moveTo(self.points[0])
                 for i, p in enumerate(self.points):
                     line_path.lineTo(p)
-                    self.draw_vertex(vrtx_path, i)
+                    if self.selected:
+                        self.draw_vertex(vrtx_path, i)
+            elif self.shape_type == "point":
+                assert len(self.points) == 1
+                self.draw_vertex(vrtx_path, 0)
             else:
                 line_path.moveTo(self.points[0])
                 # Uncommenting the following line will draw 2 paths
                 # for the 1st vertex, and make it non-filled, which
                 # may be desirable.
-                # self.draw_vertex(vrtx_path, 0)
+                self.draw_vertex(vrtx_path, 0)
 
                 for i, p in enumerate(self.points):
                     line_path.lineTo(p)
-                    self.draw_vertex(vrtx_path, i)
+                    if self.selected:
+                        self.draw_vertex(vrtx_path, i)
                 if self.is_closed():
                     line_path.lineTo(self.points[0])
 
             painter.drawPath(line_path)
             painter.drawPath(vrtx_path)
-            painter.fillPath(vrtx_path, self._vertex_fill_color)
+            if self._vertex_fill_color is not None:
+                painter.fillPath(vrtx_path, self._vertex_fill_color)
             if self.fill:
                 color = (
                     self.select_fill_color
                     if self.selected
                     else self.fill_color
                 )
                 painter.fillPath(line_path, color)
```

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/testing.py` & `anylabeling-0.2.6/anylabeling/views/labeling/testing.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/utils/__init__.py` & `anylabeling-0.2.6/anylabeling/views/labeling/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/utils/_io.py` & `anylabeling-0.2.6/anylabeling/views/labeling/utils/_io.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/utils/image.py` & `anylabeling-0.2.6/anylabeling/views/labeling/utils/image.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/utils/qt.py` & `anylabeling-0.2.6/anylabeling/views/labeling/utils/qt.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/utils/shape.py` & `anylabeling-0.2.6/anylabeling/views/labeling/utils/shape.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py` & `anylabeling-0.2.6/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui` & `anylabeling-0.2.6/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py` & `anylabeling-0.2.6/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/widgets/canvas.py` & `anylabeling-0.2.6/anylabeling/views/labeling/widgets/canvas.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/widgets/color_dialog.py` & `anylabeling-0.2.6/anylabeling/views/labeling/widgets/color_dialog.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/widgets/file_dialog_preview.py` & `anylabeling-0.2.6/anylabeling/views/labeling/widgets/file_dialog_preview.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/widgets/label_dialog.py` & `anylabeling-0.2.6/anylabeling/views/labeling/widgets/label_dialog.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/widgets/label_list_widget.py` & `anylabeling-0.2.6/anylabeling/views/labeling/widgets/label_list_widget.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/widgets/toolbar.py` & `anylabeling-0.2.6/anylabeling/views/labeling/widgets/toolbar.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py` & `anylabeling-0.2.6/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/labeling/widgets/zoom_widget.py` & `anylabeling-0.2.6/anylabeling/views/labeling/widgets/zoom_widget.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling/views/mainwindow.py` & `anylabeling-0.2.6/anylabeling/views/mainwindow.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/anylabeling.egg-info/PKG-INFO` & `anylabeling-0.2.6/anylabeling.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anylabeling
-Version: 0.2.4
+Version: 0.2.6
 Summary: Effortless data labeling with AI support
 Home-page: https://github.com/vietanhdev/anylabeling
 Author: Viet-Anh Nguyen
 Author-email: vietanh.dev@gmail.com
 License: GPLv3
 Keywords: Image Annotation,Machine Learning,Deep Learning
 Classifier: Intended Audience :: Developers
@@ -16,32 +16,33 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
-  <img style="width: 150px; max-width: 100%; height: auto; border-radius: 20px; overflow: hidden;" src="https://user-images.githubusercontent.com/18329471/232231236-6d6a1a79-22c9-4cbc-9132-c81cbc201265.png"/>
+  <img alt="AnyLabeling" style="width: 128px; max-width: 100%; height: auto;" src="https://user-images.githubusercontent.com/18329471/232250539-2b15b9ee-5593-41d0-ba22-e0442f314cce.png"/>
   <h1 align="center">🌟 AnyLabeling 🌟</h1>
   <p align="center">Effortless data labeling with AI support from <b>YOLO</b> and <b>Segment Anything</b>!<p>
   <p align="center"><b>AnyLabeling = LabelImg + Labelme + Improved UI + Auto-labeling</b><p>
 </p>
 
 ![](https://i.imgur.com/waxVImv.png)
 
 [![PyPI](https://img.shields.io/pypi/v/anylabeling)](https://pypi.org/project/anylabeling)
 [![license](https://img.shields.io/github/license/vietanhdev/anylabeling.svg)](https://github.com/vietanhdev/anylabeling/blob/master/LICENSE)
 [![open issues](https://isitmaintained.com/badge/open/vietanhdev/anylabeling.svg)](https://github.com/vietanhdev/anylabeling/issues)
 [![Pypi Downloads](https://pepy.tech/badge/anylabeling)](https://pypi.org/project/anylabeling/)
 
 <a href="https://www.youtube.com/watch?v=5iQSGL7ebXE">
-  <img alt="AnyLabeling" src="https://user-images.githubusercontent.com/18329471/231320488-2f8133bc-6b51-48f8-82a6-dd3b267f5156.png"/>
+  <img alt="AnyLabeling" src="https://user-images.githubusercontent.com/18329471/232266520-1f52cd45-0776-479e-8a3c-4fef144c6b73.png"/>
 </a>
 
-**Youtube Demo:** [https://www.youtube.com/watch?v=5iQSGL7ebXE](https://www.youtube.com/watch?v=5iQSGL7ebXE)
+- **Youtube Demo:** [https://www.youtube.com/watch?v=5iQSGL7ebXE](https://www.youtube.com/watch?v=5iQSGL7ebXE)
+- **Documentation:** [https://anylabeling.com](https://anylabeling.com)
 
 ## I. Install and run
 
 - Requirements: Python >= 3.8
 - Recommended: Miniconda/Anaconda <https://docs.conda.io/en/latest/miniconda.html>
 
 - Create environment:
```

#### html2text {}

```diff
@@ -1,32 +1,32 @@
-Metadata-Version: 2.1 Name: anylabeling Version: 0.2.4 Summary: Effortless data
+Metadata-Version: 2.1 Name: anylabeling Version: 0.2.6 Summary: Effortless data
 labeling with AI support Home-page: https://github.com/vietanhdev/anylabeling
 Author: Viet-Anh Nguyen Author-email: vietanh.dev@gmail.com License: GPLv3
 Keywords: Image Annotation,Machine Learning,Deep Learning Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3 :: Only Description-Content-Type: text/markdown
 License-File: LICENSE
- [https://user-images.githubusercontent.com/18329471/232231236-6d6a1a79-22c9-
-                          4cbc-9132-c81cbc201265.png]
+                                 [AnyLabeling]
                       ****** ð AnyLabeling ð ******
    Effortless data labeling with AI support from YOLO and Segment Anything!
         AnyLabeling = LabelImg + Labelme + Improved UI + Auto-labeling
 ![](https://i.imgur.com/waxVImv.png) [![PyPI](https://img.shields.io/pypi/v/
 anylabeling)](https://pypi.org/project/anylabeling) [![license](https://
 img.shields.io/github/license/vietanhdev/anylabeling.svg)](https://github.com/
 vietanhdev/anylabeling/blob/master/LICENSE) [![open issues](https://
 isitmaintained.com/badge/open/vietanhdev/anylabeling.svg)](https://github.com/
 vietanhdev/anylabeling/issues) [![Pypi Downloads](https://pepy.tech/badge/
-anylabeling)](https://pypi.org/project/anylabeling/) [AnyLabeling] **Youtube
+anylabeling)](https://pypi.org/project/anylabeling/) [AnyLabeling] - **Youtube
 Demo:** [https://www.youtube.com/watch?v=5iQSGL7ebXE](https://www.youtube.com/
-watch?v=5iQSGL7ebXE) ## I. Install and run - Requirements: Python >= 3.8 -
+watch?v=5iQSGL7ebXE) - **Documentation:** [https://anylabeling.com](https://
+anylabeling.com) ## I. Install and run - Requirements: Python >= 3.8 -
 Recommended: Miniconda/Anaconda
 docs.conda.io/en/latest/miniconda.html> - Create environment: ```bash conda
 create -n anylabeling python=3.8 conda activate anylabeling ``` - **(For macOS
 only)** Install PyQt5 using Conda: ```bash conda install -c conda-forge
 pyqt==5.15.7 ``` - Install anylabeling: ```bash pip install anylabeling ``` -
 Run app: ```bash anylabeling ``` Or ```bash python -m anylabeling.app ``` ##
 II. Development - Generate resources: ```bash pyrcc5 -o anylabeling/resources/
```

### Comparing `anylabeling-0.2.4/anylabeling.egg-info/SOURCES.txt` & `anylabeling-0.2.6/anylabeling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anylabeling-0.2.4/setup.py` & `anylabeling-0.2.6/setup.py`

 * *Files identical despite different names*

