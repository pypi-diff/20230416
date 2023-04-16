# Comparing `tmp/comic-ocr-0.1.3.tar.gz` & `tmp/comic-ocr-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comic-ocr-0.1.3.tar", max compression
+gzip compressed data, was "comic-ocr-0.1.4.tar", max compression
```

## Comparing `comic-ocr-0.1.3.tar` & `comic-ocr-0.1.4.tar`

### file list

```diff
@@ -1,42 +1,43 @@
--rw-r--r--   0        0        0     3038 2023-04-16 04:30:38.174028 comic-ocr-0.1.3/comic_ocr/__init__.py
--rw-r--r--   0        0        0        1 2021-11-07 02:37:21.177983 comic-ocr-0.1.3/comic_ocr/dataset/__init__.py
--rw-r--r--   0        0        0     1747 2023-01-01 08:02:03.597718 comic-ocr-0.1.3/comic_ocr/dataset/annotated_manga/__init__.py
--rw-r--r--   0        0        0     3294 2023-01-01 08:02:52.545238 comic-ocr-0.1.3/comic_ocr/dataset/generated_manga/__init__.py
--rw-r--r--   0        0        0     8056 2023-01-01 08:02:52.542738 comic-ocr-0.1.3/comic_ocr/dataset/generated_manga/generator.py
--rw-r--r--   0        0        0     4651 2023-01-01 07:58:33.181579 comic-ocr-0.1.3/comic_ocr/dataset/generated_manga/text_area.py
--rw-r--r--   0        0        0     1294 2023-01-01 08:02:52.548416 comic-ocr-0.1.3/comic_ocr/dataset/generated_manga/text_bubble.py
--rw-r--r--   0        0        0      754 2023-01-01 08:02:52.546791 comic-ocr-0.1.3/comic_ocr/dataset/generated_manga/text_rect.py
--rw-r--r--   0        0        0     1778 2023-04-16 04:35:19.910087 comic-ocr-0.1.3/comic_ocr/hub.py
--rw-r--r--   0        0        0        0 2021-11-05 12:29:52.065055 comic-ocr-0.1.3/comic_ocr/models/__init__.py
--rw-r--r--   0        0        0     4029 2023-04-16 04:30:38.174750 comic-ocr-0.1.3/comic_ocr/models/localization/__init__.py
--rw-r--r--   0        0        0        0 2021-11-07 03:56:47.882076 comic-ocr-0.1.3/comic_ocr/models/localization/conv_unet/__init__.py
--rw-r--r--   0        0        0     4438 2023-04-16 04:10:55.053923 comic-ocr-0.1.3/comic_ocr/models/localization/conv_unet/conv_fpn.py
--rw-r--r--   0        0        0     8794 2023-04-16 04:10:55.055376 comic-ocr-0.1.3/comic_ocr/models/localization/conv_unet/conv_unet.py
--rw-r--r--   0        0        0    13523 2023-02-24 10:17:27.921715 comic-ocr-0.1.3/comic_ocr/models/localization/localization_dataset.py
--rw-r--r--   0        0        0     6173 2023-04-16 04:10:55.056061 comic-ocr-0.1.3/comic_ocr/models/localization/localization_model.py
--rw-r--r--   0        0        0     5543 2023-02-26 04:02:13.567390 comic-ocr-0.1.3/comic_ocr/models/localization/localization_open_cv.py
--rw-r--r--   0        0        0     3200 2023-01-01 07:58:33.170198 comic-ocr-0.1.3/comic_ocr/models/localization/localization_utils.py
--rw-r--r--   0        0        0     8440 2023-03-11 16:23:23.086590 comic-ocr-0.1.3/comic_ocr/models/localization/train.py
--rw-r--r--   0        0        0     2384 2023-04-16 04:30:38.175013 comic-ocr-0.1.3/comic_ocr/models/recognition/__init__.py
--rw-r--r--   0        0        0        0 2022-04-04 06:56:58.048152 comic-ocr-0.1.3/comic_ocr/models/recognition/crnn/__init__.py
--rw-r--r--   0        0        0     4100 2023-03-11 10:25:30.942269 comic-ocr-0.1.3/comic_ocr/models/recognition/crnn/crnn.py
--rw-r--r--   0        0        0     1237 2022-07-31 06:31:35.098130 comic-ocr-0.1.3/comic_ocr/models/recognition/encoding.py
--rw-r--r--   0        0        0     7346 2023-01-01 08:02:52.535328 comic-ocr-0.1.3/comic_ocr/models/recognition/recognition_dataset.py
--rw-r--r--   0        0        0     7795 2022-11-05 03:31:22.717422 comic-ocr-0.1.3/comic_ocr/models/recognition/recognition_model.py
--rw-r--r--   0        0        0     5205 2022-11-05 10:59:38.247884 comic-ocr-0.1.3/comic_ocr/models/recognition/train.py
--rw-r--r--   0        0        0        0 2022-10-22 04:11:06.165788 comic-ocr-0.1.3/comic_ocr/models/recognition/trocr/__init__.py
--rw-r--r--   0        0        0     5734 2022-11-05 08:54:11.941496 comic-ocr-0.1.3/comic_ocr/models/recognition/trocr/trocr.py
--rw-r--r--   0        0        0      413 2023-01-01 06:55:13.382652 comic-ocr-0.1.3/comic_ocr/models/transforms.py
--rw-r--r--   0        0        0      231 2023-01-01 07:58:33.212997 comic-ocr-0.1.3/comic_ocr/types/__init__.py
--rw-r--r--   0        0        0       89 2022-07-31 05:40:19.127565 comic-ocr-0.1.3/comic_ocr/types/files.py
--rw-r--r--   0        0        0     1004 2023-01-01 07:58:33.221252 comic-ocr-0.1.3/comic_ocr/types/images.py
--rw-r--r--   0        0        0     1283 2023-01-01 07:58:33.223699 comic-ocr-0.1.3/comic_ocr/types/lines.py
--rw-r--r--   0        0        0     6538 2023-01-01 07:18:24.655782 comic-ocr-0.1.3/comic_ocr/types/shapes.py
--rw-r--r--   0        0        0     2372 2023-01-01 07:58:33.206920 comic-ocr-0.1.3/comic_ocr/utils/__init__.py
--rw-r--r--   0        0        0     2098 2023-01-09 05:25:50.901182 comic-ocr-0.1.3/comic_ocr/utils/files.py
--rw-r--r--   0        0        0     3151 2023-02-26 01:32:13.853604 comic-ocr-0.1.3/comic_ocr/utils/nb_annotation.py
--rw-r--r--   0        0        0     2626 2023-01-01 12:36:49.338062 comic-ocr-0.1.3/comic_ocr/utils/ploting.py
--rw-r--r--   0        0        0      858 2023-02-24 04:18:21.984041 comic-ocr-0.1.3/comic_ocr/utils/pytorch_model.py
--rw-r--r--   0        0        0      614 2023-04-16 04:30:38.175259 comic-ocr-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1103 2023-04-16 04:38:31.546007 comic-ocr-0.1.3/setup.py
--rw-r--r--   0        0        0      684 2023-04-16 04:38:31.546249 comic-ocr-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     3038 2023-04-16 04:30:38.174028 comic-ocr-0.1.4/comic_ocr/__init__.py
+-rw-r--r--   0        0        0        1 2021-11-07 02:37:21.177983 comic-ocr-0.1.4/comic_ocr/dataset/__init__.py
+-rw-r--r--   0        0        0     1747 2023-01-01 08:02:03.597718 comic-ocr-0.1.4/comic_ocr/dataset/annotated_manga/__init__.py
+-rw-r--r--   0        0        0     3294 2023-01-01 08:02:52.545238 comic-ocr-0.1.4/comic_ocr/dataset/generated_manga/__init__.py
+-rw-r--r--   0        0        0     8056 2023-01-01 08:02:52.542738 comic-ocr-0.1.4/comic_ocr/dataset/generated_manga/generator.py
+-rw-r--r--   0        0        0     4651 2023-01-01 07:58:33.181579 comic-ocr-0.1.4/comic_ocr/dataset/generated_manga/text_area.py
+-rw-r--r--   0        0        0     1294 2023-01-01 08:02:52.548416 comic-ocr-0.1.4/comic_ocr/dataset/generated_manga/text_bubble.py
+-rw-r--r--   0        0        0      754 2023-01-01 08:02:52.546791 comic-ocr-0.1.4/comic_ocr/dataset/generated_manga/text_rect.py
+-rw-r--r--   0        0        0     1778 2023-04-16 04:35:19.910087 comic-ocr-0.1.4/comic_ocr/hub.py
+-rw-r--r--   0        0        0        0 2021-11-05 12:29:52.065055 comic-ocr-0.1.4/comic_ocr/models/__init__.py
+-rw-r--r--   0        0        0     4028 2023-04-16 04:45:56.718369 comic-ocr-0.1.4/comic_ocr/models/localization/__init__.py
+-rw-r--r--   0        0        0        0 2021-11-07 03:56:47.882076 comic-ocr-0.1.4/comic_ocr/models/localization/conv_unet/__init__.py
+-rw-r--r--   0        0        0     4438 2023-04-16 04:10:55.053923 comic-ocr-0.1.4/comic_ocr/models/localization/conv_unet/conv_fpn.py
+-rw-r--r--   0        0        0     8794 2023-04-16 04:10:55.055376 comic-ocr-0.1.4/comic_ocr/models/localization/conv_unet/conv_unet.py
+-rw-r--r--   0        0        0    13523 2023-02-24 10:17:27.921715 comic-ocr-0.1.4/comic_ocr/models/localization/localization_dataset.py
+-rw-r--r--   0        0        0     6173 2023-04-16 04:10:55.056061 comic-ocr-0.1.4/comic_ocr/models/localization/localization_model.py
+-rw-r--r--   0        0        0     5543 2023-02-26 04:02:13.567390 comic-ocr-0.1.4/comic_ocr/models/localization/localization_open_cv.py
+-rw-r--r--   0        0        0     3200 2023-01-01 07:58:33.170198 comic-ocr-0.1.4/comic_ocr/models/localization/localization_utils.py
+-rw-r--r--   0        0        0     8440 2023-03-11 16:23:23.086590 comic-ocr-0.1.4/comic_ocr/models/localization/train.py
+-rw-r--r--   0        0        0     2384 2023-04-16 04:30:38.175013 comic-ocr-0.1.4/comic_ocr/models/recognition/__init__.py
+-rw-r--r--   0        0        0        0 2022-04-04 06:56:58.048152 comic-ocr-0.1.4/comic_ocr/models/recognition/crnn/__init__.py
+-rw-r--r--   0        0        0     4100 2023-03-11 10:25:30.942269 comic-ocr-0.1.4/comic_ocr/models/recognition/crnn/crnn.py
+-rw-r--r--   0        0        0     1237 2022-07-31 06:31:35.098130 comic-ocr-0.1.4/comic_ocr/models/recognition/encoding.py
+-rw-r--r--   0        0        0     7346 2023-01-01 08:02:52.535328 comic-ocr-0.1.4/comic_ocr/models/recognition/recognition_dataset.py
+-rw-r--r--   0        0        0     7795 2022-11-05 03:31:22.717422 comic-ocr-0.1.4/comic_ocr/models/recognition/recognition_model.py
+-rw-r--r--   0        0        0     5205 2022-11-05 10:59:38.247884 comic-ocr-0.1.4/comic_ocr/models/recognition/train.py
+-rw-r--r--   0        0        0        0 2022-10-22 04:11:06.165788 comic-ocr-0.1.4/comic_ocr/models/recognition/trocr/__init__.py
+-rw-r--r--   0        0        0     5734 2022-11-05 08:54:11.941496 comic-ocr-0.1.4/comic_ocr/models/recognition/trocr/trocr.py
+-rw-r--r--   0        0        0      413 2023-01-01 06:55:13.382652 comic-ocr-0.1.4/comic_ocr/models/transforms.py
+-rw-r--r--   0        0        0      231 2023-01-01 07:58:33.212997 comic-ocr-0.1.4/comic_ocr/types/__init__.py
+-rw-r--r--   0        0        0       89 2022-07-31 05:40:19.127565 comic-ocr-0.1.4/comic_ocr/types/files.py
+-rw-r--r--   0        0        0     1004 2023-01-01 07:58:33.221252 comic-ocr-0.1.4/comic_ocr/types/images.py
+-rw-r--r--   0        0        0     1283 2023-01-01 07:58:33.223699 comic-ocr-0.1.4/comic_ocr/types/lines.py
+-rw-r--r--   0        0        0     6538 2023-01-01 07:18:24.655782 comic-ocr-0.1.4/comic_ocr/types/shapes.py
+-rw-r--r--   0        0        0     2372 2023-01-01 07:58:33.206920 comic-ocr-0.1.4/comic_ocr/utils/__init__.py
+-rw-r--r--   0        0        0     2098 2023-01-09 05:25:50.901182 comic-ocr-0.1.4/comic_ocr/utils/files.py
+-rw-r--r--   0        0        0     3151 2023-02-26 01:32:13.853604 comic-ocr-0.1.4/comic_ocr/utils/nb_annotation.py
+-rw-r--r--   0        0        0     2626 2023-01-01 12:36:49.338062 comic-ocr-0.1.4/comic_ocr/utils/ploting.py
+-rw-r--r--   0        0        0      858 2023-02-24 04:18:21.984041 comic-ocr-0.1.4/comic_ocr/utils/pytorch_model.py
+-rw-r--r--   0        0        0    67873 2023-01-09 04:49:52.045331 comic-ocr-0.1.4/example/manga_annotated/xkcd_100.jpg
+-rw-r--r--   0        0        0      652 2023-04-16 04:46:21.125386 comic-ocr-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1103 2023-04-16 04:46:45.323697 comic-ocr-0.1.4/setup.py
+-rw-r--r--   0        0        0      684 2023-04-16 04:46:45.323874 comic-ocr-0.1.4/PKG-INFO
```

### Comparing `comic-ocr-0.1.3/comic_ocr/__init__.py` & `comic-ocr-0.1.4/comic_ocr/__init__.py`

 * *Files identical despite different names*

### Comparing `comic-ocr-0.1.3/comic_ocr/dataset/annotated_manga/__init__.py` & `comic-ocr-0.1.4/comic_ocr/dataset/annotated_manga/__init__.py`

 * *Files identical despite different names*

### Comparing `comic-ocr-0.1.3/comic_ocr/dataset/generated_manga/__init__.py` & `comic-ocr-0.1.4/comic_ocr/dataset/generated_manga/__init__.py`

 * *Files identical despite different names*

### Comparing `comic-ocr-0.1.3/comic_ocr/dataset/generated_manga/generator.py` & `comic-ocr-0.1.4/comic_ocr/dataset/generated_manga/generator.py`

 * *Files identical despite different names*

### Comparing `comic-ocr-0.1.3/comic_ocr/dataset/generated_manga/text_area.py` & `comic-ocr-0.1.4/comic_ocr/dataset/generated_manga/text_area.py`

 * *Files identical despite different names*

### Comparing `comic-ocr-0.1.3/comic_ocr/dataset/generated_manga/text_bubble.py` & `comic-ocr-0.1.4/comic_ocr/dataset/generated_manga/text_bubble.py`

 * *Files identical despite different names*

### Comparing `comic-ocr-0.1.3/comic_ocr/dataset/generated_manga/text_rect.py` & `comic-ocr-0.1.4/comic_ocr/dataset/generated_manga/text_rect.py`

 * *Files identical despite different names*

### Comparing `comic-ocr-0.1.3/comic_ocr/hub.py` & `comic-ocr-0.1.4/comic_ocr/hub.py`

 * *Files identical despite different names*

### Comparing `comic-ocr-0.1.3/comic_ocr/models/localization/__init__.py` & `comic-ocr-0.1.4/comic_ocr/models/localization/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from comic_ocr.types import Rectangle
 from comic_ocr.models.localization.localization_model import LocalizationModel, BasicLocalizationModel
 from comic_ocr.models.localization.localization_dataset import LocalizationDataset
 from comic_ocr.utils.files import PathLike, get_path_project_dir, load_image
 
 DEFAULT_LOCAL_TRAINED_MODEL_FILE = get_path_project_dir('trained_models/localization.pth')
-DEFAULT_EXAMPLE_IMAGE = get_path_project_dir('example/manga_annotated/normal_01.jpg')
+DEFAULT_EXAMPLE_IMAGE = get_path_project_dir('example/manga_annotated/xkcd_100.jpg')
 
 logger = logging.getLogger(__name__)
 
 
 def load_or_create_new_model(model_file: PathLike = DEFAULT_LOCAL_TRAINED_MODEL_FILE) -> LocalizationModel:
     try:
         model = load_model(model_file, test_executing_model=True)
```

### Comparing `comic-ocr-0.1.3/comic_ocr/models/localization/conv_unet/conv_fpn.py` & `comic-ocr-0.1.4/comic_ocr/models/localization/conv_unet/conv_fpn.py`

 * *Files identical despite different names*

### Comparing `comic-ocr-0.1.3/comic_ocr/models/localization/conv_unet/conv_unet.py` & `comic-ocr-0.1.4/comic_ocr/models/localization/conv_unet/conv_unet.py`

 * *Files identical despite different names*

### Comparing `comic-ocr-0.1.3/comic_ocr/models/localization/localization_dataset.py` & `comic-ocr-0.1.4/comic_ocr/models/localization/localization_dataset.py`

 * *Files identical despite different names*

### Comparing `comic-ocr-0.1.3/comic_ocr/models/localization/localization_model.py` & `comic-ocr-0.1.4/comic_ocr/models/localization/localization_model.py`

 * *Files identical despite different names*

### Comparing `comic-ocr-0.1.3/comic_ocr/models/localization/localization_open_cv.py` & `comic-ocr-0.1.4/comic_ocr/models/localization/localization_open_cv.py`

 * *Files identical despite different names*

### Comparing `comic-ocr-0.1.3/comic_ocr/models/localization/localization_utils.py` & `comic-ocr-0.1.4/comic_ocr/models/localization/localization_utils.py`

 * *Files identical despite different names*

### Comparing `comic-ocr-0.1.3/comic_ocr/models/localization/train.py` & `comic-ocr-0.1.4/comic_ocr/models/localization/train.py`

 * *Files identical despite different names*

### Comparing `comic-ocr-0.1.3/comic_ocr/models/recognition/__init__.py` & `comic-ocr-0.1.4/comic_ocr/models/recognition/__init__.py`

 * *Files identical despite different names*

### Comparing `comic-ocr-0.1.3/comic_ocr/models/recognition/crnn/crnn.py` & `comic-ocr-0.1.4/comic_ocr/models/recognition/crnn/crnn.py`

 * *Files identical despite different names*

### Comparing `comic-ocr-0.1.3/comic_ocr/models/recognition/encoding.py` & `comic-ocr-0.1.4/comic_ocr/models/recognition/encoding.py`

 * *Files identical despite different names*

### Comparing `comic-ocr-0.1.3/comic_ocr/models/recognition/recognition_dataset.py` & `comic-ocr-0.1.4/comic_ocr/models/recognition/recognition_dataset.py`

 * *Files identical despite different names*

### Comparing `comic-ocr-0.1.3/comic_ocr/models/recognition/recognition_model.py` & `comic-ocr-0.1.4/comic_ocr/models/recognition/recognition_model.py`

 * *Files identical despite different names*

### Comparing `comic-ocr-0.1.3/comic_ocr/models/recognition/train.py` & `comic-ocr-0.1.4/comic_ocr/models/recognition/train.py`

 * *Files identical despite different names*

### Comparing `comic-ocr-0.1.3/comic_ocr/models/recognition/trocr/trocr.py` & `comic-ocr-0.1.4/comic_ocr/models/recognition/trocr/trocr.py`

 * *Files identical despite different names*

### Comparing `comic-ocr-0.1.3/comic_ocr/types/images.py` & `comic-ocr-0.1.4/comic_ocr/types/images.py`

 * *Files identical despite different names*

### Comparing `comic-ocr-0.1.3/comic_ocr/types/lines.py` & `comic-ocr-0.1.4/comic_ocr/types/lines.py`

 * *Files identical despite different names*

### Comparing `comic-ocr-0.1.3/comic_ocr/types/shapes.py` & `comic-ocr-0.1.4/comic_ocr/types/shapes.py`

 * *Files identical despite different names*

### Comparing `comic-ocr-0.1.3/comic_ocr/utils/__init__.py` & `comic-ocr-0.1.4/comic_ocr/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `comic-ocr-0.1.3/comic_ocr/utils/files.py` & `comic-ocr-0.1.4/comic_ocr/utils/files.py`

 * *Files identical despite different names*

### Comparing `comic-ocr-0.1.3/comic_ocr/utils/nb_annotation.py` & `comic-ocr-0.1.4/comic_ocr/utils/nb_annotation.py`

 * *Files identical despite different names*

### Comparing `comic-ocr-0.1.3/comic_ocr/utils/ploting.py` & `comic-ocr-0.1.4/comic_ocr/utils/ploting.py`

 * *Files identical despite different names*

### Comparing `comic-ocr-0.1.3/comic_ocr/utils/pytorch_model.py` & `comic-ocr-0.1.4/comic_ocr/utils/pytorch_model.py`

 * *Files identical despite different names*

### Comparing `comic-ocr-0.1.3/pyproject.toml` & `comic-ocr-0.1.4/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "comic-ocr"
-version = "0.1.3"
+version = "0.1.4"
 description = "An OCR library comic and manga"
 authors = ["Wanasit T"]
 license = "MIT License"
 packages = [
     { include = "comic_ocr" },
 ]
-include = []
+include = ["example/manga_annotated/xkcd_100.jpg"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 torch = "^1.12.1"
 torchvision = "^0.13.1"
 opencv-python = "^4.5.4.60"
 numpy = "^1.21"
```

### Comparing `comic-ocr-0.1.3/setup.py` & `comic-ocr-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
  'torch>=1.12.1,<2.0.0',
  'torchvision>=0.13.1,<0.14.0',
  'tqdm>=4,<5',
  'transformers>=4.23.1,<5.0.0']
 
 setup_kwargs = {
     'name': 'comic-ocr',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': 'An OCR library comic and manga',
     'long_description': None,
     'author': 'Wanasit T',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `comic-ocr-0.1.3/PKG-INFO` & `comic-ocr-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comic-ocr
-Version: 0.1.3
+Version: 0.1.4
 Summary: An OCR library comic and manga
 License: MIT
 Author: Wanasit T
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

