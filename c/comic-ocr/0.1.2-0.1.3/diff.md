# Comparing `tmp/comic-ocr-0.1.2.tar.gz` & `tmp/comic-ocr-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comic-ocr-0.1.2.tar", max compression
+gzip compressed data, was "comic-ocr-0.1.3.tar", max compression
```

## Comparing `comic-ocr-0.1.2.tar` & `comic-ocr-0.1.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     2707 2022-10-02 04:18:53.468891 comic-ocr-0.1.2/comic_ocr/__init__.py
--rw-r--r--   0        0        0        1 2021-11-07 02:37:21.177983 comic-ocr-0.1.2/comic_ocr/dataset/__init__.py
--rw-r--r--   0        0        0     1748 2022-11-06 02:25:38.947785 comic-ocr-0.1.2/comic_ocr/dataset/annotated_manga/__init__.py
--rw-r--r--   0        0        0     3295 2022-07-31 06:28:53.546407 comic-ocr-0.1.2/comic_ocr/dataset/generated_manga/__init__.py
--rw-r--r--   0        0        0     8057 2022-07-31 06:29:09.613989 comic-ocr-0.1.2/comic_ocr/dataset/generated_manga/generator.py
--rw-r--r--   0        0        0     4652 2022-07-31 06:29:09.573684 comic-ocr-0.1.2/comic_ocr/dataset/generated_manga/text_area.py
--rw-r--r--   0        0        0     1295 2022-07-31 06:29:09.616365 comic-ocr-0.1.2/comic_ocr/dataset/generated_manga/text_bubble.py
--rw-r--r--   0        0        0      755 2022-07-31 06:29:09.610916 comic-ocr-0.1.2/comic_ocr/dataset/generated_manga/text_rect.py
--rw-r--r--   0        0        0        0 2021-11-05 12:29:52.065055 comic-ocr-0.1.2/comic_ocr/models/__init__.py
--rw-r--r--   0        0        0     3326 2022-07-31 06:28:54.318348 comic-ocr-0.1.2/comic_ocr/models/localization/__init__.py
--rw-r--r--   0        0        0        0 2021-11-07 03:56:47.882076 comic-ocr-0.1.2/comic_ocr/models/localization/conv_unet/__init__.py
--rw-r--r--   0        0        0     4150 2022-07-16 05:49:35.096975 comic-ocr-0.1.2/comic_ocr/models/localization/conv_unet/conv_unet.py
--rw-r--r--   0        0        0    10696 2022-10-09 04:36:29.515922 comic-ocr-0.1.2/comic_ocr/models/localization/localization_dataset.py
--rw-r--r--   0        0        0     4658 2022-07-31 06:29:09.603478 comic-ocr-0.1.2/comic_ocr/models/localization/localization_model.py
--rw-r--r--   0        0        0     5216 2022-07-31 06:29:09.639284 comic-ocr-0.1.2/comic_ocr/models/localization/localization_open_cv.py
--rw-r--r--   0        0        0     3201 2022-07-31 06:29:09.618774 comic-ocr-0.1.2/comic_ocr/models/localization/localization_utils.py
--rw-r--r--   0        0        0     4735 2022-07-31 06:29:09.593962 comic-ocr-0.1.2/comic_ocr/models/localization/train.py
--rw-r--r--   0        0        0     2366 2022-07-16 05:49:35.047670 comic-ocr-0.1.2/comic_ocr/models/recognition/__init__.py
--rw-r--r--   0        0        0        0 2022-04-04 06:56:58.048152 comic-ocr-0.1.2/comic_ocr/models/recognition/crnn/__init__.py
--rw-r--r--   0        0        0     4099 2022-11-05 09:39:58.270569 comic-ocr-0.1.2/comic_ocr/models/recognition/crnn/crnn.py
--rw-r--r--   0        0        0     1237 2022-07-31 06:31:35.098130 comic-ocr-0.1.2/comic_ocr/models/recognition/encoding.py
--rw-r--r--   0        0        0     7347 2022-11-05 10:53:33.496751 comic-ocr-0.1.2/comic_ocr/models/recognition/recognition_dataset.py
--rw-r--r--   0        0        0     7795 2022-11-05 03:31:22.717422 comic-ocr-0.1.2/comic_ocr/models/recognition/recognition_model.py
--rw-r--r--   0        0        0     5205 2022-11-05 10:59:38.247884 comic-ocr-0.1.2/comic_ocr/models/recognition/train.py
--rw-r--r--   0        0        0        0 2022-10-22 04:11:06.165788 comic-ocr-0.1.2/comic_ocr/models/recognition/trocr/__init__.py
--rw-r--r--   0        0        0     5734 2022-11-05 08:54:11.941496 comic-ocr-0.1.2/comic_ocr/models/recognition/trocr/trocr.py
--rw-r--r--   0        0        0      413 2021-11-07 02:09:58.024786 comic-ocr-0.1.2/comic_ocr/models/transforms.py
--rw-r--r--   0        0        0      235 2022-07-31 06:29:09.586655 comic-ocr-0.1.2/comic_ocr/typing/__init__.py
--rw-r--r--   0        0        0       89 2022-07-31 05:40:19.127565 comic-ocr-0.1.2/comic_ocr/typing/files.py
--rw-r--r--   0        0        0     1005 2022-07-31 06:29:09.631231 comic-ocr-0.1.2/comic_ocr/typing/images.py
--rw-r--r--   0        0        0     1284 2022-07-31 06:29:09.591415 comic-ocr-0.1.2/comic_ocr/typing/lines.py
--rw-r--r--   0        0        0     6538 2022-07-16 05:00:26.134207 comic-ocr-0.1.2/comic_ocr/typing/shapes.py
--rw-r--r--   0        0        0     2373 2022-07-31 06:31:05.944993 comic-ocr-0.1.2/comic_ocr/utils/__init__.py
--rw-r--r--   0        0        0     2046 2022-07-31 07:54:34.654288 comic-ocr-0.1.2/comic_ocr/utils/files.py
--rw-r--r--   0        0        0     3095 2022-07-31 06:29:09.584273 comic-ocr-0.1.2/comic_ocr/utils/nb_annotation.py
--rw-r--r--   0        0        0     2001 2022-04-15 03:05:08.337974 comic-ocr-0.1.2/comic_ocr/utils/ploting.py
--rw-r--r--   0        0        0      858 2022-04-25 08:18:11.103510 comic-ocr-0.1.2/comic_ocr/utils/pytorch_model.py
--rw-r--r--   0        0        0      601 2022-11-06 02:38:57.527542 comic-ocr-0.1.2/pyproject.toml
--rw-r--r--   0        0        0   827323 2022-07-31 09:47:37.500000 comic-ocr-0.1.2/trained_models/localization.bin
--rw-r--r--   0        0        0  1942545 2022-11-05 12:28:49.440047 comic-ocr-0.1.2/trained_models/recognition.bin
--rw-r--r--   0        0        0     1104 2022-11-06 02:39:01.144216 comic-ocr-0.1.2/setup.py
--rw-r--r--   0        0        0      684 2022-11-06 02:39:01.144449 comic-ocr-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     3038 2023-04-16 04:30:38.174028 comic-ocr-0.1.3/comic_ocr/__init__.py
+-rw-r--r--   0        0        0        1 2021-11-07 02:37:21.177983 comic-ocr-0.1.3/comic_ocr/dataset/__init__.py
+-rw-r--r--   0        0        0     1747 2023-01-01 08:02:03.597718 comic-ocr-0.1.3/comic_ocr/dataset/annotated_manga/__init__.py
+-rw-r--r--   0        0        0     3294 2023-01-01 08:02:52.545238 comic-ocr-0.1.3/comic_ocr/dataset/generated_manga/__init__.py
+-rw-r--r--   0        0        0     8056 2023-01-01 08:02:52.542738 comic-ocr-0.1.3/comic_ocr/dataset/generated_manga/generator.py
+-rw-r--r--   0        0        0     4651 2023-01-01 07:58:33.181579 comic-ocr-0.1.3/comic_ocr/dataset/generated_manga/text_area.py
+-rw-r--r--   0        0        0     1294 2023-01-01 08:02:52.548416 comic-ocr-0.1.3/comic_ocr/dataset/generated_manga/text_bubble.py
+-rw-r--r--   0        0        0      754 2023-01-01 08:02:52.546791 comic-ocr-0.1.3/comic_ocr/dataset/generated_manga/text_rect.py
+-rw-r--r--   0        0        0     1778 2023-04-16 04:35:19.910087 comic-ocr-0.1.3/comic_ocr/hub.py
+-rw-r--r--   0        0        0        0 2021-11-05 12:29:52.065055 comic-ocr-0.1.3/comic_ocr/models/__init__.py
+-rw-r--r--   0        0        0     4029 2023-04-16 04:30:38.174750 comic-ocr-0.1.3/comic_ocr/models/localization/__init__.py
+-rw-r--r--   0        0        0        0 2021-11-07 03:56:47.882076 comic-ocr-0.1.3/comic_ocr/models/localization/conv_unet/__init__.py
+-rw-r--r--   0        0        0     4438 2023-04-16 04:10:55.053923 comic-ocr-0.1.3/comic_ocr/models/localization/conv_unet/conv_fpn.py
+-rw-r--r--   0        0        0     8794 2023-04-16 04:10:55.055376 comic-ocr-0.1.3/comic_ocr/models/localization/conv_unet/conv_unet.py
+-rw-r--r--   0        0        0    13523 2023-02-24 10:17:27.921715 comic-ocr-0.1.3/comic_ocr/models/localization/localization_dataset.py
+-rw-r--r--   0        0        0     6173 2023-04-16 04:10:55.056061 comic-ocr-0.1.3/comic_ocr/models/localization/localization_model.py
+-rw-r--r--   0        0        0     5543 2023-02-26 04:02:13.567390 comic-ocr-0.1.3/comic_ocr/models/localization/localization_open_cv.py
+-rw-r--r--   0        0        0     3200 2023-01-01 07:58:33.170198 comic-ocr-0.1.3/comic_ocr/models/localization/localization_utils.py
+-rw-r--r--   0        0        0     8440 2023-03-11 16:23:23.086590 comic-ocr-0.1.3/comic_ocr/models/localization/train.py
+-rw-r--r--   0        0        0     2384 2023-04-16 04:30:38.175013 comic-ocr-0.1.3/comic_ocr/models/recognition/__init__.py
+-rw-r--r--   0        0        0        0 2022-04-04 06:56:58.048152 comic-ocr-0.1.3/comic_ocr/models/recognition/crnn/__init__.py
+-rw-r--r--   0        0        0     4100 2023-03-11 10:25:30.942269 comic-ocr-0.1.3/comic_ocr/models/recognition/crnn/crnn.py
+-rw-r--r--   0        0        0     1237 2022-07-31 06:31:35.098130 comic-ocr-0.1.3/comic_ocr/models/recognition/encoding.py
+-rw-r--r--   0        0        0     7346 2023-01-01 08:02:52.535328 comic-ocr-0.1.3/comic_ocr/models/recognition/recognition_dataset.py
+-rw-r--r--   0        0        0     7795 2022-11-05 03:31:22.717422 comic-ocr-0.1.3/comic_ocr/models/recognition/recognition_model.py
+-rw-r--r--   0        0        0     5205 2022-11-05 10:59:38.247884 comic-ocr-0.1.3/comic_ocr/models/recognition/train.py
+-rw-r--r--   0        0        0        0 2022-10-22 04:11:06.165788 comic-ocr-0.1.3/comic_ocr/models/recognition/trocr/__init__.py
+-rw-r--r--   0        0        0     5734 2022-11-05 08:54:11.941496 comic-ocr-0.1.3/comic_ocr/models/recognition/trocr/trocr.py
+-rw-r--r--   0        0        0      413 2023-01-01 06:55:13.382652 comic-ocr-0.1.3/comic_ocr/models/transforms.py
+-rw-r--r--   0        0        0      231 2023-01-01 07:58:33.212997 comic-ocr-0.1.3/comic_ocr/types/__init__.py
+-rw-r--r--   0        0        0       89 2022-07-31 05:40:19.127565 comic-ocr-0.1.3/comic_ocr/types/files.py
+-rw-r--r--   0        0        0     1004 2023-01-01 07:58:33.221252 comic-ocr-0.1.3/comic_ocr/types/images.py
+-rw-r--r--   0        0        0     1283 2023-01-01 07:58:33.223699 comic-ocr-0.1.3/comic_ocr/types/lines.py
+-rw-r--r--   0        0        0     6538 2023-01-01 07:18:24.655782 comic-ocr-0.1.3/comic_ocr/types/shapes.py
+-rw-r--r--   0        0        0     2372 2023-01-01 07:58:33.206920 comic-ocr-0.1.3/comic_ocr/utils/__init__.py
+-rw-r--r--   0        0        0     2098 2023-01-09 05:25:50.901182 comic-ocr-0.1.3/comic_ocr/utils/files.py
+-rw-r--r--   0        0        0     3151 2023-02-26 01:32:13.853604 comic-ocr-0.1.3/comic_ocr/utils/nb_annotation.py
+-rw-r--r--   0        0        0     2626 2023-01-01 12:36:49.338062 comic-ocr-0.1.3/comic_ocr/utils/ploting.py
+-rw-r--r--   0        0        0      858 2023-02-24 04:18:21.984041 comic-ocr-0.1.3/comic_ocr/utils/pytorch_model.py
+-rw-r--r--   0        0        0      614 2023-04-16 04:30:38.175259 comic-ocr-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1103 2023-04-16 04:38:31.546007 comic-ocr-0.1.3/setup.py
+-rw-r--r--   0        0        0      684 2023-04-16 04:38:31.546249 comic-ocr-0.1.3/PKG-INFO
```

### Comparing `comic-ocr-0.1.2/comic_ocr/__init__.py` & `comic-ocr-0.1.3/comic_ocr/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import List, Tuple, Optional
 
+from comic_ocr import hub
 from comic_ocr.models import localization
 from comic_ocr.models import recognition
-from comic_ocr.typing import Rectangle, Paragraph, Line, ImageInput, to_image_rgb
+from comic_ocr.types import Rectangle, Paragraph, Line, ImageInput, to_image_rgb
 from comic_ocr.utils.files import get_path_project_dir
 
 _localization_model: Optional[localization.LocalizationModel] = None
 _recognition_model: Optional[recognition.RecognitionModel] = None
 
 
 def read_paragraphs(image: ImageInput) -> List[Paragraph]:
@@ -39,26 +40,28 @@
 
 def localize_paragraphs(image: ImageInput) -> List[Tuple[Rectangle, List[Rectangle]]]:
     image = to_image_rgb(image)
     model = get_localization_model()
     return model.locate_paragraphs(image)
 
 
-def get_localization_model() -> localization.LocalizationModel:
+def get_localization_model(show_download_progress=True, force_reload=False) -> localization.LocalizationModel:
     global _localization_model
     if not _localization_model:
-        _localization_model = localization.load_model()
+        _localization_model = hub.download_localization_model(
+            progress=show_download_progress, force_reload=force_reload, test_executing_model=True)
 
     return _localization_model
 
 
-def get_recognition_model() -> recognition.RecognitionModel:
+def get_recognition_model(show_download_progress=True, force_reload=False) -> recognition.RecognitionModel:
     global _recognition_model
     if not _recognition_model:
-        _recognition_model = recognition.load_model()
+        _recognition_model = hub.download_recognition_model(
+            progress=show_download_progress, force_reload=force_reload, test_executing_model=True)
 
     return _recognition_model
 
 
 if __name__ == '__main__':
     from comic_ocr.utils.files import load_image
     from comic_ocr.utils import image_with_annotations
```

### Comparing `comic-ocr-0.1.2/comic_ocr/dataset/annotated_manga/__init__.py` & `comic-ocr-0.1.3/comic_ocr/dataset/annotated_manga/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-"""A module for loading annotated manga dataset
+"""A module for loading annotated comic dataset
 
 This module uses `comic_ocr.utils.labelling_notebook` for loading the annotation data.
 The annotation should be in `labelling-notebook` format:
 (ref: https://github.com/wanasit/labelling-notebook)
 
 Example:
   images, texts = load_line_annotated_dataset('./example/manga_annotated')
 
 """
 
 from typing import List, Tuple, Optional
 
 from PIL.Image import Image
 
-from comic_ocr.typing import Line
+from comic_ocr.types import Line
 from comic_ocr.utils.files import load_images_with_annotation
 from comic_ocr.utils.nb_annotation import lines_from_nb_annotation_data
 
 
 def load_line_annotated_dataset(
         dataset_dir: str,
         include_empty_text: bool = False,
```

### Comparing `comic-ocr-0.1.2/comic_ocr/dataset/generated_manga/__init__.py` & `comic-ocr-0.1.3/comic_ocr/dataset/generated_manga/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from pathlib import Path
 from typing import Optional, Tuple, List
 
 from PIL import Image
 
 from comic_ocr.dataset.generated_manga.generator import MangaGenerator
 from comic_ocr.dataset.generated_manga.text_area import TextArea
-from comic_ocr.typing import Color, Size, Line
+from comic_ocr.types import Color, Size, Line
 from comic_ocr.utils.files import load_images_with_annotation, load_images, write_json_dict
 from comic_ocr.utils.nb_annotation import lines_to_nb_annotation_data, lines_from_nb_annotation_data
 
 DEFAULT_CHAR_ALPHA = 1.0
 DEFAULT_LINE_ALPHA = 0.6
 DEFAULT_RECT_ALPHA = 0.2
```

### Comparing `comic-ocr-0.1.2/comic_ocr/dataset/generated_manga/generator.py` & `comic-ocr-0.1.3/comic_ocr/dataset/generated_manga/generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from PIL import Image, ImageDraw
 from PIL import ImageFont
 
 from comic_ocr.dataset.generated_manga.text_area import TextArea
 from comic_ocr.dataset.generated_manga.text_bubble import TextBubble
 from comic_ocr.dataset.generated_manga.text_rect import TextRect
-from comic_ocr.typing import Rectangle, Point, Drawable, Size
+from comic_ocr.types import Rectangle, Point, Drawable, Size
 from comic_ocr.utils.files import get_path_example_dir, load_images, load_texts
 
 
 @dataclass
 class MangaGenerator():
     choices_drawings: List[Image.Image]
     choices_texts: List[str]
```

### Comparing `comic-ocr-0.1.2/comic_ocr/dataset/generated_manga/text_area.py` & `comic-ocr-0.1.3/comic_ocr/dataset/generated_manga/text_area.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dataclasses import dataclass, field
 from functools import cached_property
 from typing import List, Optional
 
 from PIL import ImageFont
 
-from comic_ocr.typing import Rectangle, Point, Size, Line, Drawable, Color, to_draw
+from comic_ocr.types import Rectangle, Point, Size, Line, Drawable, Color, to_draw
 
 
 @dataclass
 class TextArea:
     xy: Point = field()
     text: str = field()
```

### Comparing `comic-ocr-0.1.2/comic_ocr/dataset/generated_manga/text_bubble.py` & `comic-ocr-0.1.3/comic_ocr/dataset/generated_manga/text_bubble.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dataclasses import dataclass, field
 from typing import List, Optional
 
 from PIL import Image, ImageDraw, ImageFont
 
 from comic_ocr.dataset.generated_manga.text_area import TextArea
-from comic_ocr.typing import Rectangle, Color, Drawable, to_draw
+from comic_ocr.types import Rectangle, Color, Drawable, to_draw
 
 
 @dataclass
 class TextBubble(TextArea):
     bubble_padding: int = field(default=3, repr=False)
     bubble_fill_color: Color = field(default='#fffffff9', repr=False)
     bubble_outline_width: int = field(default=1, repr=False)
```

### Comparing `comic-ocr-0.1.2/comic_ocr/dataset/generated_manga/text_rect.py` & `comic-ocr-0.1.3/comic_ocr/dataset/generated_manga/text_rect.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from dataclasses import dataclass, field
 
 from comic_ocr.dataset.generated_manga.text_area import TextArea
-from comic_ocr.typing import Color, Drawable, to_draw
+from comic_ocr.types import Color, Drawable, to_draw
 
 
 @dataclass
 class TextRect(TextArea):
     rect_padding: int = field(default=3)
     rect_fill_color: Color = field(default=(255, 255, 255, 250))
     rect_outline_width: int = field(default=1)
```

### Comparing `comic-ocr-0.1.2/comic_ocr/models/localization/__init__.py` & `comic-ocr-0.1.3/comic_ocr/models/localization/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,45 @@
 """A module for localization problem (aka. locating text inside image)
 
 This top-level module provide shortcut and high-level APIs for working with the LocalizationModel and its dependencies
 or implementation details (both Pytorch/ML or OpenCV).
 
 """
 import logging
-from typing import Iterable
+from typing import Iterable, Optional
 
 import torch
 
-from comic_ocr.typing import Rectangle
-from comic_ocr.models.localization.localization_model import LocalizationModel
+from comic_ocr.types import Rectangle
+from comic_ocr.models.localization.localization_model import LocalizationModel, BasicLocalizationModel
 from comic_ocr.models.localization.localization_dataset import LocalizationDataset
 from comic_ocr.utils.files import PathLike, get_path_project_dir, load_image
 
-DEFAULT_TRAINED_MODEL_FILE = get_path_project_dir('trained_models/localization.bin')
+DEFAULT_LOCAL_TRAINED_MODEL_FILE = get_path_project_dir('trained_models/localization.pth')
 DEFAULT_EXAMPLE_IMAGE = get_path_project_dir('example/manga_annotated/normal_01.jpg')
 
 logger = logging.getLogger(__name__)
 
 
-def load_or_create_new_model(model_file: PathLike = DEFAULT_TRAINED_MODEL_FILE) -> LocalizationModel:
+def load_or_create_new_model(model_file: PathLike = DEFAULT_LOCAL_TRAINED_MODEL_FILE) -> LocalizationModel:
     try:
-        model = load_model(model_file)
-        model()
-    except:
+        model = load_model(model_file, test_executing_model=True)
+        return model
+    except (Exception,):
         logger.info(f'Fail loading model at [{model_file}]. Creating a new model.')
-
     return create_new_model()
 
 
 def create_new_model() -> LocalizationModel:
-    from comic_ocr.models.localization.conv_unet.conv_unet import ConvUnet
-    return ConvUnet()
+    from comic_ocr.models.localization.conv_unet import conv_unet
+    return conv_unet.BaselineConvUnet()
 
 
 def load_model(
-        model_file: PathLike = DEFAULT_TRAINED_MODEL_FILE,
+        model_file: PathLike = DEFAULT_LOCAL_TRAINED_MODEL_FILE,
         test_executing_model: bool = True
 ) -> LocalizationModel:
     logger.info(f'Loading localization model [{model_file}]')
     model: LocalizationModel = torch.load(model_file)
 
     if test_executing_model:
         logger.info(f'Testing the model')
@@ -48,48 +47,59 @@
         _ = model.locate_paragraphs(image)
 
     return model
 
 
 def calculate_high_level_metrics(
         model: LocalizationModel,
-        dataset: LocalizationDataset
+        dataset: LocalizationDataset,
+        sample_size_limit: Optional[int] = None
 ):
+    """
+    Calculate understandable high-level metrics (e.g. accuracy for locating lines).
+    """
     assert len(dataset) > 0
-    assert dataset.output_locations_lines, 'Requires dataset with line locations information'
+    assert dataset.output_line_locations, 'Requires dataset with line locations information'
     total_tp = 0
     total_fp = 0
     total_fn = 0
 
     for i in range(len(dataset)):
+        if sample_size_limit and i >= sample_size_limit:
+            break
         baseline_line_locations = dataset.get_line_locations(i)
         line_locations = model.locate_lines(dataset.get_image(i))
         tp, fp, fn = match_location_rectangles_with_baseline(line_locations, baseline_line_locations)
         tp, fp, fn = len(tp), len(fp), len(fn)
         total_tp += tp
         total_fp += fp
         total_fn += fn
 
     return {
-        "dataset_size": len(dataset),
+        "sample_size": i,
         "total_line_level_true_positive": total_tp,
         "total_line_level_false_positive": total_fp,
         "total_line_level_false_negative": total_fn,
-        "line_level_precision": total_tp / (total_tp + total_fp),
-        "line_level_recall": total_tp / (total_tp + total_fn)
+        "line_level_precision": total_tp / (total_tp + total_fp) if total_tp + total_fp > 0 else 0,
+        "line_level_recall": total_tp / (total_tp + total_fn) if total_tp + total_fn > 0 else 0,
+        "line_level_accuracy": total_tp / (total_tp + total_fn + total_fp) if total_tp + total_fn + total_fp > 0 else 0
     }
 
 
 def match_location_rectangles_with_baseline(locations: Iterable[Rectangle], baseline_locations: Iterable[Rectangle]):
     matched_pairs = []
     unmatched_locations = []
+    matched_base_line_indexes = set()
 
     for location in locations:
         for i, baseline_location in enumerate(baseline_locations):
+            if i in matched_base_line_indexes:
+                continue
             if location.can_represent(baseline_location):
                 matched_pairs.append((location, baseline_location))
-                baseline_locations = baseline_locations[:i] + baseline_locations[i + 1:]
+                matched_base_line_indexes.add(i)
                 break
         else:
             unmatched_locations.append(location)
 
-    return matched_pairs, unmatched_locations, baseline_locations
+    unmatched_baseline_locations = [l for i, l in enumerate(baseline_locations) if i not in matched_base_line_indexes]
+    return matched_pairs, unmatched_locations, unmatched_baseline_locations
```

### Comparing `comic-ocr-0.1.2/comic_ocr/models/localization/conv_unet/conv_unet.py` & `comic-ocr-0.1.3/comic_ocr/models/localization/conv_unet/conv_fpn.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,114 +1,98 @@
 import os
+from abc import abstractmethod
+from typing import Any, Tuple
 
 import torch
 from torch import nn
 
 import torch.nn.functional as F
 
+from comic_ocr.models.localization.conv_unet.conv_unet import ConvWithPoolingToHalfSize, DoubleConvWithSecondInput
 from comic_ocr.models.localization.localization_model import LocalizationModel
 from comic_ocr.utils.files import load_images
 
 
-class ConvUnet(LocalizationModel):
-
-    def __init__(self):
-        super(ConvUnet, self).__init__()
-
-        self.down_conv_3 = ConvWithPoolingToHalfSize(3, num_output_channel=8)
-        self.down_conv_2 = ConvWithPoolingToHalfSize(8, kernel_size=5, padding=2, num_output_channel=16)
-        self.down_conv_1 = ConvWithPoolingToHalfSize(16, kernel_size=5, padding=2, num_output_channel=32)
-        self.down_conv_0 = ConvWithPoolingToHalfSize(32, kernel_size=5, padding=2, num_output_channel=64)
-
-        self.up_conv1 = DoubleConvWithSecondInput(64, 32, num_output_channel=64)
-        self.up_conv2 = DoubleConvWithSecondInput(64, 16, num_output_channel=64)
-        self.up_conv3 = DoubleConvWithSecondInput(64, 8, num_output_channel=64)
-
+class AbstractConvFPN(LocalizationModel):
+    def __init__(self,
+                 transformed_channel_size=64 + 3,
+                 hidden_size_output_char=16,
+                 hidden_size_output_line=16,
+                 **kwargs):
+        super(AbstractConvFPN, self).__init__()
+        self.down_layers = nn.ModuleList()
+        self.up_layers = nn.ModuleList()
+        self.up_layer_predicts = nn.ModuleList()
         self.output_conv_char = nn.Sequential(
-            nn.Conv2d(64 + 3, 16, kernel_size=1), nn.ReLU(inplace=True),
-            nn.Conv2d(16, 1, kernel_size=1),
+            nn.Conv2d(transformed_channel_size, hidden_size_output_char, kernel_size=1), nn.ReLU(inplace=True),
+            nn.Conv2d(hidden_size_output_line, 1, kernel_size=1),
         )
-
         self.output_conv_line = nn.Sequential(
-            nn.Conv2d(64 + 3, 16, kernel_size=1), nn.ReLU(inplace=True),
-            nn.Conv2d(16, 1, kernel_size=1),
+            nn.Conv2d(transformed_channel_size, hidden_size_output_line, kernel_size=1), nn.ReLU(inplace=True),
+            nn.Conv2d(hidden_size_output_line, 1, kernel_size=1),
         )
 
-    def forward(self, x):
-        down_3 = self.down_conv_3(x)
-        down_2 = self.down_conv_2(down_3)
-        down_1 = self.down_conv_1(down_2)
-        down_0 = self.down_conv_0(down_1)
-
-        up0 = down_0
-
-        up1 = F.interpolate(up0, down_1.size()[2:], mode='bilinear', align_corners=False)
-        up1 = self.up_conv1(up1, down_1)
-
-        up2 = F.interpolate(up1, down_2.size()[2:], mode='bilinear', align_corners=False)
-        up2 = self.up_conv2(up2, down_2)
-
-        up3 = F.interpolate(up2, down_3.size()[2:], mode='bilinear', align_corners=False)
-        up3 = self.up_conv3(up3, down_3)
-
-        y = F.interpolate(up3, x.size()[2:], mode='bilinear', align_corners=False)
-        y = torch.cat([y, x], dim=1)
+    def forward(self, x: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor, Any]:
+        down_outputs = [x]
+        for i, layer in enumerate(self.down_layers):
+            down = layer(down_outputs[i])
+            down_outputs.append(down)
+
+        up_outputs = [down_outputs.pop()]
+        for i, layer in enumerate(self.up_layers):
+            up = F.interpolate(up_outputs[i], down_outputs[-i - 1].size()[2:], mode='bilinear', align_corners=False)
+            up = layer(up, down_outputs[-i - 1])
+            up_outputs.append(up)
+
+        up_predicts = []
+        for i, up_output in enumerate(up_outputs[1:]):
+            self.up_layer_predicts[i](up_output)
+            up_predict = F.interpolate(up_output, x.size()[2:], mode='bilinear', align_corners=False)
+            up_predicts.append(up_predict)
 
+        y = torch.cat(up_predicts, dim=1)
         y_char = self.output_conv_char(y)
         y_line = self.output_conv_line(y)
-
-        return y_char[:, 0, :], y_line[:, 0, :]
+        return y_char[:, 0, :], y_line[:, 0, :], up_predicts
 
 
-class ConvWithPoolingToHalfSize(nn.Module):
+class BaselineConvFPN(AbstractConvFPN):
     def __init__(self,
-                 num_input_channel,
-                 num_output_channel,
-                 kernel_size=3,
-                 padding=1):
-        super(ConvWithPoolingToHalfSize, self).__init__()
-        self.conv = nn.Sequential(
-            nn.Conv2d(num_input_channel, num_output_channel, kernel_size=kernel_size, padding=padding),
-            nn.BatchNorm2d(num_output_channel),
-            nn.ReLU(),
-            nn.MaxPool2d(kernel_size=2, stride=2),
-        )
-
-    def forward(self, x):
-        x = self.conv(x)
-        return x
+                 **kwargs):
+        super(BaselineConvFPN, self).__init__(transformed_channel_size=64 * 3,
+                                              hidden_size_output_char=64, hidden_size_output_line=64, **kwargs)
+        self.down_layers.append(ConvWithPoolingToHalfSize(3, kernel_size=5, num_output_channel=8))
+        self.down_layers.append(ConvWithPoolingToHalfSize(8, kernel_size=5, padding=2, num_output_channel=16))
+        self.down_layers.append(ConvWithPoolingToHalfSize(16, kernel_size=5, padding=2, num_output_channel=32))
+        self.down_layers.append(ConvWithPoolingToHalfSize(32, kernel_size=5, padding=2, num_output_channel=64))
 
+        self.up_layers.append(DoubleConvWithSecondInput(64, 32, num_output_channel=64))
+        self.up_layer_predicts.append(nn.Conv2d(64, 1, kernel_size=1))
 
-class DoubleConvWithSecondInput(nn.Module):
-    def __init__(self,
-                 num_main_input_channel,
-                 num_second_input_channel,
-                 num_output_channel):
-        super(DoubleConvWithSecondInput, self).__init__()
-        self.conv = nn.Sequential(
-            nn.Conv2d(num_second_input_channel + num_main_input_channel, num_main_input_channel, kernel_size=1),
-            nn.BatchNorm2d(num_main_input_channel),
-            nn.ReLU(inplace=True),
-            nn.Conv2d(num_main_input_channel, num_output_channel, kernel_size=3, padding=1),
-            nn.BatchNorm2d(num_output_channel),
-            nn.ReLU(inplace=True)
-        )
-
-    def forward(self, input, second_input):
-        x = torch.cat([input, second_input], dim=1)
-        x = self.conv(x)
-        return x
+        self.up_layers.append(DoubleConvWithSecondInput(64, 16, num_output_channel=64))
+        self.up_layer_predicts.append(nn.Conv2d(64, 1, kernel_size=1))
 
+        self.up_layers.append(DoubleConvWithSecondInput(64, 8, num_output_channel=64))
+        self.up_layer_predicts.append(nn.Conv2d(64, 1, kernel_size=1))
 
 
 if __name__ == '__main__':
     from torchvision import models
-    from torchvision.models.vgg import model_urls
     from comic_ocr.utils.pytorch_model import get_total_parameters_count
-    module_path = os.path.dirname(__file__)
-    input_images = load_images(module_path + "/../../../out/generate/input/*.jpg")
-    output_images = load_images(module_path + "/../../../out/generate/output/*.jpg")
+    from comic_ocr.models.localization.localization_dataset import LocalizationDataset
+    from comic_ocr.utils import get_path_project_dir
+    from torch.utils.data import DataLoader
 
-    model = ConvUnet()
+    model = BaselineConvFPN()
     print(get_total_parameters_count(model))
-    # input = model.image_to_input(input_images[0]).unsqueeze(0)
-    # output_char, output_mask = model(input)
+
+    path_dataset = get_path_project_dir('data/manga_line_annotated')
+    dataset = LocalizationDataset.load_line_annotated_manga_dataset(path_dataset,
+                                                                    batch_image_size=model.preferred_image_size)
+    # try predicting
+    output_char, output_mask, up_predicts = model(dataset[0]['input'].unsqueeze(0))
+
+    # try loss calculation
+    train_dataloader = DataLoader(dataset, batch_size=2, shuffle=True, num_workers=1)
+    batch = next(iter(train_dataloader))
+    loss = model.compute_loss(batch)
+    print(loss)
```

### Comparing `comic-ocr-0.1.2/comic_ocr/models/localization/localization_model.py` & `comic-ocr-0.1.3/comic_ocr/models/localization/localization_model.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,109 +1,140 @@
-"""The module provides abstract/shared functionalities for ML model for localization
+"""An abstraction and shared functionalities for localization models.
 """
 
 import os
-from typing import Callable, Tuple, List
+from typing import Callable, Tuple, List, Any
 
 import torch
 from PIL import Image
-from torch import nn, Tensor
+from torch import nn
 
 from comic_ocr.models.localization import localization_open_cv as cv
 from comic_ocr.models.localization.localization_utils import image_to_input_tensor, output_tensor_to_image_mask
-from comic_ocr.typing import Size, Rectangle
+from comic_ocr.types import Size, Rectangle
 
-DEFAULT_LOSS_CRITERION_CHAR = nn.BCEWithLogitsLoss(pos_weight=torch.Tensor([2]))
-DEFAULT_LOSS_CRITERION_LINE = nn.BCEWithLogitsLoss(pos_weight=torch.Tensor([0.5]))
 
+def WeightedBCEWithLogitsLoss(weight: float, pos_weight: float):
+    bce_loss = nn.BCEWithLogitsLoss(pos_weight=torch.Tensor([pos_weight]))
+    return lambda y_pred, y: bce_loss(y_pred, y) * weight
 
-class LocalizationModel(nn.Module):
-    """An abstract for localization Module for text localization
 
-    The ML model (Pytorch) classifies each input image's pixel if it's part of a character, a line boundary, or a
-    paragraph boundary. The model output those probabilities as 'mask images' in training dataset format. Namely, given
-    the input source image, the model is trained to output three types of mask images.
+DEFAULT_LOSS_CRITERION_CHAR = WeightedBCEWithLogitsLoss(pos_weight=0.5, weight=2.0)
+DEFAULT_LOSS_CRITERION_LINE = WeightedBCEWithLogitsLoss(pos_weight=0.5, weight=1.0)
 
-    Args:
-        input_image (Tensor [C x H x W])
 
-    Returns probability maps (un-normalized):
-        output_mask_character (Tensor [H x W]) the probability that the pixel is character/text
-        output_mask_line (Tensor [H x W]) the probability that the pixel is inside line rect boundary
+class LocalizationModel(nn.Module):
+    """An abstract for localization models (nn.Module).
 
-    The module also applies other non-ML image-processing techniques on top of the mask images to output the locations.
+    A localization model extends this abstraction should classify if input image's pixel a character or a line (Semantic
+    Segmentation problem). Specifically, given an image as input, the model should output upto probability masks
+    (similar size to input) for each pixel is a part of a character or a line.
 
-    Example:
-        model = ....
-        paragraph_rectangles = model.locate_lines(image)
-    """
+    For training, this abstract class implements `compute_loss()` that computes the model binary classification loss on
+    a LocalizationDataset's batch (images and labelled marks).
 
-    __call__: Callable[..., Tuple[Tensor, Tensor]]
+    For evaluation or serving, this abstract class implements `locate_paragraphs()` (and `locate_lines()`) that takes
+    image input, computes the probability via the model, and uses heuristic OpenCV techniques to identify the lines.
+    """
 
     def __init__(self):
         super().__init__()
 
+    def forward(self, x: torch.Tensor) -> Tuple[torch.Tensor, Any]:
+        """Computes character and line probability marks for the input image.
+
+        Args:
+            x (torch.Tensor[?, C=3, H, W]): the input image
+
+        Returns:
+            output_mask_character (torch.Tensor[?, H, W]): The predict probability mask for characters
+            output_mask_line (torch.Tensor[?, H, W]): The predict probability mask for lines
+            other_output: Other output used by the implementation classes.
+        """
+        raise NotImplementedError
+
     @property
     def preferred_image_size(self) -> Size:
         return Size.of(500, 500)
 
     def compute_loss(
             self,
             dataset_batch,
             loss_criterion_for_char=DEFAULT_LOSS_CRITERION_CHAR,
             loss_criterion_for_line=DEFAULT_LOSS_CRITERION_LINE
-    ) -> Tensor:
+    ) -> torch.Tensor:
         input = dataset_batch['input']
-        output_char, output_line = self(input)
+        output_char, output_line, _ = self(input)
 
         loss = torch.zeros(1)
         if 'output_mask_char' in dataset_batch:
             output = dataset_batch['output_mask_char'].float()
             loss += loss_criterion_for_char(output_char, output)
 
         if 'output_mask_line' in dataset_batch:
             output = dataset_batch['output_mask_line'].float()
             loss += loss_criterion_for_line(output_line, output)
 
         return loss
 
-    def locate_paragraphs(self, image) -> List[Tuple[Rectangle, List[Rectangle]]]:
+    def locate_paragraphs(self, image, threshold=0.5) -> List[Tuple[Rectangle, List[Rectangle]]]:
         output, _ = self._create_output_mask(image)
-        return cv.locate_paragraphs_in_character_mask(output)
+        return cv.locate_paragraphs_in_character_mask(output, input_threshold=threshold)
 
-    def locate_lines(self, image) -> List[Rectangle]:
+    def locate_lines(self, image, threshold=0.5) -> List[Rectangle]:
         output, _ = self._create_output_mask(image)
-        return cv.locate_lines_in_character_mask(output)
+        return cv.locate_lines_in_character_mask(output, input_threshold=threshold)
 
     def create_output_marks(self, image) -> Tuple[Image.Image, Image.Image]:
         output_char, output_line = self._create_output_mask(image)
 
         return output_tensor_to_image_mask(output_char), output_tensor_to_image_mask(output_line)
 
-    def _create_output_mask(self, image) -> Tuple[Tensor, Tensor]:
+    def _create_output_mask(self, image) -> Tuple[torch.Tensor, torch.Tensor]:
         with torch.no_grad():
             input_tensor = image_to_input_tensor(image).unsqueeze(0)
-            output_char, output_line = self(input_tensor)
+            output_char, output_line, _ = self(input_tensor)
 
         return torch.sigmoid(output_char[0]), torch.sigmoid(output_line[0])
 
 
+class BasicLocalizationModel(LocalizationModel):
+    """A basic implementation for the LocalizationModel to be used for testing.
+
+    The model transform the input into the two outputs by two conv2d layers.
+    """
+
+    def __init__(self, kernel_size=1, stride=1):
+        super(BasicLocalizationModel, self).__init__()
+        self.output_conv_char = nn.Conv2d(3, 1, kernel_size=kernel_size, stride=stride)
+        self.output_conv_line = nn.Conv2d(3, 1, kernel_size=kernel_size, stride=stride)
+
+    def forward(self, x: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor, Any]:
+        y_char = self.output_conv_char(x)
+        y_line = self.output_conv_line(x)
+        return y_char[:, 0, :], y_line[:, 0, :], None
+
+    def reset_parameters(self):
+        self.output_conv_char.reset_parameters()
+        self.output_conv_line.reset_parameters()
+
+
 if __name__ == '__main__':
-    from comic_ocr.models.localization.conv_unet.conv_unet import ConvUnet
     from comic_ocr.utils import image_with_annotations, concatenated_images
     from comic_ocr.utils.files import load_image, get_path_project_dir
 
-    path_output_model = get_path_project_dir('data/output/models/localization.bin')
+    path_output_model = get_path_project_dir('data/output/models/localization_base.bin')
+    # path_output_model = ''
 
     if os.path.exists(path_output_model):
         print('Loading an existing model...')
         model = torch.load(path_output_model)
     else:
         print('Creating a new model...')
-        model = ConvUnet()
+        model = BasicLocalizationModel()
 
     # example = load_image(get_path_project_dir('example/manga_generated/image/0001.jpg'))
     example = load_image(get_path_project_dir('example/manga_annotated/normal_01.jpg'))
     # example = load_image(get_path_project_dir('data/manga_line_annotated/u_01.jpg'))
 
     # paragraphs = model.locate_paragraphs(example)
     #
```

### Comparing `comic-ocr-0.1.2/comic_ocr/models/localization/localization_open_cv.py` & `comic-ocr-0.1.3/comic_ocr/models/localization/localization_open_cv.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """Localization methods based-on OpenCV (opencv-python or cv2)
-
 """
 from typing import Union, Tuple, List
 
 import cv2
 import numpy as np
 import torch
 
-from comic_ocr.typing import Rectangle
+from comic_ocr.types import Rectangle
 
 
 def locate_paragraphs_in_character_mask(
         input_tensor: Union[np.ndarray, torch.Tensor],
         *args, **kwargs
 ) -> List[Tuple[Rectangle, List[Rectangle]]]:
     """Locate the lines and paragraphs in the LocalizationModel's character mask output.
@@ -29,15 +28,15 @@
     """
     lines = locate_lines_in_character_mask(input_tensor, *args, **kwargs)
     return group_lines_into_paragraphs(lines)
 
 
 def locate_lines_in_character_mask(
         input_tensor: Union[np.ndarray, torch.Tensor],
-        input_threshold: float = 0.40,
+        input_threshold: float = 0.60,
         expand_detected_component: Tuple[int, int] = (2, 1),
         expand_detected_line: Tuple[int, int] = (2, 2),
         debugging: bool = False
 ) -> List[Rectangle]:
     """Locate the lines in the LocalizationModel's character mask output.
 
     The function expects 2D array/tensor of `white text/characters (1.0) written in the black background (0.0)`
@@ -101,20 +100,26 @@
         else:
             paragraphs.append((line, [line]))
 
     return paragraphs
 
 
 def align_line_horizontal(block_a: Rectangle, block_b: Rectangle, x_min_margin=10, y_margin=2):
-    if block_b.left < block_a.left:
-        block_a, block_b = block_b, block_a
+    """Returns true if two input character blocks are aligned into horizontal line."""
 
+    # First, check if horizontal distance (x-axis) is too far apart
     x_margin = max(block_a.height, block_b.height, x_min_margin)
-    return (block_a.top - y_margin) <= block_b.center.y <= (block_a.bottom + y_margin) and \
-           (abs(block_a.left - block_b.left) - block_a.width) < x_margin
+    x_distance = max(block_a.left, block_b.left) - min(block_a.right, block_b.right)
+    if x_distance > x_margin:
+        return False
+
+    # Assume block_a is taller than block_b, we check if the block_b is vertically within block_a
+    if block_a.height < block_b.height:
+        block_a, block_b = block_b, block_a
+    return (block_b.bottom <= block_a.bottom + y_margin) and (block_b.top >= block_a.top - y_margin)
 
 
 def align_paragraph_left(paragraph_rect: Rectangle, line_rect: Rectangle, x_margin=5, y_min_margin=10):
     y_margin = max(line_rect.height / 5, y_min_margin)
 
     return abs(paragraph_rect.left - line_rect.left) < x_margin and \
            abs(paragraph_rect.bottom - line_rect.top) < y_margin
```

### Comparing `comic-ocr-0.1.2/comic_ocr/models/localization/localization_utils.py` & `comic-ocr-0.1.3/comic_ocr/models/localization/localization_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import numpy as np
 import torch
 from PIL import Image
 from torchvision.transforms import transforms
 from comic_ocr.models.transforms import AddGaussianNoise
 
-from comic_ocr.typing import Rectangle, Size
+from comic_ocr.types import Rectangle, Size
 
 TRANSFORM_TO_TENSOR = transforms.PILToTensor()
 TRANSFORM_TO_GRAY_SCALE = transforms.Grayscale()
 TRANSFORM_ADD_NOISE = AddGaussianNoise()
 
 
 def image_to_input_tensor(
```

### Comparing `comic-ocr-0.1.2/comic_ocr/models/localization/train.py` & `comic-ocr-0.1.3/comic_ocr/models/recognition/train.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,118 +1,134 @@
 import logging
 import os
 from typing import Optional, Callable
 
 import torch
-from torch import optim
 from torch.utils.data import DataLoader
 from tqdm import tqdm
 
-
-from comic_ocr.models.localization.localization_dataset import LocalizationDataset
-from comic_ocr.models.localization.localization_model import LocalizationModel
-from comic_ocr.typing import Size
-from comic_ocr.utils.pytorch_model import calculate_validation_loss
+from comic_ocr.models.recognition.recognition_dataset import RecognitionDataset
+from comic_ocr.models.recognition.recognition_model import RecognitionModel
+from comic_ocr.utils import get_path_project_dir
 
 logger = logging.getLogger(__name__)
 
 
 def train(
-        model: LocalizationModel,
-        train_dataset: LocalizationDataset,
-        validate_dataset: Optional[LocalizationDataset] = None,
-        validate_every_n: Optional[int] = 200,
-        update_callback: Optional[Callable] = None,
-        update_every_n: Optional[int] = 200,
+        model: RecognitionModel,
+        training_dataset: RecognitionDataset,
+        validation_dataset: Optional[RecognitionDataset] = None,
+        validation_every_n: Optional[int] = 200,
         epoch_count: int = 1,
         epoch_callback: Optional[Callable] = None,
+        update_callback: Optional[Callable] = None,
+        update_every_n: Optional[int] = 200,
         tqdm_disable=False,
-        batch_size=10,
-        optimizer=None
+        batch_size=50,
+        optimizer=None,
+        scheduler=None
 ):
-    optimizer = optimizer if optimizer else optim.Adam(model.parameters(), lr=0.001)
-
-    logger.info(f'Training {epoch_count} epochs, on {len(train_dataset)} samples ' +
-                f'({len(validate_dataset)} validation samples)' if validate_dataset else '')
+    # hack: try different optimizer
+    optimizer = optimizer if optimizer else torch.optim.SGD(
+        model.parameters(), lr=0.02, nesterov=True, weight_decay=1e-5, momentum=0.9)
+    scheduler = scheduler if scheduler else torch.optim.lr_scheduler.ReduceLROnPlateau(
+        optimizer, verbose=True, patience=5)
 
-    all_train_losses = []
-    all_validate_losses = []
+    training_losses = []
+    validation_losses = []
 
-    update_counter = 0
-    validate_counter = 0
+    logger.info(f'Training {epoch_count} epochs, on {len(training_dataset)} samples ' +
+                f'({len(validation_dataset)} validation samples)' if validation_dataset else '')
 
     for i_epoch in range(epoch_count):
-        with tqdm(total=len(train_dataset), disable=tqdm_disable) as tepoch:
-            tepoch.set_description(f"Epoch {i_epoch}")
 
-            epoch_training_total_loss = 0
-            epoch_training_total_count = 0
-            training_dataloader = DataLoader(train_dataset, batch_size=batch_size, shuffle=True, num_workers=0)
+        # currently, we can't have batch training because of the padding
+        # todo: support different batch size when it's possible
+        training_dataloader = DataLoader(training_dataset, batch_size=1, shuffle=True, num_workers=0)
+        valid_dataloader = DataLoader(validation_dataset, batch_size=1, shuffle=True, num_workers=0) \
+            if validation_dataset else None
 
+        with tqdm(total=len(training_dataset), disable=tqdm_disable) as tepoch:
+            tepoch.set_description(f"Epoch {i_epoch}")
+
+            batch_loss = 0.0
             for i_batch, batch in enumerate(training_dataloader):
                 optimizer.zero_grad()
                 loss = model.compute_loss(batch)
                 loss.backward()
 
+                # hack: try tuning this later
+                torch.nn.utils.clip_grad_norm_(model.parameters(), 5)
                 optimizer.step()
 
-                current_batch_loss = loss.item()
-                current_batch_size = batch['input'].size(0)
-
-                all_train_losses.append(current_batch_loss)
-                epoch_training_total_loss += current_batch_loss
-                epoch_training_total_count += current_batch_size
-
-                validate_counter += current_batch_size
-                if validate_dataset and validate_every_n and validate_counter >= validate_every_n:
-                    validate_counter = 0
-                    validation_loss = calculate_validation_loss(model, validate_dataset, batch_size=batch_size)
-                    all_validate_losses.append(validation_loss)
-
-                update_counter += current_batch_size
-                if update_callback and update_counter >= update_every_n:
-                    update_counter = 0
-                    update_callback(tepoch.n, all_train_losses, all_validate_losses)
-
-                tepoch.update(current_batch_size)
-                tepoch.set_postfix(
-                    current_batch_loss=current_batch_loss,
-                    validation_loss=all_validate_losses[-1] if all_validate_losses else 0)
-
-            training_loss = epoch_training_total_loss / epoch_training_total_count
-            validation_loss = all_validate_losses[-1] if all_validate_losses else 0
-            tepoch.set_postfix(train_loss=training_loss, validate_loss=validation_loss)
-            logger.info(f'> Finished training with training_loss={training_loss}, validation_loss={validation_loss}')
+                # Todo: remove this when we can set the real batch_size in dataloader
+                batch_loss += loss.item()
+                tepoch.update(1)
+
+                if tepoch.n % batch_size == 0:
+                    batch_loss_avg = batch_loss / batch_size
+                    batch_loss = 0
+
+                    tepoch.set_postfix(training_batch_loss=batch_loss_avg)
+                    training_losses.append(batch_loss_avg)
+
+                if validation_every_n >= 0 and tepoch.n % validation_every_n == 0:
+                    if valid_dataloader:
+                        validation_losses.append(_calculate_validation_loss(model, valid_dataloader))
+                        scheduler.step(validation_losses[-1])
+
+                if update_every_n >= 0 and tepoch.n % update_every_n == 0:
+                    if update_callback:
+                        update_callback(tepoch.n, training_losses, validation_losses)
+
+            if valid_dataloader:
+                validation_losses.append(_calculate_validation_loss(model, valid_dataloader))
+                scheduler.step(validation_losses[-1])
 
             if epoch_callback:
-                epoch_callback(i_epoch, all_train_losses, all_validate_losses)
+                epoch_callback(i_epoch, training_losses, validation_losses)
+
+    return (training_losses, validation_losses) if validation_dataset else (training_losses, None)
+
 
-    return (all_train_losses, all_validate_losses) if validate_dataset else (all_train_losses, None)
+def _calculate_validation_loss(model, valid_dataloader):
+    total_loss = 0
+    total_count = 0
+    with torch.no_grad():
+        for i_batch, batch in enumerate(valid_dataloader):
+            loss = model.compute_loss(batch)
+            total_loss += loss.item()
+            total_count += batch['input'].size(0)
+
+    return total_loss / total_count
 
 
 if __name__ == '__main__':
-    from comic_ocr.models.localization.conv_unet.conv_unet import ConvUnet
-    from comic_ocr.utils import get_path_project_dir
+    from comic_ocr.models.recognition.crnn.crnn import CRNN
+    from comic_ocr.models.recognition.trocr.trocr import TrOCR
+
+    path_dataset = get_path_project_dir('data/output/generate_manga_dataset')
+    path_output_model = get_path_project_dir('data/output/models/recognition.bin')
 
-    path_output_model = get_path_project_dir('data/output/models/localization.bin')
     if os.path.exists(path_output_model):
         print('Loading an existing model...')
         model = torch.load(path_output_model)
     else:
         print('Creating a new model...')
-        model = ConvUnet()
+        model = CRNN()
+
+    dataset = RecognitionDataset.load_generated_dataset(path_dataset)
+    print(f'Loaded generated manga dataset of size {len(dataset)}...')
 
-    path_dataset = get_path_project_dir('data/manga_line_annotated')
-    dataset = LocalizationDataset.load_line_annotated_manga_dataset(path_dataset, image_size=model.preferred_image_size)
-    print(f'Loaded dataset of size {len(dataset)}...')
+    validation_dataset = dataset.subset(to_idx=100)
+    training_dataset = dataset.subset(from_idx=100, to_idx=200)
 
-    #dataset.get_image(0).show()
-    #dataset.get_mask_line(0).show()
+    training_dataset.get_line_image(0).show()
+    training_dataset.get_line_image(1).show()
+    validation_dataset.get_line_image(0).show()
+    validation_dataset.get_line_image(1).show()
 
-    validation_dataset = dataset.subset(to_idx=2)
-    training_dataset = dataset.subset(from_idx=2)
     train(model,
-          train_dataset=training_dataset,
-          validate_dataset=validation_dataset,
-          update_callback=lambda: torch.save(model, path_output_model),
-          update_every_n=10,
+          training_dataset=training_dataset,
+          validation_dataset=validation_dataset,
+          epoch_callback=lambda: torch.save(model, path_output_model),
           epoch_count=10)
```

### Comparing `comic-ocr-0.1.2/comic_ocr/models/recognition/__init__.py` & `comic-ocr-0.1.3/comic_ocr/models/recognition/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 import torch
 
 from comic_ocr.models.recognition.encoding import encode, decode
 from comic_ocr.models.recognition.recognition_model import RecognitionModel, SUPPORT_DICT_SIZE
 from comic_ocr.models.recognition.recognition_dataset import RecognitionDataset
 from comic_ocr.utils.files import PathLike, get_path_project_dir
 
-DEFAULT_TRAINED_MODEL_FILE = get_path_project_dir('trained_models/recognition.bin')
+DEFAULT_LOCAL_TRAINED_MODEL_FILE = get_path_project_dir('trained_models/recognition.pth')
 
 logger = logging.getLogger(__name__)
 
 
-def load_or_create_new_model(model_file: PathLike = DEFAULT_TRAINED_MODEL_FILE) -> RecognitionModel:
+def load_or_create_new_model(model_file: PathLike = DEFAULT_LOCAL_TRAINED_MODEL_FILE) -> RecognitionModel:
     try:
         model = load_model(model_file)
         model()
     except:
         logger.info(f'Fail loading model at [{model_file}]. Creating a new model.')
 
     return create_new_model()
@@ -29,15 +29,15 @@
 
 def create_new_model(**kwargs) -> RecognitionModel:
     from comic_ocr.models.recognition.crnn.crnn import CRNN
     return CRNN(**kwargs)
 
 
 def load_model(
-        model_file: PathLike = DEFAULT_TRAINED_MODEL_FILE,
+        model_file: PathLike = DEFAULT_LOCAL_TRAINED_MODEL_FILE,
         test_executing_model: bool = True
 ) -> RecognitionModel:
     logger.info(f'Loading localization model [{model_file}]')
     model: RecognitionModel = torch.load(model_file)
 
     if test_executing_model:
         # TODO: test the model here
```

### Comparing `comic-ocr-0.1.2/comic_ocr/models/recognition/crnn/crnn.py` & `comic-ocr-0.1.3/comic_ocr/models/recognition/crnn/crnn.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import torch.nn.functional as F
 from torchvision.models import resnet18
 
 from comic_ocr.models.recognition.recognition_model import RecognitionModel, image_to_single_input_tensor
 
 # TODO: Remove this
 # Ref: https://stackoverflow.com/questions/53014306/error-15-initializing-libiomp5-dylib-but-found-libiomp5-dylib-already-initial
-os.environ['KMP_DUPLICATE_LIB_OK'] = 'True'
+#os.environ['KMP_DUPLICATE_LIB_OK'] = 'True'
 
 
 class CRNN(RecognitionModel):
     """
     A Text-Recognition Module based-on CRNN (Convolutional Recurrent Neural Network) framework:
     https://arxiv.org/abs/1507.05717
     """
```

### Comparing `comic-ocr-0.1.2/comic_ocr/models/recognition/encoding.py` & `comic-ocr-0.1.3/comic_ocr/models/recognition/encoding.py`

 * *Files identical despite different names*

### Comparing `comic-ocr-0.1.2/comic_ocr/models/recognition/recognition_dataset.py` & `comic-ocr-0.1.3/comic_ocr/models/recognition/recognition_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from torch.utils.data import Dataset
 
 import comic_ocr.dataset.annotated_manga as annotated_manga
 import comic_ocr.dataset.generated_manga as generated_manga
 
 from comic_ocr.models.recognition import encode
 from comic_ocr.models.recognition.recognition_model import TransformImageToTensor, RecognitionModel
-from comic_ocr.typing import Rectangle
+from comic_ocr.types import Rectangle
 
 
 class RecognitionDataset(Dataset):
     """
     TODO: support input_max_width and add custom padding logic for images
     """
```

### Comparing `comic-ocr-0.1.2/comic_ocr/models/recognition/recognition_model.py` & `comic-ocr-0.1.3/comic_ocr/models/recognition/recognition_model.py`

 * *Files identical despite different names*

### Comparing `comic-ocr-0.1.2/comic_ocr/models/recognition/trocr/trocr.py` & `comic-ocr-0.1.3/comic_ocr/models/recognition/trocr/trocr.py`

 * *Files identical despite different names*

### Comparing `comic-ocr-0.1.2/comic_ocr/typing/images.py` & `comic-ocr-0.1.3/comic_ocr/types/images.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from typing import Union, Tuple
 
 from PIL import Image, ImageDraw
 
-from comic_ocr.typing import PathLike
+from comic_ocr.types import PathLike
 
 '''
 A type representing an input image or image file. 
 '''
 ImageInput = Union[Image.Image, PathLike]
 ImageRGB = Image.Image
```

### Comparing `comic-ocr-0.1.2/comic_ocr/typing/lines.py` & `comic-ocr-0.1.3/comic_ocr/types/lines.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import json
 from dataclasses import dataclass
 from typing import Tuple, List, Union, Optional
-from comic_ocr.typing import Rectangle, RectangleLike
+from comic_ocr.types import Rectangle, RectangleLike
 
 
 class Line(tuple):
 
     def __new__(cls, located_line: Tuple[str, RectangleLike]):
         assert len(located_line) >= 2
         return tuple.__new__(Line, (located_line[0], Rectangle(located_line[1])))
```

### Comparing `comic-ocr-0.1.2/comic_ocr/typing/shapes.py` & `comic-ocr-0.1.3/comic_ocr/types/shapes.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,15 +175,15 @@
         unit_y = unit if isinstance(unit, int) else unit[1]
         return Rectangle((self[0] - unit_x, self[1] - unit_y, self[2] + unit_x, self[3] + unit_y))
 
     def close_to(self, rect: RectangleLike, threshold=0.7) -> bool:
         similarity = Rectangle.jaccard_similarity(self, rect)
         return similarity >= threshold
 
-    def can_represent(self, rect: RectangleLike, threshold_precision=0.7, threshold_recall=0.9) -> bool:
+    def can_represent(self, rect: RectangleLike, threshold_precision=0.7, threshold_recall=0.8) -> bool:
         intersect_rect = Rectangle.intersect_bounding_rect((self, rect))
         if not intersect_rect:
             return False
 
         volume_precision = intersect_rect.size.value / self.size.value
         volume_recall = intersect_rect.size.value / rect.size.value
         return volume_precision >= threshold_precision and volume_recall >= threshold_recall
```

### Comparing `comic-ocr-0.1.2/comic_ocr/utils/__init__.py` & `comic-ocr-0.1.3/comic_ocr/utils/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import List, Union
 
 from PIL import Image, ImageDraw, ImageFont
 
-from comic_ocr.typing import Rectangle, Paragraph, Line, Color
+from comic_ocr.types import Rectangle, Paragraph, Line, Color
 from comic_ocr.utils.files import get_path_project_dir
 
 
 def concatenated_images(
         images: List[Image.Image],
         num_col: int = 3,
         padding: int = 3,
```

### Comparing `comic-ocr-0.1.2/comic_ocr/utils/files.py` & `comic-ocr-0.1.3/comic_ocr/utils/files.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import glob
 import json
 import os
 from typing import Optional, Tuple, List, Dict
 
 from PIL import Image
 
-from comic_ocr.typing import PathLike, ImageRGB
+from comic_ocr.types import PathLike, ImageRGB
 from comic_ocr.utils.nb_annotation import find_annotation_data_for_image
 
 current_module_dir = os.path.dirname(__file__)
 project_root_dir = os.path.join(current_module_dir, '../../')
 
 
 def get_path_project_dir(child='') -> str:
@@ -28,14 +28,16 @@
         alt_annotation_directory: Optional[PathLike] = None
 ) -> Tuple[List[Image.Image], List[str], List[Optional[Dict]]]:
     files = glob.glob(str(glob_file_pattern))
     images = []
     image_files = []
     annotations = []
     for file in sorted(files):
+        if os.path.isdir(file):
+            continue
         if file.endswith('.json'):
             continue
         images.append(load_image(file))
         image_files.append(os.path.abspath(file))
 
         annotation_file = find_annotation_data_for_image(file, alt_annotation_directory)
         annotations.append(annotation_file)
```

### Comparing `comic-ocr-0.1.2/comic_ocr/utils/nb_annotation.py` & `comic-ocr-0.1.3/comic_ocr/utils/nb_annotation.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 This assumes each annotation is per-line.
 
 """
 import json
 import os
 from typing import List, Dict, Optional
 
-from comic_ocr.typing import Line, Rectangle
+from comic_ocr.types import Line, Rectangle
 
 
 def find_annotation_data_for_image(img_path: str, alt_directory: Optional[str] = None) -> Optional[Dict]:
     """
     Look for the annotation file for the image file (starting at the same directory)
     :param img_path: image file (full or relative path)
     :param alt_directory: (Optional) an alternative directory to look for the annotation file
@@ -50,18 +50,19 @@
 
 
 def lines_from_nb_annotation_data(
         annotation_data: Dict,
         empty_text: Optional[str] = None
 ) -> List[Line]:
     lines = []
-    for a in annotation_data['annotations']:
-        line = line_from_nb_annotation(a, empty_text=empty_text)
-        if line:
-            lines.append(line)
+    if 'annotations' in annotation_data:
+        for a in annotation_data['annotations']:
+            line = line_from_nb_annotation(a, empty_text=empty_text)
+            if line:
+                lines.append(line)
 
     return lines
 
 
 def line_to_nb_annotation(line: Line) -> Dict:
     annotation = rect_to_nb_annotation(line.location)
     annotation['text'] = line.text
```

### Comparing `comic-ocr-0.1.2/comic_ocr/utils/ploting.py` & `comic-ocr-0.1.3/comic_ocr/utils/ploting.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Union, List, Tuple
+from typing import Optional, Union, List, Tuple, Collection
 
 import numpy as np
 import matplotlib.pyplot as plt
 from PIL import Image
 
 
 def show_images(
@@ -15,15 +15,15 @@
         images = [images]
 
     if texts and not isinstance(texts, list):
         texts = [texts]
 
     plt.figure(figsize=figsize)
     col_count = min(num_col, len(images))
-    row_count = len(images) // num_col + 1
+    row_count = (len(images) + num_col - 1) // num_col
     for i in range(len(images)):
         # noinspection PyTypeChecker
         conv_img = np.asarray(images[i])
 
         plt.subplot(row_count, col_count, i + 1)
         plt.imshow(conv_img)
 
@@ -57,14 +57,31 @@
         title += f' | Truth: {text_expected}'
 
     plt.imshow(image)
     plt.title(title)
     plt.axis('off')
 
 
+def plot_metrics(
+        metrics: Collection[Tuple[str, List[float]]],
+        num_col: int = 3,
+        figsize: Tuple[int, int] = (12, 6),
+):
+    plt.figure(figsize=figsize)
+    col_count = min(num_col, len(metrics))
+    row_count = (len(metrics) + num_col - 1) // num_col
+    fig, ax = plt.subplots(row_count, col_count, figsize=figsize)
+    for i, (name, values) in enumerate(metrics):
+        sub_plt = ax[i // col_count][i % col_count] if row_count > 1 else ax[i]
+        sub_plt.set_title(name)
+        sub_plt.plot(values)
+        sub_plt.grid()
+    plt.tight_layout(h_pad=2)
+    plt.show()
+
 def plot_losses(
         train_losses: List[float],
         val_losses: List[float],
         figsize: Tuple[int, int] = (12, 6)
 ):
     """
     Plots train and validation losses
```

### Comparing `comic-ocr-0.1.2/comic_ocr/utils/pytorch_model.py` & `comic-ocr-0.1.3/comic_ocr/utils/pytorch_model.py`

 * *Files identical despite different names*

### Comparing `comic-ocr-0.1.2/pyproject.toml` & `comic-ocr-0.1.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 [tool.poetry]
 name = "comic-ocr"
-version = "0.1.2"
+version = "0.1.3"
 description = "An OCR library comic and manga"
 authors = ["Wanasit T"]
 license = "MIT License"
 packages = [
     { include = "comic_ocr" },
 ]
-include = ["trained_models/*.*"]
+include = []
 
 [tool.poetry.dependencies]
 python = "^3.8"
-torch = "^1.11.0"
-torchvision = "^0.12.0"
+torch = "^1.12.1"
+torchvision = "^0.13.1"
 opencv-python = "^4.5.4.60"
 numpy = "^1.21"
 Pillow = "^9.1"
 tqdm = "^4"
 transformers = "^4.23.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7"
 jupyter = "*"
 matplotlib = "*"
 labelling-notebook = "*"
+tensorboard = "*"
+coverage = "*"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `comic-ocr-0.1.2/setup.py` & `comic-ocr-0.1.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,32 +8,32 @@
  'comic_ocr.dataset.generated_manga',
  'comic_ocr.models',
  'comic_ocr.models.localization',
  'comic_ocr.models.localization.conv_unet',
  'comic_ocr.models.recognition',
  'comic_ocr.models.recognition.crnn',
  'comic_ocr.models.recognition.trocr',
- 'comic_ocr.typing',
+ 'comic_ocr.types',
  'comic_ocr.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['Pillow>=9.1,<10.0',
  'numpy>=1.21,<2.0',
  'opencv-python>=4.5.4.60,<5.0.0.0',
- 'torch>=1.11.0,<2.0.0',
- 'torchvision>=0.12.0,<0.13.0',
+ 'torch>=1.12.1,<2.0.0',
+ 'torchvision>=0.13.1,<0.14.0',
  'tqdm>=4,<5',
  'transformers>=4.23.1,<5.0.0']
 
 setup_kwargs = {
     'name': 'comic-ocr',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'An OCR library comic and manga',
     'long_description': None,
     'author': 'Wanasit T',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `comic-ocr-0.1.2/PKG-INFO` & `comic-ocr-0.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: comic-ocr
-Version: 0.1.2
+Version: 0.1.3
 Summary: An OCR library comic and manga
 License: MIT
 Author: Wanasit T
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Pillow (>=9.1,<10.0)
 Requires-Dist: numpy (>=1.21,<2.0)
 Requires-Dist: opencv-python (>=4.5.4.60,<5.0.0.0)
-Requires-Dist: torch (>=1.11.0,<2.0.0)
-Requires-Dist: torchvision (>=0.12.0,<0.13.0)
+Requires-Dist: torch (>=1.12.1,<2.0.0)
+Requires-Dist: torchvision (>=0.13.1,<0.14.0)
 Requires-Dist: tqdm (>=4,<5)
 Requires-Dist: transformers (>=4.23.1,<5.0.0)
```

