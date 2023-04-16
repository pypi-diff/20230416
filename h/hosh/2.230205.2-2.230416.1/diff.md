# Comparing `tmp/hosh-2.230205.2.tar.gz` & `tmp/hosh-2.230416.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hosh-2.230205.2.tar", max compression
+gzip compressed data, was "hosh-2.230416.1.tar", max compression
```

## Comparing `hosh-2.230205.2.tar` & `hosh-2.230416.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    35149 2022-08-11 20:05:58.000000 hosh-2.230205.2/LICENSE
--rw-r--r--   0        0        0     9697 2023-02-05 21:54:51.186998 hosh-2.230205.2/README.md
--rw-r--r--   0        0        0      728 2023-02-05 21:54:52.599017 hosh-2.230205.2/pyproject.toml
--rw-r--r--   0        0        0     2731 2023-02-05 16:58:49.804449 hosh-2.230205.2/src/hosh/__init__.py
--rw-r--r--   0        0        0     3217 2023-02-05 21:38:14.080692 hosh-2.230205.2/src/hosh/_internals_appearance.py
--rw-r--r--   0        0        0    10119 2023-02-05 21:48:03.293153 hosh-2.230205.2/src/hosh/config.py
--rw-r--r--   0        0        0     3254 2022-08-11 20:05:58.000000 hosh-2.230205.2/src/hosh/groups.py
--rw-r--r--   0        0        0    30399 2023-02-05 21:48:38.821663 hosh-2.230205.2/src/hosh/hosh_.py
--rw-r--r--   0        0        0     2213 2022-12-26 18:24:18.000000 hosh-2.230205.2/src/hosh/misc/__init__.py
--rw-r--r--   0        0        0    20036 2023-02-05 21:36:36.059283 hosh-2.230205.2/src/hosh/misc/colors.py
--rw-r--r--   0        0        0     5875 2022-08-11 20:05:58.000000 hosh-2.230205.2/src/hosh/misc/core.py
--rw-r--r--   0        0        0     1077 2022-08-11 20:05:58.000000 hosh-2.230205.2/src/hosh/misc/encoding/__init__.py
--rw-r--r--   0        0        0     9083 2022-08-11 20:05:58.000000 hosh-2.230205.2/src/hosh/misc/encoding/base.py
--rw-r--r--   0        0        0     3585 2022-08-11 20:05:58.000000 hosh-2.230205.2/src/hosh/misc/encoding/base777.py
--rw-r--r--   0        0        0     1403 2023-02-05 17:10:51.354402 hosh-2.230205.2/src/hosh/misc/exception.py
--rw-r--r--   0        0        0     1517 2022-12-31 19:32:46.000000 hosh-2.230205.2/src/hosh/misc/helper.py
--rw-r--r--   0        0        0     4698 2023-01-23 22:12:19.000000 hosh-2.230205.2/src/hosh/misc/identity.py
--rw-r--r--   0        0        0     4503 2022-08-11 20:05:58.000000 hosh-2.230205.2/src/hosh/misc/math.py
--rw-r--r--   0        0        0     2168 2022-08-11 20:05:58.000000 hosh-2.230205.2/src/hosh/misc/root.py
--rw-r--r--   0        0        0     1130 2023-02-05 20:39:45.847564 hosh-2.230205.2/src/hosh/theme.py
--rw-r--r--   0        0        0    10713 1970-01-01 00:00:00.000000 hosh-2.230205.2/setup.py
--rw-r--r--   0        0        0    10416 1970-01-01 00:00:00.000000 hosh-2.230205.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-08-11 20:05:58.000000 hosh-2.230416.1/LICENSE
+-rw-r--r--   0        0        0     9771 2023-04-16 16:34:09.097573 hosh-2.230416.1/README.md
+-rw-r--r--   0        0        0      776 2023-04-16 16:34:10.929602 hosh-2.230416.1/pyproject.toml
+-rw-r--r--   0        0        0     2731 2023-02-05 16:58:49.804449 hosh-2.230416.1/src/hosh/__init__.py
+-rw-r--r--   0        0        0     3217 2023-02-05 21:38:14.080692 hosh-2.230416.1/src/hosh/_internals_appearance.py
+-rw-r--r--   0        0        0    10119 2023-02-05 21:48:03.293153 hosh-2.230416.1/src/hosh/config.py
+-rw-r--r--   0        0        0     3254 2022-08-11 20:05:58.000000 hosh-2.230416.1/src/hosh/groups.py
+-rw-r--r--   0        0        0    30936 2023-04-16 16:08:38.579183 hosh-2.230416.1/src/hosh/hosh_.py
+-rw-r--r--   0        0        0     2213 2022-12-26 18:24:18.000000 hosh-2.230416.1/src/hosh/misc/__init__.py
+-rw-r--r--   0        0        0    20036 2023-02-05 21:36:36.059283 hosh-2.230416.1/src/hosh/misc/colors.py
+-rw-r--r--   0        0        0     5875 2022-08-11 20:05:58.000000 hosh-2.230416.1/src/hosh/misc/core.py
+-rw-r--r--   0        0        0     1077 2022-08-11 20:05:58.000000 hosh-2.230416.1/src/hosh/misc/encoding/__init__.py
+-rw-r--r--   0        0        0     9083 2022-08-11 20:05:58.000000 hosh-2.230416.1/src/hosh/misc/encoding/base.py
+-rw-r--r--   0        0        0     3585 2022-08-11 20:05:58.000000 hosh-2.230416.1/src/hosh/misc/encoding/base777.py
+-rw-r--r--   0        0        0     1403 2023-02-05 17:10:51.354402 hosh-2.230416.1/src/hosh/misc/exception.py
+-rw-r--r--   0        0        0     1517 2022-12-31 19:32:46.000000 hosh-2.230416.1/src/hosh/misc/helper.py
+-rw-r--r--   0        0        0     4698 2023-01-23 22:12:19.000000 hosh-2.230416.1/src/hosh/misc/identity.py
+-rw-r--r--   0        0        0     4503 2022-08-11 20:05:58.000000 hosh-2.230416.1/src/hosh/misc/math.py
+-rw-r--r--   0        0        0     2168 2022-08-11 20:05:58.000000 hosh-2.230416.1/src/hosh/misc/root.py
+-rw-r--r--   0        0        0     1130 2023-02-05 20:39:45.847564 hosh-2.230416.1/src/hosh/theme.py
+-rw-r--r--   0        0        0    10787 1970-01-01 00:00:00.000000 hosh-2.230416.1/setup.py
+-rw-r--r--   0        0        0    10490 1970-01-01 00:00:00.000000 hosh-2.230416.1/PKG-INFO
```

### Comparing `hosh-2.230205.2/LICENSE` & `hosh-2.230416.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hosh-2.230205.2/README.md` & `hosh-2.230416.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ![test](https://github.com/davips/hosh/workflows/test/badge.svg)
 [![codecov](https://codecov.io/gh/davips/hosh/branch/main/graph/badge.svg)](https://codecov.io/gh/davips/hosh)
 <a href="https://pypi.org/project/hosh">
 <img src="https://img.shields.io/pypi/v/hosh.svg?label=release&color=blue&style=flat-square" alt="pypi">
 </a>
-![Python version](https://img.shields.io/badge/python-3.8%20%7C%203.9-blue.svg)
+![Python version](https://img.shields.io/badge/python-≥3.8-blue.svg)
 [![license: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5501845.svg)](https://doi.org/10.5281/zenodo.5501845)
 [![arXiv](https://img.shields.io/badge/arXiv-2109.06028-b31b1b.svg?style=flat-square)](https://arxiv.org/abs/2109.06028)
 [![API documentation](https://img.shields.io/badge/API-autogenerated-a030a0.svg)](https://davips.github.io/hosh)
 [![Manual](https://img.shields.io/badge/manual-handcrafted-a030a0.svg)](https://hosh.page)
-
+[![Downloads](https://static.pepy.tech/badge/hosh)](https://pepy.tech/project/hosh)
 
 # hosh - Identification based on group theory
 [Website](https://hosh.page) |
 [Latest Release](https://pypi.org/project/hosh) |
 [Current Code](https://github.com/davips/hosh) |
 [API Documentation](https://davips.github.io/hosh)
```

#### html2text {}

```diff
@@ -1,35 +1,36 @@
 ![test](https://github.com/davips/hosh/workflows/test/badge.svg) [![codecov]
 (https://codecov.io/gh/davips/hosh/branch/main/graph/badge.svg)](https://
 codecov.io/gh/davips/hosh) [pypi] ![Python version](https://img.shields.io/
-badge/python-3.8%20%7C%203.9-blue.svg) [![license: GPL v3](https://
-img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-
-3.0) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5501845.svg)](https://
-doi.org/10.5281/zenodo.5501845) [![arXiv](https://img.shields.io/badge/arXiv-
-2109.06028-b31b1b.svg?style=flat-square)](https://arxiv.org/abs/2109.06028) [!
-[API documentation](https://img.shields.io/badge/API-autogenerated-a030a0.svg)]
+badge/python-â¥3.8-blue.svg) [![license: GPL v3](https://img.shields.io/badge/
+License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) [![DOI](https://
+zenodo.org/badge/DOI/10.5281/zenodo.5501845.svg)](https://doi.org/10.5281/
+zenodo.5501845) [![arXiv](https://img.shields.io/badge/arXiv-2109.06028-
+b31b1b.svg?style=flat-square)](https://arxiv.org/abs/2109.06028) [![API
+documentation](https://img.shields.io/badge/API-autogenerated-a030a0.svg)]
 (https://davips.github.io/hosh) [![Manual](https://img.shields.io/badge/manual-
-handcrafted-a030a0.svg)](https://hosh.page) # hosh - Identification based on
-group theory [Website](https://hosh.page) | [Latest Release](https://pypi.org/
-project/hosh) | [Current Code](https://github.com/davips/hosh) | [API
-Documentation](https://davips.github.io/hosh) This [Python library](https://
-pypi.org/project/hosh) / [code](https://github.com/davips/hosh) provides a
-reference implementation for the UT*.4 specification presented [here](https://
-arxiv.org/abs/2109.06028). A previous version, containing extra group theory
-content, is available in the package [GaROUPa](https://pypi.org/project/
-garoupa). Please see the [website](https://hosh.page) for more detailed usage
-information. We adopt a novel paradigm to universally unique identification
-(UUID), making identifiers deterministic and predictable, even before an object
-is generated by a (possibly costly) process. Here, data versioning and
-composition of processing steps are directly mapped as simple operations over
-identifiers. We call each of the latter a `Hosh`, i.e., an identifier is an
-_**o**perable **h**a**sh**_. A first implementation of the remaining ideas from
-the [paper](https://arxiv.org/abs/2109.06028) is provided in this [cacheable
-lazy dict](https://pypi.org/project/ldict/2.211016.3) which depends on `hosh`
-and serves as an advanced usage example.
+handcrafted-a030a0.svg)](https://hosh.page) [![Downloads](https://
+static.pepy.tech/badge/hosh)](https://pepy.tech/project/hosh) # hosh -
+Identification based on group theory [Website](https://hosh.page) | [Latest
+Release](https://pypi.org/project/hosh) | [Current Code](https://github.com/
+davips/hosh) | [API Documentation](https://davips.github.io/hosh) This [Python
+library](https://pypi.org/project/hosh) / [code](https://github.com/davips/
+hosh) provides a reference implementation for the UT*.4 specification presented
+[here](https://arxiv.org/abs/2109.06028). A previous version, containing extra
+group theory content, is available in the package [GaROUPa](https://pypi.org/
+project/garoupa). Please see the [website](https://hosh.page) for more detailed
+usage information. We adopt a novel paradigm to universally unique
+identification (UUID), making identifiers deterministic and predictable, even
+before an object is generated by a (possibly costly) process. Here, data
+versioning and composition of processing steps are directly mapped as simple
+operations over identifiers. We call each of the latter a `Hosh`, i.e., an
+identifier is an _**o**perable **h**a**sh**_. A first implementation of the
+remaining ideas from the [paper](https://arxiv.org/abs/2109.06028) is provided
+in this [cacheable lazy dict](https://pypi.org/project/ldict/2.211016.3) which
+depends on `hosh` and serves as an advanced usage example.
 A second (entirely rewritten) version is available in the package [idict]
 (https://pypi.org/project/idict), succeeded by [hoshmap](https://pypi.org/
 project/hoshmap). The most recent rewritten version of a hosh-based dict (and
 the most robust, recommended, one) is available in the package [hdict](https://
 pypi.org/project/hdict). ## Overview A product of identifiers produces a new
 identifier as shown below, where sequences of bytes (`b"..."`) are passed to
 simulate binary objects to be hashed. ![img.png](https://
```

### Comparing `hosh-2.230205.2/pyproject.toml` & `hosh-2.230416.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [tool.poetry]
 name = "hosh"
-version = "2.230205.2"
+version = "2.230416.1"
 description = "Predictable Operable HaSH-based identifiers"
 authors = ["davips <dpsabc@gmail.com>"]
 license = "GPL"
 readme = 'README.md'
 packages = [
     { include = "hosh", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
-wheel = "^0.37.0"
-blake3 = "^0.2.0"
-colored = "1.4.2"
+wheel = "^0.40.0"
+blake3 = "^0.3.3"
+colored = "1.4.2" # Newer minor version has breaking changes.
 ansi2html = "^1.6.0"
 bs4 = "^0.0.1"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 pdoc3 = "^0.10.0"
-autoreadme = "^0.2102.20"
-pytest = "^6.2.5"
-pytest-cov = "^2.12.1"
+pytest = "^7.3.1"
+pytest-cov = "^4.0.0"
 ipython = "^7.27.0"
 black = "^21.9b0"
 flake8 = "^4.0.1"
+autoreadme = "^0.2302.3"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 # 
 # [[tool.poetry.source]]
 # name = "dvpypi"
```

### Comparing `hosh-2.230205.2/src/hosh/__init__.py` & `hosh-2.230416.1/src/hosh/__init__.py`

 * *Files identical despite different names*

### Comparing `hosh-2.230205.2/src/hosh/_internals_appearance.py` & `hosh-2.230416.1/src/hosh/_internals_appearance.py`

 * *Files identical despite different names*

### Comparing `hosh-2.230205.2/src/hosh/config.py` & `hosh-2.230416.1/src/hosh/config.py`

 * *Files identical despite different names*

### Comparing `hosh-2.230205.2/src/hosh/groups.py` & `hosh-2.230416.1/src/hosh/groups.py`

 * *Files identical despite different names*

### Comparing `hosh-2.230205.2/src/hosh/hosh_.py` & `hosh-2.230416.1/src/hosh/hosh_.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,17 +184,28 @@
 
         >>> from hosh import Hosh
         >>> h = Hosh.fromid("J5.uRTue8X4r1xu.JFkPbURVVGvTRPSFLncXdyzj").rev
         >>> h.id
         'jzydXcnLFSPRTvGVVRUbPkFJ.ux1r4X8euTRu.5J'
         >>> "".join(reversed(h.id))
         'J5.uRTue8X4r1xu.JFkPbURVVGvTRPSFLncXdyzj'
+        >>> h = Hosh.fromid("ab_cabcdefabcdefabcdefabcdefabcdefabcdef")
+        >>> h.rev.id
+        'fe_dcbafedcbafedcbafedcbafedcbafedcbacba'
+        >>> h = Hosh.fromid("2_dbe78441d_____________________________")
+        >>> h.rev.id
+        'd_14487ebd2_____________________________'
         """
         if self._rev is None:
-            self._rev = Hosh.fromid("".join(reversed(self.id)))
+            id = self.id
+            if self.etype == "hybrid":
+                id = id[:2] + id[3:-2] + "_" + id[-2:]
+            elif self.etype == "unordered":
+                id = "_____________________________" + id[:1] + id[2:10] + "_" + id[10:11]
+            self._rev = Hosh.fromid("".join(reversed(id)))
         return self._rev
 
     @property
     def etype(self):
         """
         Type of this element
```

### Comparing `hosh-2.230205.2/src/hosh/misc/__init__.py` & `hosh-2.230416.1/src/hosh/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `hosh-2.230205.2/src/hosh/misc/colors.py` & `hosh-2.230416.1/src/hosh/misc/colors.py`

 * *Files identical despite different names*

### Comparing `hosh-2.230205.2/src/hosh/misc/core.py` & `hosh-2.230416.1/src/hosh/misc/core.py`

 * *Files identical despite different names*

### Comparing `hosh-2.230205.2/src/hosh/misc/encoding/__init__.py` & `hosh-2.230416.1/src/hosh/misc/encoding/__init__.py`

 * *Files identical despite different names*

### Comparing `hosh-2.230205.2/src/hosh/misc/encoding/base.py` & `hosh-2.230416.1/src/hosh/misc/encoding/base.py`

 * *Files identical despite different names*

### Comparing `hosh-2.230205.2/src/hosh/misc/encoding/base777.py` & `hosh-2.230416.1/src/hosh/misc/encoding/base777.py`

 * *Files identical despite different names*

### Comparing `hosh-2.230205.2/src/hosh/misc/exception.py` & `hosh-2.230416.1/src/hosh/misc/exception.py`

 * *Files identical despite different names*

### Comparing `hosh-2.230205.2/src/hosh/misc/helper.py` & `hosh-2.230416.1/src/hosh/misc/helper.py`

 * *Files identical despite different names*

### Comparing `hosh-2.230205.2/src/hosh/misc/identity.py` & `hosh-2.230416.1/src/hosh/misc/identity.py`

 * *Files identical despite different names*

### Comparing `hosh-2.230205.2/src/hosh/misc/math.py` & `hosh-2.230416.1/src/hosh/misc/math.py`

 * *Files identical despite different names*

### Comparing `hosh-2.230205.2/src/hosh/misc/root.py` & `hosh-2.230416.1/src/hosh/misc/root.py`

 * *Files identical despite different names*

### Comparing `hosh-2.230205.2/src/hosh/theme.py` & `hosh-2.230416.1/src/hosh/theme.py`

 * *Files identical despite different names*

### Comparing `hosh-2.230205.2/setup.py` & `hosh-2.230416.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 ['hosh', 'hosh.misc', 'hosh.misc.encoding']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['ansi2html>=1.6.0,<2.0.0',
- 'blake3>=0.2.0,<0.3.0',
+ 'blake3>=0.3.3,<0.4.0',
  'bs4>=0.0.1,<0.0.2',
  'colored==1.4.2',
- 'wheel>=0.37.0,<0.38.0']
+ 'wheel>=0.40.0,<0.41.0']
 
 setup_kwargs = {
     'name': 'hosh',
-    'version': '2.230205.2',
+    'version': '2.230416.1',
     'description': 'Predictable Operable HaSH-based identifiers',
-    'long_description': '![test](https://github.com/davips/hosh/workflows/test/badge.svg)\n[![codecov](https://codecov.io/gh/davips/hosh/branch/main/graph/badge.svg)](https://codecov.io/gh/davips/hosh)\n<a href="https://pypi.org/project/hosh">\n<img src="https://img.shields.io/pypi/v/hosh.svg?label=release&color=blue&style=flat-square" alt="pypi">\n</a>\n![Python version](https://img.shields.io/badge/python-3.8%20%7C%203.9-blue.svg)\n[![license: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)\n\n[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5501845.svg)](https://doi.org/10.5281/zenodo.5501845)\n[![arXiv](https://img.shields.io/badge/arXiv-2109.06028-b31b1b.svg?style=flat-square)](https://arxiv.org/abs/2109.06028)\n[![API documentation](https://img.shields.io/badge/API-autogenerated-a030a0.svg)](https://davips.github.io/hosh)\n[![Manual](https://img.shields.io/badge/manual-handcrafted-a030a0.svg)](https://hosh.page)\n\n\n# hosh - Identification based on group theory\n[Website](https://hosh.page) |\n[Latest Release](https://pypi.org/project/hosh) |\n[Current Code](https://github.com/davips/hosh) |\n[API Documentation](https://davips.github.io/hosh)\n\nThis [Python library](https://pypi.org/project/hosh) / [code](https://github.com/davips/hosh) provides a reference implementation for the UT*.4 specification presented [here](https://arxiv.org/abs/2109.06028).\nA previous version, containing extra group theory content, is available in the package [GaROUPa](https://pypi.org/project/garoupa).\n\nPlease see the [website](https://hosh.page) for more detailed usage information.\n\nWe adopt a novel paradigm to universally unique identification (UUID), making identifiers deterministic and predictable, \neven before an object is generated by a (possibly costly) process.   \nHere, data versioning and composition of processing steps are directly mapped as simple operations over identifiers.\nWe call each of the latter a `Hosh`, i.e., an identifier is an _**o**perable **h**a**sh**_.\n\nA first implementation of the remaining ideas from the [paper](https://arxiv.org/abs/2109.06028) is provided in this\n[cacheable lazy dict](https://pypi.org/project/ldict/2.211016.3) which depends on `hosh` and serves as an advanced usage example.\n<br>\nA second (entirely rewritten) version is available in the package [idict](https://pypi.org/project/idict), succeeded by [hoshmap](https://pypi.org/project/hoshmap).\nThe most recent rewritten version of a hosh-based dict (and the most robust, recommended, one) is available in the package [hdict](https://pypi.org/project/hdict).\n\n\n## Overview\nA product of identifiers produces a new identifier as shown below, where sequences of bytes (`b"..."`) are passed to simulate binary objects to be hashed.\n\n![img.png](https://raw.githubusercontent.com/davips/hosh/main/examples/img.png) | New identifiers are easily <br> created from the identity <br> element `ø`. Also available as `identity` for people <br>or systems allergic to <br>utf-8 encoding.\n-------------------------|-------------------------\n\n![img_1.png](https://raw.githubusercontent.com/davips/hosh/main/examples/img_1.png) | Operations can be reverted by the inverse of the identifier.\n-------------------------|-------------------------\n\n![img_2.png](https://raw.githubusercontent.com/davips/hosh/main/examples/img_2.png) | Operations are associative. <br>They are order-sensitive by default, <br>in which case they are called _ordered_ ids.\n-------------------------|-------------------------\n\nHowever, order-insensitive (called _unordered_) and order-insensitive-among-themselves (called _hybrid_) identifiers are also available. | .\n-------------------------|-------------------------\n![img_3.png](https://raw.githubusercontent.com/davips/hosh/main/examples/img_3.png) | .\n\nThis is how they affect each other: | .\n-------------------------|-------------------------\n![img_4.png](https://raw.githubusercontent.com/davips/hosh/main/examples/img_4.png) | .\n\nThe chance of collision is determined by the number of possible identifiers of each type.\nSome versions are provided, e.g.: UT32.4, UT40.4 (default), UT64.4.\nThey can be easily implemented in other languages and are \nintended to be a specification on how to identify multi-valued objects and multi-step processes.\nUnordered ids use a very narrow range of the total number of identifiers.\nThis is not a problem as they are not very useful.\n\nOne use for unordered ids could be the embedding of authorship or other metadata into an object without worrying about the timing, since the resulting id will remain the same, no matter when the unordered id is operated with the id of the object under construction. | . \n-------------------------|-------------------------\n![img_5.png](https://raw.githubusercontent.com/davips/hosh/main/examples/img_5.png) | . \n\nConversely, hybrid ids are excelent to represent values in a data structure like a map, \nsince the order is not relevant when the consumer process looks up for keys, not indexes.\nConverselly, a chain of a data processing functions usually implies one step is dependent on the result of the previous step.\nThis makes ordered ids the perfect fit to identify functions (and also their composition, as a consequence).\n\n### Relationships can also be represented\nHere is another possible use. ORCIDs are managed unique identifiers for researchers.\nThey can be directly used as digests to create operable identifiers.\nWe recommend the use of 40 digits to allow operations with SHA-1 hashes. \nThey are common in version control repositories among other uses.\n![img_orcid.png](https://raw.githubusercontent.com/davips/hosh/main/examples/img_orcid.png)\n\nUnordered relationships are represented by hybrid ids.\nAutomatic transparent conversion between ORCID dashes by a hexdecimal character can be implemented in the future if needed.\n![img_orcid-comm.png](https://raw.githubusercontent.com/davips/hosh/main/examples/img_orcid-comm.png)\n\n## More info\nAside from the [paper](https://arxiv.org/abs/2109.06028), [PyPI package](https://pypi.org/project/hosh) \nand [GitHub repository](https://github.com/davips/hosh), \none can find more information, at a higher level application perspective, \nin this presentation:\n![image](https://raw.githubusercontent.com/davips/hosh/14cb45b888eb8a18ae093d200075c1a8a7e9cacb/examples/capa-slides-gdocs.png)\nA lower level perspective is provided in the [API documentation](https://davips.github.io/hosh).\n\n## Python installation\n### from package\n```bash\n# Set up a virtualenv. \npython3 -m venv venv\nsource venv/bin/activate\n\n# Install from PyPI\npip install hosh\n```\n\n### from source\n```bash\ngit clone https://github.com/davips/hosh\ncd hosh\npoetry install\n```\n\n### Examples\nSome usage examples.\n\n**Basic operations**\n<details>\n<p>\n\n```python3\nfrom hosh import Hosh, ø  # ø is a shortcut for identity (AltGr+O in most keyboards)\n\n# Hoshes (operable hash-based elements) can be multiplied.\na = Hosh(content=b"Some large binary content...")\nb = Hosh(content=b"Some other binary content. Might be, e.g., an action or another large content.")\nc = a * b\nprint(f"{a} * {b} = {c}")\n"""\n8CG9so9N1nQ59uNO8HGYcZ4ExQW5Haw4mErvw8m8 * 7N-L-10JS-H5DN0-BXW2e5ENWFQFVWswyz39t8s9 = z3EgxfisgqbNXBd0eqDuFiaTblBLA5ZAUbvEZgOh\n"""\n```\n\n```python3\nprint(~b)\n# Multiplication can be reverted by the inverse hosh. Zero is the identity hosh.\nprint(f"{b} * {~b} = {b * ~b} = 0")\n"""\nQ6OjmYZSJ8pB3ogBVMKBOxVp-oZ80czvtUrSyTzS\n7N-L-10JS-H5DN0-BXW2e5ENWFQFVWswyz39t8s9 * Q6OjmYZSJ8pB3ogBVMKBOxVp-oZ80czvtUrSyTzS = 0000000000000000000000000000000000000000 = 0\n"""\n```\n\n```python3\n\nprint(f"{b} * {ø} = {b * ø} = b")\n"""\n7N-L-10JS-H5DN0-BXW2e5ENWFQFVWswyz39t8s9 * 0000000000000000000000000000000000000000 = 7N-L-10JS-H5DN0-BXW2e5ENWFQFVWswyz39t8s9 = b\n"""\n```\n\n```python3\n\nprint(f"{c} * {~b} = {c * ~b} = {a} = a")\n"""\nz3EgxfisgqbNXBd0eqDuFiaTblBLA5ZAUbvEZgOh * Q6OjmYZSJ8pB3ogBVMKBOxVp-oZ80czvtUrSyTzS = 8CG9so9N1nQ59uNO8HGYcZ4ExQW5Haw4mErvw8m8 = 8CG9so9N1nQ59uNO8HGYcZ4ExQW5Haw4mErvw8m8 = a\n"""\n```\n\n```python3\n\nprint(f"{~a} * {c} = {~a * c} = {b} = b")\n"""\nRNvSdLI-5RiBBGL8NekctiQofWUIeYvXFP3wvTFT * z3EgxfisgqbNXBd0eqDuFiaTblBLA5ZAUbvEZgOh = 7N-L-10JS-H5DN0-BXW2e5ENWFQFVWswyz39t8s9 = 7N-L-10JS-H5DN0-BXW2e5ENWFQFVWswyz39t8s9 = b\n"""\n```\n\n```python3\n\n# Division is shorthand for reversion.\nprint(f"{c} / {b} = {c / b} = a")\n"""\nz3EgxfisgqbNXBd0eqDuFiaTblBLA5ZAUbvEZgOh / 7N-L-10JS-H5DN0-BXW2e5ENWFQFVWswyz39t8s9 = 8CG9so9N1nQ59uNO8HGYcZ4ExQW5Haw4mErvw8m8 = a\n"""\n```\n\n```python3\n\n# Hosh multiplication is not expected to be commutative.\nprint(f"{a * b} != {b * a}")\n"""\nz3EgxfisgqbNXBd0eqDuFiaTblBLA5ZAUbvEZgOh != wwSd0LaGvuV0W-yEOfgB-yVBMlNLA5ZAUbvEZgOh\n"""\n```\n\n```python3\n\n# Hosh multiplication is associative.\nprint(f"{a * (b * c)} = {(a * b) * c}")\n"""\nRuTcC4ZIr0Y1QLzYmytPRc087a8cbbW9Nj-gXxAz = RuTcC4ZIr0Y1QLzYmytPRc087a8cbbW9Nj-gXxAz\n"""\n```\n\n\n</p>\n</details>\n\n\n## Performance\nComputation time for the simple operations performed by `hosh` can be considered negligible for most applications,\nsince the order of magnitude of creating and operating identifiers is around a few μs:\n![img_6.png](https://raw.githubusercontent.com/davips/hosh/main/examples/img_6.png)\nThe package [hoshrust](https://pypi.org/project/hoshrust) was a faster implementation of an earlier version of `hosh`.\nAs the performance of the current `hosh` seems already very high (only ~2x slower than if it was implemented in native code in like _rust_), \nwe don\'t have plans for a new \'rust\' implementation in the near future.\n\n## Grants\nThis work was partially supported by Fapesp under supervision of\nProf. André C. P. L. F. de Carvalho at CEPID-CeMEAI (Grants 2013/07375-0 – 2019/01735-0).\n',
+    'long_description': '![test](https://github.com/davips/hosh/workflows/test/badge.svg)\n[![codecov](https://codecov.io/gh/davips/hosh/branch/main/graph/badge.svg)](https://codecov.io/gh/davips/hosh)\n<a href="https://pypi.org/project/hosh">\n<img src="https://img.shields.io/pypi/v/hosh.svg?label=release&color=blue&style=flat-square" alt="pypi">\n</a>\n![Python version](https://img.shields.io/badge/python-≥3.8-blue.svg)\n[![license: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)\n\n[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5501845.svg)](https://doi.org/10.5281/zenodo.5501845)\n[![arXiv](https://img.shields.io/badge/arXiv-2109.06028-b31b1b.svg?style=flat-square)](https://arxiv.org/abs/2109.06028)\n[![API documentation](https://img.shields.io/badge/API-autogenerated-a030a0.svg)](https://davips.github.io/hosh)\n[![Manual](https://img.shields.io/badge/manual-handcrafted-a030a0.svg)](https://hosh.page)\n[![Downloads](https://static.pepy.tech/badge/hosh)](https://pepy.tech/project/hosh)\n\n# hosh - Identification based on group theory\n[Website](https://hosh.page) |\n[Latest Release](https://pypi.org/project/hosh) |\n[Current Code](https://github.com/davips/hosh) |\n[API Documentation](https://davips.github.io/hosh)\n\nThis [Python library](https://pypi.org/project/hosh) / [code](https://github.com/davips/hosh) provides a reference implementation for the UT*.4 specification presented [here](https://arxiv.org/abs/2109.06028).\nA previous version, containing extra group theory content, is available in the package [GaROUPa](https://pypi.org/project/garoupa).\n\nPlease see the [website](https://hosh.page) for more detailed usage information.\n\nWe adopt a novel paradigm to universally unique identification (UUID), making identifiers deterministic and predictable, \neven before an object is generated by a (possibly costly) process.   \nHere, data versioning and composition of processing steps are directly mapped as simple operations over identifiers.\nWe call each of the latter a `Hosh`, i.e., an identifier is an _**o**perable **h**a**sh**_.\n\nA first implementation of the remaining ideas from the [paper](https://arxiv.org/abs/2109.06028) is provided in this\n[cacheable lazy dict](https://pypi.org/project/ldict/2.211016.3) which depends on `hosh` and serves as an advanced usage example.\n<br>\nA second (entirely rewritten) version is available in the package [idict](https://pypi.org/project/idict), succeeded by [hoshmap](https://pypi.org/project/hoshmap).\nThe most recent rewritten version of a hosh-based dict (and the most robust, recommended, one) is available in the package [hdict](https://pypi.org/project/hdict).\n\n\n## Overview\nA product of identifiers produces a new identifier as shown below, where sequences of bytes (`b"..."`) are passed to simulate binary objects to be hashed.\n\n![img.png](https://raw.githubusercontent.com/davips/hosh/main/examples/img.png) | New identifiers are easily <br> created from the identity <br> element `ø`. Also available as `identity` for people <br>or systems allergic to <br>utf-8 encoding.\n-------------------------|-------------------------\n\n![img_1.png](https://raw.githubusercontent.com/davips/hosh/main/examples/img_1.png) | Operations can be reverted by the inverse of the identifier.\n-------------------------|-------------------------\n\n![img_2.png](https://raw.githubusercontent.com/davips/hosh/main/examples/img_2.png) | Operations are associative. <br>They are order-sensitive by default, <br>in which case they are called _ordered_ ids.\n-------------------------|-------------------------\n\nHowever, order-insensitive (called _unordered_) and order-insensitive-among-themselves (called _hybrid_) identifiers are also available. | .\n-------------------------|-------------------------\n![img_3.png](https://raw.githubusercontent.com/davips/hosh/main/examples/img_3.png) | .\n\nThis is how they affect each other: | .\n-------------------------|-------------------------\n![img_4.png](https://raw.githubusercontent.com/davips/hosh/main/examples/img_4.png) | .\n\nThe chance of collision is determined by the number of possible identifiers of each type.\nSome versions are provided, e.g.: UT32.4, UT40.4 (default), UT64.4.\nThey can be easily implemented in other languages and are \nintended to be a specification on how to identify multi-valued objects and multi-step processes.\nUnordered ids use a very narrow range of the total number of identifiers.\nThis is not a problem as they are not very useful.\n\nOne use for unordered ids could be the embedding of authorship or other metadata into an object without worrying about the timing, since the resulting id will remain the same, no matter when the unordered id is operated with the id of the object under construction. | . \n-------------------------|-------------------------\n![img_5.png](https://raw.githubusercontent.com/davips/hosh/main/examples/img_5.png) | . \n\nConversely, hybrid ids are excelent to represent values in a data structure like a map, \nsince the order is not relevant when the consumer process looks up for keys, not indexes.\nConverselly, a chain of a data processing functions usually implies one step is dependent on the result of the previous step.\nThis makes ordered ids the perfect fit to identify functions (and also their composition, as a consequence).\n\n### Relationships can also be represented\nHere is another possible use. ORCIDs are managed unique identifiers for researchers.\nThey can be directly used as digests to create operable identifiers.\nWe recommend the use of 40 digits to allow operations with SHA-1 hashes. \nThey are common in version control repositories among other uses.\n![img_orcid.png](https://raw.githubusercontent.com/davips/hosh/main/examples/img_orcid.png)\n\nUnordered relationships are represented by hybrid ids.\nAutomatic transparent conversion between ORCID dashes by a hexdecimal character can be implemented in the future if needed.\n![img_orcid-comm.png](https://raw.githubusercontent.com/davips/hosh/main/examples/img_orcid-comm.png)\n\n## More info\nAside from the [paper](https://arxiv.org/abs/2109.06028), [PyPI package](https://pypi.org/project/hosh) \nand [GitHub repository](https://github.com/davips/hosh), \none can find more information, at a higher level application perspective, \nin this presentation:\n![image](https://raw.githubusercontent.com/davips/hosh/14cb45b888eb8a18ae093d200075c1a8a7e9cacb/examples/capa-slides-gdocs.png)\nA lower level perspective is provided in the [API documentation](https://davips.github.io/hosh).\n\n## Python installation\n### from package\n```bash\n# Set up a virtualenv. \npython3 -m venv venv\nsource venv/bin/activate\n\n# Install from PyPI\npip install hosh\n```\n\n### from source\n```bash\ngit clone https://github.com/davips/hosh\ncd hosh\npoetry install\n```\n\n### Examples\nSome usage examples.\n\n**Basic operations**\n<details>\n<p>\n\n```python3\nfrom hosh import Hosh, ø  # ø is a shortcut for identity (AltGr+O in most keyboards)\n\n# Hoshes (operable hash-based elements) can be multiplied.\na = Hosh(content=b"Some large binary content...")\nb = Hosh(content=b"Some other binary content. Might be, e.g., an action or another large content.")\nc = a * b\nprint(f"{a} * {b} = {c}")\n"""\n8CG9so9N1nQ59uNO8HGYcZ4ExQW5Haw4mErvw8m8 * 7N-L-10JS-H5DN0-BXW2e5ENWFQFVWswyz39t8s9 = z3EgxfisgqbNXBd0eqDuFiaTblBLA5ZAUbvEZgOh\n"""\n```\n\n```python3\nprint(~b)\n# Multiplication can be reverted by the inverse hosh. Zero is the identity hosh.\nprint(f"{b} * {~b} = {b * ~b} = 0")\n"""\nQ6OjmYZSJ8pB3ogBVMKBOxVp-oZ80czvtUrSyTzS\n7N-L-10JS-H5DN0-BXW2e5ENWFQFVWswyz39t8s9 * Q6OjmYZSJ8pB3ogBVMKBOxVp-oZ80czvtUrSyTzS = 0000000000000000000000000000000000000000 = 0\n"""\n```\n\n```python3\n\nprint(f"{b} * {ø} = {b * ø} = b")\n"""\n7N-L-10JS-H5DN0-BXW2e5ENWFQFVWswyz39t8s9 * 0000000000000000000000000000000000000000 = 7N-L-10JS-H5DN0-BXW2e5ENWFQFVWswyz39t8s9 = b\n"""\n```\n\n```python3\n\nprint(f"{c} * {~b} = {c * ~b} = {a} = a")\n"""\nz3EgxfisgqbNXBd0eqDuFiaTblBLA5ZAUbvEZgOh * Q6OjmYZSJ8pB3ogBVMKBOxVp-oZ80czvtUrSyTzS = 8CG9so9N1nQ59uNO8HGYcZ4ExQW5Haw4mErvw8m8 = 8CG9so9N1nQ59uNO8HGYcZ4ExQW5Haw4mErvw8m8 = a\n"""\n```\n\n```python3\n\nprint(f"{~a} * {c} = {~a * c} = {b} = b")\n"""\nRNvSdLI-5RiBBGL8NekctiQofWUIeYvXFP3wvTFT * z3EgxfisgqbNXBd0eqDuFiaTblBLA5ZAUbvEZgOh = 7N-L-10JS-H5DN0-BXW2e5ENWFQFVWswyz39t8s9 = 7N-L-10JS-H5DN0-BXW2e5ENWFQFVWswyz39t8s9 = b\n"""\n```\n\n```python3\n\n# Division is shorthand for reversion.\nprint(f"{c} / {b} = {c / b} = a")\n"""\nz3EgxfisgqbNXBd0eqDuFiaTblBLA5ZAUbvEZgOh / 7N-L-10JS-H5DN0-BXW2e5ENWFQFVWswyz39t8s9 = 8CG9so9N1nQ59uNO8HGYcZ4ExQW5Haw4mErvw8m8 = a\n"""\n```\n\n```python3\n\n# Hosh multiplication is not expected to be commutative.\nprint(f"{a * b} != {b * a}")\n"""\nz3EgxfisgqbNXBd0eqDuFiaTblBLA5ZAUbvEZgOh != wwSd0LaGvuV0W-yEOfgB-yVBMlNLA5ZAUbvEZgOh\n"""\n```\n\n```python3\n\n# Hosh multiplication is associative.\nprint(f"{a * (b * c)} = {(a * b) * c}")\n"""\nRuTcC4ZIr0Y1QLzYmytPRc087a8cbbW9Nj-gXxAz = RuTcC4ZIr0Y1QLzYmytPRc087a8cbbW9Nj-gXxAz\n"""\n```\n\n\n</p>\n</details>\n\n\n## Performance\nComputation time for the simple operations performed by `hosh` can be considered negligible for most applications,\nsince the order of magnitude of creating and operating identifiers is around a few μs:\n![img_6.png](https://raw.githubusercontent.com/davips/hosh/main/examples/img_6.png)\nThe package [hoshrust](https://pypi.org/project/hoshrust) was a faster implementation of an earlier version of `hosh`.\nAs the performance of the current `hosh` seems already very high (only ~2x slower than if it was implemented in native code in like _rust_), \nwe don\'t have plans for a new \'rust\' implementation in the near future.\n\n## Grants\nThis work was partially supported by Fapesp under supervision of\nProf. André C. P. L. F. de Carvalho at CEPID-CeMEAI (Grants 2013/07375-0 – 2019/01735-0).\n',
     'author': 'davips',
     'author_email': 'dpsabc@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
```

#### html2text {}

```diff
@@ -1,31 +1,32 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['hosh', 'hosh.misc', 'hosh.misc.encoding'] package_data =
 \ {'': ['*']} install_requires = \ ['ansi2html>=1.6.0,<2.0.0',
-'blake3>=0.2.0,<0.3.0', 'bs4>=0.0.1,<0.0.2', 'colored==1.4.2',
-'wheel>=0.37.0,<0.38.0'] setup_kwargs = { 'name': 'hosh', 'version':
-'2.230205.2', 'description': 'Predictable Operable HaSH-based identifiers',
+'blake3>=0.3.3,<0.4.0', 'bs4>=0.0.1,<0.0.2', 'colored==1.4.2',
+'wheel>=0.40.0,<0.41.0'] setup_kwargs = { 'name': 'hosh', 'version':
+'2.230416.1', 'description': 'Predictable Operable HaSH-based identifiers',
 'long_description': '![test](https://github.com/davips/hosh/workflows/test/
 badge.svg)\n[![codecov](https://codecov.io/gh/davips/hosh/branch/main/graph/
 badge.svg)](https://codecov.io/gh/davips/hosh)\n\n[pypi]\n\n![Python version]
-(https://img.shields.io/badge/python-3.8%20%7C%203.9-blue.svg)\n[![license: GPL
-v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/
+(https://img.shields.io/badge/python-â¥3.8-blue.svg)\n[![license: GPL v3]
+(https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/
 licenses/gpl-3.0)\n\n[![DOI](https://zenodo.org/badge/DOI/10.5281/
 zenodo.5501845.svg)](https://doi.org/10.5281/zenodo.5501845)\n[![arXiv](https:/
 /img.shields.io/badge/arXiv-2109.06028-b31b1b.svg?style=flat-square)](https://
 arxiv.org/abs/2109.06028)\n[![API documentation](https://img.shields.io/badge/
 API-autogenerated-a030a0.svg)](https://davips.github.io/hosh)\n[![Manual]
 (https://img.shields.io/badge/manual-handcrafted-a030a0.svg)](https://
-hosh.page)\n\n\n# hosh - Identification based on group theory\n[Website](https:
-//hosh.page) |\n[Latest Release](https://pypi.org/project/hosh) |\n[Current
-Code](https://github.com/davips/hosh) |\n[API Documentation](https://
-davips.github.io/hosh)\n\nThis [Python library](https://pypi.org/project/hosh)
-/ [code](https://github.com/davips/hosh) provides a reference implementation
-for the UT*.4 specification presented [here](https://arxiv.org/abs/
-2109.06028).\nA previous version, containing extra group theory content, is
+hosh.page)\n[![Downloads](https://static.pepy.tech/badge/hosh)](https://
+pepy.tech/project/hosh)\n\n# hosh - Identification based on group theory\n
+[Website](https://hosh.page) |\n[Latest Release](https://pypi.org/project/hosh)
+|\n[Current Code](https://github.com/davips/hosh) |\n[API Documentation](https:
+//davips.github.io/hosh)\n\nThis [Python library](https://pypi.org/project/
+hosh) / [code](https://github.com/davips/hosh) provides a reference
+implementation for the UT*.4 specification presented [here](https://arxiv.org/
+abs/2109.06028).\nA previous version, containing extra group theory content, is
 available in the package [GaROUPa](https://pypi.org/project/garoupa).\n\nPlease
 see the [website](https://hosh.page) for more detailed usage information.\n\nWe
 adopt a novel paradigm to universally unique identification (UUID), making
 identifiers deterministic and predictable, \neven before an object is generated
 by a (possibly costly) process. \nHere, data versioning and composition of
 processing steps are directly mapped as simple operations over identifiers.\nWe
 call each of the latter a `Hosh`, i.e., an identifier is an _**o**perable
```

### Comparing `hosh-2.230205.2/PKG-INFO` & `hosh-2.230416.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 Metadata-Version: 2.1
 Name: hosh
-Version: 2.230205.2
+Version: 2.230416.1
 Summary: Predictable Operable HaSH-based identifiers
 License: GPL
 Author: davips
 Author-email: dpsabc@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ansi2html (>=1.6.0,<2.0.0)
-Requires-Dist: blake3 (>=0.2.0,<0.3.0)
+Requires-Dist: blake3 (>=0.3.3,<0.4.0)
 Requires-Dist: bs4 (>=0.0.1,<0.0.2)
 Requires-Dist: colored (==1.4.2)
-Requires-Dist: wheel (>=0.37.0,<0.38.0)
+Requires-Dist: wheel (>=0.40.0,<0.41.0)
 Description-Content-Type: text/markdown
 
 ![test](https://github.com/davips/hosh/workflows/test/badge.svg)
 [![codecov](https://codecov.io/gh/davips/hosh/branch/main/graph/badge.svg)](https://codecov.io/gh/davips/hosh)
 <a href="https://pypi.org/project/hosh">
 <img src="https://img.shields.io/pypi/v/hosh.svg?label=release&color=blue&style=flat-square" alt="pypi">
 </a>
-![Python version](https://img.shields.io/badge/python-3.8%20%7C%203.9-blue.svg)
+![Python version](https://img.shields.io/badge/python-≥3.8-blue.svg)
 [![license: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5501845.svg)](https://doi.org/10.5281/zenodo.5501845)
 [![arXiv](https://img.shields.io/badge/arXiv-2109.06028-b31b1b.svg?style=flat-square)](https://arxiv.org/abs/2109.06028)
 [![API documentation](https://img.shields.io/badge/API-autogenerated-a030a0.svg)](https://davips.github.io/hosh)
 [![Manual](https://img.shields.io/badge/manual-handcrafted-a030a0.svg)](https://hosh.page)
-
+[![Downloads](https://static.pepy.tech/badge/hosh)](https://pepy.tech/project/hosh)
 
 # hosh - Identification based on group theory
 [Website](https://hosh.page) |
 [Latest Release](https://pypi.org/project/hosh) |
 [Current Code](https://github.com/davips/hosh) |
 [API Documentation](https://davips.github.io/hosh)
```

#### html2text {}

```diff
@@ -1,45 +1,46 @@
-Metadata-Version: 2.1 Name: hosh Version: 2.230205.2 Summary: Predictable
+Metadata-Version: 2.1 Name: hosh Version: 2.230416.1 Summary: Predictable
 Operable HaSH-based identifiers License: GPL Author: davips Author-email:
 dpsabc@gmail.com Requires-Python: >=3.8 Classifier: License :: Other/
 Proprietary License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: ansi2html
-(>=1.6.0,<2.0.0) Requires-Dist: blake3 (>=0.2.0,<0.3.0) Requires-Dist: bs4
+(>=1.6.0,<2.0.0) Requires-Dist: blake3 (>=0.3.3,<0.4.0) Requires-Dist: bs4
 (>=0.0.1,<0.0.2) Requires-Dist: colored (==1.4.2) Requires-Dist: wheel
-(>=0.37.0,<0.38.0) Description-Content-Type: text/markdown ![test](https://
+(>=0.40.0,<0.41.0) Description-Content-Type: text/markdown ![test](https://
 github.com/davips/hosh/workflows/test/badge.svg) [![codecov](https://
 codecov.io/gh/davips/hosh/branch/main/graph/badge.svg)](https://codecov.io/gh/
 davips/hosh) [pypi] ![Python version](https://img.shields.io/badge/python-
-3.8%20%7C%203.9-blue.svg) [![license: GPL v3](https://img.shields.io/badge/
-License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) [![DOI](https://
+â¥3.8-blue.svg) [![license: GPL v3](https://img.shields.io/badge/License-
+GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) [![DOI](https://
 zenodo.org/badge/DOI/10.5281/zenodo.5501845.svg)](https://doi.org/10.5281/
 zenodo.5501845) [![arXiv](https://img.shields.io/badge/arXiv-2109.06028-
 b31b1b.svg?style=flat-square)](https://arxiv.org/abs/2109.06028) [![API
 documentation](https://img.shields.io/badge/API-autogenerated-a030a0.svg)]
 (https://davips.github.io/hosh) [![Manual](https://img.shields.io/badge/manual-
-handcrafted-a030a0.svg)](https://hosh.page) # hosh - Identification based on
-group theory [Website](https://hosh.page) | [Latest Release](https://pypi.org/
-project/hosh) | [Current Code](https://github.com/davips/hosh) | [API
-Documentation](https://davips.github.io/hosh) This [Python library](https://
-pypi.org/project/hosh) / [code](https://github.com/davips/hosh) provides a
-reference implementation for the UT*.4 specification presented [here](https://
-arxiv.org/abs/2109.06028). A previous version, containing extra group theory
-content, is available in the package [GaROUPa](https://pypi.org/project/
-garoupa). Please see the [website](https://hosh.page) for more detailed usage
-information. We adopt a novel paradigm to universally unique identification
-(UUID), making identifiers deterministic and predictable, even before an object
-is generated by a (possibly costly) process. Here, data versioning and
-composition of processing steps are directly mapped as simple operations over
-identifiers. We call each of the latter a `Hosh`, i.e., an identifier is an
-_**o**perable **h**a**sh**_. A first implementation of the remaining ideas from
-the [paper](https://arxiv.org/abs/2109.06028) is provided in this [cacheable
-lazy dict](https://pypi.org/project/ldict/2.211016.3) which depends on `hosh`
-and serves as an advanced usage example.
+handcrafted-a030a0.svg)](https://hosh.page) [![Downloads](https://
+static.pepy.tech/badge/hosh)](https://pepy.tech/project/hosh) # hosh -
+Identification based on group theory [Website](https://hosh.page) | [Latest
+Release](https://pypi.org/project/hosh) | [Current Code](https://github.com/
+davips/hosh) | [API Documentation](https://davips.github.io/hosh) This [Python
+library](https://pypi.org/project/hosh) / [code](https://github.com/davips/
+hosh) provides a reference implementation for the UT*.4 specification presented
+[here](https://arxiv.org/abs/2109.06028). A previous version, containing extra
+group theory content, is available in the package [GaROUPa](https://pypi.org/
+project/garoupa). Please see the [website](https://hosh.page) for more detailed
+usage information. We adopt a novel paradigm to universally unique
+identification (UUID), making identifiers deterministic and predictable, even
+before an object is generated by a (possibly costly) process. Here, data
+versioning and composition of processing steps are directly mapped as simple
+operations over identifiers. We call each of the latter a `Hosh`, i.e., an
+identifier is an _**o**perable **h**a**sh**_. A first implementation of the
+remaining ideas from the [paper](https://arxiv.org/abs/2109.06028) is provided
+in this [cacheable lazy dict](https://pypi.org/project/ldict/2.211016.3) which
+depends on `hosh` and serves as an advanced usage example.
 A second (entirely rewritten) version is available in the package [idict]
 (https://pypi.org/project/idict), succeeded by [hoshmap](https://pypi.org/
 project/hoshmap). The most recent rewritten version of a hosh-based dict (and
 the most robust, recommended, one) is available in the package [hdict](https://
 pypi.org/project/hdict). ## Overview A product of identifiers produces a new
 identifier as shown below, where sequences of bytes (`b"..."`) are passed to
 simulate binary objects to be hashed. ![img.png](https://
```

