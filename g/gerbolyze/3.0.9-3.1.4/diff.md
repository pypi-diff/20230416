# Comparing `tmp/gerbolyze-3.0.9.tar.gz` & `tmp/gerbolyze-3.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gerbolyze-3.0.9.tar", last modified: Tue Jun 21 14:25:13 2022, max compression
+gzip compressed data, was "gerbolyze-3.1.4.tar", last modified: Sun Apr 16 18:25:51 2023, max compression
```

## Comparing `gerbolyze-3.0.9.tar` & `gerbolyze-3.1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 bernd     (1000) bernd     (1000)        0 2022-06-21 14:25:13.570882 gerbolyze-3.0.9/
--rw-rw-rw-   0 bernd     (1000) bernd     (1000)    34523 2022-06-21 14:25:07.000000 gerbolyze-3.0.9/LICENSE
--rw-rw-rw-   0 bernd     (1000) bernd     (1000)      490 2022-06-21 14:25:07.000000 gerbolyze-3.0.9/MANIFEST.in
--rw-r--r--   0 bernd     (1000) bernd     (1000)    33449 2022-06-21 14:25:13.569882 gerbolyze-3.0.9/PKG-INFO
--rw-rw-rw-   0 bernd     (1000) bernd     (1000)    31613 2022-06-21 14:25:07.000000 gerbolyze-3.0.9/README.rst
-drwxr-xr-x   0 bernd     (1000) bernd     (1000)        0 2022-06-21 14:25:13.565881 gerbolyze-3.0.9/bin/
--rw-rw-rw-   0 bernd     (1000) bernd     (1000)       92 2022-06-21 14:25:07.000000 gerbolyze-3.0.9/bin/gerbolyze
-drwxr-xr-x   0 bernd     (1000) bernd     (1000)        0 2022-06-21 14:25:13.567881 gerbolyze-3.0.9/gerbolyze/
--rwxrwxrwx   0 bernd     (1000) bernd     (1000)    24207 2022-06-21 14:25:07.000000 gerbolyze-3.0.9/gerbolyze/__init__.py
--rw-rw-rw-   0 bernd     (1000) bernd     (1000)       33 2022-06-21 14:25:07.000000 gerbolyze-3.0.9/gerbolyze/__main__.py
--rw-rw-rw-   0 bernd     (1000) bernd     (1000)    18667 2022-06-21 14:25:07.000000 gerbolyze-3.0.9/gerbolyze/protoboard.py
-drwxr-xr-x   0 bernd     (1000) bernd     (1000)        0 2022-06-21 14:25:13.569882 gerbolyze-3.0.9/gerbolyze/tests/
--rw-rw-rw-   0 bernd     (1000) bernd     (1000)        0 2022-06-21 14:25:07.000000 gerbolyze-3.0.9/gerbolyze/tests/__init__.py
--rw-rw-rw-   0 bernd     (1000) bernd     (1000)     2644 2022-06-21 14:25:07.000000 gerbolyze-3.0.9/gerbolyze/tests/test_integration.py
-drwxr-xr-x   0 bernd     (1000) bernd     (1000)        0 2022-06-21 14:25:13.568882 gerbolyze-3.0.9/gerbolyze.egg-info/
--rw-r--r--   0 bernd     (1000) bernd     (1000)    33449 2022-06-21 14:25:12.000000 gerbolyze-3.0.9/gerbolyze.egg-info/PKG-INFO
--rw-r--r--   0 bernd     (1000) bernd     (1000)      349 2022-06-21 14:25:13.000000 gerbolyze-3.0.9/gerbolyze.egg-info/SOURCES.txt
--rw-r--r--   0 bernd     (1000) bernd     (1000)        1 2022-06-21 14:25:13.000000 gerbolyze-3.0.9/gerbolyze.egg-info/dependency_links.txt
--rw-r--r--   0 bernd     (1000) bernd     (1000)       90 2022-06-21 14:25:13.000000 gerbolyze-3.0.9/gerbolyze.egg-info/requires.txt
--rw-r--r--   0 bernd     (1000) bernd     (1000)       10 2022-06-21 14:25:13.000000 gerbolyze-3.0.9/gerbolyze.egg-info/top_level.txt
--rw-r--r--   0 bernd     (1000) bernd     (1000)       38 2022-06-21 14:25:13.570882 gerbolyze-3.0.9/setup.cfg
--rwxrwxrwx   0 bernd     (1000) bernd     (1000)     2608 2022-06-21 14:25:07.000000 gerbolyze-3.0.9/setup.py
+drwxr-xr-x   0 bernd     (1000) bernd     (1000)        0 2023-04-16 18:25:51.081930 gerbolyze-3.1.4/
+-rw-rw-rw-   0 bernd     (1000) bernd     (1000)    34523 2023-04-16 18:25:47.000000 gerbolyze-3.1.4/LICENSE
+-rw-rw-rw-   0 bernd     (1000) bernd     (1000)      490 2023-04-16 18:25:47.000000 gerbolyze-3.1.4/MANIFEST.in
+-rw-r--r--   0 bernd     (1000) bernd     (1000)    34257 2023-04-16 18:25:51.080930 gerbolyze-3.1.4/PKG-INFO
+-rw-rw-rw-   0 bernd     (1000) bernd     (1000)    32441 2023-04-16 18:25:47.000000 gerbolyze-3.1.4/README.rst
+drwxr-xr-x   0 bernd     (1000) bernd     (1000)        0 2023-04-16 18:25:51.076930 gerbolyze-3.1.4/bin/
+-rw-rw-rw-   0 bernd     (1000) bernd     (1000)       92 2023-04-16 18:25:47.000000 gerbolyze-3.1.4/bin/gerbolyze
+drwxr-xr-x   0 bernd     (1000) bernd     (1000)        0 2023-04-16 18:25:51.077930 gerbolyze-3.1.4/gerbolyze/
+-rwxrwxrwx   0 bernd     (1000) bernd     (1000)    27183 2023-04-16 18:25:47.000000 gerbolyze-3.1.4/gerbolyze/__init__.py
+-rw-rw-rw-   0 bernd     (1000) bernd     (1000)       33 2023-04-16 18:25:47.000000 gerbolyze-3.1.4/gerbolyze/__main__.py
+-rw-rw-rw-   0 bernd     (1000) bernd     (1000)    23446 2023-04-16 18:25:47.000000 gerbolyze-3.1.4/gerbolyze/protoboard.py
+drwxr-xr-x   0 bernd     (1000) bernd     (1000)        0 2023-04-16 18:25:51.080930 gerbolyze-3.1.4/gerbolyze/tests/
+-rw-rw-rw-   0 bernd     (1000) bernd     (1000)        0 2023-04-16 18:25:47.000000 gerbolyze-3.1.4/gerbolyze/tests/__init__.py
+-rw-rw-rw-   0 bernd     (1000) bernd     (1000)     5159 2023-04-16 18:25:47.000000 gerbolyze-3.1.4/gerbolyze/tests/test_integration.py
+drwxr-xr-x   0 bernd     (1000) bernd     (1000)        0 2023-04-16 18:25:51.079930 gerbolyze-3.1.4/gerbolyze.egg-info/
+-rw-r--r--   0 bernd     (1000) bernd     (1000)    34257 2023-04-16 18:25:51.000000 gerbolyze-3.1.4/gerbolyze.egg-info/PKG-INFO
+-rw-r--r--   0 bernd     (1000) bernd     (1000)      349 2023-04-16 18:25:51.000000 gerbolyze-3.1.4/gerbolyze.egg-info/SOURCES.txt
+-rw-r--r--   0 bernd     (1000) bernd     (1000)        1 2023-04-16 18:25:51.000000 gerbolyze-3.1.4/gerbolyze.egg-info/dependency_links.txt
+-rw-r--r--   0 bernd     (1000) bernd     (1000)       66 2023-04-16 18:25:51.000000 gerbolyze-3.1.4/gerbolyze.egg-info/requires.txt
+-rw-r--r--   0 bernd     (1000) bernd     (1000)       10 2023-04-16 18:25:51.000000 gerbolyze-3.1.4/gerbolyze.egg-info/top_level.txt
+-rw-r--r--   0 bernd     (1000) bernd     (1000)       38 2023-04-16 18:25:51.081930 gerbolyze-3.1.4/setup.cfg
+-rwxrwxrwx   0 bernd     (1000) bernd     (1000)     2581 2023-04-16 18:25:48.000000 gerbolyze-3.1.4/setup.py
```

### Comparing `gerbolyze-3.0.9/LICENSE` & `gerbolyze-3.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gerbolyze-3.0.9/PKG-INFO` & `gerbolyze-3.1.4/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: gerbolyze
-Version: 3.0.9
-Summary: A high-resolution image-to-PCB converter. Gerbolyze plots SVG, PNG and JPG onto existing gerber files. It handles almost the full SVG spec and deals with text, path outlines, patterns, arbitrary paths with self-intersections and holes, etc. fully automatically. It can vectorize raster images both by contour tracing and by grayscale dithering. All processing is done at the vector level without intermediate conversions to raster images accurately preserving the input.
-Home-page: https://github.com/jaseg/gerbolyze
-Author: jaseg
-Author-email: gerbonara@jaseg.de
-License: AGPLv3
-Project-URL: Source Code, https://git.jaseg.de/gerbolyze
-Project-URL: Bug Tracker, https://github.com/jaseg/gerbolyze/issues
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Manufacturing
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Religion
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
-Classifier: Natural Language :: English
-Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
-Classifier: Topic :: Utilities
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
 Gerbolyze high-fidelity SVG/PNG/JPG to PCB converter
 ====================================================
 
 .. note::
 
     The command-line usage and SVG template format of gerbolyze changed between v2.0 and v3.0. You can find details on
     the new format below under command_line_usage_
@@ -34,15 +10,17 @@
 Vector data from SVG files is rendered losslessly *without* an intermediate rasterization/revectorization step.
 Still, gerbolyze supports (almost) the full SVG 1.1 spec including complex, self-intersecting paths with holes,
 patterns, dashes and transformations.
 
 Raster images can either be vectorized through contour tracing (like gerbolyze v1.0 did) or they can be embedded using
 high-resolution grayscale emulation while (mostly) guaranteeing trace/space design rules.
 
-.. figure:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.0.9/pics/pcbway_sample_02_small.jpg
+Try gerbolyze online at https://dyna.kokoroyukuma.de/gerboweb
+
+.. figure:: pics/pcbway_sample_02_small.jpg
   :width: 800px
 
   Drawing by `トーコ Toko <https://twitter.com/fluffy2038/status/1317231121269104640>`__ converted using Gerbolyze and printed at PCBWay.
 
 
 Tooling for PCB art is quite limited in both open source and closed source ecosystems. Something as simple as putting a
 pretty picture on a PCB can be an extremely tedious task. Depending on the PCB tool used, various arcane incantations
@@ -54,15 +32,15 @@
 industry-standard Altium Designer. Gerbolyze is written with performance in mind and will happily vectorize tens of
 thousands of primitives, generating tens of megabytes of gerber code without crapping itself. With gerbolyze you can
 finally be confident that your PCB fab's toolchain will fall over before yours does if you overdo it with the high-poly
 anime silkscreen.
 
 Gerbolyze is based on gerbonara_.
 
-.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.0.9/pics/process-overview.png
+.. image:: pics/process-overview.png
   :width: 800px
 
 .. contents::
 
 Tl;dr: Produce high-quality artistic PCBs in three easy steps!
 --------------------------------------------------------------
 
@@ -139,15 +117,15 @@
     python3 setup.py install
 
 Features
 --------
 
 Input on the left, output on the right.
 
-.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.0.9/pics/test_svg_readme_composited.png
+.. image:: pics/test_svg_readme_composited.png
   :width: 800px
 
 * Almost full SVG 1.1 static spec coverage (!)
 
   * Paths with beziers, self-intersections and holes
   * Strokes, even with dashes and markers
   * Pattern fills and strokes
@@ -204,14 +182,24 @@
     * apply pattern fills
     * clip to clip-path
     * remove holes using Clipper
 
 * for KiCAD S-Expression export: vector-composite results using CavalierContours: subtract each clear output primitive
   from all previous dark output primitives
 
+Web interface
+-------------
+
+You can try gerbolyze online at https://dyna.kokoroyukuma.de/gerboweb
+
+The web interface does not expose all of gerbolyze's bells and whistles, but it allows you to simply paste a single SVG
+file on a board to try out gerbolyze. Upload your design on the web interface, then download the template for either the
+top or bottom side, and put your artwork on the appropriate layer of that template using Inkscape_. Finally, upload the
+modified template and let gerbolyze process your design.
+
 Command-line usage
 ------------------
 .. _command_line_usage:
 
 Generate SVG template from Gerber files:
 
 .. code-block:: shell
@@ -339,15 +327,15 @@
 Dashed strokes are supported on outline layers and can be used to make easy mouse bites.
 
 .. _subtraction_script:
 
 Subtraction scripts
 *******************
 
-.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.0.9/pics/subtract_example.png
+.. image:: pics/subtract_example.png
   :width: 800px
 
 Subtraction scripts tell ``gerbolyze paste`` to remove an area around certain input layers to from an overlay layer.
 When a input layer is given in the subtraction script, gerbolyze will dilate (extend outwards) everything on this input
 layer and remove it from the target overlay layer. By default, Gerbolyze subtracts the mask layer from the silk layer to
 make sure there are no silk primitives that overlap bare copper, and subtracts each input layer from its corresponding
 overlay to make sure the two do not overlap. In the picture above you can see both at work: The overlay contains
@@ -492,33 +480,33 @@
 
 .. for f in vec_*.png; convert -background white -gravity center $f -resize 500x500 -extent 500x500 (basename -s .png $f)-square.png; end
 .. for vec in hexgrid square poisson contours; convert vec_"$vec"_whole-square.png vec_"$vec"_detail-square.png -background transparent -splice 25x0+0+0 +append -chop 25x0+0+0 vec_"$vec"_composited.png; end
 
 ``--vectorizer poisson-disc`` (the default) 
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.0.9/pics/vec_poisson_composited.png
+.. image:: pics/vec_poisson_composited.png
   :width: 800px
 
 ``--vectorizer hex-grid``
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
-.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.0.9/pics/vec_hexgrid_composited.png
+.. image:: pics/vec_hexgrid_composited.png
   :width: 800px
 
 ``--vectorizer square-grid``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.0.9/pics/vec_square_composited.png
+.. image:: pics/vec_square_composited.png
   :width: 800px
 
 ``--vectorizer binary-contours``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.0.9/pics/vec_contours_composited.png
+.. image:: pics/vec_contours_composited.png
   :width: 800px
 
 The binary contours vectorizer requires a black-and-white binary input image. As you can see, like every bitmap tracer
 it will produce some artifacts. For artistic input this is usually not too bad as long as the input data is
 high-resolution. Antialiased edges in the input image are not only OK, they may even help with an accurate
 vectorization.
 
@@ -688,17 +676,20 @@
 
 A design rule checker is planned as a future addition to gerbolyze, but is not yet part of it. If in doubt, talk to your
 fab and consider doing a test run of your design before ordering assembled boards ;)
 
 Gallery
 -------
 
-.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.0.9/pics/sample3.jpg
+.. image:: pics/sample3.jpg
   :width: 400px
 
+For a demonstration of ``gerbolyze convert``, check out the `Gerbolyze Protoboard Index`_, where you can download gerber
+files for over 7.000 SMD and THT protoboard layouts.
+
 Licensing
 ---------
 
 This tool is licensed under the rather radical AGPLv3 license. Briefly, this means that you have to provide users of a
 webapp using this tool in the backend with this tool's source.
 
 I get that some people have issues with the AGPL. In case this license prevents you from using this software, please
@@ -709,9 +700,9 @@
 
 .. _usvg: https://github.com/RazrFalcon/resvg
 .. _Inkscape: https://inkscape.org/
 .. _pcb-tools: https://github.com/curtacircuitos/pcb-tools
 .. _pcb-tools-extension: https://github.com/opiopan/pcb-tools-extension
 .. _GIMP: https://gimp.org/
 .. _gerbonara: https://gitlab.com/gerbolyze/gerbonara
-
+.. _`Gerbolyze Protoboard Index`: https://dyna.kokoroyukuma.de/protos/
```

### Comparing `gerbolyze-3.0.9/README.rst` & `gerbolyze-3.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+Metadata-Version: 2.1
+Name: gerbolyze
+Version: 3.1.4
+Summary: A high-resolution image-to-PCB converter. Gerbolyze plots SVG, PNG and JPG onto existing gerber files. It handles almost the full SVG spec and deals with text, path outlines, patterns, arbitrary paths with self-intersections and holes, etc. fully automatically. It can vectorize raster images both by contour tracing and by grayscale dithering. All processing is done at the vector level without intermediate conversions to raster images accurately preserving the input.
+Home-page: https://github.com/jaseg/gerbolyze
+Author: jaseg
+Author-email: gerbonara@jaseg.de
+License: AGPLv3
+Project-URL: Source Code, https://git.jaseg.de/gerbolyze
+Project-URL: Bug Tracker, https://github.com/jaseg/gerbolyze/issues
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Manufacturing
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Religion
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
+Classifier: Natural Language :: English
+Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
+Classifier: Topic :: Utilities
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
 Gerbolyze high-fidelity SVG/PNG/JPG to PCB converter
 ====================================================
 
 .. note::
 
     The command-line usage and SVG template format of gerbolyze changed between v2.0 and v3.0. You can find details on
     the new format below under command_line_usage_
@@ -10,15 +33,17 @@
 Vector data from SVG files is rendered losslessly *without* an intermediate rasterization/revectorization step.
 Still, gerbolyze supports (almost) the full SVG 1.1 spec including complex, self-intersecting paths with holes,
 patterns, dashes and transformations.
 
 Raster images can either be vectorized through contour tracing (like gerbolyze v1.0 did) or they can be embedded using
 high-resolution grayscale emulation while (mostly) guaranteeing trace/space design rules.
 
-.. figure:: pics/pcbway_sample_02_small.jpg
+Try gerbolyze online at https://dyna.kokoroyukuma.de/gerboweb
+
+.. figure:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.1.4/pics/pcbway_sample_02_small.jpg
   :width: 800px
 
   Drawing by `トーコ Toko <https://twitter.com/fluffy2038/status/1317231121269104640>`__ converted using Gerbolyze and printed at PCBWay.
 
 
 Tooling for PCB art is quite limited in both open source and closed source ecosystems. Something as simple as putting a
 pretty picture on a PCB can be an extremely tedious task. Depending on the PCB tool used, various arcane incantations
@@ -30,15 +55,15 @@
 industry-standard Altium Designer. Gerbolyze is written with performance in mind and will happily vectorize tens of
 thousands of primitives, generating tens of megabytes of gerber code without crapping itself. With gerbolyze you can
 finally be confident that your PCB fab's toolchain will fall over before yours does if you overdo it with the high-poly
 anime silkscreen.
 
 Gerbolyze is based on gerbonara_.
 
-.. image:: pics/process-overview.png
+.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.1.4/pics/process-overview.png
   :width: 800px
 
 .. contents::
 
 Tl;dr: Produce high-quality artistic PCBs in three easy steps!
 --------------------------------------------------------------
 
@@ -115,15 +140,15 @@
     python3 setup.py install
 
 Features
 --------
 
 Input on the left, output on the right.
 
-.. image:: pics/test_svg_readme_composited.png
+.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.1.4/pics/test_svg_readme_composited.png
   :width: 800px
 
 * Almost full SVG 1.1 static spec coverage (!)
 
   * Paths with beziers, self-intersections and holes
   * Strokes, even with dashes and markers
   * Pattern fills and strokes
@@ -180,14 +205,24 @@
     * apply pattern fills
     * clip to clip-path
     * remove holes using Clipper
 
 * for KiCAD S-Expression export: vector-composite results using CavalierContours: subtract each clear output primitive
   from all previous dark output primitives
 
+Web interface
+-------------
+
+You can try gerbolyze online at https://dyna.kokoroyukuma.de/gerboweb
+
+The web interface does not expose all of gerbolyze's bells and whistles, but it allows you to simply paste a single SVG
+file on a board to try out gerbolyze. Upload your design on the web interface, then download the template for either the
+top or bottom side, and put your artwork on the appropriate layer of that template using Inkscape_. Finally, upload the
+modified template and let gerbolyze process your design.
+
 Command-line usage
 ------------------
 .. _command_line_usage:
 
 Generate SVG template from Gerber files:
 
 .. code-block:: shell
@@ -315,15 +350,15 @@
 Dashed strokes are supported on outline layers and can be used to make easy mouse bites.
 
 .. _subtraction_script:
 
 Subtraction scripts
 *******************
 
-.. image:: pics/subtract_example.png
+.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.1.4/pics/subtract_example.png
   :width: 800px
 
 Subtraction scripts tell ``gerbolyze paste`` to remove an area around certain input layers to from an overlay layer.
 When a input layer is given in the subtraction script, gerbolyze will dilate (extend outwards) everything on this input
 layer and remove it from the target overlay layer. By default, Gerbolyze subtracts the mask layer from the silk layer to
 make sure there are no silk primitives that overlap bare copper, and subtracts each input layer from its corresponding
 overlay to make sure the two do not overlap. In the picture above you can see both at work: The overlay contains
@@ -468,33 +503,33 @@
 
 .. for f in vec_*.png; convert -background white -gravity center $f -resize 500x500 -extent 500x500 (basename -s .png $f)-square.png; end
 .. for vec in hexgrid square poisson contours; convert vec_"$vec"_whole-square.png vec_"$vec"_detail-square.png -background transparent -splice 25x0+0+0 +append -chop 25x0+0+0 vec_"$vec"_composited.png; end
 
 ``--vectorizer poisson-disc`` (the default) 
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-.. image:: pics/vec_poisson_composited.png
+.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.1.4/pics/vec_poisson_composited.png
   :width: 800px
 
 ``--vectorizer hex-grid``
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
-.. image:: pics/vec_hexgrid_composited.png
+.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.1.4/pics/vec_hexgrid_composited.png
   :width: 800px
 
 ``--vectorizer square-grid``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-.. image:: pics/vec_square_composited.png
+.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.1.4/pics/vec_square_composited.png
   :width: 800px
 
 ``--vectorizer binary-contours``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-.. image:: pics/vec_contours_composited.png
+.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.1.4/pics/vec_contours_composited.png
   :width: 800px
 
 The binary contours vectorizer requires a black-and-white binary input image. As you can see, like every bitmap tracer
 it will produce some artifacts. For artistic input this is usually not too bad as long as the input data is
 high-resolution. Antialiased edges in the input image are not only OK, they may even help with an accurate
 vectorization.
 
@@ -664,17 +699,20 @@
 
 A design rule checker is planned as a future addition to gerbolyze, but is not yet part of it. If in doubt, talk to your
 fab and consider doing a test run of your design before ordering assembled boards ;)
 
 Gallery
 -------
 
-.. image:: pics/sample3.jpg
+.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.1.4/pics/sample3.jpg
   :width: 400px
 
+For a demonstration of ``gerbolyze convert``, check out the `Gerbolyze Protoboard Index`_, where you can download gerber
+files for over 7.000 SMD and THT protoboard layouts.
+
 Licensing
 ---------
 
 This tool is licensed under the rather radical AGPLv3 license. Briefly, this means that you have to provide users of a
 webapp using this tool in the backend with this tool's source.
 
 I get that some people have issues with the AGPL. In case this license prevents you from using this software, please
@@ -685,8 +723,8 @@
 
 .. _usvg: https://github.com/RazrFalcon/resvg
 .. _Inkscape: https://inkscape.org/
 .. _pcb-tools: https://github.com/curtacircuitos/pcb-tools
 .. _pcb-tools-extension: https://github.com/opiopan/pcb-tools-extension
 .. _GIMP: https://gimp.org/
 .. _gerbonara: https://gitlab.com/gerbolyze/gerbonara
-
+.. _`Gerbolyze Protoboard Index`: https://dyna.kokoroyukuma.de/protos/
```

### Comparing `gerbolyze-3.0.9/gerbolyze/__init__.py` & `gerbolyze-3.1.4/gerbolyze/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 import tempfile
+import logging
 import os.path as path
 from pathlib import Path
+import shlex
 import textwrap
 import subprocess
 import functools
 import os
 import base64
 import re
 import sys
 import warnings
 import shutil
 from zipfile import ZipFile, is_zipfile
+from pathlib import Path
 
-from lxml import etree
+from bs4 import BeautifulSoup
 import numpy as np
 import click
 
 import gerbonara as gn
 
+__version__ = '3.1.4'
+
 @click.group()
 def cli():
     pass
 
 @cli.command()
 @click.argument('input_gerbers', type=click.Path(exists=True, path_type=Path))
 @click.argument('input_svg', type=click.Path(exists=True, dir_okay=False, file_okay=True, allow_dash=True, path_type=Path))
@@ -30,69 +35,103 @@
 @click.option('--zip/--no-zip', 'is_zip', default=None, help='zip output files. Default: zip if output path ends with ".zip" or when outputting to stdout.')
 @click.option('--curve-tolerance', type=float, help='Tolerance for curve flattening in mm')
 @click.option('--no-subtract', 'no_subtract', flag_value=True, help='Disable subtraction')
 @click.option('--subtract', help='Use user subtraction script from argument')
 @click.option('--trace-space', type=float, default=0.1, help='passed through to svg-flatten')
 @click.option('--vectorizer', help='passed through to svg-flatten')
 @click.option('--vectorizer-map', help='passed through to svg-flatten')
+@click.option('--excellon-conversion-errors', type=click.Choice(['raise', 'warn', 'ignore']), default='raise', help='Method of error handling during SVG to Excellon conversion')
 @click.option('--preserve-aspect-ratio', help='PNG/JPG files only: passed through to svg-flatten')
 @click.option('--exclude-groups', help='passed through to svg-flatten')
+@click.option('--circle-test-tolerance', help='passed through to svg-flatten')
+@click.option('--log-level', default='info', type=click.Choice(['debug', 'info', 'warning', 'error', 'critical']), help='log level')
 def paste(input_gerbers, input_svg, output_gerbers, is_zip,
         dilate, curve_tolerance, no_subtract, subtract,
-        preserve_aspect_ratio,
-        trace_space, vectorizer, vectorizer_map, exclude_groups):
+        preserve_aspect_ratio, circle_test_tolerance,
+        trace_space, vectorizer, vectorizer_map, exclude_groups,
+        excellon_conversion_errors, log_level):
     """ Render vector data and raster images from SVG file into gerbers. """
 
+    logging.basicConfig(level=getattr(logging, log_level.upper()))
+
     subtract_map = parse_subtract_script('' if no_subtract else subtract, dilate)
 
     stack = gn.LayerStack.open(input_gerbers, lazy=True)
     (bb_min_x, bb_min_y), (bb_max_x, bb_max_y) = bounds = stack.board_bounds()
 
-    output_is_zip = output_gerbers.lower().endswith('.zip') if is_zip is None else is_zip
+    output_is_zip = output_gerbers.name.lower().endswith('.zip') if is_zip is None else is_zip
 
     # Create output dir if it does not exist yet. Do this now so we fail early
     if not output_is_zip:
         output_gerbers.mkdir(exist_ok=True)
 
     @functools.lru_cache()
     def do_dilate(layer, amount):
         return dilate_gerber(layer, bounds, amount, curve_tolerance)
-    
-    for (side, use), layer in stack.graphic_layers.items():
-        overlay_grb = svg_to_gerber(input_svg,
-                trace_space=trace_space, vectorizer=vectorizer, vectorizer_map=vectorizer_map,
-                exclude_groups=exclude_groups, curve_tolerance=curve_tolerance,
-                preserve_aspect_ratio=preserve_aspect_ratio,
-                outline_mode=(use == 'outline'),
-                only_groups=f'g-{side}-{use}')
 
-        if not overlay_grb:
-            print(f'Overlay {side} {use} layer is empty. Skipping.')
-            continue
+    with tempfile.NamedTemporaryFile(suffix='.svg') as processed_svg:
+        run_cargo_command('usvg', *shlex.split(os.environ.get('USVG_OPTIONS', '')), input_svg, processed_svg.name)
 
-        # only open lazily loaded layer if we need it. Replace lazy wrapper in stack with loaded layer.
-        stack.graphic_layers[(side, use)] = layer = layer.instance
-
-        # move overlay from svg origin to gerber origin
-        overlay_grb.offset(bb_min_x, bb_min_y)
+        with open(processed_svg.name) as f:
+            soup = BeautifulSoup(f.read(), features='xml')
+    
+        for (side, use), layer in [
+                *stack.graphic_layers.items(),
+                (('drill', 'plated'), stack.drill_pth),
+                (('drill', 'nonplated'), stack.drill_npth)]:
+            logging.info(f'Layer {side} {use}')
+            if (soup_layer := soup.find(id=f'g-{side}-{use}')):
+                if not soup_layer.contents:
+                    logging.info(f'    Corresponding overlay layer is empty. Skipping.')
+            else:
+                logging.info(f'    Corresponding overlay layer not found. Skipping.')
+                continue
 
-        # dilated subtract layers on top of overlay
-        if side in ('top', 'bottom'): # do not process subtraction scripts for inner layers
-            dilations = subtract_map.get(use, [])
-            for d_layer, amount in dilations:
-                dilated = do_dilate(stack[(side, d_layer)], amount)
-                layer.merge(dilated, mode='below', keep_settings=True)
+            if layer is None:
+                loggin.error(f'    Corresponding overlay layer is non-empty, but the corresponding layer could not be found in the input gerbers. Skipping.')
+                continue
+            
+            # only open lazily loaded layer if we need it. Replace lazy wrapper in stack with loaded layer.
+            layer = layer.instance
+            logging.info(f'    Loaded layer: {layer}')
+
+            overlay_grb = svg_to_gerber(processed_svg.name, no_usvg=True,
+                    trace_space=trace_space, vectorizer=vectorizer, vectorizer_map=vectorizer_map,
+                    exclude_groups=exclude_groups, curve_tolerance=curve_tolerance,
+                    preserve_aspect_ratio=preserve_aspect_ratio, circle_test_tolerance=circle_test_tolerance,
+                    outline_mode=(use == 'outline' or side == 'drill'),
+                    only_groups=f'g-{side}-{use}')
+
+            logging.info(f'    Converted overlay: {overlay_grb}')
+
+            # move overlay from svg origin to gerber origin
+            overlay_grb.offset(bb_min_x, bb_min_y)
+
+            # dilated subtract layers on top of overlay
+            if side in ('top', 'bottom'): # do not process subtraction scripts for inner layers, outline, and drill files
+                dilations = subtract_map.get(use, [])
+                for d_layer, amount in dilations:
+                    dilated = do_dilate(stack[(side, d_layer)], amount)
+                    layer.merge(dilated, mode='below', keep_settings=True)
 
-        # overlay on bottom
-        layer.merge(overlay_grb, mode='below', keep_settings=True)
+            if side == 'drill':
+                try:
+                    overlay_grb = overlay_grb.to_excellon(plated=layer.is_plated_tristate,
+                                                          errors=excellon_conversion_errors)
+                except ValueError as e:
+                    raise click.ClickException(f'Some objects on the {use} drill layer could not be converted from SVG to Excellon. This may be because they are not sufficiently circular to be matched. You can either increase the --circle-test-tolerance parameter from its default value of 0.1, or you can convert this error into a warning by passing --excellon-conversion-errors "warn" or "ignore".') from e
+
+            # overlay on bottom
+            layer.merge(overlay_grb, mode='below', keep_settings=True)
+            logging.info(f'    Merged layer and overlay: {layer}')
 
-    if output_is_zip:
-        stack.save_to_zipfile(output_gerbers)
-    else:
-        stack.save_to_directory(output_gerbers)
+        if output_is_zip:
+            stack.save_to_zipfile(output_gerbers)
+        else:
+            stack.save_to_directory(output_gerbers)
 
 @cli.command()
 @click.argument('input_gerbers', type=click.Path(exists=True))
 @click.argument('output_svg', required=False)
 @click.option('-t' ,'--top', help='Render board top side.', is_flag=True)
 @click.option('-b' ,'--bottom', help='Render board bottom side.', is_flag=True)
 @click.option('-f' ,'--force', help='Overwrite existing output file when autogenerating file name.', is_flag=True)
@@ -124,37 +163,38 @@
 
     else:
         output_svg = Path(output_svg)
 
     stack = gn.LayerStack.open(source, lazy=True)
     svg = stack.to_pretty_svg(side=('top' if top else 'bottom'), inkscape=True)
 
-    template_layers = [ f'{ttype}-{use}' for use in [ 'copper', 'mask', 'silk' ] ] + ['mechanical outline']
+    template_layers = [f'{ttype}-copper', f'{ttype}-mask', f'{ttype}-silk', f'{ttype}-paste',
+                       'mechanical outline', 'drill plated', 'drill nonplated']
     silk = template_layers[-2]
 
     if vector:
         output_svg.write_text(create_template_from_svg(svg, template_layers, current_layer=silk))
 
     else:
         with tempfile.NamedTemporaryFile(suffix='.svg') as temp_svg, \
             tempfile.NamedTemporaryFile(suffix='.png') as temp_png:
             Path(temp_svg.name).write_text(str(svg))
-            run_resvg(temp_svg.name, temp_png.name, dpi=f'{raster_dpi:.0f}')
+            run_cargo_command('resvg', temp_svg.name, temp_png.name, dpi=f'{raster_dpi:.0f}')
             output_svg.write_text(template_svg_for_png(stack.board_bounds(), Path(temp_png.name).read_bytes(),
                 template_layers, current_layer=silk))
 
 
 class ClickSizeParam(click.ParamType):
     name = 'Size'
 
     def convert(self, value, param, ctx):
         if isinstance(value, tuple):
             return value
 
-        if not (m := re.match('([0-9]+\.?[0-9]*)(mm|cm|in)?[xX*/,×]([0-9]+\.?[0-9]*)(mm|cm|in)?', value)):
+        if not (m := re.match(r'([0-9]+\.?[0-9]*)(mm|cm|in)?[xX*/,×]([0-9]+\.?[0-9]*)(mm|cm|in)?', value)):
             self.fail('Size must have format [width]x[height][unit]. The unit can be mm, cm or in. The unit is optional and defaults to mm.', param=param, ctx=ctx)
 
         w, unit1, h, unit2 = m.groups()
         if unit1 and unit2 and unit1 != unit2:
             self.fail('Width and height must use the same unit. Two different units given for width and height: width is in {unit1}, and height is in {unit2}.', param=param, ctx=ctx)
 
         unit = (unit1 or unit2) or 'mm'
@@ -184,111 +224,123 @@
 
         if copper_layers > 0:
             current_layer = 'top copper'
             inner = [ 'inner{i} copper' for i in range(max(0, copper_layers-2)) ]
             layers += ['top copper', *inner, 'bottom copper'][:copper_layers]
 
         layers += ['bottom mask', 'bottom silk', 'bottom paste']
-        layers += ['outline', 'plated drill', 'nonplated drill', 'comments']
+        layers += ['mechanical outline', 'drill plated', 'drill nonplated', 'other comments']
     if layers and current_layer is None:
         current_layer = layers[0]
 
     out.write(empty_pcb_template(size, layers, current_layer))
     out.flush()
     if output_svg != '-':
         out.close()
 
 
 @cli.command()
 @click.argument('input_svg', type=click.Path(exists=True, path_type=Path))
 @click.argument('output_gerbers', type=click.Path(path_type=Path))
 @click.option('-n', '--naming-scheme', default='kicad', type=click.Choice(['kicad', 'altium']), help='Naming scheme for gerber output file names.')
 @click.option('--zip/--no-zip', 'is_zip', default=None, help='zip output files. Default: zip if output path ends with ".zip" or when outputting to stdout.')
-@click.option('--separate-drill-file/--composite-drill-file', 'separate_drill', help='Use Altium composite Excellon drill file format (default)')
+@click.option('--composite-drill-file/--separate-drill-file', 'composite_drill', help='Use Altium composite Excellon drill file format (default)')
 @click.option('--dilate', default=0.1, type=float, help='Default dilation for subtraction operations in mm')
 @click.option('--curve-tolerance', type=float, help='Tolerance for curve flattening in mm')
-@click.option('--no-subtract', 'no_subtract', flag_value=True, help='Disable subtraction')
-@click.option('--subtract', help='Use user subtraction script from argument (see description above)')
+@click.option('--subtract', help='Use user subtraction script from argument (default for "convert": none)')
 @click.option('--trace-space', type=float, default=0.1, help='passed through to svg-flatten')
 @click.option('--vectorizer', help='passed through to svg-flatten')
 @click.option('--vectorizer-map', help='passed through to svg-flatten')
 @click.option('--exclude-groups', help='passed through to svg-flatten')
+@click.option('--circle-test-tolerance', help='passed through to svg-flatten')
 @click.option('--pattern-complete-tiles-only', is_flag=True, help='passed through to svg-flatten')
 @click.option('--use-apertures-for-patterns', is_flag=True, help='passed through to svg-flatten')
-def convert(input_svg, output_gerbers, is_zip, dilate, curve_tolerance, no_subtract, subtract, trace_space, vectorizer,
-        vectorizer_map, exclude_groups, separate_drill, naming_scheme,
-        pattern_complete_tiles_only, use_apertures_for_patterns):
+@click.option('--log-level', default='info', type=click.Choice(['debug', 'info', 'warning', 'error', 'critical']), help='log level')
+def convert(input_svg, output_gerbers, is_zip, dilate, curve_tolerance, subtract, trace_space, vectorizer,
+        vectorizer_map, exclude_groups, composite_drill, naming_scheme, circle_test_tolerance,
+        pattern_complete_tiles_only, use_apertures_for_patterns, log_level):
     ''' Convert SVG file directly to gerbers.
 
     Unlike `gerbolyze paste`, this does not add the SVG's contents to existing gerbers. It allows you to directly create
     PCBs using Inkscape similar to PCBModE.
     '''
+    logging.basicConfig(level=getattr(logging, log_level.upper()))
 
-    subtract_map = parse_subtract_script('' if no_subtract else subtract, dilate, default_script=DEFAULT_CONVERT_SUB_SCRIPT)
+    subtract_map = parse_subtract_script(subtract, dilate, default_script='')
     output_is_zip = output_gerbers.name.lower().endswith('.zip') if is_zip is None else is_zip
 
-    stack = gn.LayerStack({}, [], board_name=input_svg.stem, original_path=input_svg)
+    with tempfile.NamedTemporaryFile(suffix='.svg') as processed_svg:
+        run_cargo_command('usvg', *shlex.split(os.environ.get('USVG_OPTIONS', '')), input_svg, processed_svg.name)
 
-    for group_id, label in get_layers_from_svg(input_svg.read_text()):
-        if not group_id or not label or 'no export' in label:
-            continue
+        soup = BeautifulSoup(input_svg.read_text(), features='xml')
+        layers = {e.get('id'): e.get('inkscape:label') for e in soup.find_all('g', recursive=True)}
 
-        if label == 'outline':
-            side, use = 'mechanical', 'outline'
-        elif label == 'comments':
-            side, use = 'other', 'comments'
-        elif len(label.split()) != 2:
-            warnings.warn('Unknown layer {label}')
-            continue
-        else:
-            side, use = label.split()
+        stack = gn.LayerStack({}, None, None, [], board_name=input_svg.stem, original_path=input_svg)
 
-        grb = svg_to_gerber(input_svg,
-                trace_space=trace_space, vectorizer=vectorizer, vectorizer_map=vectorizer_map,
-                exclude_groups=exclude_groups, curve_tolerance=curve_tolerance, only_groups=group_id,
-                pattern_complete_tiles_only=pattern_complete_tiles_only,
-                use_apertures_for_patterns=(use_apertures_for_patterns and use not in ('outline', 'drill')),
-                outline_mode=(use == 'outline' or use == 'drill'))
-        grb.original_path = Path()
-
-        if use == 'drill':
-            if side == 'plated':
-                stack.drill_pth = grb.to_excellon(plated=True)
-            elif side == 'nonplated':
-                stack.drill_npth = grb.to_excellon(plated=False)
-            else:
-                warnings.warn(f'Invalid drill layer type "{side}". Must be one of "plated" or "nonplated"')
+        for group_id, label in layers.items():
+            label = label or ''
+            if not group_id or 'no export' in label:
+                continue
 
-        else:
-            stack.graphic_layers[(side, use)] = grb
+            if not group_id.startswith('g-'):
+                continue
+            group_id = group_id[2:]
 
-    bounds = stack.board_bounds()
-    @functools.lru_cache()
-    def do_dilate(layer, amount):
-        return dilate_gerber(layer, bounds, amount, curve_tolerance)
+            if group_id == 'outline':
+                side, use = 'mechanical', 'outline'
+            elif group_id == 'comments':
+                side, use = 'other', 'comments'
+            elif len(group_id.split('-')) != 2:
+                warnings.warn(f'Unknown layer {group_id}')
+                continue
+            else:
+                side, use = group_id.split('-')
 
-    for (side, use), layer in stack.graphic_layers.items():
-        # dilated subtract layers on top of overlay
-        if side in ('top', 'bottom'): # do not process subtraction scripts for inner layers
-            dilations = subtract_map.get(use, [])
-            for d_layer, amount in dilations:
-                d_layer =  stack.graphic_layers[(side, d_layer)]
-                dilated = do_dilate(d_layer, amount)
-                layer.merge(dilated, mode='above', keep_settings=True)
-
-    if not separate_drill:
-        print('Merging drill layers...')
-        stack.merge_drill_layers()
-
-    naming_scheme = getattr(gn.layers.NamingScheme, naming_scheme)
-    if output_is_zip:
-        stack.save_to_zipfile(output_gerbers, naming_scheme=naming_scheme)
-    else:
-        stack.save_to_directory(output_gerbers, naming_scheme=naming_scheme)
+            grb = svg_to_gerber(processed_svg.name, no_usvg=True,
+                    trace_space=trace_space, vectorizer=vectorizer, vectorizer_map=vectorizer_map,
+                    exclude_groups=exclude_groups, curve_tolerance=curve_tolerance, only_groups=f'g-{group_id}',
+                    circle_test_tolerance=circle_test_tolerance, pattern_complete_tiles_only=pattern_complete_tiles_only,
+                    use_apertures_for_patterns=(use_apertures_for_patterns and use not in ('outline', 'drill')),
+                    outline_mode=(use == 'outline' or side == 'drill'))
+            grb.original_path = Path()
+
+            if side == 'drill':
+                if use == 'plated':
+                    stack.drill_pth = grb.to_excellon(plated=True)
+                elif use == 'nonplated':
+                    stack.drill_npth = grb.to_excellon(plated=False)
+                else:
+                    warnings.warn(f'Invalid drill layer type "{side}". Must be one of "plated" or "nonplated"')
 
+            else:
+                stack.graphic_layers[(side, use)] = grb
+
+        bounds = stack.board_bounds()
+        @functools.lru_cache()
+        def do_dilate(layer, amount):
+            return dilate_gerber(layer, bounds, amount, curve_tolerance)
+
+        for (side, use), layer in stack.graphic_layers.items():
+            # dilated subtract layers on top of overlay
+            if side in ('top', 'bottom'): # do not process subtraction scripts for inner layers
+                dilations = subtract_map.get(use, [])
+                for d_layer, amount in dilations:
+                    d_layer =  stack.graphic_layers[(side, d_layer)]
+                    dilated = do_dilate(d_layer, amount)
+                    layer.merge(dilated, mode='above', keep_settings=True)
+
+        if composite_drill:
+            logging.info('Merging drill layers...')
+            stack.merge_drill_layers()
+
+        naming_scheme = getattr(gn.layers.NamingScheme, naming_scheme)
+        if output_is_zip:
+            stack.save_to_zipfile(output_gerbers, naming_scheme=naming_scheme)
+        else:
+            stack.save_to_directory(output_gerbers, naming_scheme=naming_scheme)
 
 
 # Subtraction script handling
 #============================
 
 DEFAULT_SUB_SCRIPT = '''
 out.silk -= in.mask
@@ -309,15 +361,15 @@
     lines = script.replace(';', '\n').splitlines()
     for line in lines:
         line = line.strip()
         if not line or line.startswith('#'):
             continue
 
         line = line.lower()
-        line = re.sub('\s', '', line)
+        line = re.sub(r'\s', '', line)
 
         # out.copper -= in.copper+0.1
         varname = r'([a-z]+\.[a-z]+)'
         floatnum = r'([+-][.0-9]+)'
         match = re.fullmatch(fr'{varname}-={varname}{floatnum}?', line)
         if not match:
             raise ValueError(f'Cannot parse line: {line}')
@@ -330,82 +382,58 @@
         _in, _, in_layer = in_var.partition('.')
 
         dilation = float(dilation) if dilation else default_dilation
 
         subtract_script[out_layer] = subtract_script.get(out_layer, []) + [(in_layer, dilation)]
     return subtract_script
 
-# Parameter parsing foo
-#======================
-
-def parse_bbox(bbox):
-    if not bbox:
-        return None
-    elems = [ int(elem) for elem in re.split('[,/ ]', bbox) ]
-    if len(elems) not in (2, 4):
-        raise click.BadParameter(
-                '--bbox must be either two floating-point values like: w,h or four like: x,y,w,h')
-
-    elems = [ float(e) for e in elems ]
-
-    if len(elems) == 2:
-        bounds = [0, 0, *elems]
-    else:
-        bounds = elems
-    
-    # now transform bounds to the format pcb-tools uses. Instead of (x, y, w, h) or even (x1, y1, x2, y2), that
-    # is ((x1, x2), (y1, y2)
-
-    x, y, w, h = bounds
-    return ((x, x+w), (y, y+h))
-
 # Utility foo
 # ===========
 
-def run_resvg(input_file, output_file, **resvg_args):
-
-    args = []
-    for key, value in resvg_args.items():
+def run_cargo_command(binary, *args, **kwargs):
+    cmd_args = []
+    for key, value in kwargs.items():
         if value is not None:
             if value is False:
                 continue
 
-            args.append(f'--{key.replace("_", "-")}')
+            cmd_args.append(f'--{key.replace("_", "-")}')
 
             if value is not True:
-                args.append(value)
-
-    args += [input_file, output_file]
+                cmd_args.append(value)
+    cmd_args.extend(map(str, args))
 
     # By default, try a number of options:
     candidates = [
         # somewhere in $PATH
-        'resvg',
-        'wasi-resvg',
+        binary,
+        # wasi-wrapper in $PATH
+        f'wasi-{binary}',
         # in user-local cargo installation
-        Path.home() / '.cargo' / 'bin' / 'resvg',
-        # wasi-resvg in user-local pip installation
-        Path.home() / '.local' / 'bin' / 'wasi-resvg',
+        Path.home() / '.cargo' / 'bin' / binary,
+        # wasi-wrapper in user-local pip installation
+        Path.home() / '.local' / 'bin' / f'wasi-{binary}',
         # next to our current python interpreter (e.g. in virtualenv)
-        str(Path(sys.executable).parent / 'wasi-resvg')
+        str(Path(sys.executable).parent / f'wasi-{binary}')
         ]
 
-    # if RESVG envvar is set, try that first.
-    if 'RESVG' in os.environ:
-        candidates = [os.environ['RESVG'], *candidates]
+    # if envvar is set, try that first.
+    if (env_var := os.environ.get(binary.upper())):
+        candidates = [env_var, *candidates]
 
-    for candidate in candidates:
+    for cand in candidates:
         try:
-            res = subprocess.run([candidate, *args], check=True)
-            print('used resvg:', candidate)
+            logging.debug(f'trying {binary}: {cand}')
+            logging.debug(f'with args: {" ".join(cmd_args)}')
+            res = subprocess.run([cand, *cmd_args], check=True)
             break
         except FileNotFoundError:
             continue
     else:
-        raise SystemError('resvg executable not found')
+        raise SystemError(f'{binary} executable not found')
 
 
 
 def calculate_apertureless_bounding_box(cam):
     ''' pcb-tools'es default bounding box function returns the bounding box of the primitives including apertures (i.e.
     line widths). For determining a board's size from the outline layer, we want the bounding box disregarding
     apertures.
@@ -489,21 +517,23 @@
 
     return str(svg)
 
 # SVG/gerber import
 #==================
 
 def dilate_gerber(layer, bounds, dilation, curve_tolerance):
-    with tempfile.NamedTemporaryFile(suffix='.svg') as temp_svg:
-        Path(temp_svg.name).write_text(str(layer.instance.to_svg(force_bounds=bounds, fg='white')))
+    with tempfile.NamedTemporaryFile(suffix='.svg') as temp_in_svg,\
+         tempfile.NamedTemporaryFile(suffix='.svg') as temp_out_svg:
+        Path(temp_in_svg.name).write_text(str(layer.instance.to_svg(force_bounds=bounds, fg='white')))
+        run_cargo_command('usvg', temp_in_svg.name, temp_out_svg.name)
 
         # dilate & render back to gerber
         # NOTE: Maybe reconsider or nicely document dilation semantics ; It is weird that negative dilations affect
         # clear color and positive affects dark colors
-        out = svg_to_gerber(temp_svg.name, dilate=-dilation, curve_tolerance=curve_tolerance)
+        out = svg_to_gerber(temp_out_svg.name, no_usvg=True, dilate=-dilation, curve_tolerance=curve_tolerance)
         return out
 
 def svg_to_gerber(infile, outline_mode=False, **kwargs):
     infile = Path(infile)
 
     args = [ '--format', ('gerber-outline' if outline_mode else 'gerber'),
             '--precision', '6', # intermediate file, use higher than necessary precision
@@ -514,17 +544,19 @@
             args.append('--' + k.replace('_', '-'))
             if not isinstance(v, bool):
                 args.append(str(v))
 
     with tempfile.NamedTemporaryFile(suffix='.gbr') as temp_gbr:
         args += [str(infile), str(temp_gbr.name)]
 
+        logging.debug(f'svg-flatten args: {" ".join(args)}')
+
         if 'SVG_FLATTEN' in os.environ:
+            logging.debug('using svg-flatten at $SVG_FLATTEN')
             subprocess.run([os.environ['SVG_FLATTEN'], *args], check=True)
-            print('used svg-flatten at $SVG_FLATTEN')
 
         else:
             # By default, try four options:
             for candidate in [
                     # somewhere in $PATH
                     'svg-flatten',
                     None, # direct WASI import
@@ -541,34 +573,24 @@
                     # next to this python source file in the development repo
                     str(Path(__file__).parent.parent / 'svg-flatten' / 'build' / 'svg-flatten') ]:
 
                 try:
                     if candidate is None:
                         import svg_flatten_wasi
                         svg_flatten_wasi.run_svg_flatten.callback(args[-2], args[-1], args[:-2], no_usvg=False)
-                        print('used svg_flatten_wasi python package') 
+                        logging.debug('using svg_flatten_wasi python package') 
 
                     else:
                         subprocess.run([candidate, *args], check=True)
-                        print('used svg-flatten at', candidate)
+                        logging.debug('using svg-flatten at', candidate)
 
                     break
                 except (FileNotFoundError, ModuleNotFoundError):
                     continue
 
             else:
                 raise SystemError('svg-flatten executable not found')
 
         return gn.rs274x.GerberFile.open(temp_gbr.name)
 
-def get_layers_from_svg(svg_data):
-    svg = etree.fromstring(svg_data.encode('utf-8'))
-    SVG_NS = '{http://www.w3.org/2000/svg}'
-    INKSCAPE_NS = '{http://www.inkscape.org/namespaces/inkscape}'
-
-    # find groups
-    for group in svg.findall(SVG_NS+'g'):
-        yield group.get('id'), group.get(INKSCAPE_NS+'label')
-   
-
 if __name__ == '__main__':
     cli()
```

### Comparing `gerbolyze-3.0.9/gerbolyze/protoboard.py` & `gerbolyze-3.1.4/gerbolyze/protoboard.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,52 +4,66 @@
 import textwrap
 import ast
 import uuid
 
 svg_str = lambda content: content if isinstance(content, str) else '\n'.join(str(c) for c in content)
 
 class Pattern:
-    def __init__(self, w, h, content):
-        self.w = w
-        self.h = h
-        self.content = content
+    def __init__(self, w, h=None):
+        self.vb_w = self.w = w
+        self.vb_h = self.h = h or w
 
     def svg_def(self, svg_id, off_x, off_y):
         return textwrap.dedent(f'''
-            <pattern id="{svg_id}" x="{off_x}" y="{off_y}" viewBox="0,0,{self.w},{self.h}" width="{self.w}" height="{self.h}" patternUnits="userSpaceOnUse">
+            <pattern id="{svg_id}" x="{off_x}" y="{off_y}" viewBox="0,0,{self.vb_w},{self.vb_h}" width="{self.w}" height="{self.h}" patternUnits="userSpaceOnUse">
                 {svg_str(self.content)}
             </pattern>''')
-
+    
 def make_rect(svg_id, x, y, w, h, clip=''):
     #import random
     #c = random.randint(0, 2**24)
     #return f'<rect x="{x}" y="{y}" width="{w}" height="{h}" fill="#{c:06x}"/>'
     return f'<rect x="{x}" y="{y}" width="{w}" height="{h}" {clip} fill="url(#{svg_id})"/>'
 
 class CirclePattern(Pattern):
     def __init__(self, d, w, h=None):
+        super().__init__(w, h)
         self.d = d
-        self.w = w
-        self.h = h or w
 
     @property
     def content(self):
         return f'<circle cx="{self.w/2}" cy="{self.h/2}" r="{self.d/2}"/>'
 
 class RectPattern(Pattern):
     def __init__(self, rw, rh, w, h):
+        super().__init__(w, h)
         self.rw, self.rh = rw, rh
-        self.w, self.h = w, h
 
     @property
     def content(self):
         x = (self.w - self.rw) / 2
         y = (self.h - self.rh) / 2
         return f'<rect x="{x}" y="{y}" width="{self.rw}" height="{self.rh}"/>'
 
+class ManhattanPattern(Pattern):
+    def __init__(self, pitch=2.54*4, gap=0.2):
+        super().__init__(pitch)
+        self.vb_w, self.vb_h = 1, 1
+        self.gap = gap
+
+    @property
+    def content(self):
+        return textwrap.dedent('''
+                <rect x="0"   y="0"   width="0.5" height="0.5" style="fill: black; stroke: white; stroke-width: 0.01mm"/>
+                <rect x="0"   y="0.5" width="0.5" height="0.5" style="fill: black; stroke: white; stroke-width: 0.01mm"/>
+                <rect x="0.5" y="0"   width="0.5" height="0.5" style="fill: black; stroke: white; stroke-width: 0.01mm"/>
+                <rect x="0.5" y="0.5" width="0.5" height="0.5" style="fill: black; stroke: white; stroke-width: 0.01mm"/>
+                <rect x="0.3" y="0.3" width="0.4" height="0.4" style="fill: black; stroke: white; stroke-width: 0.01mm" transform="rotate(45 0.5 0.5)"/>
+                '''.strip())
+
 make_layer = lambda layer_name, content: \
   f'<g id="g-{layer_name.replace(" ", "-")}" inkscape:label="{layer_name}" inkscape:groupmode="layer">{svg_str(content)}</g>'
 
 svg_template = textwrap.dedent('''
     <?xml version="1.0" encoding="UTF-8" standalone="no"?>
     <svg version="1.1" width="{w}mm" height="{h}mm" viewBox="0 0 {w} {h}" id="svg18" sodipodi:docname="proto.svg"
        inkscape:version="1.2 (dc2aedaf03, 2022-05-15)"
@@ -86,14 +100,19 @@
 
     @property
     def pitch(self):
         if self.pitch_x != self.pitch_y:
             raise ValueError('Pattern has different X and Y pitches')
         return self.pitch_x
 
+    def fit_size(self, w, h):
+        x, y, w, h = self.fit_rect(0, 0, w, h, False)
+        t, r, b, l = self.border
+        return (w+l+r), (h+t+b)
+
     def fit_rect(self, x, y, w, h, center=True):
         t, r, b, l = self.border
         x, y, w, h = (x+l), (y+t), (w-l-r), (h-t-b)
 
         w_mod, h_mod = round((w + 5e-7) % self.pitch_x, 6), round((h + 5e-7) % self.pitch_y, 6)
         w_fit, h_fit = round(w - w_mod, 6), round(h - h_mod, 6)
 
@@ -101,16 +120,23 @@
             x = x + (w-w_fit)/2
             y = y + (h-h_fit)/2
             return x, y, w_fit, h_fit
 
         else:
             return x, y, w_fit, h_fit
 
-    def generate(self, x, y, w, h, defs=None, center=True, clip=''):
-        return {}
+    def generate(self, x, y, w, h, center=True, clip='', tight_layout=False):
+        yield {}
+
+    def symmetric_sides(self):
+        return False
+
+    def used_patterns(self):
+        yield self
+
 
 class EmptyProtoArea:
     def __init__(self, copper=False, border=None):
         self.copper = copper
 
         if border is None:
             self.border = (0, 0, 0, 0)
@@ -118,34 +144,45 @@
             if len(border == 4):
                 self.border = border
             else:
                 raise TypeError('border must be None, int, or a 4-tuple of floats (top, right, bottom, left)')
         else:
             self.border = (border, border, border, border)
 
-    def generate(self, x, y, w, h, defs=None, center=True, clip=''):
+    def fit_size(self, w, h):
+        return w, h
+
+    def generate(self, x, y, w, h, center=True, clip='', tight_layout=False):
         if self.copper:
             t, r, b, l = self.border
             x, y, w, h = x+l, y+t, w-l-r, h-t-b
-            return { 'top copper': f'<rect x="{x}" y="{y}" width="{w}" height="{h}" {clip} fill="black"/>' }
+            yield { 'top copper': f'<rect x="{x}" y="{y}" width="{w}" height="{h}" {clip} fill="black"/>' }
         else:
-            return {}
+            yield {}
+
+    def used_patterns(self):
+        yield self
 
-class THTProtoAreaCircles(PatternProtoArea):
-    def __init__(self, pad_dia=2.0, drill=1.0, pitch=2.54, sides='both', plated=True, border=None):
+
+class THTProtoArea(PatternProtoArea):
+    def __init__(self, pad_size=2.0, drill=1.0, pitch=2.54, sides='both', plated=True, border=None, pad_shape='circle'):
         super().__init__(pitch, border=border)
-        self.pad_dia = pad_dia
+        self.pad_size = pad_size
+        self.pad_shape = pad_shape.lower().rstrip('s')
         self.drill = drill
         self.drill_pattern = CirclePattern(self.drill, self.pitch)
-        self.pad_pattern = CirclePattern(self.pad_dia, self.pitch)
+        if self.pad_shape == 'circle':
+            self.pad_pattern = CirclePattern(self.pad_size, self.pitch)
+        elif self.pad_shape == 'square':
+            self.pad_pattern = RectPattern(self.pad_size, self.pad_size, self.pitch, self.pitch)
         self.patterns = [self.drill_pattern, self.pad_pattern]
         self.plated = plated
         self.sides = sides
     
-    def generate(self, x, y, w, h, defs=None, center=True, clip=''):
+    def generate(self, x, y, w, h, center=True, clip='', tight_layout=False):
         x, y, w, h = self.fit_rect(x, y, w, h, center)
         drill = 'plated drill' if self.plated else 'nonplated drill'
 
         pad_id = str(uuid.uuid4())
         drill_id = str(uuid.uuid4())
 
         d = { drill: make_rect(drill_id, x, y, w, h, clip),
@@ -156,35 +193,59 @@
         if self.sides in ('top', 'both'):
             d['top copper'] = make_rect(pad_id, x, y, w, h, clip)
             d['top mask'] = make_rect(pad_id, x, y, w, h, clip)
         if self.sides in ('bottom', 'both'):
             d['bottom copper'] = make_rect(pad_id, x, y, w, h, clip)
             d['bottom mask'] = make_rect(pad_id, x, y, w, h, clip)
 
-        return d
+        yield d
 
     def __repr__(self):
-        return f'THTCircles(d={self.pad_dia}, h={self.drill}, p={self.pitch}, sides={self.sides}, plated={self.plated})'
+        return f'THTPads(size={self.pad_size}, h={self.drill}, p={self.pitch}, sides={self.sides}, plated={self.plated}, pad_shape="{self.pad_shape}")'
+
+    def symmetric_sides(self):
+        return True
+
 
 class SMDProtoAreaRectangles(PatternProtoArea):
     def __init__(self, pitch_x, pitch_y, w=None, h=None, border=None):
         super().__init__(pitch_x, pitch_y, border=border)
         w = w or pitch_x - 0.15
         h = h or pitch_y - 0.15
         self.w, self.h = w, h
         self.pad_pattern = RectPattern(w, h, pitch_x, pitch_y)
         self.patterns = [self.pad_pattern]
 
-    def generate(self, x, y, w, h, defs=None, center=True, clip=''):
+    def generate(self, x, y, w, h, center=True, clip='', tight_layout=False):
         x, y, w, h = self.fit_rect(x, y, w, h, center)
         pad_id = str(uuid.uuid4())
-        return {'defs': [self.pad_pattern.svg_def(pad_id, x, y)],
+        yield {'defs': [self.pad_pattern.svg_def(pad_id, x, y)],
             'top copper': make_rect(pad_id, x, y, w, h, clip),
             'top mask': make_rect(pad_id, x, y, w, h, clip)}
 
+    def symmetric_sides(self):
+        return False
+
+class ManhattanProtoArea(PatternProtoArea):
+    def __init__(self, pitch=2.54*4, gap=0.25, border=None):
+        super().__init__(pitch, pitch, border=border)
+        self.gap = gap
+        self.pad_pattern = ManhattanPattern(pitch, gap)
+        self.patterns = [self.pad_pattern]
+
+    def generate(self, x, y, w, h, center=True, clip='', tight_layout=False):
+        x, y, w, h = self.fit_rect(x, y, w, h, center)
+        pad_id = str(uuid.uuid4())
+        yield {'defs': [self.pad_pattern.svg_def(pad_id, x, y)],
+            'top copper': make_rect(pad_id, x, y, w, h, clip),
+            'top mask': make_rect(pad_id, x, y, w, h, clip)}
+
+    def symmetric_sides(self):
+        return False
+
 LAYERS = [
         'top paste',
         'top silk',
         'top mask',
         'top copper',
         'bottom copper',
         'bottom mask',
@@ -192,30 +253,39 @@
         'bottom paste',
         'outline',
         'nonplated drill',
         'plated drill'
         ]
 
 class ProtoBoard:
-    def __init__(self, defs, expr, mounting_holes=None, border=None, center=True):
+    def __init__(self, defs, expr, mounting_holes=None, border=None, center=True, tight_layout=False):
         self.defs = eval_defs(defs)
-        self.layout = parse_layout(expr)
+        self.layout = parse_layout(expr, self.defs)
         self.mounting_holes = mounting_holes
         self.center = center
+        self.tight_layout = tight_layout
 
         if border is None:
             self.border = (0, 0, 0, 0)
         elif hasattr(border, '__iter__'):
             if len(border == 4):
                 self.border = border
             else:
                 raise TypeError('border must be None, int, or a 4-tuple of floats (top, right, bottom, left)')
         else:
             self.border = (border, border, border, border)
 
+    @property
+    def symmetric_sides(self):
+        return self.layout.symmetric_sides()
+
+    @property
+    def used_patterns(self):
+        return set(self.layout.used_patterns())
+
     def generate(self, w, h):
         out = {l: [] for l in LAYERS}
         svg_defs = []
         clip = ''
 
         if self.mounting_holes:
             d, o, *k = self.mounting_holes # diameter, offset from edge, keepout to proto area
@@ -238,15 +308,15 @@
             out['nonplated drill'].append([
                 f'<circle cx="{o}" cy="{o}" r="{d/2}"/>',
                 f'<circle cx="{w-o}" cy="{o}" r="{d/2}"/>',
                 f'<circle cx="{w-o}" cy="{h-o}" r="{d/2}"/>',
                 f'<circle cx="{o}" cy="{h-o}" r="{d/2}"/>' ])
 
         t, r, b, l = self.border
-        for layer_dict in self.layout.generate(l, t, w-l-r, h-t-b, self.defs, self.center, clip):
+        for layer_dict in self.layout.generate(l, t, w-l-r, h-t-b, self.center, clip, self.tight_layout):
             for l in LAYERS:
                 if l in layer_dict:
                     out[l].append(layer_dict[l])
             svg_defs += layer_dict.get('defs', [])
 
         out['outline'] = f'<rect x="0" y="0" width="{w}" height="{h}" fill="none" stroke="black" stroke-width="0.1mm"/>'
 
@@ -284,33 +354,54 @@
     def __init__(self, content, direction, proportions):
         self.content = content
         self.direction = direction
         self.proportions = proportions
         if len(content) != len(proportions):
             raise ValueError('proportions and content must have same length')
 
-    def generate(self, x, y, w, h, defs, center=True, clip=''):
-        for (c_x, c_y, c_w, c_h), child in self.layout_2d(x, y, w, h):
-            if isinstance(child, str):
-                yield defs[child].generate(c_x, c_y, c_w, c_h, defs, center, clip)
-
-            else:
-                yield from child.generate(c_x, c_y, c_w, c_h, defs, center, clip)
+    def generate(self, x, y, w, h, center=True, clip='', tight_layout=False):
+        for (c_x, c_y, c_w, c_h), child in self.layout_2d(x, y, w, h, tight_layout):
+            yield from child.generate(c_x, c_y, c_w, c_h, center, clip, tight_layout)
+
+    def fit_size(self, w, h):
+        widths = []
+        heights = []
+        for (_x, _y, w, h), child in self.layout_2d(0, 0, w, h, True):
+            if not isinstance(child, EmptyProtoArea):
+                widths.append(w)
+                heights.append(h)
+        if self.direction == 'h':
+            return sum(widths), max(heights)
+        else:
+            return max(widths), sum(heights)
 
-    def layout_2d(self, x, y, w, h):
+    def layout_2d(self, x, y, w, h, tight_layout=False):
+        actual_l = 0
+        target_l = 0
         for l, child in zip(self.layout(w if self.direction == 'h' else h), self.content):
-            this_w, this_h = w, h
             this_x, this_y = x, y
+            this_w, this_h = w, h
+            target_l += l
 
             if self.direction == 'h':
-                this_w = l
-                x += l
+                this_w = target_l - actual_l
             else:
-                this_h = l
-                y += l
+                this_h = target_l - actual_l
+
+            if tight_layout:
+                this_w, this_h = child.fit_size(this_w, this_h)
+
+            if self.direction == 'h':
+                x += this_w
+                actual_l += this_w
+                this_h = h
+            else:
+                y += this_h
+                actual_l += this_h
+                this_w = w
 
             yield (this_x, this_y, this_w, this_h), child
 
     def layout(self, length):
         out = [ eval_value(value, length) for value in self.proportions ]
         total_length = sum(value for value in out if value is not None)
         if length - total_length < -1e-6:
@@ -321,14 +412,22 @@
         return [ (leftover * (value or 1.0) / sum_props if not isinstance(value, str) else calculated)
                 for value, calculated in zip(self.proportions, out) ]
 
     def __str__(self):
         children = ', '.join( f'{elem}:{width}' for elem, width in zip(self.content, self.proportions))
         return f'PropLayout[{self.direction.upper()}]({children})'
 
+    def symmetric_sides(self):
+        return all(child.symmetric_sides() for child in self.content)
+
+    def used_patterns(self):
+        for child in self.content:
+            yield from child.used_patterns()
+
+
 class TwoSideLayout:
     def __init__(self, top, bottom):
         self.top, self.bottom = top, bottom
 
     def flip(self, defs):
         out = dict(defs)
         for layer in ('copper', 'mask', 'silk', 'paste'):
@@ -343,47 +442,60 @@
             if bval:
                 defs[top] = bval
             elif top in defs:
                 del defs[top]
 
         return defs
 
-    def generate(self, x, y, w, h, defs, center=True, clip=''):
-        if isinstance(self.top, str):
-            yield defs[self.top].generate(x, y, w, h, defs, center, clip)
-        else:
-            yield from self.top.generate(x, y, w, h, defs, center, clip)
+    def fit_size(self, w, h):
+        top, bottom = self.top, self.bottom
+        w1, h1 = top.fit_size(w, h)
+        w2, h2 = bottom.fit_size(w, h)
+        if isinstance(top, EmptyProtoArea):
+            if isinstance(bottom, EmptyProtoArea):
+                return w1, h1
+            return w2, h2
+        if isinstance(bottom, EmptyProtoArea):
+            return w1, h1
+        return max(w1, w2), max(h1, h2)
+
+    def generate(self, x, y, w, h, center=True, clip='', tight_layout=False):
+        yield from self.top.generate(x, y, w, h, center, clip, tight_layout)
+        yield from map(self.flip, self.bottom.generate(x, y, w, h, center, clip, tight_layout))
+
+    def symmetric_sides(self):
+        return self.top == self.bottom
+
+    def used_patterns(self):
+        yield from self.top.used_patterns()
+        yield from self.bottom.used_patterns()
 
-        if isinstance(self.bottom, str):
-            yield self.flip(defs[self.bottom].generate(x, y, w, h, defs, center, clip))
-        else:
-            yield from map(self.flip, self.bottom.generate(x, y, w, h, defs, center, clip))
 
-def _map_expression(node):
+def _map_expression(node, defs):
     if isinstance(node, ast.Name):
-        return node.id
+        return defs[node.id]
 
     elif isinstance(node, ast.Constant):
         return node.value
 
 
     elif isinstance(node, ast.BinOp) and isinstance(node.op, (ast.BitOr, ast.BitAnd, ast.Add)):
         left_prop = right_prop = None
 
         left, right = node.left, node.right
 
         if isinstance(left, ast.BinOp) and isinstance(left.op, ast.MatMult):
-            left_prop = _map_expression(left.right)
+            left_prop = _map_expression(left.right, defs)
             left = left.left
 
         if isinstance(right, ast.BinOp) and isinstance(right.op, ast.MatMult):
-            right_prop = _map_expression(right.right)
+            right_prop = _map_expression(right.right, defs)
             right = right.left
 
-        left, right = _map_expression(left), _map_expression(right)
+        left, right = _map_expression(left, defs), _map_expression(right, defs)
 
         direction = 'h' if isinstance(node.op, ast.BitOr) else 'v'
         if isinstance(left, PropLayout) and left.direction == direction and left_prop is None:
             left.content.append(right)
             left.proportions.append(right_prop)
             return left
 
@@ -403,41 +515,42 @@
         
     elif isinstance(node, ast.BinOp) and isinstance(node.op, ast.MatMult):
         raise SyntaxError(f'Unexpected width specification "{ast.unparse(node.right)}"')
 
     else:
         raise SyntaxError(f'Invalid layout expression "{ast.unparse(node)}"')
 
-def parse_layout(expr):
+def parse_layout(expr, defs):
     ''' Example layout:
 
         ( tht @ 2in | smd ) @ 50% / tht
     '''
 
     expr = re.sub(r'\s', '', expr)
     expr = re.sub(r'([0-9]*\.?[0-9]+)([Mm][Mm]|[Cc][Mm]|[Ii][Nn]|[Mm][Ii][Ll]|%)', r'"\1\2"', expr)
     expr = expr.replace('/', '&')
     try:
         expr = ast.parse(expr, mode='eval').body
         match expr:
             case ast.Name():
-                return PropLayout([expr.id], 'h', [None])
+                return PropLayout([defs[expr.id]], 'h', [None])
 
             case ast.BinOp(op=ast.MatMult()):
                 assert isinstance(expr.right, ast.Constant)
-                return PropLayout([_map_expression(expr.left)], 'h', [expr.right.value])
+                return PropLayout([_map_expression(expr.left, defs)], 'h', [expr.right.value])
 
             case _:
-                return _map_expression(expr)
+                return _map_expression(expr, defs)
     except SyntaxError as e:
         raise SyntaxError('Invalid layout expression') from e
 
 PROTO_AREA_TYPES = {
-    'THTCircles': THTProtoAreaCircles,
+    'THTPads': THTProtoArea,
     'SMDPads': SMDProtoAreaRectangles,
+    'Manhattan': ManhattanProtoArea,
     'Empty': EmptyProtoArea,
 }
 
 def eval_defs(defs):
     defs = defs.replace('\n', ';')
     defs = re.sub(r'\s', '', defs)
 
@@ -460,14 +573,35 @@
 
             else:
                 args.append(ast.literal_eval(elem))
 
         out[key] = PROTO_AREA_TYPES[pattern](*args, **kws)
     return out
 
+COMMON_DEFS = '''
+empty = Empty(copper=False);
+ground = Empty(copper=True);
+
+tht = THTPads();
+manhattan = Manhattan();
+tht50 = THTPads(pad_size=1.0, drill=0.6, pitch=1.27);
+
+smd100 = SMDPads(1.27, 2.54);
+smd100r = SMDPads(2.54, 1.27);
+smd950 = SMDPads(0.95, 2.5);
+smd950r = SMDPads(2.5, 0.95);
+smd800 = SMDPads(0.80, 2.0);
+smd800r = SMDPads(2.0, 0.80);
+smd650 = SMDPads(0.65, 2.0);
+smd650r = SMDPads(2.0, 0.65);
+smd500 = SMDPads(0.5, 2.0);
+smd500r = SMDPads(2.0, 0.5);
+'''
+
+
 if __name__ == '__main__':
 #    import sys
 #    print('===== Layout expressions =====')
 #    for line in [
 #            'tht',
 #            'tht@1mm',
 #            'tht|tht',
@@ -490,11 +624,13 @@
 #            'tht = THTCircles(10, 20)',
 #            'tht = THTCircles(plated=False)',
 #            'tht = THTCircles(10, plated=False)',
 #            ]:
 #        print(line, '->', eval_defs(line))
 #    print()
 #    print('===== Proto board =====')
-    #b = ProtoBoard('tht = THTCircles(); tht_small = THTCircles(pad_dia=1.0, drill=0.6, pitch=1.27)',
+    #b = ProtoBoard('tht = THTCircles(); tht_small = THTCircles(pad_size=1.0, drill=0.6, pitch=1.27)',
     #        'tht@1in|(tht_small@2/tht@1)', mounting_holes=(3.2, 5.0, 5.0), border=2, center=False)
-    b = ProtoBoard('tht = THTCircles(); smd1 = SMDPads(0.8, 1.27); smd2 = SMDPads(0.95, 1.895); plane=Empty(copper=True)', 'tht@1in | (smd1 + plane)', mounting_holes=(3.2, 5.0, 5.0), border=2)
+    #b = ProtoBoard('tht = THTCircles(); smd1 = SMDPads(2.0, 2.0); smd2 = SMDPads(0.95, 1.895); plane=Empty(copper=True)', 'tht@25mm | (smd1 + plane)', mounting_holes=(3.2, 5.0, 5.0), border=2, tight_layout=True)
+    #b = ProtoBoard(COMMON_DEFS, f'((smd100 + smd100) | (smd950 + smd950) | tht50@20mm)@20mm / tht', mounting_holes=(3.2,5,5), border=1, tight_layout=True, center=True)
+    b = ProtoBoard(COMMON_DEFS, f'manhattan', mounting_holes=(3.2,5,5), border=1, tight_layout=True, center=True)
     print(b.generate(80, 60))
```

### Comparing `gerbolyze-3.0.9/gerbolyze.egg-info/PKG-INFO` & `gerbolyze-3.1.4/gerbolyze.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: gerbolyze
-Version: 3.0.9
+Version: 3.1.4
 Summary: A high-resolution image-to-PCB converter. Gerbolyze plots SVG, PNG and JPG onto existing gerber files. It handles almost the full SVG spec and deals with text, path outlines, patterns, arbitrary paths with self-intersections and holes, etc. fully automatically. It can vectorize raster images both by contour tracing and by grayscale dithering. All processing is done at the vector level without intermediate conversions to raster images accurately preserving the input.
 Home-page: https://github.com/jaseg/gerbolyze
 Author: jaseg
 Author-email: gerbonara@jaseg.de
 License: AGPLv3
 Project-URL: Source Code, https://git.jaseg.de/gerbolyze
 Project-URL: Bug Tracker, https://github.com/jaseg/gerbolyze/issues
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Manufacturing
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Religion
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
@@ -34,15 +33,17 @@
 Vector data from SVG files is rendered losslessly *without* an intermediate rasterization/revectorization step.
 Still, gerbolyze supports (almost) the full SVG 1.1 spec including complex, self-intersecting paths with holes,
 patterns, dashes and transformations.
 
 Raster images can either be vectorized through contour tracing (like gerbolyze v1.0 did) or they can be embedded using
 high-resolution grayscale emulation while (mostly) guaranteeing trace/space design rules.
 
-.. figure:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.0.9/pics/pcbway_sample_02_small.jpg
+Try gerbolyze online at https://dyna.kokoroyukuma.de/gerboweb
+
+.. figure:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.1.4/pics/pcbway_sample_02_small.jpg
   :width: 800px
 
   Drawing by `トーコ Toko <https://twitter.com/fluffy2038/status/1317231121269104640>`__ converted using Gerbolyze and printed at PCBWay.
 
 
 Tooling for PCB art is quite limited in both open source and closed source ecosystems. Something as simple as putting a
 pretty picture on a PCB can be an extremely tedious task. Depending on the PCB tool used, various arcane incantations
@@ -54,15 +55,15 @@
 industry-standard Altium Designer. Gerbolyze is written with performance in mind and will happily vectorize tens of
 thousands of primitives, generating tens of megabytes of gerber code without crapping itself. With gerbolyze you can
 finally be confident that your PCB fab's toolchain will fall over before yours does if you overdo it with the high-poly
 anime silkscreen.
 
 Gerbolyze is based on gerbonara_.
 
-.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.0.9/pics/process-overview.png
+.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.1.4/pics/process-overview.png
   :width: 800px
 
 .. contents::
 
 Tl;dr: Produce high-quality artistic PCBs in three easy steps!
 --------------------------------------------------------------
 
@@ -139,15 +140,15 @@
     python3 setup.py install
 
 Features
 --------
 
 Input on the left, output on the right.
 
-.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.0.9/pics/test_svg_readme_composited.png
+.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.1.4/pics/test_svg_readme_composited.png
   :width: 800px
 
 * Almost full SVG 1.1 static spec coverage (!)
 
   * Paths with beziers, self-intersections and holes
   * Strokes, even with dashes and markers
   * Pattern fills and strokes
@@ -204,14 +205,24 @@
     * apply pattern fills
     * clip to clip-path
     * remove holes using Clipper
 
 * for KiCAD S-Expression export: vector-composite results using CavalierContours: subtract each clear output primitive
   from all previous dark output primitives
 
+Web interface
+-------------
+
+You can try gerbolyze online at https://dyna.kokoroyukuma.de/gerboweb
+
+The web interface does not expose all of gerbolyze's bells and whistles, but it allows you to simply paste a single SVG
+file on a board to try out gerbolyze. Upload your design on the web interface, then download the template for either the
+top or bottom side, and put your artwork on the appropriate layer of that template using Inkscape_. Finally, upload the
+modified template and let gerbolyze process your design.
+
 Command-line usage
 ------------------
 .. _command_line_usage:
 
 Generate SVG template from Gerber files:
 
 .. code-block:: shell
@@ -339,15 +350,15 @@
 Dashed strokes are supported on outline layers and can be used to make easy mouse bites.
 
 .. _subtraction_script:
 
 Subtraction scripts
 *******************
 
-.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.0.9/pics/subtract_example.png
+.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.1.4/pics/subtract_example.png
   :width: 800px
 
 Subtraction scripts tell ``gerbolyze paste`` to remove an area around certain input layers to from an overlay layer.
 When a input layer is given in the subtraction script, gerbolyze will dilate (extend outwards) everything on this input
 layer and remove it from the target overlay layer. By default, Gerbolyze subtracts the mask layer from the silk layer to
 make sure there are no silk primitives that overlap bare copper, and subtracts each input layer from its corresponding
 overlay to make sure the two do not overlap. In the picture above you can see both at work: The overlay contains
@@ -492,33 +503,33 @@
 
 .. for f in vec_*.png; convert -background white -gravity center $f -resize 500x500 -extent 500x500 (basename -s .png $f)-square.png; end
 .. for vec in hexgrid square poisson contours; convert vec_"$vec"_whole-square.png vec_"$vec"_detail-square.png -background transparent -splice 25x0+0+0 +append -chop 25x0+0+0 vec_"$vec"_composited.png; end
 
 ``--vectorizer poisson-disc`` (the default) 
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.0.9/pics/vec_poisson_composited.png
+.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.1.4/pics/vec_poisson_composited.png
   :width: 800px
 
 ``--vectorizer hex-grid``
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
-.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.0.9/pics/vec_hexgrid_composited.png
+.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.1.4/pics/vec_hexgrid_composited.png
   :width: 800px
 
 ``--vectorizer square-grid``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.0.9/pics/vec_square_composited.png
+.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.1.4/pics/vec_square_composited.png
   :width: 800px
 
 ``--vectorizer binary-contours``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.0.9/pics/vec_contours_composited.png
+.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.1.4/pics/vec_contours_composited.png
   :width: 800px
 
 The binary contours vectorizer requires a black-and-white binary input image. As you can see, like every bitmap tracer
 it will produce some artifacts. For artistic input this is usually not too bad as long as the input data is
 high-resolution. Antialiased edges in the input image are not only OK, they may even help with an accurate
 vectorization.
 
@@ -688,17 +699,20 @@
 
 A design rule checker is planned as a future addition to gerbolyze, but is not yet part of it. If in doubt, talk to your
 fab and consider doing a test run of your design before ordering assembled boards ;)
 
 Gallery
 -------
 
-.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.0.9/pics/sample3.jpg
+.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.1.4/pics/sample3.jpg
   :width: 400px
 
+For a demonstration of ``gerbolyze convert``, check out the `Gerbolyze Protoboard Index`_, where you can download gerber
+files for over 7.000 SMD and THT protoboard layouts.
+
 Licensing
 ---------
 
 This tool is licensed under the rather radical AGPLv3 license. Briefly, this means that you have to provide users of a
 webapp using this tool in the backend with this tool's source.
 
 I get that some people have issues with the AGPL. In case this license prevents you from using this software, please
@@ -709,9 +723,8 @@
 
 .. _usvg: https://github.com/RazrFalcon/resvg
 .. _Inkscape: https://inkscape.org/
 .. _pcb-tools: https://github.com/curtacircuitos/pcb-tools
 .. _pcb-tools-extension: https://github.com/opiopan/pcb-tools-extension
 .. _GIMP: https://gimp.org/
 .. _gerbonara: https://gitlab.com/gerbolyze/gerbonara
-
-
+.. _`Gerbolyze Protoboard Index`: https://dyna.kokoroyukuma.de/protos/
```

### Comparing `gerbolyze-3.0.9/setup.py` & `gerbolyze-3.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     url='https://github.com/jaseg/gerbolyze',
     project_urls={
         'Source Code': 'https://git.jaseg.de/gerbolyze',
         'Bug Tracker': 'https://github.com/jaseg/gerbolyze/issues',
     },
     author = 'jaseg',
     author_email = 'gerbonara@jaseg.de',
-    install_requires = ['gerbonara', 'numpy', 'python-slugify', 'lxml', 'click', 'resvg-wasi >= 0.23.0', 'svg-flatten-wasi[resvg-wasi]'],
+    install_requires = ['gerbonara >= 1.0.0', 'numpy', 'python-slugify', 'lxml', 'click', 'svg-flatten-wasi'],
     license = 'AGPLv3',
     classifiers = [
         'Development Status :: 5 - Production/Stable',
         'Environment :: Console',
         'Intended Audience :: Manufacturing',
         'Intended Audience :: Science/Research',
         'Intended Audience :: Religion',
```

