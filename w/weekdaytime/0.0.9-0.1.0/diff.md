# Comparing `tmp/weekdaytime-0.0.9.tar.gz` & `tmp/weekdaytime-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\weekdaytime-0.0.9.tar", last modified: Mon Apr 10 10:57:09 2023, max compression
+gzip compressed data, was "dist\weekdaytime-0.1.0.tar", last modified: Sun Apr 16 14:07:03 2023, max compression
```

## Comparing `weekdaytime-0.0.9.tar` & `weekdaytime-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 10:57:09.000000 weekdaytime-0.0.9/
--rw-rw-rw-   0        0        0     1091 2023-04-05 09:07:45.000000 weekdaytime-0.0.9/LICENSE
--rw-rw-rw-   0        0        0       34 2023-04-10 10:38:24.000000 weekdaytime-0.0.9/MANIFEST.in
--rw-rw-rw-   0        0        0     5018 2023-04-10 10:57:09.000000 weekdaytime-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     4689 2023-04-10 10:50:15.000000 weekdaytime-0.0.9/README.md
--rw-rw-rw-   0        0        0      148 2023-04-10 10:57:09.000000 weekdaytime-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      515 2023-04-10 10:50:49.000000 weekdaytime-0.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-10 10:57:09.000000 weekdaytime-0.0.9/weekdaytime/
--rw-rw-rw-   0        0        0     7096 2023-04-10 09:20:43.000000 weekdaytime-0.0.9/weekdaytime/period.py
--rw-rw-rw-   0        0        0     2345 2023-04-08 14:41:13.000000 weekdaytime-0.0.9/weekdaytime/weekdaytime.py
--rw-rw-rw-   0        0        0       89 2023-04-10 10:50:53.000000 weekdaytime-0.0.9/weekdaytime/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 10:57:09.000000 weekdaytime-0.0.9/weekdaytime.egg-info/
--rw-rw-rw-   0        0        0        1 2023-04-10 10:57:09.000000 weekdaytime-0.0.9/weekdaytime.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-10 10:57:09.000000 weekdaytime-0.0.9/weekdaytime.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     5018 2023-04-10 10:57:09.000000 weekdaytime-0.0.9/weekdaytime.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-04-10 10:57:09.000000 weekdaytime-0.0.9/weekdaytime.egg-info/requires.txt
--rw-rw-rw-   0        0        0      329 2023-04-10 10:57:09.000000 weekdaytime-0.0.9/weekdaytime.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       12 2023-04-10 10:57:09.000000 weekdaytime-0.0.9/weekdaytime.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 14:07:03.000000 weekdaytime-0.1.0/
+-rw-rw-rw-   0        0        0     1091 2023-04-05 09:07:45.000000 weekdaytime-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-04-10 10:38:24.000000 weekdaytime-0.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     6261 2023-04-16 14:07:03.000000 weekdaytime-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5932 2023-04-16 14:04:54.000000 weekdaytime-0.1.0/README.md
+-rw-rw-rw-   0        0        0      148 2023-04-16 14:07:03.000000 weekdaytime-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      515 2023-04-16 13:54:25.000000 weekdaytime-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 14:07:03.000000 weekdaytime-0.1.0/weekdaytime/
+-rw-rw-rw-   0        0        0     8883 2023-04-16 04:50:24.000000 weekdaytime-0.1.0/weekdaytime/period.py
+-rw-rw-rw-   0        0        0     2345 2023-04-08 14:41:13.000000 weekdaytime-0.1.0/weekdaytime/weekdaytime.py
+-rw-rw-rw-   0        0        0       89 2023-04-16 13:54:03.000000 weekdaytime-0.1.0/weekdaytime/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 14:07:03.000000 weekdaytime-0.1.0/weekdaytime.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-04-16 14:07:03.000000 weekdaytime-0.1.0/weekdaytime.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-10 10:57:09.000000 weekdaytime-0.1.0/weekdaytime.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     6261 2023-04-16 14:07:03.000000 weekdaytime-0.1.0/weekdaytime.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2023-04-16 14:07:03.000000 weekdaytime-0.1.0/weekdaytime.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      329 2023-04-16 14:07:03.000000 weekdaytime-0.1.0/weekdaytime.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       12 2023-04-16 14:07:03.000000 weekdaytime-0.1.0/weekdaytime.egg-info/top_level.txt
```

### Comparing `weekdaytime-0.0.9/LICENSE` & `weekdaytime-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `weekdaytime-0.0.9/PKG-INFO` & `weekdaytime-0.1.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,27 @@
-Metadata-Version: 2.1
-Name: weekdaytime
-Version: 0.0.9
-Summary: Python library that models available periods in a week
-Home-page: https://github.com/AaronTHCheung/weekdaytime
-Author: Aaron Cheung
-License: MIT
-Platform: UNKNOWN
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # weekdaytime: modelling availability within a week
 This library includes Python classes for modelling available periods within a week.
 
 ## Key features
 - Simple checking of whether visiting period is within an available period. The expression
     ```
     visit_period in available_period
     ```
     evaluates to True if and only if ```visit_period``` is within ```available_period```.
 - Manipulate period objects with bitwise operators (```|, &, ~, ^```)
 - Convert period string into a period object, and vise versa (e.g., `'09:00~15:00,17:00~21:00;15:00~02:00(Fri,Sat)'`)
+- (*New in version 0.1.0*) A period can be instantiated with JSON dictionary obtained as the ```opening_hours/periods``` field in a Google Maps Places (Details) API response (https://developers.google.com/maps/documentation/places/web-service/details#PlaceOpeningHours)
 
 ## Installation
 1. Python version must not be less than 3.6.
 2. The dependent library `bitarray` requires Microsoft Visual C++ 14.0. Get it with "Microsoft Visual C++ Build Tools": https://visualstudio.microsoft.com/downloads/
-3. 
-    - Install with pip using the command
-        ```
-        pip install weekdaytime
-        ```
-    - Alternatively, the library can also be installed with anaconda using the command
-        ```
-        conda install weekdaytime
-        ```
+3. Install with pip using the command
+    ```
+    pip install weekdaytime
+    ```
 
 ## Usage
 ### weekdaytime class
 A weekdaytime instance specifies a point in time in a week.
 ```
 from weekdaytime import weekdaytime as wdt
 
@@ -136,7 +120,28 @@
 
 # Specifying all opening weekdays, the effect is the same
 avail_string = '09:00~15:00,17:00~21:00(Mon,Tue,Thu);12:00~02:00(Fri,Sat);09:00~21:00(Sun)'
 p = period.strpperiod(avail_string)
 print(p)  # '09:00~15:00,17:00~21:00(Mon,Tue,Thu);00:00~02:00,09:00~21:00(Sun);12:00~24:00(Fri);00:00~02:00,12:00~24:00(Sat)'
 ```
 
+---
+*New in version 0.1.0*
+
+A period can be instantiated with JSON dictionary obtained as the ```opening_hours/periods``` field in a Google Maps Places (Details) API response (https://developers.google.com/maps/documentation/places/web-service/details#PlaceOpeningHours)
+```
+from weekdaytime import period
+
+gperiods1 = [{'open': {'day': 0, 'time': '0000'}}]
+gperiods2 = [{'close': {'day': 1, 'time': '2100'}, 'open': {'day': 1, 'time': '0900'}}, 
+             {'close': {'day': 2, 'time': '2100'}, 'open': {'day': 2, 'time': '0900'}}, 
+             {'close': {'day': 3, 'time': '2100'}, 'open': {'day': 3, 'time': '0900'}}, 
+             {'close': {'day': 4, 'time': '2100'}, 'open': {'day': 4, 'time': '0900'}}, 
+             {'close': {'day': 5, 'time': '2100'}, 'open': {'day': 5, 'time': '0900'}}, 
+             {'close': {'day': 6, 'time': '1800'}, 'open': {'day': 6, 'time': '0900'}}]
+
+p1 = period.from_googlemaps_periods(gperiods1)
+p2 = period.from_googlemaps_periods(gperiods2)
+
+print(p1)    # '00:00~24:00(Sun,Mon,Tue,Wed,Thu,Fri,Sat)'
+print(p2)    # '09:00~21:00(Mon,Tue,Wed,Thu,Fri);09:00~18:00(Sat)'
+```
```

### Comparing `weekdaytime-0.0.9/setup.py` & `weekdaytime-0.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 from pathlib import Path
 
 long_description = (Path(__file__).parent/'README.md').read_text()
 setup(
     name='weekdaytime',
-    version='0.0.9',
+    version='0.1.0',
     description='Python library that models available periods in a week',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Aaron Cheung',
     packages=['weekdaytime'],
     python_requires='>=3.6',
     install_requires=[
```

### Comparing `weekdaytime-0.0.9/weekdaytime/period.py` & `weekdaytime-0.1.0/weekdaytime/period.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from bitarray import bitarray, frozenbitarray
 from bitarray.util import intervals
 import re
 from weekdaytime import weekdaytime
 from itertools import combinations
+from typing import List,Dict
 
 class period():
     def __init__(self, *args: weekdaytime):
         '''
         args is [start1_weekdaytime, end1_weekdaytime, start2_weekdaytime, end2_weekdaytime, ... ]
         '''
 
@@ -30,22 +31,62 @@
         if isinstance(ba, bitarray) and len(ba.unpack()) == 60*24*7:
             p = period()
             p._fba = frozenbitarray(ba)
             return p
         else:
             raise Exception('argument is not a valid bitarray instance with size 60*24*7')
         
+    # New in version 0.1.0
+    @staticmethod
+    def from_googlemaps_periods(gperiods: List[Dict]):
+        mows = []
+        open_predicates = []
+        for gperiod in gperiods:
+            for k,v in gperiod.items():
+                weekday = v['day']
+                hour = int(v['time'][:2])
+                minute = int(v['time'][2:])
+                mows.append(weekday*24*60 + hour*60 + minute)
+                open_predicates.append(True if k=='open' else False)
+
+        ba = bitarray(60*24*7)        
+        # check if even number of mows, if not then the resulting period is available 24/7
+        if len(mows) % 2 != 0:
+            ba.setall(1)
+            return period.from_bitarray(ba)
+        
+        ba.setall(0)
+        sort_idxs = [i[0] for i in sorted(enumerate(mows), key=lambda x: x[1])]
+        for i in range(len(mows)//2):
+            idx_open  = sort_idxs[2*i]
+            idx_close = sort_idxs[2*i+1]
+            open_predicate_open = open_predicates[idx_open]
+            open_predicate_close = open_predicates[idx_close]
+
+            if open_predicate_open == True and open_predicate_close == False:
+                # open close check passed, fill ba
+                mow_open = mows[idx_open]
+                mow_close = mows[idx_close]
+                ba |= period(weekdaytime.from_min_of_week(mow_open),
+                             weekdaytime.from_min_of_week(mow_close))._fba
+            else:
+                # some opens have no closes
+                raise Exception('Invalid input google maps api response periods')
+
+        return period.from_bitarray(ba)
+        
+
     @staticmethod
     def strpperiod(string: str):
         # string example: 09:00~15:00,17:00~20:00;14:00~02:00(Fri);12:00~20:00(Sat,Sun)
         ba = bitarray(60*24*7)
         ba.setall(0)
 
         generic_string = ''
-        m = re.search(';|^([0-9:~,]+);|$', string)
+        m = re.search(';|^([0-9:~,]+)(;|$)', string)
         if m.group(0) != '' and m.groups()[0] is not None:
             # there is a weekday-generic part
             generic_string = m.group(1)
             specific_string = string[:m.span()[0]] + ';' + string[m.span()[1]:]
         else:
             # all parts are weekday-specific
             specific_string = string
@@ -64,20 +105,23 @@
                 end_minute_of_day = end_hour * 60 + end_minute
                 if end_minute_of_day < start_minute_of_day: end_minute_of_day += 60 * 24  # across midnight
 
                 starts_minute_of_day.append(start_minute_of_day)
                 ends_minute_of_day.append(end_minute_of_day)
                 
             for weekdayAbbrev in weekdayAbbrev_string.split(','):
-                start_weekday = weekdaytime.intfweekday(weekdayAbbrev)
-                specific_predicates[start_weekday] = 1
-                for s, e in zip(starts_minute_of_day, ends_minute_of_day):
-                    start_weekdaytime = weekdaytime.from_min_of_week(start_weekday * 24 * 60 + s)
-                    end_weekdaytime = weekdaytime.from_min_of_week(start_weekday * 24 * 60 + e)
-                    ba |= period(start_weekdaytime, end_weekdaytime)._fba
+                try:
+                    start_weekday = weekdaytime.intfweekday(weekdayAbbrev)
+                    specific_predicates[start_weekday] = 1
+                    for s, e in zip(starts_minute_of_day, ends_minute_of_day):
+                        start_weekdaytime = weekdaytime.from_min_of_week(start_weekday * 24 * 60 + s)
+                        end_weekdaytime = weekdaytime.from_min_of_week(start_weekday * 24 * 60 + e)
+                        ba |= period(start_weekdaytime, end_weekdaytime)._fba
+                except Exception:
+                    pass
 
         # remaining days are filled with weekday-generic information
         for time_substring in generic_string.split(','):
             if len(time_substring) != 11: continue
             start_hour, start_minute, end_hour, end_minute = [int(x) for x in re.split(':|~', time_substring)]
 
             start_minute_of_day = start_hour * 60 + start_minute
```

### Comparing `weekdaytime-0.0.9/weekdaytime/weekdaytime.py` & `weekdaytime-0.1.0/weekdaytime/weekdaytime.py`

 * *Files identical despite different names*

### Comparing `weekdaytime-0.0.9/weekdaytime.egg-info/PKG-INFO` & `weekdaytime-0.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weekdaytime
-Version: 0.0.9
+Version: 0.1.0
 Summary: Python library that models available periods in a week
 Home-page: https://github.com/AaronTHCheung/weekdaytime
 Author: Aaron Cheung
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -17,27 +17,23 @@
 - Simple checking of whether visiting period is within an available period. The expression
     ```
     visit_period in available_period
     ```
     evaluates to True if and only if ```visit_period``` is within ```available_period```.
 - Manipulate period objects with bitwise operators (```|, &, ~, ^```)
 - Convert period string into a period object, and vise versa (e.g., `'09:00~15:00,17:00~21:00;15:00~02:00(Fri,Sat)'`)
+- (*New in version 0.1.0*) A period can be instantiated with JSON dictionary obtained as the ```opening_hours/periods``` field in a Google Maps Places (Details) API response (https://developers.google.com/maps/documentation/places/web-service/details#PlaceOpeningHours)
 
 ## Installation
 1. Python version must not be less than 3.6.
 2. The dependent library `bitarray` requires Microsoft Visual C++ 14.0. Get it with "Microsoft Visual C++ Build Tools": https://visualstudio.microsoft.com/downloads/
-3. 
-    - Install with pip using the command
-        ```
-        pip install weekdaytime
-        ```
-    - Alternatively, the library can also be installed with anaconda using the command
-        ```
-        conda install weekdaytime
-        ```
+3. Install with pip using the command
+    ```
+    pip install weekdaytime
+    ```
 
 ## Usage
 ### weekdaytime class
 A weekdaytime instance specifies a point in time in a week.
 ```
 from weekdaytime import weekdaytime as wdt
 
@@ -136,7 +132,30 @@
 
 # Specifying all opening weekdays, the effect is the same
 avail_string = '09:00~15:00,17:00~21:00(Mon,Tue,Thu);12:00~02:00(Fri,Sat);09:00~21:00(Sun)'
 p = period.strpperiod(avail_string)
 print(p)  # '09:00~15:00,17:00~21:00(Mon,Tue,Thu);00:00~02:00,09:00~21:00(Sun);12:00~24:00(Fri);00:00~02:00,12:00~24:00(Sat)'
 ```
 
+---
+*New in version 0.1.0*
+
+A period can be instantiated with JSON dictionary obtained as the ```opening_hours/periods``` field in a Google Maps Places (Details) API response (https://developers.google.com/maps/documentation/places/web-service/details#PlaceOpeningHours)
+```
+from weekdaytime import period
+
+gperiods1 = [{'open': {'day': 0, 'time': '0000'}}]
+gperiods2 = [{'close': {'day': 1, 'time': '2100'}, 'open': {'day': 1, 'time': '0900'}}, 
+             {'close': {'day': 2, 'time': '2100'}, 'open': {'day': 2, 'time': '0900'}}, 
+             {'close': {'day': 3, 'time': '2100'}, 'open': {'day': 3, 'time': '0900'}}, 
+             {'close': {'day': 4, 'time': '2100'}, 'open': {'day': 4, 'time': '0900'}}, 
+             {'close': {'day': 5, 'time': '2100'}, 'open': {'day': 5, 'time': '0900'}}, 
+             {'close': {'day': 6, 'time': '1800'}, 'open': {'day': 6, 'time': '0900'}}]
+
+p1 = period.from_googlemaps_periods(gperiods1)
+p2 = period.from_googlemaps_periods(gperiods2)
+
+print(p1)    # '00:00~24:00(Sun,Mon,Tue,Wed,Thu,Fri,Sat)'
+print(p2)    # '09:00~21:00(Mon,Tue,Wed,Thu,Fri);09:00~18:00(Sat)'
+```
+
+
```

