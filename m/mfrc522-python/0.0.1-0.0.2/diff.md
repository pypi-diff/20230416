# Comparing `tmp/mfrc522-python-0.0.1.tar.gz` & `tmp/mfrc522-python-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mfrc522-python-0.0.1.tar", last modified: Fri Apr 14 17:20:41 2023, max compression
+gzip compressed data, was "mfrc522-python-0.0.2.tar", last modified: Sun Apr 16 16:11:43 2023, max compression
```

## Comparing `mfrc522-python-0.0.1.tar` & `mfrc522-python-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 17:20:41.848362 mfrc522-python-0.0.1/
--rw-rw-rw-   0        0        0    35823 2023-04-14 07:25:25.000000 mfrc522-python-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      700 2023-04-14 17:20:41.848362 mfrc522-python-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      104 2023-04-14 07:25:25.000000 mfrc522-python-0.0.1/README.md
--rw-rw-rw-   0        0        0      674 2023-04-14 08:59:07.000000 mfrc522-python-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-14 17:20:41.848362 mfrc522-python-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-14 17:20:41.781566 mfrc522-python-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-14 17:20:41.822821 mfrc522-python-0.0.1/src/mfrc522/
--rw-rw-rw-   0        0        0    22659 2023-04-14 08:28:28.000000 mfrc522-python-0.0.1/src/mfrc522/MFRC522.py
--rw-rw-rw-   0        0        0       50 2023-04-14 07:25:25.000000 mfrc522-python-0.0.1/src/mfrc522/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 17:20:41.845354 mfrc522-python-0.0.1/src/mfrc522_python.egg-info/
--rw-rw-rw-   0        0        0      700 2023-04-14 17:20:40.000000 mfrc522-python-0.0.1/src/mfrc522_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2023-04-14 17:20:40.000000 mfrc522-python-0.0.1/src/mfrc522_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 17:20:40.000000 mfrc522-python-0.0.1/src/mfrc522_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-14 17:20:40.000000 mfrc522-python-0.0.1/src/mfrc522_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 16:11:43.037782 mfrc522-python-0.0.2/
+-rw-rw-rw-   0        0        0    35823 2023-04-15 05:57:40.000000 mfrc522-python-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     3120 2023-04-16 16:11:43.037782 mfrc522-python-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2526 2023-04-16 16:10:38.000000 mfrc522-python-0.0.2/README.md
+-rw-rw-rw-   0        0        0      674 2023-04-16 16:11:20.000000 mfrc522-python-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-16 16:11:43.038785 mfrc522-python-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-16 16:11:43.009786 mfrc522-python-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-16 16:11:43.017779 mfrc522-python-0.0.2/src/mfrc522/
+-rw-rw-rw-   0        0        0    22665 2023-04-16 14:58:59.000000 mfrc522-python-0.0.2/src/mfrc522/MFRC522.py
+-rw-rw-rw-   0        0        0       50 2023-04-15 05:57:40.000000 mfrc522-python-0.0.2/src/mfrc522/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 16:11:43.035784 mfrc522-python-0.0.2/src/mfrc522_python.egg-info/
+-rw-rw-rw-   0        0        0     3120 2023-04-16 16:11:42.000000 mfrc522-python-0.0.2/src/mfrc522_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      247 2023-04-16 16:11:43.000000 mfrc522-python-0.0.2/src/mfrc522_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 16:11:42.000000 mfrc522-python-0.0.2/src/mfrc522_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-16 16:11:42.000000 mfrc522-python-0.0.2/src/mfrc522_python.egg-info/top_level.txt
```

### Comparing `mfrc522-python-0.0.1/LICENSE` & `mfrc522-python-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mfrc522-python-0.0.1/pyproject.toml` & `mfrc522-python-0.0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mfrc522-python"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="AnonymousXsn"},
 ]
 description = "The mfrc522 library is used to interact with RFID readers that use the MFRC522 chip"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: POSIX :: Linux",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/AnonymousXsn/MFRC522-python3"
-"Bug Tracker" = "https://github.com/AnonymousXsn/MFRC522-python3/issues"
+"Homepage" = "https://github.com/AnonymousXsn/MFRC522-python"
+"Bug Tracker" = "https://github.com/AnonymousXsn/MFRC522-python/issues"
```

### Comparing `mfrc522-python-0.0.1/src/mfrc522/MFRC522.py` & `mfrc522-python-0.0.2/src/mfrc522/MFRC522.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,15 +164,15 @@
         """
         Write a value to a register of the MFRC522 chip using SPI communication.
 
         This method sends a write command to the MFRC522 chip using the SPI interface, specifying the
         register address and the value to be written.
 
         Args:
-            addr (int): the address of the register to write to, in the range 0x00-0xFF.
+            :param: (int): the address of the register to write to, in the range 0x00-0xFF.
             val (int): the value to write to the register, in the range 0x00-0xFF.
         """
         val = self.spi.xfer2([(addr << 1) & 0x7E, val])
 
     def ReadReg(self, addr):
         """
         Read the value of a register of the MFRC522 chip using SPI communication.
@@ -576,15 +576,16 @@
             return backData
         # if response data length is not 16, return None
         else:
             return None
 
     def WriteTag(self, blockAddr, writeData):
         """
-        Writes data to a specified block address in the RFID tag.
+        Writes data to a specified block address in the RFID tag.'
+
         Args:
             blockAddr (int): The block address where data needs to be written
             writeData (list): A list of 16 bytes of data to be written to the block
 
         Returns:
             None
         """
```

