# Comparing `tmp/cursesplus-2.0.2.tar.gz` & `tmp/cursesplus-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cursesplus-2.0.2.tar", last modified: Fri Apr 14 17:55:16 2023, max compression
+gzip compressed data, was "cursesplus-2.0.3.tar", last modified: Sun Apr 16 17:47:53 2023, max compression
```

## Comparing `cursesplus-2.0.2.tar` & `cursesplus-2.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-04-14 17:55:16.873825 cursesplus-2.0.2/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1089 2023-04-07 16:31:31.000000 cursesplus-2.0.2/LICENSE
--rw-r--r--   0 jordan    (1000) jordan    (1000)     1617 2023-04-14 17:55:16.873825 cursesplus-2.0.2/PKG-INFO
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1014 2023-04-14 17:48:06.000000 cursesplus-2.0.2/README.md
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      659 2023-04-14 17:55:01.000000 cursesplus-2.0.2/pyproject.toml
--rw-r--r--   0 jordan    (1000) jordan    (1000)       38 2023-04-14 17:55:16.873825 cursesplus-2.0.2/setup.cfg
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-04-14 17:55:16.873825 cursesplus-2.0.2/src/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      555 2023-04-07 16:31:31.000000 cursesplus-2.0.2/src/__cptest.py
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-04-14 17:55:16.873825 cursesplus-2.0.2/src/cursesplus/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      892 2023-04-07 16:31:31.000000 cursesplus-2.0.2/src/cursesplus/__init__.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)    11516 2023-04-07 16:31:31.000000 cursesplus-2.0.2/src/cursesplus/cp.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)    11277 2023-04-07 16:45:57.000000 cursesplus-2.0.2/src/cursesplus/filedialog.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     5980 2023-04-14 17:54:57.000000 cursesplus-2.0.2/src/cursesplus/messagebox.py
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-04-14 17:55:16.873825 cursesplus-2.0.2/src/cursesplus.egg-info/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1617 2023-04-14 17:55:16.000000 cursesplus-2.0.2/src/cursesplus.egg-info/PKG-INFO
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      306 2023-04-14 17:55:16.000000 cursesplus-2.0.2/src/cursesplus.egg-info/SOURCES.txt
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)        1 2023-04-14 17:55:16.000000 cursesplus-2.0.2/src/cursesplus.egg-info/dependency_links.txt
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)       20 2023-04-14 17:55:16.000000 cursesplus-2.0.2/src/cursesplus.egg-info/top_level.txt
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-04-16 17:47:53.832487 cursesplus-2.0.3/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1089 2023-04-07 16:31:31.000000 cursesplus-2.0.3/LICENSE
+-rw-r--r--   0 jordan    (1000) jordan    (1000)     1624 2023-04-16 17:47:53.832487 cursesplus-2.0.3/PKG-INFO
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1021 2023-04-16 17:47:37.000000 cursesplus-2.0.3/README.md
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      659 2023-04-16 17:47:19.000000 cursesplus-2.0.3/pyproject.toml
+-rw-r--r--   0 jordan    (1000) jordan    (1000)       38 2023-04-16 17:47:53.832487 cursesplus-2.0.3/setup.cfg
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-04-16 17:47:53.812487 cursesplus-2.0.3/src/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      555 2023-04-07 16:31:31.000000 cursesplus-2.0.3/src/__cptest.py
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-04-16 17:47:53.822487 cursesplus-2.0.3/src/cursesplus/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      892 2023-04-07 16:31:31.000000 cursesplus-2.0.3/src/cursesplus/__init__.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)    11516 2023-04-07 16:31:31.000000 cursesplus-2.0.3/src/cursesplus/cp.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)    11982 2023-04-16 17:46:39.000000 cursesplus-2.0.3/src/cursesplus/filedialog.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     5980 2023-04-14 17:54:57.000000 cursesplus-2.0.3/src/cursesplus/messagebox.py
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-04-16 17:47:53.822487 cursesplus-2.0.3/src/cursesplus.egg-info/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1624 2023-04-16 17:47:53.000000 cursesplus-2.0.3/src/cursesplus.egg-info/PKG-INFO
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      306 2023-04-16 17:47:53.000000 cursesplus-2.0.3/src/cursesplus.egg-info/SOURCES.txt
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)        1 2023-04-16 17:47:53.000000 cursesplus-2.0.3/src/cursesplus.egg-info/dependency_links.txt
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)       20 2023-04-16 17:47:53.000000 cursesplus-2.0.3/src/cursesplus.egg-info/top_level.txt
```

### Comparing `cursesplus-2.0.2/LICENSE` & `cursesplus-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cursesplus-2.0.2/PKG-INFO` & `cursesplus-2.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cursesplus
-Version: 2.0.2
+Version: 2.0.3
 Summary: An extension program to curses that offers option menus, message boxes, file dialogs and more
 Author-email: Enderbyte Programs <enderbyte09@gmail.com>
 Project-URL: Homepage, https://github.com/Enderbyte-Programs/Curses-Plus
 Project-URL: Bug Tracker, https://github.com/Enderbyte-Programs/Curses-Plus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -36,17 +36,17 @@
 Microsoft Windows 11
 Any modern distro of Linux that supports Python3
 
 **Python Version 3.6 or newer**
 
 ## What's New?
 
-### Version 2.0.1
+### Version 2.0.3
 
-Colour is now optional in messagebox
+Huge performance improvements to filedialog
 
 ### Version 2.0: Incompatible api changes
 
 -askyesno now MUST be messagebox.askyesno
 -Rewrite colour system. load_colours() is now nonexistent.
 -Now use set_colour(background,foreground). A set of colour constants are defined in the cp class.
```

### Comparing `cursesplus-2.0.2/README.md` & `cursesplus-2.0.3/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 Microsoft Windows 11
 Any modern distro of Linux that supports Python3
 
 **Python Version 3.6 or newer**
 
 ## What's New?
 
-### Version 2.0.1
+### Version 2.0.3
 
-Colour is now optional in messagebox
+Huge performance improvements to filedialog
 
 ### Version 2.0: Incompatible api changes
 
 -askyesno now MUST be messagebox.askyesno
 -Rewrite colour system. load_colours() is now nonexistent.
 -Now use set_colour(background,foreground). A set of colour constants are defined in the cp class.
```

### Comparing `cursesplus-2.0.2/pyproject.toml` & `cursesplus-2.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "cursesplus"
-version = "2.0.2"
+version = "2.0.3"
 authors = [{name="Enderbyte Programs",email="enderbyte09@gmail.com"},]
 description = "An extension program to curses that offers option menus, message boxes, file dialogs and more"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"License :: OSI Approved :: MIT License",
```

### Comparing `cursesplus-2.0.2/src/__cptest.py` & `cursesplus-2.0.3/src/__cptest.py`

 * *Files identical despite different names*

### Comparing `cursesplus-2.0.2/src/cursesplus/__init__.py` & `cursesplus-2.0.3/src/cursesplus/__init__.py`

 * *Files identical despite different names*

### Comparing `cursesplus-2.0.2/src/cursesplus/cp.py` & `cursesplus-2.0.3/src/cursesplus/cp.py`

 * *Files identical despite different names*

### Comparing `cursesplus-2.0.2/src/cursesplus/filedialog.py` & `cursesplus-2.0.3/src/cursesplus/filedialog.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,35 +51,48 @@
 
     RETURNS the full file path chosen
     """
     xoffset: int = 0
     yoffset: int = 0
     activefilter: int = 0
     selected: int = 0
+    refresh: bool = False
+    masterlist: list = list[Fileobj]
+    directories = [directory+"/"+l for l in os.listdir(directory) if os.path.isdir(directory+"/"+l)]
+    if filter[activefilter][0].strip() == "*":
+        files = [directory+"/"+l for l in os.listdir(directory) if os.path.isfile(directory+"/"+l)]
+    else:
+        files = glob.glob(directory+"/"+filter[activefilter][0])
+    directories.sort()
+    files.sort()
+    #displaymsg(stdscr,directories+files)
+    masterlist = [Fileobj(f) for f in (directories+files)]
     while True:
-        masterlist: list = list[Fileobj]
+        
         mx,my = os.get_terminal_size()
         MAXNL = mx - 33
         stdscr.clear()
         cp.rectangle(stdscr,2,0,my-2,mx-1)
         cp.filline(stdscr,0,cp.set_color(cp.BLUE,cp.WHITE))
         cp.filline(stdscr,1,cp.set_color(cp.GREEN,cp.WHITE))
         cp.filline(stdscr,my-2,cp.set_color(cp.WHITE,cp.BLACK))
         cp.filline(stdscr,my-1,cp.set_color(cp.RED,cp.WHITE))
         topline = "Name"+" "*(MAXNL-4)+"|"+"Size     "+"|Date Modified"
         topline = topline+(mx-2-len(topline))*" "
-        directories = [directory+"/"+l for l in os.listdir(directory) if os.path.isdir(directory+"/"+l)]
-        if filter[activefilter][0].strip() == "*":
-            files = [directory+"/"+l for l in os.listdir(directory) if os.path.isfile(directory+"/"+l)]
-        else:
-            files = glob.glob(directory+"/"+filter[activefilter][0])
-        directories.sort()
-        files.sort()
-        #displaymsg(stdscr,directories+files)
-        masterlist = [Fileobj(f) for f in (directories+files)]
+        if refresh:
+            masterlist: list = list[Fileobj]
+            directories = [directory+"/"+l for l in os.listdir(directory) if os.path.isdir(directory+"/"+l)]
+            if filter[activefilter][0].strip() == "*":
+                files = [directory+"/"+l for l in os.listdir(directory) if os.path.isfile(directory+"/"+l)]
+            else:
+                files = glob.glob(directory+"/"+filter[activefilter][0])
+            directories.sort()
+            files.sort()
+            #displaymsg(stdscr,directories+files)
+            masterlist = [Fileobj(f) for f in (directories+files)]
         stdscr.addstr(0,0,title+"|H for Help|Press Shift-Left Arrow to move up directory"[0:mx],cp.set_colour(cp.BLUE,cp.WHITE))
         stdscr.addstr(1,0,directory[xoffset:xoffset+mx],cp.set_colour(cp.GREEN,cp.WHITE))
         stdscr.addstr(my-2,0,f"{filter[activefilter][1]} ({filter[activefilter][0]}) [{len(masterlist)} objects found]"[0:mx],cp.set_colour(cp.WHITE,cp.BLACK))
         stdscr.addstr(2,1,topline[0:mx-1])
         
         try:
             stdscr.addstr(my-1,0,masterlist[selected].path[xoffset:xoffset+mx],cp.set_colour(cp.RED,cp.WHITE))
@@ -101,15 +114,15 @@
                 stdscr.addstr(3+indx,1,wstr)
             ind += 1
             indx += 1#Inc both
 
         
         stdscr.refresh()
         ch = stdscr.getch()
-
+        refresh = False
         if ch == cp.curses.KEY_LEFT and xoffset > 0:
             xoffset -= 1
         elif ch == cp.curses.KEY_RIGHT:
             xoffset += 1
         elif ch == cp.curses.KEY_UP and selected > 0:
             selected -= 1
             if selected < yoffset:
@@ -118,31 +131,34 @@
             if selected - yoffset > my - 7:
                 yoffset += 1
             selected += 1
         elif ch == 102:
             activefilter = cp.displayops(stdscr,[f"{f[1]} ({f[0]})" for f in filter],"Please choose a filter")
             selected = 0
             yoffset = 0
+            refresh = True
         elif ch == cp.curses.KEY_ENTER or ch == 10 or ch == 13:
             if masterlist[selected].isdir:
                 directory = masterlist[selected].path
                 selected = 0
+                refresh = True
                 yoffset = 0
             else:
                 return masterlist[selected].path
         elif ch == cp.curses.KEY_SLEFT or ch == 98:
             directory = "/".join(directory.split("/")[0:-1])
             selected = 0
             yoffset = 0
+            refresh = True
             if directory == "":
                 directory = "/"
         elif ch == 104:
             cp.displaymsg(stdscr,["List of Keybinds","Down Arrow: Scroll down","Up Arrow: Scroll up","Left Arrow: Scroll left","Right Arrow: Scroll right","Shift-left arrow: Move up to parent Directory","Enter: Open/select","F: Change filter"])
 
-        masterlist.clear()
+        #masterlist.clear()
 
 def openfilesdialog(stdscr,title: str = "Please choose a file",filter: str = [["*","All Files"]],directory: str = os.getcwd()) -> list:
     """Start a filedialog to select multiple files. title is the prompt the user recieves. filter is the file filter. The filter syntax is the same as TK syntax. The first
     filter provided is the main filter. 
     Filter Syntax: 
     [[GLOB,NAME],[GLOB,NAME]]
     Glob is a pattern to match for files (like *.txt)
```

### Comparing `cursesplus-2.0.2/src/cursesplus/messagebox.py` & `cursesplus-2.0.3/src/cursesplus/messagebox.py`

 * *Files identical despite different names*

### Comparing `cursesplus-2.0.2/src/cursesplus.egg-info/PKG-INFO` & `cursesplus-2.0.3/src/cursesplus.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cursesplus
-Version: 2.0.2
+Version: 2.0.3
 Summary: An extension program to curses that offers option menus, message boxes, file dialogs and more
 Author-email: Enderbyte Programs <enderbyte09@gmail.com>
 Project-URL: Homepage, https://github.com/Enderbyte-Programs/Curses-Plus
 Project-URL: Bug Tracker, https://github.com/Enderbyte-Programs/Curses-Plus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -36,17 +36,17 @@
 Microsoft Windows 11
 Any modern distro of Linux that supports Python3
 
 **Python Version 3.6 or newer**
 
 ## What's New?
 
-### Version 2.0.1
+### Version 2.0.3
 
-Colour is now optional in messagebox
+Huge performance improvements to filedialog
 
 ### Version 2.0: Incompatible api changes
 
 -askyesno now MUST be messagebox.askyesno
 -Rewrite colour system. load_colours() is now nonexistent.
 -Now use set_colour(background,foreground). A set of colour constants are defined in the cp class.
```

