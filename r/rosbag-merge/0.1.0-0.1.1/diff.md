# Comparing `tmp/rosbag_merge-0.1.0.tar.gz` & `tmp/rosbag_merge-0.1.1.tar.gz`

## Comparing `rosbag_merge-0.1.0.tar` & `rosbag_merge-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 rosbag_merge-0.1.0/INSTALL.md
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 rosbag_merge-0.1.0/requirements.txt
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 rosbag_merge-0.1.0/.github/workflows/publish-to-pypi-and-test-pypi.yml
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 rosbag_merge-0.1.0/examples/main_direct.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 rosbag_merge-0.1.0/src/rosbag_merge/__init__.py
--rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 rosbag_merge-0.1.0/src/rosbag_merge/bag_stream.py
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 rosbag_merge-0.1.0/src/rosbag_merge/csv_merge.py
--rwxr-xr-x   0        0        0     6382 2020-02-02 00:00:00.000000 rosbag_merge-0.1.0/src/rosbag_merge/main.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 rosbag_merge-0.1.0/src/rosbag_merge/merge_bags.py
--rw-r--r--   0        0        0    10427 2020-02-02 00:00:00.000000 rosbag_merge-0.1.0/src/rosbag_merge/rosbag_to_csv.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 rosbag_merge-0.1.0/tests/topic_list.txt
--rw-r--r--   0        0        0    20625 2020-02-02 00:00:00.000000 rosbag_merge-0.1.0/tests/data/raw/TB3_WAFFLE_SLAM_cmd_vel_only.bag
--rw-r--r--   0        0        0   331893 2020-02-02 00:00:00.000000 rosbag_merge-0.1.0/tests/data/raw/TB3_WAFFLE_SLAM_imu_only.bag
--rw-r--r--   0        0        0   121303 2020-02-02 00:00:00.000000 rosbag_merge-0.1.0/tests/data/raw/TB3_WAFFLE_SLAM_odom_tf_static.bag
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 rosbag_merge-0.1.0/.gitignore
--rw-r--r--   0        0        0    10762 2020-02-02 00:00:00.000000 rosbag_merge-0.1.0/LICENSE
--rw-r--r--   0        0        0     2931 2020-02-02 00:00:00.000000 rosbag_merge-0.1.0/README.md
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 rosbag_merge-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    16050 2020-02-02 00:00:00.000000 rosbag_merge-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 rosbag_merge-0.1.1/INSTALL.md
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 rosbag_merge-0.1.1/requirements.txt
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 rosbag_merge-0.1.1/.github/workflows/publish-to-pypi-and-test-pypi.yml
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 rosbag_merge-0.1.1/examples/main_direct.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 rosbag_merge-0.1.1/src/rosbag_merge/__init__.py
+-rw-r--r--   0        0        0     3669 2020-02-02 00:00:00.000000 rosbag_merge-0.1.1/src/rosbag_merge/bag_stream.py
+-rwxr-xr-x   0        0        0     4875 2020-02-02 00:00:00.000000 rosbag_merge-0.1.1/src/rosbag_merge/main.py
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 rosbag_merge-0.1.1/src/rosbag_merge/deprecated/csv_merge.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 rosbag_merge-0.1.1/src/rosbag_merge/deprecated/merge_bags.py
+-rw-r--r--   0        0        0    10427 2020-02-02 00:00:00.000000 rosbag_merge-0.1.1/src/rosbag_merge/deprecated/rosbag_to_csv.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 rosbag_merge-0.1.1/tests/topic_list.txt
+-rw-r--r--   0        0        0    20625 2020-02-02 00:00:00.000000 rosbag_merge-0.1.1/tests/data/raw/TB3_WAFFLE_SLAM_cmd_vel_only.bag
+-rw-r--r--   0        0        0   331893 2020-02-02 00:00:00.000000 rosbag_merge-0.1.1/tests/data/raw/TB3_WAFFLE_SLAM_imu_only.bag
+-rw-r--r--   0        0        0   121303 2020-02-02 00:00:00.000000 rosbag_merge-0.1.1/tests/data/raw/TB3_WAFFLE_SLAM_odom_tf_static.bag
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 rosbag_merge-0.1.1/.gitignore
+-rw-r--r--   0        0        0    10762 2020-02-02 00:00:00.000000 rosbag_merge-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 rosbag_merge-0.1.1/README.md
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 rosbag_merge-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    14969 2020-02-02 00:00:00.000000 rosbag_merge-0.1.1/PKG-INFO
```

### Comparing `rosbag_merge-0.1.0/.github/workflows/publish-to-pypi-and-test-pypi.yml` & `rosbag_merge-0.1.1/.github/workflows/publish-to-pypi-and-test-pypi.yml`

 * *Files identical despite different names*

### Comparing `rosbag_merge-0.1.0/src/rosbag_merge/csv_merge.py` & `rosbag_merge-0.1.1/src/rosbag_merge/deprecated/csv_merge.py`

 * *Files identical despite different names*

### Comparing `rosbag_merge-0.1.0/src/rosbag_merge/main.py` & `rosbag_merge-0.1.1/src/rosbag_merge/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 #! /usr/bin/env python3
-from . import bag_stream
-from . import csv_merge
 import argparse
 
+from . import bag_stream
 import os
 import sys
 import glob 
 
 from icecream import ic
 ic.configureOutput(includeContext=True)
 
@@ -15,22 +14,14 @@
 
 """
 
 def refine_args(args:argparse.Namespace)-> argparse.Namespace:
     # Refine the arguments to handle simplified inputs such as directories, files with lists of topics, etc.
     retval = args
 
-    # Handle default arguments
-    if "merge_csvs" not in args:
-        args.merge_csvs = False
-    if "write_csvs" not in args:
-        args.write_csvs = False
-    if "write_bag" not in args:
-        args.write_bag = False
-
     # make sequence of topics from a topic file
     if args.topic_file :
         if ("topics" not in args) or (not args.topics):
             args.topics = []
         with open(args.topic_file) as f:
             lines = [line.strip() for line in f]
         args.topics.extend(lines)
@@ -48,29 +39,24 @@
                     if "input_bags" not in args:
                         args.input_bags = []
                     args.input_bags.append(full_file_path)
     # TODO, if outpath, then join outpath with out file paths, must also do with the csv writer
     no_outbag_actions = (not args.outbag_name) and (args.write_bag) 
     if (no_outbag_actions):
         ic("Writing bags requires an outbag suffix.")
-    no_input_files = (("input_bags" not in args) or (not len(args.input_bags))) and (("input_csvs" not in args) or (not len(args.input_csvs)))
+    no_input_files = (("input_bags" not in args) or (not len(args.input_bags)))
     args.write_bag = True if args.output_path and args.outbag_name else False
     requesting_write_without_output_path =  not args.output_path and (args.merge_csvs or args.write_csvs or args.write_bag)
-    no_csvs_to_merge = (("input_csvs" not in args) or not (len(args.input_csvs) or args.write_csvs)) and args.merge_csvs
-    if (no_csvs_to_merge):
-        ic("unable to merge non-existent (present tense and future) csvs.")
-    if (no_outbag_actions or no_input_files or requesting_write_without_output_path or no_csvs_to_merge):
+    if (no_outbag_actions or no_input_files or requesting_write_without_output_path):
         if no_outbag_actions : 
             ic(no_outbag_actions)
         if no_input_files : 
             ic(no_input_files)
         if requesting_write_without_output_path : 
             ic(requesting_write_without_output_path)
-        if no_csvs_to_merge : 
-            ic(no_csvs_to_merge)
         
         create_parser().print_help()
         retval = None  # Invalid args, so make it clear
     return retval
 
 
 def create_parser()-> argparse.ArgumentParser:
@@ -85,29 +71,21 @@
     )
     parser.add_argument('--outbag_name', '-obn',
         type=str,
         help='The output bag name ( file to write to )',
         default=None,
     )
     parser.add_argument('--write_bag', action='store_true')
-    parser.add_argument('--write_csvs', action='store_true')
-    parser.add_argument('--merge_csvs', action='store_true')
     # add an argument for the sequence of input bags
     parser.add_argument('--input_bags', '-ib',
         type=str,
         nargs='+',
         help='A list of input bag files. (global paths)',
         default=[],
     )
-    parser.add_argument('--input_csvs', '-ic',
-        type=str,
-        nargs='+',
-        help='A list of input csv files. (global paths)',
-        default=[],
-    )
     parser.add_argument('--input_paths', '-ip',
         type=str,
         nargs='+',
         help='A list of input directories with bag files. (global paths)',
         default="./",
     )
     # add an argument for the topics to filter
@@ -136,29 +114,19 @@
 def main(args:argparse.Namespace=None):
     if not args:
         args = parse_args(sys.argv[1:])
     # Refine arguments here so simplified args can be used.
     args = refine_args(args)
     if args is None:
         return  # Invalid arguments, return
-    if(args.merge_csvs):
-        # TODO , see why can't make csvs and merge in the same call to main
-        expecting_to_merge_newly_written_csvs = args.write_csvs and (not len(args.input_csvs))
-        if(expecting_to_merge_newly_written_csvs):
-            # gather newly made csvs from the output path
-            args.input_csvs.extend(glob.glob(os.path.join(args.output_path,"*-single-topic.csv")))
-            csv_merge.merge_csvs_using_dask(args.input_csvs)
-    else:
-        bag_stream.main(input_bags=args.input_bags 
-                        ,write_bag=args.write_bag
-                        ,write_csvs=args.write_csvs
-                        ,output_path=args.output_path
-                        ,outbag_name=args.outbag_name
-                        ,topics=args.topics
-                        ) 
+    bag_stream.main(input_bags=args.input_bags 
+                    ,output_path=args.output_path
+                    ,outbag_name=args.outbag_name
+                    ,topics=args.topics
+                    ) 
 
 if __name__ == "__main__":
     # Load command line arguments here so that the main function can be called directly from import
     args = parse_args(sys.argv[1:])
     main(args)
 
 # explicitly define the outward facing API of this module (either command line or direct call to the main function)
```

### Comparing `rosbag_merge-0.1.0/src/rosbag_merge/merge_bags.py` & `rosbag_merge-0.1.1/src/rosbag_merge/deprecated/merge_bags.py`

 * *Files identical despite different names*

### Comparing `rosbag_merge-0.1.0/src/rosbag_merge/rosbag_to_csv.py` & `rosbag_merge-0.1.1/src/rosbag_merge/deprecated/rosbag_to_csv.py`

 * *Files identical despite different names*

### Comparing `rosbag_merge-0.1.0/tests/data/raw/TB3_WAFFLE_SLAM_cmd_vel_only.bag` & `rosbag_merge-0.1.1/tests/data/raw/TB3_WAFFLE_SLAM_cmd_vel_only.bag`

 * *Files identical despite different names*

### Comparing `rosbag_merge-0.1.0/tests/data/raw/TB3_WAFFLE_SLAM_imu_only.bag` & `rosbag_merge-0.1.1/tests/data/raw/TB3_WAFFLE_SLAM_imu_only.bag`

 * *Files identical despite different names*

### Comparing `rosbag_merge-0.1.0/tests/data/raw/TB3_WAFFLE_SLAM_odom_tf_static.bag` & `rosbag_merge-0.1.1/tests/data/raw/TB3_WAFFLE_SLAM_odom_tf_static.bag`

 * *Files identical despite different names*

### Comparing `rosbag_merge-0.1.0/LICENSE` & `rosbag_merge-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rosbag_merge-0.1.0/README.md` & `rosbag_merge-0.1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -32,23 +32,14 @@
 
 ```--topics```
 * Topics which should be filtered. Use this to speed up all of the processing. To use all topics then simply omit the flag.
 
 ```--topic-file```
 * Topics which should be filtered. Use this to speed up all of the processing. To use all topics then simply omit the flag. A file representing a list of topics. One topic per line.
 
-```--write_bag```
-* Including the flag tells ```rosbag-tools``` to write a new bag. Be sure to include an ```--outbag-name```.
-
-```--write_csvs```
-* Including the flag tells ```rosbag-tools``` to write a csv's with the topic data of interest.
-
-```--merge_csvs```
-* Takes the csvs in the input path and makes a single csv. The csv will fill topic data such that the new csv fills in data to share the same time and is easier to vizualize on plotjuggler or through matplotlib.
-
 > NOTE : More arguments are available if you want to use specific CSV's or Bag files. Run `rosbag-merge -h` for more information.
 
 ### Some environment variables
 
 ```
 export IN_PATH=/path/to/data
 export OUT_PATH=/path/to/data
@@ -72,27 +63,8 @@
 ```
 rosbag-merge --input_paths $IN_PATH --output_path $OUT_PATH --outbag_name $OUTBAG_NAME --topics $INPUT_TOPICS --write_bag 
 ```
 
 To merge bag files with select topics, and make single topics csvs.
 ```
 rosbag-merge --input_paths $IN_PATH --output_path $OUT_PATH --outbag_name $OUTBAG_NAME --write_bag --write_csvs 
-```
-
-Loop through the bag msgs and make single topics csvs.
-```
-rosbag-merge --input_paths $IN_PATH --output_path $OUT_PATH --outbag_name $OUTBAG_NAME --write_csvs 
-```
-
-Loop through the bag msgs and make single topics csvs.
-```
-rosbag-merge --input_paths $IN_PATH --output_path $OUT_PATH --outbag_name $OUTBAG_NAME --write_csvs 
-```
-
-
-### Merge CSVs
-
-For now, merging csvs must be done **after** making the CSVs on a previous command.
-```
-rosbag-merge --input_paths $IN_PATH --output_path $OUT_PATH  --merge_csvs
-```
-
+```
```

### Comparing `rosbag_merge-0.1.0/pyproject.toml` & `rosbag_merge-0.1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 [project]
 # add the distribution name of the package, the tar ball and python wheel use this name, this name goes the /home/$USER/.local/lib/python3.8/site-packages/
 name = "rosbag_merge"
 
 # version is the package version. See the version specifier specification
 # for more details on versions. Some build backends allow it to be 
 # specified another way, such as from a file or a git tag.
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Jonathan Sanabria", email="jonsanria@gmail.com" },
 ]
 description = "A gathering of tools for merging rosbags and saving their topic information to csv."
 readme = "README.md"
 license = { file="LICENSE" }
 
@@ -34,21 +34,17 @@
     "Intended Audience :: Developers",
     "Intended Audience :: System Administrators",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
-    "rosbag",
-    "rospy",
-    "dask",
-    "pandas",
+    "rosbags",
     "icecream",
     "tqdm",
-    "numpy==1.21" # wait for dask to solve solve AttributeError: module 'numpy' has no attribute 'typeDict'
 ]
 
 # this installs an executable in /home/$USER/.local/bin/rosbag-tools
 [project.scripts]
 rosbag-merge = "rosbag_merge.main:main"
 
 [project.urls]
```

### Comparing `rosbag_merge-0.1.0/PKG-INFO` & `rosbag_merge-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosbag_merge
-Version: 0.1.0
+Version: 0.1.1
 Summary: A gathering of tools for merging rosbags and saving their topic information to csv.
 Project-URL: Homepage, https://github.com/1hada/rosbag-merge/
 Project-URL: Bug Tracker, https://github.com/1hada/rosbag-merge/issues/
 Author-email: Jonathan Sanabria <jonsanria@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -198,20 +198,16 @@
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
-Requires-Dist: dask
 Requires-Dist: icecream
-Requires-Dist: numpy==1.21
-Requires-Dist: pandas
-Requires-Dist: rosbag
-Requires-Dist: rospy
+Requires-Dist: rosbags
 Requires-Dist: tqdm
 Description-Content-Type: text/markdown
 
 
 
 ### Getting Started
 
@@ -245,23 +241,14 @@
 
 ```--topics```
 * Topics which should be filtered. Use this to speed up all of the processing. To use all topics then simply omit the flag.
 
 ```--topic-file```
 * Topics which should be filtered. Use this to speed up all of the processing. To use all topics then simply omit the flag. A file representing a list of topics. One topic per line.
 
-```--write_bag```
-* Including the flag tells ```rosbag-tools``` to write a new bag. Be sure to include an ```--outbag-name```.
-
-```--write_csvs```
-* Including the flag tells ```rosbag-tools``` to write a csv's with the topic data of interest.
-
-```--merge_csvs```
-* Takes the csvs in the input path and makes a single csv. The csv will fill topic data such that the new csv fills in data to share the same time and is easier to vizualize on plotjuggler or through matplotlib.
-
 > NOTE : More arguments are available if you want to use specific CSV's or Bag files. Run `rosbag-merge -h` for more information.
 
 ### Some environment variables
 
 ```
 export IN_PATH=/path/to/data
 export OUT_PATH=/path/to/data
@@ -285,27 +272,8 @@
 ```
 rosbag-merge --input_paths $IN_PATH --output_path $OUT_PATH --outbag_name $OUTBAG_NAME --topics $INPUT_TOPICS --write_bag 
 ```
 
 To merge bag files with select topics, and make single topics csvs.
 ```
 rosbag-merge --input_paths $IN_PATH --output_path $OUT_PATH --outbag_name $OUTBAG_NAME --write_bag --write_csvs 
-```
-
-Loop through the bag msgs and make single topics csvs.
-```
-rosbag-merge --input_paths $IN_PATH --output_path $OUT_PATH --outbag_name $OUTBAG_NAME --write_csvs 
-```
-
-Loop through the bag msgs and make single topics csvs.
-```
-rosbag-merge --input_paths $IN_PATH --output_path $OUT_PATH --outbag_name $OUTBAG_NAME --write_csvs 
-```
-
-
-### Merge CSVs
-
-For now, merging csvs must be done **after** making the CSVs on a previous command.
-```
-rosbag-merge --input_paths $IN_PATH --output_path $OUT_PATH  --merge_csvs
-```
-
+```
```

