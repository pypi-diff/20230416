# Comparing `tmp/sunnyday-IZPy-1.0.0.tar.gz` & `tmp/sunnyday-IZPy-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sunnyday-IZPy-1.0.0.tar", last modified: Sun Apr 16 17:33:13 2023, max compression
+gzip compressed data, was "sunnyday-IZPy-2.0.0.tar", last modified: Sun Apr 16 19:07:12 2023, max compression
```

## Comparing `sunnyday-IZPy-1.0.0.tar` & `sunnyday-IZPy-2.0.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 17:33:13.600028 sunnyday-IZPy-1.0.0/
--rw-rw-rw-   0        0        0      288 2023-04-16 17:33:13.597031 sunnyday-IZPy-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-16 17:33:13.600028 sunnyday-IZPy-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      454 2023-04-16 17:33:09.000000 sunnyday-IZPy-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-16 17:33:13.549029 sunnyday-IZPy-1.0.0/sunnyday_IZPy/
--rw-rw-rw-   0        0        0       44 2023-04-16 17:26:06.000000 sunnyday-IZPy-1.0.0/sunnyday_IZPy/__init__.py
--rw-rw-rw-   0        0        0     2377 2023-04-16 16:34:58.000000 sunnyday-IZPy-1.0.0/sunnyday_IZPy/sunnyday.py
-drwxrwxrwx   0        0        0        0 2023-04-16 17:33:13.586028 sunnyday-IZPy-1.0.0/sunnyday_IZPy.egg-info/
--rw-rw-rw-   0        0        0      288 2023-04-16 17:33:13.000000 sunnyday-IZPy-1.0.0/sunnyday_IZPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-04-16 17:33:13.000000 sunnyday-IZPy-1.0.0/sunnyday_IZPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 17:33:13.000000 sunnyday-IZPy-1.0.0/sunnyday_IZPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-16 17:33:13.000000 sunnyday-IZPy-1.0.0/sunnyday_IZPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-16 17:33:13.000000 sunnyday-IZPy-1.0.0/sunnyday_IZPy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 19:07:12.283152 sunnyday-IZPy-2.0.0/
+-rw-rw-rw-   0        0        0      387 2023-04-16 19:07:12.282153 sunnyday-IZPy-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-16 19:07:12.283152 sunnyday-IZPy-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      557 2023-04-16 19:06:29.000000 sunnyday-IZPy-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 19:07:12.236155 sunnyday-IZPy-2.0.0/sunnyday_IZPy/
+-rw-rw-rw-   0        0        0       44 2023-04-16 17:26:06.000000 sunnyday-IZPy-2.0.0/sunnyday_IZPy/__init__.py
+-rw-rw-rw-   0        0        0     2616 2023-04-16 18:59:18.000000 sunnyday-IZPy-2.0.0/sunnyday_IZPy/sunnyday.py
+drwxrwxrwx   0        0        0        0 2023-04-16 19:07:12.281153 sunnyday-IZPy-2.0.0/sunnyday_IZPy.egg-info/
+-rw-rw-rw-   0        0        0      387 2023-04-16 19:07:12.000000 sunnyday-IZPy-2.0.0/sunnyday_IZPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-04-16 19:07:12.000000 sunnyday-IZPy-2.0.0/sunnyday_IZPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 19:07:12.000000 sunnyday-IZPy-2.0.0/sunnyday_IZPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-16 19:07:12.000000 sunnyday-IZPy-2.0.0/sunnyday_IZPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-16 19:07:12.000000 sunnyday-IZPy-2.0.0/sunnyday_IZPy.egg-info/top_level.txt
```

### Comparing `sunnyday-IZPy-1.0.0/sunnyday_IZPy/sunnyday.py` & `sunnyday-IZPy-2.0.0/sunnyday_IZPy/sunnyday.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,14 +21,17 @@
     >>> weather2 = Weather(apiKey='30327208ce508bd9097832f10c756ab9', lat=41.1, lon=-4.1)
 
     ## Get complete weather data for the next 12 hours
     >>> weather1.next_12h()
 
     ## Simplified data for the next 12 hours
     >>> weather1.next_12h_simplified()
+
+    Sample url to get sky condition icons:
+    https://openweathermap.org/img/wn/10d@2x.png
     """
 
     def __init__(self, apiKey, city=None, lat=None, lon=None):
 
         if city:
             url = f"http://api.openweathermap.org/data/2.5/forecast?q={city}&appid={apiKey}&units=metric"
             r = requests.get(url)
@@ -57,11 +60,17 @@
         """
         simple_data = []
         for d in self.next_12h():
             simple_data.append(
                 (
                     d["dt_txt"],
                     f'{d["main"]["temp"]} °C',
-                    d["weather"][0]["description"].capitalize()
+                    d["weather"][0]["description"].capitalize(),
+                    d["weather"][0]["icon"]
                 )
             )
         return simple_data
+
+
+w = Weather("30327208ce508bd9097832f10c756ab9", 'Zagreb')
+
+print(w.next_12h_simplified())
```

