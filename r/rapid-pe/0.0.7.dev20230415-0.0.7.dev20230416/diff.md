# Comparing `tmp/rapid_pe-0.0.7.dev20230415.tar.gz` & `tmp/rapid_pe-0.0.7.dev20230416.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapid_pe-0.0.7.dev20230415.tar", last modified: Sat Apr 15 05:03:33 2023, max compression
+gzip compressed data, was "rapid_pe-0.0.7.dev20230416.tar", last modified: Sun Apr 16 05:03:30 2023, max compression
```

## Comparing `rapid_pe-0.0.7.dev20230415.tar` & `rapid_pe-0.0.7.dev20230416.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 05:03:33.835948 rapid_pe-0.0.7.dev20230415/
--rw-rw-rw-   0 root         (0) root         (0)    18022 2023-04-10 05:03:08.000000 rapid_pe-0.0.7.dev20230415/COPYING
--rw-r--r--   0 root         (0) root         (0)     1366 2023-04-15 05:03:33.835948 rapid_pe-0.0.7.dev20230415/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      365 2023-04-10 05:03:08.000000 rapid_pe-0.0.7.dev20230415/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 05:03:33.828948 rapid_pe-0.0.7.dev20230415/bin/
--rw-rw-rw-   0 root         (0) root         (0)     8155 2023-04-10 05:03:08.000000 rapid_pe-0.0.7.dev20230415/bin/rapidpe_calculate_overlap
--rw-rw-rw-   0 root         (0) root         (0)    16683 2023-04-10 05:03:08.000000 rapid_pe-0.0.7.dev20230415/bin/rapidpe_compute_intrinsic_fisher
--rw-rw-rw-   0 root         (0) root         (0)    37924 2023-04-10 05:03:08.000000 rapid_pe-0.0.7.dev20230415/bin/rapidpe_compute_intrinsic_grid
--rw-rw-rw-   0 root         (0) root         (0)    12663 2023-04-10 05:03:08.000000 rapid_pe-0.0.7.dev20230415/bin/rapidpe_create_event_dag
--rw-rw-rw-   0 root         (0) root         (0)    26192 2023-04-10 05:03:08.000000 rapid_pe-0.0.7.dev20230415/bin/rapidpe_integrate_extrinsic_likelihood
--rw-rw-rw-   0 root         (0) root         (0)     5035 2023-04-10 05:03:08.000000 rapid_pe-0.0.7.dev20230415/bin/rapidpe_triangulation
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 05:03:33.833948 rapid_pe-0.0.7.dev20230415/rapid_pe/
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-04-10 05:03:08.000000 rapid_pe-0.0.7.dev20230415/rapid_pe/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    32921 2023-04-10 05:03:08.000000 rapid_pe-0.0.7.dev20230415/rapid_pe/amrlib.py
--rw-rw-rw-   0 root         (0) root         (0)    12507 2023-04-10 05:03:08.000000 rapid_pe-0.0.7.dev20230415/rapid_pe/common_cl.py
--rw-rw-rw-   0 root         (0) root         (0)    12397 2023-04-10 05:03:08.000000 rapid_pe-0.0.7.dev20230415/rapid_pe/dagutils.py
--rw-rw-rw-   0 root         (0) root         (0)    23687 2023-04-10 05:03:08.000000 rapid_pe-0.0.7.dev20230415/rapid_pe/effectiveFisher.py
--rw-rw-rw-   0 root         (0) root         (0)    20243 2023-04-10 05:03:08.000000 rapid_pe-0.0.7.dev20230415/rapid_pe/factored_likelihood.py
--rw-rw-rw-   0 root         (0) root         (0)    57880 2023-04-10 05:03:08.000000 rapid_pe-0.0.7.dev20230415/rapid_pe/lalsimutils.py
--rw-rw-rw-   0 root         (0) root         (0)    33626 2023-04-10 05:03:08.000000 rapid_pe-0.0.7.dev20230415/rapid_pe/mcsampler.py
--rw-rw-rw-   0 root         (0) root         (0)    11383 2023-04-10 05:03:08.000000 rapid_pe-0.0.7.dev20230415/rapid_pe/sph_harmonics.py
--rw-rw-rw-   0 root         (0) root         (0)    10345 2023-04-10 05:03:08.000000 rapid_pe-0.0.7.dev20230415/rapid_pe/statutils.py
--rw-rw-rw-   0 root         (0) root         (0)     1427 2023-04-10 05:03:08.000000 rapid_pe-0.0.7.dev20230415/rapid_pe/synchlib.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 05:03:33.835948 rapid_pe-0.0.7.dev20230415/rapid_pe/tests/
--rw-rw-rw-   0 root         (0) root         (0)       55 2023-04-10 05:03:08.000000 rapid_pe-0.0.7.dev20230415/rapid_pe/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      342 2023-04-10 05:03:08.000000 rapid_pe-0.0.7.dev20230415/rapid_pe/tests/test_common_cl.py
--rw-rw-rw-   0 root         (0) root         (0)    10349 2023-04-10 05:03:08.000000 rapid_pe-0.0.7.dev20230415/rapid_pe/xmlutils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 05:03:33.834948 rapid_pe-0.0.7.dev20230415/rapid_pe.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1366 2023-04-15 05:03:33.000000 rapid_pe-0.0.7.dev20230415/rapid_pe.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      724 2023-04-15 05:03:33.000000 rapid_pe-0.0.7.dev20230415/rapid_pe.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-15 05:03:33.000000 rapid_pe-0.0.7.dev20230415/rapid_pe.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      119 2023-04-15 05:03:33.000000 rapid_pe-0.0.7.dev20230415/rapid_pe.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-04-15 05:03:33.000000 rapid_pe-0.0.7.dev20230415/rapid_pe.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-15 05:03:33.835948 rapid_pe-0.0.7.dev20230415/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2966 2023-04-10 05:03:08.000000 rapid_pe-0.0.7.dev20230415/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 05:03:30.847900 rapid_pe-0.0.7.dev20230416/
+-rw-rw-rw-   0 root         (0) root         (0)    18022 2023-04-16 05:03:21.000000 rapid_pe-0.0.7.dev20230416/COPYING
+-rw-r--r--   0 root         (0) root         (0)     1366 2023-04-16 05:03:30.847900 rapid_pe-0.0.7.dev20230416/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      365 2023-04-16 05:03:21.000000 rapid_pe-0.0.7.dev20230416/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 05:03:30.845900 rapid_pe-0.0.7.dev20230416/bin/
+-rw-rw-rw-   0 root         (0) root         (0)     8155 2023-04-16 05:03:21.000000 rapid_pe-0.0.7.dev20230416/bin/rapidpe_calculate_overlap
+-rw-rw-rw-   0 root         (0) root         (0)    16683 2023-04-16 05:03:21.000000 rapid_pe-0.0.7.dev20230416/bin/rapidpe_compute_intrinsic_fisher
+-rw-rw-rw-   0 root         (0) root         (0)    37924 2023-04-16 05:03:21.000000 rapid_pe-0.0.7.dev20230416/bin/rapidpe_compute_intrinsic_grid
+-rw-rw-rw-   0 root         (0) root         (0)    12710 2023-04-16 05:03:21.000000 rapid_pe-0.0.7.dev20230416/bin/rapidpe_create_event_dag
+-rw-rw-rw-   0 root         (0) root         (0)    26192 2023-04-16 05:03:21.000000 rapid_pe-0.0.7.dev20230416/bin/rapidpe_integrate_extrinsic_likelihood
+-rw-rw-rw-   0 root         (0) root         (0)     5035 2023-04-16 05:03:21.000000 rapid_pe-0.0.7.dev20230416/bin/rapidpe_triangulation
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 05:03:30.846900 rapid_pe-0.0.7.dev20230416/rapid_pe/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-04-16 05:03:21.000000 rapid_pe-0.0.7.dev20230416/rapid_pe/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    32921 2023-04-16 05:03:21.000000 rapid_pe-0.0.7.dev20230416/rapid_pe/amrlib.py
+-rw-rw-rw-   0 root         (0) root         (0)    12507 2023-04-16 05:03:21.000000 rapid_pe-0.0.7.dev20230416/rapid_pe/common_cl.py
+-rw-rw-rw-   0 root         (0) root         (0)    12337 2023-04-16 05:03:21.000000 rapid_pe-0.0.7.dev20230416/rapid_pe/dagutils.py
+-rw-rw-rw-   0 root         (0) root         (0)    23687 2023-04-16 05:03:21.000000 rapid_pe-0.0.7.dev20230416/rapid_pe/effectiveFisher.py
+-rw-rw-rw-   0 root         (0) root         (0)    20243 2023-04-16 05:03:21.000000 rapid_pe-0.0.7.dev20230416/rapid_pe/factored_likelihood.py
+-rw-rw-rw-   0 root         (0) root         (0)    57880 2023-04-16 05:03:21.000000 rapid_pe-0.0.7.dev20230416/rapid_pe/lalsimutils.py
+-rw-rw-rw-   0 root         (0) root         (0)    33626 2023-04-16 05:03:21.000000 rapid_pe-0.0.7.dev20230416/rapid_pe/mcsampler.py
+-rw-rw-rw-   0 root         (0) root         (0)    11383 2023-04-16 05:03:21.000000 rapid_pe-0.0.7.dev20230416/rapid_pe/sph_harmonics.py
+-rw-rw-rw-   0 root         (0) root         (0)    10345 2023-04-16 05:03:21.000000 rapid_pe-0.0.7.dev20230416/rapid_pe/statutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1427 2023-04-16 05:03:21.000000 rapid_pe-0.0.7.dev20230416/rapid_pe/synchlib.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 05:03:30.847900 rapid_pe-0.0.7.dev20230416/rapid_pe/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       55 2023-04-16 05:03:21.000000 rapid_pe-0.0.7.dev20230416/rapid_pe/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      342 2023-04-16 05:03:21.000000 rapid_pe-0.0.7.dev20230416/rapid_pe/tests/test_common_cl.py
+-rw-rw-rw-   0 root         (0) root         (0)    10349 2023-04-16 05:03:21.000000 rapid_pe-0.0.7.dev20230416/rapid_pe/xmlutils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 05:03:30.847900 rapid_pe-0.0.7.dev20230416/rapid_pe.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1366 2023-04-16 05:03:30.000000 rapid_pe-0.0.7.dev20230416/rapid_pe.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      724 2023-04-16 05:03:30.000000 rapid_pe-0.0.7.dev20230416/rapid_pe.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 05:03:30.000000 rapid_pe-0.0.7.dev20230416/rapid_pe.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      119 2023-04-16 05:03:30.000000 rapid_pe-0.0.7.dev20230416/rapid_pe.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-04-16 05:03:30.000000 rapid_pe-0.0.7.dev20230416/rapid_pe.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-16 05:03:30.847900 rapid_pe-0.0.7.dev20230416/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2966 2023-04-16 05:03:21.000000 rapid_pe-0.0.7.dev20230416/setup.py
```

### Comparing `rapid_pe-0.0.7.dev20230415/COPYING` & `rapid_pe-0.0.7.dev20230416/COPYING`

 * *Files identical despite different names*

### Comparing `rapid_pe-0.0.7.dev20230415/PKG-INFO` & `rapid_pe-0.0.7.dev20230416/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapid_pe
-Version: 0.0.7.dev20230415
+Version: 0.0.7.dev20230416
 Summary: RapidPE: The original low-latency gravitational wave parameter estimation code.
 Home-page: https://git.ligo.org/rapidpe-rift/rapidpe/
 License: GPL-2+
 Project-URL: Bug Tracker, https://git.ligo.org/rapidpe-rift/rapidpe/-/issues/
 Project-URL: Source Code, https://git.ligo.org/rapidpe-rift/rapidpe/
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
```

### Comparing `rapid_pe-0.0.7.dev20230415/bin/rapidpe_calculate_overlap` & `rapid_pe-0.0.7.dev20230416/bin/rapidpe_calculate_overlap`

 * *Files identical despite different names*

### Comparing `rapid_pe-0.0.7.dev20230415/bin/rapidpe_compute_intrinsic_fisher` & `rapid_pe-0.0.7.dev20230416/bin/rapidpe_compute_intrinsic_fisher`

 * *Files identical despite different names*

### Comparing `rapid_pe-0.0.7.dev20230415/bin/rapidpe_compute_intrinsic_grid` & `rapid_pe-0.0.7.dev20230416/bin/rapidpe_compute_intrinsic_grid`

 * *Files identical despite different names*

### Comparing `rapid_pe-0.0.7.dev20230415/bin/rapidpe_create_event_dag` & `rapid_pe-0.0.7.dev20230416/bin/rapidpe_create_event_dag`

 * *Files 4% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 argp.add_argument("--write-eff-lambda", action="store_true", help="Use psi0 column of template bank XML as effective lambda point to calculate in DAG.")
 argp.add_argument("--write-deff-lambda", action="store_true", help="Use psi3 column of template bank XML as delta effective lambda point to calculate in DAG.")
 argp.add_argument("--condor-command", action="append", help="Append these condor commands to the submit files. Useful for account group information.")
 argp.add_argument("--accounting-group-user",default=None, help="accounting-group-user for condor")
 argp.add_argument("--exe-integrate-likelihood", default=None, help="This is executable to use to integrate the extrinsic likelihood per intrinsic grid point. It will default to the lalsuite rapidpe_integrate_extrinsic_likelihood.")
 argp.add_argument("--integration-args-dict", default="", help="Pass these options as the kwargs input of the integrate dag creation function. They will be set, without editing, as input to the integration exe. If you use this, it will not be possible to also pass other command line arguments to the integration executable via the create_event_dag command line.")
 argp.add_argument("--iteration-level", default=None, help="integer denoting the iteration level")
-
+argp.add_argument("--cProfile", action="store_true", help="if True, cProfile each ILE job.")
 
 for cat, val in MAXJOBS.items():
     optname = "--maxjobs-%s" % cat.lower().replace("_", "-")
     argp.add_argument(optname, type=int, default=MAXJOBS[cat], help="Set MAXJOBS in DAGs for category %s. Default is %s" % (cat, str(val)))
 
 # Options transferred to ILE
 common_cl.add_datasource_params(argp)
@@ -213,15 +213,15 @@
 ile_job_type.write_sub_file()
 
 
 
 with open(ile_sub_name,'r') as integrate_sub_file:
     integrate_subfile_content = integrate_sub_file.read()
 
-if 'cProfile' in ast.literal_eval(opts.integration_args_dict):
+if opts.cProfile:
     uniq_str = "$(cluster)-$(process)"
     cprofile_stats_file = os.path.join(opts.log_directory, f'cprofile_integrate-{uniq_str}')
     replacement_pattern = rf'\1 -m cProfile -o {cprofile_stats_file}-\3.out {exe} \2\3\4'
 else:
     replacement_pattern =  rf'\1 {exe} \2\3\4'
 
 replaced_integrate_subfile_content = re.sub(r'^(\s*arguments\s*=\s*\")(.*)(ILE_iteration_[0-9]+)(.*)$', replacement_pattern,integrate_subfile_content,flags = re.MULTILINE)
```

### Comparing `rapid_pe-0.0.7.dev20230415/bin/rapidpe_integrate_extrinsic_likelihood` & `rapid_pe-0.0.7.dev20230416/bin/rapidpe_integrate_extrinsic_likelihood`

 * *Files identical despite different names*

### Comparing `rapid_pe-0.0.7.dev20230415/bin/rapidpe_triangulation` & `rapid_pe-0.0.7.dev20230416/bin/rapidpe_triangulation`

 * *Files identical despite different names*

### Comparing `rapid_pe-0.0.7.dev20230415/rapid_pe/amrlib.py` & `rapid_pe-0.0.7.dev20230416/rapid_pe/amrlib.py`

 * *Files identical despite different names*

### Comparing `rapid_pe-0.0.7.dev20230415/rapid_pe/common_cl.py` & `rapid_pe-0.0.7.dev20230416/rapid_pe/common_cl.py`

 * *Files identical despite different names*

### Comparing `rapid_pe-0.0.7.dev20230415/rapid_pe/dagutils.py` & `rapid_pe-0.0.7.dev20230416/rapid_pe/dagutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,16 +105,14 @@
         ile_job.add_file_opt("output-file", "%s-%s.%s" % (ofname, uniq_str, ext))
         del kwargs["output-file"]
         #if kwargs.has_key("save-samples") and kwargs["save-samples"] == True:
         if "save-samples" in kwargs and kwargs["save-samples"] == True:
             ile_job.add_opt("save-samples", '')
             del kwargs["save-samples"]
 
-    if "cProfile" in kwargs:
-        del kwargs["cProfile"]
     del kwargs["iteration-level"]
     #
     # Add normal arguments
     # FIXME: Get valid options from a module
     #
     for opt, param in kwargs.items():
         if isinstance(param, list) or isinstance(param, tuple):
```

### Comparing `rapid_pe-0.0.7.dev20230415/rapid_pe/effectiveFisher.py` & `rapid_pe-0.0.7.dev20230416/rapid_pe/effectiveFisher.py`

 * *Files identical despite different names*

### Comparing `rapid_pe-0.0.7.dev20230415/rapid_pe/factored_likelihood.py` & `rapid_pe-0.0.7.dev20230416/rapid_pe/factored_likelihood.py`

 * *Files identical despite different names*

### Comparing `rapid_pe-0.0.7.dev20230415/rapid_pe/lalsimutils.py` & `rapid_pe-0.0.7.dev20230416/rapid_pe/lalsimutils.py`

 * *Files identical despite different names*

### Comparing `rapid_pe-0.0.7.dev20230415/rapid_pe/mcsampler.py` & `rapid_pe-0.0.7.dev20230416/rapid_pe/mcsampler.py`

 * *Files identical despite different names*

### Comparing `rapid_pe-0.0.7.dev20230415/rapid_pe/sph_harmonics.py` & `rapid_pe-0.0.7.dev20230416/rapid_pe/sph_harmonics.py`

 * *Files identical despite different names*

### Comparing `rapid_pe-0.0.7.dev20230415/rapid_pe/statutils.py` & `rapid_pe-0.0.7.dev20230416/rapid_pe/statutils.py`

 * *Files identical despite different names*

### Comparing `rapid_pe-0.0.7.dev20230415/rapid_pe/synchlib.py` & `rapid_pe-0.0.7.dev20230416/rapid_pe/synchlib.py`

 * *Files identical despite different names*

### Comparing `rapid_pe-0.0.7.dev20230415/rapid_pe/xmlutils.py` & `rapid_pe-0.0.7.dev20230416/rapid_pe/xmlutils.py`

 * *Files identical despite different names*

### Comparing `rapid_pe-0.0.7.dev20230415/rapid_pe.egg-info/PKG-INFO` & `rapid_pe-0.0.7.dev20230416/rapid_pe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapid-pe
-Version: 0.0.7.dev20230415
+Version: 0.0.7.dev20230416
 Summary: RapidPE: The original low-latency gravitational wave parameter estimation code.
 Home-page: https://git.ligo.org/rapidpe-rift/rapidpe/
 License: GPL-2+
 Project-URL: Bug Tracker, https://git.ligo.org/rapidpe-rift/rapidpe/-/issues/
 Project-URL: Source Code, https://git.ligo.org/rapidpe-rift/rapidpe/
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
```

### Comparing `rapid_pe-0.0.7.dev20230415/rapid_pe.egg-info/SOURCES.txt` & `rapid_pe-0.0.7.dev20230416/rapid_pe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rapid_pe-0.0.7.dev20230415/setup.py` & `rapid_pe-0.0.7.dev20230416/setup.py`

 * *Files identical despite different names*

