# Comparing `tmp/metalcompute-0.2.3.tar.gz` & `tmp/metalcompute-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metalcompute-0.2.3.tar", last modified: Tue Dec 28 15:12:36 2021, max compression
+gzip compressed data, was "metalcompute-0.2.4.tar", last modified: Sun Apr 16 13:46:44 2023, max compression
```

## Comparing `metalcompute-0.2.3.tar` & `metalcompute-0.2.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 15:12:36.903970 metalcompute-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2021-12-28 15:12:36.000000 metalcompute-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       19 2021-12-28 15:12:36.000000 metalcompute-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5134 2021-12-28 15:12:36.903970 metalcompute-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3410 2021-12-28 15:12:36.000000 metalcompute-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 15:12:36.903970 metalcompute-0.2.3/examples/
--rwxr-xr-x   0 runner    (1001) docker     (121)     2971 2021-12-28 15:12:36.000000 metalcompute-0.2.3/examples/metalcompute-mandelbrot
--rwxr-xr-x   0 runner    (1001) docker     (121)     2883 2021-12-28 15:12:36.000000 metalcompute-0.2.3/examples/metalcompute-measure
--rwxr-xr-x   0 runner    (1001) docker     (121)      654 2021-12-28 15:12:36.000000 metalcompute-0.2.3/examples/metalcompute-pipe
--rwxr-xr-x   0 runner    (1001) docker     (121)     2860 2021-12-28 15:12:36.000000 metalcompute-0.2.3/examples/metalcompute-raymarch
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 15:12:36.903970 metalcompute-0.2.3/metalcompute.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5134 2021-12-28 15:12:36.000000 metalcompute-0.2.3/metalcompute.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      360 2021-12-28 15:12:36.000000 metalcompute-0.2.3/metalcompute.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-28 15:12:36.000000 metalcompute-0.2.3/metalcompute.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2021-12-28 15:12:36.000000 metalcompute-0.2.3/metalcompute.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       95 2021-12-28 15:12:36.000000 metalcompute-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-28 15:12:36.903970 metalcompute-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2482 2021-12-28 15:12:36.000000 metalcompute-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 15:12:36.903970 metalcompute-0.2.3/src/
--rw-r--r--   0 runner    (1001) docker     (121)    24966 2021-12-28 15:12:36.000000 metalcompute-0.2.3/src/metalcompute.c
--rw-r--r--   0 runner    (1001) docker     (121)    17995 2021-12-28 15:12:36.000000 metalcompute-0.2.3/src/metalcompute.swift
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:46:44.004340 metalcompute-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-16 13:46:40.000000 metalcompute-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-16 13:46:40.000000 metalcompute-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-04-16 13:46:44.004340 metalcompute-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-04-16 13:46:40.000000 metalcompute-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:46:44.004340 metalcompute-0.2.4/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2971 2023-04-16 13:46:40.000000 metalcompute-0.2.4/examples/metalcompute-mandelbrot
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2885 2023-04-16 13:46:40.000000 metalcompute-0.2.4/examples/metalcompute-measure
+-rwxr-xr-x   0 runner    (1001) docker     (123)      654 2023-04-16 13:46:40.000000 metalcompute-0.2.4/examples/metalcompute-pipe
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2860 2023-04-16 13:46:40.000000 metalcompute-0.2.4/examples/metalcompute-raymarch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:46:44.004340 metalcompute-0.2.4/metalcompute.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-04-16 13:46:43.000000 metalcompute-0.2.4/metalcompute.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-16 13:46:43.000000 metalcompute-0.2.4/metalcompute.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 13:46:43.000000 metalcompute-0.2.4/metalcompute.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-16 13:46:43.000000 metalcompute-0.2.4/metalcompute.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-16 13:46:40.000000 metalcompute-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 13:46:44.004340 metalcompute-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-04-16 13:46:40.000000 metalcompute-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:46:44.004340 metalcompute-0.2.4/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    25123 2023-04-16 13:46:40.000000 metalcompute-0.2.4/src/metalcompute.c
+-rw-r--r--   0 runner    (1001) docker     (123)    17995 2023-04-16 13:46:40.000000 metalcompute-0.2.4/src/metalcompute.swift
```

### Comparing `metalcompute-0.2.3/LICENSE` & `metalcompute-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `metalcompute-0.2.3/PKG-INFO` & `metalcompute-0.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metalcompute
-Version: 0.2.3
+Version: 0.2.4
 Summary: A python library to run metal compute kernels on macOS
 Home-page: https://github.com/baldand/py-metal-compute
 Author: Andrew Baldwin
 Author-email: metalcompute@dehabit.info
 License: UNKNOWN
 Project-URL: Issue Tracker, https://github.com/baldand/py-metal-compute/issues
 Description: # metalcompute for Python
@@ -134,14 +134,22 @@
         Render took 0.401446s
         Writing image to mandelbrot.png
         Image encoding took 1.35182s
         ```
         
         ![Mandelbrot set](images/mandelbrot.jpg)
         
+        ### Livecoding visual kernels in VSCode
+        
+        There is an example script to allow livecoding of visual metal kernels entirely within VSCode using a localhost http server to render frames.
+        
+        It also includes syntax error highlighting in the editor.
+        
+        See [livemetal.py](examples/livecode)
+        
         ## Status
         
         This is a preview version. 
         
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `metalcompute-0.2.3/README.md` & `metalcompute-0.2.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -125,10 +125,18 @@
 Render took 0.401446s
 Writing image to mandelbrot.png
 Image encoding took 1.35182s
 ```
 
 ![Mandelbrot set](images/mandelbrot.jpg)
 
+### Livecoding visual kernels in VSCode
+
+There is an example script to allow livecoding of visual metal kernels entirely within VSCode using a localhost http server to render frames.
+
+It also includes syntax error highlighting in the editor.
+
+See [livemetal.py](examples/livecode)
+
 ## Status
 
 This is a preview version.
```

### Comparing `metalcompute-0.2.3/examples/metalcompute-mandelbrot` & `metalcompute-0.2.4/examples/metalcompute-mandelbrot`

 * *Files identical despite different names*

### Comparing `metalcompute-0.2.3/examples/metalcompute-measure` & `metalcompute-0.2.4/examples/metalcompute-measure`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
     kernel_end = """
     }
     float v = v1 + v2 + v3 + v4;
     out[id] = v;
 }
     """
-    count = 1024*64
+    count = 8*1024*64
 
     print("Running compute intensive Metal kernel to measure TFLOPS...")
     dev = mc.Device(device_index)
     steps = 700
     fn = dev.kernel(kernel_start+kernel_step*steps+kernel_end)\
         .function("test")
     in_buf = array('f',[0.42])
```

### Comparing `metalcompute-0.2.3/examples/metalcompute-pipe` & `metalcompute-0.2.4/examples/metalcompute-pipe`

 * *Files identical despite different names*

### Comparing `metalcompute-0.2.3/examples/metalcompute-raymarch` & `metalcompute-0.2.4/examples/metalcompute-raymarch`

 * *Files identical despite different names*

### Comparing `metalcompute-0.2.3/metalcompute.egg-info/PKG-INFO` & `metalcompute-0.2.4/metalcompute.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metalcompute
-Version: 0.2.3
+Version: 0.2.4
 Summary: A python library to run metal compute kernels on macOS
 Home-page: https://github.com/baldand/py-metal-compute
 Author: Andrew Baldwin
 Author-email: metalcompute@dehabit.info
 License: UNKNOWN
 Project-URL: Issue Tracker, https://github.com/baldand/py-metal-compute/issues
 Description: # metalcompute for Python
@@ -134,14 +134,22 @@
         Render took 0.401446s
         Writing image to mandelbrot.png
         Image encoding took 1.35182s
         ```
         
         ![Mandelbrot set](images/mandelbrot.jpg)
         
+        ### Livecoding visual kernels in VSCode
+        
+        There is an example script to allow livecoding of visual metal kernels entirely within VSCode using a localhost http server to render frames.
+        
+        It also includes syntax error highlighting in the editor.
+        
+        See [livemetal.py](examples/livecode)
+        
         ## Status
         
         This is a preview version. 
         
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `metalcompute-0.2.3/setup.py` & `metalcompute-0.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,25 +13,25 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 def build_swift():
     print("Building swift object files")
     os.system("mkdir -p build/swift")
-    os.system("swiftc src/metalcompute.swift -I src -static -emit-library -target arm64-apple-macos11 -o build/swift/metalcomputeswiftarm.a")
-    os.system("swiftc src/metalcompute.swift -I src -static -emit-library -target x86_64-apple-macos11 -o build/swift/metalcomputeswiftx64.a")
+    os.system("swiftc -parse-as-library -c src/metalcompute.swift -I src -target arm64-apple-macos11 -o build/swift/metalcomputeswiftarm.a")
+    os.system("swiftc -parse-as-library -c src/metalcompute.swift -I src -target x86_64-apple-macos11 -o build/swift/metalcomputeswiftx64.a")
     os.system("lipo -create build/swift/metalcomputeswiftarm.a build/swift/metalcomputeswiftx64.a -o build/swift/metalcomputeswift.a")
 
 class build(build_module.build_ext):
     def run(self):
         build_swift()
         build_module.build_ext.run(self)
 
 setup(name="metalcompute",
-    version="0.2.3",
+    version="0.2.4",
     author="Andrew Baldwin",
     author_email="metalcompute@dehabit.info",
     description="A python library to run metal compute kernels on macOS",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/baldand/py-metal-compute",
     project_urls={
```

### Comparing `metalcompute-0.2.3/src/metalcompute.c` & `metalcompute-0.2.4/src/metalcompute.c`

 * *Files 1% similar despite different names*

```diff
@@ -554,23 +554,25 @@
 
     if (!PyObject_TypeCheck(dev_obj, &DeviceType)) {
         mc_err(FirstArgumentNotDevice);
         return -1;
     }
 
     // Is the argument an integer length?
+
     PyObject* as_long = PyNumber_Long(length_or_buffer);
+    int possible_buffer = PyObject_CheckBuffer(length_or_buffer);
     PyErr_Clear();
-    if (as_long != NULL) {
+    if (possible_buffer && !PyObject_GetBuffer(length_or_buffer, &buffer, PyBUF_ND)) {
+        length = buffer.len;
+        src = buffer.buf;
+    } else if (as_long != NULL) {
         // Yes
         length = PyLong_AsLongLong(as_long);
         src = NULL;
-    } else if (!PyObject_GetBuffer(length_or_buffer, &buffer, PyBUF_ND)) {
-        length = buffer.len;
-        src = buffer.buf;
     } else {
         // Nothing we can use
         mc_err(UnsupportedInputFormat);
         return -1;
     }
 
     if (mc_err(mc_sw_buf_open(&(dev_obj->dev_handle), length, src, &(self->buf_handle)))) {
@@ -717,17 +719,20 @@
     }
 
     if (mc_err(mc_sw_run_open(
         &(fn_obj->kern_obj->dev_obj->dev_handle),
         &(fn_obj->kern_obj->kern_handle),
         &(fn_obj->fn_handle),
         &(self->run_handle)))) {
+        free(self->run_handle.bufs);
         return -1;
     }
 
+    free(self->run_handle.bufs);
+
     self->fn_obj = fn_obj;
     Py_INCREF(fn_obj);
     // Keep this so that we have reference to all argument objects
     self->tuple_bufs = tuple_bufs;
 
     return 0;
 }
```

### Comparing `metalcompute-0.2.3/src/metalcompute.swift` & `metalcompute-0.2.4/src/metalcompute.swift`

 * *Files identical despite different names*

