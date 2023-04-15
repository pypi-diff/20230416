# Comparing `tmp/wwpdb.utils.dp-0.44.1.tar.gz` & `tmp/wwpdb.utils.dp-0.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.utils.dp-0.44.1.tar", last modified: Fri Jan 13 17:36:31 2023, max compression
+gzip compressed data, was "wwpdb.utils.dp-0.45.tar", last modified: Sat Apr 15 23:48:07 2023, max compression
```

## Comparing `wwpdb.utils.dp-0.44.1.tar` & `wwpdb.utils.dp-0.45.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-01-13 17:36:31.163682 wwpdb.utils.dp-0.44.1/
--rw-r--r--   0 vsts      (1001) docker     (123)       96 2023-01-13 17:35:37.000000 wwpdb.utils.dp-0.44.1/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (123)      552 2023-01-13 17:35:37.000000 wwpdb.utils.dp-0.44.1/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (123)      104 2023-01-13 17:35:37.000000 wwpdb.utils.dp-0.44.1/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (123)      757 2023-01-13 17:36:31.163682 wwpdb.utils.dp-0.44.1/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      180 2023-01-13 17:35:37.000000 wwpdb.utils.dp-0.44.1/README.md
--rwxr-xr-x   0 vsts      (1001) docker     (123)      108 2023-01-13 17:36:31.163682 wwpdb.utils.dp-0.44.1/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (123)     2125 2023-01-13 17:35:37.000000 wwpdb.utils.dp-0.44.1/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-01-13 17:36:31.159682 wwpdb.utils.dp-0.44.1/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-01-13 17:35:37.000000 wwpdb.utils.dp-0.44.1/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-01-13 17:36:31.159682 wwpdb.utils.dp-0.44.1/wwpdb/utils/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-01-13 17:35:37.000000 wwpdb.utils.dp-0.44.1/wwpdb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-01-13 17:36:31.163682 wwpdb.utils.dp-0.44.1/wwpdb/utils/dp/
--rw-r--r--   0 vsts      (1001) docker     (123)     5332 2023-01-13 17:35:37.000000 wwpdb.utils.dp-0.44.1/wwpdb/utils/dp/CentreOfMass.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11569 2023-01-13 17:35:37.000000 wwpdb.utils.dp-0.44.1/wwpdb/utils/dp/DataFileAdapter.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2358 2023-01-13 17:35:37.000000 wwpdb.utils.dp-0.44.1/wwpdb/utils/dp/DensityWrapper.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1918 2023-01-13 17:35:37.000000 wwpdb.utils.dp-0.44.1/wwpdb/utils/dp/PdbxChemShiftReport.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2694 2023-01-13 17:35:37.000000 wwpdb.utils.dp-0.44.1/wwpdb/utils/dp/PdbxMergeCategory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5231 2023-01-13 17:35:37.000000 wwpdb.utils.dp-0.44.1/wwpdb/utils/dp/PdbxSFMapCoefficients.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2368 2023-01-13 17:35:37.000000 wwpdb.utils.dp-0.44.1/wwpdb/utils/dp/PdbxStripCategory.py
--rw-r--r--   0 vsts      (1001) docker     (123)   205886 2023-01-13 17:35:37.000000 wwpdb.utils.dp-0.44.1/wwpdb/utils/dp/RcsbDpUtility.py
--rw-r--r--   0 vsts      (1001) docker     (123)    17219 2023-01-13 17:35:37.000000 wwpdb.utils.dp-0.44.1/wwpdb/utils/dp/RunRemote.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4429 2023-01-13 17:35:37.000000 wwpdb.utils.dp-0.44.1/wwpdb/utils/dp/ValidationWrapper.py
--rw-r--r--   0 vsts      (1001) docker     (123)      156 2023-01-13 17:35:37.000000 wwpdb.utils.dp-0.44.1/wwpdb/utils/dp/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-01-13 17:36:31.163682 wwpdb.utils.dp-0.44.1/wwpdb/utils/dp/electron_density/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-01-13 17:35:37.000000 wwpdb.utils.dp-0.44.1/wwpdb/utils/dp/electron_density/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3930 2023-01-13 17:35:37.000000 wwpdb.utils.dp-0.44.1/wwpdb/utils/dp/electron_density/common_functions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3801 2023-01-13 17:35:37.000000 wwpdb.utils.dp-0.44.1/wwpdb/utils/dp/electron_density/em_density_map.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10279 2023-01-13 17:35:37.000000 wwpdb.utils.dp-0.44.1/wwpdb/utils/dp/electron_density/x_ray_density_map.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-01-13 17:36:31.159682 wwpdb.utils.dp-0.44.1/wwpdb.utils.dp.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      757 2023-01-13 17:36:31.000000 wwpdb.utils.dp-0.44.1/wwpdb.utils.dp.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      898 2023-01-13 17:36:31.000000 wwpdb.utils.dp-0.44.1/wwpdb.utils.dp.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-01-13 17:36:31.000000 wwpdb.utils.dp-0.44.1/wwpdb.utils.dp.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-01-13 17:36:18.000000 wwpdb.utils.dp-0.44.1/wwpdb.utils.dp.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)      103 2023-01-13 17:36:31.000000 wwpdb.utils.dp-0.44.1/wwpdb.utils.dp.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-01-13 17:36:31.000000 wwpdb.utils.dp-0.44.1/wwpdb.utils.dp.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-15 23:48:07.176215 wwpdb.utils.dp-0.45/
+-rw-r--r--   0 vsts      (1001) docker     (123)       96 2023-04-15 23:47:02.000000 wwpdb.utils.dp-0.45/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)      552 2023-04-15 23:47:02.000000 wwpdb.utils.dp-0.45/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (123)      104 2023-04-15 23:47:02.000000 wwpdb.utils.dp-0.45/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (123)      755 2023-04-15 23:48:07.176215 wwpdb.utils.dp-0.45/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      180 2023-04-15 23:47:02.000000 wwpdb.utils.dp-0.45/README.md
+-rwxr-xr-x   0 vsts      (1001) docker     (123)      108 2023-04-15 23:48:07.176215 wwpdb.utils.dp-0.45/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     2125 2023-04-15 23:47:02.000000 wwpdb.utils.dp-0.45/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-15 23:48:07.168214 wwpdb.utils.dp-0.45/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-04-15 23:47:02.000000 wwpdb.utils.dp-0.45/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-15 23:48:07.172215 wwpdb.utils.dp-0.45/wwpdb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-04-15 23:47:02.000000 wwpdb.utils.dp-0.45/wwpdb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-15 23:48:07.176215 wwpdb.utils.dp-0.45/wwpdb/utils/dp/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5332 2023-04-15 23:47:02.000000 wwpdb.utils.dp-0.45/wwpdb/utils/dp/CentreOfMass.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11569 2023-04-15 23:47:02.000000 wwpdb.utils.dp-0.45/wwpdb/utils/dp/DataFileAdapter.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2358 2023-04-15 23:47:02.000000 wwpdb.utils.dp-0.45/wwpdb/utils/dp/DensityWrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1782 2023-04-15 23:47:02.000000 wwpdb.utils.dp-0.45/wwpdb/utils/dp/DepositorSyncUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1918 2023-04-15 23:47:02.000000 wwpdb.utils.dp-0.45/wwpdb/utils/dp/PdbxChemShiftReport.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2694 2023-04-15 23:47:02.000000 wwpdb.utils.dp-0.45/wwpdb/utils/dp/PdbxMergeCategory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5231 2023-04-15 23:47:02.000000 wwpdb.utils.dp-0.45/wwpdb/utils/dp/PdbxSFMapCoefficients.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2368 2023-04-15 23:47:02.000000 wwpdb.utils.dp-0.45/wwpdb/utils/dp/PdbxStripCategory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   206750 2023-04-15 23:47:02.000000 wwpdb.utils.dp-0.45/wwpdb/utils/dp/RcsbDpUtility.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    17219 2023-04-15 23:47:02.000000 wwpdb.utils.dp-0.45/wwpdb/utils/dp/RunRemote.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4429 2023-04-15 23:47:02.000000 wwpdb.utils.dp-0.45/wwpdb/utils/dp/ValidationWrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      154 2023-04-15 23:47:02.000000 wwpdb.utils.dp-0.45/wwpdb/utils/dp/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-15 23:48:07.176215 wwpdb.utils.dp-0.45/wwpdb/utils/dp/electron_density/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-15 23:47:02.000000 wwpdb.utils.dp-0.45/wwpdb/utils/dp/electron_density/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3930 2023-04-15 23:47:02.000000 wwpdb.utils.dp-0.45/wwpdb/utils/dp/electron_density/common_functions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3801 2023-04-15 23:47:02.000000 wwpdb.utils.dp-0.45/wwpdb/utils/dp/electron_density/em_density_map.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10279 2023-04-15 23:47:02.000000 wwpdb.utils.dp-0.45/wwpdb/utils/dp/electron_density/x_ray_density_map.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-15 23:48:07.172215 wwpdb.utils.dp-0.45/wwpdb.utils.dp.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      755 2023-04-15 23:48:07.000000 wwpdb.utils.dp-0.45/wwpdb.utils.dp.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      934 2023-04-15 23:48:07.000000 wwpdb.utils.dp-0.45/wwpdb.utils.dp.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-15 23:48:07.000000 wwpdb.utils.dp-0.45/wwpdb.utils.dp.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-15 23:47:53.000000 wwpdb.utils.dp-0.45/wwpdb.utils.dp.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)      103 2023-04-15 23:48:07.000000 wwpdb.utils.dp-0.45/wwpdb.utils.dp.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-04-15 23:48:07.000000 wwpdb.utils.dp-0.45/wwpdb.utils.dp.egg-info/top_level.txt
```

### Comparing `wwpdb.utils.dp-0.44.1/LICENSE` & `wwpdb.utils.dp-0.45/LICENSE`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.44.1/PKG-INFO` & `wwpdb.utils.dp-0.45/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.dp
-Version: 0.44.1
+Version: 0.45
 Summary: API for Common Data Processing Operations
 Home-page: https://github.com/wwpdb/py-wwpdb_utils_dp
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.utils.dp-0.44.1/setup.py` & `wwpdb.utils.dp-0.45/setup.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.44.1/wwpdb/utils/dp/CentreOfMass.py` & `wwpdb.utils.dp-0.45/wwpdb/utils/dp/CentreOfMass.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.44.1/wwpdb/utils/dp/DataFileAdapter.py` & `wwpdb.utils.dp-0.45/wwpdb/utils/dp/DataFileAdapter.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.44.1/wwpdb/utils/dp/DensityWrapper.py` & `wwpdb.utils.dp-0.45/wwpdb/utils/dp/DensityWrapper.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.44.1/wwpdb/utils/dp/PdbxChemShiftReport.py` & `wwpdb.utils.dp-0.45/wwpdb/utils/dp/PdbxChemShiftReport.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.44.1/wwpdb/utils/dp/PdbxMergeCategory.py` & `wwpdb.utils.dp-0.45/wwpdb/utils/dp/PdbxMergeCategory.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.44.1/wwpdb/utils/dp/PdbxSFMapCoefficients.py` & `wwpdb.utils.dp-0.45/wwpdb/utils/dp/PdbxSFMapCoefficients.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.44.1/wwpdb/utils/dp/PdbxStripCategory.py` & `wwpdb.utils.dp-0.45/wwpdb/utils/dp/PdbxStripCategory.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.44.1/wwpdb/utils/dp/RcsbDpUtility.py` & `wwpdb.utils.dp-0.45/wwpdb/utils/dp/RcsbDpUtility.py`

 * *Files 1% similar despite different names*

```diff
@@ -352,15 +352,15 @@
             "em-density-bcif",
             "xray-density-bcif",
             "centre-of-mass",
         ]
 
         self.__sequenceOps = ["seq-blastp", "seq-blastn", "fetch-uniprot", "fetch-gb", "format-uniprot", "format-gb", "backup-seqdb"]
         self.__validateOps = ["validate-geometry"]
-        self.__dbOps = ["db-loader"]
+        self.__dbOps = ["db-loader", "sync-depositors"]
         self.__emOps = [
             "mapfix-big",
             "em2em-spider",
             "fsc_check",
             "img-convert",
             "annot-read-map-header",
             "annot-read-map-header-in-place",
@@ -2024,15 +2024,15 @@
                 shutil.copyfile(xyzPathFull, xyzWrkPath)
             else:
                 xyzPath = "none"
                 xyzPathFull = "none"
 
             # First add data items to the model
             cmd += " ; " + maxitCmd + " -o 8  -i " + xyzWrkPath + " -dep -log maxit.log "
-            cmd += " ; mv -f " + xyzWrkPath + ".cif " + xyzCnvWrkPath
+            cmd += " ; mv -f " + xyzWrkPath + ".cif " + xyzCnvWrkPath  # pylint: disable=used-before-assignment
             #
             cmd += thisCmd + " -input " + iPath + " -output " + oPath + " -ciffile " + xyzCnvWrkPath + " -log " + lCheckPath
             cmd += " > " + tPath + " 2>&1 ; cat " + tPath + " >> " + lPath
 
         elif op == "annot-chem-shifts-update":
             #  iPath input is the target chemical shift file oPath is the output cs file
             #
@@ -2973,14 +2973,17 @@
 
         Now using only validation pack functions.
         """
         #
         # Set application specific path details here -
         #
         self.__packagePath = self.__cICommon.get_site_packages_path()
+        self.__siteConfigDir = self.__getConfigPath("TOP_WWPDB_SITE_CONFIG_DIR")
+        self.__siteLoc = self.__cI.get("WWPDB_SITE_LOC")
+        self.__site_config_command = ". %s/init/env.sh -s %s -l %s" % (self.__siteConfigDir, self.__siteId, self.__siteLoc)
 
         #
         #
         iPath = self.__getSourceWrkFile(self.__stepNo)
         # iPathList = self.__getSourceWrkFileList(self.__stepNo)
         oPath = self.__getResultWrkFile(self.__stepNo)
         lPath = self.__getLogWrkFile(self.__stepNo)
@@ -3032,14 +3035,22 @@
 
             cmd += "; rm -f DB_LOADER.sql "
             thisCmd = " ; " + dbLoaderCmd
             cmd += thisCmd + " -server mysql " + filecmd + " -map " + mappingfile + " -db " + dbServer + firstcmd
             #
             cmd += " > " + tPath + " 2>&1 ; cat " + tPath + " >> " + lPath
             cmd += " ; cp DB_LOADER.sql " + oPath
+        elif op == "sync-depositors":
+            depId = self.__inputParamDict.get("depId", None)
+            modelFilePath = self.__inputParamDict.get("modelFilePath", None)
+
+            cmd += "; {}".format(self.__site_config_command)
+            cmd += " ; python -m wwpdb.apps.deposit.scripts.sync_depositors --dep-id " + depId + " --model-file " + modelFilePath
+            #
+            cmd += " > " + tPath + " 2>&1 ; cat " + tPath + " >> " + lPath
         else:
             return -1
         #
 
         if self.__debug:
             logger.info("+RcsbDpUtility._dbStep()  - Application string:\n%s\n", cmd.replace(";", "\n"))
         #
@@ -3221,15 +3232,15 @@
 
             if "map_file_path" in self.__inputParamDict:
                 inpMapFilePath = self.__inputParamDict["map_file_path"]
             # Export map header as JSON packet -
             jarPath = os.path.join(self.__packagePath, "mapFix", "mapFixAnot.jar")
             cmd += self.__javaPath + " -Xms256m -Xmx256m -jar " + jarPath
             # -out is a temporary file place holder --
-            cmd += " -in " + inpMapFilePath + " -out  dummy-out.map "
+            cmd += " -in " + inpMapFilePath + " -out  dummy-out.map "  # pylint: disable=used-before-assignment
             # these dummy arguments required to run this code --
             cmd += " -voxel 1.0 1.0 1.0 -label test "
             # oPath here will be the JSON  output containing may header details --
             cmd += " ; } 2> " + ePath + " 1> " + oPath
             cmd += " ; cat " + ePath + " > " + lPath
 
         elif op == "annot-update-map-header-in-place":
@@ -3250,15 +3261,15 @@
 
             if "output_map_file_path" in self.__inputParamDict:
                 outMapFilePath = self.__inputParamDict["output_map_file_path"]
             #
             jarPath = os.path.join(self.__packagePath, "mapFix", "mapFixAnot.jar")
             cmd += self.__javaPath + " -Xms256m -Xmx256m -jar " + jarPath
             # -out is a temporary file place holder --
-            cmd += " -in " + inpMapFilePath + " -out  " + outMapFilePath
+            cmd += " -in " + inpMapFilePath + " -out  " + outMapFilePath  # pylint: disable=used-before-assignment
             #
             if "voxel" in self.__inputParamDict:
                 argVal = self.__inputParamDict["voxel"]
                 cmd += " -voxel " + argVal
 
             if "cell" in self.__inputParamDict:
                 argVal = self.__inputParamDict["cell"]
```

### Comparing `wwpdb.utils.dp-0.44.1/wwpdb/utils/dp/RunRemote.py` & `wwpdb.utils.dp-0.45/wwpdb/utils/dp/RunRemote.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.44.1/wwpdb/utils/dp/ValidationWrapper.py` & `wwpdb.utils.dp-0.45/wwpdb/utils/dp/ValidationWrapper.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.44.1/wwpdb/utils/dp/electron_density/common_functions.py` & `wwpdb.utils.dp-0.45/wwpdb/utils/dp/electron_density/common_functions.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.44.1/wwpdb/utils/dp/electron_density/em_density_map.py` & `wwpdb.utils.dp-0.45/wwpdb/utils/dp/electron_density/em_density_map.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.44.1/wwpdb/utils/dp/electron_density/x_ray_density_map.py` & `wwpdb.utils.dp-0.45/wwpdb/utils/dp/electron_density/x_ray_density_map.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.44.1/wwpdb.utils.dp.egg-info/PKG-INFO` & `wwpdb.utils.dp-0.45/wwpdb.utils.dp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.dp
-Version: 0.44.1
+Version: 0.45
 Summary: API for Common Data Processing Operations
 Home-page: https://github.com/wwpdb/py-wwpdb_utils_dp
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.utils.dp-0.44.1/wwpdb.utils.dp.egg-info/SOURCES.txt` & `wwpdb.utils.dp-0.45/wwpdb.utils.dp.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 wwpdb.utils.dp.egg-info/not-zip-safe
 wwpdb.utils.dp.egg-info/requires.txt
 wwpdb.utils.dp.egg-info/top_level.txt
 wwpdb/utils/__init__.py
 wwpdb/utils/dp/CentreOfMass.py
 wwpdb/utils/dp/DataFileAdapter.py
 wwpdb/utils/dp/DensityWrapper.py
+wwpdb/utils/dp/DepositorSyncUtil.py
 wwpdb/utils/dp/PdbxChemShiftReport.py
 wwpdb/utils/dp/PdbxMergeCategory.py
 wwpdb/utils/dp/PdbxSFMapCoefficients.py
 wwpdb/utils/dp/PdbxStripCategory.py
 wwpdb/utils/dp/RcsbDpUtility.py
 wwpdb/utils/dp/RunRemote.py
 wwpdb/utils/dp/ValidationWrapper.py
```

