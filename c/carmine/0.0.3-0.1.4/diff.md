# Comparing `tmp/carmine-0.0.3.tar.gz` & `tmp/carmine-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carmine-0.0.3.tar", last modified: Wed Mar 22 12:37:40 2023, max compression
+gzip compressed data, was "carmine-0.1.4.tar", last modified: Sun Apr 16 10:30:13 2023, max compression
```

## Comparing `carmine-0.0.3.tar` & `carmine-0.1.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    10280 2023-03-13 16:39:00.652994 carmine-0.0.3/COPYING
--rw-r--r--   0        0        0    10280 2023-03-12 21:27:59.270487 carmine-0.0.3/LICENSES/Apache-2.0.txt
--rw-r--r--   0        0        0    17023 2023-03-12 21:27:58.962486 carmine-0.0.3/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0        0        0    18375 2023-03-12 21:27:59.574487 carmine-0.0.3/LICENSES/CC-BY-SA-4.0.txt
--rw-r--r--   0        0        0      119 2023-03-13 16:39:00.652994 carmine-0.0.3/LICENSES/LicenseRef-DCO-1.1-license.txt
--rw-r--r--   0        0        0     1496 2023-03-22 12:37:23.778062 carmine-0.0.3/README.md
--rw-r--r--   0        0        0      929 2023-03-22 12:35:48.621860 carmine-0.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-13 00:47:37.817234 carmine-0.0.3/src/carmine/__init__.py
--rw-r--r--   0        0        0      844 2023-03-20 15:33:37.686508 carmine-0.0.3/src/carmine/cli.py
--rw-r--r--   0        0        0      208 2023-03-13 01:14:34.326480 carmine-0.0.3/tests/test_cli.py
--rw-r--r--   0        0        0     1744 1970-01-01 00:00:00.000000 carmine-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    10280 2023-04-16 10:05:48.022311 carmine-0.1.4/COPYING
+-rw-r--r--   0        0        0    10280 2023-03-12 21:27:59.270487 carmine-0.1.4/LICENSES/Apache-2.0.txt
+-rw-r--r--   0        0        0    17023 2023-03-12 21:27:58.962486 carmine-0.1.4/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0        0        0    18375 2023-03-12 21:27:59.574487 carmine-0.1.4/LICENSES/CC-BY-SA-4.0.txt
+-rw-r--r--   0        0        0      119 2023-04-16 10:05:48.022311 carmine-0.1.4/LICENSES/LicenseRef-DCO-1.1-license.txt
+-rw-r--r--   0        0        0     2005 2023-04-16 10:30:06.540813 carmine-0.1.4/README.md
+-rw-r--r--   0        0        0     1021 2023-04-16 10:30:13.952786 carmine-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-03 19:58:28.554502 carmine-0.1.4/src/carmine/__init__.py
+-rw-r--r--   0        0        0      737 2023-04-16 10:26:21.322208 carmine-0.1.4/src/carmine/cli.py
+-rw-r--r--   0        0        0      208 2023-03-13 01:14:34.326480 carmine-0.1.4/tests/test_cli.py
+-rw-r--r--   0        0        0     2692 1970-01-01 00:00:00.000000 carmine-0.1.4/PKG-INFO
```

### Comparing `carmine-0.0.3/COPYING` & `carmine-0.1.4/COPYING`

 * *Files identical despite different names*

### Comparing `carmine-0.0.3/LICENSES/Apache-2.0.txt` & `carmine-0.1.4/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `carmine-0.0.3/LICENSES/CC-BY-4.0.txt` & `carmine-0.1.4/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `carmine-0.0.3/LICENSES/CC-BY-SA-4.0.txt` & `carmine-0.1.4/LICENSES/CC-BY-SA-4.0.txt`

 * *Files identical despite different names*

### Comparing `carmine-0.0.3/README.md` & `carmine-0.1.4/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -5,37 +5,59 @@
 ## Usage
 
 Add `carmine` as a developer dependency, and all the included tools will be
 available for documentation, linting and testing.
 
 Run `carmine` to see a list of top-level dependencies and version numbers.
 
-### Documentation
+For documentation on individual tools, see links below.
+
+### Document toolchain
 
 - [mkdocs](https://www.mkdocs.org)
 
     - [mdformat_mkdocs](https://pypi.org/project/mdformat_mkdocs/)
     - [mkdocs-awesome-pages-plugin](https://pypi.org/project/mkdocs-awesome-pages-plugin/)
     - [mkdocs-mermaid2-plugin](https://pypi.org/project/mkdocs-mermaid2-plugin/)
 
-### Linting
+### Linter toolchain
 
 - [black](https://black.readthedocs.io/en/stable/)
 
 - [mdformat](https://mdformat.readthedocs.io/en/stable/)
 
 - [reuse](https://reuse.software)
 
-### Testing
+### Testing toolchain
 
 - [coverage](https://coverage.readthedocs.io/en/stable/)
 
 - [pytest](https://docs.pytest.org/en/stable/)
 
-For more details on intended use see `syllabub`.
+### Under consideration
+
+- [duty](https://pawamoy.github.io/duty/)
+
+- [griffe](https://mkdocstrings.github.io/griffe/)
+
+- [mkdocs-coverage](https://pawamoy.github.io/mkdocs-coverage/)
+
+- [mkdocstrings](https://mkdocstrings.github.io)
+
+### Recommended extras
+
+**Command line interface**
+
+- [Click](https://palletsprojects.com/p/click/)
+
+- [mkdocs-click](https://pypi.org/project/mkdocs-click/)
+
+**Slides**
+
+- [slide-template](https://github.com/fhiegel/slide-template) (MkDocs)
 
 <!-- start @generated footer -->
 
 # Sharing and contributions
 
 ```
 Carmine toolchain
@@ -45,9 +67,9 @@
 ```
 
 Shared under Apache-2.0. We adhere to the Contributor Covenant 2.1, and certify
 origin per DCO 1.1 with a signed-off-by line. Contributions under the same
 terms are welcome.
 
 Submit security and conduct issues as private tickets. Sign commits with
-`git commit --signoff`. For a software bill of materials run `reuse sbom`. For
+`git commit --signoff`. For a software bill of materials run `reuse spdx`. For
 more details see CONDUCT, COPYING and CONTRIBUTING.
```

### Comparing `carmine-0.0.3/pyproject.toml` & `carmine-0.1.4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 [project]
 name = "carmine"
-version = "0.0.3"
 description = "An opinionated Python toolchain made by crushing bugs."
 authors = [
     { name = "David Seaward", email = "david@librem.one" },
 ]
 dependencies = [
     "black ~= 23.0",
     "coverage>=7.2.1",
@@ -14,27 +13,34 @@
     "mkdocs-awesome-pages-plugin>=2.8.0",
     "mkdocs-mermaid2-plugin>=0.6.0",
     "pytest>=7.2.2",
     "reuse>=1.1.2",
 ]
 requires-python = ">=3.10"
 readme = "README.md"
+dynamic = []
+version = "0.1.4"
 
 [project.license]
 text = "Apache-2.0"
 
 [project.scripts]
 carmine = "carmine.cli:invoke"
 
+[project.urls]
+Source = "https://gitlab.com/lfdo/toolchain/carmine"
+Project = "https://lofidevops.neocities.org"
+
 [build-system]
 requires = [
-    "pdm-pep517>=1.0.0",
+    "pdm-backend",
 ]
-build-backend = "pdm.pep517.api"
+build-backend = "pdm.backend"
+
+[tool.pdm.version]
+source = "scm"
 
 [tool.syllabub.project]
 conduct = "contributor-covenant-2.1"
 copyright = "Copyright 2023 David Seaward and contributors"
 origin = "DCO-1.1-git-signoff"
-sbom = "reuse sbom"
 title = "Carmine toolchain"
-url = "https://lofidevops.neocities.org"
```

### Comparing `carmine-0.0.3/src/carmine/cli.py` & `carmine-0.1.4/src/carmine/cli.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # SPDX-License-Identifier: Apache-2.0
 # SPDX-FileCopyrightText: Copyright 2023 David Seaward and contributors
 
-import black
-import coverage
-import mdformat
-import mdformat_mkdocs
-import mkdocs
-import pytest
-import reuse
+from importlib.metadata import version, PackageNotFoundError
 
-# import mkdocs_awesome_pages_plugin
-# import mermaid2
 
+def get_version(package_name):
+    try:
+        return version(package_name)
+    except PackageNotFoundError:
+        return "unknown"
 
-def invoke():
-    versions = {
-        "black": black.__version__,
-        "coverage": coverage.__version__,
-        "mdformat": mdformat.__version__,
-        "mdformat_mkdocs": mdformat_mkdocs.__version__,
-        "mkdocs": mkdocs.__version__,
-        "mkdocs_awesome_pages_plugin": "No builtin value",
-        "mkdocs_mermaid2_plugin": "No builtin value",
-        "pytest": pytest.__version__,
-        "reuse": reuse.__version__,
-    }
 
-    for library, version in versions.items():
-        print(f"{library}: {version}")
+def invoke():
+    package_list = [
+        "carmine",
+        "black",
+        "coverage",
+        "mdformat",
+        "mdformat_mkdocs",
+        "mkdocs",
+        "mkdocs_awesome_pages_plugin",
+        "mkdocs_mermaid2_plugin",
+        "pytest",
+        "reuse",
+    ]
+
+    for package in package_list:
+        _version = get_version(package)
+        print(f"{package}: {_version}")
 
 
 if __name__ == "__main__":
     invoke()
```

### Comparing `carmine-0.0.3/PKG-INFO` & `carmine-0.1.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,83 @@
 Metadata-Version: 2.1
 Name: carmine
-Version: 0.0.3
+Version: 0.1.4
 Summary: An opinionated Python toolchain made by crushing bugs.
+Author-Email: David Seaward <david@librem.one>
 License: Apache-2.0
-Author-email: David Seaward <david@librem.one>
+Project-URL: Source, https://gitlab.com/lfdo/toolchain/carmine
+Project-URL: Project, https://lofidevops.neocities.org
 Requires-Python: >=3.10
+Requires-Dist: black~=23.0
+Requires-Dist: coverage>=7.2.1
+Requires-Dist: mdformat>=0.7.16
+Requires-Dist: mdformat_mkdocs[recommended]>=1.0.0
+Requires-Dist: mkdocs>=1.4.2
+Requires-Dist: mkdocs-awesome-pages-plugin>=2.8.0
+Requires-Dist: mkdocs-mermaid2-plugin>=0.6.0
+Requires-Dist: pytest>=7.2.2
+Requires-Dist: reuse>=1.1.2
 Description-Content-Type: text/markdown
 
 # Carmine toolchain
 
 An opinionated Python toolchain made by crushing bugs.
 
 ## Usage
 
 Add `carmine` as a developer dependency, and all the included tools will be
 available for documentation, linting and testing.
 
 Run `carmine` to see a list of top-level dependencies and version numbers.
 
-### Documentation
+For documentation on individual tools, see links below.
+
+### Document toolchain
 
 - [mkdocs](https://www.mkdocs.org)
 
     - [mdformat_mkdocs](https://pypi.org/project/mdformat_mkdocs/)
     - [mkdocs-awesome-pages-plugin](https://pypi.org/project/mkdocs-awesome-pages-plugin/)
     - [mkdocs-mermaid2-plugin](https://pypi.org/project/mkdocs-mermaid2-plugin/)
 
-### Linting
+### Linter toolchain
 
 - [black](https://black.readthedocs.io/en/stable/)
 
 - [mdformat](https://mdformat.readthedocs.io/en/stable/)
 
 - [reuse](https://reuse.software)
 
-### Testing
+### Testing toolchain
 
 - [coverage](https://coverage.readthedocs.io/en/stable/)
 
 - [pytest](https://docs.pytest.org/en/stable/)
 
-For more details on intended use see `syllabub`.
+### Under consideration
+
+- [duty](https://pawamoy.github.io/duty/)
+
+- [griffe](https://mkdocstrings.github.io/griffe/)
+
+- [mkdocs-coverage](https://pawamoy.github.io/mkdocs-coverage/)
+
+- [mkdocstrings](https://mkdocstrings.github.io)
+
+### Recommended extras
+
+**Command line interface**
+
+- [Click](https://palletsprojects.com/p/click/)
+
+- [mkdocs-click](https://pypi.org/project/mkdocs-click/)
+
+**Slides**
+
+- [slide-template](https://github.com/fhiegel/slide-template) (MkDocs)
 
 <!-- start @generated footer -->
 
 # Sharing and contributions
 
 ```
 Carmine toolchain
@@ -54,10 +87,9 @@
 ```
 
 Shared under Apache-2.0. We adhere to the Contributor Covenant 2.1, and certify
 origin per DCO 1.1 with a signed-off-by line. Contributions under the same
 terms are welcome.
 
 Submit security and conduct issues as private tickets. Sign commits with
-`git commit --signoff`. For a software bill of materials run `reuse sbom`. For
+`git commit --signoff`. For a software bill of materials run `reuse spdx`. For
 more details see CONDUCT, COPYING and CONTRIBUTING.
-
```

