# Comparing `tmp/e-qsl-0.1.7.tar.gz` & `tmp/e-qsl-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e-qsl-0.1.7.tar", last modified: Thu Mar 30 17:26:48 2023, max compression
+gzip compressed data, was "e-qsl-0.1.8.tar", last modified: Sun Apr 16 14:08:35 2023, max compression
```

## Comparing `e-qsl-0.1.7.tar` & `e-qsl-0.1.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 fred       (501) staff       (20)        0 2023-03-30 17:26:48.007295 e-qsl-0.1.7/
--rw-r--r--   0 fred       (501) staff       (20)     1879 2023-03-29 02:24:01.000000 e-qsl-0.1.7/.gitignore
--rw-r--r--   0 fred       (501) staff       (20)      890 2023-03-30 17:26:48.005225 e-qsl-0.1.7/PKG-INFO
--rw-r--r--   0 fred       (501) staff       (20)      239 2023-03-29 15:20:51.000000 e-qsl-0.1.7/README.md
-drwxr-xr-x   0 fred       (501) staff       (20)        0 2023-03-30 17:26:47.980366 e-qsl-0.1.7/card/
--rw-r--r--   0 fred       (501) staff       (20)   281258 2023-03-08 22:15:25.000000 e-qsl-0.1.7/card/default.jpg
-drwxr-xr-x   0 fred       (501) staff       (20)        0 2023-03-30 17:26:47.989429 e-qsl-0.1.7/e_qsl.egg-info/
--rw-r--r--   0 fred       (501) staff       (20)      890 2023-03-30 17:26:47.000000 e-qsl-0.1.7/e_qsl.egg-info/PKG-INFO
--rw-r--r--   0 fred       (501) staff       (20)      366 2023-03-30 17:26:47.000000 e-qsl-0.1.7/e_qsl.egg-info/SOURCES.txt
--rw-r--r--   0 fred       (501) staff       (20)        1 2023-03-30 17:26:47.000000 e-qsl-0.1.7/e_qsl.egg-info/dependency_links.txt
--rw-r--r--   0 fred       (501) staff       (20)       35 2023-03-30 17:26:47.000000 e-qsl-0.1.7/e_qsl.egg-info/entry_points.txt
--rw-r--r--   0 fred       (501) staff       (20)       29 2023-03-30 17:26:47.000000 e-qsl-0.1.7/e_qsl.egg-info/requires.txt
--rw-r--r--   0 fred       (501) staff       (20)        5 2023-03-30 17:26:47.000000 e-qsl-0.1.7/e_qsl.egg-info/top_level.txt
--rwxr-xr-x   0 fred       (501) staff       (20)     8852 2023-03-30 17:25:10.000000 e-qsl-0.1.7/eqsl.py
--rw-r--r--   0 fred       (501) staff       (20)     1029 2023-03-26 16:32:15.000000 e-qsl-0.1.7/eqsl.yaml.sample
-drwxr-xr-x   0 fred       (501) staff       (20)        0 2023-03-30 17:26:47.994085 e-qsl-0.1.7/fonts/
--rw-r--r--   0 fred       (501) staff       (20)    78296 2023-03-08 21:55:36.000000 e-qsl-0.1.7/fonts/DroidSansMono.ttf
--rw-r--r--   0 fred       (501) staff       (20)   183188 2023-03-10 00:22:58.000000 e-qsl-0.1.7/fonts/Ubuntu Mono derivative Powerline Bold.ttf
--rwxr-xr-x   0 fred       (501) staff       (20)    54508 2023-03-08 21:55:47.000000 e-qsl-0.1.7/fonts/VeraMono-Italic.ttf
-drwxr-xr-x   0 fred       (501) staff       (20)        0 2023-03-30 17:26:47.997571 e-qsl-0.1.7/misc/
--rw-r--r--   0 fred       (501) staff       (20)   191436 2023-03-10 15:39:28.000000 e-qsl-0.1.7/misc/qsl-example.jpg
--rw-r--r--   0 fred       (501) staff       (20)       38 2023-03-30 17:26:48.007822 e-qsl-0.1.7/setup.cfg
--rwxr-xr-x   0 fred       (501) staff       (20)     1336 2023-03-30 17:26:11.000000 e-qsl-0.1.7/setup.py
+drwxr-xr-x   0 fred       (501) staff       (20)        0 2023-04-16 14:08:35.483422 e-qsl-0.1.8/
+-rw-r--r--   0 fred       (501) staff       (20)     1879 2023-03-29 02:24:01.000000 e-qsl-0.1.8/.gitignore
+-rw-r--r--   0 fred       (501) staff       (20)      890 2023-04-16 14:08:35.482705 e-qsl-0.1.8/PKG-INFO
+-rw-r--r--   0 fred       (501) staff       (20)      239 2023-03-29 15:20:51.000000 e-qsl-0.1.8/README.md
+drwxr-xr-x   0 fred       (501) staff       (20)        0 2023-04-16 14:08:35.468450 e-qsl-0.1.8/card/
+-rw-r--r--   0 fred       (501) staff       (20)   281258 2023-03-08 22:15:25.000000 e-qsl-0.1.8/card/default.jpg
+drwxr-xr-x   0 fred       (501) staff       (20)        0 2023-04-16 14:08:35.473305 e-qsl-0.1.8/e_qsl.egg-info/
+-rw-r--r--   0 fred       (501) staff       (20)      890 2023-04-16 14:08:34.000000 e-qsl-0.1.8/e_qsl.egg-info/PKG-INFO
+-rw-r--r--   0 fred       (501) staff       (20)      366 2023-04-16 14:08:35.000000 e-qsl-0.1.8/e_qsl.egg-info/SOURCES.txt
+-rw-r--r--   0 fred       (501) staff       (20)        1 2023-04-16 14:08:34.000000 e-qsl-0.1.8/e_qsl.egg-info/dependency_links.txt
+-rw-r--r--   0 fred       (501) staff       (20)       35 2023-04-16 14:08:34.000000 e-qsl-0.1.8/e_qsl.egg-info/entry_points.txt
+-rw-r--r--   0 fred       (501) staff       (20)       29 2023-04-16 14:08:34.000000 e-qsl-0.1.8/e_qsl.egg-info/requires.txt
+-rw-r--r--   0 fred       (501) staff       (20)        5 2023-04-16 14:08:34.000000 e-qsl-0.1.8/e_qsl.egg-info/top_level.txt
+-rwxr-xr-x   0 fred       (501) staff       (20)     8965 2023-04-16 14:06:57.000000 e-qsl-0.1.8/eqsl.py
+-rw-r--r--   0 fred       (501) staff       (20)     1075 2023-04-16 14:00:01.000000 e-qsl-0.1.8/eqsl.yaml.sample
+drwxr-xr-x   0 fred       (501) staff       (20)        0 2023-04-16 14:08:35.478460 e-qsl-0.1.8/fonts/
+-rw-r--r--   0 fred       (501) staff       (20)    78296 2023-03-08 21:55:36.000000 e-qsl-0.1.8/fonts/DroidSansMono.ttf
+-rw-r--r--   0 fred       (501) staff       (20)   183188 2023-03-10 00:22:58.000000 e-qsl-0.1.8/fonts/Ubuntu Mono derivative Powerline Bold.ttf
+-rwxr-xr-x   0 fred       (501) staff       (20)    54508 2023-03-08 21:55:47.000000 e-qsl-0.1.8/fonts/VeraMono-Italic.ttf
+drwxr-xr-x   0 fred       (501) staff       (20)        0 2023-04-16 14:08:35.480113 e-qsl-0.1.8/misc/
+-rw-r--r--   0 fred       (501) staff       (20)   191436 2023-03-10 15:39:28.000000 e-qsl-0.1.8/misc/qsl-example.jpg
+-rw-r--r--   0 fred       (501) staff       (20)       38 2023-04-16 14:08:35.483581 e-qsl-0.1.8/setup.cfg
+-rwxr-xr-x   0 fred       (501) staff       (20)     1336 2023-04-16 14:07:50.000000 e-qsl-0.1.8/setup.py
```

### Comparing `e-qsl-0.1.7/.gitignore` & `e-qsl-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `e-qsl-0.1.7/PKG-INFO` & `e-qsl-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e-qsl
-Version: 0.1.7
+Version: 0.1.8
 Summary: Send contacts confirmation cards (QSL Cards)
 Home-page: https://github.com/0x9900/QSL/
 Author: Fred C. (W6BSD)
 Author-email: w6bsd@bsdworld.org
 License: BSD-3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Telecommunications Industry
```

### Comparing `e-qsl-0.1.7/card/default.jpg` & `e-qsl-0.1.8/card/default.jpg`

 * *Files identical despite different names*

### Comparing `e-qsl-0.1.7/e_qsl.egg-info/PKG-INFO` & `e-qsl-0.1.8/e_qsl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e-qsl
-Version: 0.1.7
+Version: 0.1.8
 Summary: Send contacts confirmation cards (QSL Cards)
 Home-page: https://github.com/0x9900/QSL/
 Author: Fred C. (W6BSD)
 Author-email: w6bsd@bsdworld.org
 License: BSD-3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Telecommunications Industry
```

### Comparing `e-qsl-0.1.7/eqsl.py` & `e-qsl-0.1.8/eqsl.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,25 +119,27 @@
   img = img.resize((width, vsize), Image.Resampling.LANCZOS)
 
   overlay = Image.new('RGBA', img.size)
   draw = ImageDraw.Draw(overlay)
   draw_rectangle(draw, ((112, vsize-220), (912, vsize-20)), width=3)
 
   textbox = ImageDraw.Draw(overlay)
+  date = datetime.fromtimestamp(qso.timestamp).strftime("%A %B %d, %Y at %X UTC")
   y_pos = vsize - 215
   x_pos = 132
-  textbox.text((x_pos, y_pos), f"From: {qso.OPERATOR}", font=font_call, fill=TEXT_COLOR)
-  textbox.text((x_pos, y_pos+32), f"  To: {qso.CALL}", font=font_call, fill=TEXT_COLOR)
-  textbox.text((x_pos, y_pos+80), (f'Mode: {qso.MODE} • Band: {qso.BAND} • '
-                                  f'RST Send: {qso.RST_SENT} • RST Recieved: {qso.RST_RCVD}'
+  textbox.text((x_pos, y_pos), f"From: {qso.OPERATOR}  To: {qso.CALL}",
+               font=font_call, fill=TEXT_COLOR)
+  textbox.text((x_pos, y_pos+55), (f'Mode: {qso.MODE} • Band: {qso.BAND} • '
+                                   f'RST Send: {qso.RST_SENT} • RST Recieved: {qso.RST_RCVD}'
                                   ), font=font_text, fill=TEXT_COLOR)
-  date = datetime.fromtimestamp(qso.timestamp).strftime("%A %B %d, %Y at %X UTC")
-  textbox.text((x_pos, y_pos+105), f'Date: {date}', font=font_text, fill=TEXT_COLOR)
-  textbox.text((x_pos, y_pos+130),
-               f' Rig: {qso.MY_RIG} • Grid: {qso.MY_GRIDSQUARE} • Power: {int(qso.TX_PWR)} Watt',
+  textbox.text((x_pos, y_pos+80), f'Date: {date}', font=font_text, fill=TEXT_COLOR)
+  textbox.text((x_pos, y_pos+105), f' Rig: {qso.MY_RIG} • Power: {int(qso.TX_PWR)} Watt',
+               font=font_text, fill=TEXT_COLOR)
+  textbox.text((x_pos, y_pos+130), (f'Grid: {qso.MY_GRIDSQUARE} • CQ Zone: {config.ituzone} • '
+                                    f'ITU Zone: {config.cqzone}'),
                font=font_text, fill=TEXT_COLOR)
 
   textbox.text((x_pos, y_pos+165), signature, font=font_foot, fill=TEXT_COLOR)
 
   textbox.text((NEW_WIDTH-90, vsize-30), '@0x9900', font=font_foot, fill=(0xff, 0xff, 0xff))
 
   img = Image.alpha_composite(img, overlay)
```

### Comparing `e-qsl-0.1.7/eqsl.yaml.sample` & `e-qsl-0.1.8/eqsl.yaml.sample`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 
 call: <your call>
+ituzone: <your ituzone>
+cqzone: <your cqzone>
 adif_file: </path/to/your/logfile.adif>
 
 smtp_server: <yours goes here>
 smtp_login: <yours goes here>
 smtp_password: <yours goes here>
 smtp_port: 25
 smtp_from: <yours goes here>
```

### Comparing `e-qsl-0.1.7/fonts/DroidSansMono.ttf` & `e-qsl-0.1.8/fonts/DroidSansMono.ttf`

 * *Files identical despite different names*

### Comparing `e-qsl-0.1.7/fonts/Ubuntu Mono derivative Powerline Bold.ttf` & `e-qsl-0.1.8/fonts/Ubuntu Mono derivative Powerline Bold.ttf`

 * *Files identical despite different names*

### Comparing `e-qsl-0.1.7/fonts/VeraMono-Italic.ttf` & `e-qsl-0.1.8/fonts/VeraMono-Italic.ttf`

 * *Files identical despite different names*

### Comparing `e-qsl-0.1.7/misc/qsl-example.jpg` & `e-qsl-0.1.8/misc/qsl-example.jpg`

 * *Files identical despite different names*

### Comparing `e-qsl-0.1.7/setup.py` & `e-qsl-0.1.8/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 
 import sys
 
 from setuptools import setup
 
 __author__ = "Fred C. (W6BSD)"
-__version__ = "0.1.7"
+__version__ = "0.1.8"
 __license__ = 'BSD-3'
 
 py_version = sys.version_info[:2]
 if py_version < (3, 8):
   raise RuntimeError('eqsl requires Python 3.8 or later')
 
 def readme():
```

