# Comparing `tmp/xpywm-1.8.tar.gz` & `tmp/xpywm-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/xpywm-1.8.tar", last modified: Sun Oct 20 03:45:05 2019, max compression
+gzip compressed data, was "dist/xpywm-1.9.tar", last modified: Fri Oct 25 00:10:24 2019, max compression
```

## Comparing `xpywm-1.8.tar` & `xpywm-1.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 ohsaki    (1000) ohsaki    (1000)        0 2019-10-20 03:45:05.000000 xpywm-1.8/
--rw-r--r--   0 ohsaki    (1000) ohsaki    (1000)     8209 2019-10-20 03:45:05.000000 xpywm-1.8/PKG-INFO
--rw-r--r--   0 ohsaki    (1000) ohsaki    (1000)     6136 2019-07-06 09:14:52.000000 xpywm-1.8/README.md
--rw-r--r--   0 ohsaki    (1000) ohsaki    (1000)       38 2019-10-20 03:45:05.000000 xpywm-1.8/setup.cfg
--rwxr-xr-x   0 ohsaki    (1000) ohsaki    (1000)      929 2019-10-20 03:44:56.000000 xpywm-1.8/setup.py
--rwxr-xr-x   0 ohsaki    (1000) ohsaki    (1000)    36351 2019-10-20 03:44:21.000000 xpywm-1.8/xpywm
-drwxr-xr-x   0 ohsaki    (1000) ohsaki    (1000)        0 2019-10-20 03:45:05.000000 xpywm-1.8/xpywm.egg-info/
--rw-r--r--   0 ohsaki    (1000) ohsaki    (1000)     8209 2019-10-20 03:45:05.000000 xpywm-1.8/xpywm.egg-info/PKG-INFO
--rw-r--r--   0 ohsaki    (1000) ohsaki    (1000)      168 2019-10-20 03:45:05.000000 xpywm-1.8/xpywm.egg-info/SOURCES.txt
--rw-r--r--   0 ohsaki    (1000) ohsaki    (1000)        1 2019-10-20 03:45:05.000000 xpywm-1.8/xpywm.egg-info/dependency_links.txt
--rw-r--r--   0 ohsaki    (1000) ohsaki    (1000)        5 2019-10-20 03:45:05.000000 xpywm-1.8/xpywm.egg-info/requires.txt
--rw-r--r--   0 ohsaki    (1000) ohsaki    (1000)        1 2019-10-20 03:45:05.000000 xpywm-1.8/xpywm.egg-info/top_level.txt
+drwxr-xr-x   0 ohsaki    (1000) ohsaki    (1000)        0 2019-10-25 00:10:24.000000 xpywm-1.9/
+-rw-r--r--   0 ohsaki    (1000) ohsaki    (1000)     8209 2019-10-25 00:10:24.000000 xpywm-1.9/PKG-INFO
+-rw-r--r--   0 ohsaki    (1000) ohsaki    (1000)     6136 2019-07-06 09:14:52.000000 xpywm-1.9/README.md
+-rw-r--r--   0 ohsaki    (1000) ohsaki    (1000)       38 2019-10-25 00:10:24.000000 xpywm-1.9/setup.cfg
+-rwxr-xr-x   0 ohsaki    (1000) ohsaki    (1000)      929 2019-10-25 00:10:11.000000 xpywm-1.9/setup.py
+-rwxr-xr-x   0 ohsaki    (1000) ohsaki    (1000)    37479 2019-10-25 00:08:10.000000 xpywm-1.9/xpywm
+drwxr-xr-x   0 ohsaki    (1000) ohsaki    (1000)        0 2019-10-25 00:10:24.000000 xpywm-1.9/xpywm.egg-info/
+-rw-r--r--   0 ohsaki    (1000) ohsaki    (1000)     8209 2019-10-25 00:10:24.000000 xpywm-1.9/xpywm.egg-info/PKG-INFO
+-rw-r--r--   0 ohsaki    (1000) ohsaki    (1000)      168 2019-10-25 00:10:24.000000 xpywm-1.9/xpywm.egg-info/SOURCES.txt
+-rw-r--r--   0 ohsaki    (1000) ohsaki    (1000)        1 2019-10-25 00:10:24.000000 xpywm-1.9/xpywm.egg-info/dependency_links.txt
+-rw-r--r--   0 ohsaki    (1000) ohsaki    (1000)        5 2019-10-25 00:10:24.000000 xpywm-1.9/xpywm.egg-info/requires.txt
+-rw-r--r--   0 ohsaki    (1000) ohsaki    (1000)        1 2019-10-25 00:10:24.000000 xpywm-1.9/xpywm.egg-info/top_level.txt
```

### Comparing `xpywm-1.8/PKG-INFO` & `xpywm-1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xpywm
-Version: 1.8
+Version: 1.9
 Summary: A simple but extensible X11 window manager written in Python
 Home-page: https://github.com/h-ohsaki/xpywm.git
 Author: Hiroyuki Ohsaki
 Author-email: ohsaki@lsnl.jp
 License: UNKNOWN
 Description: # NAME
```

### Comparing `xpywm-1.8/README.md` & `xpywm-1.9/README.md`

 * *Files identical despite different names*

### Comparing `xpywm-1.8/setup.py` & `xpywm-1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='xpywm',
-    version='1.8',
+    version='1.9',
     author='Hiroyuki Ohsaki',
     author_email='ohsaki@lsnl.jp',
     description='A simple but extensible X11 window manager written in Python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/h-ohsaki/xpywm.git',
     packages=setuptools.find_packages(),
```

### Comparing `xpywm-1.8/xpywm` & `xpywm-1.9/xpywm`

 * *Files 4% similar despite different names*

```diff
@@ -196,16 +196,15 @@
     enable the output with the resolution of 800 x 600 pixels."""
     output = subprocess.getoutput('xrandr')
     m = re.search(r'\n(DP-?\d|HDMI-?\d) connected', output, re.MULTILINE)
     if m:
         output = m.group(1)
         # NOTE: some LCD projectors fails to recognize without turning off
         os.system('xrandr --output {} --off'.format(output))
-        os.system(
-            'xrandr --output {} --mode 800x600'.format(output))
+        os.system('xrandr --output {} --mode 800x600'.format(output))
         return
 
 def get_mixer_level():
     """Return the master playback volume of the default ALSA audio device.
     Volume ranges between 0 and 100."""
     output = subprocess.getoutput('amixer get Master')
     m = re.search(r'Playback.*\[(\d+)%\]', output)
@@ -326,14 +325,30 @@
         except:
             return ''
         if cls is not None:
             return cls
         else:
             return ''
 
+    def get_window_geometry(self, window):
+        """Obtain the geometry and attributes of the window WINDOW.  Return as
+        a Xlib.protocol.rq.Struct object.  Valid attributes are x, y, width,
+        height, root, depth, border_width, and sequence_number.  Return None
+        if the geometry is not retrieved."""
+        try:
+            return window.get_geometry()
+        except:
+            return None
+
+    def get_window_attribute(self, window):
+        try:
+            return window.get_attributes()
+        except:
+            return None
+
     def window_shortname(self, window):
         return '0x{:x} [{}]'.format(window.id, self.get_window_class(window))
 
     def get_screen_size(self):
         """Return the dimension (WIDTH, HEIGHT) of the current screen as a
         tuple in pixels.  If xrandr command exsits and either DP (DisplayPort)
         or HDMI output is active, return its dimensionn instead of the screen
@@ -436,15 +451,17 @@
         debug('draw_frame_windows: %s', self.window_shortname(window))
         if 'mpv' in self.get_window_class(window):
             self.hide_frame_windows(window)
         else:
             self._draw_frame_windows(window)
 
     def _draw_frame_windows(self, window):
-        geom = window.get_geometry()
+        geom = self.get_window_geometry(window)
+        if geom is None:
+            return
         for side in ['frame_l', 'frame_r', 'frame_u', 'frame_d', 'title']:
             x, y, width, height = 0, 0, 0, 0
             if side == 'frame_l':
                 x = geom.x - FRAME_WIDTH
                 y = geom.y
                 width = FRAME_WIDTH
                 height = geom.height
@@ -489,18 +506,16 @@
             win = self.frame_windows[side]
             win.unmap()
 
     def manage_window(self, window):
         """The window WINDOW is put under the control of the window manager.
         The window is forced to be mapped on the current virtual screen.  The
         geometry of the window is unchnaged."""
-        # skip if the window seems invalid
-        try:
-            attrs = window.get_attributes()
-        except:
+        attrs = self.get_window_attribute(window)
+        if attrs is None:
             return
         # skip if the window should not be intercepted by window manager
         if attrs.override_redirect:
             return
         # skip if the window is under our control
         if self.is_managed_window(window):
             return
@@ -568,60 +583,68 @@
         self.draw_frame_windows(window)
 
     def focus_next_window(self, window=None):
         """Change the active window from the window WINDOW to the next one.
         The active window is raised and focused.  The pointer is moved to the
         north-west of the window."""
         def _sort_key(window):
-            geom = window.get_geometry()
-            return geom.x * 10000 + geom.y
+            geom = self.get_window_geometry(window)
+            if geom is None:
+                return 100000000
+            else:
+                return geom.x * 10000 + geom.y
 
         # sort active windows with their geometries
         windows = sorted(self.exposed_windows, key=_sort_key)
         try:
             i = windows.index(window)
             next_window = windows[(i + 1) % len(windows)]
         except ValueError:
             if windows:
                 next_window = windows[0]
             else:
                 return
         next_window.raise_window()
-        geom = next_window.get_geometry()
         next_window.warp_pointer(PNT_OFFSET, PNT_OFFSET)
         self.focus_window(next_window)
 
     def is_maximized(self, window):
         """Check if the window WINDOW seems to have been maximized."""
-        geom = window.get_geometry()
+        geom = self.get_window_geometry(window)
+        if geom is None:
+            return False
         width, height = self.get_usable_screen_size()
         if geom.x == 0 and geom.width == width:
             return True
         if geom.y == Y_OFFSET and geom.height == height:
             return True
         return False
 
     def save_window_geometry(self, window):
         """Save the current geometry of the window WINDOW."""
-        geom = window.get_geometry()
+        geom = self.get_window_geometry(window)
+        if geom is None:
+            return
         self.geometries[window] = {
             'x': geom.x, 'y': geom.y, 'width': geom.width, 'height':
             geom.height
         }
 
     def load_window_geometry(self, window):
         """Return the saved geometry of the window WINDOW.  If not saved yet,
         return None."""
         return self.geometries.get(window, None)
 
     def maximize_window(self, window, horizontally=True, vertically=True):
         """Resize the geometry of the window WINDOW to cover the screen
         horizontally and/or vertically."""
         screen_width, screen_height = self.get_usable_screen_size()
-        geom = window.get_geometry()
+        geom = self.get_window_geometry(window)
+        if geom is None:
+            return
         x, y = geom.x, geom.y
         width, height = geom.width, geom.height
         if horizontally:
             x, width = 0, screen_width
         if vertically:
             y, height = Y_OFFSET, screen_height
         window.configure(x=x, y=y, width=width, height=height)
@@ -635,15 +658,17 @@
 
     def find_geometry_by_rules(self, window):
         """Look through the configuration variable LAYOUT_RULES and identify
         the desired geometry (x, y, width, and height) of WINDOW.  The geometry is returned as
         a dictionary.  Return None if no rule is found."""
         debug('find_geometry_by_rules: %s', self.window_shortname(window))
         cls = self.get_window_class(window)
-        cur_geom = window.get_geometry()
+        cur_geom = self.get_window_geometry(window)
+        if cur_geom is None:
+            return None
         screen_width, screen_height = self.get_usable_screen_size()
         for regexp, geom in LAYOUT_RULES.items():
             if re.search(regexp, cls, flags=re.IGNORECASE):
                 debug("  rule found -> '%s': %s", regexp, geom)
                 # toggle the location of office applications
                 if 'office' in regexp and cur_geom.x > screen_width / 4:
                     geom = [0, 0, .5 + LAYOUT_OFFSET, 1]
@@ -760,14 +785,20 @@
 
     def cb_focus_next_window(self, event):
         window = event.child
         self.focus_next_window(window)
 
     def cb_maximize_window(self, event, horizontally=True):
         window = event.child
+        attrs = self.get_window_attribute(window)
+        if attrs is None:
+            return
+        # ignore if the window should not be intercepted by window manager
+        if attrs.override_redirect:
+            return
         if self.is_maximized(window) and self.load_window_geometry(window):
             window.configure(**self.load_window_geometry(window))
             self.draw_frame_windows(window)
             window.warp_pointer(PNT_OFFSET, PNT_OFFSET)
         else:
             self.save_window_geometry(window)
             self.maximize_window(window, horizontally=horizontally)
@@ -834,15 +865,16 @@
         the button is relased."""
         window = event.child
         self.screen.root.grab_pointer(
             True, X.PointerMotionMask | X.ButtonReleaseMask, X.GrabModeAsync,
             X.GrabModeAsync, X.NONE, X.NONE, 0)
         self.drag_window = window
         self.drag_button = event.detail
-        self.drag_geometry = window.get_geometry()
+        # FIXME: drag_geometry might be None
+        self.drag_geometry = self.get_window_geometry(window)
         self.drag_start_xy = event.root_x, event.root_y
 
     def handle_button_release(self, event):
         """Terminate window repositioning/resizing."""
         self.display.ungrab_pointer(0)
 
     def _may_switch_virtual_screen(self, x, y):
```

### Comparing `xpywm-1.8/xpywm.egg-info/PKG-INFO` & `xpywm-1.9/xpywm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xpywm
-Version: 1.8
+Version: 1.9
 Summary: A simple but extensible X11 window manager written in Python
 Home-page: https://github.com/h-ohsaki/xpywm.git
 Author: Hiroyuki Ohsaki
 Author-email: ohsaki@lsnl.jp
 License: UNKNOWN
 Description: # NAME
```

