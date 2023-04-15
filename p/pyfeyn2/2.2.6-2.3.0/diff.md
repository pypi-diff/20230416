# Comparing `tmp/pyfeyn2-2.2.6.tar.gz` & `tmp/pyfeyn2-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfeyn2-2.2.6.tar", max compression
+gzip compressed data, was "pyfeyn2-2.3.0.tar", max compression
```

## Comparing `pyfeyn2-2.2.6.tar` & `pyfeyn2-2.3.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0    35149 2023-04-12 17:41:17.301008 pyfeyn2-2.2.6/LICENSE
--rw-r--r--   0        0        0     3115 2023-04-12 17:41:17.301008 pyfeyn2-2.2.6/README.md
--rw-r--r--   0        0        0      154 2023-04-12 17:41:17.377009 pyfeyn2-2.2.6/pyfeyn2/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 17:41:17.377009 pyfeyn2-2.2.6/pyfeyn2/auto/__init__.py
--rw-r--r--   0        0        0     2841 2023-04-12 17:41:17.377009 pyfeyn2-2.2.6/pyfeyn2/auto/bend.py
--rw-r--r--   0        0        0      774 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/auto/label.py
--rw-r--r--   0        0        0     2073 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/auto/position.py
--rw-r--r--   0        0        0        0 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/auto/reshuffle.py
--rw-r--r--   0        0        0     3332 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/feynmandiagram.py
--rw-r--r--   0        0        0     2742 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/interface/dot.py
--rw-r--r--   0        0        0      273 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/interface/hepmc.py
--rw-r--r--   0        0        0      238 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/interface/qgraf.py
--rw-r--r--   0        0        0      169 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/mkfeyndiag.py
--rw-r--r--   0        0        0        0 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/__init__.py
--rw-r--r--   0        0        0     3651 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/all.py
--rw-r--r--   0        0        0        0 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/latex/__init__.py
--rw-r--r--   0        0        0     3494 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/latex/dot.py
--rw-r--r--   0        0        0     5920 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/latex/feynmp.py
--rw-r--r--   0        0        0     1616 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/latex/latex.py
--rw-r--r--   0        0        0     2407 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/latex/metapost.py
--rw-r--r--   0        0        0     6302 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/latex/tikzfeynman.py
--rw-r--r--   0        0        0     6026 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/mpl/feynmanrender.py
--rw-r--r--   0        0        0        0 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/pyx/__init__.py
--rw-r--r--   0        0        0     7132 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/pyx/blobs.py
--rw-r--r--   0        0        0     1319 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/pyx/config.py
--rw-r--r--   0        0        0    13169 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/pyx/deco.py
--rw-r--r--   0        0        0     2561 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/pyx/diagrams.py
--rw-r--r--   0        0        0    41341 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/pyx/lines.py
--rw-r--r--   0        0        0     3549 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/pyx/paint.py
--rw-r--r--   0        0        0    12623 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/pyx/points.py
--rw-r--r--   0        0        0     8043 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/pyx/pyxrender.py
--rw-r--r--   0        0        0     1501 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/pyx/utils.py
--rw-r--r--   0        0        0     2914 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/render.py
--rw-r--r--   0        0        0     7120 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/text/ascii.py
--rw-r--r--   0        0        0      745 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/text/asciipdf.py
--rw-r--r--   0        0        0     2228 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/text/label.py
--rw-r--r--   0        0        0     1547 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/text/line.py
--rw-r--r--   0        0        0     1502 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/text/plainpdf.py
--rw-r--r--   0        0        0      483 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/text/point.py
--rw-r--r--   0        0        0     3846 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/text/style.py
--rw-r--r--   0        0        0     1401 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/text/unicode.py
--rw-r--r--   0        0        0     1858 2023-04-12 17:41:17.381009 pyfeyn2-2.2.6/pyfeyn2/render/text/unicodepdf.py
--rw-r--r--   0        0        0     2480 2023-04-12 17:41:19.381020 pyfeyn2-2.2.6/pyproject.toml
--rw-r--r--   0        0        0     4903 1970-01-01 00:00:00.000000 pyfeyn2-2.2.6/setup.py
--rw-r--r--   0        0        0     4775 1970-01-01 00:00:00.000000 pyfeyn2-2.2.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-15 22:22:39.919773 pyfeyn2-2.3.0/LICENSE
+-rw-r--r--   0        0        0     3115 2023-04-15 22:22:39.919773 pyfeyn2-2.3.0/README.md
+-rw-r--r--   0        0        0      154 2023-04-15 22:22:40.003773 pyfeyn2-2.3.0/pyfeyn2/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-15 22:22:40.003773 pyfeyn2-2.3.0/pyfeyn2/auto/__init__.py
+-rw-r--r--   0        0        0     2841 2023-04-15 22:22:40.003773 pyfeyn2-2.3.0/pyfeyn2/auto/bend.py
+-rw-r--r--   0        0        0      774 2023-04-15 22:22:40.003773 pyfeyn2-2.3.0/pyfeyn2/auto/label.py
+-rw-r--r--   0        0        0     2073 2023-04-15 22:22:40.003773 pyfeyn2-2.3.0/pyfeyn2/auto/position.py
+-rw-r--r--   0        0        0        0 2023-04-15 22:22:40.003773 pyfeyn2-2.3.0/pyfeyn2/auto/reshuffle.py
+-rw-r--r--   0        0        0     3332 2023-04-15 22:22:40.003773 pyfeyn2-2.3.0/pyfeyn2/feynmandiagram.py
+-rw-r--r--   0        0        0     2733 2023-04-15 22:22:40.003773 pyfeyn2-2.3.0/pyfeyn2/interface/dot.py
+-rw-r--r--   0        0        0      273 2023-04-15 22:22:40.003773 pyfeyn2-2.3.0/pyfeyn2/interface/hepmc.py
+-rw-r--r--   0        0        0      238 2023-04-15 22:22:40.003773 pyfeyn2-2.3.0/pyfeyn2/interface/qgraf.py
+-rw-r--r--   0        0        0     2691 2023-04-15 22:22:40.003773 pyfeyn2-2.3.0/pyfeyn2/mkfeyndiag.py
+-rw-r--r--   0        0        0        0 2023-04-15 22:22:40.003773 pyfeyn2-2.3.0/pyfeyn2/render/__init__.py
+-rw-r--r--   0        0        0     3657 2023-04-15 22:22:40.003773 pyfeyn2-2.3.0/pyfeyn2/render/all.py
+-rw-r--r--   0        0        0        0 2023-04-15 22:22:40.003773 pyfeyn2-2.3.0/pyfeyn2/render/latex/__init__.py
+-rw-r--r--   0        0        0     3638 2023-04-15 22:22:40.007773 pyfeyn2-2.3.0/pyfeyn2/render/latex/dot.py
+-rw-r--r--   0        0        0     5977 2023-04-15 22:22:40.007773 pyfeyn2-2.3.0/pyfeyn2/render/latex/feynmp.py
+-rw-r--r--   0        0        0     1616 2023-04-15 22:22:40.007773 pyfeyn2-2.3.0/pyfeyn2/render/latex/latex.py
+-rw-r--r--   0        0        0     2407 2023-04-15 22:22:40.007773 pyfeyn2-2.3.0/pyfeyn2/render/latex/metapost.py
+-rw-r--r--   0        0        0     6640 2023-04-15 22:22:40.007773 pyfeyn2-2.3.0/pyfeyn2/render/latex/tikzfeynman.py
+-rw-r--r--   0        0        0     7108 2023-04-15 22:22:40.007773 pyfeyn2-2.3.0/pyfeyn2/render/mpl/feynmanrender.py
+-rw-r--r--   0        0        0        0 2023-04-15 22:22:40.007773 pyfeyn2-2.3.0/pyfeyn2/render/pyx/__init__.py
+-rw-r--r--   0        0        0     7132 2023-04-15 22:22:40.007773 pyfeyn2-2.3.0/pyfeyn2/render/pyx/blobs.py
+-rw-r--r--   0        0        0     1319 2023-04-15 22:22:40.007773 pyfeyn2-2.3.0/pyfeyn2/render/pyx/config.py
+-rw-r--r--   0        0        0    13245 2023-04-15 22:22:40.007773 pyfeyn2-2.3.0/pyfeyn2/render/pyx/deco.py
+-rw-r--r--   0        0        0     2561 2023-04-15 22:22:40.007773 pyfeyn2-2.3.0/pyfeyn2/render/pyx/diagrams.py
+-rw-r--r--   0        0        0    41394 2023-04-15 22:22:40.007773 pyfeyn2-2.3.0/pyfeyn2/render/pyx/lines.py
+-rw-r--r--   0        0        0     3549 2023-04-15 22:22:40.007773 pyfeyn2-2.3.0/pyfeyn2/render/pyx/paint.py
+-rw-r--r--   0        0        0    12623 2023-04-15 22:22:40.007773 pyfeyn2-2.3.0/pyfeyn2/render/pyx/points.py
+-rw-r--r--   0        0        0     9184 2023-04-15 22:22:40.007773 pyfeyn2-2.3.0/pyfeyn2/render/pyx/pyxrender.py
+-rw-r--r--   0        0        0     1501 2023-04-15 22:22:40.007773 pyfeyn2-2.3.0/pyfeyn2/render/pyx/utils.py
+-rw-r--r--   0        0        0     2914 2023-04-15 22:22:40.007773 pyfeyn2-2.3.0/pyfeyn2/render/render.py
+-rw-r--r--   0        0        0     9026 2023-04-15 22:22:40.007773 pyfeyn2-2.3.0/pyfeyn2/render/text/ascii.py
+-rw-r--r--   0        0        0      863 2023-04-15 22:22:40.007773 pyfeyn2-2.3.0/pyfeyn2/render/text/asciipdf.py
+-rw-r--r--   0        0        0     2364 2023-04-15 22:22:40.007773 pyfeyn2-2.3.0/pyfeyn2/render/text/label.py
+-rw-r--r--   0        0        0     1701 2023-04-15 22:22:40.007773 pyfeyn2-2.3.0/pyfeyn2/render/text/line.py
+-rw-r--r--   0        0        0     2113 2023-04-15 22:22:40.007773 pyfeyn2-2.3.0/pyfeyn2/render/text/plainpdf.py
+-rw-r--r--   0        0        0      527 2023-04-15 22:22:40.007773 pyfeyn2-2.3.0/pyfeyn2/render/text/point.py
+-rw-r--r--   0        0        0     3846 2023-04-15 22:22:40.007773 pyfeyn2-2.3.0/pyfeyn2/render/text/style.py
+-rw-r--r--   0        0        0     1401 2023-04-15 22:22:40.007773 pyfeyn2-2.3.0/pyfeyn2/render/text/unicode.py
+-rw-r--r--   0        0        0     1976 2023-04-15 22:22:40.007773 pyfeyn2-2.3.0/pyfeyn2/render/text/unicodepdf.py
+-rw-r--r--   0        0        0     2511 2023-04-15 22:22:42.135772 pyfeyn2-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4903 1970-01-01 00:00:00.000000 pyfeyn2-2.3.0/setup.py
+-rw-r--r--   0        0        0     4775 1970-01-01 00:00:00.000000 pyfeyn2-2.3.0/PKG-INFO
```

### Comparing `pyfeyn2-2.2.6/LICENSE` & `pyfeyn2-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.6/README.md` & `pyfeyn2-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.6/pyfeyn2/auto/bend.py` & `pyfeyn2-2.3.0/pyfeyn2/auto/bend.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.6/pyfeyn2/auto/label.py` & `pyfeyn2-2.3.0/pyfeyn2/auto/label.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.6/pyfeyn2/auto/position.py` & `pyfeyn2-2.3.0/pyfeyn2/auto/position.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.6/pyfeyn2/feynmandiagram.py` & `pyfeyn2-2.3.0/pyfeyn2/feynmandiagram.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.6/pyfeyn2/interface/dot.py` & `pyfeyn2-2.3.0/pyfeyn2/interface/dot.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 def _fake_styler(fd, p):
     return 'style="draw=none"'
 
 
 def get_rankdir(fdstyle):
     rankdir = None
-    if fdstyle.getProperty("direction") is not None:
-        warn("direction is unknwon, using default of 'right'")
+    if fdstyle.getProperty("direction") is None:
+        warn("direction is unkown, using default of 'right'")
         rankdir = "LR"
     else:
         rdir = fdstyle.getProperty("direction").value
         if rdir == "right":
             rankdir = "LR"
         elif rdir == "left":
             rankdir = "RL"
@@ -27,15 +27,15 @@
         else:
             raise Exception(f"Unknown direction: {rdir}")
     return rankdir
 
 
 def get_layout(fdstyle):
     layout = None
-    if fdstyle.getProperty("layout") is not None:
+    if fdstyle.getProperty("layout") is None:
         warn("layout is unknwon, using default of 'dot'")
         layout = "dot"
     else:
         layout = fdstyle.getProperty("layout").value
     return layout
```

### Comparing `pyfeyn2-2.2.6/pyfeyn2/render/all.py` & `pyfeyn2-2.3.0/pyfeyn2/render/all.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 
 renders = {
     "tikz": TikzFeynmanRender,
     "pyx": PyxRender,
     "feynmp": FeynmpRender,
     "feynman": FeynmanRender,
     "dot": DotRender,
-    "ascii": ASCIIPDFRender,
-    "unicode": UnicodePDFRender,
+    "asciipdf": ASCIIPDFRender,
+    "unicodepdf": UnicodePDFRender,
 }
 
 
 class AllRender(LatexRender):
     """Render all diagrams to PDF."""
 
     def __init__(
```

### Comparing `pyfeyn2-2.2.6/pyfeyn2/render/latex/dot.py` & `pyfeyn2-2.3.0/pyfeyn2/render/latex/dot.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,19 +16,21 @@
 map_feyn_to_tikz = {
     "vector": "decorate,decoration=snake",
     "boson": "decorate,decoration=snake",
     "photon": "decorate,decoration=snake",
     "gluon": "decorate,decoration={coil,aspect=0.3,segment length=1mm}",
     "ghost": "dotted",
     "fermion": "decorate,postaction={decorate,draw,red,decoration={markings,mark=at position 0.5 with {\\arrow{>}}}}",
+    "anti fermion": "decorate,postaction={decorate,draw,red,decoration={markings,mark=at position 0.5 with {\\arrow{<}}}}",
     "higgs": "densely dashed",
     "scalar": "densely dashed",
     "slepton": "densely dashed",
     "squark": "densely dashed",
     "zigzag": "decorate,decoration=zigzag",
+    "line": "draw",
     "phantom": "draw=none",
 }
 
 
 def stylize_connect(fd: FeynmanDiagram, c: Connector) -> str:
     fstyle = fd.get_style(c)
     if fstyle.getProperty("line") is not None:
```

### Comparing `pyfeyn2-2.2.6/pyfeyn2/render/latex/feynmp.py` & `pyfeyn2-2.3.0/pyfeyn2/render/latex/feynmp.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from pyfeyn2 import feynmandiagram
 from pyfeyn2.feynmandiagram import Connector
 from pyfeyn2.render.latex.metapost import MetaPostRender
 
 # converte FeynmanDiagram to tikz-feynman
 
 type_map = {
+    "line": ["plain"],
     "gluon": ["gluon"],
     "curly": ["curly"],
     "dbl_curly": ["dbl_curly"],
     "dashes": ["dashes"],
     "scalar": ["scalar"],
     "dashes_arrow": ["dashes_arrow"],
     "dbl_dashes": ["dbl_dashes"],
@@ -23,15 +24,15 @@
     "dots_arrow": ["dots_arrow"],
     "ghost": ["ghost"],
     "dbl_dots": ["dbl_dots"],
     "dbl_dots_arrow": ["dbl_dots_arrow"],
     "phantom": ["phantom"],
     "phantom_arrow": ["phantom_arrow"],
     "plain": ["plain"],
-    "plain_arrow": ["plain_arrow"],
+    "plain_arrow": ["plain_arrkddow"],
     "fermion": ["fermion"],
     "anti fermion": ["fermion"],
     "electron": ["electron"],
     "quark": ["quark"],
     "double": ["double"],
     "dbl_plain": ["dbl_plain"],
     "double_arrow": ["double_arrow"],
@@ -123,17 +124,18 @@
                     lid = l.target
                     ltarget = l.id
                 if inward:
                     src += f"\t\t\\fmf{{{ttype}{style}}}{{{lid},{ltarget}}}\n"
                 else:
                     src += f"\t\t\\fmf{{{ttype}{style}}}{{{ltarget},{lid}}}\n"
                 style = ""
+        return src
 
-    do_legs(src, incoming, True)
-    do_legs(src, outgoing, False)
+    src = do_legs(src, incoming, True)
+    src = do_legs(src, outgoing, False)
 
     for p in fd.propagators:
         pstyle = fd.get_style(p)
         if pstyle.getProperty("line") is not None:
             tttype = type_map[pstyle.getProperty("line").value]
         else:
             tttype = p.type  # fallback to type if no line style is set
```

### Comparing `pyfeyn2-2.2.6/pyfeyn2/render/latex/latex.py` & `pyfeyn2-2.3.0/pyfeyn2/render/latex/latex.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.6/pyfeyn2/render/latex/metapost.py` & `pyfeyn2-2.3.0/pyfeyn2/render/latex/metapost.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.6/pyfeyn2/render/latex/tikzfeynman.py` & `pyfeyn2-2.3.0/pyfeyn2/render/latex/tikzfeynman.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import List
+from warnings import warn
 
 from pylatex import Command
 from pylatex.utils import NoEscape
 
 from pyfeyn2.feynmandiagram import Connector, FeynmanDiagram, Leg, Vertex
 from pyfeyn2.render.latex.latex import LatexRender
 
@@ -59,19 +60,24 @@
     if c.label is not None:
         ret += ",edge label=" + c.label
     # if c.edge_label_ is not None: style += ",edge label'=" + c.edge_label_
     if (
         style.getProperty("momentum-arrow") is not None
         and style.getProperty("momentum-arrow").value == "true"
     ):
-        if (
-            style.getProperty("momentum-arrow-flip") is not None
-            and style.getProperty("momentum-arrow-flip").value == "true"
-        ):
-            ret += ",momentum'=" + c.momentum.name
+        if style.getProperty("momentum-arrow-sense") is not None:
+            if style.getProperty("momentum-arrow-sense").value == -1:
+                ret += ",momentum'=" + c.momentum.name
+            elif style.getProperty("momentum-arrow-sense").value == 0:
+                warn(
+                    "momentum-arrow=true but momentum-arrow-sense=0, ignoring momentum-arrow"
+                )
+                pass
+            else:
+                ret += ",momentum=" + c.momentum.name
         else:
             ret += ",momentum=" + c.momentum.name
     if style.opacity is not None and style.opacity != "":
         ret += ",opacity=" + str(style.opacity)
     if style.color is not None and style.color != "":
         ret += "," + str(style.color)
     if style.getProperty("bend-direction") is not None:
@@ -194,14 +200,15 @@
             "opacity",
             "bend-direction",
             "bend-in",
             "bend-out",
             "bend-loop",
             "bend-min-distance",
             "momentum-arrow",
+            "momentum-arrow-sense",
         ]
 
     @classmethod
     def valid_attributes(cls) -> List[str]:
         return super(TikzFeynmanRender, cls).valid_attributes() + [
             "x",
             "y",
```

### Comparing `pyfeyn2-2.2.6/pyfeyn2/render/pyx/blobs.py` & `pyfeyn2-2.3.0/pyfeyn2/render/pyx/blobs.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.6/pyfeyn2/render/pyx/config.py` & `pyfeyn2-2.3.0/pyfeyn2/render/pyx/config.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.6/pyfeyn2/render/pyx/deco.py` & `pyfeyn2-2.3.0/pyfeyn2/render/pyx/deco.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,33 +22,36 @@
 ###########################################################################################
 
 
 ## Arrow decorator class
 class Arrow(pyx.deco.deco, pyx.attr.attr):
     """Arrow for Feynman diagram lines"""
 
-    def __init__(self, pos=0.5, size=6 * pyx.unit.v_pt, angle=45, constriction=0.8):
+    def __init__(
+        self, pos=0.5, size=6 * pyx.unit.v_pt, angle=45, constriction=0.8, sense=1
+    ):
         """Constructor."""
         self.pos = pos
         self.size = size
         self.angle = angle
         self.constriction = constriction
+        self.sense = sense
 
-    def decorate(self, dp):
+    def decorate(self, dp, textengine=None):
         """Attach arrow to a path (usually a line)."""
         dp.ensurenormpath()
         constrictionlen = (
             self.size * self.constriction * math.cos(self.angle * math.pi / 360.0)
         )
         arrowtopos = self.pos * dp.path.arclen() + 0.5 * self.size
         arrowtopath = dp.path.split(arrowtopos)[0]
         arrowpath = getarrowpath(
             arrowtopath,
             self.pos * dp.path.arclen(),
-            1,
+            self.sense,
             self.size,
             45,
             self.constriction,
             constrictionlen,
         )
         dp.ornaments.fill(arrowpath)
         return dp
```

### Comparing `pyfeyn2-2.2.6/pyfeyn2/render/pyx/diagrams.py` & `pyfeyn2-2.3.0/pyfeyn2/render/pyx/diagrams.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.6/pyfeyn2/render/pyx/lines.py` & `pyfeyn2-2.3.0/pyfeyn2/render/pyx/lines.py`

 * *Files 0% similar despite different names*

```diff
@@ -1321,16 +1321,18 @@
 NamedLine = {
     "line": Line,
     "higgs": Scalar,
     "photon": Vector,
     "vector": Vector,
     "gluon": Gluon,
     "fermion": Line,
+    "anti fermion": Line,
     "graviton": Graviton,
     "gaugino": Gaugino,
     "gluino": Gluino,
     "gravitino": Gravitino,
     "scalar": Scalar,
+    "anti scalar": Scalar,
     "ghost": Ghost,
     "phantom": Phantom,
     "boson": Vector,
 }
```

### Comparing `pyfeyn2-2.2.6/pyfeyn2/render/pyx/paint.py` & `pyfeyn2-2.3.0/pyfeyn2/render/pyx/paint.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.6/pyfeyn2/render/pyx/points.py` & `pyfeyn2-2.3.0/pyfeyn2/render/pyx/points.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.6/pyfeyn2/render/pyx/pyxrender.py` & `pyfeyn2-2.3.0/pyfeyn2/render/pyx/pyxrender.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+from warnings import warn
 
 import pyx
 from IPython.display import display
 from pyx import *
 from wand.image import Image as WImage
 
 # from pyfeyn2.feynmandiagram import Line, Point
@@ -29,15 +30,15 @@
         delete = False
         if file is None:
             file = "tmp.pdf"
             delete = True
         pyxfd = FeynDiagram()
         for v in self.fd.vertices:
             dp = DecoratedPoint(v.x, v.y)
-            dp = self.apply_layout(v.raw_style(), dp)
+            dp = self.apply_layout(self.fd.get_style(v).cssText.replace("\n", " "), dp)
             if v.label is not None:
                 dp.setFillstyles(PointLabel(dp, v.label, displace=3, angle=90))
             pyxfd.add(dp)
         for l in self.fd.legs:
             lstyle = self.fd.get_style(l)
             tar = self.fd.get_vertex(l.target)
             if lstyle.getProperty("line") is not None:
@@ -46,33 +47,32 @@
                 lname = l.type  # fallback to type
             if l.is_incoming():
                 nl = NamedLine[lname](Point(l.x, l.y), Point(tar.x, tar.y))
             elif l.is_outgoing():
                 nl = NamedLine[lname](Point(tar.x, tar.y), Point(l.x, l.y))
             if lstyle.getProperty("bend") is not None:
                 nl = nl.bend(lstyle.getProperty("bend").value)
-            nl = self.apply_layout(v.raw_style(), nl)
+            nl = self.apply_layout(self.fd.get_style(l).cssText.replace("\n", " "), nl)
             nl = nl.addLabel(l.label)
 
         for p in self.fd.propagators:
             pstyle = self.fd.get_style(p)
             src = self.fd.get_vertex(p.source)
             tar = self.fd.get_vertex(p.target)
             if pstyle.getProperty("line") is not None:
                 lname = pstyle.getProperty("line").value
             else:
                 lname = p.type
             nl = NamedLine[lname](Point(src.x, src.y), Point(tar.x, tar.y))
-            print(nl, lname)
             if pstyle.getProperty("bend") is not None:
                 nl = nl.bend(pstyle.getProperty("bend").value)
-            nl = self.apply_layout(v.raw_style(), nl)
+            nl = self.apply_layout(self.fd.get_style(p).cssText.replace("\n", " "), nl)
             nl = nl.addLabel(p.label)
         pyxfd.draw(file)
-        print("Drawing to %s" % file)
+        # print("Drawing to %s" % file)
         wi = WImage(filename=file, resolution=resolution, width=width, height=height)
         if delete:
             os.remove(file)
         if show:
             display(wi)
         if clean_up:
             # TODO: clean up
@@ -118,14 +118,16 @@
                 marksize = 0.075
             obj.setMark(marktype(size=marksize))
         if (
             "arrow-size" in styledict
             or "arrow-angle" in styledict
             or "arrow-constrict" in styledict
             or "arrow-pos" in styledict
+            or "arrow-sense" in styledict
+            or "arrow-displace" in styledict
         ) and isinstance(obj, Line):
             try:
                 arrsize = pyx.unit.length(float(styledict["arrow-size"]), unit="cm")
             except Exception:
                 arrsize = 6 * pyx.unit.v_pt
             try:
                 arrangle = float(styledict["arrow-angle"])
@@ -135,17 +137,32 @@
                 arrconstrict = float(styledict["arrow-constrict"])
             except Exception:
                 arrconstrict = 0.8
             try:
                 arrpos = float(styledict["arrow-pos"])
             except Exception:
                 arrpos = 0.5
-            obj.addArrow(arrow=Arrow(arrpos, arrsize, arrangle, arrconstrict))
+            try:
+                arrsense = float(styledict["arrow-sense"])
+            except Exception:
+                arrsense = 1
+            if arrsense == 1 or arrsense == -1:
+                obj.addArrow(
+                    arrow=Arrow(arrpos, arrsize, arrangle, arrconstrict, arrsense)
+                )
+            elif arrsense == 0:
+                # no arrow
+                pass
+            else:
+                warn("arrow-sense must be 1, -1 or 0 (no arrow).")
+            # obj.addArrow(arrow=Arrow(arrpos, arrsize, arrangle, arrconstrict, arrsense))
         if (
-            "parallel-arrow-size" in styledict
+            "momentum-arrow" in styledict
+            or "momentum-arrow-sense" in styledict
+            or "parallel-arrow-size" in styledict
             or "parallel-arrow-angle" in styledict
             or "parallel-arrow-constrict" in styledict
             or "parallel-arrow-pos" in styledict
             or "parallel-arrow-length" in styledict
             or "parallel-arrow-displace" in styledict
             or "parallel-arrow-sense" in styledict
         ) and isinstance(obj, Line):
@@ -172,20 +189,30 @@
             except Exception:
                 arrlen = 0.5 * pyx.unit.v_cm
             try:
                 arrdisp = float(styledict["parallel-arrow-displace"])
             except Exception:
                 arrdisp = 0.3
             try:
-                arrsense = int(styledict["parallel-arrow-sense"])
+                arrsense = int(styledict["momentum-arrow-sense"])
             except Exception:
                 arrsense = +1
-            obj.addParallelArrow(
-                arrpos, arrdisp, arrlen, arrsize, arrangle, arrconstrict, arrsense
-            )
+                try:
+                    arrsense = int(styledict["parallel-arrow-sense"])
+                except Exception:
+                    arrsense = +1
+            if arrsense == 1 or arrsense == -1:
+                obj.addParallelArrow(
+                    arrpos, arrdisp, arrlen, arrsize, arrangle, arrconstrict, arrsense
+                )
+            elif arrsense == 0:
+                # no arrow
+                pass
+            else:
+                warn("momentum-arrow-sense must be 1, -1 or 0 (no arrow).")
         if "is3d" in styledict and isinstance(obj, Line):
             fwords = ["0", "no", "false", "f", "off"]
             twords = ["1", "yes", "true", "t", "on"]
             if styledict["is3d"].lstrip().lower() in fwords:
                 obj.set3D(False)
             elif styledict["is3d"].lstrip().lower() in twords:
                 obj.set3D(True)
@@ -207,10 +234,12 @@
 
     @classmethod
     def valid_styles(cls):
         return super(PyxRender, cls).valid_styles() + [
             "line",
             "bend",
             "arrow-pos",
-            # "arrow-sense",  #           "parallel-arrow-sense",
-            # "arrow-displace",  #           "parallel-arrow-displace",
+            "arrow-sense",
+            "arrow-size",
+            "arrow-angle",
+            "arrow-constrict",
         ]
```

### Comparing `pyfeyn2-2.2.6/pyfeyn2/render/pyx/utils.py` & `pyfeyn2-2.3.0/pyfeyn2/render/pyx/utils.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.6/pyfeyn2/render/render.py` & `pyfeyn2-2.3.0/pyfeyn2/render/render.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.6/pyfeyn2/render/text/asciipdf.py` & `pyfeyn2-2.3.0/pyfeyn2/render/text/asciipdf.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,11 +18,18 @@
         file=None,
         show=True,
         resolution=100,
         width=None,
         height=None,
         clean_up=True,
     ):
-        ASCIIRender.render(self, file, show, resolution, width, height)
+        ASCIIRender.render(
+            self,
+            file=None,
+            show=False,
+            resolution=resolution,
+            width=width,
+            height=height,
+        )
         return PlainPDFRender.render(
             self, file, show, resolution, width, height, clean_up
         )
```

### Comparing `pyfeyn2-2.2.6/pyfeyn2/render/text/label.py` & `pyfeyn2-2.3.0/pyfeyn2/render/text/label.py`

 * *Files 21% similar despite different names*

```diff
@@ -33,15 +33,26 @@
             .replace("}", "")
             .replace("\\(", "")
             .replace("\\)", "")
             .replace("\\", "")
             .replace("^", "")
         )
 
-    def draw(self, pane, isrc, itar, scalex=1, scaley=1, kickx=0, kicky=0):
+    def draw(
+        self,
+        pane,
+        isrc,
+        itar,
+        scalex=1,
+        scaley=1,
+        kickx=0,
+        kicky=0,
+        colorer=lambda x: x,
+        **kwargs
+    ):
         jsrc = copy.copy(isrc)
         jtar = copy.copy(itar)
 
         # reduce length to 1/3 in the middle
         jsrc.x = (itar.x - isrc.x) / 3.0 + isrc.x
         jsrc.y = (itar.y - isrc.y) / 3.0 + isrc.y
         jtar.x = (itar.x - isrc.x) / 3.0 * 2.0 + isrc.x
@@ -67,9 +78,9 @@
                 jsrc.x -= shift / scalex
                 jtar.x -= shift / scalex
             # down to up -> shift right
             else:
                 jsrc.x += shift / scalex
                 jtar.x += shift / scalex
 
-        super().draw(pane, jsrc, jtar, scalex, scaley, kickx, kicky)
+        super().draw(pane, jsrc, jtar, scalex, scaley, kickx, kicky, colorer, **kwargs)
         self.index = 0
```

### Comparing `pyfeyn2-2.2.6/pyfeyn2/render/text/line.py` & `pyfeyn2-2.3.0/pyfeyn2/render/text/line.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,39 +5,50 @@
         begin=" ",
         end=" ",
     ):
         self.begin = begin
         self.end = end
         self.style = style
 
-    def draw(self, pane, isrc, itar, scalex=1, scaley=1, kickx=0, kicky=0):
+    def draw(
+        self,
+        pane,
+        isrc,
+        itar,
+        scalex=1,
+        scaley=1,
+        kickx=0,
+        kicky=0,
+        colorer=lambda x: x,
+        **kwargs,
+    ):
         # width = len(pane[0])
         # height = len(pane)
         # TODO normalize to width and height as well
         srcx = int((isrc.x + kickx) * scalex)
         srcy = int((isrc.y + kicky) * scaley)
         tarx = int((itar.x + kickx) * scalex)
         tary = int((itar.y + kicky) * scaley)
 
         if abs(srcx - tarx) > abs(srcy - tary):
             for i in range(srcx, tarx, 1 if srcx < tarx else -1):
                 v = self.style.next(tarx - srcx, tary - srcy)
                 if v is not None:
                     pane[round(srcy + (tary - srcy) * (i - srcx) / (-srcx + tarx))][
                         i
-                    ] = v
+                    ] = colorer(v)
         else:
             for i in range(srcy, tary, 1 if srcy < tary else -1):
                 v = self.style.next(tarx - srcx, tary - srcy)
                 if v is not None:
                     pane[i][
                         round(srcx + (tarx - srcx) * (i - srcy) / (-srcy + tary))
-                    ] = v
+                    ] = colorer(v)
         # call once to increase the index
         v = self.style.next(tarx - srcx, tary - srcy)
 
         if v is None:
             return
         if self.begin is not None and self.begin != "":
-            pane[srcy][srcx] = self.begin
+            pane[srcy][srcx] = colorer(self.begin)
         if self.end is not None and self.end != "":
-            pane[tary][tarx] = self.end
+            pane[tary][tarx] = colorer(self.end)
```

### Comparing `pyfeyn2-2.2.6/pyfeyn2/render/text/plainpdf.py` & `pyfeyn2-2.3.0/pyfeyn2/render/text/plainpdf.py`

 * *Files 20% similar despite different names*

```diff
@@ -23,17 +23,38 @@
             fd,
             documentclass=documentclass,
             document_options=document_options,
             *args,
             **kwargs,
         )
         self.preamble.append(Command("usepackage", NoEscape("listings")))
+        self.preamble.append(Command("usepackage", NoEscape("xcolor")))
         self.environment = environment
         self.environment_arg = environment_arg
 
+    def get_color_text(self, text, color):
+        """
+        Return text with color via LaTeX commands.
+        """
+        self.preamble.append(
+            Command(
+                "lstset",
+                NoEscape(
+                    "moredelim=[is][\color{"
+                    + color
+                    + "}]{@"
+                    + color
+                    + "!}{!"
+                    + color
+                    + "@}"
+                ),
+            )
+        )
+        return "@" + color + "!" + text + "!" + color + "@"
+
     def render(
         self,
         file=None,
         show=True,
         resolution=100,
         width=None,
         height=None,
```

### Comparing `pyfeyn2-2.2.6/pyfeyn2/render/text/style.py` & `pyfeyn2-2.3.0/pyfeyn2/render/text/style.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.6/pyfeyn2/render/text/unicode.py` & `pyfeyn2-2.3.0/pyfeyn2/render/text/unicode.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.2.6/pyfeyn2/render/text/unicodepdf.py` & `pyfeyn2-2.3.0/pyfeyn2/render/text/unicodepdf.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,11 +57,18 @@
         file=None,
         show=True,
         resolution=100,
         width=None,
         height=None,
         clean_up=True,
     ):
-        UnicodeRender.render(self, file, show, resolution, width, height)
+        UnicodeRender.render(
+            self,
+            file=None,
+            show=False,
+            resolution=resolution,
+            width=width,
+            height=height,
+        )
         return PlainPDFRender.render(
             self, file, show, resolution, width, height, clean_up
         )
```

### Comparing `pyfeyn2-2.2.6/pyproject.toml` & `pyfeyn2-2.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyfeyn2"
-version = "2.2.6"
+version = "2.3.0"
 description = "PyFeyn is a package which makes drawing Feynman diagrams simple and programmatic.  Feynman diagrams are important constructs in perturbative field theory, so being able to draw them in a programmatic fashion is important if attempting to enumerate a large number of diagram configurations is important. The output quality of PyFeyn diagrams (into PDF or EPS formats) is very high, and special effects can be obtained by using constructs from PyX, which PyFeyn is based around"
 authors = ["Alexander Puck Neuwirth <alexander@neuwirth-informatik.de>"]
 readme = "README.md"
 repository = "https://github.com/APN-Pucky/pyfeyn2"
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -25,15 +25,15 @@
 ipyparallel = "*"
 deprecated = "*"
 deprecation = "*"
 cssselect ="*"
 smpl_io = "*"
 smpl_doc = "*"
 smpl_util= "*"
-feynml = {version = ">=0.1.3", extras = ["interface"]}
+feynml = {version = ">=0.1.6", extras = ["interface"]}
 #feynml= {path= "../feynml", develop = true }
 
 [tool.poetry.scripts]
 mkfeyndiag = "pyfeyn2.mkfeyndiag:main"
 
 [tool.poetry.group.docs]
 optional = true
@@ -44,14 +44,16 @@
 sphinxcontrib-napoleon = "*"
 nbsphinx = "*"
 jupyter-sphinx = "*"
 sphinx_autobuild = "*"
 sphinx_math_dollar = "*"
 myst-parser  = "*"
 toml = "*"
+colorama = "*"
+termcolor = "*"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^2.20.0"
 pytest = "*"
```

### Comparing `pyfeyn2-2.2.6/setup.py` & `pyfeyn2-2.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ['Wand',
  'cssselect',
  'cssutils',
  'deprecated',
  'deprecation',
  'dot2tex',
  'feynman>=2.0,<3.0',
- 'feynml[interface]>=0.1.3',
+ 'feynml[interface]>=0.1.6',
  'graphviz',
  'ipyparallel',
  'matplotlib>=1.4.0,<4.0.0',
  'numpy>=1.6,<1.24',
  'particle',
  'pydot',
  'pygments',
@@ -39,15 +39,15 @@
  'xsdata[cli,lxml,soap]']
 
 entry_points = \
 {'console_scripts': ['mkfeyndiag = pyfeyn2.mkfeyndiag:main']}
 
 setup_kwargs = {
     'name': 'pyfeyn2',
-    'version': '2.2.6',
+    'version': '2.3.0',
     'description': 'PyFeyn is a package which makes drawing Feynman diagrams simple and programmatic.  Feynman diagrams are important constructs in perturbative field theory, so being able to draw them in a programmatic fashion is important if attempting to enumerate a large number of diagram configurations is important. The output quality of PyFeyn diagrams (into PDF or EPS formats) is very high, and special effects can be obtained by using constructs from PyX, which PyFeyn is based around',
     'long_description': "# PyFeyn2\n\nForked from <https://pyfeyn.hepforge.org/> \n\nPyFeyn is a Python-language based system for drawing Feynman diagrams. It was inspired by the C++ FeynDiagram system, and aims to provide the same functionality and quality of output as that, with the added benefits of a modern interpreted language, an improved interface and output direct to both EPS and PDF. Behind the scenes, PyFeyn uses the excellent PyX system - you can use PyX constructs in PyFeyn diagrams if you want, too.\n\n[![PyPI version][pypi image]][pypi link] [![PyPI version][pypi versions]][pypi link]  ![downloads](https://img.shields.io/pypi/dm/pyfeyn2.svg)\n\n[![test][a t image]][a t link]      [![Coverage Status][c t i]][c t l]  [![Codacy Badge][cc c i]][cc c l]   [![Codacy Badge][cc q i]][cc q l]  [![Documentation][rtd t i]][rtd t l]\n\n## Dependencies\n\n*   libmagickwand-dev (to display pdfs in a jupyter-notebook, might require a policy change of the imagemagick config for PDFs, see Troubleshooting)\n*   ghostscript\n*   latexmk\n*   (graphviz)\n*   (feynmp-auto/feynmf)\n\n## Installation\n\n```sh\npoerty install --with docs --with dev\npoetry shell\n```\n\n## Documentation\n\n*   <https://pyfeyn2.readthedocs.io/en/stable/>\n*   <https://apn-pucky.github.io/pyfeyn2/index.html>\n\n## Similar Feynman diagram rendering project:\n\n*   <https://github.com/ndeutschmann/qgraf-xml-drawer>\n*   <https://github.com/GkAntonius/feynman>\n*   <https://github.com/JP-Ellis/tikz-feynman>\n*   <https://pyfeyn.hepforge.org/> \n*   <https://feynml.hepforge.org/>\n*   <http://www.feyndiagram.com/>\n\nSeveral of these are integrated into pyfeyn2.\n\n## Troubleshooting\n\n*   [ImageMagick security policy 'PDF' blocking conversion]( https://stackoverflow.com/questions/52998331/imagemagick-security-policy-pdf-blocking-conversion )\n\n## Development\n\n\n### package/python structure:\n\n*   <https://mathspp.com/blog/how-to-create-a-python-package-in-2022>\n*   <https://www.brainsorting.com/posts/publish-a-package-on-pypi-using-poetry/>\n\n[pypi image]: https://badge.fury.io/py/pyfeyn2.svg\n[pypi link]: https://pypi.org/project/pyfeyn2/\n[pypi versions]: https://img.shields.io/pypi/pyversions/pyfeyn2.svg\n\n[a t link]: https://github.com/APN-Pucky/pyfeyn2/actions/workflows/test.yml\n[a t image]: https://github.com/APN-Pucky/pyfeyn2/actions/workflows/test.yml/badge.svg\n\n[cc q i]: https://app.codacy.com/project/badge/Grade/135bae47c6344ab0bfb180135ea1db44\n[cc q l]: https://www.codacy.com/gh/APN-Pucky/pyfeyn2/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=APN-Pucky/pyfeyn2&amp;utm_campaign=Badge_Grade\n[cc c i]: https://app.codacy.com/project/badge/Coverage/135bae47c6344ab0bfb180135ea1db44\n[cc c l]: https://www.codacy.com/gh/APN-Pucky/pyfeyn2/dashboard?utm_source=github.com&utm_medium=referral&utm_content=APN-Pucky/pyfeyn2&utm_campaign=Badge_Coverage\n\n[c t l]: https://coveralls.io/github/APN-Pucky/pyfeyn2?branch=master\n[c t i]: https://coveralls.io/repos/github/APN-Pucky/pyfeyn2/badge.svg?branch=master\n\n[rtd t i]: https://readthedocs.org/projects/pyfeyn2/badge/?version=latest\n[rtd t l]: https://pyfeyn2.readthedocs.io/en/latest/?badge=latest\n",
     'author': 'Alexander Puck Neuwirth',
     'author_email': 'alexander@neuwirth-informatik.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/APN-Pucky/pyfeyn2',
```

### Comparing `pyfeyn2-2.2.6/PKG-INFO` & `pyfeyn2-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfeyn2
-Version: 2.2.6
+Version: 2.3.0
 Summary: PyFeyn is a package which makes drawing Feynman diagrams simple and programmatic.  Feynman diagrams are important constructs in perturbative field theory, so being able to draw them in a programmatic fashion is important if attempting to enumerate a large number of diagram configurations is important. The output quality of PyFeyn diagrams (into PDF or EPS formats) is very high, and special effects can be obtained by using constructs from PyX, which PyFeyn is based around
 Home-page: https://github.com/APN-Pucky/pyfeyn2
 Author: Alexander Puck Neuwirth
 Author-email: alexander@neuwirth-informatik.de
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -14,15 +14,15 @@
 Requires-Dist: Wand
 Requires-Dist: cssselect
 Requires-Dist: cssutils
 Requires-Dist: deprecated
 Requires-Dist: deprecation
 Requires-Dist: dot2tex
 Requires-Dist: feynman (>=2.0,<3.0)
-Requires-Dist: feynml[interface] (>=0.1.3)
+Requires-Dist: feynml[interface] (>=0.1.6)
 Requires-Dist: graphviz
 Requires-Dist: ipyparallel
 Requires-Dist: matplotlib (>=1.4.0,<4.0.0)
 Requires-Dist: numpy (>=1.6,<1.24)
 Requires-Dist: particle
 Requires-Dist: pydot
 Requires-Dist: pygments
```

