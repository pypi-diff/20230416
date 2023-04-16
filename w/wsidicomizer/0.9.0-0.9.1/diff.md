# Comparing `tmp/wsidicomizer-0.9.0.tar.gz` & `tmp/wsidicomizer-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wsidicomizer-0.9.0.tar", max compression
+gzip compressed data, was "wsidicomizer-0.9.1.tar", max compression
```

## Comparing `wsidicomizer-0.9.0.tar` & `wsidicomizer-0.9.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1736 2023-04-03 13:27:43.550591 wsidicomizer-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     8205 2023-04-03 13:27:43.536187 wsidicomizer-0.9.0/README.md
--rw-r--r--   0        0        0      921 2023-03-31 14:54:00.526989 wsidicomizer-0.9.0/wsidicomizer/__init__.py
--rw-r--r--   0        0        0    10732 2023-04-03 13:27:43.562194 wsidicomizer-0.9.0/wsidicomizer/cli.py
--rw-r--r--   0        0        0     1197 2023-04-03 06:05:46.207813 wsidicomizer-0.9.0/wsidicomizer/config.py
--rw-r--r--   0        0        0    23475 2023-04-03 13:27:43.573183 wsidicomizer-0.9.0/wsidicomizer/dataset.py
--rw-r--r--   0        0        0     6541 2023-04-03 06:06:10.389778 wsidicomizer-0.9.0/wsidicomizer/dicomizer_source.py
--rw-r--r--   0        0        0     6049 2023-03-31 14:54:00.541987 wsidicomizer-0.9.0/wsidicomizer/encoding.py
--rw-r--r--   0        0        0      789 2023-04-03 13:27:43.575189 wsidicomizer-0.9.0/wsidicomizer/extras/bioformats/__init__.py
--rw-r--r--   0        0        0     2228 2023-04-03 13:27:43.576394 wsidicomizer-0.9.0/wsidicomizer/extras/bioformats/bioformats_cli.py
--rw-r--r--   0        0        0     3913 2023-04-03 13:27:43.577186 wsidicomizer-0.9.0/wsidicomizer/extras/bioformats/bioformats_dicomizer.py
--rw-r--r--   0        0        0     4418 2023-04-03 13:27:43.578184 wsidicomizer-0.9.0/wsidicomizer/extras/bioformats/bioformats_image_data.py
--rw-r--r--   0        0        0    14802 2023-04-03 13:27:43.579183 wsidicomizer-0.9.0/wsidicomizer/extras/bioformats/bioformats_reader.py
--rw-r--r--   0        0        0     5403 2023-04-03 13:27:43.580183 wsidicomizer-0.9.0/wsidicomizer/extras/bioformats/bioformats_source.py
--rw-r--r--   0        0        0      769 2023-04-03 06:08:44.876033 wsidicomizer-0.9.0/wsidicomizer/extras/openslide/__init__.py
--rw-r--r--   0        0        0     2227 2023-04-03 06:08:51.748970 wsidicomizer-0.9.0/wsidicomizer/extras/openslide/openslide.py
--rw-r--r--   0        0        0    16631 2023-04-03 13:27:43.582423 wsidicomizer-0.9.0/wsidicomizer/extras/openslide/openslide_image_data.py
--rw-r--r--   0        0        0     1476 2023-04-03 13:27:43.593514 wsidicomizer-0.9.0/wsidicomizer/extras/openslide/openslide_metadata.py
--rw-r--r--   0        0        0     3681 2023-04-03 06:08:23.708456 wsidicomizer-0.9.0/wsidicomizer/extras/openslide/openslide_source.py
--rw-r--r--   0        0        0     2069 2023-04-03 06:06:15.956751 wsidicomizer-0.9.0/wsidicomizer/image_data.py
--rw-r--r--   0        0        0      860 2023-04-03 13:27:43.595183 wsidicomizer-0.9.0/wsidicomizer/sources/__init__.py
--rw-r--r--   0        0        0      746 2023-03-31 14:54:00.564988 wsidicomizer-0.9.0/wsidicomizer/sources/czi/__init__.py
--rw-r--r--   0        0        0    13161 2023-04-03 13:27:43.605550 wsidicomizer-0.9.0/wsidicomizer/sources/czi/czi_image_data.py
--rw-r--r--   0        0        0     7933 2023-03-31 14:54:00.571987 wsidicomizer-0.9.0/wsidicomizer/sources/czi/czi_metadata.py
--rw-r--r--   0        0        0     2899 2023-04-03 07:52:59.920634 wsidicomizer-0.9.0/wsidicomizer/sources/czi/czi_source.py
--rw-r--r--   0        0        0      771 2023-03-31 14:54:00.577999 wsidicomizer-0.9.0/wsidicomizer/sources/opentile/__init__.py
--rw-r--r--   0        0        0     8756 2023-04-03 13:27:43.614520 wsidicomizer-0.9.0/wsidicomizer/sources/opentile/opentile_image_data.py
--rw-r--r--   0        0        0     3102 2023-04-03 06:11:05.325431 wsidicomizer-0.9.0/wsidicomizer/sources/opentile/opentile_source.py
--rw-r--r--   0        0        0      775 2023-04-03 13:27:43.622220 wsidicomizer-0.9.0/wsidicomizer/sources/tiffslide/__init__.py
--rw-r--r--   0        0        0    15167 2023-04-03 13:27:43.632185 wsidicomizer-0.9.0/wsidicomizer/sources/tiffslide/tiffslide_image_data.py
--rw-r--r--   0        0        0     1443 2023-04-03 13:27:43.641887 wsidicomizer-0.9.0/wsidicomizer/sources/tiffslide/tiffslide_metadata.py
--rw-r--r--   0        0        0     3575 2023-04-03 13:27:43.651744 wsidicomizer-0.9.0/wsidicomizer/sources/tiffslide/tiffslide_source.py
--rw-r--r--   0        0        0     9561 2023-04-03 13:27:43.660567 wsidicomizer-0.9.0/wsidicomizer/wsidicomizer.py
--rw-r--r--   0        0        0     9782 1970-01-01 00:00:00.000000 wsidicomizer-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1733 2023-04-16 18:01:15.190683 wsidicomizer-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     8205 2023-04-03 13:27:43.536187 wsidicomizer-0.9.1/README.md
+-rw-r--r--   0        0        0      921 2023-04-16 18:01:15.195683 wsidicomizer-0.9.1/wsidicomizer/__init__.py
+-rw-r--r--   0        0        0    10732 2023-04-03 13:27:43.562194 wsidicomizer-0.9.1/wsidicomizer/cli.py
+-rw-r--r--   0        0        0     1197 2023-04-03 06:05:46.207813 wsidicomizer-0.9.1/wsidicomizer/config.py
+-rw-r--r--   0        0        0    23475 2023-04-16 18:01:15.243759 wsidicomizer-0.9.1/wsidicomizer/dataset.py
+-rw-r--r--   0        0        0     6735 2023-04-16 18:01:15.266942 wsidicomizer-0.9.1/wsidicomizer/dicomizer_source.py
+-rw-r--r--   0        0        0     6049 2023-03-31 14:54:00.541987 wsidicomizer-0.9.1/wsidicomizer/encoding.py
+-rw-r--r--   0        0        0      789 2023-04-03 13:27:43.575189 wsidicomizer-0.9.1/wsidicomizer/extras/bioformats/__init__.py
+-rw-r--r--   0        0        0     2228 2023-04-03 13:27:43.576394 wsidicomizer-0.9.1/wsidicomizer/extras/bioformats/bioformats_cli.py
+-rw-r--r--   0        0        0     3913 2023-04-16 18:01:15.299403 wsidicomizer-0.9.1/wsidicomizer/extras/bioformats/bioformats_dicomizer.py
+-rw-r--r--   0        0        0     4418 2023-04-03 13:27:43.578184 wsidicomizer-0.9.1/wsidicomizer/extras/bioformats/bioformats_image_data.py
+-rw-r--r--   0        0        0    14802 2023-04-08 06:20:09.255055 wsidicomizer-0.9.1/wsidicomizer/extras/bioformats/bioformats_reader.py
+-rw-r--r--   0        0        0     5403 2023-04-16 18:01:15.324824 wsidicomizer-0.9.1/wsidicomizer/extras/bioformats/bioformats_source.py
+-rw-r--r--   0        0        0      769 2023-04-03 06:08:44.876033 wsidicomizer-0.9.1/wsidicomizer/extras/openslide/__init__.py
+-rw-r--r--   0        0        0     2227 2023-04-03 06:08:51.748970 wsidicomizer-0.9.1/wsidicomizer/extras/openslide/openslide.py
+-rw-r--r--   0        0        0    16631 2023-04-03 13:27:43.582423 wsidicomizer-0.9.1/wsidicomizer/extras/openslide/openslide_image_data.py
+-rw-r--r--   0        0        0     1476 2023-04-03 13:27:43.593514 wsidicomizer-0.9.1/wsidicomizer/extras/openslide/openslide_metadata.py
+-rw-r--r--   0        0        0     3787 2023-04-16 18:01:15.353013 wsidicomizer-0.9.1/wsidicomizer/extras/openslide/openslide_source.py
+-rw-r--r--   0        0        0     2069 2023-04-03 06:06:15.956751 wsidicomizer-0.9.1/wsidicomizer/image_data.py
+-rw-r--r--   0        0        0      860 2023-04-03 13:27:43.595183 wsidicomizer-0.9.1/wsidicomizer/sources/__init__.py
+-rw-r--r--   0        0        0      746 2023-03-31 14:54:00.564988 wsidicomizer-0.9.1/wsidicomizer/sources/czi/__init__.py
+-rw-r--r--   0        0        0    13161 2023-04-03 13:27:43.605550 wsidicomizer-0.9.1/wsidicomizer/sources/czi/czi_image_data.py
+-rw-r--r--   0        0        0     7933 2023-04-16 18:01:15.358822 wsidicomizer-0.9.1/wsidicomizer/sources/czi/czi_metadata.py
+-rw-r--r--   0        0        0     2899 2023-04-16 18:01:15.407906 wsidicomizer-0.9.1/wsidicomizer/sources/czi/czi_source.py
+-rw-r--r--   0        0        0      771 2023-04-16 18:02:33.046081 wsidicomizer-0.9.1/wsidicomizer/sources/opentile/__init__.py
+-rw-r--r--   0        0        0     8756 2023-04-08 06:20:09.243941 wsidicomizer-0.9.1/wsidicomizer/sources/opentile/opentile_image_data.py
+-rw-r--r--   0        0        0     3102 2023-04-16 18:01:15.432092 wsidicomizer-0.9.1/wsidicomizer/sources/opentile/opentile_source.py
+-rw-r--r--   0        0        0      775 2023-04-03 13:27:43.622220 wsidicomizer-0.9.1/wsidicomizer/sources/tiffslide/__init__.py
+-rw-r--r--   0        0        0    15167 2023-04-16 18:01:15.458910 wsidicomizer-0.9.1/wsidicomizer/sources/tiffslide/tiffslide_image_data.py
+-rw-r--r--   0        0        0     1443 2023-04-16 18:01:15.485967 wsidicomizer-0.9.1/wsidicomizer/sources/tiffslide/tiffslide_metadata.py
+-rw-r--r--   0        0        0     3575 2023-04-16 18:01:15.515906 wsidicomizer-0.9.1/wsidicomizer/sources/tiffslide/tiffslide_source.py
+-rw-r--r--   0        0        0     9561 2023-04-16 18:01:15.541906 wsidicomizer-0.9.1/wsidicomizer/wsidicomizer.py
+-rw-r--r--   0        0        0     9782 1970-01-01 00:00:00.000000 wsidicomizer-0.9.1/PKG-INFO
```

### Comparing `wsidicomizer-0.9.0/pyproject.toml` & `wsidicomizer-0.9.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wsidicomizer"
-version = "0.9.0"
+version = "0.9.1"
 description = "Tool for reading WSI files from proprietary formats and optionally convert them to to DICOM"
 authors = ["Erik O Gabrielsson <erik.o.gabrielsson@sectra.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/imi-bigpicture/wsidicomizer"
 keywords = ["whole slide image", "digital pathology", "dicom", "converter"]
 classifiers = [
@@ -47,10 +47,10 @@
 openslide-python = "^1.1.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-wsidicomizer = "wsidicomizer.cli.wsidicomizer_cli:main"
-bioformats_wsidicomizer = "wsidicomizer.cli.bioformats_cli:main"
+wsidicomizer = "wsidicomizer.cli:main"
+bioformats_wsidicomizer = "wsidicomizer.extras.bioformats.bioformats_cli:main"
```

### Comparing `wsidicomizer-0.9.0/README.md` & `wsidicomizer-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.0/wsidicomizer/__init__.py` & `wsidicomizer-0.9.1/wsidicomizer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,8 +18,8 @@
     create_patient_module,
     create_sample,
     create_specimen_module,
     create_study_module,
 )
 from wsidicomizer.wsidicomizer import WsiDicomizer
 
-__version__ = "0.9.0"
+__version__ = "0.9.1"
```

### Comparing `wsidicomizer-0.9.0/wsidicomizer/cli.py` & `wsidicomizer-0.9.1/wsidicomizer/cli.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.0/wsidicomizer/config.py` & `wsidicomizer-0.9.1/wsidicomizer/config.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.0/wsidicomizer/dataset.py` & `wsidicomizer-0.9.1/wsidicomizer/dataset.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.0/wsidicomizer/dicomizer_source.py` & `wsidicomizer-0.9.1/wsidicomizer/dicomizer_source.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,194 +1,194 @@
-#    Copyright 2021, 2022, 2023 SECTRA AB
-#
-#    Licensed under the Apache License, Version 2.0 (the "License");
-#    you may not use this file except in compliance with the License.
-#    You may obtain a copy of the License at
-#
-#        http://www.apache.org/licenses/LICENSE-2.0
-#
-#    Unless required by applicable law or agreed to in writing, software
-#    distributed under the License is distributed on an "AS IS" BASIS,
-#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#    See the License for the specific language governing permissions and
-#    limitations under the License.
-
-"""Module containing a base Source implementation suitable for use with non-DICOM
-files."""
-
-from abc import ABCMeta, abstractmethod
-from pathlib import Path
-from typing import List, Optional, Sequence, Union
-
-from opentile.metadata import Metadata
-from pydicom import Dataset, config
-from pydicom.dataset import Dataset
-from wsidicom.instance import ImageType, WsiDataset, WsiInstance
-from wsidicom.source import Source
-from wsidicom.graphical_annotations import AnnotationInstance
-
-from wsidicomizer.dataset import create_base_dataset, populate_base_dataset
-from wsidicomizer.encoding import Encoder
-from wsidicomizer.image_data import DicomizerImageData
-
-config.enforce_valid_values = True
-config.future_behavior()
-
-
-class DicomizerSource(Source, metaclass=ABCMeta):
-    """
-    Metaclass for Dicomizer sources. Subclasses should implement the method
-    is_supported(), _create_level_image_data(), _create_label_image_data(), and
-     _create_overview_image_data() and the properties metadata, pyramid_levels,
-     has_label, and has_overview. Subclasses can override the __init__().
-    """
-
-    def __init__(
-        self,
-        filepath: Path,
-        encoder: Encoder,
-        tile_size: int = 512,
-        modules: Optional[Union[Dataset, Sequence[Dataset]]] = None,
-        include_levels: Optional[Sequence[int]] = None,
-        include_label: bool = True,
-        include_overview: bool = True,
-        include_confidential: bool = True,
-    ) -> None:
-        self._filepath = filepath
-        self._encoder = encoder
-        self._tile_size = tile_size
-        self._modules = modules
-        self._include_levels = include_levels
-        self._include_label = include_label
-        self._include_overview = include_overview
-        self._include_confidential = include_confidential
-        self._base_dataset = populate_base_dataset(
-            self.metadata, create_base_dataset(modules), include_confidential
-        )
-
-    @staticmethod
-    @abstractmethod
-    def is_supported(path: Path) -> bool:
-        """Return True if file in filepath is supported by Dicomizer."""
-        raise NotImplementedError()
-
-    @property
-    @abstractmethod
-    def metadata(self) -> Metadata:
-        """Return metadata for file."""
-        raise NotImplementedError()
-
-    @property
-    @abstractmethod
-    def pyramid_levels(self) -> List[int]:
-        """Return pyramid levels (scalings) for file."""
-        raise NotImplementedError()
-
-    @property
-    @abstractmethod
-    def has_label(self) -> bool:
-        """Return True if file has a label image."""
-        raise NotImplementedError()
-
-    @property
-    @abstractmethod
-    def has_overview(self) -> bool:
-        """Return True if file has a overview image."""
-        raise NotImplementedError()
-
-    @abstractmethod
-    def _create_level_image_data(self, level_index: int) -> DicomizerImageData:
-        """Return image data instance for level."""
-        raise NotImplementedError()
-
-    @abstractmethod
-    def _create_label_image_data(
-        self,
-    ) -> DicomizerImageData:
-        """Return image data instance for label."""
-        raise NotImplementedError()
-
-    @abstractmethod
-    def _create_overview_image_data(self) -> DicomizerImageData:
-        """Return image data instance for overview."""
-        raise NotImplementedError()
-
-    @property
-    def base_dataset(self) -> WsiDataset:
-        return WsiDataset(self._base_dataset)
-
-    @property
-    def level_instances(self) -> List[WsiInstance]:
-        return [
-            WsiInstance.create_instance(
-                self._create_level_image_data(level_index),
-                self._base_dataset,
-                ImageType.VOLUME,
-            )
-            for level_index in range(len(self.pyramid_levels))
-            if self._is_included_level(
-                self.pyramid_levels[level_index],
-                self.pyramid_levels,
-                self._include_levels,
-            )
-        ]
-
-    @property
-    def label_instances(self) -> List[WsiInstance]:
-        if not self.has_label or not self._include_label:
-            return []
-
-        label = WsiInstance.create_instance(
-            self._create_label_image_data(), self._base_dataset, ImageType.LABEL
-        )
-        return [label]
-
-    @property
-    def overview_instances(self) -> List[WsiInstance]:
-        if not self.has_overview or not self._include_overview:
-            return []
-
-        overview = WsiInstance.create_instance(
-            self._create_overview_image_data(), self._base_dataset, ImageType.OVERVIEW
-        )
-        return [overview]
-
-    @property
-    def annotation_instances(self) -> List[AnnotationInstance]:
-        return []
-
-    @staticmethod
-    def _is_included_level(
-        level: int,
-        present_levels: Sequence[int],
-        include_indices: Optional[Sequence[int]] = None,
-    ) -> bool:
-        """Return true if pyramid level is in included levels.
-
-        Parameters
-        ----------
-        level: int
-            Pyramid level to check.
-        present_levels: Sequence[int]
-            List of pyramid levels present.
-        include_indices: Optional[Sequence[int]] = None
-            Optional list indices (in present levels) to include, e.g. [0, 1]
-            includes the two lowest levels. Negative indicies can be used,
-            e.g. [-1, -2] includes the two highest levels. Default of None
-            will not limit the selection. An empty sequence will exluded all
-            levels.
-
-        Returns
-        ----------
-        bool
-            True if level should be included.
-        """
-        if level not in present_levels:
-            return False
-        if include_indices is None:
-            return True
-        absolute_levels = [
-            present_levels[level]
-            for level in include_indices
-            if -len(present_levels) <= level < len(present_levels)
-        ]
-        return level in absolute_levels
+#    Copyright 2021, 2022, 2023 SECTRA AB
+#
+#    Licensed under the Apache License, Version 2.0 (the "License");
+#    you may not use this file except in compliance with the License.
+#    You may obtain a copy of the License at
+#
+#        http://www.apache.org/licenses/LICENSE-2.0
+#
+#    Unless required by applicable law or agreed to in writing, software
+#    distributed under the License is distributed on an "AS IS" BASIS,
+#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#    See the License for the specific language governing permissions and
+#    limitations under the License.
+
+"""Module containing a base Source implementation suitable for use with non-DICOM
+files."""
+
+from abc import ABCMeta, abstractmethod
+from pathlib import Path
+from typing import List, Optional, Sequence, Union
+
+from opentile.metadata import Metadata
+from pydicom import Dataset, config
+from pydicom.dataset import Dataset
+from wsidicom.instance import ImageType, WsiDataset, WsiInstance
+from wsidicom.source import Source
+from wsidicom.graphical_annotations import AnnotationInstance
+
+from wsidicomizer.dataset import create_base_dataset, populate_base_dataset
+from wsidicomizer.encoding import Encoder
+from wsidicomizer.image_data import DicomizerImageData
+
+config.enforce_valid_values = True
+config.future_behavior()
+
+
+class DicomizerSource(Source, metaclass=ABCMeta):
+    """
+    Metaclass for Dicomizer sources. Subclasses should implement the method
+    is_supported(), _create_level_image_data(), _create_label_image_data(), and
+     _create_overview_image_data() and the properties metadata, pyramid_levels,
+     has_label, and has_overview. Subclasses can override the __init__().
+    """
+
+    def __init__(
+        self,
+        filepath: Path,
+        encoder: Encoder,
+        tile_size: int = 512,
+        modules: Optional[Union[Dataset, Sequence[Dataset]]] = None,
+        include_levels: Optional[Sequence[int]] = None,
+        include_label: bool = True,
+        include_overview: bool = True,
+        include_confidential: bool = True,
+    ) -> None:
+        self._filepath = filepath
+        self._encoder = encoder
+        self._tile_size = tile_size
+        self._modules = modules
+        self._include_levels = include_levels
+        self._include_label = include_label
+        self._include_overview = include_overview
+        self._include_confidential = include_confidential
+        self._base_dataset = populate_base_dataset(
+            self.metadata, create_base_dataset(modules), include_confidential
+        )
+
+    @staticmethod
+    @abstractmethod
+    def is_supported(path: Path) -> bool:
+        """Return True if file in filepath is supported by Dicomizer."""
+        raise NotImplementedError()
+
+    @property
+    @abstractmethod
+    def metadata(self) -> Metadata:
+        """Return metadata for file."""
+        raise NotImplementedError()
+
+    @property
+    @abstractmethod
+    def pyramid_levels(self) -> List[int]:
+        """Return pyramid levels (scalings) for file."""
+        raise NotImplementedError()
+
+    @property
+    @abstractmethod
+    def has_label(self) -> bool:
+        """Return True if file has a label image."""
+        raise NotImplementedError()
+
+    @property
+    @abstractmethod
+    def has_overview(self) -> bool:
+        """Return True if file has a overview image."""
+        raise NotImplementedError()
+
+    @abstractmethod
+    def _create_level_image_data(self, level_index: int) -> DicomizerImageData:
+        """Return image data instance for level."""
+        raise NotImplementedError()
+
+    @abstractmethod
+    def _create_label_image_data(
+        self,
+    ) -> DicomizerImageData:
+        """Return image data instance for label."""
+        raise NotImplementedError()
+
+    @abstractmethod
+    def _create_overview_image_data(self) -> DicomizerImageData:
+        """Return image data instance for overview."""
+        raise NotImplementedError()
+
+    @property
+    def base_dataset(self) -> WsiDataset:
+        return WsiDataset(self._base_dataset)
+
+    @property
+    def level_instances(self) -> List[WsiInstance]:
+        return [
+            WsiInstance.create_instance(
+                self._create_level_image_data(level_index),
+                self._base_dataset,
+                ImageType.VOLUME,
+            )
+            for level_index in range(len(self.pyramid_levels))
+            if self._is_included_level(
+                self.pyramid_levels[level_index],
+                self.pyramid_levels,
+                self._include_levels,
+            )
+        ]
+
+    @property
+    def label_instances(self) -> List[WsiInstance]:
+        if not self.has_label or not self._include_label:
+            return []
+
+        label = WsiInstance.create_instance(
+            self._create_label_image_data(), self._base_dataset, ImageType.LABEL
+        )
+        return [label]
+
+    @property
+    def overview_instances(self) -> List[WsiInstance]:
+        if not self.has_overview or not self._include_overview:
+            return []
+
+        overview = WsiInstance.create_instance(
+            self._create_overview_image_data(), self._base_dataset, ImageType.OVERVIEW
+        )
+        return [overview]
+
+    @property
+    def annotation_instances(self) -> List[AnnotationInstance]:
+        return []
+
+    @staticmethod
+    def _is_included_level(
+        level: int,
+        present_levels: Sequence[int],
+        include_indices: Optional[Sequence[int]] = None,
+    ) -> bool:
+        """Return true if pyramid level is in included levels.
+
+        Parameters
+        ----------
+        level: int
+            Pyramid level to check.
+        present_levels: Sequence[int]
+            List of pyramid levels present.
+        include_indices: Optional[Sequence[int]] = None
+            Optional list indices (in present levels) to include, e.g. [0, 1]
+            includes the two lowest levels. Negative indicies can be used,
+            e.g. [-1, -2] includes the two highest levels. Default of None
+            will not limit the selection. An empty sequence will exluded all
+            levels.
+
+        Returns
+        ----------
+        bool
+            True if level should be included.
+        """
+        if level not in present_levels:
+            return False
+        if include_indices is None:
+            return True
+        absolute_levels = [
+            present_levels[level]
+            for level in include_indices
+            if -len(present_levels) <= level < len(present_levels)
+        ]
+        return level in absolute_levels
```

### Comparing `wsidicomizer-0.9.0/wsidicomizer/encoding.py` & `wsidicomizer-0.9.1/wsidicomizer/encoding.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.0/wsidicomizer/extras/bioformats/__init__.py` & `wsidicomizer-0.9.1/wsidicomizer/extras/bioformats/__init__.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.0/wsidicomizer/extras/bioformats/bioformats_cli.py` & `wsidicomizer-0.9.1/wsidicomizer/extras/bioformats/bioformats_cli.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.0/wsidicomizer/extras/bioformats/bioformats_dicomizer.py` & `wsidicomizer-0.9.1/wsidicomizer/extras/bioformats/bioformats_dicomizer.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.0/wsidicomizer/extras/bioformats/bioformats_image_data.py` & `wsidicomizer-0.9.1/wsidicomizer/extras/bioformats/bioformats_image_data.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.0/wsidicomizer/extras/bioformats/bioformats_reader.py` & `wsidicomizer-0.9.1/wsidicomizer/extras/bioformats/bioformats_reader.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.0/wsidicomizer/extras/bioformats/bioformats_source.py` & `wsidicomizer-0.9.1/wsidicomizer/extras/bioformats/bioformats_source.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.0/wsidicomizer/extras/openslide/__init__.py` & `wsidicomizer-0.9.1/wsidicomizer/extras/openslide/__init__.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.0/wsidicomizer/extras/openslide/openslide.py` & `wsidicomizer-0.9.1/wsidicomizer/extras/openslide/openslide.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.0/wsidicomizer/extras/openslide/openslide_image_data.py` & `wsidicomizer-0.9.1/wsidicomizer/extras/openslide/openslide_image_data.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.0/wsidicomizer/extras/openslide/openslide_metadata.py` & `wsidicomizer-0.9.1/wsidicomizer/extras/openslide/openslide_metadata.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.0/wsidicomizer/extras/openslide/openslide_source.py` & `wsidicomizer-0.9.1/wsidicomizer/extras/openslide/openslide_source.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,106 +1,106 @@
-#    Copyright 2021, 2022, 2023 SECTRA AB
-#
-#    Licensed under the Apache License, Version 2.0 (the "License");
-#    you may not use this file except in compliance with the License.
-#    You may obtain a copy of the License at
-#
-#        http://www.apache.org/licenses/LICENSE-2.0
-#
-#    Unless required by applicable law or agreed to in writing, software
-#    distributed under the License is distributed on an "AS IS" BASIS,
-#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#    See the License for the specific language governing permissions and
-#    limitations under the License.
-
-"""Source for reading openslide compatible file."""
-
-import math
-from pathlib import Path
-from typing import List, Optional, Sequence, Union
-
-from opentile.metadata import Metadata
-from pydicom import Dataset
-
-from wsidicomizer.dicomizer_source import DicomizerSource
-from wsidicomizer.encoding import Encoder
-from wsidicomizer.extras.openslide.openslide import OpenSlide
-from wsidicomizer.extras.openslide.openslide_image_data import (
-    OpenSlideAssociatedImageData,
-    OpenSlideAssociatedImageType,
-    OpenSlideLevelImageData,
-)
-from wsidicomizer.extras.openslide.openslide_metadata import OpenSlideMetadata
-from wsidicomizer.image_data import DicomizerImageData
-
-
-class OpenSlideSource(DicomizerSource):
-    def __init__(
-        self,
-        filepath: Path,
-        encoder: Encoder,
-        tile_size: int = 512,
-        modules: Optional[Union[Dataset, Sequence[Dataset]]] = None,
-        include_levels: Optional[Sequence[int]] = None,
-        include_label: bool = True,
-        include_overview: bool = True,
-        include_confidential: bool = True,
-    ) -> None:
-        self._slide = OpenSlide(filepath)
-        self._pyramid_levels = self._get_pyramid_levels(self._slide)
-        self._metadata = OpenSlideMetadata(self._slide)
-        super().__init__(
-            filepath,
-            encoder,
-            tile_size,
-            modules,
-            include_levels,
-            include_label,
-            include_overview,
-            include_confidential,
-        )
-
-    def close(self) -> None:
-        return self._slide.close()
-
-    @property
-    def has_label(self) -> bool:
-        return OpenSlideAssociatedImageType.LABEL.value in self._slide.associated_images
-
-    @property
-    def has_overview(self) -> bool:
-        return OpenSlideAssociatedImageType.MACRO.value in self._slide.associated_images
-
-    @property
-    def metadata(self) -> Metadata:
-        return self._metadata
-
-    @property
-    def pyramid_levels(self) -> List[int]:
-        return self._pyramid_levels
-
-    @staticmethod
-    def is_supported(filepath: Path) -> bool:
-        """Return True if file in filepath is supported by OpenSlide."""
-        return OpenSlide.detect_format(str(filepath)) is not None
-
-    def _create_level_image_data(self, level_index: int) -> DicomizerImageData:
-        return OpenSlideLevelImageData(
-            self._slide, level_index, self._tile_size, self._encoder
-        )
-
-    def _create_label_image_data(self) -> DicomizerImageData:
-        return OpenSlideAssociatedImageData(
-            self._slide, OpenSlideAssociatedImageType.LABEL, self._encoder
-        )
-
-    def _create_overview_image_data(self) -> DicomizerImageData:
-        return OpenSlideAssociatedImageData(
-            self._slide, OpenSlideAssociatedImageType.MACRO, self._encoder
-        )
-
-    @staticmethod
-    def _get_pyramid_levels(slide: OpenSlide) -> List[int]:
-        """Return list of pyramid levels present in openslide slide."""
-        return [
-            int(math.log2(int(downsample))) for downsample in slide.level_downsamples
-        ]
+#    Copyright 2021, 2022, 2023 SECTRA AB
+#
+#    Licensed under the Apache License, Version 2.0 (the "License");
+#    you may not use this file except in compliance with the License.
+#    You may obtain a copy of the License at
+#
+#        http://www.apache.org/licenses/LICENSE-2.0
+#
+#    Unless required by applicable law or agreed to in writing, software
+#    distributed under the License is distributed on an "AS IS" BASIS,
+#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#    See the License for the specific language governing permissions and
+#    limitations under the License.
+
+"""Source for reading openslide compatible file."""
+
+import math
+from pathlib import Path
+from typing import List, Optional, Sequence, Union
+
+from opentile.metadata import Metadata
+from pydicom import Dataset
+
+from wsidicomizer.dicomizer_source import DicomizerSource
+from wsidicomizer.encoding import Encoder
+from wsidicomizer.extras.openslide.openslide import OpenSlide
+from wsidicomizer.extras.openslide.openslide_image_data import (
+    OpenSlideAssociatedImageData,
+    OpenSlideAssociatedImageType,
+    OpenSlideLevelImageData,
+)
+from wsidicomizer.extras.openslide.openslide_metadata import OpenSlideMetadata
+from wsidicomizer.image_data import DicomizerImageData
+
+
+class OpenSlideSource(DicomizerSource):
+    def __init__(
+        self,
+        filepath: Path,
+        encoder: Encoder,
+        tile_size: int = 512,
+        modules: Optional[Union[Dataset, Sequence[Dataset]]] = None,
+        include_levels: Optional[Sequence[int]] = None,
+        include_label: bool = True,
+        include_overview: bool = True,
+        include_confidential: bool = True,
+    ) -> None:
+        self._slide = OpenSlide(filepath)
+        self._pyramid_levels = self._get_pyramid_levels(self._slide)
+        self._metadata = OpenSlideMetadata(self._slide)
+        super().__init__(
+            filepath,
+            encoder,
+            tile_size,
+            modules,
+            include_levels,
+            include_label,
+            include_overview,
+            include_confidential,
+        )
+
+    def close(self) -> None:
+        return self._slide.close()
+
+    @property
+    def has_label(self) -> bool:
+        return OpenSlideAssociatedImageType.LABEL.value in self._slide.associated_images
+
+    @property
+    def has_overview(self) -> bool:
+        return OpenSlideAssociatedImageType.MACRO.value in self._slide.associated_images
+
+    @property
+    def metadata(self) -> Metadata:
+        return self._metadata
+
+    @property
+    def pyramid_levels(self) -> List[int]:
+        return self._pyramid_levels
+
+    @staticmethod
+    def is_supported(filepath: Path) -> bool:
+        """Return True if file in filepath is supported by OpenSlide."""
+        return OpenSlide.detect_format(str(filepath)) is not None
+
+    def _create_level_image_data(self, level_index: int) -> DicomizerImageData:
+        return OpenSlideLevelImageData(
+            self._slide, level_index, self._tile_size, self._encoder
+        )
+
+    def _create_label_image_data(self) -> DicomizerImageData:
+        return OpenSlideAssociatedImageData(
+            self._slide, OpenSlideAssociatedImageType.LABEL, self._encoder
+        )
+
+    def _create_overview_image_data(self) -> DicomizerImageData:
+        return OpenSlideAssociatedImageData(
+            self._slide, OpenSlideAssociatedImageType.MACRO, self._encoder
+        )
+
+    @staticmethod
+    def _get_pyramid_levels(slide: OpenSlide) -> List[int]:
+        """Return list of pyramid levels present in openslide slide."""
+        return [
+            int(math.log2(int(downsample))) for downsample in slide.level_downsamples
+        ]
```

### Comparing `wsidicomizer-0.9.0/wsidicomizer/image_data.py` & `wsidicomizer-0.9.1/wsidicomizer/image_data.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.0/wsidicomizer/sources/__init__.py` & `wsidicomizer-0.9.1/wsidicomizer/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.0/wsidicomizer/sources/czi/__init__.py` & `wsidicomizer-0.9.1/wsidicomizer/sources/czi/__init__.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.0/wsidicomizer/sources/czi/czi_image_data.py` & `wsidicomizer-0.9.1/wsidicomizer/sources/czi/czi_image_data.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.0/wsidicomizer/sources/czi/czi_metadata.py` & `wsidicomizer-0.9.1/wsidicomizer/sources/czi/czi_metadata.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.0/wsidicomizer/sources/czi/czi_source.py` & `wsidicomizer-0.9.1/wsidicomizer/sources/czi/czi_source.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.0/wsidicomizer/sources/opentile/__init__.py` & `wsidicomizer-0.9.1/wsidicomizer/sources/opentile/__init__.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.0/wsidicomizer/sources/opentile/opentile_image_data.py` & `wsidicomizer-0.9.1/wsidicomizer/sources/opentile/opentile_image_data.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.0/wsidicomizer/sources/opentile/opentile_source.py` & `wsidicomizer-0.9.1/wsidicomizer/sources/opentile/opentile_source.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.0/wsidicomizer/sources/tiffslide/__init__.py` & `wsidicomizer-0.9.1/wsidicomizer/sources/tiffslide/__init__.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.0/wsidicomizer/sources/tiffslide/tiffslide_image_data.py` & `wsidicomizer-0.9.1/wsidicomizer/sources/tiffslide/tiffslide_image_data.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.0/wsidicomizer/sources/tiffslide/tiffslide_metadata.py` & `wsidicomizer-0.9.1/wsidicomizer/sources/tiffslide/tiffslide_metadata.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.0/wsidicomizer/sources/tiffslide/tiffslide_source.py` & `wsidicomizer-0.9.1/wsidicomizer/sources/tiffslide/tiffslide_source.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.0/wsidicomizer/wsidicomizer.py` & `wsidicomizer-0.9.1/wsidicomizer/wsidicomizer.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.0/PKG-INFO` & `wsidicomizer-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wsidicomizer
-Version: 0.9.0
+Version: 0.9.1
 Summary: Tool for reading WSI files from proprietary formats and optionally convert them to to DICOM
 Home-page: https://github.com/imi-bigpicture/wsidicomizer
 License: Apache-2.0
 Keywords: whole slide image,digital pathology,dicom,converter
 Author: Erik O Gabrielsson
 Author-email: erik.o.gabrielsson@sectra.com
 Requires-Python: >=3.8,<3.12
```

