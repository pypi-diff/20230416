# Comparing `tmp/asaman-0.1.6.tar.gz` & `tmp/asaman-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asaman-0.1.6.tar", last modified: Sun Oct  3 16:00:18 2021, max compression
+gzip compressed data, was "asaman-0.2.0.tar", last modified: Sun Apr 16 07:26:03 2023, max compression
```

## Comparing `asaman-0.1.6.tar` & `asaman-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 kdas      (1000) kdas      (1000)        0 2021-10-03 16:00:18.500541 asaman-0.1.6/
--rw-r--r--   0 kdas      (1000) kdas      (1000)     1066 2021-10-03 15:53:23.000000 asaman-0.1.6/LICENSE
--rw-r--r--   0 kdas      (1000) kdas      (1000)      148 2021-10-03 15:53:23.000000 asaman-0.1.6/MANIFEST.in
--rw-r--r--   0 kdas      (1000) kdas      (1000)     6304 2021-10-03 16:00:18.499541 asaman-0.1.6/PKG-INFO
--rw-r--r--   0 kdas      (1000) kdas      (1000)     5864 2021-10-03 15:55:14.000000 asaman-0.1.6/README.md
-drwxr-xr-x   0 kdas      (1000) kdas      (1000)        0 2021-10-03 16:00:18.499541 asaman-0.1.6/asaman/
--rw-r--r--   0 kdas      (1000) kdas      (1000)     9542 2021-10-03 15:53:23.000000 asaman-0.1.6/asaman/__init__.py
-drwxr-xr-x   0 kdas      (1000) kdas      (1000)        0 2021-10-03 16:00:18.499541 asaman-0.1.6/asaman.egg-info/
--rw-r--r--   0 kdas      (1000) kdas      (1000)     6304 2021-10-03 16:00:18.000000 asaman-0.1.6/asaman.egg-info/PKG-INFO
--rw-r--r--   0 kdas      (1000) kdas      (1000)      328 2021-10-03 16:00:18.000000 asaman-0.1.6/asaman.egg-info/SOURCES.txt
--rw-r--r--   0 kdas      (1000) kdas      (1000)        1 2021-10-03 16:00:18.000000 asaman-0.1.6/asaman.egg-info/dependency_links.txt
--rw-r--r--   0 kdas      (1000) kdas      (1000)       73 2021-10-03 16:00:18.000000 asaman-0.1.6/asaman.egg-info/entry_points.txt
--rw-r--r--   0 kdas      (1000) kdas      (1000)       30 2021-10-03 16:00:18.000000 asaman-0.1.6/asaman.egg-info/requires.txt
--rw-r--r--   0 kdas      (1000) kdas      (1000)        7 2021-10-03 16:00:18.000000 asaman-0.1.6/asaman.egg-info/top_level.txt
--rw-r--r--   0 kdas      (1000) kdas      (1000)       59 2021-10-03 15:53:23.000000 asaman-0.1.6/dev-requirements.in
--rw-r--r--   0 kdas      (1000) kdas      (1000)     2415 2021-10-03 15:53:23.000000 asaman-0.1.6/dev-requirements.txt
--rw-r--r--   0 kdas      (1000) kdas      (1000)      147 2021-10-03 15:53:23.000000 asaman-0.1.6/pyproject.toml
--rw-r--r--   0 kdas      (1000) kdas      (1000)       94 2021-10-03 15:53:23.000000 asaman-0.1.6/requirements.in
--rw-r--r--   0 kdas      (1000) kdas      (1000)     2358 2021-10-03 15:53:23.000000 asaman-0.1.6/requirements.txt
--rw-r--r--   0 kdas      (1000) kdas      (1000)       38 2021-10-03 16:00:18.500541 asaman-0.1.6/setup.cfg
--rw-r--r--   0 kdas      (1000) kdas      (1000)      890 2021-10-03 15:58:33.000000 asaman-0.1.6/setup.py
+-rw-r--r--   0        0        0      863 2023-03-09 09:29:11.152792 asaman-0.2.0/.github/workflows/github-actions.yml
+-rw-r--r--   0        0        0      266 2021-10-05 09:02:57.760675 asaman-0.2.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     1066 2021-10-03 15:53:23.164770 asaman-0.2.0/LICENSE
+-rw-r--r--   0        0        0     6961 2023-04-16 07:24:08.410438 asaman-0.2.0/README.md
+-rw-r--r--   0        0        0    12131 2023-04-16 07:24:08.410438 asaman-0.2.0/asaman/__init__.py
+-rw-r--r--   0        0        0     1380 2023-04-16 07:24:08.411438 asaman-0.2.0/dev-ci.txt
+-rw-r--r--   0        0        0      174 2023-04-16 07:24:08.411438 asaman-0.2.0/dev-requirements.in
+-rw-r--r--   0        0        0     1390 2023-04-16 07:24:08.411438 asaman-0.2.0/dev-requirements.txt
+-rw-r--r--   0        0        0      638 2021-10-05 05:06:13.614201 asaman-0.2.0/docs/Makefile
+-rw-r--r--   0        0        0      799 2021-10-05 05:06:13.616201 asaman-0.2.0/docs/make.bat
+-rw-r--r--   0        0        0       20 2021-10-05 09:04:05.395133 asaman-0.2.0/docs/requirements.txt
+-rw-r--r--   0        0        0     1885 2023-04-16 07:24:08.411438 asaman-0.2.0/docs/source/conf.py
+-rw-r--r--   0        0        0      654 2021-10-12 07:09:53.897433 asaman-0.2.0/docs/source/hacking.rst
+-rw-r--r--   0        0        0      568 2021-10-13 09:30:04.118485 asaman-0.2.0/docs/source/index.rst
+-rw-r--r--   0        0        0      196 2021-10-05 05:15:36.281858 asaman-0.2.0/docs/source/install.rst
+-rw-r--r--   0        0        0     4071 2023-03-09 08:59:08.269150 asaman-0.2.0/docs/source/usage.rst
+-rw-r--r--   0        0        0      746 2021-10-05 03:18:05.770095 asaman-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      151 2023-04-16 07:24:08.411438 asaman-0.2.0/requirements.in
+-rw-r--r--   0        0        0     2467 2023-04-16 07:24:08.411438 asaman-0.2.0/requirements.txt
+-rw-r--r--   0        0        0        3 2023-03-09 09:29:11.152792 asaman-0.2.0/test.in
+-rw-r--r--   0        0        0      759 2023-03-09 09:29:11.152792 asaman-0.2.0/test.txt
+-rw-r--r--   0        0        0       62 2021-10-06 04:36:45.710606 asaman-0.2.0/tests/test_requirements.py
+-rw-r--r--   0        0        0     7462 1970-01-01 00:00:00.000000 asaman-0.2.0/PKG-INFO
```

### Comparing `asaman-0.1.6/LICENSE` & `asaman-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asaman-0.1.6/PKG-INFO` & `asaman-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,24 @@
-Metadata-Version: 2.1
-Name: asaman
-Version: 0.1.6
-Summary: A tool to build reproducible wheels.
-Home-page: https://github.com/kushaldas/asaman
-Author: Kushal Das
-Author-email: mail@kushaldas.in
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
+# asaman: Amra Saman (আমরা সমান)
 
-## asaman: Amra Saman
+This is a tool to build reproducible wheels for your Python project or for all of your dependencies. What this means is if you use the same Operating System version and similar system level dependencies, you will always get the same wheel generated. This enables us to have a bit more protection from side-channel attacks. Any user of the wheels can verify that they are using the correct build from the exact source via verifying the builds themselves.
 
-This is a tool to build reproducible wheels for you Python project or for all of your dependencies. Means, if you use the same Operating System version and similar system level dependencies, you will always get the same wheel generated. Thus enabling us to have a bit more protection from side-channel attacks. Any user of the wheels can verify that they are using the correct build from the exact source via verifying the builds themselves.
 
 ## Why do we need a reproducible wheel?
 
 A few different positive points:
 
-- If we build the wheels from a known source (via pinned hashes in requirements file), we can also verify if we are using the correct wheels build from them.
-- Any user/developer can rebuild the wheels from the pinned source, and should get the exact same wheel as output. Thus if anything gets into the build process (say in CI), or the wheel is actually built from a different source, automated tools can identify those.
+- If we build the wheels from a known source (e.g. via pinned hashes in requirements file), we can also verify if we are using the correct wheels built from them.
+- Any user/developer can rebuild the wheels from the pinned source and should get the exact same wheel as output. Thus if anything gets into the build process (say in CI), or the wheel is actually built from a different source, automated tools can identify that difference.
 
 
 ## How to install?
 
 ```bash
-python3 -m pip install amrasaman
+python3 -m pip install asaman
 ```
 
 ## How to build reproducible wheels?
 
 ```
 asaman --help
 Usage: asaman [OPTIONS]
@@ -44,48 +30,54 @@
   -d, --directory DIRECTORY  A directory containing all source tarballs and
                              zips.
   -o, --output DIRECTORY     The output directory to store all wheel files.
                              Default: ./wheels
   -r, --requirement FILE     Path to the requirement.txt file which contains
                              all packages to build along with hashes.
   --sde TEXT                 Custom SOURCE_DATE_EPOCH value.
+  --no-hash                  DO NOT USE UNLESS VERY SURE: In case we skip hash
+                             checking for download.  [default: False]
+  --keep-sources             Copy over the sources to output directory
+                             [default: False]
+  --with-index TEXT          In case you want to install build time
+                             dependencies from an index, pass the URL.
+                             [default: ]
+  --trusted-host TEXT        Pass --trusted-host VALUE to pip, helps in local
+                             indexes over HTTP. Pass the correct hostname.
+                             [default: ]
+  --skip-build-deps          While downloading the sources, skip downloading
+                             the build dependencies as source  [default: True]
   --help                     Show this message and exit.
 ```
 
-To build a reproducible wheel for a given source tar ball.
-
+To build a reproducible wheel for a given source tarball:
 ```
 asaman -s dist/yourpackage_4.2.0.tar.gz
 ```
 
-By default the freshly built wheel will be stored in the `./wheels/` directory, you can select any directory for the same using `-o` or `--output` option.
-
-To built reproducible wheels for all the sources from a directory.
-
+By default the freshly built wheel will be stored in the `./wheels/` directory. You can specify a different directory using `-o`/`--output`.
 
+To build reproducible wheels for all the sources from a directory:
 ```
 asaman -d path/to/sources/
 ```
 
-Or, you can point to a requirements file which contains all the dependencies along with hashes.
-
+Or, you can point to a requirements file which contains all the dependencies along with hashes:
 ```
 asaman -r requirements.txt
 ```
 
 
 ## How to generate a requirements file with hashes from the reproducible wheels?
 
 ```
 asaman-generate requirements.txt
 ```
 
-The `asaman-generate` command will help you to create a fresh `verified-requirements.txt`, which
-will contain the hashes from reproducible wheels. You can pass `-o/--output` option to pass your
-custom file name.
+The `asaman-generate` command will help you to create a fresh `verified-requirements.txt`, which will contain the hashes from reproducible wheels. You can pass the `-o`/`--output` option to pass your custom file name.
 
 ```
 asaman-generate --help
 Usage: asaman-generate [OPTIONS] REQUIREMENT
 
   Tool to build verified requirements file from reproducible wheels.
 
@@ -93,25 +85,27 @@
   -o, --output FILE       The output file. Default: verified-{requirement}.txt
   -w, --wheels DIRECTORY  The directory with reproducible wheels.
   -s, --skip TEXT         The packages we don't want in our final requirement
                           file.
   --help                  Show this message and exit.
 ```
 
-## How to create a requirement file with hashes from PyPI or your personal index?
+## How to create a requirements file with hashes from PyPI or your personal index?
 
-Use [pip-tools](https://github.com/jazzband/pip-tools/) project.
+Use the [pip-tools](https://github.com/jazzband/pip-tools/) project.
 
 ```
 pip-compile --generate-hashes --allow-unsafe --output-file=requirements.txt requirements.in
 ```
 
-Please make sure that you note down all the build dependencies  of any given `dependency`, otherwise during the build process, `pip` will download from PyPI and install them in the build environment. If you are building from a requirements file, during download and extracting each source tar ball, you can notice if the dependency has any build time dependency or not. Otherwise, you can manually look at the build time dependencies. 
+Please make sure that include all the build dependencies of any dependency. If you don't then `pip` will download the build dependencies from PyPI and install them in the build environment.
+
+To help identify build dependencies while you are building from a requirements file, during download and extracting each source tarball via `pip`, you can notice any dependency which has build time dependency or not. Otherwise, you can manually look at the build-time dependencies.
 
-For example in the following text you can find a few packages with build time dependencies.
+For example, in the following text you can find a few packages with build time dependencies.
 Look at the lines with **Getting requirements to build wheel**.
 
 ```
 Collecting build==0.7.0
   Using cached build-0.7.0.tar.gz (15 kB)
   Installing build dependencies ... done
   Getting requirements to build wheel ... done
@@ -129,47 +123,48 @@
   Getting requirements to build wheel ... done
     Preparing wheel metadata ... done
 ```
 
 
 ## Bootstrapping the build environment
 
-For any production use, you should also bootstrap the build environment, and create the initial virtual environment to build all dependencies in that environment only. You can store the wheels in any place you want (S3, or git-lfs), and start from there during creating the environment next time.
-
-In following commands, we will create a set of wheels for such bootstrap environment where the build requirements are mentioned in `bootstrap.in` 
+For any production use, you should also bootstrap the build environment and create the initial virtual environment to build all dependencies in that environment only. You can store the wheels in any place you want e.g. (S3, or git-lfs), and start from there when creating the environment next time.
 
+In the following commands, we will create a set of wheels for such a bootstrap environment. We will start with listing the build requirements in `bootstrap.in` with the following contents:
 ```
 amrasaman >=0.1.0
 ```
 
 ```
 python3 -m venv .venv
 source .venv/bin/activate
-python3 -m pip install pip-tools # This is coming directly from pypi
+python3 -m pip install pip-tools # This is being downloaded directly from PyPI.
 pip-compile --generate-hashes --allow-unsafe --output-file=bootstrap.txt bootstrap.in
 asaman -r bootstrap.txt
 ```
 
 This will create all the wheels in the `./wheels` directory.
-From next time, one can install them from the `./wheels` directory directory.
 
-But, first we will create a new requirements file with only the hashes from our reproducible wheels, the output file name will be `verified-bootstrap.txt`.
+
+Next time we can install the wheels from the `./wheels` directory. But first we will create a new requirements file with only the hashes from our reproducible wheels, the output file name will be `verified-bootstrap.txt`.
 
 ```
 asaman-generate bootstrap.txt
 ```
 
-Now we can use this file to create the environment.
+Now we can use this requirements file to create the environment.
 
 ```
 python3 -m venv .venv
 source .venv/bin/activate
 python3 -m pip install --no-index --find-links ./wheels --require-hashes --only-binary :all: -r verified-bootstrap.txt 
 ```
 
 
+## Meaning of the name
 
+In Bengali it means "we are same"
 
+## Developer documentation
 
-
-
+Read the [hacking guide](https://asaman.readthedocs.io/en/latest/hacking.html).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `asaman-0.1.6/README.md` & `asaman-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,40 @@
-## asaman: Amra Saman
+Metadata-Version: 2.1
+Name: asaman
+Version: 0.2.0
+Summary: A tool to create reproducible wheels
+Author-email: Kushal Das <mail@kushaldas.in>
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Classifier: License :: OSI Approved :: MIT License
+Requires-Dist: wheel
+Requires-Dist: build>=0.7.0
+Requires-Dist: click
+Requires-Dist: pep517
+Requires-Dist: setuptools
+Project-URL: Documentation, https://asaman.readthedocs.io/en/latest/
+Project-URL: Source, https://github.com/kushaldas/asaman
+
+# asaman: Amra Saman (আমরা সমান)
+
+This is a tool to build reproducible wheels for your Python project or for all of your dependencies. What this means is if you use the same Operating System version and similar system level dependencies, you will always get the same wheel generated. This enables us to have a bit more protection from side-channel attacks. Any user of the wheels can verify that they are using the correct build from the exact source via verifying the builds themselves.
 
-This is a tool to build reproducible wheels for you Python project or for all of your dependencies. Means, if you use the same Operating System version and similar system level dependencies, you will always get the same wheel generated. Thus enabling us to have a bit more protection from side-channel attacks. Any user of the wheels can verify that they are using the correct build from the exact source via verifying the builds themselves.
 
 ## Why do we need a reproducible wheel?
 
 A few different positive points:
 
-- If we build the wheels from a known source (via pinned hashes in requirements file), we can also verify if we are using the correct wheels build from them.
-- Any user/developer can rebuild the wheels from the pinned source, and should get the exact same wheel as output. Thus if anything gets into the build process (say in CI), or the wheel is actually built from a different source, automated tools can identify those.
+- If we build the wheels from a known source (e.g. via pinned hashes in requirements file), we can also verify if we are using the correct wheels built from them.
+- Any user/developer can rebuild the wheels from the pinned source and should get the exact same wheel as output. Thus if anything gets into the build process (say in CI), or the wheel is actually built from a different source, automated tools can identify that difference.
 
 
 ## How to install?
 
 ```bash
-python3 -m pip install amrasaman
+python3 -m pip install asaman
 ```
 
 ## How to build reproducible wheels?
 
 ```
 asaman --help
 Usage: asaman [OPTIONS]
@@ -29,48 +46,54 @@
   -d, --directory DIRECTORY  A directory containing all source tarballs and
                              zips.
   -o, --output DIRECTORY     The output directory to store all wheel files.
                              Default: ./wheels
   -r, --requirement FILE     Path to the requirement.txt file which contains
                              all packages to build along with hashes.
   --sde TEXT                 Custom SOURCE_DATE_EPOCH value.
+  --no-hash                  DO NOT USE UNLESS VERY SURE: In case we skip hash
+                             checking for download.  [default: False]
+  --keep-sources             Copy over the sources to output directory
+                             [default: False]
+  --with-index TEXT          In case you want to install build time
+                             dependencies from an index, pass the URL.
+                             [default: ]
+  --trusted-host TEXT        Pass --trusted-host VALUE to pip, helps in local
+                             indexes over HTTP. Pass the correct hostname.
+                             [default: ]
+  --skip-build-deps          While downloading the sources, skip downloading
+                             the build dependencies as source  [default: True]
   --help                     Show this message and exit.
 ```
 
-To build a reproducible wheel for a given source tar ball.
-
+To build a reproducible wheel for a given source tarball:
 ```
 asaman -s dist/yourpackage_4.2.0.tar.gz
 ```
 
-By default the freshly built wheel will be stored in the `./wheels/` directory, you can select any directory for the same using `-o` or `--output` option.
-
-To built reproducible wheels for all the sources from a directory.
-
+By default the freshly built wheel will be stored in the `./wheels/` directory. You can specify a different directory using `-o`/`--output`.
 
+To build reproducible wheels for all the sources from a directory:
 ```
 asaman -d path/to/sources/
 ```
 
-Or, you can point to a requirements file which contains all the dependencies along with hashes.
-
+Or, you can point to a requirements file which contains all the dependencies along with hashes:
 ```
 asaman -r requirements.txt
 ```
 
 
 ## How to generate a requirements file with hashes from the reproducible wheels?
 
 ```
 asaman-generate requirements.txt
 ```
 
-The `asaman-generate` command will help you to create a fresh `verified-requirements.txt`, which
-will contain the hashes from reproducible wheels. You can pass `-o/--output` option to pass your
-custom file name.
+The `asaman-generate` command will help you to create a fresh `verified-requirements.txt`, which will contain the hashes from reproducible wheels. You can pass the `-o`/`--output` option to pass your custom file name.
 
 ```
 asaman-generate --help
 Usage: asaman-generate [OPTIONS] REQUIREMENT
 
   Tool to build verified requirements file from reproducible wheels.
 
@@ -78,25 +101,27 @@
   -o, --output FILE       The output file. Default: verified-{requirement}.txt
   -w, --wheels DIRECTORY  The directory with reproducible wheels.
   -s, --skip TEXT         The packages we don't want in our final requirement
                           file.
   --help                  Show this message and exit.
 ```
 
-## How to create a requirement file with hashes from PyPI or your personal index?
+## How to create a requirements file with hashes from PyPI or your personal index?
 
-Use [pip-tools](https://github.com/jazzband/pip-tools/) project.
+Use the [pip-tools](https://github.com/jazzband/pip-tools/) project.
 
 ```
 pip-compile --generate-hashes --allow-unsafe --output-file=requirements.txt requirements.in
 ```
 
-Please make sure that you note down all the build dependencies  of any given `dependency`, otherwise during the build process, `pip` will download from PyPI and install them in the build environment. If you are building from a requirements file, during download and extracting each source tar ball, you can notice if the dependency has any build time dependency or not. Otherwise, you can manually look at the build time dependencies. 
+Please make sure that include all the build dependencies of any dependency. If you don't then `pip` will download the build dependencies from PyPI and install them in the build environment.
+
+To help identify build dependencies while you are building from a requirements file, during download and extracting each source tarball via `pip`, you can notice any dependency which has build time dependency or not. Otherwise, you can manually look at the build-time dependencies.
 
-For example in the following text you can find a few packages with build time dependencies.
+For example, in the following text you can find a few packages with build time dependencies.
 Look at the lines with **Getting requirements to build wheel**.
 
 ```
 Collecting build==0.7.0
   Using cached build-0.7.0.tar.gz (15 kB)
   Installing build dependencies ... done
   Getting requirements to build wheel ... done
@@ -114,45 +139,49 @@
   Getting requirements to build wheel ... done
     Preparing wheel metadata ... done
 ```
 
 
 ## Bootstrapping the build environment
 
-For any production use, you should also bootstrap the build environment, and create the initial virtual environment to build all dependencies in that environment only. You can store the wheels in any place you want (S3, or git-lfs), and start from there during creating the environment next time.
-
-In following commands, we will create a set of wheels for such bootstrap environment where the build requirements are mentioned in `bootstrap.in` 
+For any production use, you should also bootstrap the build environment and create the initial virtual environment to build all dependencies in that environment only. You can store the wheels in any place you want e.g. (S3, or git-lfs), and start from there when creating the environment next time.
 
+In the following commands, we will create a set of wheels for such a bootstrap environment. We will start with listing the build requirements in `bootstrap.in` with the following contents:
 ```
 amrasaman >=0.1.0
 ```
 
 ```
 python3 -m venv .venv
 source .venv/bin/activate
-python3 -m pip install pip-tools # This is coming directly from pypi
+python3 -m pip install pip-tools # This is being downloaded directly from PyPI.
 pip-compile --generate-hashes --allow-unsafe --output-file=bootstrap.txt bootstrap.in
 asaman -r bootstrap.txt
 ```
 
 This will create all the wheels in the `./wheels` directory.
-From next time, one can install them from the `./wheels` directory directory.
 
-But, first we will create a new requirements file with only the hashes from our reproducible wheels, the output file name will be `verified-bootstrap.txt`.
+
+Next time we can install the wheels from the `./wheels` directory. But first we will create a new requirements file with only the hashes from our reproducible wheels, the output file name will be `verified-bootstrap.txt`.
 
 ```
 asaman-generate bootstrap.txt
 ```
 
-Now we can use this file to create the environment.
+Now we can use this requirements file to create the environment.
 
 ```
 python3 -m venv .venv
 source .venv/bin/activate
 python3 -m pip install --no-index --find-links ./wheels --require-hashes --only-binary :all: -r verified-bootstrap.txt 
 ```
 
 
+## Meaning of the name
+
+In Bengali it means "we are same"
 
+## Developer documentation
 
+Read the [hacking guide](https://asaman.readthedocs.io/en/latest/hacking.html).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `asaman-0.1.6/asaman/__init__.py` & `asaman-0.2.0/asaman/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,18 @@
+"A tool to create reproducible wheels"
+
+__version__ = "0.2.0"
+
 import glob
 import os
 import shutil
 import subprocess
 import sys
 import tempfile
+from pip_requirements_parser import RequirementsFile
 
 import click
 
 # Variables for various operations
 
 # To remember the time Aaron Swartz made the first commit
 # to SecureDrop project.
@@ -43,75 +48,109 @@
         subprocess.check_call(cmd)
 
     for source in zipsources:
         cmd = ["unzip", source, "-d", WHEEL_BUILD_DIR]
         subprocess.check_call(cmd)
 
 
-def build_sources(tmpdir: str):
+def build_sources(tmpdir: str, with_index: str = "", trusted_host: str = ""):
     "Builds reproducible wheels from temporary extract source files"
     project_names = os.listdir(WHEEL_BUILD_DIR)
+    if with_index:
+        # Set the index value for PIP
+        os.environ["PIP_INDEX_URL"] = with_index
+        print(f"Seting PIP_INDEX_URL={with_index}")
     for project in project_names:
         click.echo(f"{project}")
         source_path = os.path.join(WHEEL_BUILD_DIR, project)
         cmd = [
             "python3",
             "-m",
             "build",
             "--wheel",
             source_path,
-            "--no-isolation",
             "-o",
             tmpdir,
         ]
+        # Normally we build without isolation
+        # This means we have to handle all build dependencies,
+        # unless we pass an index.
+        if not with_index:
+            cmd.append("--no-isolation")
+
+        # We want to trust the PIP_INDEX_URL (in case of without HTTPS)
+        if trusted_host:
+            cmd.append(f"--config-setting=--trusted-host={trusted_host}")
+            os.environ["PIP_TRUSTED_HOST"] = trusted_host
+            print(f"Setting PIP_TRUSTED_HOST={trusted_host}")
+        # Execute the build command
         subprocess.check_call(cmd)
         click.echo(f"build command used: {' '.join(cmd)}")
+    # All done, unset the URL
+    os.environ["PIP_INDEX_URL"] = ""
 
 
-def copy_wheels(tmpdir: str, output: str):
-    "Copies the freshly built wheels to a dirctory"
+def copy_files(tmpdir: str, output: str, keep_sources: bool):
+    "Copies the freshly built wheels or sources to a dirctory"
 
     # If the output directory does not exists then create
     if not os.path.exists(output):
         os.mkdir(output)
 
     # First find all the wheels
     names = os.listdir(tmpdir)
     for name in names:
-        if not name.endswith(".whl"):
-            # we want only wheel files
-            continue
+        if not keep_sources:
+            if not name.endswith(".whl"):
+                # we want only wheel files
+                continue
         filepath = os.path.join(tmpdir, name)
         shutil.copy(filepath, output, follow_symlinks=True)
 
 
 def find_and_extract_sources(directory: str):
     "Finds all the source files from a given directory and extracts them."
 
     tarsources = glob.glob(f"{directory}/*.tar.gz")
     zipsources = glob.glob(f"{directory}/*.zip")
     extract_sources(tarsources=tarsources, zipsources=zipsources)
 
 
-def download_sources(requirements: str, output: str):
+def download_sources(requirements: str, output: str, no_hash=False, skip_build_deps=True):
     "Downloads all sources from a given requirements file."
     click.echo("Downloading sources using the requirements file.")
     cmd = [
         "python3",
         "-m",
         "pip",
         "download",
-        "--no-binary",
-        ":all:",
-        "--require-hashes",
-        "--dest",
-        output,
-        "--requirement",
-        requirements,
     ]
+    if not skip_build_deps:
+        cmd.append("--no-binary")
+        cmd.append(":all:")
+    else:
+        # Here we find all the actual package names and add them to no binary list
+        rf = RequirementsFile.from_file(requirements)
+        data = rf.to_dict()
+        for req in data["requirements"]:
+            cmd.append("--no-binary")
+            cmd.append(f"{req['name']}")
+
+    if not no_hash:
+        cmd.append("--require-hashes")
+    cmd.append("--no-deps")
+    cmd.extend(
+        [
+            "--dest",
+            output,
+            "--requirement",
+            requirements,
+        ]
+    )
+    print(cmd)
     subprocess.check_call(cmd)
 
 
 @click.command(name="asaman", help="Tool to build reproducible wheels.")
 @click.option(
     "-s",
     "--source",
@@ -140,15 +179,59 @@
     "--requirement",
     type=click.Path(
         exists=True, file_okay=True, dir_okay=False, readable=True, resolve_path=True
     ),
     help="Path to the requirement.txt file which contains all packages to build along with hashes.",
 )
 @click.option("--sde", type=click.STRING, help="Custom SOURCE_DATE_EPOCH value.")
-def cli(source: str, directory: str, output: str, requirement: str, sde: str):
+@click.option(
+    "--no-hash",
+    is_flag=True,
+    show_default=True,
+    default=False,
+    help="DO NOT USE UNLESS VERY SURE: In case we skip hash checking for download.",
+)
+@click.option(
+    "--keep-sources",
+    is_flag=True,
+    show_default=True,
+    default=False,
+    help="Copy over the sources to output directory",
+)
+@click.option(
+    "--with-index",
+    show_default=True,
+    default="",
+    help="In case you want to install build time dependencies from an index, pass the URL.",
+)
+@click.option(
+    "--trusted-host",
+    show_default=True,
+    default="",
+    help="Pass --trusted-host VALUE to pip, helps in local indexes over HTTP. Pass the correct hostname.",
+)
+@click.option(
+    "--skip-build-deps",
+    is_flag=True,
+    show_default=True,
+    default=True,
+    help="While downloading the sources, skip downloading the build dependencies as source",
+)
+def cli(
+    source: str,
+    directory: str,
+    output: str,
+    requirement: str,
+    sde: str,
+    no_hash: bool,
+    keep_sources: bool,
+    with_index: str,
+    trusted_host: str,
+    skip_build_deps: bool,
+):
     if not any([source, directory, requirement]):
         show_help(cli)
         sys.exit(1)
 
     if sde:
         os.environ["SOURCE_DATE_EPOCH"] = sde
     # First let us create the temporary directories
@@ -171,19 +254,19 @@
             sys.exit(1)
     if directory:
         find_and_extract_sources(directory)
 
     with tempfile.TemporaryDirectory() as tmpdir:
         # Check if we have a requirements file, then download the sources first
         if requirement:
-            download_sources(requirement, tmpdir)
+            download_sources(requirement, tmpdir, no_hash, skip_build_deps)
             find_and_extract_sources(tmpdir)
         # Time to build the wheels.
-        build_sources(tmpdir)
-        copy_wheels(tmpdir, output)
+        build_sources(tmpdir, with_index=with_index, trusted_host=trusted_host)
+        copy_files(tmpdir, output, keep_sources)
         # All done for now
         click.echo(f"All wheels can be found at {output}")
 
 
 @click.command(
     name="asaman-generate",
     help="Tool to build verified requirements file from reproducible wheels.",
```

### Comparing `asaman-0.1.6/dev-requirements.txt` & `asaman-0.2.0/requirements.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 #
-# This file is autogenerated by pip-compile with python 3.9
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.11
+# by the following command:
 #
-#    pip-compile --allow-unsafe --generate-hashes --output-file=dev-requirements.txt dev-requirements.in
+#    pip-compile --allow-unsafe --generate-hashes --output-file=requirements.txt requirements.in
 #
+build==0.10.0 \
+    --hash=sha256:af266720050a66c893a6096a2f410989eeac74ff9a68ba194b3f6473e8e26171 \
+    --hash=sha256:d5b71264afdb5951d6704482aac78de887c80691c52b88a9ad195983ca2c9269
+    # via -r requirements.in
 click==8.0.1 \
     --hash=sha256:8c04c11192119b1ef78ea049e0a6f0463e4c48ef00a30160c704337586f3ad7a \
     --hash=sha256:fba402a4a47334742d782209a7c79bc448911afe1149d07bdabdf480b3e2f4b6
-    # via pip-tools
+    # via -r requirements.in
+flit-core==3.3.0 \
+    --hash=sha256:9b247b3095cb3c43933a59a7433f92ddfdd7fc843e08ef0f4550d53a9cfbbef6 \
+    --hash=sha256:b1404accffd6504b5f24eeca9ec5d3c877f828d16825348ba81515fa084bd5f0
+    # via -r requirements.in
 packaging==21.0 \
     --hash=sha256:7dc96269f53a4ccec5c0670940a4281106dd0bb343f47b7471f779df49c2fbe7 \
     --hash=sha256:c86254f9220d55e31cc94d69bade760f0847da8000def4dfe1c6b872fd14ff14
-    # via setuptools-scm
-pep517==0.11.0 \
-    --hash=sha256:3fa6b85b9def7ba4de99fb7f96fe3f02e2d630df8aa2720a5cf3b183f087a738 \
-    --hash=sha256:e1ba5dffa3a131387979a68ff3e391ac7d645be409216b961bc2efe6468ab0b2
-    # via pip-tools
-pip-tools==6.3.0 \
-    --hash=sha256:1835a1848bdfb22b2b6e5d10d630844ff5ee15e24b6c3bf92319c76f205d347f \
-    --hash=sha256:f5119d08558d4b44f5d3be6c433a5710050282d5aeecb1bfa392e86963827548
-    # via -r dev-requirements.in
+    # via
+    #   build
+    #   pip-requirements-parser
+pip-requirements-parser==32.0.1 \
+    --hash=sha256:4659bc2a667783e7a15d190f6fccf8b2486685b6dba4c19c3876314769c57526 \
+    --hash=sha256:b4fa3a7a0be38243123cf9d1f3518da10c51bdb165a2b2985566247f9155a7d3
+    # via -r requirements.in
 pyparsing==2.4.7 \
     --hash=sha256:c203ec8783bf771a155b207279b9bccb8dea02d8f0c9e5f8ead507bc3246ecc1 \
     --hash=sha256:ef9d7589ef3c200abe66653d3f1ab1033c3c419ae9b9bdb1240a85b024efc88b
-    # via packaging
-setuptools-scm==6.3.2 \
-    --hash=sha256:4c64444b1d49c4063ae60bfe1680f611c8b13833d556fd1d6050c0023162a119 \
-    --hash=sha256:a49aa8081eeb3514eb9728fa5040f2eaa962d6c6f4ec9c32f6c1fba88f88a0f2
-    # via -r dev-requirements.in
-tomli==1.2.1 \
-    --hash=sha256:8dd0e9524d6f386271a36b41dbf6c57d8e32fd96fd22b6584679dc569d20899f \
-    --hash=sha256:a5b75cb6f3968abb47af1b40c1819dc519ea82bcc065776a866e8d74c5ca9442
     # via
-    #   pep517
-    #   setuptools-scm
+    #   packaging
+    #   pip-requirements-parser
+pyproject-hooks==1.0.0 \
+    --hash=sha256:283c11acd6b928d2f6a7c73fa0d01cb2bdc5f07c57a2eeb6e83d5e56b97976f8 \
+    --hash=sha256:f271b298b97f5955d53fb12b72c1fb1948c22c1a6b70b315c54cedaca0264ef5
+    # via build
+toml==0.10.2 \
+    --hash=sha256:806143ae5bfb6a3c6e736a764057db0e6a0e05e338b5630894a5f779cabb4f9b \
+    --hash=sha256:b3bda1d108d5dd99f4a20d24d9c348e91c4db7ab1b749200bded2f839ccbe68f
+    # via flit-core
 wheel==0.37.0 \
     --hash=sha256:21014b2bd93c6d0034b6ba5d35e4eb284340e09d63c59aef6fc14b0f346146fd \
     --hash=sha256:e2ef7239991699e3355d54f8e968a21bb940a1dbf34a4d226741e64462516fad
-    # via pip-tools
+    # via -r requirements.in
 
 # The following packages are considered to be unsafe in a requirements file:
 pip==21.2.4 \
     --hash=sha256:0eb8a1516c3d138ae8689c0c1a60fde7143310832f9dc77e11d8a4bc62de193b \
     --hash=sha256:fa9ebb85d3fd607617c0c44aca302b1b45d87f9c2a1649b46c26167ca4296323
-    # via pip-tools
-setuptools==58.2.0 \
-    --hash=sha256:2551203ae6955b9876741a26ab3e767bb3242dafe86a32a749ea0d78b6792f11 \
-    --hash=sha256:2c55bdb85d5bb460bd2e3b12052b677879cffcf46c0c688f2e5bf51d36001145
-    # via
-    #   pip-tools
-    #   setuptools-scm
+    # via -r requirements.in
```

