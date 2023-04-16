# Comparing `tmp/ztfquery-1.8.1.tar.gz` & `tmp/ztfquery-1.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ztfquery-1.8.1.tar", last modified: Sat Nov 16 09:13:33 2019, max compression
+gzip compressed data, was "dist/ztfquery-1.8.4.tar", last modified: Thu Mar 26 12:59:30 2020, max compression
```

## Comparing `ztfquery-1.8.1.tar` & `ztfquery-1.8.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 mrigault   (501) staff       (20)        0 2019-11-16 09:13:33.000000 ztfquery-1.8.1/
--rw-r--r--   0 mrigault   (501) staff       (20)      794 2019-11-16 09:13:33.000000 ztfquery-1.8.1/PKG-INFO
-drwxr-xr-x   0 mrigault   (501) staff       (20)        0 2019-11-16 09:13:33.000000 ztfquery-1.8.1/ztfquery.egg-info/
--rw-r--r--   0 mrigault   (501) staff       (20)      794 2019-11-16 09:13:33.000000 ztfquery-1.8.1/ztfquery.egg-info/PKG-INFO
--rw-r--r--   0 mrigault   (501) staff       (20)      709 2019-11-16 09:13:33.000000 ztfquery-1.8.1/ztfquery.egg-info/SOURCES.txt
--rw-r--r--   0 mrigault   (501) staff       (20)        9 2019-11-16 09:13:33.000000 ztfquery-1.8.1/ztfquery.egg-info/top_level.txt
--rw-r--r--   0 mrigault   (501) staff       (20)        1 2019-11-16 09:13:33.000000 ztfquery-1.8.1/ztfquery.egg-info/dependency_links.txt
-drwxr-xr-x   0 mrigault   (501) staff       (20)        0 2019-11-16 09:13:33.000000 ztfquery-1.8.1/ztfquery/
--rw-r--r--   0 mrigault   (501) staff       (20)    32969 2019-09-12 10:12:54.000000 ztfquery-1.8.1/ztfquery/marshal.py
--rw-r--r--   0 mrigault   (501) staff       (20)    15095 2019-06-12 16:17:00.000000 ztfquery-1.8.1/ztfquery/lightcurve.py
--rw-r--r--   0 mrigault   (501) staff       (20)    12010 2019-11-16 08:55:41.000000 ztfquery-1.8.1/ztfquery/fields.py
--rw-r--r--   0 mrigault   (501) staff       (20)    34780 2019-09-20 08:09:06.000000 ztfquery-1.8.1/ztfquery/query.py
--rw-r--r--   0 mrigault   (501) staff       (20)    22995 2019-09-26 10:36:15.000000 ztfquery-1.8.1/ztfquery/sedm.py
--rw-r--r--   0 mrigault   (501) staff       (20)     9291 2019-01-23 13:44:20.000000 ztfquery-1.8.1/ztfquery/buildurl.py
--rw-r--r--   0 mrigault   (501) staff       (20)    13496 2019-06-12 09:47:51.000000 ztfquery-1.8.1/ztfquery/metasearch.py
--rw-r--r--   0 mrigault   (501) staff       (20)     7998 2019-11-16 09:04:04.000000 ztfquery-1.8.1/ztfquery/io.py
--rw-r--r--   0 mrigault   (501) staff       (20)       90 2019-11-16 09:07:28.000000 ztfquery-1.8.1/ztfquery/__init__.py
-drwxr-xr-x   0 mrigault   (501) staff       (20)        0 2019-11-16 09:13:33.000000 ztfquery-1.8.1/ztfquery/utils/
--rw-r--r--   0 mrigault   (501) staff       (20)     6469 2018-06-06 14:57:27.000000 ztfquery-1.8.1/ztfquery/utils/tools.py
--rw-r--r--   0 mrigault   (501) staff       (20)        3 2018-06-06 14:42:22.000000 ztfquery-1.8.1/ztfquery/utils/__init__.py
--rw-r--r--   0 mrigault   (501) staff       (20)     2964 2018-06-13 08:06:06.000000 ztfquery-1.8.1/ztfquery/utils/stamps.py
--rw-r--r--   0 mrigault   (501) staff       (20)    28386 2018-08-10 10:43:19.000000 ztfquery-1.8.1/ztfquery/query2.py
--rw-r--r--   0 mrigault   (501) staff       (20)     3319 2019-08-07 17:37:49.000000 ztfquery-1.8.1/ztfquery/ccd.py
-drwxr-xr-x   0 mrigault   (501) staff       (20)        0 2019-11-16 09:13:33.000000 ztfquery-1.8.1/ztfquery/data/
--rw-r--r--   0 mrigault   (501) staff       (20)    28668 2018-12-04 14:02:48.000000 ztfquery-1.8.1/ztfquery/data/filter_p48_i.dat
--rw-r--r--   0 mrigault   (501) staff       (20)       12 2018-04-23 15:10:31.000000 ztfquery-1.8.1/ztfquery/data/source
--rw-r--r--   0 mrigault   (501) staff       (20)     6230 2019-08-07 15:49:45.000000 ztfquery-1.8.1/ztfquery/data/ztf_ccd_quad_layout.tbl
--rw-r--r--   0 mrigault   (501) staff       (20)   123299 2018-04-29 13:32:13.000000 ztfquery-1.8.1/ztfquery/data/ztf_fields.txt
--rw-r--r--   0 mrigault   (501) staff       (20)     1419 2018-04-29 15:10:54.000000 ztfquery-1.8.1/ztfquery/data/ztf_ccd_layout.tbl
--rw-r--r--   0 mrigault   (501) staff       (20)    95447 2018-12-04 14:02:54.000000 ztfquery-1.8.1/ztfquery/data/filter_p48_r.dat
--rw-r--r--   0 mrigault   (501) staff       (20)    52676 2018-12-04 14:02:43.000000 ztfquery-1.8.1/ztfquery/data/filter_p48_g.dat
--rw-r--r--   0 mrigault   (501) staff       (20)       52 2019-03-19 12:22:17.000000 ztfquery-1.8.1/ztfquery/photometry.py
--rw-r--r--   0 mrigault   (501) staff       (20)     2342 2019-08-31 10:12:44.000000 ztfquery-1.8.1/ztfquery/filters.py
--rwxr-xr-x   0 mrigault   (501) staff       (20)     7820 2019-08-22 12:54:04.000000 ztfquery-1.8.1/ztfquery/alert.py
--rw-r--r--   0 mrigault   (501) staff       (20)    24643 2019-07-08 12:38:48.000000 ztfquery-1.8.1/README.md
--rw-r--r--   0 mrigault   (501) staff       (20)     1863 2019-11-16 09:07:32.000000 ztfquery-1.8.1/setup.py
--rw-r--r--   0 mrigault   (501) staff       (20)       38 2019-11-16 09:13:33.000000 ztfquery-1.8.1/setup.cfg
+drwxr-xr-x   0 mrigault   (501) staff       (20)        0 2020-03-26 12:59:30.000000 ztfquery-1.8.4/
+-rw-r--r--   0 mrigault   (501) staff       (20)      794 2020-03-26 12:59:30.000000 ztfquery-1.8.4/PKG-INFO
+drwxr-xr-x   0 mrigault   (501) staff       (20)        0 2020-03-26 12:59:30.000000 ztfquery-1.8.4/ztfquery.egg-info/
+-rw-r--r--   0 mrigault   (501) staff       (20)      794 2020-03-26 12:59:30.000000 ztfquery-1.8.4/ztfquery.egg-info/PKG-INFO
+-rw-r--r--   0 mrigault   (501) staff       (20)      709 2020-03-26 12:59:30.000000 ztfquery-1.8.4/ztfquery.egg-info/SOURCES.txt
+-rw-r--r--   0 mrigault   (501) staff       (20)        9 2020-03-26 12:59:30.000000 ztfquery-1.8.4/ztfquery.egg-info/top_level.txt
+-rw-r--r--   0 mrigault   (501) staff       (20)        1 2020-03-26 12:59:30.000000 ztfquery-1.8.4/ztfquery.egg-info/dependency_links.txt
+drwxr-xr-x   0 mrigault   (501) staff       (20)        0 2020-03-26 12:59:30.000000 ztfquery-1.8.4/ztfquery/
+-rw-r--r--   0 mrigault   (501) staff       (20)    32969 2019-09-12 10:12:54.000000 ztfquery-1.8.4/ztfquery/marshal.py
+-rw-r--r--   0 mrigault   (501) staff       (20)    15095 2019-06-12 16:17:00.000000 ztfquery-1.8.4/ztfquery/lightcurve.py
+-rw-r--r--   0 mrigault   (501) staff       (20)    12010 2019-11-16 08:55:41.000000 ztfquery-1.8.4/ztfquery/fields.py
+-rw-r--r--   0 mrigault   (501) staff       (20)    42868 2020-03-19 11:19:26.000000 ztfquery-1.8.4/ztfquery/query.py
+-rw-r--r--   0 mrigault   (501) staff       (20)    22995 2019-09-26 10:36:15.000000 ztfquery-1.8.4/ztfquery/sedm.py
+-rw-r--r--   0 mrigault   (501) staff       (20)     9954 2020-03-19 11:17:08.000000 ztfquery-1.8.4/ztfquery/buildurl.py
+-rw-r--r--   0 mrigault   (501) staff       (20)    13496 2019-06-12 09:47:51.000000 ztfquery-1.8.4/ztfquery/metasearch.py
+-rw-r--r--   0 mrigault   (501) staff       (20)    17705 2020-02-04 14:29:11.000000 ztfquery-1.8.4/ztfquery/io.py
+-rw-r--r--   0 mrigault   (501) staff       (20)       90 2020-03-26 12:58:07.000000 ztfquery-1.8.4/ztfquery/__init__.py
+drwxr-xr-x   0 mrigault   (501) staff       (20)        0 2020-03-26 12:59:30.000000 ztfquery-1.8.4/ztfquery/utils/
+-rw-r--r--   0 mrigault   (501) staff       (20)     6469 2018-06-06 14:57:27.000000 ztfquery-1.8.4/ztfquery/utils/tools.py
+-rw-r--r--   0 mrigault   (501) staff       (20)        3 2018-06-06 14:42:22.000000 ztfquery-1.8.4/ztfquery/utils/__init__.py
+-rw-r--r--   0 mrigault   (501) staff       (20)     2964 2018-06-13 08:06:06.000000 ztfquery-1.8.4/ztfquery/utils/stamps.py
+-rw-r--r--   0 mrigault   (501) staff       (20)    28386 2018-08-10 10:43:19.000000 ztfquery-1.8.4/ztfquery/query2.py
+-rw-r--r--   0 mrigault   (501) staff       (20)     3319 2019-08-07 17:37:49.000000 ztfquery-1.8.4/ztfquery/ccd.py
+drwxr-xr-x   0 mrigault   (501) staff       (20)        0 2020-03-26 12:59:30.000000 ztfquery-1.8.4/ztfquery/data/
+-rw-r--r--   0 mrigault   (501) staff       (20)    28668 2018-12-04 14:02:48.000000 ztfquery-1.8.4/ztfquery/data/filter_p48_i.dat
+-rw-r--r--   0 mrigault   (501) staff       (20)       12 2018-04-23 15:10:31.000000 ztfquery-1.8.4/ztfquery/data/source
+-rw-r--r--   0 mrigault   (501) staff       (20)     6230 2019-08-07 15:49:45.000000 ztfquery-1.8.4/ztfquery/data/ztf_ccd_quad_layout.tbl
+-rw-r--r--   0 mrigault   (501) staff       (20)   123299 2018-04-29 13:32:13.000000 ztfquery-1.8.4/ztfquery/data/ztf_fields.txt
+-rw-r--r--   0 mrigault   (501) staff       (20)     1419 2018-04-29 15:10:54.000000 ztfquery-1.8.4/ztfquery/data/ztf_ccd_layout.tbl
+-rw-r--r--   0 mrigault   (501) staff       (20)    95447 2018-12-04 14:02:54.000000 ztfquery-1.8.4/ztfquery/data/filter_p48_r.dat
+-rw-r--r--   0 mrigault   (501) staff       (20)    52676 2018-12-04 14:02:43.000000 ztfquery-1.8.4/ztfquery/data/filter_p48_g.dat
+-rw-r--r--   0 mrigault   (501) staff       (20)       52 2019-03-19 12:22:17.000000 ztfquery-1.8.4/ztfquery/photometry.py
+-rw-r--r--   0 mrigault   (501) staff       (20)     2342 2019-08-31 10:12:44.000000 ztfquery-1.8.4/ztfquery/filters.py
+-rwxr-xr-x   0 mrigault   (501) staff       (20)     7820 2019-08-22 12:54:04.000000 ztfquery-1.8.4/ztfquery/alert.py
+-rw-r--r--   0 mrigault   (501) staff       (20)    24643 2019-07-08 12:38:48.000000 ztfquery-1.8.4/README.md
+-rw-r--r--   0 mrigault   (501) staff       (20)     1863 2020-03-26 12:58:00.000000 ztfquery-1.8.4/setup.py
+-rw-r--r--   0 mrigault   (501) staff       (20)       38 2020-03-26 12:59:30.000000 ztfquery-1.8.4/setup.cfg
```

### Comparing `ztfquery-1.8.1/PKG-INFO` & `ztfquery-1.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ztfquery
-Version: 1.8.1
+Version: 1.8.4
 Summary: access ZTF data from python 
 Home-page: https://github.com/MickaelRigault/ztfquery
 Author: Mickael Rigault
 Author-email: m.rigault@ipnl.in2p3.fr
 Maintainer: Mickael Rigault
 Maintainer-email: m.rigault@ipnl.in2p3.fr
 License: BSD (3-clause)
```

### Comparing `ztfquery-1.8.1/ztfquery.egg-info/PKG-INFO` & `ztfquery-1.8.4/ztfquery.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ztfquery
-Version: 1.8.1
+Version: 1.8.4
 Summary: access ZTF data from python 
 Home-page: https://github.com/MickaelRigault/ztfquery
 Author: Mickael Rigault
 Author-email: m.rigault@ipnl.in2p3.fr
 Maintainer: Mickael Rigault
 Maintainer-email: m.rigault@ipnl.in2p3.fr
 License: BSD (3-clause)
```

### Comparing `ztfquery-1.8.1/ztfquery.egg-info/SOURCES.txt` & `ztfquery-1.8.4/ztfquery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ztfquery-1.8.1/ztfquery/marshal.py` & `ztfquery-1.8.4/ztfquery/marshal.py`

 * *Files identical despite different names*

### Comparing `ztfquery-1.8.1/ztfquery/lightcurve.py` & `ztfquery-1.8.4/ztfquery/lightcurve.py`

 * *Files identical despite different names*

### Comparing `ztfquery-1.8.1/ztfquery/fields.py` & `ztfquery-1.8.4/ztfquery/fields.py`

 * *Files identical despite different names*

### Comparing `ztfquery-1.8.1/ztfquery/query.py` & `ztfquery-1.8.4/ztfquery/query.py`

 * *Files 14% similar despite different names*

```diff
@@ -246,15 +246,18 @@
 
     
     # Generic that should automatically work as long as get_data_path is defined.
     def download_data(self, suffix=None, source="IRSA", indexes=None,
                      download_dir=None,
                      show_progress = True, notebook=False, verbose=True,
                      nodl = False, overwrite=False, nprocess=None,
-                     auth=None, **kwargs):
+                     auth=None,
+                     filecheck=True, erasebad=True, redownload=True,
+                     ignore_warnings=False,
+                     **kwargs):
         """ 
         Parameters
         ----------
         suffix: [string] -optional-
             What kind of data do you want? 
             Here is the list of available options depending on you image kind:
         
@@ -299,14 +302,26 @@
         nprocess: [None/int] -optional-
             Number of parallel downloading you want to do. 
             If None, it will be set to 1 and will not use multiprocess
 
         auth: [str, str] -optional-
             [username, password] of you IRSA account.
             If used, information stored in ~/.ztfquery will be ignored.
+        
+        //  File check
+
+        filecheck: [bool] -optional-
+            Shall this check if the downloaded data actually works ?
+
+        erasebad: [bool] -optional-
+            Do you want to remove from your local directory the corrupted files ?
+
+        redownload: [bool] -optional-
+            Shall corrupted file be automatically re downloaded ?
+            (Only works for IRSA files ('/sci/','/raw/', '/ref/', '/cal/')
 
         """
         # login
         if auth is not None:
             from .io import get_cookie
             cookie = get_cookie(*auth)
         else:
@@ -326,22 +341,34 @@
             self.download_location   = [download_dir + "/%s"%(d_.split("/")[-1])
                                         for d_ in self._relative_data_path]
             
         if nodl:
             return self.to_download_urls, self.download_location
         
         # Actual Download
-        io.download_url(self.to_download_urls, self.download_location,
+        with warnings.catch_warnings():
+            if ignore_warnings:
+                warnings.simplefilter("ignore")
+            io.download_url(self.to_download_urls, self.download_location,
                         show_progress = show_progress, notebook=notebook, verbose=verbose,
-                        overwrite=overwrite, nprocess=nprocess, cookies=cookie)
+                        overwrite=overwrite, nprocess=nprocess, cookies=cookie,
+                        filecheck=False)
+
+        if filecheck:
+            fileissue = io.test_files(self.download_location, erasebad=erasebad, redownload=True, nprocess=nprocess)
+            if fileissue is not None and len(fileissue) > 0:
+                warnings.warn("%d file failed (returned)"%len(fileissue))
+                
                 
     # --------- #
     #  GETTER   #
     # --------- #
-    def get_local_data(self, suffix=None, exists=True, indexes=None):
+    def get_local_data(self, suffix=None, exists=True, filecheck=True, indexes=None,
+                           badfiles=False, source="local",
+                           ignore_warnings=False, **kwargs):
         """ the lists of files stored in your local copy of the ztf database.
         [This methods uses the get_data_path() method assuming source='local']
 
         Parameters
         ----------
         suffix: [string] -optional-
             What kind of data do you want? 
@@ -378,23 +405,179 @@
             - unc:            returns `caltype`unc.fits
 
         exists: [bool] -optional-
             returns only the file that exists in your computer. 
             If false, this will return the expected path of the requested data, 
             even though they might not exist.
 
+
+        source: [str] -optional-
+            Where are the data stored ? 
+            default is 'local' this will use you $ZTFDATA path. 
+            You can also directly provide here where the IRSA data structure starts.
         Returns
         -------
         list
         """
-        files = self.get_data_path(suffix=suffix, source="local", indexes=indexes)
+        files = self.get_data_path(suffix=suffix, source=source, indexes=indexes)
         if not exists:
             return files
-        return [f for f in files if os.path.isfile( f )]
 
+        localfile = [f for f in files if os.path.isfile( f )]
+        if filecheck or badfiles or kwargs.get("redownload",False):
+            with warnings.catch_warnings():
+                if ignore_warnings:
+                    warnings.simplefilter("ignore")
+                badfiles_ = io.test_files(localfile, erasebad=False, **kwargs)
+                
+            if badfiles:
+                return badfiles_
+            elif badfiles_ is not None and len(badfiles_)>1:
+                return [f for f in localfile if f not in badfiles_]
+        return localfile
+
+    def get_missing_data_index(self, suffix=None, which="any"):
+        """ 
+        Parameters
+        ----------
+        suffix: [string] -optional-
+            What kind of data do you want? 
+            Here is the list of available options depending on you image kind:
+        
+            # Science image (kind="sci"):
+            - sciimg.fits (primary science image) # (default)
+            - mskimg.fits (bit-mask image)
+            - psfcat.fits (PSF-fit photometry catalog)
+            - sexcat.fits (nested-aperture photometry catalog)
+            - sciimgdao.psf (spatially varying PSF estimate in DAOPhot's lookup table format)
+            - sciimgdaopsfcent.fits (PSF estimate at science image center as a FITS image)
+            - sciimlog.txt (log output from instrumental calibration pipeline)
+            - scimrefdiffimg.fits.fz (difference image: science minus reference; fpack-compressed)
+            - diffimgpsf.fits (PSF estimate for difference image as a FITS image)
+            - diffimlog.txt (log output from image subtraction and extraction pipeline)
+            - log.txt (overall system summary log from realtime pipeline)
+            
+            # Reference image (kind="ref"):
+            -log.txt
+            -refcov.fits
+            -refimg.fits # (default)
+            -refimlog.txt
+            -refpsfcat.fits
+            -refsexcat.fits
+            -refunc.fits
+
+            # Raw images (kind="raw")
+            No Choice so suffix is ignored for raw data
+            
+            # Calibration (kind="cal")
+            - None (#default) returns `caltype`.fits
+            - log:            returns `caltype`log.txt
+            - unc:            returns `caltype`unc.fits
+
+
+        which: [string] -optional-
+            Which missing data are you looking for:
+            - any/all: missing because bad local files or because not downloaded yet.
+            - bad/corrupted: missing because the local files are corrupted
+            - notdl/dl/nodl: missing because not downloaded. 
+
+        Returns
+        -------
+        list of self.metadata indexes
+        """
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")
+            if which in ["all", "any"]:
+                all_local = self.get_data_path(suffix ,source="local")
+                actual_local = self.get_local_data(suffix, exists=True, filecheck=True)            
+            elif which in ["bad", "corrupted"]:
+                all_local = self.get_local_data(suffix, exists=True, filecheck=False)
+                actual_local = self.get_local_data(suffix, exists=True, filecheck=True)
+            elif which in ["notdl", "dl","nodl"]:
+                all_local = self.get_data_path(suffix ,source="local")
+                actual_local = self.get_local_data(suffix, exists=False, filecheck=False)
+            else:
+                raise ValueError("cannot parse which %s: any, bad, notdl available"%which)
+
+        id_ = [i for i,f in enumerate(all_local) if f not in actual_local]
+        return self.metatable.index[id_]
+        
+    def purge_corrupted_local_data(self, suffix=None, erasebad=False, redownload=False,
+                                       indexes=None, verbose=True,
+                                       nprocess=4, **kwargs):
+        """ 
+        Parameters
+        ----------
+        suffix: [string] -optional-
+            What kind of data do you want? 
+            Here is the list of available options depending on you image kind:
+        
+            # Science image (kind="sci"):
+            - sciimg.fits (primary science image) # (default)
+            - mskimg.fits (bit-mask image)
+            - psfcat.fits (PSF-fit photometry catalog)
+            - sexcat.fits (nested-aperture photometry catalog)
+            - sciimgdao.psf (spatially varying PSF estimate in DAOPhot's lookup table format)
+            - sciimgdaopsfcent.fits (PSF estimate at science image center as a FITS image)
+            - sciimlog.txt (log output from instrumental calibration pipeline)
+            - scimrefdiffimg.fits.fz (difference image: science minus reference; fpack-compressed)
+            - diffimgpsf.fits (PSF estimate for difference image as a FITS image)
+            - diffimlog.txt (log output from image subtraction and extraction pipeline)
+            - log.txt (overall system summary log from realtime pipeline)
+            
+            # Reference image (kind="ref"):
+            -log.txt
+            -refcov.fits
+            -refimg.fits # (default)
+            -refimlog.txt
+            -refpsfcat.fits
+            -refsexcat.fits
+            -refunc.fits
+
+            # Raw images (kind="raw")
+            No Choice so suffix is ignored for raw data
+            
+            # Calibration (kind="cal")
+            - None (#default) returns `caltype`.fits
+            - log:            returns `caltype`log.txt
+            - unc:            returns `caltype`unc.fits
+
+
+        erasebad: [bool] -optional-
+            Do you want to remove from your local directory the corrupted files ?
+        
+        redownload: [bool] -optional-
+            Shall corrupted file be automatically re downloaded ?
+            (Only works for IRSA files ('/sci/','/raw/', '/ref/', '/cal/')
+
+        Returns
+        -------
+        list of files
+        """
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")
+            badfiles = self.get_local_data(suffix=suffix, exists=True, filecheck=True, indexes=indexes, badfiles=True,
+                                            redownload=redownload, nprocess=nprocess, **kwargs)
+
+        if badfiles is None or len(badfiles)==0:
+            return None
+        
+        if erasebad and not redownload:
+            if verbose:
+                print("Removing %d files"%len(badfiles))
+            for file_ in badfiles:
+                os.remove(file_)
+        elif redownload:
+            if verbose:
+                print("%d files have been redownloaded"%len(badfiles))
+        else:
+            if verbose:
+                print("%d files to be removed (run this with erasebad=True)"%len(badfiles))
+                
+        return badfiles
 
     
 class ZTFQuery( _ZTFTableHandler_, _ZTFDownloader_ ):
     """ """
     # ------------ #
     #  DOWNLOADER  #
     # ------------ #
@@ -709,15 +892,15 @@
         self._metadata = DEFAULT[kind]
         self._metadata["kind"] = kind
         for k,v in kwargs.items():
             self._metadata[k] = v
         # -> python3    self._metadata = **{DEFAULT[kind], **kwargs}; self._metadata["kind"] = kind
             
     # WRONG SO FAR
-    def get_data_path(self, mask=None, suffix=None, source=None, verbose=False, ):
+    def get_data_path(self, mask=None, suffix=None, source=None, verbose=False, indexes=None):
         """ generic method to build the url/fullpath or the requested data.
         This method is based on the `builurl.py` module of ztfquery.
         
         Parameters
         ----------
         mask: [None / list of int / boolean array] -optional-
            only use the data entry for the given mask:
```

### Comparing `ztfquery-1.8.1/ztfquery/sedm.py` & `ztfquery-1.8.4/ztfquery/sedm.py`

 * *Files identical despite different names*

### Comparing `ztfquery-1.8.1/ztfquery/buildurl.py` & `ztfquery-1.8.4/ztfquery/buildurl.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 #
 
 
 """ Library to convert 'meta' information into URL assuming: 
 https://irsa.ipac.caltech.edu/docs/program_interface/ztf_metadata.html
 """
 import os
-
+import warnings
+import numpy as np
 # ========================== #
 #                            #
 #   Generic Query            #
 #                            #
 # ========================== #
 
 KNOWN_SCIENCE_SUFFIXES = {    "sciimg.fits":"(primary science image)",
@@ -23,30 +24,44 @@
                       "scimrefdiffimg.fits.fz":"(difference image: science minus reference; fpack-compressed)",
                       "diffimgpsf.fits":"(PSF estimate for difference image as a FITS image)",
                       "diffimlog.txt":"(log output from image subtraction and extraction pipeline)",
                       "log.txt":"(overall system summary log from realtime pipeline)"}
 
 # SOURCES 
 DATA_BASEURL   = "https://irsa.ipac.caltech.edu/ibe/data/ztf/products/"
+ZTFIRSA_BASE = ["/ref/","/sci/","/raw/","/cal/"]
+
 from .io import LOCALSOURCE
 DEFAULT_SOURCE = DATA_BASEURL
 
 
 # ================== #
 #  Building the URL  #
 # ================== #
+def _localsource_to_source_(localfilepath, source=None):
+    """ """
+    filesource = _source_to_location_(source)
+    if LOCALSOURCE not in localfilepath:
+        raise ValueError("Cannot parse the location of the given file. %s, %s expected to be part of the path"%(localfilepath,LOCALSOURCE))
+
+    if np.any([k in localfilepath for k in ZTFIRSA_BASE]):
+        return localfilepath.replace(LOCALSOURCE, filesource), "irsa"
+    else:
+        warnings.warn("Cannot recover the online url, only IRSA ZTF files are implemented.")
+        return None, "None"
+    
 def _source_to_location_(source):
     """ convert flexible source naming into actual source path """
     if source is None: source = "irsa"
     source = source.lower()
 
     if source in ["none"]:
         return ""
     
-    if source in [DATA_BASEURL, LOCALSOURCE]:
+    if source in [DATA_BASEURL, LOCALSOURCE] or "/" in source:
         return source
     
     if source in ['irsa', 'ipac', "web", "online", "ztf"]:
         return DEFAULT_SOURCE
         
     if source in ["local", "cmp", "computer"]:
         return LOCALSOURCE
```

### Comparing `ztfquery-1.8.1/ztfquery/metasearch.py` & `ztfquery-1.8.4/ztfquery/metasearch.py`

 * *Files identical despite different names*

### Comparing `ztfquery-1.8.1/ztfquery/utils/tools.py` & `ztfquery-1.8.4/ztfquery/utils/tools.py`

 * *Files identical despite different names*

### Comparing `ztfquery-1.8.1/ztfquery/utils/stamps.py` & `ztfquery-1.8.4/ztfquery/utils/stamps.py`

 * *Files identical despite different names*

### Comparing `ztfquery-1.8.1/ztfquery/query2.py` & `ztfquery-1.8.4/ztfquery/query2.py`

 * *Files identical despite different names*

### Comparing `ztfquery-1.8.1/ztfquery/ccd.py` & `ztfquery-1.8.4/ztfquery/ccd.py`

 * *Files identical despite different names*

### Comparing `ztfquery-1.8.1/ztfquery/data/filter_p48_i.dat` & `ztfquery-1.8.4/ztfquery/data/filter_p48_i.dat`

 * *Files identical despite different names*

### Comparing `ztfquery-1.8.1/ztfquery/data/ztf_ccd_quad_layout.tbl` & `ztfquery-1.8.4/ztfquery/data/ztf_ccd_quad_layout.tbl`

 * *Files identical despite different names*

### Comparing `ztfquery-1.8.1/ztfquery/data/ztf_fields.txt` & `ztfquery-1.8.4/ztfquery/data/ztf_fields.txt`

 * *Files identical despite different names*

### Comparing `ztfquery-1.8.1/ztfquery/data/ztf_ccd_layout.tbl` & `ztfquery-1.8.4/ztfquery/data/ztf_ccd_layout.tbl`

 * *Files identical despite different names*

### Comparing `ztfquery-1.8.1/ztfquery/data/filter_p48_r.dat` & `ztfquery-1.8.4/ztfquery/data/filter_p48_r.dat`

 * *Files identical despite different names*

### Comparing `ztfquery-1.8.1/ztfquery/data/filter_p48_g.dat` & `ztfquery-1.8.4/ztfquery/data/filter_p48_g.dat`

 * *Files identical despite different names*

### Comparing `ztfquery-1.8.1/ztfquery/filters.py` & `ztfquery-1.8.4/ztfquery/filters.py`

 * *Files identical despite different names*

### Comparing `ztfquery-1.8.1/ztfquery/alert.py` & `ztfquery-1.8.4/ztfquery/alert.py`

 * *Files identical despite different names*

### Comparing `ztfquery-1.8.1/README.md` & `ztfquery-1.8.4/README.md`

 * *Files identical despite different names*

### Comparing `ztfquery-1.8.1/setup.py` & `ztfquery-1.8.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 DISTNAME = 'ztfquery'
 AUTHOR = 'Mickael Rigault'
 MAINTAINER = 'Mickael Rigault' 
 MAINTAINER_EMAIL = 'm.rigault@ipnl.in2p3.fr'
 URL = 'https://github.com/MickaelRigault/ztfquery'
 LICENSE = 'BSD (3-clause)'
 DOWNLOAD_URL = 'https://github.com/MickaelRigault/ztfquery/tarball/1.8'
-VERSION = '1.8.1'
+VERSION = '1.8.4'
 
 try:
     from setuptools import setup, find_packages
     _has_setuptools = True
 except ImportError:
     from distutils.core import setup
     _has_setuptools = False
```

