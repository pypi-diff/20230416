# Comparing `tmp/pandasflow-0.1.5.tar.gz` & `tmp/pandasflow-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasflow-0.1.5.tar", last modified: Sun Apr 16 09:57:43 2023, max compression
+gzip compressed data, was "pandasflow-0.1.6.tar", last modified: Sun Apr 16 10:15:39 2023, max compression
```

## Comparing `pandasflow-0.1.5.tar` & `pandasflow-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 09:57:43.155625 pandasflow-0.1.5/
--rw-rw-rw-   0        0        0    35823 2023-04-09 14:36:14.000000 pandasflow-0.1.5/LICENCE
--rw-rw-rw-   0        0        0      755 2023-04-16 09:57:43.155625 pandasflow-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-04-15 18:28:12.000000 pandasflow-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-16 09:57:43.152639 pandasflow-0.1.5/pandasflow/
--rw-rw-rw-   0        0        0      258 2023-04-16 09:57:39.000000 pandasflow-0.1.5/pandasflow/__init__.py
--rw-rw-rw-   0        0        0      395 2023-04-15 15:57:08.000000 pandasflow-0.1.5/pandasflow/get_import.py
--rw-rw-rw-   0        0        0      217 2023-04-14 13:37:47.000000 pandasflow-0.1.5/pandasflow/mean_error.py
--rw-rw-rw-   0        0        0      614 2023-04-13 15:00:40.000000 pandasflow-0.1.5/pandasflow/reset_mi.py
--rw-rw-rw-   0        0        0     2699 2023-04-16 09:55:37.000000 pandasflow-0.1.5/pandasflow/train_valid_test_split.py
-drwxrwxrwx   0        0        0        0 2023-04-16 09:57:43.154627 pandasflow-0.1.5/pandasflow.egg-info/
--rw-rw-rw-   0        0        0      755 2023-04-16 09:57:43.000000 pandasflow-0.1.5/pandasflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2023-04-16 09:57:43.000000 pandasflow-0.1.5/pandasflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 09:57:43.000000 pandasflow-0.1.5/pandasflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-16 09:57:43.000000 pandasflow-0.1.5/pandasflow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 09:57:43.156638 pandasflow-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      712 2023-04-16 09:52:13.000000 pandasflow-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 10:15:39.415896 pandasflow-0.1.6/
+-rw-rw-rw-   0        0        0    35823 2023-04-09 14:36:14.000000 pandasflow-0.1.6/LICENCE
+-rw-rw-rw-   0        0        0      670 2023-04-16 10:15:39.415896 pandasflow-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2023-04-16 10:15:23.000000 pandasflow-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-16 10:15:39.413004 pandasflow-0.1.6/pandasflow/
+-rw-rw-rw-   0        0        0      258 2023-04-16 10:15:32.000000 pandasflow-0.1.6/pandasflow/__init__.py
+-rw-rw-rw-   0        0        0      395 2023-04-15 15:57:08.000000 pandasflow-0.1.6/pandasflow/get_import.py
+-rw-rw-rw-   0        0        0      217 2023-04-14 13:37:47.000000 pandasflow-0.1.6/pandasflow/mean_error.py
+-rw-rw-rw-   0        0        0      614 2023-04-13 15:00:40.000000 pandasflow-0.1.6/pandasflow/reset_mi.py
+-rw-rw-rw-   0        0        0     2691 2023-04-16 10:02:05.000000 pandasflow-0.1.6/pandasflow/train_valid_test_split.py
+drwxrwxrwx   0        0        0        0 2023-04-16 10:15:39.414998 pandasflow-0.1.6/pandasflow.egg-info/
+-rw-rw-rw-   0        0        0      670 2023-04-16 10:15:39.000000 pandasflow-0.1.6/pandasflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2023-04-16 10:15:39.000000 pandasflow-0.1.6/pandasflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 10:15:39.000000 pandasflow-0.1.6/pandasflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-16 10:15:39.000000 pandasflow-0.1.6/pandasflow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 10:15:39.416587 pandasflow-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      712 2023-04-16 09:52:13.000000 pandasflow-0.1.6/setup.py
```

### Comparing `pandasflow-0.1.5/LICENCE` & `pandasflow-0.1.6/LICENCE`

 * *Files identical despite different names*

### Comparing `pandasflow-0.1.5/pandasflow/reset_mi.py` & `pandasflow-0.1.6/pandasflow/reset_mi.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.1.5/pandasflow/train_valid_test_split.py` & `pandasflow-0.1.6/pandasflow/train_valid_test_split.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 	
 	print(f'''
 train:	{len(train)},	{train_pie}
 valid:	{len(valid)},	{valid_pie}
 test:	{len(test)},	{test_pie}
 ---
 IniData	{len(arrays[0])}
-Amount	{len(train) + len(valid) + len(test)}, {amount_len}
+Amount	{amount_len}, {amount_len / len(arrays[0])}
 '''[1:-1])
 	
 	return train, valid, test
 
 
 if __name__ == "__main__":
 	train, valid, test = train_valid_test_split([0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10] * 3, round_=2)
```

### Comparing `pandasflow-0.1.5/setup.py` & `pandasflow-0.1.6/setup.py`

 * *Files identical despite different names*

