# Comparing `tmp/sunnyday-IZPy-2.0.0.tar.gz` & `tmp/sunnyday-IZPy-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sunnyday-IZPy-2.0.0.tar", last modified: Sun Apr 16 19:07:12 2023, max compression
+gzip compressed data, was "sunnyday-IZPy-2.1.0.tar", last modified: Sun Apr 16 19:26:19 2023, max compression
```

## Comparing `sunnyday-IZPy-2.0.0.tar` & `sunnyday-IZPy-2.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 19:07:12.283152 sunnyday-IZPy-2.0.0/
--rw-rw-rw-   0        0        0      387 2023-04-16 19:07:12.282153 sunnyday-IZPy-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-16 19:07:12.283152 sunnyday-IZPy-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0      557 2023-04-16 19:06:29.000000 sunnyday-IZPy-2.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-16 19:07:12.236155 sunnyday-IZPy-2.0.0/sunnyday_IZPy/
--rw-rw-rw-   0        0        0       44 2023-04-16 17:26:06.000000 sunnyday-IZPy-2.0.0/sunnyday_IZPy/__init__.py
--rw-rw-rw-   0        0        0     2616 2023-04-16 18:59:18.000000 sunnyday-IZPy-2.0.0/sunnyday_IZPy/sunnyday.py
-drwxrwxrwx   0        0        0        0 2023-04-16 19:07:12.281153 sunnyday-IZPy-2.0.0/sunnyday_IZPy.egg-info/
--rw-rw-rw-   0        0        0      387 2023-04-16 19:07:12.000000 sunnyday-IZPy-2.0.0/sunnyday_IZPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-04-16 19:07:12.000000 sunnyday-IZPy-2.0.0/sunnyday_IZPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 19:07:12.000000 sunnyday-IZPy-2.0.0/sunnyday_IZPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-16 19:07:12.000000 sunnyday-IZPy-2.0.0/sunnyday_IZPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-16 19:07:12.000000 sunnyday-IZPy-2.0.0/sunnyday_IZPy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 19:26:17.948710 sunnyday-IZPy-2.1.0/
+-rw-rw-rw-   0        0        0      387 2023-04-16 19:26:17.944714 sunnyday-IZPy-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-16 19:26:17.948710 sunnyday-IZPy-2.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      557 2023-04-16 19:24:57.000000 sunnyday-IZPy-2.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 19:26:17.900196 sunnyday-IZPy-2.1.0/sunnyday_IZPy/
+-rw-rw-rw-   0        0        0       44 2023-04-16 17:26:06.000000 sunnyday-IZPy-2.1.0/sunnyday_IZPy/__init__.py
+-rw-rw-rw-   0        0        0     2519 2023-04-16 19:18:16.000000 sunnyday-IZPy-2.1.0/sunnyday_IZPy/sunnyday.py
+drwxrwxrwx   0        0        0        0 2023-04-16 19:26:17.936201 sunnyday-IZPy-2.1.0/sunnyday_IZPy.egg-info/
+-rw-rw-rw-   0        0        0      387 2023-04-16 19:26:17.000000 sunnyday-IZPy-2.1.0/sunnyday_IZPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-04-16 19:26:17.000000 sunnyday-IZPy-2.1.0/sunnyday_IZPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 19:26:17.000000 sunnyday-IZPy-2.1.0/sunnyday_IZPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-16 19:26:17.000000 sunnyday-IZPy-2.1.0/sunnyday_IZPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-16 19:26:17.000000 sunnyday-IZPy-2.1.0/sunnyday_IZPy.egg-info/top_level.txt
```

### Comparing `sunnyday-IZPy-2.0.0/setup.py` & `sunnyday-IZPy-2.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 import setuptools
 
 setuptools.setup(
     name='sunnyday-IZPy',
     packages=setuptools.find_packages(),
-    version='2.0.0',
+    version='2.1.0',
     license='MIT',
     description='Weather forecast data',
     author='Ivo Zelic',
     author_email='izpy81@gmail.com',
     url='https://github.com/DevIvo81/App-011-WeatherApp',
     keywords=['weather', 'forecast', 'openweather'],
     install_requires=['requests', ],
```

### Comparing `sunnyday-IZPy-2.0.0/sunnyday_IZPy/sunnyday.py` & `sunnyday-IZPy-2.1.0/sunnyday_IZPy/sunnyday.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,12 +65,7 @@
                     d["dt_txt"],
                     f'{d["main"]["temp"]} °C',
                     d["weather"][0]["description"].capitalize(),
                     d["weather"][0]["icon"]
                 )
             )
         return simple_data
-
-
-w = Weather("30327208ce508bd9097832f10c756ab9", 'Zagreb')
-
-print(w.next_12h_simplified())
```

