# Comparing `tmp/napari_spreadsheet-0.0.3.tar.gz` & `tmp/napari_spreadsheet-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari_spreadsheet-0.0.3.tar", last modified: Sun Feb 12 14:54:28 2023, max compression
+gzip compressed data, was "napari_spreadsheet-0.0.4.tar", last modified: Sun Apr 16 03:18:56 2023, max compression
```

## Comparing `napari_spreadsheet-0.0.3.tar` & `napari_spreadsheet-0.0.4.tar`

### file list

```diff
@@ -1,26 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-02-12 14:54:28.596791 napari_spreadsheet-0.0.3/
--rw-rw-rw-   0        0        0     1515 2022-08-14 14:53:05.000000 napari_spreadsheet-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      101 2022-08-14 14:53:05.000000 napari_spreadsheet-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     4273 2023-02-12 14:54:28.597799 napari_spreadsheet-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3131 2023-01-10 06:07:41.000000 napari_spreadsheet-0.0.3/README.md
--rw-rw-rw-   0        0        0      192 2022-08-14 14:53:05.000000 napari_spreadsheet-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0     1553 2023-02-12 14:54:28.607784 napari_spreadsheet-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0       41 2022-08-28 02:06:11.000000 napari_spreadsheet-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-12 14:54:28.457165 napari_spreadsheet-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-02-12 14:54:28.493230 napari_spreadsheet-0.0.3/src/napari_spreadsheet/
--rw-rw-rw-   0        0        0      246 2023-01-10 06:07:43.000000 napari_spreadsheet-0.0.3/src/napari_spreadsheet/__init__.py
--rw-rw-rw-   0        0        0      614 2022-08-15 03:07:53.000000 napari_spreadsheet-0.0.3/src/napari_spreadsheet/_reader.py
-drwxrwxrwx   0        0        0        0 2023-02-12 14:54:28.593785 napari_spreadsheet-0.0.3/src/napari_spreadsheet/_tests/
--rw-rw-rw-   0        0        0        0 2022-08-14 14:53:07.000000 napari_spreadsheet-0.0.3/src/napari_spreadsheet/_tests/__init__.py
--rw-rw-rw-   0        0        0      870 2023-01-10 07:11:09.000000 napari_spreadsheet-0.0.3/src/napari_spreadsheet/_tests/test_widget.py
--rw-rw-rw-   0        0        0      827 2022-08-22 12:01:31.000000 napari_spreadsheet-0.0.3/src/napari_spreadsheet/_types.py
--rw-rw-rw-   0        0        0     1540 2022-08-28 01:39:35.000000 napari_spreadsheet-0.0.3/src/napari_spreadsheet/_utils.py
--rw-rw-rw-   0        0        0     7215 2023-02-12 14:51:54.000000 napari_spreadsheet-0.0.3/src/napari_spreadsheet/_widget.py
--rw-rw-rw-   0        0        0      632 2022-08-15 03:07:21.000000 napari_spreadsheet-0.0.3/src/napari_spreadsheet/napari.yaml
-drwxrwxrwx   0        0        0        0 2023-02-12 14:54:28.587791 napari_spreadsheet-0.0.3/src/napari_spreadsheet.egg-info/
--rw-rw-rw-   0        0        0     4273 2023-02-12 14:54:27.000000 napari_spreadsheet-0.0.3/src/napari_spreadsheet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      632 2023-02-12 14:54:28.000000 napari_spreadsheet-0.0.3/src/napari_spreadsheet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-12 14:54:27.000000 napari_spreadsheet-0.0.3/src/napari_spreadsheet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-02-12 14:54:27.000000 napari_spreadsheet-0.0.3/src/napari_spreadsheet.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      106 2023-02-12 14:54:27.000000 napari_spreadsheet-0.0.3/src/napari_spreadsheet.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-02-12 14:54:27.000000 napari_spreadsheet-0.0.3/src/napari_spreadsheet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 03:18:56.434872 napari_spreadsheet-0.0.4/
+-rw-rw-rw-   0        0        0     1515 2022-08-14 14:53:05.000000 napari_spreadsheet-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      101 2022-08-14 14:53:05.000000 napari_spreadsheet-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     4465 2023-04-16 03:18:56.435868 napari_spreadsheet-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3323 2023-02-16 02:16:02.000000 napari_spreadsheet-0.0.4/README.md
+-rw-rw-rw-   0        0        0      192 2022-08-14 14:53:05.000000 napari_spreadsheet-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0     1553 2023-04-16 03:18:56.438869 napari_spreadsheet-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0       41 2022-08-28 02:06:11.000000 napari_spreadsheet-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 03:18:56.339846 napari_spreadsheet-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-04-16 03:18:56.376841 napari_spreadsheet-0.0.4/src/napari_spreadsheet/
+-rw-rw-rw-   0        0        0      246 2023-01-10 06:07:43.000000 napari_spreadsheet-0.0.4/src/napari_spreadsheet/__init__.py
+-rw-rw-rw-   0        0        0     5310 2023-04-13 12:35:56.000000 napari_spreadsheet-0.0.4/src/napari_spreadsheet/_conversion.py
+-rw-rw-rw-   0        0        0     8176 2023-04-13 14:18:54.000000 napari_spreadsheet-0.0.4/src/napari_spreadsheet/_linker.py
+-rw-rw-rw-   0        0        0      622 2023-04-12 15:27:41.000000 napari_spreadsheet-0.0.4/src/napari_spreadsheet/_reader.py
+drwxrwxrwx   0        0        0        0 2023-04-16 03:18:56.432872 napari_spreadsheet-0.0.4/src/napari_spreadsheet/_tests/
+-rw-rw-rw-   0        0        0        0 2022-08-14 14:53:07.000000 napari_spreadsheet-0.0.4/src/napari_spreadsheet/_tests/__init__.py
+-rw-rw-rw-   0        0        0     2516 2023-04-13 14:19:27.000000 napari_spreadsheet-0.0.4/src/napari_spreadsheet/_tests/test_conversion.py
+-rw-rw-rw-   0        0        0      657 2023-04-12 15:34:14.000000 napari_spreadsheet-0.0.4/src/napari_spreadsheet/_tests/test_reader.py
+-rw-rw-rw-   0        0        0     1523 2023-04-16 02:40:36.000000 napari_spreadsheet-0.0.4/src/napari_spreadsheet/_tests/test_widget.py
+-rw-rw-rw-   0        0        0     1395 2023-04-16 02:40:39.000000 napari_spreadsheet-0.0.4/src/napari_spreadsheet/_types.py
+-rw-rw-rw-   0        0        0     2040 2023-04-16 02:32:01.000000 napari_spreadsheet-0.0.4/src/napari_spreadsheet/_utils.py
+-rw-rw-rw-   0        0        0    12810 2023-04-16 02:41:54.000000 napari_spreadsheet-0.0.4/src/napari_spreadsheet/_widget.py
+-rw-rw-rw-   0        0        0      632 2022-08-15 03:07:21.000000 napari_spreadsheet-0.0.4/src/napari_spreadsheet/napari.yaml
+drwxrwxrwx   0        0        0        0 2023-04-16 03:18:56.420887 napari_spreadsheet-0.0.4/src/napari_spreadsheet.egg-info/
+-rw-rw-rw-   0        0        0     4465 2023-04-16 03:18:56.000000 napari_spreadsheet-0.0.4/src/napari_spreadsheet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      798 2023-04-16 03:18:56.000000 napari_spreadsheet-0.0.4/src/napari_spreadsheet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 03:18:56.000000 napari_spreadsheet-0.0.4/src/napari_spreadsheet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-04-16 03:18:56.000000 napari_spreadsheet-0.0.4/src/napari_spreadsheet.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      106 2023-04-16 03:18:56.000000 napari_spreadsheet-0.0.4/src/napari_spreadsheet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-16 03:18:56.000000 napari_spreadsheet-0.0.4/src/napari_spreadsheet.egg-info/top_level.txt
```

### Comparing `napari_spreadsheet-0.0.3/LICENSE` & `napari_spreadsheet-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `napari_spreadsheet-0.0.3/PKG-INFO` & `napari_spreadsheet-0.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari_spreadsheet
-Version: 0.0.3
+Version: 0.0.4
 Summary: A spreadsheet widget for napari
 Home-page: https://github.com/hanjinliu/napari-spreadsheet
 Author: Hanjin Liu
 Author-email: liuhanjin-sc@g.ecc.u-tokyo.ac.jp
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/hanjinliu/napari-spreadsheet/issues
 Project-URL: Documentation, https://github.com/hanjinliu/napari-spreadsheet#README.md
@@ -37,17 +37,17 @@
 
 ### Highlights
 
 - Convert layer features to a spreadsheet.
 - Update layer features from a spreadsheet.
 - Send spreadsheet data to the namespace of napari's console directly.
 
-![](images/image.png)
+![](https://github.com/hanjinliu/napari-spreadsheet/blob/main/images/image.png)
 
-This plugin is largely dependent on [tabulous](https://github.com/hanjinliu/tabulous).
+This plugin is largely dependent on [tabulous](https://github.com/hanjinliu/tabulous). To know more about the user interface, please see the [documentation](https://hanjinliu.github.io/tabulous/main/user_interface.html).
 
 ----------------------------------
 
 This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
 
 <!--
 Don't miss the full getting started guide to set up your new package:
```

### Comparing `napari_spreadsheet-0.0.3/README.md` & `napari_spreadsheet-0.0.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 
 ### Highlights
 
 - Convert layer features to a spreadsheet.
 - Update layer features from a spreadsheet.
 - Send spreadsheet data to the namespace of napari's console directly.
 
-![](images/image.png)
+![](https://github.com/hanjinliu/napari-spreadsheet/blob/main/images/image.png)
 
-This plugin is largely dependent on [tabulous](https://github.com/hanjinliu/tabulous).
+This plugin is largely dependent on [tabulous](https://github.com/hanjinliu/tabulous). To know more about the user interface, please see the [documentation](https://hanjinliu.github.io/tabulous/main/user_interface.html).
 
 ----------------------------------
 
 This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
 
 <!--
 Don't miss the full getting started guide to set up your new package:
```

### Comparing `napari_spreadsheet-0.0.3/setup.cfg` & `napari_spreadsheet-0.0.4/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206e 6170 6172 695f 7370 7265 6164   = napari_spread
 00000020: 7368 6565 740d 0a76 6572 7369 6f6e 203d  sheet..version =
-00000030: 2030 2e30 2e33 0d0a 6465 7363 7269 7074   0.0.3..descript
+00000030: 2030 2e30 2e34 0d0a 6465 7363 7269 7074   0.0.4..descript
 00000040: 696f 6e20 3d20 4120 7370 7265 6164 7368  ion = A spreadsh
 00000050: 6565 7420 7769 6467 6574 2066 6f72 206e  eet widget for n
 00000060: 6170 6172 690d 0a6c 6f6e 675f 6465 7363  apari..long_desc
 00000070: 7269 7074 696f 6e20 3d20 6669 6c65 3a20  ription = file: 
 00000080: 5245 4144 4d45 2e6d 640d 0a6c 6f6e 675f  README.md..long_
 00000090: 6465 7363 7269 7074 696f 6e5f 636f 6e74  description_cont
 000000a0: 656e 745f 7479 7065 203d 2074 6578 742f  ent_type = text/
@@ -66,15 +66,15 @@
 00000410: 730d 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a  s....[options]..
 00000420: 7061 636b 6167 6573 203d 2066 696e 643a  packages = find:
 00000430: 0d0a 696e 7374 616c 6c5f 7265 7175 6972  ..install_requir
 00000440: 6573 203d 200d 0a09 6d61 6769 6367 7569  es = ...magicgui
 00000450: 0d0a 096e 6170 6172 690d 0a09 6e75 6d70  ...napari...nump
 00000460: 790d 0a09 7061 6e64 6173 0d0a 0971 7470  y...pandas...qtp
 00000470: 790d 0a09 7461 6275 6c6f 7573 3e3d 302e  y...tabulous>=0.
-00000480: 342e 320d 0a70 7974 686f 6e5f 7265 7175  4.2..python_requ
+00000480: 352e 300d 0a70 7974 686f 6e5f 7265 7175  5.0..python_requ
 00000490: 6972 6573 203d 203e 3d33 2e38 0d0a 696e  ires = >=3.8..in
 000004a0: 636c 7564 655f 7061 636b 6167 655f 6461  clude_package_da
 000004b0: 7461 203d 2054 7275 650d 0a70 6163 6b61  ta = True..packa
 000004c0: 6765 5f64 6972 203d 200d 0a09 3d73 7263  ge_dir = ...=src
 000004d0: 0d0a 0d0a 5b6f 7074 696f 6e73 2e70 6163  ....[options.pac
 000004e0: 6b61 6765 732e 6669 6e64 5d0d 0a77 6865  kages.find]..whe
 000004f0: 7265 203d 2073 7263 0d0a 0d0a 5b6f 7074  re = src....[opt
```

### Comparing `napari_spreadsheet-0.0.3/src/napari_spreadsheet/_tests/test_widget.py` & `napari_spreadsheet-0.0.4/src/napari_spreadsheet/_tests/test_widget.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import napari
 
-from napari_spreadsheet import MainWidget
+from napari_spreadsheet import MainWidget, current_widget
 
 
 def test_layer_features(make_napari_viewer):
     viewer: napari.Viewer = make_napari_viewer()
     layer = viewer.add_points(
         [[0, 0], [0, 1], [1, 0]],
         features={"a": [0, 0, 1], "b": ["x", "y", "z"]},
@@ -14,17 +14,38 @@
     wdt.load_layer_features(layer)
     assert wdt._table_viewer.current_table.data.shape == (3, 2)
     wdt._table_viewer.current_table.cell[0, 0] = -1
     wdt.update_layer_features(layer)
     assert layer.features.iloc[0, 0] == -1
 
 
+def test_layer_text(make_napari_viewer):
+    viewer: napari.Viewer = make_napari_viewer()
+    layer = viewer.add_points(
+        [[0, 0], [0, 1], [1, 0]],
+        features={"a": [0, 0, 1], "b": ["x", "y", "z"]},
+        text=["a", "b", "c"],
+    )
+
+    wdt = MainWidget(viewer)
+    wdt.load_layer_text(layer)
+    wdt._table_viewer.current_table.cell[0, 0] = "x"
+    wdt.update_layer_text(layer)
+    assert layer.text.string.array[0] == "x"
+
+
 def test_popup(make_napari_viewer):
     viewer: napari.Viewer = make_napari_viewer()
     wdt = MainWidget(viewer)
     wdt.popup_current_table()
 
 
 def test_open_new_widget(make_napari_viewer):
     viewer: napari.Viewer = make_napari_viewer()
     wdt = MainWidget(viewer)
     wdt.open_new_widget()
+
+
+def test_current_widget(make_napari_viewer):
+    viewer: napari.Viewer = make_napari_viewer()
+    wdt = MainWidget(viewer)
+    assert current_widget() is wdt._table_viewer
```

### Comparing `napari_spreadsheet-0.0.3/src/napari_spreadsheet/_utils.py` & `napari_spreadsheet-0.0.4/src/napari_spreadsheet/_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,56 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Callable
 
 from magicgui.widgets import ComboBox, Dialog, LineEdit
 from qtpy import QtWidgets as QtW
 
-if TYPE_CHECKING:
-    from ._types import LayerWithFeatures
+if TYPE_CHECKING:  # pragma: no cover
+    from napari.layers import Layer
 
 
-def get_str(
+def get_str_by_dialog(
     label: str = "string",
     value: str = "",
     parent: QtW.QWidget | None = None,
 ) -> str | None:
     dlg = Dialog(widgets=[LineEdit(label=label, value=value)])
     dlg.native.setParent(parent, dlg.native.windowFlags())
     if dlg.exec():
         out = dlg[0].value
     else:
         out = None
     return out
 
 
-def get_layer(
-    label: str = "layer",
-    value=None,
+def get_layer_by_dialog(
     parent: QtW.QWidget | None = None,
-) -> LayerWithFeatures | None:
-    from ._types import get_layers_with_features
-
-    cbox = ComboBox(
-        choices=get_layers_with_features, label=label, nullable=False
-    )
+    choices=None,
+) -> Layer | None:
+    cbox = ComboBox(choices=choices, label="Layer", nullable=False)
     dlg = Dialog(widgets=[cbox])
     dlg.native.setParent(parent, dlg.native.windowFlags())
     dlg.reset_choices()
     if dlg.exec():
         out = dlg[0].value
     else:
         out = None
     return out
 
 
+def get_layers(w):
+    from napari.utils._magicgui import find_viewer_ancestor
+
+    viewer = find_viewer_ancestor(w)
+    if viewer is None:
+        return []
+    return list(viewer.layers)
+
+
 def create_button(
     slot: Callable,
     *,
     name: str | None = None,
     tooltip: str | None = None,
 ) -> QtW.QPushButton:
     """Create a QPushButton from a function."""
@@ -54,7 +58,22 @@
         name = slot.__name__
     if tooltip is None and slot.__doc__ is not None:
         tooltip = slot.__doc__.strip()
     btn = QtW.QPushButton(name)
     btn.clicked.connect(lambda: slot())
     btn.setToolTip(tooltip)
     return btn
+
+
+def create_menubutton(
+    name: str,
+    slots: list[tuple[str, Callable]],
+) -> QtW.QPushButton:
+    btn = QtW.QPushButton()
+    btn.setText(name)
+    menu = QtW.QMenu(btn)
+    menu.setToolTipsVisible(True)
+    for slot_name, slot in slots:
+        action = menu.addAction(slot_name, slot)
+        action.setToolTip(slot.__doc__)
+    btn.setMenu(menu)
+    return btn
```

### Comparing `napari_spreadsheet-0.0.3/src/napari_spreadsheet/napari.yaml` & `napari_spreadsheet-0.0.4/src/napari_spreadsheet/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari_spreadsheet-0.0.3/src/napari_spreadsheet.egg-info/PKG-INFO` & `napari_spreadsheet-0.0.4/src/napari_spreadsheet.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-spreadsheet
-Version: 0.0.3
+Version: 0.0.4
 Summary: A spreadsheet widget for napari
 Home-page: https://github.com/hanjinliu/napari-spreadsheet
 Author: Hanjin Liu
 Author-email: liuhanjin-sc@g.ecc.u-tokyo.ac.jp
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/hanjinliu/napari-spreadsheet/issues
 Project-URL: Documentation, https://github.com/hanjinliu/napari-spreadsheet#README.md
@@ -37,17 +37,17 @@
 
 ### Highlights
 
 - Convert layer features to a spreadsheet.
 - Update layer features from a spreadsheet.
 - Send spreadsheet data to the namespace of napari's console directly.
 
-![](images/image.png)
+![](https://github.com/hanjinliu/napari-spreadsheet/blob/main/images/image.png)
 
-This plugin is largely dependent on [tabulous](https://github.com/hanjinliu/tabulous).
+This plugin is largely dependent on [tabulous](https://github.com/hanjinliu/tabulous). To know more about the user interface, please see the [documentation](https://hanjinliu.github.io/tabulous/main/user_interface.html).
 
 ----------------------------------
 
 This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
 
 <!--
 Don't miss the full getting started guide to set up your new package:
```

### Comparing `napari_spreadsheet-0.0.3/src/napari_spreadsheet.egg-info/SOURCES.txt` & `napari_spreadsheet-0.0.4/src/napari_spreadsheet.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 src/napari_spreadsheet/__init__.py
+src/napari_spreadsheet/_conversion.py
+src/napari_spreadsheet/_linker.py
 src/napari_spreadsheet/_reader.py
 src/napari_spreadsheet/_types.py
 src/napari_spreadsheet/_utils.py
 src/napari_spreadsheet/_widget.py
 src/napari_spreadsheet/napari.yaml
 src/napari_spreadsheet.egg-info/PKG-INFO
 src/napari_spreadsheet.egg-info/SOURCES.txt
 src/napari_spreadsheet.egg-info/dependency_links.txt
 src/napari_spreadsheet.egg-info/entry_points.txt
 src/napari_spreadsheet.egg-info/requires.txt
 src/napari_spreadsheet.egg-info/top_level.txt
 src/napari_spreadsheet/_tests/__init__.py
+src/napari_spreadsheet/_tests/test_conversion.py
+src/napari_spreadsheet/_tests/test_reader.py
 src/napari_spreadsheet/_tests/test_widget.py
```

