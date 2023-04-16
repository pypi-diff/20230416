# Comparing `tmp/lbutils-mp-0.2.3.tar.gz` & `tmp/lbutils-mp-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lbutils-mp-0.2.3.tar", last modified: Sat Apr 15 10:21:12 2023, max compression
+gzip compressed data, was "lbutils-mp-0.2.4.tar", last modified: Sun Apr 16 19:40:19 2023, max compression
```

## Comparing `lbutils-mp-0.2.3.tar` & `lbutils-mp-0.2.4.tar`

### file list

```diff
@@ -1,42 +1,41 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-15 10:21:12.860083 lbutils-mp-0.2.3/
--rw-rw-r--   0 david     (1000) david     (1000)     1064 2023-03-28 09:54:55.000000 lbutils-mp-0.2.3/LICENCE
--rw-rw-r--   0 david     (1000) david     (1000)     6193 2023-04-15 10:21:12.860083 lbutils-mp-0.2.3/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)     5583 2023-04-13 07:19:57.000000 lbutils-mp-0.2.3/README.md
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-15 10:21:12.856083 lbutils-mp-0.2.3/lbutils/
--rw-rw-r--   0 david     (1000) david     (1000)     2911 2023-04-13 06:53:45.000000 lbutils-mp-0.2.3/lbutils/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     1456 2023-04-13 06:56:17.000000 lbutils-mp-0.2.3/lbutils/abc.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-15 10:21:12.856083 lbutils-mp-0.2.3/lbutils/drivers/
--rw-rw-r--   0 david     (1000) david     (1000)     2256 2023-04-13 06:48:47.000000 lbutils-mp-0.2.3/lbutils/drivers/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     8527 2023-04-13 07:51:03.000000 lbutils-mp-0.2.3/lbutils/drivers/seven_segment.py
--rw-rw-r--   0 david     (1000) david     (1000)    12530 2023-04-13 07:50:12.000000 lbutils-mp-0.2.3/lbutils/drivers/seven_segment_hex.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-15 10:21:12.856083 lbutils-mp-0.2.3/lbutils/examples/
--rw-rw-r--   0 david     (1000) david     (1000)     2291 2023-04-13 06:59:17.000000 lbutils-mp-0.2.3/lbutils/examples/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-15 10:21:12.856083 lbutils-mp-0.2.3/lbutils/graphics/
--rw-rw-r--   0 david     (1000) david     (1000)     4632 2023-04-13 06:44:10.000000 lbutils-mp-0.2.3/lbutils/graphics/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)    25143 2023-04-15 10:13:15.000000 lbutils-mp-0.2.3/lbutils/graphics/canvas.py
--rw-rw-r--   0 david     (1000) david     (1000)    11384 2023-04-15 10:13:15.000000 lbutils-mp-0.2.3/lbutils/graphics/colours.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-15 10:21:12.860083 lbutils-mp-0.2.3/lbutils/graphics/fonts/
--rw-rw-r--   0 david     (1000) david     (1000)     2903 2023-04-12 21:25:04.000000 lbutils-mp-0.2.3/lbutils/graphics/fonts/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     8797 2023-04-12 21:21:45.000000 lbutils-mp-0.2.3/lbutils/graphics/fonts/base_font.py
--rw-rw-r--   0 david     (1000) david     (1000)    10858 2023-04-12 17:06:52.000000 lbutils-mp-0.2.3/lbutils/graphics/fonts/font06.py
--rw-rw-r--   0 david     (1000) david     (1000)    13731 2023-04-12 17:06:52.000000 lbutils-mp-0.2.3/lbutils/graphics/fonts/font08.py
--rw-rw-r--   0 david     (1000) david     (1000)    12653 2023-04-13 21:29:43.000000 lbutils-mp-0.2.3/lbutils/graphics/fonts/org_01.py
--rw-rw-r--   0 david     (1000) david     (1000)    14044 2023-04-15 10:13:15.000000 lbutils-mp-0.2.3/lbutils/graphics/helpers.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-15 10:21:12.860083 lbutils-mp-0.2.3/lbutils/helpers/
--rw-rw-r--   0 david     (1000) david     (1000)     1614 2023-04-12 20:42:47.000000 lbutils-mp-0.2.3/lbutils/helpers/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     3859 2023-04-12 20:42:47.000000 lbutils-mp-0.2.3/lbutils/helpers/i2c.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-15 10:21:12.860083 lbutils-mp-0.2.3/lbutils/pmods/
--rw-rw-r--   0 david     (1000) david     (1000)     1897 2023-04-12 20:46:12.000000 lbutils-mp-0.2.3/lbutils/pmods/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-15 10:21:12.860083 lbutils-mp-0.2.3/lbutils/pmods/i2c/
--rw-rw-r--   0 david     (1000) david     (1000)     1617 2023-04-14 20:27:40.000000 lbutils-mp-0.2.3/lbutils/pmods/i2c/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-15 10:21:12.860083 lbutils-mp-0.2.3/lbutils/pmods/spi/
--rw-rw-r--   0 david     (1000) david     (1000)     4133 2023-04-14 20:27:40.000000 lbutils-mp-0.2.3/lbutils/pmods/spi/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)    20877 2023-04-15 10:13:15.000000 lbutils-mp-0.2.3/lbutils/pmods/spi/oledrgb.py
--rw-rw-r--   0 david     (1000) david     (1000)     3517 2023-04-12 20:37:20.000000 lbutils-mp-0.2.3/lbutils/typing.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-15 10:21:12.860083 lbutils-mp-0.2.3/lbutils_mp.egg-info/
--rw-rw-r--   0 david     (1000) david     (1000)     6193 2023-04-15 10:21:12.000000 lbutils-mp-0.2.3/lbutils_mp.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)      796 2023-04-15 10:21:12.000000 lbutils-mp-0.2.3/lbutils_mp.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2023-04-15 10:21:12.000000 lbutils-mp-0.2.3/lbutils_mp.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1000) david     (1000)        8 2023-04-15 10:21:12.000000 lbutils-mp-0.2.3/lbutils_mp.egg-info/top_level.txt
--rw-rw-r--   0 david     (1000) david     (1000)     2136 2023-04-15 10:13:32.000000 lbutils-mp-0.2.3/pyproject.toml
--rw-rw-r--   0 david     (1000) david     (1000)       38 2023-04-15 10:21:12.860083 lbutils-mp-0.2.3/setup.cfg
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-16 19:40:19.822734 lbutils-mp-0.2.4/
+-rw-rw-r--   0 david     (1000) david     (1000)     1064 2023-03-28 09:54:55.000000 lbutils-mp-0.2.4/LICENCE
+-rw-rw-r--   0 david     (1000) david     (1000)     6193 2023-04-16 19:40:19.822734 lbutils-mp-0.2.4/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)     5583 2023-04-13 07:19:57.000000 lbutils-mp-0.2.4/README.md
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-16 19:40:19.818734 lbutils-mp-0.2.4/lbutils/
+-rw-rw-r--   0 david     (1000) david     (1000)     2911 2023-04-13 06:53:45.000000 lbutils-mp-0.2.4/lbutils/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1456 2023-04-13 06:56:17.000000 lbutils-mp-0.2.4/lbutils/abc.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-16 19:40:19.818734 lbutils-mp-0.2.4/lbutils/drivers/
+-rw-rw-r--   0 david     (1000) david     (1000)     2290 2023-04-16 19:34:09.000000 lbutils-mp-0.2.4/lbutils/drivers/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2028 2023-04-16 19:34:09.000000 lbutils-mp-0.2.4/lbutils/drivers/common.py
+-rw-rw-r--   0 david     (1000) david     (1000)     8502 2023-04-16 19:34:09.000000 lbutils-mp-0.2.4/lbutils/drivers/seven_segment.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12508 2023-04-16 19:34:09.000000 lbutils-mp-0.2.4/lbutils/drivers/seven_segment_hex.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-16 19:40:19.822734 lbutils-mp-0.2.4/lbutils/graphics/
+-rw-rw-r--   0 david     (1000) david     (1000)     6423 2023-04-16 19:34:09.000000 lbutils-mp-0.2.4/lbutils/graphics/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)    35666 2023-04-16 19:34:09.000000 lbutils-mp-0.2.4/lbutils/graphics/canvas.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11687 2023-04-16 19:34:09.000000 lbutils-mp-0.2.4/lbutils/graphics/colours.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-16 19:40:19.822734 lbutils-mp-0.2.4/lbutils/graphics/fonts/
+-rw-rw-r--   0 david     (1000) david     (1000)     2903 2023-04-12 21:25:04.000000 lbutils-mp-0.2.4/lbutils/graphics/fonts/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     8797 2023-04-12 21:21:45.000000 lbutils-mp-0.2.4/lbutils/graphics/fonts/base_font.py
+-rw-rw-r--   0 david     (1000) david     (1000)    10858 2023-04-12 17:06:52.000000 lbutils-mp-0.2.4/lbutils/graphics/fonts/font06.py
+-rw-rw-r--   0 david     (1000) david     (1000)    13731 2023-04-12 17:06:52.000000 lbutils-mp-0.2.4/lbutils/graphics/fonts/font08.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12653 2023-04-13 21:29:43.000000 lbutils-mp-0.2.4/lbutils/graphics/fonts/org_01.py
+-rw-rw-r--   0 david     (1000) david     (1000)    16691 2023-04-16 19:34:09.000000 lbutils-mp-0.2.4/lbutils/graphics/helpers.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-16 19:40:19.822734 lbutils-mp-0.2.4/lbutils/helpers/
+-rw-rw-r--   0 david     (1000) david     (1000)     1614 2023-04-12 20:42:47.000000 lbutils-mp-0.2.4/lbutils/helpers/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3859 2023-04-12 20:42:47.000000 lbutils-mp-0.2.4/lbutils/helpers/i2c.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-16 19:40:19.822734 lbutils-mp-0.2.4/lbutils/pmods/
+-rw-rw-r--   0 david     (1000) david     (1000)     1897 2023-04-12 20:46:12.000000 lbutils-mp-0.2.4/lbutils/pmods/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-16 19:40:19.822734 lbutils-mp-0.2.4/lbutils/pmods/i2c/
+-rw-rw-r--   0 david     (1000) david     (1000)     1617 2023-04-14 20:27:40.000000 lbutils-mp-0.2.4/lbutils/pmods/i2c/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-16 19:40:19.822734 lbutils-mp-0.2.4/lbutils/pmods/spi/
+-rw-rw-r--   0 david     (1000) david     (1000)     4133 2023-04-14 20:27:40.000000 lbutils-mp-0.2.4/lbutils/pmods/spi/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)    29840 2023-04-16 19:34:09.000000 lbutils-mp-0.2.4/lbutils/pmods/spi/oledrgb.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3517 2023-04-12 20:37:20.000000 lbutils-mp-0.2.4/lbutils/typing.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-16 19:40:19.822734 lbutils-mp-0.2.4/lbutils_mp.egg-info/
+-rw-rw-r--   0 david     (1000) david     (1000)     6193 2023-04-16 19:40:19.000000 lbutils-mp-0.2.4/lbutils_mp.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)      793 2023-04-16 19:40:19.000000 lbutils-mp-0.2.4/lbutils_mp.egg-info/SOURCES.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2023-04-16 19:40:19.000000 lbutils-mp-0.2.4/lbutils_mp.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        8 2023-04-16 19:40:19.000000 lbutils-mp-0.2.4/lbutils_mp.egg-info/top_level.txt
+-rw-rw-r--   0 david     (1000) david     (1000)     2148 2023-04-16 19:40:02.000000 lbutils-mp-0.2.4/pyproject.toml
+-rw-rw-r--   0 david     (1000) david     (1000)       38 2023-04-16 19:40:19.822734 lbutils-mp-0.2.4/setup.cfg
```

### Comparing `lbutils-mp-0.2.3/LICENCE` & `lbutils-mp-0.2.4/LICENCE`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.3/PKG-INFO` & `lbutils-mp-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbutils-mp
-Version: 0.2.3
+Version: 0.2.4
 Summary: Utility library for MicroPython, used at Leeds Beckett University and primarily aimed at the Pico H/W microcontrollers
 Author-email: David Love <david.love@leedsbeckett.ac.uk>
 Project-URL: Homepage, https://github.com/dlove24/lbutils
 Project-URL: Documentation, https://dlove24.github.io/lbutils/lbutils/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lbutils-mp-0.2.3/README.md` & `lbutils-mp-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.3/lbutils/__init__.py` & `lbutils-mp-0.2.4/lbutils/__init__.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.3/lbutils/abc.py` & `lbutils-mp-0.2.4/lbutils/abc.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.3/lbutils/drivers/__init__.py` & `lbutils-mp-0.2.4/lbutils/drivers/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,9 +40,11 @@
 
 This version is written for MicroPython 3.4, and has been tested on:
 
   * Raspberry Pi Pico H/W
 """
 
 ### Expose the `drivers` module interface as a full package
+from .common import PIN_ON_SENSE
+
 from .seven_segment import SegDisplay
 from .seven_segment_hex import SegHexDisplay
```

### Comparing `lbutils-mp-0.2.3/lbutils/drivers/seven_segment.py` & `lbutils-mp-0.2.4/lbutils/drivers/seven_segment.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,14 +75,16 @@
 
 # Import MicroPython libraries for GPIO access if available
 try:
     from machine import Pin
 except ImportError:
     print("Ignoring MicroPython includes")
 
+from .common import PIN_ON_SENSE
+
 ##
 ## Classes
 ##
 
 
 class SegDisplay:
     """Simple (decimal) numeric driver for a seven-segment display, requiring
@@ -152,44 +154,43 @@
             raise ValueError("The GPIO Request List is empty")
         elif len(gpio_request) != 7:
             raise ValueError("The GPIO Request List must be EXACTLY seven entries long")
         else:
             for segment in range(7):
                 self.pin_list.append(Pin(gpio_request[segment], Pin.OUT))
 
-    def display(self, character: int, inverted: bool = False) -> None:
+    def display(self, character: int, pin_on: PIN_ON_SENSE = "LOW") -> None:
         """Display the given `character` on the seven-segment display, using the
         `_char_list` as a guide for which pins to turn on or off. By default the
         `display` method will use the entries in the `_char_list` directly: if
         you need to invert the 'normal' sense, set the `inverted` parameter to
         `True`.
 
         Parameters
         ----------
 
         character: int
             The value to be displayed on the seven segment display, which must be
             between zero ('0') and nine ('9')
-        inverted: bool, optional
-            By default the `display` method assumes that pulling a GPIO pin *low*
-            will turn the relevant segment *on*; i.e. the typical behaviour for a
-            common anode display. If the attached display needs to raise a GPIO
-            pin *high* to set the segment *on* (i.e. the typical behaviour for a
-            common cathode display), call the `display` method with `inverted`
-            set to `True`.
+        pin_on: PIN_ON_SENSE, optional
+            When set to `"HIGH"` the GPIO pins need to be set 'high' ('1') for
+            the device segment to turn on (the typical behaviour for a common
+            anode display). When set to `"LOW"` the GPIO pins need to be set
+            'low' ('0') for the device segment to turn on (the typical behaviour
+            for a common cathode display.
 
         Raises
         ------
 
         IndexError
             The `character` is not in a range that can be displayed.
         """
         # For a character in the valid range...
         if 0 <= character <= 9:
-            if not inverted:
+            if pin_on == "LOW":
                 # ... if the request is to display in the non-inverted form, then
                 # select the row in `_char_list` corresponding to the character to
                 # be displayed and then set in turn each of the GPIO pins corresponding
                 # to the segment values either high or low depending on the column
                 # value in `_char_list` for that segment value
                 for pin in range(7):
                     self.pin_list[pin].value(self._char_list[character][pin])
```

### Comparing `lbutils-mp-0.2.3/lbutils/drivers/seven_segment_hex.py` & `lbutils-mp-0.2.4/lbutils/drivers/seven_segment_hex.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,14 +79,16 @@
 
 # Import the Python type libraries if available
 try:
     from typing import Union
 except ImportError:
     print("The Python type library isn't present. Ignoring.")
 
+from .common import PIN_ON_SENSE
+
 ##
 ## Constants
 ##
 
 ASCII_UPPERCASE = set("abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ")
 """Constant for the set of ASCII letters."""
 ASCII_DIGITS = set("0123456789")
@@ -177,15 +179,15 @@
             raise ValueError("The GPIO Request List is empty")
         elif len(gpio_request) != 7:
             raise ValueError("The GPIO Request List must be EXACTLY seven entries long")
         else:
             for segment in range(7):
                 self.pin_list.append(Pin(gpio_request[segment], Pin.OUT))
 
-    def display(self, character: Union[int, str], inverted: bool = False) -> None:
+    def display(self, character: Union[int, str], pin_on: PIN_ON_SENSE = "LOW") -> None:
         """Display the given `character` on the seven-segment display, using the
         `_char_list` as a guide for which pins to turn on or off. By default the
         `display` method will use the entries in the `_char_list` directly: if
         you need to invert the 'normal' sense, set the `inverted` parameter to
         `True`.
 
         Parameters
@@ -200,35 +202,34 @@
             ('F'), and will be interpreted as a single, hexadecimal digit.
 
             `str`: The value will be interpreted directly as a hexadecimal digit,
             and must be in the range `[0..F]`.
 
             If the type does not conform to the above, then a `TypeError` will be
             raised.
-        inverted: bool, optional
-            By default the `display` method assumes that pulling a GPIO pin _low_
-            will turn the relevant segment _on_; i.e. the typical behaviour for a
-            common anode display. If the attached display needs to raise a GPIO
-            pin _high_ to set the segment _on_ (i.e. the typical behaviour for a
-            common cathode display), call the `display` method with `inverted`
-            set to `True`.
+        pin_on: PIN_ON_SENSE, optional
+            When set to `"HIGH"` the GPIO pins need to be set 'high' ('1') for
+            the device segment to turn on (the typical behaviour for a common
+            anode display). When set to `"LOW"` the GPIO pins need to be set
+            'low' ('0') for the device segment to turn on (the typical behaviour
+            for a common cathode display.
 
         Raises
         ------
 
         IndexError
             The `character` is not in a range that can be displayed.
         TypeError
             The `character` is not either an `int` or a `str`
         """
         # Convert a decimal integer in the range [0..15], and then display
         if isinstance(character, int):
             # For a character in the valid range...
             if 0 <= character <= 15:
-                if not inverted:
+                if pin_on == "LOW":
                     # ... if the request is to display in the non-inverted form, then
                     # select the row in `_char_list` corresponding to the character to
                     # be displayed and then set in turn each of the GPIO pins corresponding
                     # to the segment values either high or low depending on the column
                     # value in `_char_list` for that segment value
                     for pin in range(7):
                         self.pin_list[pin].value(self._char_list[character][pin])
@@ -252,15 +253,15 @@
 
             # Check if this normalise character is a valid hexadecimal digit...
             if normalised_character in ASCII_HEX_DIGITS:
                 # ... if so, convert the hexadecimal string to an integer, so we can use
                 # this as the index for the character lookup
                 _char_list_index = int(normalised_character, 16)
 
-                if not inverted:
+                if pin_on == "LOW":
                     # If the request is to display in the non-inverted form, then
                     # select the row in `_char_list` corresponding to the `_char_list_index` to
                     # be displayed and then set in turn each of the GPIO pins corresponding
                     # to the segment values either high or low depending on the column
                     # value in `_char_list` for that segment value
                     for pin in range(7):
                         self.pin_list[pin].value(self._char_list[_char_list_index][pin])
```

### Comparing `lbutils-mp-0.2.3/lbutils/graphics/__init__.py` & `lbutils-mp-0.2.4/lbutils/graphics/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -25,45 +25,79 @@
 through a base class called [`Canvas`][lbutils.graphics.Canvas], which is
 expected to be instantiated as sub-class of one of the driver classes, e.g.
 [`lbutils.pmods.spi.OLEDrgb`][lbutils.pmods.spi.OLEDrgb]. The following
 description therefore describes the methods and attributes common to all derived
 drivers: but see the individual drivers for attributes and methods that may be
 specific to the device in question.
 
-Much of the functionality of the `Canvas` class is provided by related
-'helper' classes. Some of these helper classes such as [`Pen`]
-[lbutils.graphics.Pen] or [`Colour`][lbutils.graphics.Colour] may be useful
-more widely in graphics and drawing routines. Other helper classes such as
-the [`BaseFont`][lbutils.graphics.fonts.BaseFont] are likely to be useful
-only in the context of the `Canvas` class (and sub-classes).
+### User and Library Cursors
+
+The `Canvas` will maintain two internal drawing references
 
-As above, the main aim of the `Canvas` class (and the graphics library generally
-is to provide a basic set of capabilities which can be relied on by all users (and
-higher-level libraries). Those common facilities can be divided into the following
-categories, and are described in more detail in the following sections
+1. A [`cursor`]
+[lbutils.graphics.Canvas.cursor], representing the current
+[`x`][lbutils.graphics.Canvas.x] and [`y`][lbutils.graphics.Canvas.y]
+drawing co-ordinates. This [`cursor`]
+[lbutils.graphics.Canvas.cursor] should be assumed to be under the
+control of the _library_ (`Canvas`). For instance, many of the drawing methods,
+this internal state will be modified to point to the _next_ location which is
+commonly used in sequence. For example the [`write_text`]
+[lbutils.graphics.Canvas.write_text] updates the [`cursor`]
+[lbutils.graphics.Canvas.cursor] to point to position at the end of the text
+string. Or the [`draw_line`] [lbutils.graphics.Canvas.draw_line] method will
+change the [`cursor`] [lbutils.graphics.Canvas.cursor] to the end of the
+line just drawn. This behaviour makes it easier to sequence multiple drawing
+methods: especially in the common case where a single origin is used to draw
+multiple lines or other primitives in succession to create more complex shapes.
+2. An [`origin`]
+[lbutils.graphics.Canvas.origin], representing a reference point for
+a sequence of drawing commands or drawing primitives. This [`origin`]
+[lbutils.graphics.Canvas.origin] is assumed to be under the control of
+the _user_, and will usually _not_ be modified by the internal drawing commands.
+Instead an application can set the [`origin`]
+[lbutils.graphics.Canvas.origin], then use the drawing primitives with the
+addition of `from_origin` in the method name. Any internal change of state in
+the [`cursor`]
+[lbutils.graphics.Canvas.cursor] will not be reflected in a subsequent change
+to the origin.
+
+### Library Organisation and Helper Classes
+
+The main aim of the `Canvas` class (and the graphics library generally is to
+provide a basic set of capabilities which can be relied on by all users (and
+higher-level libraries). Those common facilities can be divided into the
+following categories, and are described in more detail in the following sections
 
 * **[Colour Support and Representation][lbutils.graphics.colours]**. Classes
 such as `Colour` which holds the internal colour representations used by the
 graphics library. Also provides methods to convert between common colour formats
 and representations, such as RGB565 and RGB588.
-* **[Common Drawing Primitives][lbutils.graphics.canvas]**. The drawing primitives
-provided by the `Canvas` class of the library, such as circles, rectangles and
-lines. These primitives are guaranteed to be available in all graphics drivers:
-but depending on the driver may or may not be accelerated,
+* **[Common Drawing Primitives][lbutils.graphics.Canvas]**. The drawing
+primitives provided by the `Canvas` class of the library, such as circles,
+rectangles and lines. These primitives are guaranteed to be available in all
+graphics drivers: but depending on the driver may or may not be accelerated.
 * **[Fonts and Font Handling][lbutils.graphics.fonts]**. Describes the internal
 font representation used in this library, and the details of the fonts available
 for use.
 * **[Helper Classes][lbutils.graphics.helpers]**. Provides utility classes and
 functions which ease the abstraction of the main graphics Canvas library, e.g.
 [`Pixel`][lbutils.graphics.Pixel]. These are provided outside the main `Canvas`
 class as being the most suitable classes for re-use in other drawing and graphics
 routines.
 
 ## Implementation
 
+Much of the functionality of the [`Canvas`]
+[lbutils.graphics.Canvas] class is provided by related
+'helper' classes. Some of these helper classes such as [`Pen`]
+[lbutils.graphics.Pen] or [`Colour`][lbutils.graphics.Colour] may be useful
+more widely in graphics and drawing routines. Other helper classes such as
+the [`BaseFont`][lbutils.graphics.fonts.BaseFont] are likely to be useful
+only in the context of the `Canvas` class (and sub-classes).
+
 The only methods _required_ to be implemented in sub-classes of [`Canvas`]
 [lbutils.graphics.Canvas] are [`read_pixel`][lbutils.graphics.Canvas.read_pixel]
 and [`write_pixel`][lbutils.graphics.Canvas.write_pixel]. All the drawing
 primitives, including font support, can be implemented by `Canvas` using only
 those two methods. However, in most cases the drawing speed is unacceptably slow,
 and so in _most_ cases sub-classes will also choose to override methods such as
 [`draw_line`][lbutils.graphics.Canvas.draw_line] where such facilities are
@@ -75,10 +109,10 @@
 
 *   Raspberry Pi Pico W (MicroPython 3.4)
 """
 
 ### Expose the `graphics` module interface as a full package
 __all__ = ["colours", "canvas", "helpers"]
 
-from .colours import Colour
-from .canvas import Canvas, FrameBufferCanvas
+from .colours import DEVICE_BIT_ORDER, Colour
+from .canvas import RECTANGLE_STYLE, Canvas, FrameBufferCanvas
 from .helpers import Pen, Pixel, BoundPixel
```

### Comparing `lbutils-mp-0.2.3/lbutils/graphics/colours.py` & `lbutils-mp-0.2.4/lbutils/graphics/colours.py`

 * *Files 9% similar despite different names*

```diff
@@ -70,14 +70,23 @@
 ## Tested Implementations
 
 *   Raspberry Pi Pico W (MicroPython 3.4)
 *   CPython (3.10)
 """
 
 ###
+### Enumerations. MicroPython doesn't have actual an actual `enum` (yet), so
+### these serve as common cases where a selection of values need to be defined
+###
+
+DEVICE_BIT_ORDER = {"ARM", "INTEL"}
+"""Set the bit order to be used (mostly in graphics code) for low-level
+manipulation of bits send to, and received from, devices."""
+
+###
 ### Classes
 ###
 
 
 class Colour:
     """A (packed) representation of a colour value, as `r` (red), `g` (green)
     and `b` (blue) components. The principle purpose of this class is to both
@@ -96,18 +105,18 @@
     as_565: int, read-only
         Provides the colour value in the RGB565 format, using a single
         byte in the the standard platform representation.
     as_888: int, read-only
         Provides the colour value in the RGB888 format, using a
         double word for the colour value in the standard platform
         representation.
-    isARM: bool, read-write
-        Flag indicating if the colour value should use the ARM byte
-        packing order in colour conversions. Defaults to `True` as
-        set by the default constructor.
+    bit_order: DEVICE_BIT_ORDER, read-write
+        Argument indicating if the underlying bit order used for
+        the bit packing order in colour conversions. Defaults to
+        `ARM` as set by the default constructor.
 
     Implementation
     --------------
 
     Where possible attribute values are cached, and so the first
     call of the attribute will be slightly slower than subsequent calls.
 
@@ -118,15 +127,17 @@
         constructor the behaviour of the class is undefined.
     """
 
     ##
     ## Constructors
     ##
 
-    def __init__(self, r: int, g: int, b: int, isARM: bool = True) -> None:
+    def __init__(
+        self, r: int, g: int, b: int, bit_order: DEVICE_BIT_ORDER = "ARM"
+    ) -> None:
         """Creates a representation of a colour value, from the three integers
         `r` (red), `g` (green) and `b` (blue). The class will accept anything
         which can be coerced to an integer as arguments: the access through the
         attributes will determine the representation used when displaying the
         colour.
 
         Parameters
@@ -134,25 +145,24 @@
 
         r: int
             The integer representing the red component of the colour.
         g: int
             The integer representing the green component of the colour.
         b: int
             The integer representing the blue component of the colour.
-        isARM: bool, optional
-            Determines if the current platform is an ARM processor or not. This
-            value is used to determine which order for the `word` representation
-            of the colour returned to the caller. Defaults to `True` as required
-            by the Pico H/W platform of the micro-controller development board.
+        bit_order: DEVICE_BIT_ORDER, read-write
+            Argument indicating if the underlying bit order used for
+            the bit packing order in colour conversions. Defaults to
+            `ARM` as set by the default constructor.
         """
         self._r = int(r)
         self._g = int(g)
         self._b = int(b)
 
-        self.isARM = isARM
+        self.bit_order = "ARM"
 
         # Cached values
         self._565 = None
         self._888 = None
 
         self._bR = None
         self._bG = None
@@ -214,15 +224,15 @@
             A packed byte value of the colour representation.
 
         """
         # Check for a cached value ...
         if self._565 is None:
             # ... if there isn't one, calculate what the byte representation
             #     should look like
-            if self.isARM:
+            if self.bit_order == "ARM":
                 self._565 = (
                     (self._g & 0x1C) << 1
                     | (self._b >> 3)
                     | (self._r & 0xF8)
                     | self._g >> 5
                 )
             else:
@@ -259,15 +269,15 @@
             A packed double word value of the colour representation.
 
         """
         # Check for a cached value ...
         if self._888 is None:
             # ... if there isn't one, calculate what the byte representation
             #     should look like
-            if self.isARM:
+            if self.bit_order == "ARM":
                 self._888 = (
                     (self._g & 0x1C) << 1
                     | (self._b >> 3)
                     | (self._r & 0xF8)
                     | self._g >> 5
                 )
             else:
```

### Comparing `lbutils-mp-0.2.3/lbutils/graphics/fonts/__init__.py` & `lbutils-mp-0.2.4/lbutils/graphics/fonts/__init__.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.3/lbutils/graphics/fonts/base_font.py` & `lbutils-mp-0.2.4/lbutils/graphics/fonts/base_font.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.3/lbutils/graphics/fonts/font06.py` & `lbutils-mp-0.2.4/lbutils/graphics/fonts/font06.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.3/lbutils/graphics/fonts/font08.py` & `lbutils-mp-0.2.4/lbutils/graphics/fonts/font08.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.3/lbutils/graphics/fonts/org_01.py` & `lbutils-mp-0.2.4/lbutils/graphics/fonts/org_01.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.3/lbutils/graphics/helpers.py` & `lbutils-mp-0.2.4/lbutils/graphics/helpers.py`

 * *Files 22% similar despite different names*

```diff
@@ -34,29 +34,32 @@
 # Import the typing hints if available. Use our backup version
 # if the offical library is missing
 try:
     from typing import Type
 except ImportError:
     from lbutils.typing import Type
 
-from .colours import Colour, COLOUR_WHITE, COLOUR_BLACK
+# Import the math library (needed for polar co-ordinates)
+from math import cos, sin
+
+from .colours import COLOUR_WHITE, COLOUR_BLACK, Colour
 
 ###
 ### Classes
 ###
 
 
 class Pen:
     """Implements a convenience class for the graphics library, which represents
     a 'pen' with a specified foreground and background colour, and thickness.
     The primary purpose of this class is to make it easy to swap between common
     colour and line values; for instance using two pens to allow a swap between
     'highlight' and 'normal' text colours. This can be accomplished by defining
     the foreground and background colour of the
-    [`Canvas`][lbutils.graphics.canvas] as needed: this class simply makes that
+    [`Canvas`][lbutils.graphics.Canvas] as needed: this class simply makes that
     switch easier.
 
     Example
     -------
 
     Two new pens can be defined for 'normal' and 'alert' text as
 
@@ -110,15 +113,15 @@
     instances such as cursors where a relationship between a X and a Y co-
     ordinate must be maintained. This is also useful when two or more co-
     ordinates need to be tracked, or to be switched between. For instance an
     'origin' co-ordinate for a drawing, and a 'current' co-ordinate around the
     origin where lines are being drawn to and from.
 
     !!! note "Implementation Defined Origin"
-            As for the [`Canvas`][lbutils.graphics.canvas] class, the
+            As for the [`Canvas`][lbutils.graphics.Canvas] class, the
             interpretation of the point '(0, 0)' is defined by the underlying
             graphics implementation. For instance the '(0, 0)' point may
             represent the top-left corner or the canvas, or the bottom- left hand
             corner. For details of how this point will be chosen (or changed),
             see the implementation of the specified sub-class of `Canvas` that is
             implemented by the chosen display driver.
 
@@ -131,15 +134,20 @@
             The Y co-ordinate value.
     x_y: int
             A tuple representing the co-ordinate (x ,y).
 
     Methods
     ----------
 
-    * `move_to()`. Move the internal co-ordinate to the value (x, y).
+    * `move_to()`. Move the internal co-ordinate to the value (x, y). An alias
+    for the [`x_y`][lbutils.graphics.Pixel.x_y] property.
+    * `offset()`. Returns a `tuple` representing the (x, y) co-ordinate of the
+    current `Pixel` with the specified Cartesian off-set applied.
+    * `offset_polar()`. Returns a `tuple` representing the (x, y) co-ordinate of
+    the current `Pixel` with the specified Polar off-set applied.
     """
 
     ##
     ## Constructors
     ##
 
     def __init__(self, x: int, y: int) -> None:
@@ -148,15 +156,15 @@
 
         Parameters
         ----------
 
         x: int
                 The initial X co-ordinate value.
         y: int
-                The initial Y co-ordinate value
+                The initial Y co-ordinate value.
         """
         self.x = int(x)
         self.y = int(y)
 
     ##
     ## Properties
     ##
@@ -208,32 +216,133 @@
 
         ValueError:
             If the `x` or `y` co-ordinate in the `xy` tuple cannot be converted
             to an integer.
         """
         self.x_y = xy
 
+    def offset(self, x: int = 0, y: int = 0) -> tuple:
+        """Returns a `tuple` representing the (x, y) co-ordinate of the current
+        `Pixel` with the specified Cartesian off-set applied.
+
+        Example
+        -------
+
+        Given a `Pixel` object called `origin` with representing the co-ordinates
+        '(0, 10)'
+
+        ````python
+        origin = Pixel(0, 10)
+        ````
+
+        then calling
+
+        ````python
+        new_origin = origin.offset(10, 10)
+        ````
+
+        or better
+
+        ````python
+        new_origin = origin.offset(x = 10, y = 10)
+        ````
+
+        will return the tuple `[10, 20]` as `new_origin`.
+
+        Parameters
+        ----------
+
+        x: int, optional
+            The offset to apply to the x co-ordinate value of the `Pixel`.
+        y: int, optional
+            The offset to apply to the x co-ordinate value of the `Pixel`.
+
+        Returns
+        -------
+
+        tuple:
+            The (x, y) co-ordinate as a two value `tuple`  with the
+            first value of the `tuple` representing the `x` co-ordinate and the
+            second value of the `tuple` representing the `y` co-ordinate.
+        """
+        return [self.x + x, self.y + y]
+
+    def offset_polar(self, r: int = 0, theta: int = 0) -> tuple:
+        """Returns a `tuple` representing the (x, y) co-ordinate of the current
+        `Pixel` with the specified Polar off-set applied as the radius `r` and
+        angle `theta`.
+
+        !!! Note "Floating Point Calculations"
+            Although the _return_ values of the `offset_polar` function will be
+            integers, floating point routines are used internally to calculate
+            the sine and cosine of the angle `theta`. This may result in this
+            routine being slower than expected on some platforms.
+
+        Example
+        -------
+
+        Given a `Pixel` object called `origin` with representing the co-ordinates
+        '(0, 10)'
+
+        ````python
+        origin = Pixel(0, 10)
+        ````
+
+        then calling
+
+        ````python
+        new_origin = origin.offset_polar(13, 22)
+        ````
+
+        or better
+
+        ````python
+        new_origin = origin.offset(r = 13, theta = 22)
+        ````
+
+        will return the tuple `[12, 5]` as `new_origin`.
+
+        Parameters
+        ----------
+
+        r: int, optional
+            The offset to apply to the x co-ordinate value of the `Pixel`,
+            specified as the _radius_ of the Polar co-ordinate.
+        theta: int, optional
+            The offset to apply to the x co-ordinate value of the `Pixel`,
+            specified as the _angle_ of the Polar co-ordinate.
+
+        Returns
+        -------
+
+        tuple:
+            The (x, y) co-ordinate as a two value `tuple`  with the
+            first value of the `tuple` representing the `x` co-ordinate and the
+            second value of the `tuple` representing the `y` co-ordinate.
+        """
+        return [int(self.x + (r * cos(theta))), int(self.y + (r * sin(theta)))]
+
 
 class BoundPixel(Pixel):
     """Represents a Cartesian co-ordinate between limits. Used as a convenience
     class for instances such as cursors where a relationship between a X and a Y
     co-ordinate must be maintained. This is also useful when two or more co-
     ordinates need to be tracked, or to be switched between. For instance an
     'origin' co-ordinate for a drawing, and a 'current' co-ordinate around the
     origin where lines are being drawn to and from.
 
     Unlike the [`Pixel`][lbutils.graphics.Pixel] class, the `BoundPxiel` will
     also ensure that the X and Y co-ordinates are maintained between minimum and
-    maximum value for the `width` or `height`. This is useful for instances where a
-    cursor, for instance, must only take values within the limits of a display. It
-    can also be used where a clipping region is being defined to ensure that values
-    cannot lie outside the clipped region.
+    maximum value for the `width` or `height`. This is useful for instances where
+    a cursor, for instance, must only take values within the limits of a display.
+    It can also be used where a clipping region is being defined to ensure that
+    values cannot lie outside the clipped region.
 
     !!! note "Implementation Defined Origin"
-            As for the [`Canvas`][lbutils.graphics.canvas] class, the
+            As for the [`Canvas`][lbutils.graphics.Canvas] class, the
             interpretation of the point '(0, 0)' is defined by the underlying
             graphics implementation. For instance the '(0, 0)' point may
             represent the top-left corner or the canvas, or the bottom- left hand
             corner. For details of how this point will be chosen (or changed),
             see the implementation of the specified sub-class of `Canvas` that is
             implemented by the chosen display driver.
 
@@ -264,15 +373,14 @@
         self,
         x: int,
         y: int,
         max_x: int,
         max_y: int,
         min_x: int = 0,
         min_y: int = 0,
-        clip: bool = True,
     ) -> None:
         """Creates a `Pixel` instance holding the specified `x` and `y` co-
         ordinates, together representing the Cartesian point '(`x`, `y`)'. This
         `x` and `y` value is guaranteed to be maintained between `min_x` and
         `max_x` for the `x` co- ordinate, and `min_y` and `max_y` for the `y`
         co-ordinate.
 
@@ -289,27 +397,22 @@
                 The maximum value allowed for the `y` co-ordinate.
         min_x: int, optional
                 The minimum value allowed for the `x` co-ordinate. Defaults to
                 `0`.
         min_y: int, optional
                 The minimum value allowed for the `y` co-ordinate. Defaults to
                 `0`.`
-        clip: bool, optional
-                If set to `True`, the default, silently clip the `x` and `y` co-
-                ordinates to the specified limits. If set to `False`, instead
-                raise a `ValueError` if the `x` or `y` co-ordinates do not fall
-                into the allowed limits.
 
         Implementation
         --------------
 
         As the `x` and `y` attributes of this class are compared on each write,
-        this class is by definition slower and potentially more resource intensive that
-        the underlying `Pixel` class. If the costs of the bounds-check are not required,
-        using the 'raw' `Pixel` class may be preferable.
+        this class is by definition slower and potentially more resource
+        intensive that the underlying `Pixel` class. If the costs of the bounds-
+        check are not required, using the 'raw' `Pixel` class may be preferable.
 
         !!! note
                 The parameter order is specified to allow easier definition
                 in the common case where the lower limits for `x` and `y` are
                 `0`, and the positional parameter order is being used. If all
                 four limits are being used, consider the use of named
                 parameters to avoid ambiguity.
@@ -323,91 +426,66 @@
         self.max_y = int(max_y)
 
         # Now attempt to set the actual `x` and `y` inside those
         # parameters
         self.x = int(x)
         self.y = int(y)
 
-        # Set the clipping switch
-        self.clip = clip
-
     ##
     ## Properties
     ##
 
     @property
     def x(self) -> int:
         """The `x` co-ordinate of the `BoundPxiel`, checking that it lies within
         the specified `min_x` and `max_x` limits.
 
-        Raises
-        ------
-
-        `ValueError`:
-                If `clip` is set to `False`
+        If the `x` co-ordinate does lie outside the specified region, set it to
+        the `min_x` or `max_x` limit as appropriate.
         """
         if self.min_x <= self._x <= self.max_x:
             return self._x
         else:
-            if self.clip:
-                if self._x > self.max_x:
-                    self._x = self.max_x
-                if self._x < self.min_x:
-                    self._x = self.min_x
-
-                return self._x
+            if self._x > self.max_x:
+                self._x = self.max_x
+            if self._x < self.min_x:
+                self._x = self.min_x
 
-            else:
-                raise (ValueError("Pixel limits exceeded"))
+            return self._x
 
     @x.setter
     def x(self, value: int) -> None:
         if self.min_x <= value <= self.max_x:
             self._x = value
         else:
-            if self.clip:
-                if value > self.max_x:
-                    self._x = self.max_x
-                if value < self.min_x:
-                    self._x = self.min_x
-
-            else:
-                raise (ValueError("Pixel limits exceeded"))
+            if value > self.max_x:
+                self._x = self.max_x
+            if value < self.min_x:
+                self._x = self.min_x
 
     @property
     def y(self) -> int:
         """The `y` co-ordinate of the `BoundPxiel`, checking that it lies within
         the specified `min_x` and `max_y` limits.
 
-        Raises
-        ------
-
-        `ValueError`:
-                If `clip` is set to `False`
+        If the `y` co-ordinate does lie outside the specified region, set it to
+        the `min_y` or `may_y` limit as appropriate.
         """
         if self.min_y <= self._y <= self.max_y:
             return self._y
         else:
-            if self.clip:
-                if self._y > self.max_y:
-                    self._y = self.max_y
-                if self._y < self.min_y:
-                    self._y = self.min_y
-
-                return self._y
+            if self._y > self.max_y:
+                self._y = self.max_y
+            if self._y < self.min_y:
+                self._y = self.min_y
 
-            else:
-                raise (ValueError("Pixel limits exceeded"))
+            return self._y
 
     @y.setter
     def y(self, value: int) -> None:
         if self.min_y <= value <= self.max_y:
             self._y = value
         else:
-            if self.clip:
-                if value > self.max_y:
-                    self._y = self.max_y
-                if value < self.min_y:
-                    self._y = self.min_y
-
-            else:
-                raise (ValueError("Pixel limits exceeded"))
+            if value > self.max_y:
+                self._y = self.max_y
+            if value < self.min_y:
+                self._y = self.min_y
```

### Comparing `lbutils-mp-0.2.3/lbutils/helpers/__init__.py` & `lbutils-mp-0.2.4/lbutils/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.3/lbutils/helpers/i2c.py` & `lbutils-mp-0.2.4/lbutils/helpers/i2c.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.3/lbutils/pmods/__init__.py` & `lbutils-mp-0.2.4/lbutils/pmods/__init__.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.3/lbutils/pmods/i2c/__init__.py` & `lbutils-mp-0.2.4/lbutils/pmods/i2c/__init__.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.3/lbutils/pmods/spi/__init__.py` & `lbutils-mp-0.2.4/lbutils/pmods/spi/__init__.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.3/lbutils/typing.py` & `lbutils-mp-0.2.4/lbutils/typing.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.3/lbutils_mp.egg-info/PKG-INFO` & `lbutils-mp-0.2.4/lbutils_mp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbutils-mp
-Version: 0.2.3
+Version: 0.2.4
 Summary: Utility library for MicroPython, used at Leeds Beckett University and primarily aimed at the Pico H/W microcontrollers
 Author-email: David Love <david.love@leedsbeckett.ac.uk>
 Project-URL: Homepage, https://github.com/dlove24/lbutils
 Project-URL: Documentation, https://dlove24.github.io/lbutils/lbutils/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lbutils-mp-0.2.3/lbutils_mp.egg-info/SOURCES.txt` & `lbutils-mp-0.2.4/lbutils_mp.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 LICENCE
 README.md
 pyproject.toml
 lbutils/__init__.py
 lbutils/abc.py
 lbutils/typing.py
 lbutils/drivers/__init__.py
+lbutils/drivers/common.py
 lbutils/drivers/seven_segment.py
 lbutils/drivers/seven_segment_hex.py
-lbutils/examples/__init__.py
 lbutils/graphics/__init__.py
 lbutils/graphics/canvas.py
 lbutils/graphics/colours.py
 lbutils/graphics/helpers.py
 lbutils/graphics/fonts/__init__.py
 lbutils/graphics/fonts/base_font.py
 lbutils/graphics/fonts/font06.py
```

### Comparing `lbutils-mp-0.2.3/pyproject.toml` & `lbutils-mp-0.2.4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lbutils-mp"
-version = "0.2.3"
+version = "0.2.4"
 authors = [
   { name="David Love", email="david.love@leedsbeckett.ac.uk" },
 ]
 description = "Utility library for MicroPython, used at Leeds Beckett University and primarily aimed at the Pico H/W microcontrollers"
 readme = "README.md"
 requires-python = ">=3.4"
 classifiers = [
@@ -29,15 +29,15 @@
 black = true
 
 [tool.setuptools]
 packages = ["lbutils", "lbutils.drivers", "lbutils.graphics", "lbutils.graphics.fonts", "lbutils.helpers", "lbutils.pmods", "lbutils.pmods.spi", "lbutils.pmods.i2c"]
 
 [tool.ruff]
 # Enable pycodestyle (`E`) and Pyflakes (`F`) codes by default.
-select = ["E", "F"]
+select = ["E", "F", "Q", "FBT"]
 
 # Allow autofix for all enabled rules (when `--fix`) is provided.
 fixable = ["A", "B", "C", "D", "E", "F", "G", "I", "N", "Q", "S", "T", "W", "ANN", "ARG", "BLE", "COM", "DJ", "DTZ", "EM", "ERA", "EXE", "FBT", "ICN", "INP", "ISC", "NPY", "PD", "PGH", "PIE", "PL", "PT", "PTH", "PYI", "RET", "RSE", "RUF", "SIM", "SLF", "TCH", "TID", "TRY", "UP", "YTT"]
 unfixable = []
 
 # Exclude a variety of commonly ignored directories.
 exclude = [
```

