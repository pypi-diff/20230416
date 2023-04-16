# Comparing `tmp/gerbolyze-3.1.4.tar.gz` & `tmp/gerbolyze-3.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gerbolyze-3.1.4.tar", last modified: Sun Apr 16 18:25:51 2023, max compression
+gzip compressed data, was "gerbolyze-3.1.5.tar", last modified: Sun Apr 16 18:39:39 2023, max compression
```

## Comparing `gerbolyze-3.1.4.tar` & `gerbolyze-3.1.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 bernd     (1000) bernd     (1000)        0 2023-04-16 18:25:51.081930 gerbolyze-3.1.4/
--rw-rw-rw-   0 bernd     (1000) bernd     (1000)    34523 2023-04-16 18:25:47.000000 gerbolyze-3.1.4/LICENSE
--rw-rw-rw-   0 bernd     (1000) bernd     (1000)      490 2023-04-16 18:25:47.000000 gerbolyze-3.1.4/MANIFEST.in
--rw-r--r--   0 bernd     (1000) bernd     (1000)    34257 2023-04-16 18:25:51.080930 gerbolyze-3.1.4/PKG-INFO
--rw-rw-rw-   0 bernd     (1000) bernd     (1000)    32441 2023-04-16 18:25:47.000000 gerbolyze-3.1.4/README.rst
-drwxr-xr-x   0 bernd     (1000) bernd     (1000)        0 2023-04-16 18:25:51.076930 gerbolyze-3.1.4/bin/
--rw-rw-rw-   0 bernd     (1000) bernd     (1000)       92 2023-04-16 18:25:47.000000 gerbolyze-3.1.4/bin/gerbolyze
-drwxr-xr-x   0 bernd     (1000) bernd     (1000)        0 2023-04-16 18:25:51.077930 gerbolyze-3.1.4/gerbolyze/
--rwxrwxrwx   0 bernd     (1000) bernd     (1000)    27183 2023-04-16 18:25:47.000000 gerbolyze-3.1.4/gerbolyze/__init__.py
--rw-rw-rw-   0 bernd     (1000) bernd     (1000)       33 2023-04-16 18:25:47.000000 gerbolyze-3.1.4/gerbolyze/__main__.py
--rw-rw-rw-   0 bernd     (1000) bernd     (1000)    23446 2023-04-16 18:25:47.000000 gerbolyze-3.1.4/gerbolyze/protoboard.py
-drwxr-xr-x   0 bernd     (1000) bernd     (1000)        0 2023-04-16 18:25:51.080930 gerbolyze-3.1.4/gerbolyze/tests/
--rw-rw-rw-   0 bernd     (1000) bernd     (1000)        0 2023-04-16 18:25:47.000000 gerbolyze-3.1.4/gerbolyze/tests/__init__.py
--rw-rw-rw-   0 bernd     (1000) bernd     (1000)     5159 2023-04-16 18:25:47.000000 gerbolyze-3.1.4/gerbolyze/tests/test_integration.py
-drwxr-xr-x   0 bernd     (1000) bernd     (1000)        0 2023-04-16 18:25:51.079930 gerbolyze-3.1.4/gerbolyze.egg-info/
--rw-r--r--   0 bernd     (1000) bernd     (1000)    34257 2023-04-16 18:25:51.000000 gerbolyze-3.1.4/gerbolyze.egg-info/PKG-INFO
--rw-r--r--   0 bernd     (1000) bernd     (1000)      349 2023-04-16 18:25:51.000000 gerbolyze-3.1.4/gerbolyze.egg-info/SOURCES.txt
--rw-r--r--   0 bernd     (1000) bernd     (1000)        1 2023-04-16 18:25:51.000000 gerbolyze-3.1.4/gerbolyze.egg-info/dependency_links.txt
--rw-r--r--   0 bernd     (1000) bernd     (1000)       66 2023-04-16 18:25:51.000000 gerbolyze-3.1.4/gerbolyze.egg-info/requires.txt
--rw-r--r--   0 bernd     (1000) bernd     (1000)       10 2023-04-16 18:25:51.000000 gerbolyze-3.1.4/gerbolyze.egg-info/top_level.txt
--rw-r--r--   0 bernd     (1000) bernd     (1000)       38 2023-04-16 18:25:51.081930 gerbolyze-3.1.4/setup.cfg
--rwxrwxrwx   0 bernd     (1000) bernd     (1000)     2581 2023-04-16 18:25:48.000000 gerbolyze-3.1.4/setup.py
+drwxr-xr-x   0 bernd     (1000) bernd     (1000)        0 2023-04-16 18:39:39.785167 gerbolyze-3.1.5/
+-rw-rw-rw-   0 bernd     (1000) bernd     (1000)    34523 2023-04-16 18:39:36.000000 gerbolyze-3.1.5/LICENSE
+-rw-rw-rw-   0 bernd     (1000) bernd     (1000)      490 2023-04-16 18:39:36.000000 gerbolyze-3.1.5/MANIFEST.in
+-rw-r--r--   0 bernd     (1000) bernd     (1000)    34257 2023-04-16 18:39:39.785167 gerbolyze-3.1.5/PKG-INFO
+-rw-rw-rw-   0 bernd     (1000) bernd     (1000)    32441 2023-04-16 18:39:36.000000 gerbolyze-3.1.5/README.rst
+drwxr-xr-x   0 bernd     (1000) bernd     (1000)        0 2023-04-16 18:39:39.780166 gerbolyze-3.1.5/bin/
+-rw-rw-rw-   0 bernd     (1000) bernd     (1000)       92 2023-04-16 18:39:36.000000 gerbolyze-3.1.5/bin/gerbolyze
+drwxr-xr-x   0 bernd     (1000) bernd     (1000)        0 2023-04-16 18:39:39.782167 gerbolyze-3.1.5/gerbolyze/
+-rwxrwxrwx   0 bernd     (1000) bernd     (1000)    27183 2023-04-16 18:39:36.000000 gerbolyze-3.1.5/gerbolyze/__init__.py
+-rw-rw-rw-   0 bernd     (1000) bernd     (1000)       33 2023-04-16 18:39:36.000000 gerbolyze-3.1.5/gerbolyze/__main__.py
+-rw-rw-rw-   0 bernd     (1000) bernd     (1000)    23446 2023-04-16 18:39:36.000000 gerbolyze-3.1.5/gerbolyze/protoboard.py
+drwxr-xr-x   0 bernd     (1000) bernd     (1000)        0 2023-04-16 18:39:39.784167 gerbolyze-3.1.5/gerbolyze/tests/
+-rw-rw-rw-   0 bernd     (1000) bernd     (1000)        0 2023-04-16 18:39:36.000000 gerbolyze-3.1.5/gerbolyze/tests/__init__.py
+-rw-rw-rw-   0 bernd     (1000) bernd     (1000)     5159 2023-04-16 18:39:36.000000 gerbolyze-3.1.5/gerbolyze/tests/test_integration.py
+drwxr-xr-x   0 bernd     (1000) bernd     (1000)        0 2023-04-16 18:39:39.783167 gerbolyze-3.1.5/gerbolyze.egg-info/
+-rw-r--r--   0 bernd     (1000) bernd     (1000)    34257 2023-04-16 18:39:39.000000 gerbolyze-3.1.5/gerbolyze.egg-info/PKG-INFO
+-rw-r--r--   0 bernd     (1000) bernd     (1000)      349 2023-04-16 18:39:39.000000 gerbolyze-3.1.5/gerbolyze.egg-info/SOURCES.txt
+-rw-r--r--   0 bernd     (1000) bernd     (1000)        1 2023-04-16 18:39:39.000000 gerbolyze-3.1.5/gerbolyze.egg-info/dependency_links.txt
+-rw-r--r--   0 bernd     (1000) bernd     (1000)       66 2023-04-16 18:39:39.000000 gerbolyze-3.1.5/gerbolyze.egg-info/requires.txt
+-rw-r--r--   0 bernd     (1000) bernd     (1000)       10 2023-04-16 18:39:39.000000 gerbolyze-3.1.5/gerbolyze.egg-info/top_level.txt
+-rw-r--r--   0 bernd     (1000) bernd     (1000)       38 2023-04-16 18:39:39.785167 gerbolyze-3.1.5/setup.cfg
+-rwxrwxrwx   0 bernd     (1000) bernd     (1000)     2581 2023-04-16 18:39:36.000000 gerbolyze-3.1.5/setup.py
```

### Comparing `gerbolyze-3.1.4/LICENSE` & `gerbolyze-3.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gerbolyze-3.1.4/PKG-INFO` & `gerbolyze-3.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gerbolyze
-Version: 3.1.4
+Version: 3.1.5
 Summary: A high-resolution image-to-PCB converter. Gerbolyze plots SVG, PNG and JPG onto existing gerber files. It handles almost the full SVG spec and deals with text, path outlines, patterns, arbitrary paths with self-intersections and holes, etc. fully automatically. It can vectorize raster images both by contour tracing and by grayscale dithering. All processing is done at the vector level without intermediate conversions to raster images accurately preserving the input.
 Home-page: https://github.com/jaseg/gerbolyze
 Author: jaseg
 Author-email: gerbonara@jaseg.de
 License: AGPLv3
 Project-URL: Source Code, https://git.jaseg.de/gerbolyze
 Project-URL: Bug Tracker, https://github.com/jaseg/gerbolyze/issues
@@ -35,15 +35,15 @@
 patterns, dashes and transformations.
 
 Raster images can either be vectorized through contour tracing (like gerbolyze v1.0 did) or they can be embedded using
 high-resolution grayscale emulation while (mostly) guaranteeing trace/space design rules.
 
 Try gerbolyze online at https://dyna.kokoroyukuma.de/gerboweb
 
-.. figure:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.1.4/pics/pcbway_sample_02_small.jpg
+.. figure:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.1.5/pics/pcbway_sample_02_small.jpg
   :width: 800px
 
   Drawing by `トーコ Toko <https://twitter.com/fluffy2038/status/1317231121269104640>`__ converted using Gerbolyze and printed at PCBWay.
 
 
 Tooling for PCB art is quite limited in both open source and closed source ecosystems. Something as simple as putting a
 pretty picture on a PCB can be an extremely tedious task. Depending on the PCB tool used, various arcane incantations
@@ -55,15 +55,15 @@
 industry-standard Altium Designer. Gerbolyze is written with performance in mind and will happily vectorize tens of
 thousands of primitives, generating tens of megabytes of gerber code without crapping itself. With gerbolyze you can
 finally be confident that your PCB fab's toolchain will fall over before yours does if you overdo it with the high-poly
 anime silkscreen.
 
 Gerbolyze is based on gerbonara_.
 
-.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.1.4/pics/process-overview.png
+.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.1.5/pics/process-overview.png
   :width: 800px
 
 .. contents::
 
 Tl;dr: Produce high-quality artistic PCBs in three easy steps!
 --------------------------------------------------------------
 
@@ -140,15 +140,15 @@
     python3 setup.py install
 
 Features
 --------
 
 Input on the left, output on the right.
 
-.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.1.4/pics/test_svg_readme_composited.png
+.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.1.5/pics/test_svg_readme_composited.png
   :width: 800px
 
 * Almost full SVG 1.1 static spec coverage (!)
 
   * Paths with beziers, self-intersections and holes
   * Strokes, even with dashes and markers
   * Pattern fills and strokes
@@ -350,15 +350,15 @@
 Dashed strokes are supported on outline layers and can be used to make easy mouse bites.
 
 .. _subtraction_script:
 
 Subtraction scripts
 *******************
 
-.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.1.4/pics/subtract_example.png
+.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.1.5/pics/subtract_example.png
   :width: 800px
 
 Subtraction scripts tell ``gerbolyze paste`` to remove an area around certain input layers to from an overlay layer.
 When a input layer is given in the subtraction script, gerbolyze will dilate (extend outwards) everything on this input
 layer and remove it from the target overlay layer. By default, Gerbolyze subtracts the mask layer from the silk layer to
 make sure there are no silk primitives that overlap bare copper, and subtracts each input layer from its corresponding
 overlay to make sure the two do not overlap. In the picture above you can see both at work: The overlay contains
@@ -503,33 +503,33 @@
 
 .. for f in vec_*.png; convert -background white -gravity center $f -resize 500x500 -extent 500x500 (basename -s .png $f)-square.png; end
 .. for vec in hexgrid square poisson contours; convert vec_"$vec"_whole-square.png vec_"$vec"_detail-square.png -background transparent -splice 25x0+0+0 +append -chop 25x0+0+0 vec_"$vec"_composited.png; end
 
 ``--vectorizer poisson-disc`` (the default) 
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.1.4/pics/vec_poisson_composited.png
+.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.1.5/pics/vec_poisson_composited.png
   :width: 800px
 
 ``--vectorizer hex-grid``
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
-.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.1.4/pics/vec_hexgrid_composited.png
+.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.1.5/pics/vec_hexgrid_composited.png
   :width: 800px
 
 ``--vectorizer square-grid``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.1.4/pics/vec_square_composited.png
+.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.1.5/pics/vec_square_composited.png
   :width: 800px
 
 ``--vectorizer binary-contours``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.1.4/pics/vec_contours_composited.png
+.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.1.5/pics/vec_contours_composited.png
   :width: 800px
 
 The binary contours vectorizer requires a black-and-white binary input image. As you can see, like every bitmap tracer
 it will produce some artifacts. For artistic input this is usually not too bad as long as the input data is
 high-resolution. Antialiased edges in the input image are not only OK, they may even help with an accurate
 vectorization.
 
@@ -699,15 +699,15 @@
 
 A design rule checker is planned as a future addition to gerbolyze, but is not yet part of it. If in doubt, talk to your
 fab and consider doing a test run of your design before ordering assembled boards ;)
 
 Gallery
 -------
 
-.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.1.4/pics/sample3.jpg
+.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.1.5/pics/sample3.jpg
   :width: 400px
 
 For a demonstration of ``gerbolyze convert``, check out the `Gerbolyze Protoboard Index`_, where you can download gerber
 files for over 7.000 SMD and THT protoboard layouts.
 
 Licensing
 ---------
```

### Comparing `gerbolyze-3.1.4/README.rst` & `gerbolyze-3.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `gerbolyze-3.1.4/gerbolyze/__init__.py` & `gerbolyze-3.1.5/gerbolyze/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 from bs4 import BeautifulSoup
 import numpy as np
 import click
 
 import gerbonara as gn
 
-__version__ = '3.1.4'
+__version__ = '3.1.5'
 
 @click.group()
 def cli():
     pass
 
 @cli.command()
 @click.argument('input_gerbers', type=click.Path(exists=True, path_type=Path))
```

### Comparing `gerbolyze-3.1.4/gerbolyze/protoboard.py` & `gerbolyze-3.1.5/gerbolyze/protoboard.py`

 * *Files identical despite different names*

### Comparing `gerbolyze-3.1.4/gerbolyze/tests/test_integration.py` & `gerbolyze-3.1.5/gerbolyze/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `gerbolyze-3.1.4/gerbolyze.egg-info/PKG-INFO` & `gerbolyze-3.1.5/gerbolyze.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gerbolyze
-Version: 3.1.4
+Version: 3.1.5
 Summary: A high-resolution image-to-PCB converter. Gerbolyze plots SVG, PNG and JPG onto existing gerber files. It handles almost the full SVG spec and deals with text, path outlines, patterns, arbitrary paths with self-intersections and holes, etc. fully automatically. It can vectorize raster images both by contour tracing and by grayscale dithering. All processing is done at the vector level without intermediate conversions to raster images accurately preserving the input.
 Home-page: https://github.com/jaseg/gerbolyze
 Author: jaseg
 Author-email: gerbonara@jaseg.de
 License: AGPLv3
 Project-URL: Source Code, https://git.jaseg.de/gerbolyze
 Project-URL: Bug Tracker, https://github.com/jaseg/gerbolyze/issues
@@ -35,15 +35,15 @@
 patterns, dashes and transformations.
 
 Raster images can either be vectorized through contour tracing (like gerbolyze v1.0 did) or they can be embedded using
 high-resolution grayscale emulation while (mostly) guaranteeing trace/space design rules.
 
 Try gerbolyze online at https://dyna.kokoroyukuma.de/gerboweb
 
-.. figure:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.1.4/pics/pcbway_sample_02_small.jpg
+.. figure:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.1.5/pics/pcbway_sample_02_small.jpg
   :width: 800px
 
   Drawing by `トーコ Toko <https://twitter.com/fluffy2038/status/1317231121269104640>`__ converted using Gerbolyze and printed at PCBWay.
 
 
 Tooling for PCB art is quite limited in both open source and closed source ecosystems. Something as simple as putting a
 pretty picture on a PCB can be an extremely tedious task. Depending on the PCB tool used, various arcane incantations
@@ -55,15 +55,15 @@
 industry-standard Altium Designer. Gerbolyze is written with performance in mind and will happily vectorize tens of
 thousands of primitives, generating tens of megabytes of gerber code without crapping itself. With gerbolyze you can
 finally be confident that your PCB fab's toolchain will fall over before yours does if you overdo it with the high-poly
 anime silkscreen.
 
 Gerbolyze is based on gerbonara_.
 
-.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.1.4/pics/process-overview.png
+.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.1.5/pics/process-overview.png
   :width: 800px
 
 .. contents::
 
 Tl;dr: Produce high-quality artistic PCBs in three easy steps!
 --------------------------------------------------------------
 
@@ -140,15 +140,15 @@
     python3 setup.py install
 
 Features
 --------
 
 Input on the left, output on the right.
 
-.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.1.4/pics/test_svg_readme_composited.png
+.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.1.5/pics/test_svg_readme_composited.png
   :width: 800px
 
 * Almost full SVG 1.1 static spec coverage (!)
 
   * Paths with beziers, self-intersections and holes
   * Strokes, even with dashes and markers
   * Pattern fills and strokes
@@ -350,15 +350,15 @@
 Dashed strokes are supported on outline layers and can be used to make easy mouse bites.
 
 .. _subtraction_script:
 
 Subtraction scripts
 *******************
 
-.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.1.4/pics/subtract_example.png
+.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.1.5/pics/subtract_example.png
   :width: 800px
 
 Subtraction scripts tell ``gerbolyze paste`` to remove an area around certain input layers to from an overlay layer.
 When a input layer is given in the subtraction script, gerbolyze will dilate (extend outwards) everything on this input
 layer and remove it from the target overlay layer. By default, Gerbolyze subtracts the mask layer from the silk layer to
 make sure there are no silk primitives that overlap bare copper, and subtracts each input layer from its corresponding
 overlay to make sure the two do not overlap. In the picture above you can see both at work: The overlay contains
@@ -503,33 +503,33 @@
 
 .. for f in vec_*.png; convert -background white -gravity center $f -resize 500x500 -extent 500x500 (basename -s .png $f)-square.png; end
 .. for vec in hexgrid square poisson contours; convert vec_"$vec"_whole-square.png vec_"$vec"_detail-square.png -background transparent -splice 25x0+0+0 +append -chop 25x0+0+0 vec_"$vec"_composited.png; end
 
 ``--vectorizer poisson-disc`` (the default) 
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.1.4/pics/vec_poisson_composited.png
+.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.1.5/pics/vec_poisson_composited.png
   :width: 800px
 
 ``--vectorizer hex-grid``
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
-.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.1.4/pics/vec_hexgrid_composited.png
+.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.1.5/pics/vec_hexgrid_composited.png
   :width: 800px
 
 ``--vectorizer square-grid``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.1.4/pics/vec_square_composited.png
+.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.1.5/pics/vec_square_composited.png
   :width: 800px
 
 ``--vectorizer binary-contours``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.1.4/pics/vec_contours_composited.png
+.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.1.5/pics/vec_contours_composited.png
   :width: 800px
 
 The binary contours vectorizer requires a black-and-white binary input image. As you can see, like every bitmap tracer
 it will produce some artifacts. For artistic input this is usually not too bad as long as the input data is
 high-resolution. Antialiased edges in the input image are not only OK, they may even help with an accurate
 vectorization.
 
@@ -699,15 +699,15 @@
 
 A design rule checker is planned as a future addition to gerbolyze, but is not yet part of it. If in doubt, talk to your
 fab and consider doing a test run of your design before ordering assembled boards ;)
 
 Gallery
 -------
 
-.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.1.4/pics/sample3.jpg
+.. image:: https://gitlab.com/gerbolyze/gerbolyze/-/raw/v3.1.5/pics/sample3.jpg
   :width: 400px
 
 For a demonstration of ``gerbolyze convert``, check out the `Gerbolyze Protoboard Index`_, where you can download gerber
 files for over 7.000 SMD and THT protoboard layouts.
 
 Licensing
 ---------
```

### Comparing `gerbolyze-3.1.4/setup.py` & `gerbolyze-3.1.5/setup.py`

 * *Files identical despite different names*

