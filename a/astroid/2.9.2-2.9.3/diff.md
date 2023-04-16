# Comparing `tmp/astroid-2.9.2.tar.gz` & `tmp/astroid-2.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astroid-2.9.2.tar", last modified: Mon Jan  3 23:16:59 2022, max compression
+gzip compressed data, was "astroid-2.9.3.tar", last modified: Sun Jan  9 16:18:57 2022, max compression
```

## Comparing `astroid-2.9.2.tar` & `astroid-2.9.3.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 23:16:59.551513 astroid-2.9.2/
--rw-r--r--   0 runner    (1001) docker     (121)    26516 2022-01-03 23:16:49.000000 astroid-2.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      144 2022-01-03 23:16:49.000000 astroid-2.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4388 2022-01-03 23:16:59.551513 astroid-2.9.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 23:16:59.547513 astroid-2.9.2/astroid/
--rw-r--r--   0 runner    (1001) docker     (121)     4806 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1530 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/__pkginfo__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3484 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/_ast.py
--rw-r--r--   0 runner    (1001) docker     (121)    13365 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/arguments.py
--rw-r--r--   0 runner    (1001) docker     (121)      493 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/astroid_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)    21392 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/bases.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 23:16:59.551513 astroid-2.9.2/astroid/brain/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/brain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1114 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/brain/brain_argparse.py
--rw-r--r--   0 runner    (1001) docker     (121)     2682 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/brain/brain_attrs.py
--rw-r--r--   0 runner    (1001) docker     (121)      921 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/brain/brain_boto3.py
--rw-r--r--   0 runner    (1001) docker     (121)    31376 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/brain/brain_builtin_inference.py
--rw-r--r--   0 runner    (1001) docker     (121)     4822 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/brain/brain_collections.py
--rw-r--r--   0 runner    (1001) docker     (121)      967 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/brain/brain_crypt.py
--rw-r--r--   0 runner    (1001) docker     (121)     2426 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/brain/brain_ctypes.py
--rw-r--r--   0 runner    (1001) docker     (121)     3400 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/brain/brain_curses.py
--rw-r--r--   0 runner    (1001) docker     (121)    14886 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/brain/brain_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/brain/brain_dateutil.py
--rw-r--r--   0 runner    (1001) docker     (121)     2445 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/brain/brain_fstrings.py
--rw-r--r--   0 runner    (1001) docker     (121)     5759 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/brain/brain_functools.py
--rw-r--r--   0 runner    (1001) docker     (121)     8148 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/brain/brain_gi.py
--rw-r--r--   0 runner    (1001) docker     (121)     2459 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/brain/brain_hashlib.py
--rw-r--r--   0 runner    (1001) docker     (121)    10798 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/brain/brain_http.py
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/brain/brain_hypothesis.py
--rw-r--r--   0 runner    (1001) docker     (121)     1720 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/brain/brain_io.py
--rw-r--r--   0 runner    (1001) docker     (121)     2959 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/brain/brain_mechanize.py
--rw-r--r--   0 runner    (1001) docker     (121)     3516 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/brain/brain_multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (121)    21078 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/brain/brain_namedtuple_enum.py
--rw-r--r--   0 runner    (1001) docker     (121)     2581 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/brain/brain_nose.py
--rw-r--r--   0 runner    (1001) docker     (121)      924 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/brain/brain_numpy_core_fromnumeric.py
--rw-r--r--   0 runner    (1001) docker     (121)     1490 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/brain/brain_numpy_core_function_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     4402 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/brain/brain_numpy_core_multiarray.py
--rw-r--r--   0 runner    (1001) docker     (121)     1785 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/brain/brain_numpy_core_numeric.py
--rw-r--r--   0 runner    (1001) docker     (121)     8737 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/brain/brain_numpy_core_numerictypes.py
--rw-r--r--   0 runner    (1001) docker     (121)     5084 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/brain/brain_numpy_core_umath.py
--rw-r--r--   0 runner    (1001) docker     (121)      788 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/brain/brain_numpy_ma.py
--rw-r--r--   0 runner    (1001) docker     (121)     9142 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/brain/brain_numpy_ndarray.py
--rw-r--r--   0 runner    (1001) docker     (121)     3627 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/brain/brain_numpy_random_mtrand.py
--rw-r--r--   0 runner    (1001) docker     (121)     2798 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/brain/brain_numpy_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2386 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/brain/brain_pkg_resources.py
--rw-r--r--   0 runner    (1001) docker     (121)     2631 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/brain/brain_pytest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2812 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/brain/brain_qt.py
--rw-r--r--   0 runner    (1001) docker     (121)     2615 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/brain/brain_random.py
--rw-r--r--   0 runner    (1001) docker     (121)     2576 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/brain/brain_re.py
--rw-r--r--   0 runner    (1001) docker     (121)     1640 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/brain/brain_responses.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2618 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/brain/brain_scipy_signal.py
--rw-r--r--   0 runner    (1001) docker     (121)     3782 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/brain/brain_signal.py
--rw-r--r--   0 runner    (1001) docker     (121)     8090 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/brain/brain_six.py
--rw-r--r--   0 runner    (1001) docker     (121)      780 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/brain/brain_sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (121)     3915 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/brain/brain_ssl.py
--rw-r--r--   0 runner    (1001) docker     (121)     4233 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/brain/brain_subprocess.py
--rw-r--r--   0 runner    (1001) docker     (121)     1119 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/brain/brain_threading.py
--rw-r--r--   0 runner    (1001) docker     (121)     2243 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/brain/brain_type.py
--rw-r--r--   0 runner    (1001) docker     (121)    14654 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/brain/brain_typing.py
--rw-r--r--   0 runner    (1001) docker     (121)      907 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/brain/brain_unittest.py
--rw-r--r--   0 runner    (1001) docker     (121)      851 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/brain/brain_uuid.py
--rw-r--r--   0 runner    (1001) docker     (121)      489 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/brain/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)    17995 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/builder.py
--rw-r--r--   0 runner    (1001) docker     (121)      434 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/const.py
--rw-r--r--   0 runner    (1001) docker     (121)     6390 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/context.py
--rw-r--r--   0 runner    (1001) docker     (121)     6994 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)     9128 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     9522 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/filter_statements.py
--rw-r--r--   0 runner    (1001) docker     (121)    10960 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)    37072 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/inference.py
--rw-r--r--   0 runner    (1001) docker     (121)     2396 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/inference_tip.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 23:16:59.551513 astroid-2.9.2/astroid/interpreter/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/interpreter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 23:16:59.551513 astroid-2.9.2/astroid/interpreter/_import/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/interpreter/_import/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13084 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/interpreter/_import/spec.py
--rw-r--r--   0 runner    (1001) docker     (121)      577 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/interpreter/_import/util.py
--rw-r--r--   0 runner    (1001) docker     (121)     2270 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/interpreter/dunder_lookup.py
--rw-r--r--   0 runner    (1001) docker     (121)    28089 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/interpreter/objectmodel.py
--rw-r--r--   0 runner    (1001) docker     (121)    14861 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     6047 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/mixins.py
--rw-r--r--   0 runner    (1001) docker     (121)    23384 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/modutils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1573 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/node_classes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 23:16:59.551513 astroid-2.9.2/astroid/nodes/
--rw-r--r--   0 runner    (1001) docker     (121)     5460 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    24779 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/nodes/as_string.py
--rw-r--r--   0 runner    (1001) docker     (121)      724 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/nodes/const.py
--rw-r--r--   0 runner    (1001) docker     (121)   166435 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/nodes/node_classes.py
--rw-r--r--   0 runner    (1001) docker     (121)    26964 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/nodes/node_ng.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 23:16:59.551513 astroid-2.9.2/astroid/nodes/scoped_nodes/
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/nodes/scoped_nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   109939 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/nodes/scoped_nodes/scoped_nodes.py
--rw-r--r--   0 runner    (1001) docker     (121)    11709 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/objects.py
--rw-r--r--   0 runner    (1001) docker     (121)    31076 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/protocols.py
--rw-r--r--   0 runner    (1001) docker     (121)    18102 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/raw_building.py
--rw-r--r--   0 runner    (1001) docker     (121)    88326 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/rebuilder.py
--rw-r--r--   0 runner    (1001) docker     (121)      704 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/scoped_nodes.py
--rw-r--r--   0 runner    (1001) docker     (121)     2920 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3631 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/transforms.py
--rw-r--r--   0 runner    (1001) docker     (121)     4304 2022-01-03 23:16:49.000000 astroid-2.9.2/astroid/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 23:16:59.547513 astroid-2.9.2/astroid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4388 2022-01-03 23:16:59.000000 astroid-2.9.2/astroid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2846 2022-01-03 23:16:59.000000 astroid-2.9.2/astroid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-03 23:16:59.000000 astroid-2.9.2/astroid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      198 2022-01-03 23:16:59.000000 astroid-2.9.2/astroid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-01-03 23:16:59.000000 astroid-2.9.2/astroid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2520 2022-01-03 23:16:59.555513 astroid-2.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-03 23:16:49.000000 astroid-2.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 16:18:57.837204 astroid-2.9.3/
+-rw-r--r--   0 runner    (1001) docker     (121)    26516 2022-01-09 16:18:47.000000 astroid-2.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      144 2022-01-09 16:18:47.000000 astroid-2.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     4388 2022-01-09 16:18:57.837204 astroid-2.9.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 16:18:57.829204 astroid-2.9.3/astroid/
+-rw-r--r--   0 runner    (1001) docker     (121)     4806 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1530 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/__pkginfo__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3484 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/_ast.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13365 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (121)      493 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/astroid_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21392 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/bases.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 16:18:57.837204 astroid-2.9.3/astroid/brain/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1114 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2682 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (121)      921 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_boto3.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31376 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_builtin_inference.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4822 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_collections.py
+-rw-r--r--   0 runner    (1001) docker     (121)      967 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_crypt.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2426 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_ctypes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3400 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_curses.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14886 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_dateutil.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2445 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_fstrings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5759 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_functools.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8148 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_gi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2459 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_hashlib.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10798 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_http.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_hypothesis.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1720 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_io.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2959 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_mechanize.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3516 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21078 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_namedtuple_enum.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2581 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_nose.py
+-rw-r--r--   0 runner    (1001) docker     (121)      924 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_numpy_core_fromnumeric.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1490 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_numpy_core_function_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4402 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_numpy_core_multiarray.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1785 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_numpy_core_numeric.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8737 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_numpy_core_numerictypes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5084 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_numpy_core_umath.py
+-rw-r--r--   0 runner    (1001) docker     (121)      788 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_numpy_ma.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9142 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_numpy_ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3627 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_numpy_random_mtrand.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2798 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_numpy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2386 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_pkg_resources.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2631 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_pytest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2812 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_qt.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2615 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_random.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2576 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_re.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1640 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_responses.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2618 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_scipy_signal.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3782 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_signal.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8090 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_six.py
+-rw-r--r--   0 runner    (1001) docker     (121)      780 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3915 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4233 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1119 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_threading.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2243 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14654 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_typing.py
+-rw-r--r--   0 runner    (1001) docker     (121)      907 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_unittest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      851 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/brain_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (121)      489 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/brain/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17995 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/builder.py
+-rw-r--r--   0 runner    (1001) docker     (121)      434 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/const.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6390 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/context.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6994 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9128 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9522 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/filter_statements.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10960 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    37072 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/inference.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2396 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/inference_tip.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 16:18:57.837204 astroid-2.9.3/astroid/interpreter/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/interpreter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 16:18:57.837204 astroid-2.9.3/astroid/interpreter/_import/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/interpreter/_import/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13084 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/interpreter/_import/spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)      577 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/interpreter/_import/util.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2270 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/interpreter/dunder_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28089 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/interpreter/objectmodel.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14861 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6047 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23522 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/modutils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1573 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/node_classes.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 16:18:57.837204 astroid-2.9.3/astroid/nodes/
+-rw-r--r--   0 runner    (1001) docker     (121)     5460 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24779 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/nodes/as_string.py
+-rw-r--r--   0 runner    (1001) docker     (121)      724 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/nodes/const.py
+-rw-r--r--   0 runner    (1001) docker     (121)   166435 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/nodes/node_classes.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26964 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/nodes/node_ng.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 16:18:57.837204 astroid-2.9.3/astroid/nodes/scoped_nodes/
+-rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/nodes/scoped_nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)   109939 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/nodes/scoped_nodes/scoped_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11709 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/objects.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31076 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18102 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/raw_building.py
+-rw-r--r--   0 runner    (1001) docker     (121)    88326 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/rebuilder.py
+-rw-r--r--   0 runner    (1001) docker     (121)      704 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/scoped_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2920 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3631 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4304 2022-01-09 16:18:47.000000 astroid-2.9.3/astroid/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 16:18:57.829204 astroid-2.9.3/astroid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4388 2022-01-09 16:18:57.000000 astroid-2.9.3/astroid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2846 2022-01-09 16:18:57.000000 astroid-2.9.3/astroid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-09 16:18:57.000000 astroid-2.9.3/astroid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      198 2022-01-09 16:18:57.000000 astroid-2.9.3/astroid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-01-09 16:18:57.000000 astroid-2.9.3/astroid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2520 2022-01-09 16:18:57.837204 astroid-2.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-09 16:18:47.000000 astroid-2.9.3/setup.py
```

### Comparing `astroid-2.9.2/LICENSE` & `astroid-2.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/PKG-INFO` & `astroid-2.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astroid
-Version: 2.9.2
+Version: 2.9.3
 Summary: An abstract syntax tree for Python with inference support.
 Home-page: https://github.com/PyCQA/astroid
 Author: Python Code Quality Authority
 Author-email: code-quality@python.org
 License: LGPL-2.1-or-later
 Project-URL: Bug tracker, https://github.com/PyCQA/astroid/issues
 Project-URL: Discord server, https://discord.gg/Egy6P8AMB5
```

### Comparing `astroid-2.9.2/astroid/__init__.py` & `astroid-2.9.3/astroid/__init__.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/__pkginfo__.py` & `astroid-2.9.3/astroid/__pkginfo__.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,9 +20,9 @@
 # Copyright (c) 2020 Michael <michael-k@users.noreply.github.com>
 # Copyright (c) 2021 Pierre Sassoulas <pierre.sassoulas@gmail.com>
 # Copyright (c) 2021 Marc Mueller <30130371+cdce8p@users.noreply.github.com>
 
 # Licensed under the LGPL: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html
 # For details: https://github.com/PyCQA/astroid/blob/main/LICENSE
 
-__version__ = "2.9.2"
+__version__ = "2.9.3"
 version = __version__
```

### Comparing `astroid-2.9.2/astroid/_ast.py` & `astroid-2.9.3/astroid/_ast.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/arguments.py` & `astroid-2.9.3/astroid/arguments.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/bases.py` & `astroid-2.9.3/astroid/bases.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/brain/brain_argparse.py` & `astroid-2.9.3/astroid/brain/brain_argparse.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/brain/brain_attrs.py` & `astroid-2.9.3/astroid/brain/brain_attrs.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/brain/brain_boto3.py` & `astroid-2.9.3/astroid/brain/brain_boto3.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/brain/brain_builtin_inference.py` & `astroid-2.9.3/astroid/brain/brain_builtin_inference.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/brain/brain_collections.py` & `astroid-2.9.3/astroid/brain/brain_collections.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/brain/brain_crypt.py` & `astroid-2.9.3/astroid/brain/brain_crypt.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/brain/brain_ctypes.py` & `astroid-2.9.3/astroid/brain/brain_ctypes.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/brain/brain_curses.py` & `astroid-2.9.3/astroid/brain/brain_curses.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/brain/brain_dataclasses.py` & `astroid-2.9.3/astroid/brain/brain_dataclasses.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/brain/brain_dateutil.py` & `astroid-2.9.3/astroid/brain/brain_dateutil.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/brain/brain_fstrings.py` & `astroid-2.9.3/astroid/brain/brain_fstrings.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/brain/brain_functools.py` & `astroid-2.9.3/astroid/brain/brain_functools.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/brain/brain_gi.py` & `astroid-2.9.3/astroid/brain/brain_gi.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/brain/brain_hashlib.py` & `astroid-2.9.3/astroid/brain/brain_hashlib.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/brain/brain_http.py` & `astroid-2.9.3/astroid/brain/brain_http.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/brain/brain_hypothesis.py` & `astroid-2.9.3/astroid/brain/brain_hypothesis.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/brain/brain_io.py` & `astroid-2.9.3/astroid/brain/brain_io.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/brain/brain_mechanize.py` & `astroid-2.9.3/astroid/brain/brain_mechanize.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/brain/brain_multiprocessing.py` & `astroid-2.9.3/astroid/brain/brain_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/brain/brain_namedtuple_enum.py` & `astroid-2.9.3/astroid/brain/brain_namedtuple_enum.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/brain/brain_nose.py` & `astroid-2.9.3/astroid/brain/brain_nose.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/brain/brain_numpy_core_fromnumeric.py` & `astroid-2.9.3/astroid/brain/brain_numpy_core_fromnumeric.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/brain/brain_numpy_core_function_base.py` & `astroid-2.9.3/astroid/brain/brain_numpy_core_function_base.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/brain/brain_numpy_core_multiarray.py` & `astroid-2.9.3/astroid/brain/brain_numpy_core_multiarray.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/brain/brain_numpy_core_numeric.py` & `astroid-2.9.3/astroid/brain/brain_numpy_core_numeric.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/brain/brain_numpy_core_numerictypes.py` & `astroid-2.9.3/astroid/brain/brain_numpy_core_numerictypes.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/brain/brain_numpy_core_umath.py` & `astroid-2.9.3/astroid/brain/brain_numpy_core_umath.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/brain/brain_numpy_ma.py` & `astroid-2.9.3/astroid/brain/brain_numpy_ma.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/brain/brain_numpy_ndarray.py` & `astroid-2.9.3/astroid/brain/brain_numpy_ndarray.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/brain/brain_numpy_random_mtrand.py` & `astroid-2.9.3/astroid/brain/brain_numpy_random_mtrand.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/brain/brain_numpy_utils.py` & `astroid-2.9.3/astroid/brain/brain_numpy_utils.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/brain/brain_pkg_resources.py` & `astroid-2.9.3/astroid/brain/brain_pkg_resources.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/brain/brain_pytest.py` & `astroid-2.9.3/astroid/brain/brain_pytest.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/brain/brain_qt.py` & `astroid-2.9.3/astroid/brain/brain_qt.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/brain/brain_random.py` & `astroid-2.9.3/astroid/brain/brain_random.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/brain/brain_re.py` & `astroid-2.9.3/astroid/brain/brain_re.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/brain/brain_responses.py` & `astroid-2.9.3/astroid/brain/brain_responses.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/brain/brain_scipy_signal.py` & `astroid-2.9.3/astroid/brain/brain_scipy_signal.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/brain/brain_signal.py` & `astroid-2.9.3/astroid/brain/brain_signal.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/brain/brain_six.py` & `astroid-2.9.3/astroid/brain/brain_six.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/brain/brain_sqlalchemy.py` & `astroid-2.9.3/astroid/brain/brain_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/brain/brain_ssl.py` & `astroid-2.9.3/astroid/brain/brain_ssl.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/brain/brain_subprocess.py` & `astroid-2.9.3/astroid/brain/brain_subprocess.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/brain/brain_threading.py` & `astroid-2.9.3/astroid/brain/brain_threading.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/brain/brain_type.py` & `astroid-2.9.3/astroid/brain/brain_type.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/brain/brain_typing.py` & `astroid-2.9.3/astroid/brain/brain_typing.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/brain/brain_unittest.py` & `astroid-2.9.3/astroid/brain/brain_unittest.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/brain/brain_uuid.py` & `astroid-2.9.3/astroid/brain/brain_uuid.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/builder.py` & `astroid-2.9.3/astroid/builder.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/context.py` & `astroid-2.9.3/astroid/context.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/decorators.py` & `astroid-2.9.3/astroid/decorators.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/exceptions.py` & `astroid-2.9.3/astroid/exceptions.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/filter_statements.py` & `astroid-2.9.3/astroid/filter_statements.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/helpers.py` & `astroid-2.9.3/astroid/helpers.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/inference.py` & `astroid-2.9.3/astroid/inference.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/inference_tip.py` & `astroid-2.9.3/astroid/inference_tip.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/interpreter/_import/spec.py` & `astroid-2.9.3/astroid/interpreter/_import/spec.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/interpreter/_import/util.py` & `astroid-2.9.3/astroid/interpreter/_import/util.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/interpreter/dunder_lookup.py` & `astroid-2.9.3/astroid/interpreter/dunder_lookup.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/interpreter/objectmodel.py` & `astroid-2.9.3/astroid/interpreter/objectmodel.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/manager.py` & `astroid-2.9.3/astroid/manager.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/mixins.py` & `astroid-2.9.3/astroid/mixins.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/modutils.py` & `astroid-2.9.3/astroid/modutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -293,26 +293,32 @@
     if os.path.normcase(abs_filename).startswith(path_to_check):
         importable_path = abs_filename
 
     real_filename = os.path.realpath(filename)
     if os.path.normcase(real_filename).startswith(path_to_check):
         importable_path = real_filename
 
+    # if "var" in path_to_check:
+    #     breakpoint()
+
     if importable_path:
         base_path = os.path.splitext(importable_path)[0]
         relative_base_path = base_path[len(path_to_check) :]
         return [pkg for pkg in relative_base_path.split(os.sep) if pkg]
 
     return None
 
 
 def modpath_from_file_with_callback(filename, path=None, is_package_cb=None):
     filename = os.path.expanduser(_path_from_filename(filename))
+    paths_to_check = sys.path.copy()
+    if path:
+        paths_to_check += path
     for pathname in itertools.chain(
-        path or [], map(_cache_normalize_path, sys.path), sys.path
+        paths_to_check, map(_cache_normalize_path, paths_to_check)
     ):
         if not pathname:
             continue
         modpath = _get_relative_base_path(filename, pathname)
         if not modpath:
             continue
         if is_package_cb(pathname, modpath[:-1]):
```

### Comparing `astroid-2.9.2/astroid/node_classes.py` & `astroid-2.9.3/astroid/node_classes.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/nodes/__init__.py` & `astroid-2.9.3/astroid/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/nodes/as_string.py` & `astroid-2.9.3/astroid/nodes/as_string.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/nodes/const.py` & `astroid-2.9.3/astroid/nodes/const.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/nodes/node_classes.py` & `astroid-2.9.3/astroid/nodes/node_classes.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/nodes/node_ng.py` & `astroid-2.9.3/astroid/nodes/node_ng.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/nodes/scoped_nodes/__init__.py` & `astroid-2.9.3/astroid/nodes/scoped_nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/nodes/scoped_nodes/scoped_nodes.py` & `astroid-2.9.3/astroid/nodes/scoped_nodes/scoped_nodes.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/objects.py` & `astroid-2.9.3/astroid/objects.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/protocols.py` & `astroid-2.9.3/astroid/protocols.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/raw_building.py` & `astroid-2.9.3/astroid/raw_building.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/rebuilder.py` & `astroid-2.9.3/astroid/rebuilder.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/scoped_nodes.py` & `astroid-2.9.3/astroid/scoped_nodes.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/test_utils.py` & `astroid-2.9.3/astroid/test_utils.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/transforms.py` & `astroid-2.9.3/astroid/transforms.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid/util.py` & `astroid-2.9.3/astroid/util.py`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/astroid.egg-info/PKG-INFO` & `astroid-2.9.3/astroid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astroid
-Version: 2.9.2
+Version: 2.9.3
 Summary: An abstract syntax tree for Python with inference support.
 Home-page: https://github.com/PyCQA/astroid
 Author: Python Code Quality Authority
 Author-email: code-quality@python.org
 License: LGPL-2.1-or-later
 Project-URL: Bug tracker, https://github.com/PyCQA/astroid/issues
 Project-URL: Discord server, https://discord.gg/Egy6P8AMB5
```

### Comparing `astroid-2.9.2/astroid.egg-info/SOURCES.txt` & `astroid-2.9.3/astroid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `astroid-2.9.2/setup.cfg` & `astroid-2.9.3/setup.cfg`

 * *Files identical despite different names*

