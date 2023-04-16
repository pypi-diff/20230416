# Comparing `tmp/calendar_widget-1.0.0.tar.gz` & `tmp/calendar_widget-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calendar_widget-1.0.0.tar", last modified: Sat Apr 15 02:39:17 2023, max compression
+gzip compressed data, was "calendar_widget-1.0.1.tar", last modified: Sun Apr 16 14:30:49 2023, max compression
```

## Comparing `calendar_widget-1.0.0.tar` & `calendar_widget-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 02:39:17.312541 calendar_widget-1.0.0/
--rw-rw-rw-   0        0        0    26526 2023-04-14 15:16:21.000000 calendar_widget-1.0.0/LICENSE.md
--rw-rw-rw-   0        0        0     5816 2023-04-15 02:39:17.297025 calendar_widget-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     4995 2023-04-15 02:32:47.000000 calendar_widget-1.0.0/README.md
--rw-rw-rw-   0        0        0      763 2023-04-15 02:37:10.000000 calendar_widget-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-15 02:39:17.312541 calendar_widget-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-15 02:39:17.093774 calendar_widget-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-15 02:39:17.171909 calendar_widget-1.0.0/src/calendar_widget/
--rw-rw-rw-   0        0        0    32465 2023-04-14 15:16:21.000000 calendar_widget-1.0.0/src/calendar_widget/Calendar_Widget.py
--rw-rw-rw-   0        0        0       37 2023-04-15 01:39:22.000000 calendar_widget-1.0.0/src/calendar_widget/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-15 02:39:17.250141 calendar_widget-1.0.0/src/calendar_widget.egg-info/
--rw-rw-rw-   0        0        0     5816 2023-04-15 02:39:17.000000 calendar_widget-1.0.0/src/calendar_widget.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2023-04-15 02:39:17.000000 calendar_widget-1.0.0/src/calendar_widget.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 02:39:17.000000 calendar_widget-1.0.0/src/calendar_widget.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-15 02:39:17.000000 calendar_widget-1.0.0/src/calendar_widget.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 14:30:49.478744 calendar_widget-1.0.1/
+-rw-rw-rw-   0        0        0    26526 2023-04-14 15:16:21.000000 calendar_widget-1.0.1/LICENSE.md
+-rw-rw-rw-   0        0        0     5816 2023-04-16 14:30:49.478744 calendar_widget-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4995 2023-04-15 03:23:35.000000 calendar_widget-1.0.1/README.md
+-rw-rw-rw-   0        0        0      763 2023-04-16 14:30:02.000000 calendar_widget-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-16 14:30:49.478744 calendar_widget-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-16 14:30:49.369363 calendar_widget-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-16 14:30:49.431869 calendar_widget-1.0.1/src/calendar_widget/
+-rw-rw-rw-   0        0        0    32351 2023-04-16 14:28:58.000000 calendar_widget-1.0.1/src/calendar_widget/Calendar_Widget.py
+-rw-rw-rw-   0        0        0       37 2023-04-15 01:39:22.000000 calendar_widget-1.0.1/src/calendar_widget/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 14:30:49.478744 calendar_widget-1.0.1/src/calendar_widget.egg-info/
+-rw-rw-rw-   0        0        0     5816 2023-04-16 14:30:49.000000 calendar_widget-1.0.1/src/calendar_widget.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2023-04-16 14:30:49.000000 calendar_widget-1.0.1/src/calendar_widget.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 14:30:49.000000 calendar_widget-1.0.1/src/calendar_widget.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-16 14:30:49.000000 calendar_widget-1.0.1/src/calendar_widget.egg-info/top_level.txt
```

### Comparing `calendar_widget-1.0.0/LICENSE.md` & `calendar_widget-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `calendar_widget-1.0.0/PKG-INFO` & `calendar_widget-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calendar_widget
-Version: 1.0.0
+Version: 1.0.1
 Summary: Calendar widget for use with python tkinter
 Author-email: Spartanlasergun <bns360@live.com>
 Project-URL: Homepage, https://github.com/Spartanlasergun/calendar_widget
 Project-URL: Bug Tracker, https://github.com/Spartanlasergun/calendar_widget/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `calendar_widget-1.0.0/README.md` & `calendar_widget-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `calendar_widget-1.0.0/pyproject.toml` & `calendar_widget-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "calendar_widget"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Spartanlasergun", email="bns360@live.com" },
 ]
 description = "Calendar widget for use with python tkinter"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `calendar_widget-1.0.0/src/calendar_widget/Calendar_Widget.py` & `calendar_widget-1.0.1/src/calendar_widget/Calendar_Widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,23 +60,18 @@
             self.date_text_fill = "white"
             self.trail_box_fill = "gray20"
             self.trail_text_fill = "gray60"
             self.date_highlight = "lime"
             self.text_highlight_fill = "black"
 
 
-        # The minimum width of the calendar object is set at 300 pixels. The depth and the padding are both factors of
+        # The default width of the calendar object is set at 300 pixels. The depth and the padding are both factors of
         # the width.
-        if size < 300:
-            size = 300
-        size = size
         depth = (0.666 * size)
-        depth = depth
         padding = int(size * 0.03333)
-        padding = padding
 
         # create the tkinter canvas onto which the calendar will be created
         self.Calendar = tkinter.Canvas(window_name, width=size, height=depth,
                                        background=background, relief=calendar_relief)
 
         # position the calendar with the default "pack" option or according the user specified x and y coordinates
         if (pos_x == 0) and (pos_y == 0):
```

### Comparing `calendar_widget-1.0.0/src/calendar_widget.egg-info/PKG-INFO` & `calendar_widget-1.0.1/src/calendar_widget.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calendar-widget
-Version: 1.0.0
+Version: 1.0.1
 Summary: Calendar widget for use with python tkinter
 Author-email: Spartanlasergun <bns360@live.com>
 Project-URL: Homepage, https://github.com/Spartanlasergun/calendar_widget
 Project-URL: Bug Tracker, https://github.com/Spartanlasergun/calendar_widget/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

