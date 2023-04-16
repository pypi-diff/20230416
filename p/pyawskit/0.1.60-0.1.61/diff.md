# Comparing `tmp/pyawskit-0.1.60.tar.gz` & `tmp/pyawskit-0.1.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyawskit-0.1.60.tar", last modified: Wed Jun  9 08:08:01 2021, max compression
+gzip compressed data, was "pyawskit-0.1.61.tar", last modified: Sun Apr 16 13:56:00 2023, max compression
```

## Comparing `pyawskit-0.1.60.tar` & `pyawskit-0.1.61.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2021-06-09 08:08:01.695785 pyawskit-0.1.60/
--rw-r--r--   0 mark      (1000) mark      (1000)       25 2017-11-26 05:03:48.000000 pyawskit-0.1.60/MANIFEST.in
--rw-r--r--   0 mark      (1000) mark      (1000)     1451 2021-06-09 08:08:01.695785 pyawskit-0.1.60/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      316 2021-06-09 08:07:42.000000 pyawskit-0.1.60/README.rst
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2021-06-09 08:08:01.694785 pyawskit-0.1.60/pyawskit/
--rw-rw-r--   0 mark      (1000) mark      (1000)        0 2016-11-03 02:32:24.000000 pyawskit-0.1.60/pyawskit/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)     3635 2020-11-21 23:57:10.000000 pyawskit-0.1.60/pyawskit/aws.py
--rw-r--r--   0 mark      (1000) mark      (1000)     7692 2020-11-16 13:24:05.000000 pyawskit-0.1.60/pyawskit/common.py
--rw-r--r--   0 mark      (1000) mark      (1000)      425 2020-07-25 11:32:57.000000 pyawskit-0.1.60/pyawskit/configs.py
--rw-r--r--   0 mark      (1000) mark      (1000)    13937 2020-11-16 13:23:16.000000 pyawskit-0.1.60/pyawskit/main.py
--rw-r--r--   0 mark      (1000) mark      (1000)     2828 2020-11-16 13:22:21.000000 pyawskit-0.1.60/pyawskit/os_utils.py
--rw-r--r--   0 mark      (1000) mark      (1000)      211 2021-06-09 08:07:42.000000 pyawskit-0.1.60/pyawskit/static.py
--rw-r--r--   0 mark      (1000) mark      (1000)     3346 2021-06-09 08:07:07.000000 pyawskit-0.1.60/pyawskit/utils.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2021-06-09 08:08:01.695785 pyawskit-0.1.60/pyawskit.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)     1451 2021-06-09 08:08:01.000000 pyawskit-0.1.60/pyawskit.egg-info/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      386 2021-06-09 08:08:01.000000 pyawskit-0.1.60/pyawskit.egg-info/SOURCES.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        1 2021-06-09 08:08:01.000000 pyawskit-0.1.60/pyawskit.egg-info/dependency_links.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       49 2021-06-09 08:08:01.000000 pyawskit-0.1.60/pyawskit.egg-info/entry_points.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       80 2021-06-09 08:08:01.000000 pyawskit-0.1.60/pyawskit.egg-info/requires.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        9 2021-06-09 08:08:01.000000 pyawskit-0.1.60/pyawskit.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       67 2021-06-09 08:08:01.695785 pyawskit-0.1.60/setup.cfg
--rw-r--r--   0 mark      (1000) mark      (1000)     1810 2021-06-09 08:07:42.000000 pyawskit-0.1.60/setup.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-16 13:56:00.683488 pyawskit-0.1.61/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1069 2023-04-16 13:55:50.000000 pyawskit-0.1.61/LICENSE
+-rw-r--r--   0 mark      (1000) mark      (1000)     1401 2023-04-16 13:56:00.683488 pyawskit-0.1.61/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      415 2023-04-16 13:55:50.000000 pyawskit-0.1.61/README.rst
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-16 13:56:00.683488 pyawskit-0.1.61/pyawskit/
+-rw-rw-r--   0 mark      (1000) mark      (1000)        0 2016-11-03 02:32:24.000000 pyawskit-0.1.61/pyawskit/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     3635 2020-11-21 23:57:10.000000 pyawskit-0.1.61/pyawskit/aws.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     7604 2023-03-08 22:51:40.000000 pyawskit-0.1.61/pyawskit/common.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1058 2021-09-08 16:57:25.000000 pyawskit-0.1.61/pyawskit/configs.py
+-rw-r--r--   0 mark      (1000) mark      (1000)    14050 2023-04-16 13:55:36.000000 pyawskit-0.1.61/pyawskit/main.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     2847 2022-07-01 11:36:28.000000 pyawskit-0.1.61/pyawskit/os_utils.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      211 2023-04-16 13:55:50.000000 pyawskit-0.1.61/pyawskit/static.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     3356 2022-07-01 11:39:13.000000 pyawskit-0.1.61/pyawskit/utils.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-16 13:56:00.683488 pyawskit-0.1.61/pyawskit.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)     1401 2023-04-16 13:56:00.000000 pyawskit-0.1.61/pyawskit.egg-info/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      382 2023-04-16 13:56:00.000000 pyawskit-0.1.61/pyawskit.egg-info/SOURCES.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-04-16 13:56:00.000000 pyawskit-0.1.61/pyawskit.egg-info/dependency_links.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       48 2023-04-16 13:56:00.000000 pyawskit-0.1.61/pyawskit.egg-info/entry_points.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       80 2023-04-16 13:56:00.000000 pyawskit-0.1.61/pyawskit.egg-info/requires.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        9 2023-04-16 13:56:00.000000 pyawskit-0.1.61/pyawskit.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       67 2023-04-16 13:56:00.684488 pyawskit-0.1.61/setup.cfg
+-rw-r--r--   0 mark      (1000) mark      (1000)     1730 2023-04-16 13:55:50.000000 pyawskit-0.1.61/setup.py
```

### Comparing `pyawskit-0.1.60/PKG-INFO` & `pyawskit-0.1.61/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 Metadata-Version: 2.1
 Name: pyawskit
-Version: 0.1.60
+Version: 0.1.61
 Summary: pyawskit is a collection of utilities to help interact with aws
 Home-page: https://veltzer.github.io/pyawskit
+Download-URL: https://github.com/veltzer/pyawskit
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
 License: MIT
-Download-URL: https://github.com/veltzer/pyawskit
-Description: ==========
-        *pyawskit*
-        ==========
-        
-        .. image:: https://img.shields.io/pypi/v/pyawskit
-        
-        .. image:: https://img.shields.io/github/license/veltzer/pyawskit
-        
-        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-        
-        project website: https://veltzer.github.io/pyawskit
-        
-        author: Mark Veltzer
-        
-        version: 0.1.60
-        
-        
-        
 Keywords: aws,utils,python,API,command,line
 Platform: python3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+==========
+*pyawskit*
+==========
+
+.. image:: https://img.shields.io/pypi/v/pyawskit
+
+.. image:: https://img.shields.io/github/license/veltzer/pyawskit
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+
+project website: https://veltzer.github.io/pyawskit
+
+author: Mark Veltzer
+
+version: 0.1.61
+
+	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2016, 2017, 2018, 2019, 2020, 2021, 2022, 2023
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyawskit-0.1.60/pyawskit/aws.py` & `pyawskit-0.1.61/pyawskit/aws.py`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.60/pyawskit/common.py` & `pyawskit-0.1.61/pyawskit/common.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,25 +3,27 @@
 import logging
 import os
 import socket
 import stat
 import subprocess
 import sys
 import time
-from typing import List
+from typing import List, Optional
 
 import boto3
 import requests
 
 
 def load_json_config(
     name: str,
 ):
+    home = os.getenv("HOME")
+    assert home is not None
     path = os.path.join(
-        os.getenv('HOME'),
+        home,
         ".pyawskit",
         name + ".json",
     )
     with open(path, "rt") as input_handle:
         obj = json.load(input_handle)
     return obj
 
@@ -35,30 +37,30 @@
         Wait for network service to appear
         http://code.activestate.com/recipes/576655-wait-for-network-service-to-appear/
         :param port:
         :param server:
         :param timeout
     """
     s = socket.socket()
-    end = None
+    end: float
     if timeout:
         # time module is needed to calc timeout shared between two exceptions
         end = time.time() + timeout
 
     while True:
         try:
             if timeout:
                 next_timeout = end - time.time()
                 if next_timeout < 0:
                     return False
                 s.settimeout(next_timeout)
 
             s.connect((server, port))
 
-        except socket.timeout as _:
+        except socket.timeout:
             # this exception occurs only if timeout is set
             if timeout:
                 return False
 
         except socket.error as err:
             # catch timeout exception from underlying network library
             # this one is different from socket.timeout
@@ -69,41 +71,41 @@
             return True
 
 
 def get_disks() -> List[str]:
     # another option is to take the output of lsblk(1)
     # which is not amazon specific and has nice format of data.
     url = "http://169.254.169.254/latest/meta-data/block-device-mapping"
-    r = requests.get(url)
+    r = requests.get(url, timeout=5)
     disks = []
     for line in r.content.decode().split("\n"):
         if not line.startswith('ephemeral'):
             continue
-        ephemeral_url = 'http://169.254.169.254/latest/meta-data/block-device-mapping/{}'.format(line)
-        r = requests.get(ephemeral_url)
+        ephemeral_url = f"http://169.254.169.254/latest/meta-data/block-device-mapping/{line}"
+        r = requests.get(ephemeral_url, timeout=5)
         assert r.status_code == 200
         content = r.content.decode()
         assert content.startswith('sd')
         assert len(content) == 3
         letter = content[2]
-        device = '/dev/xvd{}'.format(letter)
+        device = f"/dev/xvd{letter}"
         mode = os.stat(device).st_mode
         if not stat.S_ISBLK(mode):
             continue
         disks.append(device)
     return disks
 
 
 def erase_partition_table(disk: str) -> None:
     logger = logging.getLogger(__name__)
     logger.info("erasing partition table on disk [%s]", disk)
     subprocess.check_call([
         "/bin/dd",
         "if=/dev/zero",
-        "of={}".format(disk),
+        f"of={disk}"
         "bs=4096",
         "count=1024",
     ], stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
 
 
 def reread_partition_table() -> None:
     logger = logging.getLogger(__name__)
@@ -115,72 +117,68 @@
 
 def all_regions() -> List[str]:
     client = boto3.client('ec2')
     regions = [region['RegionName'] for region in client.describe_regions()['Regions']]
     return regions
 
 
-def format_device(disk: str, label: str = None) -> None:
+def format_device(disk: str, label: Optional[str] = None) -> None:
     logger = logging.getLogger(__name__)
-    logger.info("formatting the new device [%s]", disk)
+    logger.info(f"formatting the new device [{disk}]")
     args = [
         "/sbin/mkfs.ext4",
         disk,
     ]
     if label is not None:
         args.extend([
             "-L",
             label,
         ])
     subprocess.check_call(args, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
 
 
 def update_file(
-    filename: str = None,
-    pattern: str = None,
+    filename: str,
+    pattern: str,
     do_all: bool = False,
 ):
     logger = logging.getLogger(__name__)
-    assert filename is not None
-    assert pattern is not None
 
     config_file = os.path.expanduser(filename)
     if os.path.isfile(config_file):
         with open(config_file) as file_handle:
             lines = file_handle.readlines()
     else:
         lines = []
 
     # cut down auto generated lines if they exist...
     comment_line = "# DO NOT EDIT BEYOND THIS LINE - LEAVE THIS LINE AS IS\n"
-    try:
+    if comment_line in lines:
         location_of_comment_line = lines.index(comment_line)
         lines = lines[:location_of_comment_line]
-    except ValueError:
-        pass
 
     filter_file = os.path.expanduser("~/.pyawskit/aws_filter.json")
     if os.path.isfile(filter_file):
-        logger.info('reading [{0}]...'.format(filter_file))
+        logger.info(f"reading [{filter_file}]...")
         with open(filter_file) as file_handle:
             filters = json.loads(file_handle.read())
     else:
-        logger.info('no filter file [{0}] exists...'.format(filter_file))
+        logger.info(f"no filter file [{filter_file}] exists...")
         filters = []
 
     # look for servers matching the query, in all regions
     instances = []
     for region in all_regions():
         ec2 = boto3.resource('ec2', region_name=region)
         if do_all:
             instances.extend(list(ec2.instances.all()))
         else:
             instances.extend(list(ec2.instances.filter(Filters=filters)))
     num_of_instances = len(instances)
-    logger.info("Found {} instance(s)".format(num_of_instances))
+    logger.info(f"Found {num_of_instances} instance(s)")
     # assert num_of_instances > 0
 
     # add the comment line
     lines.append(comment_line)
 
     # add bunch of lines for each server
     added = 0
@@ -190,15 +188,15 @@
         tags_dict = {}
         for tag in instance.tags:
             tags_dict[tag["Key"]] = tag["Value"]
         if "Name" not in tags_dict:
             continue
         host = tags_dict["Name"]
         if host == "" or " " in host:
-            logger.info('Name [{0}] for host is bad. Try non empty names without spaces...'.format(host))
+            logger.info(f"Name [{host}] for host is bad. Try non empty names without spaces...")
             continue
         # public_ip = instance.public_dns_name
         # if public_ip == "":
         #    continue
         # logger.info(dir(instance))
         private_ip = instance.private_ip_address
         if private_ip == "":
@@ -210,16 +208,16 @@
         )
         lines.extend(pattern_to_add)
         added += 1
 
     # print the final lines to the config file
     with open(config_file, "wt") as file_handle:
         file_handle.writelines(lines)
-    logger.info("Added {} instance(s)".format(added))
-    logger.info("Written {}".format(config_file))
+    logger.info(f"Added {added} instance(s)")
+    logger.info(f"Written {config_file}")
 
 
 def mount_disk(disk: str, folder: str) -> None:
     logger = logging.getLogger(__name__)
     logger.info("mounting the new device [%s, %s]", disk, folder)
     if not os.path.isdir(folder):
         os.makedirs(folder)
```

### Comparing `pyawskit-0.1.60/pyawskit/main.py` & `pyawskit-0.1.61/pyawskit/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 from pytconf import register_main, config_arg_parse_and_launch, register_endpoint
 
 import pyawskit.common
 from pyawskit.aws import ProcessData, request_spot_instances, tag_resources, poll_instances_till_done, wait_for_ssh, \
     attach_disks
 from pyawskit.common import update_etc_hosts, update_ssh_config, update_file, do_hush_login, wait_net_service, \
     get_disks, erase_partition_table, reread_partition_table, format_device, mount_disk
-from pyawskit.configs import ConfigFilter, ConfigName
+from pyawskit.configs import ConfigFilter, ConfigName, ConfigWork
 
 from pyawskit.static import APP_NAME, VERSION_STR
-from pyawskit.utils import object_exists, process_one_file, print_exception
+from pyawskit.utils import object_exists, compress_one_file, print_exception
 
 
 FILE_ETC_HOSTS = "/etc/hosts"
 
 
 @register_endpoint(
     description="Compress an S3 folder",
@@ -47,27 +47,26 @@
     s3 = boto3.resource('s3')
     bucket = s3.Bucket(bucket_name)
     gen = bucket.objects.filter(Prefix=folder_in)
     if do_progress:
         gen = tqdm.tqdm(gen)
     jobs = []
     for object_summary in gen:
-        print('doing [{}]'.format(object_summary.key))
+        print(f"doing [{object_summary.key}]")
         full_name = object_summary.key
         basename = os.path.basename(full_name)
         compressed_basename = basename + '.gz'
         full_compressed_name = os.path.join(folder_out, compressed_basename)
         if object_exists(s3, bucket_name, full_compressed_name):
             print('object exists, skipping')
             continue
         jobs.append([basename, full_name, compressed_basename, full_compressed_name, bucket_name])
-    pool = multiprocessing.Pool(processes=multiprocessing.cpu_count())
-    pool.map_async(process_one_file, jobs, error_callback=print_exception)
-    pool.close()
-    pool.join()
+    with multiprocessing.Pool(processes=multiprocessing.cpu_count()) as pool:
+        pool.map_async(compress_one_file, jobs, error_callback=print_exception)
+        pool.join()
 
 
 @register_endpoint(
     description="Copy important files to a machine like key files and such",
 )
 def copy_to_machine() -> None:
     """
@@ -85,15 +84,15 @@
     assert len(sys.argv) == 2
     machine_name = sys.argv[1]
     args = [
         "scp",
         "-r",
     ]
     args.extend(map(os.path.expanduser, folders_to_copy))
-    args.append("{machine_name}:~".format(machine_name=machine_name))
+    args.append(f"{machine_name}:~")
     # subprocess.check_call(args, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
     subprocess.check_call(args)
 
 
 @register_endpoint(
     description="Generate /etc/hosts file for you. Must be run as root",
     configs=[
@@ -102,15 +101,15 @@
 )
 def generate_etc_hosts() -> None:
     """
     This script will update ~/.aws/config file with the names of your machines.
     Notice that you must hold all of your .pem files in ~/.aws/keys
     """
     if not os.geteuid() == 0 and not os.access(FILE_ETC_HOSTS, os.W_OK):
-        sys.exit('script must be run as root or {} must be writable'.format(FILE_ETC_HOSTS))
+        sys.exit(f"script must be run as root or {FILE_ETC_HOSTS} must be writable")
     update_etc_hosts(all_hosts=not ConfigFilter.filter)
 
 
 @register_endpoint(
     description="Generate ~/ssh/config or ~/.ssh/config.d/99_dynamic.conf file for you",
     configs=[
         ConfigFilter,
@@ -192,15 +191,15 @@
     command line option) whether to run this multi-core or not.
     """
     pyawskit.common.check_root()
     # TODO: ask the user for yes/no confirmation since we are brutally
     # erasing all of the local disks...
     disks = pyawskit.common.get_disks()
     for disk in disks:
-        folder = "/mnt/{}".format(disk)
+        folder = f"/mnt/{disk}"
         pyawskit.common.erase_partition_table(disk=disk)
         pyawskit.common.format_device(disk=disk)
         pyawskit.common.mount_disk(disk=disk, folder=folder)
 
 
 @register_endpoint(
     description="Prepares your account on a new AWS machine",
@@ -274,147 +273,143 @@
     - http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/raid-config.html
     - http://www.tecmint.com/create-raid0-in-linux/
     - http://dev.bizo.com/2012/07/mdadm-device-or-resource-busy.html
 
     TODO:
     - make this script work in parallel. But for the dd(1) and mkfs(1) parts.
     """
-    device_file = "/dev/md0"
-    mount_point = "/mnt/raid0"
-    mdadm_config_file = '/etc/mdadm/mdadm.conf'
-    mdadm_binary = "/sbin/mdadm"
-    fstab_filename = "/etc/fstab"
-    file_system_type = "ext4"
-    name_of_raid_device = "MY_RAID"
-    start_stop_queue = False
-    write_etc_mdadm = False
-    add_line_to_fstab = False
 
     logger = logging.getLogger(__name__)
     logger.info("looking for disks...")
     disks = get_disks()
-    if len(disks) == 0:
-        print('found no disks, exiting...', file=sys.stderr)
-        sys.exit(1)
+    assert len(disks) > 0, "found no disks"
 
-    logger.info("got %d disks %s", len(disks), str(disks))
+    logger.info(f"got {len(disks)} disks {str(disks)}")
 
-    logger.info("checking if any of the disks are mounted [%s]", ','.join(disks))
-    manager = pymount.mgr.Manager()
-    for disk in disks:
-        if manager.is_mounted(disk):
-            mount_point = manager.get_mount_point(disk)
-            logger.info("unmounting device [%s] from [%s]", device_file, mount_point)
-            subprocess.check_call([
-                "/bin/umount",
-                mount_point,
-            ])
-        else:
-            logger.info("device [%s] is not mounted, good", device_file)
-
-    logger.info("checking if the md device is mounted...[%s]", device_file)
-    if manager.is_mounted(device_file):
-        mount_point = manager.get_mount_point(device_file)
-        logger.info("unmounting device [%s] from [%s]", device_file, mount_point)
-        subprocess.check_call([
-            "/bin/umount",
-            mount_point,
-        ])
-        logger.info("unmount of [%s] was ok", device_file)
-    else:
-        logger.info("device [%s] is not mounted, good...", device_file)
+    check_unmounted(logger, disks)
 
-    logger.info("checking if device exists [%s]", device_file)
-    if os.path.exists(device_file):
-        logger.info("stopping md on the current device [%s]", device_file)
+    logger.info(f"checking if device exists [{ConfigWork.device_file}]")
+    if os.path.exists(ConfigWork.device_file):
+        logger.info(f"stopping md on the current device [{ConfigWork.device_file}]")
         subprocess.check_call([
-            mdadm_binary,
+            ConfigWork.mdadm_binary,
             "--stop",
-            device_file,
+            ConfigWork.device_file,
         ], stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
-        logger.info("stopped md on [%s] successfully...", device_file)
+        logger.info(f"stopped md on [{ConfigWork.device_file}] successfully...")
     else:
-        logger.info("no md [%s], good", device_file)
+        logger.info(f"no md [{ConfigWork.device_file}], good")
 
     for disk in disks:
         erase_partition_table(disk)
     reread_partition_table()
 
-    logger.info("creating the new md device...")
-    if start_stop_queue:
-        subprocess.check_call([
-            "/sbin/udevadm",
-            "control",
-            "--stop-exec-queue",
-        ])
-    args = [
-        mdadm_binary,
-        "--create",
-        device_file,
-        "--level=0",  # RAID 0 for performance
-        "--name={}".format(name_of_raid_device),
-        # "-c256",
-        "--raid-devices={}".format(len(disks)),
-    ]
-    args.extend(disks)
-    subprocess.check_call(args, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
-    if start_stop_queue:
+    create_new_device(logger, disks)
+
+    if ConfigWork.start_stop_queue:
         subprocess.check_call([
             "/sbin/udevadm",
             "control",
             "--start-exec-queue",
         ])
 
     # removed writing /etc/mdadm because it was causing problems
-    if write_etc_mdadm:
-        logger.info("writing the details of the new device in [%s]", mdadm_config_file)
-        mdadm_handle = open(mdadm_config_file, "at")
-        subprocess.check_call([
-            mdadm_binary,
-            "--detail",
-            "--scan",
-            "--verbose",
-        ], stdout=mdadm_handle, stderr=subprocess.DEVNULL)
+    if ConfigWork.write_etc_mdadm:
+        logger.info(f"writing the details of the new device in [{ConfigWork.mdadm_config_file}]")
+        with open(ConfigWork.mdadm_config_file, "at") as mdadm_handle:
+            subprocess.check_call([
+                ConfigWork.mdadm_binary,
+                "--detail",
+                "--scan",
+                "--verbose",
+            ], stdout=mdadm_handle, stderr=subprocess.DEVNULL)
 
-    format_device(device_file, label=name_of_raid_device)
+    format_device(ConfigWork.device_file, label=ConfigWork.name_of_raid_device)
 
-    mount_disk(disk=device_file, folder=mount_point)
+    mount_disk(disk=ConfigWork.device_file, folder=ConfigWork.mount_point)
 
-    if add_line_to_fstab:
-        logger.info("checking if need to add line to [%s] for mount on reboot...", fstab_filename)
+    if ConfigWork.add_line_to_fstab:
+        logger.info(f"checking if need to add line to [{ConfigWork.fstab_filename}] for mount on reboot...")
         line_to_add = " ".join([
-            # device_file,
-            "LABEL={}".format(name_of_raid_device),
-            mount_point,
-            file_system_type,
+            # ConfigWork.device_file,
+            f"LABEL={ConfigWork.name_of_raid_device}",
+            ConfigWork.mount_point,
+            ConfigWork.file_system_type,
             "defaults",
             "0",
             "0",
         ])
         found_line_to_add = False
-        with open(fstab_filename) as file_handle:
+        with open(ConfigWork.fstab_filename) as file_handle:
             for line in file_handle:
                 line = line.rstrip()
                 if line == line_to_add:
                     found_line_to_add = True
                     break
         if found_line_to_add:
             logger.info("found the line to add. not doing anything...")
         else:
-            logger.info("adding line to [%s]", fstab_filename)
-            with open(fstab_filename, "at") as file_handle:
-                file_handle.write(line_to_add+"\n")
+            logger.info("adding line to [%s]", ConfigWork.fstab_filename)
+            with open(ConfigWork.fstab_filename, "at") as file_handle:
+                file_handle.write(line_to_add + "\n")
     # create ubuntu folder and chown it to ubuntu
 
 
 @register_main(
-    main_description="Pyawskit is you AWS Swiss Army Knife",
+    main_description="Pyawskit is your AWS Swiss Army Knife",
     app_name=APP_NAME,
     version=VERSION_STR,
 )
 def main():
     setup()
     config_arg_parse_and_launch()
 
 
+def create_new_device(logger, disks):
+    logger.info("creating the new md device...")
+    if ConfigWork.start_stop_queue:
+        subprocess.check_call([
+            "/sbin/udevadm",
+            "control",
+            "--stop-exec-queue",
+        ])
+    args = [
+        ConfigWork.mdadm_binary,
+        "--create",
+        ConfigWork.device_file,
+        "--level=0",  # RAID 0 for performance
+        f"--name={ConfigWork.name_of_raid_device}",
+        # "-c256",
+        f"--raid-devices={len(disks)}",
+    ]
+    args.extend(disks)
+    subprocess.check_call(args, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
+
+
+def check_unmounted(logger, disks):
+    logger.info(f"checking if any of the disks are mounted [{'.'.join(disks)}]")
+    manager = pymount.mgr.Manager()
+    for disk in disks:
+        if manager.is_mounted(disk):
+            mount_point = manager.get_mount_point(disk)
+            logger.info(f"unmounting device [{ConfigWork.device_file}] from [{mount_point}]")
+            subprocess.check_call([
+                "/bin/umount",
+                mount_point,
+            ])
+        else:
+            logger.info(f"device [{ConfigWork.device_file}] is not mounted, good")
+    logger.info(f"checking if the md device is mounted...[{ConfigWork.device_file}]")
+    if manager.is_mounted(ConfigWork.device_file):
+        mount_point = manager.get_mount_point(ConfigWork.device_file)
+        logger.info(f"unmounting device [{ConfigWork.device_file}] from [{mount_point}]")
+        subprocess.check_call([
+            "/bin/umount",
+            mount_point,
+        ])
+        logger.info(f"unmount of [{ConfigWork.device_file}] was ok")
+    else:
+        logger.info(f"device [{ConfigWork.device_file}] is not mounted, good...")
+
+
 if __name__ == '__main__':
     main()
```

### Comparing `pyawskit-0.1.60/pyawskit/os_utils.py` & `pyawskit-0.1.61/pyawskit/os_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import enum
 import subprocess
 import sys
+import shutil
+import os.path
+
+from typing import List, Dict
 
 from pyawskit.common import run_devnull
 
 
 class OSType(enum.Enum):
     ubuntu = 1
     aml = 2
 
 
-os_data = dict()
+os_data = {}
 OS_TYPE = "OS_TYPE"
 
 
 def set_timezone() -> None:
     subprocess.check_call([
         "timedatectl",
         "set-timezone",
@@ -23,29 +27,23 @@
 
 
 def detect_os() -> None:
     """
     first find out if we are on ubuntu or amazon linux
     :return:
     """
-    # noinspection PyBroadException,PyPep8
-    try:
-        if subprocess.check_output(['lsb_release', '--id', '-s']).decode().rstrip() == 'Ubuntu':
+    lsb_release = shutil.which("lsb_release")
+    if lsb_release is not None:
+        if subprocess.check_output([lsb_release, '--id', '-s']).decode().rstrip() == 'Ubuntu':
             os_data[OS_TYPE] = OSType.ubuntu
-    except Exception:
-        pass
-    # noinspection PyBroadException,PyPep8
-    try:
+    if os.path.isfile("/etc/issue"):
         with open('/etc/issue') as f:
             d = f.read()
             if d.startswith('Amazon Linux AMI'):
                 os_type = OSType.aml
-    except Exception:
-        pass
-
     if os_type is None:
         sys.exit('could not detect the os running')
 
 
 def is_os_type(t) -> bool:
     return os_data["OS_TYPE"] == t
 
@@ -60,15 +58,15 @@
 
 
 def install_packages() -> None:
     """
     install necessary package per platform
     :return:
     """
-    list_of_packages = {
+    list_of_packages: Dict[OSType, List[str]] = {
         OSType.ubuntu: [
             # python
             'python-pip',
             'python-dev',
             'python3-pip',
             'python3-dev',
             # amazon stuff
```

### Comparing `pyawskit-0.1.60/pyawskit/utils.py` & `pyawskit-0.1.61/pyawskit/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os.path
 import shutil
 import subprocess
 import sys
 
+from typing import Any, List
+
 import boto3
 # noinspection PyPackageRequirements
 import botocore
 # noinspection PyPackageRequirements
 import botocore.exceptions
 import pypipegzip
 
@@ -29,18 +31,15 @@
         f_out = pypipegzip.pypipegzip.zipopen(file_out, 'wb')
         shutil.copyfileobj(f_in, f_out)
         f_out.close()
 
 
 def gzip_file_process(file_in: str, file_out: str) -> None:
     subprocess.check_call(
-        'gzip < {file_in} > {file_out}'.format(
-            file_in=file_in,
-            file_out=file_out,
-        ),
+        f"gzip < {file_in} > {file_out}",
         shell=True,
     )
 
 
 def object_exists(s3_connection, check_bucket_name: str, object_name: str) -> bool:
     """
     It seems funny we have to write this method but it seems that this
@@ -50,15 +49,15 @@
 
     :param s3_connection:
     :param check_bucket_name:
     :param object_name:
     :return: whether the object exists
     """
     try:
-        #s3_connection.Object(check_bucket_name, object_name).load()
+        # s3_connection.Object(check_bucket_name, object_name).load()
         s3_connection.head_object(Bucket=check_bucket_name, Key=object_name)
     except botocore.exceptions.ClientError as e:
         if e.response['Error']['Code'] == "404":
             return False
         raise
     return True
 
@@ -77,26 +76,28 @@
         if e.response['Error']['Code'] == "404":
             return False
         raise
     return True
 
 
 def catch_all(the_function):
-    print('there')
-
     def new_function(*args, **kwargs):
-        print('here')
+        # pylint: disable=broad-except
         try:
             return the_function(*args, **kwargs)
         except Exception as e:
             print('got exception', e)
             sys.exit(1)
     return new_function
 
 
+def compress_one_file(_list: List[Any]) -> Any:
+    pass
+
+
 def process_one_file(basename, full_name, compressed_basename, full_compressed_name, bucket_name):
     s3 = boto3.resource('s3')
     bucket = s3.Bucket(bucket_name)
 
     print('downloading', full_name, basename)
     bucket.download_file(full_name, basename)
```

### Comparing `pyawskit-0.1.60/pyawskit.egg-info/PKG-INFO` & `pyawskit-0.1.61/pyawskit.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 Metadata-Version: 2.1
 Name: pyawskit
-Version: 0.1.60
+Version: 0.1.61
 Summary: pyawskit is a collection of utilities to help interact with aws
 Home-page: https://veltzer.github.io/pyawskit
+Download-URL: https://github.com/veltzer/pyawskit
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
 License: MIT
-Download-URL: https://github.com/veltzer/pyawskit
-Description: ==========
-        *pyawskit*
-        ==========
-        
-        .. image:: https://img.shields.io/pypi/v/pyawskit
-        
-        .. image:: https://img.shields.io/github/license/veltzer/pyawskit
-        
-        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-        
-        project website: https://veltzer.github.io/pyawskit
-        
-        author: Mark Veltzer
-        
-        version: 0.1.60
-        
-        
-        
 Keywords: aws,utils,python,API,command,line
 Platform: python3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+==========
+*pyawskit*
+==========
+
+.. image:: https://img.shields.io/pypi/v/pyawskit
+
+.. image:: https://img.shields.io/github/license/veltzer/pyawskit
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+
+project website: https://veltzer.github.io/pyawskit
+
+author: Mark Veltzer
+
+version: 0.1.61
+
+	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2016, 2017, 2018, 2019, 2020, 2021, 2022, 2023
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyawskit-0.1.60/setup.py` & `pyawskit-0.1.61/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,67 +5,62 @@
     with open('README.rst') as f:
         return f.read()
 
 
 setuptools.setup(
     # the first three fields are a must according to the documentation
     name="pyawskit",
-    version="0.1.60",
+    version="0.1.61",
     packages=[
-        'pyawskit',
+        "pyawskit",
     ],
     # from here all is optional
     description="pyawskit is a collection of utilities to help interact with aws",
     long_description=get_readme(),
     long_description_content_type="text/x-rst",
     author="Mark Veltzer",
     author_email="mark.veltzer@gmail.com",
     maintainer="Mark Veltzer",
     maintainer_email="mark.veltzer@gmail.com",
     keywords=[
-        'aws',
-        'utils',
-        'python',
-        'API',
-        'command',
-        'line',
+        "aws",
+        "utils",
+        "python",
+        "API",
+        "command",
+        "line",
     ],
     url="https://veltzer.github.io/pyawskit",
     download_url="https://github.com/veltzer/pyawskit",
     license="MIT",
     platforms=[
-        'python3',
+        "python3",
     ],
     install_requires=[
-        'pylogconf',
-        'pyfakeuse',
-        'pypipegzip',
-        'tqdm',
-        'requests',
-        'boto3',
-        'pymount',
-        'ujson',
-        'sultan',
-        'pytconf',
+        "pylogconf",
+        "pyfakeuse",
+        "pypipegzip",
+        "tqdm",
+        "requests",
+        "boto3",
+        "pymount",
+        "ujson",
+        "sultan",
+        "pytconf",
     ],
-    extras_require={
-    },
     classifiers=[
-        'Development Status :: 4 - Beta',
-        'Environment :: Console',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Topic :: Utilities',
-        'License :: OSI Approved :: MIT License',
-    ],
-    data_files=[
+        "Development Status :: 4 - Beta",
+        "Environment :: Console",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3 :: Only",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Topic :: Utilities",
+        "License :: OSI Approved :: MIT License",
     ],
     entry_points={"console_scripts": [
-        'pyawskit=pyawskit.main:main',
+        "pyawskit=pyawskit.main:main",
     ]},
-    python_requires=">=3.6",
 )
```

