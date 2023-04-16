# Comparing `tmp/pandasflow-0.1.6.tar.gz` & `tmp/pandasflow-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasflow-0.1.6.tar", last modified: Sun Apr 16 10:15:39 2023, max compression
+gzip compressed data, was "pandasflow-0.1.7.tar", last modified: Sun Apr 16 13:34:06 2023, max compression
```

## Comparing `pandasflow-0.1.6.tar` & `pandasflow-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 10:15:39.415896 pandasflow-0.1.6/
--rw-rw-rw-   0        0        0    35823 2023-04-09 14:36:14.000000 pandasflow-0.1.6/LICENCE
--rw-rw-rw-   0        0        0      670 2023-04-16 10:15:39.415896 pandasflow-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      221 2023-04-16 10:15:23.000000 pandasflow-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-16 10:15:39.413004 pandasflow-0.1.6/pandasflow/
--rw-rw-rw-   0        0        0      258 2023-04-16 10:15:32.000000 pandasflow-0.1.6/pandasflow/__init__.py
--rw-rw-rw-   0        0        0      395 2023-04-15 15:57:08.000000 pandasflow-0.1.6/pandasflow/get_import.py
--rw-rw-rw-   0        0        0      217 2023-04-14 13:37:47.000000 pandasflow-0.1.6/pandasflow/mean_error.py
--rw-rw-rw-   0        0        0      614 2023-04-13 15:00:40.000000 pandasflow-0.1.6/pandasflow/reset_mi.py
--rw-rw-rw-   0        0        0     2691 2023-04-16 10:02:05.000000 pandasflow-0.1.6/pandasflow/train_valid_test_split.py
-drwxrwxrwx   0        0        0        0 2023-04-16 10:15:39.414998 pandasflow-0.1.6/pandasflow.egg-info/
--rw-rw-rw-   0        0        0      670 2023-04-16 10:15:39.000000 pandasflow-0.1.6/pandasflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2023-04-16 10:15:39.000000 pandasflow-0.1.6/pandasflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 10:15:39.000000 pandasflow-0.1.6/pandasflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-16 10:15:39.000000 pandasflow-0.1.6/pandasflow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 10:15:39.416587 pandasflow-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      712 2023-04-16 09:52:13.000000 pandasflow-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:34:06.169701 pandasflow-0.1.7/
+-rw-rw-rw-   0        0        0    35823 2023-04-09 14:36:14.000000 pandasflow-0.1.7/LICENCE
+-rw-rw-rw-   0        0        0      694 2023-04-16 13:34:06.169701 pandasflow-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2023-04-16 10:16:48.000000 pandasflow-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-16 13:34:06.165658 pandasflow-0.1.7/pandasflow/
+-rw-rw-rw-   0        0        0      343 2023-04-16 13:32:33.000000 pandasflow-0.1.7/pandasflow/__init__.py
+-rw-rw-rw-   0        0        0      395 2023-04-15 15:57:08.000000 pandasflow-0.1.7/pandasflow/get_import.py
+-rw-rw-rw-   0        0        0      217 2023-04-14 13:37:47.000000 pandasflow-0.1.7/pandasflow/mean_error.py
+-rw-rw-rw-   0        0        0      614 2023-04-13 15:00:40.000000 pandasflow-0.1.7/pandasflow/reset_mi.py
+-rw-rw-rw-   0        0        0     2690 2023-04-16 13:29:59.000000 pandasflow-0.1.7/pandasflow/train_test_split.py
+-rw-rw-rw-   0        0        0     2936 2023-04-16 13:25:55.000000 pandasflow-0.1.7/pandasflow/train_valid_test_split.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:34:06.168738 pandasflow-0.1.7/pandasflow.egg-info/
+-rw-rw-rw-   0        0        0      694 2023-04-16 13:34:06.000000 pandasflow-0.1.7/pandasflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      369 2023-04-16 13:34:06.000000 pandasflow-0.1.7/pandasflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 13:34:06.000000 pandasflow-0.1.7/pandasflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-04-16 13:34:06.000000 pandasflow-0.1.7/pandasflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-16 13:34:06.000000 pandasflow-0.1.7/pandasflow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 13:34:06.169701 pandasflow-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      736 2023-04-16 13:33:39.000000 pandasflow-0.1.7/setup.py
```

### Comparing `pandasflow-0.1.6/LICENCE` & `pandasflow-0.1.7/LICENCE`

 * *Files identical despite different names*

### Comparing `pandasflow-0.1.6/pandasflow/reset_mi.py` & `pandasflow-0.1.7/pandasflow/reset_mi.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.1.6/pandasflow/train_valid_test_split.py` & `pandasflow-0.1.7/pandasflow/train_valid_test_split.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import pandas as pd
 from sklearn.model_selection import train_test_split
 
 def train_valid_test_split(
 	*arrays,
 	test_size=None,
 	train_size=0.6,
 	random_state=42,
@@ -50,28 +51,32 @@
 	valid, test = train_test_split(valid_test, test_size=test_size_pice, random_state=random_state, shuffle=shuffle, stratify=stratify)
 	
 	train_pie = len(train) / len(arrays[0])
 	valid_pie = len(valid) / len(arrays[0])
 	test_pie = len(test) / len(arrays[0])
 	
 	amount_len = len(train) + len(valid) + len(test)
+	amount_prop = amount_len / len(arrays[0])
 	
 	if round_ not in [None, 'n', 'N'] and round_ > 0:
 		train_pie = round(train_pie, round_)
 		valid_pie = round(valid_pie, round_)
 		test_pie = round(test_pie, round_)
 	
-	
-	print(f'''
-train:	{len(train)},	{train_pie}
-valid:	{len(valid)},	{valid_pie}
-test:	{len(test)},	{test_pie}
----
-IniData	{len(arrays[0])}
-Amount	{amount_len}, {amount_len / len(arrays[0])}
-'''[1:-1])
+	table = pd.DataFrame({
+		#count
+		' ': [len(train), len(valid), len(test), '', amount_len, len(arrays[0])],
+		#proportion
+		'  ': [train_pie, valid_pie, test_pie, '', amount_prop, '']})
+	
+	table.index = ['train', 'valid', 'test', '---', 'Amount', 'InitData']
+	print(table)
+	
+	if amount_prop != 1.0 or len(arrays[0]) != amount_len:
+		print('---')
+		print('Some data is droped')
 	
 	return train, valid, test
 
 
 if __name__ == "__main__":
 	train, valid, test = train_valid_test_split([0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10] * 3, round_=2)
```

### Comparing `pandasflow-0.1.6/setup.py` & `pandasflow-0.1.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 setup(
     name="pandasflow",
     version=pandasflow.__version__,
     author="Priboy313",
     author_email="Priboy313@yandex.ru",
-    description="Module for friendly workflow on pandas",
+    description="A set of custom python modules for friendly workflow on pandas",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/Priboy313/pandasflow",
     packages=find_packages(),
     install_requires=pandasflow.requirements,
     classifiers=[
         "Programming Language :: Python :: 3.10",
```

