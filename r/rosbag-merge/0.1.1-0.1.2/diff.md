# Comparing `tmp/rosbag_merge-0.1.1.tar.gz` & `tmp/rosbag_merge-0.1.2.tar.gz`

## Comparing `rosbag_merge-0.1.1.tar` & `rosbag_merge-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 rosbag_merge-0.1.1/INSTALL.md
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 rosbag_merge-0.1.1/requirements.txt
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 rosbag_merge-0.1.1/.github/workflows/publish-to-pypi-and-test-pypi.yml
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 rosbag_merge-0.1.1/examples/main_direct.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 rosbag_merge-0.1.1/src/rosbag_merge/__init__.py
--rw-r--r--   0        0        0     3669 2020-02-02 00:00:00.000000 rosbag_merge-0.1.1/src/rosbag_merge/bag_stream.py
--rwxr-xr-x   0        0        0     4875 2020-02-02 00:00:00.000000 rosbag_merge-0.1.1/src/rosbag_merge/main.py
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 rosbag_merge-0.1.1/src/rosbag_merge/deprecated/csv_merge.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 rosbag_merge-0.1.1/src/rosbag_merge/deprecated/merge_bags.py
--rw-r--r--   0        0        0    10427 2020-02-02 00:00:00.000000 rosbag_merge-0.1.1/src/rosbag_merge/deprecated/rosbag_to_csv.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 rosbag_merge-0.1.1/tests/topic_list.txt
--rw-r--r--   0        0        0    20625 2020-02-02 00:00:00.000000 rosbag_merge-0.1.1/tests/data/raw/TB3_WAFFLE_SLAM_cmd_vel_only.bag
--rw-r--r--   0        0        0   331893 2020-02-02 00:00:00.000000 rosbag_merge-0.1.1/tests/data/raw/TB3_WAFFLE_SLAM_imu_only.bag
--rw-r--r--   0        0        0   121303 2020-02-02 00:00:00.000000 rosbag_merge-0.1.1/tests/data/raw/TB3_WAFFLE_SLAM_odom_tf_static.bag
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 rosbag_merge-0.1.1/.gitignore
--rw-r--r--   0        0        0    10762 2020-02-02 00:00:00.000000 rosbag_merge-0.1.1/LICENSE
--rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 rosbag_merge-0.1.1/README.md
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 rosbag_merge-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    14969 2020-02-02 00:00:00.000000 rosbag_merge-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 rosbag_merge-0.1.2/INSTALL.md
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 rosbag_merge-0.1.2/requirements.txt
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 rosbag_merge-0.1.2/.github/workflows/publish-to-pypi-and-test-pypi.yml
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 rosbag_merge-0.1.2/examples/main_direct.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 rosbag_merge-0.1.2/src/rosbag_merge/__init__.py
+-rw-r--r--   0        0        0     3669 2020-02-02 00:00:00.000000 rosbag_merge-0.1.2/src/rosbag_merge/bag_stream.py
+-rwxr-xr-x   0        0        0     4875 2020-02-02 00:00:00.000000 rosbag_merge-0.1.2/src/rosbag_merge/main.py
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 rosbag_merge-0.1.2/src/rosbag_merge/deprecated/csv_merge.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 rosbag_merge-0.1.2/src/rosbag_merge/deprecated/merge_bags.py
+-rw-r--r--   0        0        0    10427 2020-02-02 00:00:00.000000 rosbag_merge-0.1.2/src/rosbag_merge/deprecated/rosbag_to_csv.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 rosbag_merge-0.1.2/tests/topic_list.txt
+-rw-r--r--   0        0        0    20625 2020-02-02 00:00:00.000000 rosbag_merge-0.1.2/tests/data/raw/TB3_WAFFLE_SLAM_cmd_vel_only.bag
+-rw-r--r--   0        0        0   331893 2020-02-02 00:00:00.000000 rosbag_merge-0.1.2/tests/data/raw/TB3_WAFFLE_SLAM_imu_only.bag
+-rw-r--r--   0        0        0   121303 2020-02-02 00:00:00.000000 rosbag_merge-0.1.2/tests/data/raw/TB3_WAFFLE_SLAM_odom_tf_static.bag
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 rosbag_merge-0.1.2/.gitignore
+-rw-r--r--   0        0        0    10762 2020-02-02 00:00:00.000000 rosbag_merge-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 rosbag_merge-0.1.2/README.md
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 rosbag_merge-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    14969 2020-02-02 00:00:00.000000 rosbag_merge-0.1.2/PKG-INFO
```

### Comparing `rosbag_merge-0.1.1/.github/workflows/publish-to-pypi-and-test-pypi.yml` & `rosbag_merge-0.1.2/.github/workflows/publish-to-pypi-and-test-pypi.yml`

 * *Files identical despite different names*

### Comparing `rosbag_merge-0.1.1/examples/main_direct.py` & `rosbag_merge-0.1.2/examples/main_direct.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 main_args = argparse.Namespace()
 main_args.input_paths = [os.path.join(os.getcwd(),"tests","data","raw")]
 main_args.output_path = os.path.join(os.getcwd(),"tests","data")
 main_args.outbag_name = "merged_bag"
 main_args.topic_file = os.path.join(os.getcwd(),"tests","topic_list.txt")
 # remove previous bag
 try:
-    os.remove(os.path.join(main_args.output_path,"merged_bag.bag"))
-    print("% s removed successfully" % path)
+    outbag = os.path.join(main_args.output_path,f"{main_args.outbag_name}.bag")
+    os.remove(outbag)
+    print(f"{outbag} removed successfully")
 except OSError as error:
     print(error)
     print("File path can not be removed")
 # Call the function
 main(main_args)
```

### Comparing `rosbag_merge-0.1.1/src/rosbag_merge/bag_stream.py` & `rosbag_merge-0.1.2/src/rosbag_merge/bag_stream.py`

 * *Files identical despite different names*

### Comparing `rosbag_merge-0.1.1/src/rosbag_merge/main.py` & `rosbag_merge-0.1.2/src/rosbag_merge/main.py`

 * *Files identical despite different names*

### Comparing `rosbag_merge-0.1.1/src/rosbag_merge/deprecated/csv_merge.py` & `rosbag_merge-0.1.2/src/rosbag_merge/deprecated/csv_merge.py`

 * *Files identical despite different names*

### Comparing `rosbag_merge-0.1.1/src/rosbag_merge/deprecated/merge_bags.py` & `rosbag_merge-0.1.2/src/rosbag_merge/deprecated/merge_bags.py`

 * *Files identical despite different names*

### Comparing `rosbag_merge-0.1.1/src/rosbag_merge/deprecated/rosbag_to_csv.py` & `rosbag_merge-0.1.2/src/rosbag_merge/deprecated/rosbag_to_csv.py`

 * *Files identical despite different names*

### Comparing `rosbag_merge-0.1.1/tests/data/raw/TB3_WAFFLE_SLAM_cmd_vel_only.bag` & `rosbag_merge-0.1.2/tests/data/raw/TB3_WAFFLE_SLAM_cmd_vel_only.bag`

 * *Files identical despite different names*

### Comparing `rosbag_merge-0.1.1/tests/data/raw/TB3_WAFFLE_SLAM_imu_only.bag` & `rosbag_merge-0.1.2/tests/data/raw/TB3_WAFFLE_SLAM_imu_only.bag`

 * *Files identical despite different names*

### Comparing `rosbag_merge-0.1.1/tests/data/raw/TB3_WAFFLE_SLAM_odom_tf_static.bag` & `rosbag_merge-0.1.2/tests/data/raw/TB3_WAFFLE_SLAM_odom_tf_static.bag`

 * *Files identical despite different names*

### Comparing `rosbag_merge-0.1.1/LICENSE` & `rosbag_merge-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rosbag_merge-0.1.1/README.md` & `rosbag_merge-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `rosbag_merge-0.1.1/pyproject.toml` & `rosbag_merge-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 [project]
 # add the distribution name of the package, the tar ball and python wheel use this name, this name goes the /home/$USER/.local/lib/python3.8/site-packages/
 name = "rosbag_merge"
 
 # version is the package version. See the version specifier specification
 # for more details on versions. Some build backends allow it to be 
 # specified another way, such as from a file or a git tag.
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Jonathan Sanabria", email="jonsanria@gmail.com" },
 ]
 description = "A gathering of tools for merging rosbags and saving their topic information to csv."
 readme = "README.md"
 license = { file="LICENSE" }
```

### Comparing `rosbag_merge-0.1.1/PKG-INFO` & `rosbag_merge-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosbag_merge
-Version: 0.1.1
+Version: 0.1.2
 Summary: A gathering of tools for merging rosbags and saving their topic information to csv.
 Project-URL: Homepage, https://github.com/1hada/rosbag-merge/
 Project-URL: Bug Tracker, https://github.com/1hada/rosbag-merge/issues/
 Author-email: Jonathan Sanabria <jonsanria@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

