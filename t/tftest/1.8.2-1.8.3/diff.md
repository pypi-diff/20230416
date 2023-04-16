# Comparing `tmp/tftest-1.8.2.tar.gz` & `tmp/tftest-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tftest-1.8.2.tar", last modified: Thu Jan 26 11:18:39 2023, max compression
+gzip compressed data, was "tftest-1.8.3.tar", last modified: Sun Apr 16 10:11:46 2023, max compression
```

## Comparing `tftest-1.8.2.tar` & `tftest-1.8.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 ludomagno  (1000) ludomagno  (1000)        0 2023-01-26 11:18:39.525570 tftest-1.8.2/
--rw-r--r--   0 ludomagno  (1000) ludomagno  (1000)    11358 2019-03-22 10:16:40.000000 tftest-1.8.2/LICENSE
--rw-r--r--   0 ludomagno  (1000) ludomagno  (1000)     6345 2023-01-26 11:18:39.524569 tftest-1.8.2/PKG-INFO
--rw-r--r--   0 ludomagno  (1000) ludomagno  (1000)     5888 2022-11-02 06:43:54.000000 tftest-1.8.2/README.md
--rw-r--r--   0 ludomagno  (1000) ludomagno  (1000)       38 2023-01-26 11:18:39.525570 tftest-1.8.2/setup.cfg
--rw-r-----   0 ludomagno  (1000) ludomagno  (1000)     1331 2022-10-02 16:38:55.000000 tftest-1.8.2/setup.py
-drwxr-xr-x   0 ludomagno  (1000) ludomagno  (1000)        0 2023-01-26 11:18:39.524569 tftest-1.8.2/test/
--rw-r--r--   0 ludomagno  (1000) ludomagno  (1000)     5036 2023-01-26 11:01:12.000000 tftest-1.8.2/test/test_args.py
--rw-r-----   0 ludomagno  (1000) ludomagno  (1000)      989 2022-05-03 17:38:56.000000 tftest-1.8.2/test/test_backend_config.py
--rw-r--r--   0 ludomagno  (1000) ludomagno  (1000)     6280 2022-11-09 06:41:18.000000 tftest-1.8.2/test/test_cache.py
--rw-r-----   0 ludomagno  (1000) ludomagno  (1000)     1150 2022-05-03 17:45:33.000000 tftest-1.8.2/test/test_files.py
--rw-r-----   0 ludomagno  (1000) ludomagno  (1000)     1322 2022-05-03 17:38:59.000000 tftest-1.8.2/test/test_no_outputs.py
--rw-r-----   0 ludomagno  (1000) ludomagno  (1000)     1505 2022-09-15 05:23:54.000000 tftest-1.8.2/test/test_pickle.py
--rw-r-----   0 ludomagno  (1000) ludomagno  (1000)     2663 2022-08-04 06:30:41.000000 tftest-1.8.2/test/test_plan.py
--rw-r-----   0 ludomagno  (1000) ludomagno  (1000)     2246 2022-05-03 17:45:33.000000 tftest-1.8.2/test/test_prevent_destroy.py
--rw-r-----   0 ludomagno  (1000) ludomagno  (1000)     1002 2022-05-03 17:39:03.000000 tftest-1.8.2/test/test_sample_apply.py
--rw-r-----   0 ludomagno  (1000) ludomagno  (1000)     1344 2022-05-03 17:39:05.000000 tftest-1.8.2/test/test_sample_plan.py
--rw-r-----   0 ludomagno  (1000) ludomagno  (1000)      993 2022-08-04 10:45:46.000000 tftest-1.8.2/test/test_sample_plan_error.py
--rw-r-----   0 ludomagno  (1000) ludomagno  (1000)      925 2022-05-03 17:39:04.000000 tftest-1.8.2/test/test_sample_plan_no_variables.py
--rw-r-----   0 ludomagno  (1000) ludomagno  (1000)     1181 2022-05-03 17:39:06.000000 tftest-1.8.2/test/test_state.py
--rw-r-----   0 ludomagno  (1000) ludomagno  (1000)     2784 2022-05-03 17:45:33.000000 tftest-1.8.2/test/test_tg_all.py
--rw-r-----   0 ludomagno  (1000) ludomagno  (1000)     1005 2022-05-03 17:39:09.000000 tftest-1.8.2/test/test_value_dict.py
--rw-r-----   0 ludomagno  (1000) ludomagno  (1000)     1543 2022-07-11 12:25:59.000000 tftest-1.8.2/test/test_workspace.py
-drwxr-xr-x   0 ludomagno  (1000) ludomagno  (1000)        0 2023-01-26 11:18:39.524569 tftest-1.8.2/tftest.egg-info/
--rw-r--r--   0 ludomagno  (1000) ludomagno  (1000)     6345 2023-01-26 11:18:39.000000 tftest-1.8.2/tftest.egg-info/PKG-INFO
--rw-r--r--   0 ludomagno  (1000) ludomagno  (1000)      537 2023-01-26 11:18:39.000000 tftest-1.8.2/tftest.egg-info/SOURCES.txt
--rw-r--r--   0 ludomagno  (1000) ludomagno  (1000)        1 2023-01-26 11:18:39.000000 tftest-1.8.2/tftest.egg-info/dependency_links.txt
--rw-r--r--   0 ludomagno  (1000) ludomagno  (1000)        7 2023-01-26 11:18:39.000000 tftest-1.8.2/tftest.egg-info/top_level.txt
--rw-r--r--   0 ludomagno  (1000) ludomagno  (1000)    28361 2023-01-26 11:14:14.000000 tftest-1.8.2/tftest.py
+drwxr-xr-x   0 ludomagno  (1000) ludomagno  (1000)        0 2023-04-16 10:11:46.448596 tftest-1.8.3/
+-rw-r--r--   0 ludomagno  (1000) ludomagno  (1000)    11358 2019-03-22 10:16:40.000000 tftest-1.8.3/LICENSE
+-rw-r--r--   0 ludomagno  (1000) ludomagno  (1000)     6345 2023-04-16 10:11:46.448596 tftest-1.8.3/PKG-INFO
+-rw-r--r--   0 ludomagno  (1000) ludomagno  (1000)     5888 2022-11-02 06:43:54.000000 tftest-1.8.3/README.md
+-rw-r--r--   0 ludomagno  (1000) ludomagno  (1000)       38 2023-04-16 10:11:46.448596 tftest-1.8.3/setup.cfg
+-rw-r-----   0 ludomagno  (1000) ludomagno  (1000)     1331 2022-10-02 16:38:55.000000 tftest-1.8.3/setup.py
+drwxr-xr-x   0 ludomagno  (1000) ludomagno  (1000)        0 2023-04-16 10:11:46.447596 tftest-1.8.3/test/
+-rw-r--r--   0 ludomagno  (1000) ludomagno  (1000)     5036 2023-01-26 11:01:12.000000 tftest-1.8.3/test/test_args.py
+-rw-r-----   0 ludomagno  (1000) ludomagno  (1000)      989 2022-05-03 17:38:56.000000 tftest-1.8.3/test/test_backend_config.py
+-rw-r--r--   0 ludomagno  (1000) ludomagno  (1000)     6280 2022-11-09 06:41:18.000000 tftest-1.8.3/test/test_cache.py
+-rw-r-----   0 ludomagno  (1000) ludomagno  (1000)     1150 2022-05-03 17:45:33.000000 tftest-1.8.3/test/test_files.py
+-rw-r-----   0 ludomagno  (1000) ludomagno  (1000)     1322 2022-05-03 17:38:59.000000 tftest-1.8.3/test/test_no_outputs.py
+-rw-r-----   0 ludomagno  (1000) ludomagno  (1000)     1505 2022-09-15 05:23:54.000000 tftest-1.8.3/test/test_pickle.py
+-rw-r-----   0 ludomagno  (1000) ludomagno  (1000)     2663 2022-08-04 06:30:41.000000 tftest-1.8.3/test/test_plan.py
+-rw-r-----   0 ludomagno  (1000) ludomagno  (1000)     2246 2022-05-03 17:45:33.000000 tftest-1.8.3/test/test_prevent_destroy.py
+-rw-r-----   0 ludomagno  (1000) ludomagno  (1000)     1002 2022-05-03 17:39:03.000000 tftest-1.8.3/test/test_sample_apply.py
+-rw-r-----   0 ludomagno  (1000) ludomagno  (1000)     1344 2022-05-03 17:39:05.000000 tftest-1.8.3/test/test_sample_plan.py
+-rw-r-----   0 ludomagno  (1000) ludomagno  (1000)      993 2022-08-04 10:45:46.000000 tftest-1.8.3/test/test_sample_plan_error.py
+-rw-r-----   0 ludomagno  (1000) ludomagno  (1000)      925 2022-05-03 17:39:04.000000 tftest-1.8.3/test/test_sample_plan_no_variables.py
+-rw-r-----   0 ludomagno  (1000) ludomagno  (1000)     1181 2022-05-03 17:39:06.000000 tftest-1.8.3/test/test_state.py
+-rw-r-----   0 ludomagno  (1000) ludomagno  (1000)     2784 2022-05-03 17:45:33.000000 tftest-1.8.3/test/test_tg_all.py
+-rw-r-----   0 ludomagno  (1000) ludomagno  (1000)     1005 2022-05-03 17:39:09.000000 tftest-1.8.3/test/test_value_dict.py
+-rw-r-----   0 ludomagno  (1000) ludomagno  (1000)     1543 2022-07-11 12:25:59.000000 tftest-1.8.3/test/test_workspace.py
+drwxr-xr-x   0 ludomagno  (1000) ludomagno  (1000)        0 2023-04-16 10:11:46.448596 tftest-1.8.3/tftest.egg-info/
+-rw-r--r--   0 ludomagno  (1000) ludomagno  (1000)     6345 2023-04-16 10:11:46.000000 tftest-1.8.3/tftest.egg-info/PKG-INFO
+-rw-r--r--   0 ludomagno  (1000) ludomagno  (1000)      537 2023-04-16 10:11:46.000000 tftest-1.8.3/tftest.egg-info/SOURCES.txt
+-rw-r--r--   0 ludomagno  (1000) ludomagno  (1000)        1 2023-04-16 10:11:46.000000 tftest-1.8.3/tftest.egg-info/dependency_links.txt
+-rw-r--r--   0 ludomagno  (1000) ludomagno  (1000)        7 2023-04-16 10:11:46.000000 tftest-1.8.3/tftest.egg-info/top_level.txt
+-rw-r--r--   0 ludomagno  (1000) ludomagno  (1000)    28712 2023-04-16 10:07:35.000000 tftest-1.8.3/tftest.py
```

### Comparing `tftest-1.8.2/LICENSE` & `tftest-1.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tftest-1.8.2/PKG-INFO` & `tftest-1.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tftest
-Version: 1.8.2
+Version: 1.8.3
 Summary: Simple Terraform test helper
 Home-page: https://github.com/GoogleCloudPlatform/terraform-python-testing-helper
 Author: Ludovico Magnocavallo
 Author-email: ludomagno@google.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `tftest-1.8.2/README.md` & `tftest-1.8.3/README.md`

 * *Files identical despite different names*

### Comparing `tftest-1.8.2/setup.py` & `tftest-1.8.3/setup.py`

 * *Files identical despite different names*

### Comparing `tftest-1.8.2/test/test_args.py` & `tftest-1.8.3/test/test_args.py`

 * *Files identical despite different names*

### Comparing `tftest-1.8.2/test/test_backend_config.py` & `tftest-1.8.3/test/test_backend_config.py`

 * *Files identical despite different names*

### Comparing `tftest-1.8.2/test/test_cache.py` & `tftest-1.8.3/test/test_cache.py`

 * *Files identical despite different names*

### Comparing `tftest-1.8.2/test/test_files.py` & `tftest-1.8.3/test/test_files.py`

 * *Files identical despite different names*

### Comparing `tftest-1.8.2/test/test_no_outputs.py` & `tftest-1.8.3/test/test_no_outputs.py`

 * *Files identical despite different names*

### Comparing `tftest-1.8.2/test/test_pickle.py` & `tftest-1.8.3/test/test_pickle.py`

 * *Files identical despite different names*

### Comparing `tftest-1.8.2/test/test_plan.py` & `tftest-1.8.3/test/test_plan.py`

 * *Files identical despite different names*

### Comparing `tftest-1.8.2/test/test_prevent_destroy.py` & `tftest-1.8.3/test/test_prevent_destroy.py`

 * *Files identical despite different names*

### Comparing `tftest-1.8.2/test/test_sample_apply.py` & `tftest-1.8.3/test/test_sample_apply.py`

 * *Files identical despite different names*

### Comparing `tftest-1.8.2/test/test_sample_plan.py` & `tftest-1.8.3/test/test_sample_plan.py`

 * *Files identical despite different names*

### Comparing `tftest-1.8.2/test/test_sample_plan_error.py` & `tftest-1.8.3/test/test_sample_plan_error.py`

 * *Files identical despite different names*

### Comparing `tftest-1.8.2/test/test_sample_plan_no_variables.py` & `tftest-1.8.3/test/test_sample_plan_no_variables.py`

 * *Files identical despite different names*

### Comparing `tftest-1.8.2/test/test_state.py` & `tftest-1.8.3/test/test_state.py`

 * *Files identical despite different names*

### Comparing `tftest-1.8.2/test/test_tg_all.py` & `tftest-1.8.3/test/test_tg_all.py`

 * *Files identical despite different names*

### Comparing `tftest-1.8.2/test/test_value_dict.py` & `tftest-1.8.3/test/test_value_dict.py`

 * *Files identical despite different names*

### Comparing `tftest-1.8.2/test/test_workspace.py` & `tftest-1.8.3/test/test_workspace.py`

 * *Files identical despite different names*

### Comparing `tftest-1.8.2/tftest.egg-info/PKG-INFO` & `tftest-1.8.3/tftest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tftest
-Version: 1.8.2
+Version: 1.8.3
 Summary: Simple Terraform test helper
 Home-page: https://github.com/GoogleCloudPlatform/terraform-python-testing-helper
 Author: Ludovico Magnocavallo
 Author-email: ludomagno@google.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `tftest-1.8.2/tftest.egg-info/SOURCES.txt` & `tftest-1.8.3/tftest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tftest-1.8.2/tftest.py` & `tftest-1.8.3/tftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 import weakref
 
 from functools import partial
 from hashlib import sha1
 from pathlib import Path
 from typing import List
 
-__version__ = '1.8.2'
+__version__ = '1.8.3'
 
 _LOGGER = logging.getLogger('tftest')
 
 TerraformCommandOutput = collections.namedtuple('TerraformCommandOutput',
                                                 'retcode out err')
 
 TerraformStateResource = collections.namedtuple(
@@ -103,16 +103,15 @@
 
   cmd_args += [
       f'--terragrunt-{arg.replace("_", "-")}' for arg in _TG_BOOL_ARGS
       if kw.get(f"tg_{arg}")
   ]
   for arg in _TG_KV_ARGS:
     if kw.get(f"tg_{arg}"):
-      cmd_args += [f'--terragrunt-{arg.replace("_", "-")}',
-                   kw[f"tg_{arg}"]]
+      cmd_args += [f'--terragrunt-{arg.replace("_", "-")}', kw[f"tg_{arg}"]]
   if kw.get('tg_parallelism'):
     cmd_args.append(f'--terragrunt-parallelism {kw["tg_parallelism"]}')
   if isinstance(kw.get('tg_override_attr'), dict):
     cmd_args += [
         '--terragrunt-override-attr={}={}'.format(k, v)
         for k, v in kw.get('tg_override_attr').items()
     ]
@@ -131,29 +130,32 @@
     cmd_args.append('-json')
   if kw.get('lock') is False:
     cmd_args.append('-lock=false')
   if kw.get('plugin_dir'):
     cmd_args += ['-plugin-dir', kw['plugin_dir']]
   if kw.get('refresh') is False:
     cmd_args.append('-refresh=false')
+  if kw.get('state'):
+    cmd_args += ['-state', kw['state']]
   if kw.get('upgrade'):
     cmd_args.append('-upgrade')
   if isinstance(init_vars, dict):
     cmd_args += [
         '-backend-config={}={}'.format(k, v) for k, v in init_vars.items()
     ]
   elif isinstance(init_vars, str):
     cmd_args += ['-backend-config', '{}'.format(init_vars)]
   if tf_vars:
     cmd_args += list(
         itertools.chain.from_iterable(
             ("-var",
-             "{}={}".format(k, json.dumps(v) if isinstance(v, (dict, list)) else v))
-            for k, v in tf_vars.items()
-        ))
+             "{}={}".format(k,
+                            json.dumps(v) if isinstance(v, (dict,
+                                                            list)) else v))
+            for k, v in tf_vars.items()))
   if targets:
     cmd_args += [("-target={}".format(t)) for t in targets]
   if kw.get('tf_var_file'):
     tf_var_file = kw['tf_var_file']
     if isinstance(tf_var_file, (list, tuple)):
       cmd_args += ['-var-file={}'.format(v) for v in tf_var_file]
     else:
@@ -323,16 +325,15 @@
     self._basedir = basedir or os.getcwd()
     self.binary = binary
     self.tfdir = self._abspath(tfdir)
     self._env = env or {}
     self.env = os.environ.copy()
     self.tg_run_all = False
     self._plan_formatter = lambda out: TerraformPlanOutput(json.loads(out))
-    self._output_formatter = lambda out: TerraformValueDict(
-        json.loads(out))
+    self._output_formatter = lambda out: TerraformValueDict(json.loads(out))
     self.enable_cache = enable_cache
     if not cache_dir:
       self.cache_dir = Path(os.path.dirname(
           inspect.stack()[1].filename)) / ".tftest-cache"
     else:
       self.cache_dir = Path(cache_dir)
     if env is not None:
@@ -359,53 +360,52 @@
     path = os.path.join(tfdir, 'terraform.tfstate')
     if os.path.isfile(path):
       os.unlink(path)
     path = os.path.join(tfdir, '**', '.terragrunt-cache*')
     for tg_dir in glob.glob(path, recursive=True):
       if os.path.isdir(tg_dir):
         shutil.rmtree(tg_dir, onerror=remove_readonly)
-    _LOGGER.debug(
-        'Restoring original TF files after prevent destroy changes')
+    _LOGGER.debug('Restoring original TF files after prevent destroy changes')
     if restore_files:
       for bkp_file in Path(tfdir).rglob('*.bkp'):
         try:
-          shutil.copy(str(bkp_file),
-                      f'{str(bkp_file).strip(".bkp")}')
+          shutil.copy(str(bkp_file), f'{str(bkp_file).strip(".bkp")}')
         except (IOError, OSError):
           _LOGGER.exception(
               f'Unable to restore terraform file {bkp_file.resolve()}')
           raise TerraformTestError(
               f'Restore of terraform file ({bkp_file.resolve()}) failed')
         else:
           bkp_file.unlink(True)
 
   def _abspath(self, path):
     """Make relative path absolute from base dir."""
     return path if os.path.isabs(path) else os.path.join(self._basedir, path)
 
-  def _dirhash(self, directory, hash, ignore_hidden=False, exclude_directories=[], excluded_extensions=[]):
+  def _dirhash(self, directory, hash, ignore_hidden=False,
+               exclude_directories=[], excluded_extensions=[]):
     """Returns hash of directory's file contents"""
     assert Path(directory).is_dir()
     try:
-      dir_iter = sorted(Path(directory).iterdir(),
-                        key=lambda p: str(p).lower())
+      dir_iter = sorted(Path(directory).iterdir(), key=lambda p: str(p).lower())
     except FileNotFoundError:
       return hash
     for path in dir_iter:
       if path.is_file():
         if ignore_hidden and path.name.startswith("."):
           continue
         if path.suffix in excluded_extensions:
           continue
         with open(path, "rb") as f:
           for chunk in iter(lambda: f.read(4096), b""):
             hash.update(chunk)
       elif path.is_dir() and path.name not in exclude_directories:
         hash = self._dirhash(path, hash, ignore_hidden=ignore_hidden,
-                             exclude_directories=exclude_directories, excluded_extensions=excluded_extensions)
+                             exclude_directories=exclude_directories,
+                             excluded_extensions=excluded_extensions)
     return hash
 
   def generate_cache_hash(self, method_kwargs):
     """Returns a hash value using the instance's attributes and method keyword arguments"""
     params = {
         **{
             k: v for k, v in self.__dict__.items()
@@ -417,26 +417,31 @@
     }
 
     # creates hash of file contents
     for path_param in ["extra_files", "tf_var_file"]:
       if path_param in method_kwargs:
         if isinstance(method_kwargs[path_param], list):
           params[path_param] = [
-              sha1(open(fp, 'rb').read()).hexdigest() for fp in method_kwargs[path_param]]
+              sha1(open(fp, 'rb').read()).hexdigest()
+              for fp in method_kwargs[path_param]
+          ]
         else:
           params[path_param] = sha1(
               open(method_kwargs[path_param], 'rb').read()).hexdigest()
 
     # creates hash of all file content within tfdir
     # excludes .terraform/, hidden files, tfstate files from being used for hash
-    params["tfdir"] = self._dirhash(
-        self.tfdir, sha1(), ignore_hidden=True, exclude_directories=[".terraform"], excluded_extensions=['.backup', '.tfstate']).hexdigest()
-
-    return sha1(json.dumps(params, sort_keys=True,
-                           default=str).encode("cp037")).hexdigest() + ".pickle"
+    params["tfdir"] = self._dirhash(self.tfdir, sha1(), ignore_hidden=True,
+                                    exclude_directories=[".terraform"],
+                                    excluded_extensions=['.backup', '.tfstate'
+                                                        ]).hexdigest()
+
+    return sha1(
+        json.dumps(params, sort_keys=True,
+                   default=str).encode("cp037")).hexdigest() + ".pickle"
 
   def _cache(func):
 
     def cache(self, **kwargs):
       """
       Runs the tftest instance method or retreives the cache value if it exists
 
@@ -591,47 +596,48 @@
         if len(ws) > 0
     ]:
       cmd_args = ['new', name]
     return self.execute_command('workspace', *cmd_args).out
 
   @_cache
   def plan(self, input=False, color=False, refresh=True, tf_vars=None,
-           targets=None, output=False, tf_var_file=None, use_cache=False, **kw):
+           targets=None, output=False, tf_var_file=None, state=None,
+           use_cache=False, **kw):
     """
     Run Terraform plan command, optionally returning parsed plan output.
 
     Args:
       input: Ask for input for variables if not directly set.
       no_color: If specified, output won't contain any color.
       refresh: Update state prior to checking for differences.
       tf_vars: Dict of variables in the Terraform configuration.
       targets: List of resources to target. Operation will be limited to this resource
         and its dependencies
       output: Determines if output will be returned.
       tf_var_file: Path to terraform variable configuration file relative to `self.tfdir`.
+      state: Path to state file to use when reading the prior state snapshot.
     """
     cmd_args = parse_args(input=input, color=color, refresh=refresh,
                           tf_vars=tf_vars, targets=targets,
-                          tf_var_file=tf_var_file, **kw)
+                          tf_var_file=tf_var_file, state=state, **kw)
     if not output:
       return self.execute_command('plan', *cmd_args).out
     with tempfile.NamedTemporaryFile() as fp:
       fp.close()
     # for tg we need to specify a temp name that is relative for the output to go into each
     # of the .terragrunt-cache, then plan / show would work, otherwise it overwrites each other!
     temp_file = fp.name if len(self._tg_ra()) == 0 else os.path.basename(
         fp.name)
     cmd_args.append('-out={}'.format(temp_file))
     self.execute_command('plan', *cmd_args)
     result = self.execute_command('show', '-no-color', '-json', temp_file)
     try:
       return self._plan_formatter(result.out)
     except json.JSONDecodeError as e:
-      raise TerraformTestError(
-          'Error decoding plan output: {}'.format(e))
+      raise TerraformTestError('Error decoding plan output: {}'.format(e))
 
   @_cache
   def apply(self, input=False, color=False, auto_approve=True, tf_vars=None,
             targets=None, tf_var_file=None, use_cache=False, **kw):
     """
     Run Terraform apply command.
```

