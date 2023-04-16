# Comparing `tmp/cmyt-1.1.3.tar.gz` & `tmp/cmyt-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmyt-1.1.3.tar", last modified: Sat Dec 24 13:23:51 2022, max compression
+gzip compressed data, was "cmyt-1.2.0.tar", last modified: Sun Apr 16 18:27:36 2023, max compression
```

## Comparing `cmyt-1.1.3.tar` & `cmyt-1.2.0.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-24 13:23:51.008893 cmyt-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2022-12-24 13:23:41.000000 cmyt-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4384 2022-12-24 13:23:51.008893 cmyt-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2022-12-24 13:23:41.000000 cmyt-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-24 13:23:51.004893 cmyt-1.1.3/cmyt/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2022-12-24 13:23:41.000000 cmyt-1.1.3/cmyt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2022-12-24 13:23:41.000000 cmyt-1.1.3/cmyt/cm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-24 13:23:51.004893 cmyt-1.1.3/cmyt/colormaps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-24 13:23:41.000000 cmyt-1.1.3/cmyt/colormaps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2022-12-24 13:23:41.000000 cmyt-1.1.3/cmyt/colormaps/algae.py
--rw-r--r--   0 runner    (1001) docker     (123)    19063 2022-12-24 13:23:41.000000 cmyt-1.1.3/cmyt/colormaps/arbre.py
--rw-r--r--   0 runner    (1001) docker     (123)    19345 2022-12-24 13:23:41.000000 cmyt-1.1.3/cmyt/colormaps/dusk.py
--rw-r--r--   0 runner    (1001) docker     (123)    19006 2022-12-24 13:23:41.000000 cmyt-1.1.3/cmyt/colormaps/kelp.py
--rw-r--r--   0 runner    (1001) docker     (123)    19059 2022-12-24 13:23:41.000000 cmyt-1.1.3/cmyt/colormaps/octarine.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2022-12-24 13:23:41.000000 cmyt-1.1.3/cmyt/colormaps/pastel.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2022-12-24 13:23:41.000000 cmyt-1.1.3/cmyt/colormaps/pixel_blue.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2022-12-24 13:23:41.000000 cmyt-1.1.3/cmyt/colormaps/pixel_green.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2022-12-24 13:23:41.000000 cmyt-1.1.3/cmyt/colormaps/pixel_red.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2022-12-24 13:23:41.000000 cmyt-1.1.3/cmyt/colormaps/xray.py
--rw-r--r--   0 runner    (1001) docker     (123)     6169 2022-12-24 13:23:41.000000 cmyt-1.1.3/cmyt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-24 13:23:51.004893 cmyt-1.1.3/cmyt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4384 2022-12-24 13:23:50.000000 cmyt-1.1.3/cmyt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      588 2022-12-24 13:23:51.000000 cmyt-1.1.3/cmyt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-24 13:23:50.000000 cmyt-1.1.3/cmyt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2022-12-24 13:23:50.000000 cmyt-1.1.3/cmyt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2022-12-24 13:23:50.000000 cmyt-1.1.3/cmyt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2022-12-24 13:23:41.000000 cmyt-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      189 2022-12-24 13:23:51.008893 cmyt-1.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-24 13:23:51.004893 cmyt-1.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2022-12-24 13:23:41.000000 cmyt-1.1.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2022-12-24 13:23:41.000000 cmyt-1.1.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2022-12-24 13:23:41.000000 cmyt-1.1.3/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2022-12-24 13:23:41.000000 cmyt-1.1.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:27:36.192787 cmyt-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-04-16 18:27:24.000000 cmyt-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-04-16 18:27:36.192787 cmyt-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-04-16 18:27:24.000000 cmyt-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:27:36.188787 cmyt-1.2.0/cmyt/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-16 18:27:24.000000 cmyt-1.2.0/cmyt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-16 18:27:24.000000 cmyt-1.2.0/cmyt/cm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:27:36.192787 cmyt-1.2.0/cmyt/colormaps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 18:27:24.000000 cmyt-1.2.0/cmyt/colormaps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-16 18:27:24.000000 cmyt-1.2.0/cmyt/colormaps/algae.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17723 2023-04-16 18:27:24.000000 cmyt-1.2.0/cmyt/colormaps/apricity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19063 2023-04-16 18:27:24.000000 cmyt-1.2.0/cmyt/colormaps/arbre.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19345 2023-04-16 18:27:24.000000 cmyt-1.2.0/cmyt/colormaps/dusk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19006 2023-04-16 18:27:24.000000 cmyt-1.2.0/cmyt/colormaps/kelp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19059 2023-04-16 18:27:24.000000 cmyt-1.2.0/cmyt/colormaps/octarine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-16 18:27:24.000000 cmyt-1.2.0/cmyt/colormaps/pastel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-16 18:27:24.000000 cmyt-1.2.0/cmyt/colormaps/pixel_blue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-16 18:27:24.000000 cmyt-1.2.0/cmyt/colormaps/pixel_green.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-16 18:27:24.000000 cmyt-1.2.0/cmyt/colormaps/pixel_red.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-16 18:27:24.000000 cmyt-1.2.0/cmyt/colormaps/xray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-04-16 18:27:24.000000 cmyt-1.2.0/cmyt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:27:36.188787 cmyt-1.2.0/cmyt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-04-16 18:27:36.000000 cmyt-1.2.0/cmyt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-16 18:27:36.000000 cmyt-1.2.0/cmyt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 18:27:36.000000 cmyt-1.2.0/cmyt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-16 18:27:36.000000 cmyt-1.2.0/cmyt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-16 18:27:36.000000 cmyt-1.2.0/cmyt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-04-16 18:27:24.000000 cmyt-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 18:27:36.192787 cmyt-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:27:36.192787 cmyt-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-16 18:27:24.000000 cmyt-1.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-16 18:27:24.000000 cmyt-1.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-16 18:27:24.000000 cmyt-1.2.0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-16 18:27:24.000000 cmyt-1.2.0/tests/test_utils.py
```

### Comparing `cmyt-1.1.3/LICENSE` & `cmyt-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cmyt-1.1.3/PKG-INFO` & `cmyt-1.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmyt
-Version: 1.1.3
+Version: 1.2.0
 Summary: A collection of Matplotlib colormaps from the yt project
 Author-email: The yt project <yt-dev@python.org>
 License: BSD 3-Clause
 Project-URL: Homepage, https://yt-project.org/
 Project-URL: Source, https://github.com/yt-project/cmyt/
 Project-URL: Tracker, https://github.com/yt-project/cmyt/issues
 Keywords: visualization
@@ -17,30 +17,29 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
 
 # cmyt
 
 [![PyPI](https://img.shields.io/pypi/v/cmyt.svg?logo=pypi&logoColor=white&label=PyPI)](https://pypi.org/project/cmyt)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/cmyt.svg?logo=condaforge&logoColor=white)](https://anaconda.org/conda-forge/cmyt)
 [![Supported Python Versions](https://img.shields.io/badge/requires-Python%20≥%203.8-blue?logo=python&logoColor=white)](https://pypi.org/project/cmyt/)
 
 [![CI](https://github.com/yt-project/cmyt/actions/workflows/ci.yml/badge.svg)](https://github.com/yt-project/cmyt/actions/workflows/ci.yml)
 [![CI (bleeding edge)](https://github.com/yt-project/cmyt/actions/workflows/bleeding-edge.yaml/badge.svg)](https://github.com/yt-project/cmyt/actions/workflows/bleeding-edge.yaml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/yt-project/cmyt/main.svg)](https://results.pre-commit.ci/latest/github/yt-project/cmyt/main)
 
 [![yt-project](https://img.shields.io/static/v1?label="works%20with"&message="yt"&color="blueviolet")](https://yt-project.org)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 
 <a href="http://yt-project.org"><img src="https://raw.githubusercontent.com/yt-project/yt/main/doc/source/_static/yt_logo.png" width="150"></a>
 
 Matplotlib colormaps from the yt project !
 
 ## Colormaps overview
 
@@ -61,15 +60,15 @@
     <img src="https://raw.githubusercontent.com/yt-project/cmyt/main/doc/overview_misc.png" width="800"></a>
 </p>
 
 ## Installation
 
 with `pip`
 ```shell
-python3 -m pip install cmyt
+python -m pip install cmyt
 ```
 or with `conda`
 ```shell
 conda install -c conda-forge cmyt
 ```
 
 ## Usage
```

#### html2text {}

```diff
@@ -1,47 +1,49 @@
-Metadata-Version: 2.1 Name: cmyt Version: 1.1.3 Summary: A collection of
+Metadata-Version: 2.1 Name: cmyt Version: 1.2.0 Summary: A collection of
 Matplotlib colormaps from the yt project Author-email: The yt project
 python.org> License: BSD 3-Clause Project-URL: Homepage, https://yt-
 project.org/ Project-URL: Source, https://github.com/yt-project/cmyt/ Project-
 URL: Tracker, https://github.com/yt-project/cmyt/issues Keywords: visualization
 Classifier: Development Status :: 5 - Production/Stable Classifier: Framework
 :: Matplotlib Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: BSD License Classifier: Operating System :: MacOS ::
 MacOS X Classifier: Operating System :: POSIX :: AIX Classifier: Operating
 System :: POSIX :: Linux Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Topic ::
 Scientific/Engineering :: Visualization Classifier: Typing :: Typed Requires-
-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra: dev
-License-File: LICENSE # cmyt [![PyPI](https://img.shields.io/pypi/v/
+Python: >=3.8 Description-Content-Type: text/markdown License-File: LICENSE #
+cmyt [![PyPI](https://img.shields.io/pypi/v/
 cmyt.svg?logo=pypi&logoColor=white&label=PyPI)](https://pypi.org/project/cmyt)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/
 cmyt.svg?logo=condaforge&logoColor=white)](https://anaconda.org/conda-forge/
 cmyt) [![Supported Python Versions](https://img.shields.io/badge/requires-
 Python%20â¥%203.8-blue?logo=python&logoColor=white)](https://pypi.org/project/
 cmyt/) [![CI](https://github.com/yt-project/cmyt/actions/workflows/ci.yml/
 badge.svg)](https://github.com/yt-project/cmyt/actions/workflows/ci.yml) [![CI
 (bleeding edge)](https://github.com/yt-project/cmyt/actions/workflows/bleeding-
 edge.yaml/badge.svg)](https://github.com/yt-project/cmyt/actions/workflows/
 bleeding-edge.yaml) [![pre-commit.ci status](https://results.pre-commit.ci/
 badge/github/yt-project/cmyt/main.svg)](https://results.pre-commit.ci/latest/
 github/yt-project/cmyt/main) [![yt-project](https://img.shields.io/static/
 v1?label="works%20with"&message="yt"&color="blueviolet")](https://yt-
 project.org) [![Code style: black](https://img.shields.io/badge/code%20style-
-black-000000.svg)](https://github.com/psf/black) [https://
-raw.githubusercontent.com/yt-project/yt/main/doc/source/_static/yt_logo.png]
+black-000000.svg)](https://github.com/psf/black) [![Ruff](https://
+img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/
+ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff) [https:
+//raw.githubusercontent.com/yt-project/yt/main/doc/source/_static/yt_logo.png]
 Matplotlib colormaps from the yt project ! ## Colormaps overview The following
 colormaps, as well as their respective reversed (`*_r`) versions are available
 ### Perceptually uniform sequential colormaps
          [https://raw.githubusercontent.com/yt-project/cmyt/main/doc/
                       overview_perceptually_uniform.png]
 ### Monochromatic sequential colormaps
 [https://raw.githubusercontent.com/yt-project/cmyt/main/doc/overview_pixel.png]
 ### Miscellaneous
 [https://raw.githubusercontent.com/yt-project/cmyt/main/doc/overview_misc.png]
-## Installation with `pip` ```shell python3 -m pip install cmyt ``` or with
+## Installation with `pip` ```shell python -m pip install cmyt ``` or with
 `conda` ```shell conda install -c conda-forge cmyt ``` ## Usage cmyt integrates
 with matplotlib in a similar fashion to [cmocean](https://matplotlib.org/
 cmocean/) or [cmasher](https://cmasher.readthedocs.io) ```python import numpy
 as np import matplotlib.pyplot as plt import cmyt # that's it ! # generate
 example data prng = np.random.RandomState(0x4D3D3D3) noise = prng.random_sample
 ((100, 100)) x, y = np.mgrid[-50:50, -50:50] z = 5 * np.exp(-(x**2 + y**2) /
 1000) # setup the figure fig, ax = plt.subplots() ax.set(aspect="equal") # now
```

### Comparing `cmyt-1.1.3/README.md` & `cmyt-1.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 [![CI](https://github.com/yt-project/cmyt/actions/workflows/ci.yml/badge.svg)](https://github.com/yt-project/cmyt/actions/workflows/ci.yml)
 [![CI (bleeding edge)](https://github.com/yt-project/cmyt/actions/workflows/bleeding-edge.yaml/badge.svg)](https://github.com/yt-project/cmyt/actions/workflows/bleeding-edge.yaml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/yt-project/cmyt/main.svg)](https://results.pre-commit.ci/latest/github/yt-project/cmyt/main)
 
 [![yt-project](https://img.shields.io/static/v1?label="works%20with"&message="yt"&color="blueviolet")](https://yt-project.org)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 
 <a href="http://yt-project.org"><img src="https://raw.githubusercontent.com/yt-project/yt/main/doc/source/_static/yt_logo.png" width="150"></a>
 
 Matplotlib colormaps from the yt project !
 
 ## Colormaps overview
 
@@ -35,15 +35,15 @@
     <img src="https://raw.githubusercontent.com/yt-project/cmyt/main/doc/overview_misc.png" width="800"></a>
 </p>
 
 ## Installation
 
 with `pip`
 ```shell
-python3 -m pip install cmyt
+python -m pip install cmyt
 ```
 or with `conda`
 ```shell
 conda install -c conda-forge cmyt
 ```
 
 ## Usage
```

#### html2text {}

```diff
@@ -9,26 +9,28 @@
 (bleeding edge)](https://github.com/yt-project/cmyt/actions/workflows/bleeding-
 edge.yaml/badge.svg)](https://github.com/yt-project/cmyt/actions/workflows/
 bleeding-edge.yaml) [![pre-commit.ci status](https://results.pre-commit.ci/
 badge/github/yt-project/cmyt/main.svg)](https://results.pre-commit.ci/latest/
 github/yt-project/cmyt/main) [![yt-project](https://img.shields.io/static/
 v1?label="works%20with"&message="yt"&color="blueviolet")](https://yt-
 project.org) [![Code style: black](https://img.shields.io/badge/code%20style-
-black-000000.svg)](https://github.com/psf/black) [https://
-raw.githubusercontent.com/yt-project/yt/main/doc/source/_static/yt_logo.png]
+black-000000.svg)](https://github.com/psf/black) [![Ruff](https://
+img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/
+ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff) [https:
+//raw.githubusercontent.com/yt-project/yt/main/doc/source/_static/yt_logo.png]
 Matplotlib colormaps from the yt project ! ## Colormaps overview The following
 colormaps, as well as their respective reversed (`*_r`) versions are available
 ### Perceptually uniform sequential colormaps
          [https://raw.githubusercontent.com/yt-project/cmyt/main/doc/
                       overview_perceptually_uniform.png]
 ### Monochromatic sequential colormaps
 [https://raw.githubusercontent.com/yt-project/cmyt/main/doc/overview_pixel.png]
 ### Miscellaneous
 [https://raw.githubusercontent.com/yt-project/cmyt/main/doc/overview_misc.png]
-## Installation with `pip` ```shell python3 -m pip install cmyt ``` or with
+## Installation with `pip` ```shell python -m pip install cmyt ``` or with
 `conda` ```shell conda install -c conda-forge cmyt ``` ## Usage cmyt integrates
 with matplotlib in a similar fashion to [cmocean](https://matplotlib.org/
 cmocean/) or [cmasher](https://cmasher.readthedocs.io) ```python import numpy
 as np import matplotlib.pyplot as plt import cmyt # that's it ! # generate
 example data prng = np.random.RandomState(0x4D3D3D3) noise = prng.random_sample
 ((100, 100)) x, y = np.mgrid[-50:50, -50:50] z = 5 * np.exp(-(x**2 + y**2) /
 1000) # setup the figure fig, ax = plt.subplots() ax.set(aspect="equal") # now
```

### Comparing `cmyt-1.1.3/cmyt/cm.py` & `cmyt-1.2.0/cmyt/cm.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from importlib import import_module
 
 import numpy as np
 
-from cmyt.utils import cmyt_cmaps
-from cmyt.utils import ColorDict
-from cmyt.utils import register_colormap
+from cmyt.utils import ColorDict, cmyt_cmaps, register_colormap
 
 
 def _luts_to_cdict(luts: np.ndarray) -> ColorDict:
     _vs = np.linspace(0, 1, 256)
 
     return {
         "red": np.transpose([_vs, luts[0], luts[0]]),
```

### Comparing `cmyt-1.1.3/cmyt/colormaps/algae.py` & `cmyt-1.2.0/cmyt/colormaps/algae.py`

 * *Files identical despite different names*

### Comparing `cmyt-1.1.3/cmyt/colormaps/arbre.py` & `cmyt-1.2.0/cmyt/colormaps/arbre.py`

 * *Files identical despite different names*

### Comparing `cmyt-1.1.3/cmyt/colormaps/dusk.py` & `cmyt-1.2.0/cmyt/colormaps/dusk.py`

 * *Files identical despite different names*

### Comparing `cmyt-1.1.3/cmyt/colormaps/kelp.py` & `cmyt-1.2.0/cmyt/colormaps/kelp.py`

 * *Files identical despite different names*

### Comparing `cmyt-1.1.3/cmyt/colormaps/octarine.py` & `cmyt-1.2.0/cmyt/colormaps/octarine.py`

 * *Files identical despite different names*

### Comparing `cmyt-1.1.3/cmyt/colormaps/pastel.py` & `cmyt-1.2.0/cmyt/colormaps/pastel.py`

 * *Files identical despite different names*

### Comparing `cmyt-1.1.3/cmyt/colormaps/xray.py` & `cmyt-1.2.0/cmyt/colormaps/xray.py`

 * *Files identical despite different names*

### Comparing `cmyt-1.1.3/cmyt/utils.py` & `cmyt-1.2.0/cmyt/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,15 @@
 import os
 import re
 import sys
-from typing import Dict
-from typing import Final
-from typing import Iterable
-from typing import Literal
-from typing import Optional
-from typing import Tuple
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Dict, Final, Iterable, Literal, Optional, Tuple
 
 import matplotlib
 import numpy as np
-from matplotlib.colors import Colormap
-from matplotlib.colors import LinearSegmentedColormap
+from matplotlib.colors import Colormap, LinearSegmentedColormap
 from more_itertools import always_iterable
 
 # type aliases
 
 if TYPE_CHECKING:
     from matplotlib.axes import Axes
     from matplotlib.figure import Figure
@@ -26,14 +19,15 @@
 
 ColorDict = Dict[PrimaryColorName, Iterable[Tuple[float, float, float]]]
 
 # this is used in cmyt.cm to programmatically import all cmaps
 cmyt_cmaps = frozenset(
     (
         "algae",
+        "apricity",
         "arbre",
         "dusk",
         "kelp",
         "octarine",
         "pastel",
         "pixel_blue",
         "pixel_green",
```

### Comparing `cmyt-1.1.3/cmyt.egg-info/PKG-INFO` & `cmyt-1.2.0/cmyt.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmyt
-Version: 1.1.3
+Version: 1.2.0
 Summary: A collection of Matplotlib colormaps from the yt project
 Author-email: The yt project <yt-dev@python.org>
 License: BSD 3-Clause
 Project-URL: Homepage, https://yt-project.org/
 Project-URL: Source, https://github.com/yt-project/cmyt/
 Project-URL: Tracker, https://github.com/yt-project/cmyt/issues
 Keywords: visualization
@@ -17,30 +17,29 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
 
 # cmyt
 
 [![PyPI](https://img.shields.io/pypi/v/cmyt.svg?logo=pypi&logoColor=white&label=PyPI)](https://pypi.org/project/cmyt)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/cmyt.svg?logo=condaforge&logoColor=white)](https://anaconda.org/conda-forge/cmyt)
 [![Supported Python Versions](https://img.shields.io/badge/requires-Python%20≥%203.8-blue?logo=python&logoColor=white)](https://pypi.org/project/cmyt/)
 
 [![CI](https://github.com/yt-project/cmyt/actions/workflows/ci.yml/badge.svg)](https://github.com/yt-project/cmyt/actions/workflows/ci.yml)
 [![CI (bleeding edge)](https://github.com/yt-project/cmyt/actions/workflows/bleeding-edge.yaml/badge.svg)](https://github.com/yt-project/cmyt/actions/workflows/bleeding-edge.yaml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/yt-project/cmyt/main.svg)](https://results.pre-commit.ci/latest/github/yt-project/cmyt/main)
 
 [![yt-project](https://img.shields.io/static/v1?label="works%20with"&message="yt"&color="blueviolet")](https://yt-project.org)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 
 <a href="http://yt-project.org"><img src="https://raw.githubusercontent.com/yt-project/yt/main/doc/source/_static/yt_logo.png" width="150"></a>
 
 Matplotlib colormaps from the yt project !
 
 ## Colormaps overview
 
@@ -61,15 +60,15 @@
     <img src="https://raw.githubusercontent.com/yt-project/cmyt/main/doc/overview_misc.png" width="800"></a>
 </p>
 
 ## Installation
 
 with `pip`
 ```shell
-python3 -m pip install cmyt
+python -m pip install cmyt
 ```
 or with `conda`
 ```shell
 conda install -c conda-forge cmyt
 ```
 
 ## Usage
```

#### html2text {}

```diff
@@ -1,47 +1,49 @@
-Metadata-Version: 2.1 Name: cmyt Version: 1.1.3 Summary: A collection of
+Metadata-Version: 2.1 Name: cmyt Version: 1.2.0 Summary: A collection of
 Matplotlib colormaps from the yt project Author-email: The yt project
 python.org> License: BSD 3-Clause Project-URL: Homepage, https://yt-
 project.org/ Project-URL: Source, https://github.com/yt-project/cmyt/ Project-
 URL: Tracker, https://github.com/yt-project/cmyt/issues Keywords: visualization
 Classifier: Development Status :: 5 - Production/Stable Classifier: Framework
 :: Matplotlib Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: BSD License Classifier: Operating System :: MacOS ::
 MacOS X Classifier: Operating System :: POSIX :: AIX Classifier: Operating
 System :: POSIX :: Linux Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Topic ::
 Scientific/Engineering :: Visualization Classifier: Typing :: Typed Requires-
-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra: dev
-License-File: LICENSE # cmyt [![PyPI](https://img.shields.io/pypi/v/
+Python: >=3.8 Description-Content-Type: text/markdown License-File: LICENSE #
+cmyt [![PyPI](https://img.shields.io/pypi/v/
 cmyt.svg?logo=pypi&logoColor=white&label=PyPI)](https://pypi.org/project/cmyt)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/
 cmyt.svg?logo=condaforge&logoColor=white)](https://anaconda.org/conda-forge/
 cmyt) [![Supported Python Versions](https://img.shields.io/badge/requires-
 Python%20â¥%203.8-blue?logo=python&logoColor=white)](https://pypi.org/project/
 cmyt/) [![CI](https://github.com/yt-project/cmyt/actions/workflows/ci.yml/
 badge.svg)](https://github.com/yt-project/cmyt/actions/workflows/ci.yml) [![CI
 (bleeding edge)](https://github.com/yt-project/cmyt/actions/workflows/bleeding-
 edge.yaml/badge.svg)](https://github.com/yt-project/cmyt/actions/workflows/
 bleeding-edge.yaml) [![pre-commit.ci status](https://results.pre-commit.ci/
 badge/github/yt-project/cmyt/main.svg)](https://results.pre-commit.ci/latest/
 github/yt-project/cmyt/main) [![yt-project](https://img.shields.io/static/
 v1?label="works%20with"&message="yt"&color="blueviolet")](https://yt-
 project.org) [![Code style: black](https://img.shields.io/badge/code%20style-
-black-000000.svg)](https://github.com/psf/black) [https://
-raw.githubusercontent.com/yt-project/yt/main/doc/source/_static/yt_logo.png]
+black-000000.svg)](https://github.com/psf/black) [![Ruff](https://
+img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/
+ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff) [https:
+//raw.githubusercontent.com/yt-project/yt/main/doc/source/_static/yt_logo.png]
 Matplotlib colormaps from the yt project ! ## Colormaps overview The following
 colormaps, as well as their respective reversed (`*_r`) versions are available
 ### Perceptually uniform sequential colormaps
          [https://raw.githubusercontent.com/yt-project/cmyt/main/doc/
                       overview_perceptually_uniform.png]
 ### Monochromatic sequential colormaps
 [https://raw.githubusercontent.com/yt-project/cmyt/main/doc/overview_pixel.png]
 ### Miscellaneous
 [https://raw.githubusercontent.com/yt-project/cmyt/main/doc/overview_misc.png]
-## Installation with `pip` ```shell python3 -m pip install cmyt ``` or with
+## Installation with `pip` ```shell python -m pip install cmyt ``` or with
 `conda` ```shell conda install -c conda-forge cmyt ``` ## Usage cmyt integrates
 with matplotlib in a similar fashion to [cmocean](https://matplotlib.org/
 cmocean/) or [cmasher](https://cmasher.readthedocs.io) ```python import numpy
 as np import matplotlib.pyplot as plt import cmyt # that's it ! # generate
 example data prng = np.random.RandomState(0x4D3D3D3) noise = prng.random_sample
 ((100, 100)) x, y = np.mgrid[-50:50, -50:50] z = 5 * np.exp(-(x**2 + y**2) /
 1000) # setup the figure fig, ax = plt.subplots() ax.set(aspect="equal") # now
```

### Comparing `cmyt-1.1.3/cmyt.egg-info/SOURCES.txt` & `cmyt-1.2.0/cmyt.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 LICENSE
 README.md
 pyproject.toml
-setup.cfg
 cmyt/__init__.py
 cmyt/cm.py
 cmyt/utils.py
 cmyt.egg-info/PKG-INFO
 cmyt.egg-info/SOURCES.txt
 cmyt.egg-info/dependency_links.txt
 cmyt.egg-info/requires.txt
 cmyt.egg-info/top_level.txt
 cmyt/colormaps/__init__.py
 cmyt/colormaps/algae.py
+cmyt/colormaps/apricity.py
 cmyt/colormaps/arbre.py
 cmyt/colormaps/dusk.py
 cmyt/colormaps/kelp.py
 cmyt/colormaps/octarine.py
 cmyt/colormaps/pastel.py
 cmyt/colormaps/pixel_blue.py
 cmyt/colormaps/pixel_green.py
```

### Comparing `cmyt-1.1.3/pyproject.toml` & `cmyt-1.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 [build-system]
-requires = [
-    "setuptools>=61.2",
-]
+requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cmyt"
-version = "1.1.3"
+version = "1.2.0"
 description = "A collection of Matplotlib colormaps from the yt project"
 authors = [
     { name = "The yt project", email = "yt-dev@python.org" },
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Framework :: Matplotlib",
@@ -34,60 +32,61 @@
     "more-itertools>=8.4",
     "numpy>=1.17.4",
 ]
 
 [project.license]
 text = "BSD 3-Clause"
 
-[project.optional-dependencies]
-dev = [
-    "pytest>=6.2.4",
-    "pytest-cov>=2.12.1",
-    "pytest-mpl>=0.13",
-]
-
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
 
 [project.urls]
 Homepage = "https://yt-project.org/"
 Source = "https://github.com/yt-project/cmyt/"
 Tracker = "https://github.com/yt-project/cmyt/issues"
 
-[tool.black]
-line-length = 88
-target-version = [
-  'py38',
-  'py39',
-  'py310',
+[tool.setuptools]
+license-files = [
+    "LICENSE",
+]
+include-package-data = false
+
+[tool.setuptools.packages.find]
+namespaces = false
+
+[tool.ruff]
+exclude = ["*__init__.py"]
+ignore = ["E501"]
+select = [
+    "E",
+    "F",
+    "W",
+    "B",
+    "I",
+    "UP",
 ]
 
+[tool.ruff.isort]
+combine-as-imports = true
+
 [tool.mypy]
 python_version = "3.8"
 warn_unused_configs = true
 warn_unused_ignores = true
 warn_unreachable = true
 show_error_context = true
 show_error_codes = true
 disallow_untyped_defs = true
+ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
 module = "tests.*"
 disallow_untyped_defs = true
 ignore_errors = true
 
 [tool.pytest.ini_options]
 filterwarnings = [
     "error",
 ]
 addopts = "--doctest-modules"
 testpaths = ["tests"]
-
-[tool.setuptools]
-license-files = [
-    "LICENSE",
-]
-include-package-data = false
-
-[tool.setuptools.packages.find]
-namespaces = false
```

### Comparing `cmyt-1.1.3/tests/test_integration.py` & `cmyt-1.2.0/tests/test_integration.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import pytest
 
 import cmyt
-from cmyt.utils import cmyt_cmaps
-from cmyt.utils import prefix_name
+from cmyt.utils import cmyt_cmaps, prefix_name
 
 mpl_compare = pytest.mark.mpl_image_compare(
     savefig_kwargs={"bbox_inches": "tight"},
     style="default",
     tolerance=10,
 )
```

### Comparing `cmyt-1.1.3/tests/test_utils.py` & `cmyt-1.2.0/tests/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import pytest
 
 import cmyt  # noqa: F401
 from cmyt.utils import create_cmap_overview
 
-
 mpl_compare = pytest.mark.mpl_image_compare(
     savefig_kwargs={"bbox_inches": "tight"},
     style="default",
 )
 
 
 @mpl_compare
```

