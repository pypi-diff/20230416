# Comparing `tmp/talqual-0.0.2.tar.gz` & `tmp/talqual-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/talqual-0.0.2.tar", last modified: Tue Apr  7 11:43:04 2020, max compression
+gzip compressed data, was "talqual-0.0.3.tar", last modified: Sat Apr 15 22:09:43 2023, max compression
```

## Comparing `talqual-0.0.2.tar` & `talqual-0.0.3.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-07 11:43:04.000000 talqual-0.0.2/
--rw-rw-rw-   0 root         (0) root         (0)      233 2020-04-07 11:42:24.000000 talqual-0.0.2/CHANGES.txt
--rw-rw-rw-   0 root         (0) root         (0)    35146 2020-04-07 11:42:24.000000 talqual-0.0.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       80 2020-04-07 11:42:24.000000 talqual-0.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5653 2020-04-07 11:43:04.000000 talqual-0.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3734 2020-04-07 11:42:24.000000 talqual-0.0.2/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      183 2020-04-07 11:43:04.000000 talqual-0.0.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1480 2020-04-07 11:42:24.000000 talqual-0.0.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-07 11:43:04.000000 talqual-0.0.2/talqual/
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-04-07 11:42:24.000000 talqual-0.0.2/talqual/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       60 2020-04-07 11:42:24.000000 talqual-0.0.2/talqual/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     1627 2020-04-07 11:42:24.000000 talqual-0.0.2/talqual/batch.py
--rw-rw-rw-   0 root         (0) root         (0)     1177 2020-04-07 11:42:24.000000 talqual-0.0.2/talqual/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      626 2020-04-07 11:42:24.000000 talqual-0.0.2/talqual/importer.py
--rw-rw-rw-   0 root         (0) root         (0)      882 2020-04-07 11:42:24.000000 talqual-0.0.2/talqual/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-07 11:43:04.000000 talqual-0.0.2/talqual/static/
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-04-07 11:37:07.000000 talqual-0.0.2/talqual/static/__init__.py
--rw-r--r--   0 root         (0) root         (0)    43064 2020-04-07 11:38:27.000000 talqual-0.0.2/talqual/static/org.transcrypt.__runtime__.js
--rw-r--r--   0 root         (0) root         (0)     7526 2020-04-07 11:38:27.000000 talqual-0.0.2/talqual/static/scripts.js
--rw-rw-rw-   0 root         (0) root         (0)     5488 2020-04-07 11:42:24.000000 talqual-0.0.2/talqual/templates.py
--rw-rw-rw-   0 root         (0) root         (0)     1352 2020-04-07 11:42:24.000000 talqual-0.0.2/talqual/views.py
--rw-rw-rw-   0 root         (0) root         (0)      475 2020-04-07 11:42:24.000000 talqual-0.0.2/talqual/zpt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-07 11:43:04.000000 talqual-0.0.2/talqual.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5653 2020-04-07 11:43:04.000000 talqual-0.0.2/talqual.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      508 2020-04-07 11:43:04.000000 talqual-0.0.2/talqual.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-04-07 11:43:04.000000 talqual-0.0.2/talqual.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       69 2020-04-07 11:43:04.000000 talqual-0.0.2/talqual.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      148 2020-04-07 11:43:04.000000 talqual-0.0.2/talqual.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2020-04-07 11:43:04.000000 talqual-0.0.2/talqual.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 22:09:43.114677 talqual-0.0.3/
+-rw-rw-rw-   0 root         (0) root         (0)      518 2023-04-15 22:09:09.000000 talqual-0.0.3/CHANGES.txt
+-rw-rw-rw-   0 root         (0) root         (0)    35146 2023-04-15 22:09:09.000000 talqual-0.0.3/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-04-15 22:09:09.000000 talqual-0.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8078 2023-04-15 22:09:43.114677 talqual-0.0.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6739 2023-04-15 22:09:09.000000 talqual-0.0.3/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      500 2023-04-15 22:09:43.114677 talqual-0.0.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1990 2023-04-15 22:09:09.000000 talqual-0.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 22:09:43.113677 talqual-0.0.3/talqual/
+-rw-rw-rw-   0 root         (0) root         (0)      250 2023-04-15 22:09:09.000000 talqual-0.0.3/talqual/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-04-15 22:09:09.000000 talqual-0.0.3/talqual/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1627 2023-04-15 22:09:09.000000 talqual-0.0.3/talqual/batch.py
+-rw-rw-rw-   0 root         (0) root         (0)     1679 2023-04-15 22:09:09.000000 talqual-0.0.3/talqual/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2739 2023-04-15 22:09:09.000000 talqual-0.0.3/talqual/data.py
+-rw-rw-rw-   0 root         (0) root         (0)      921 2023-04-15 22:09:09.000000 talqual-0.0.3/talqual/importer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1532 2023-04-15 22:09:09.000000 talqual-0.0.3/talqual/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 22:09:43.114677 talqual-0.0.3/talqual/static/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 22:04:22.000000 talqual-0.0.3/talqual/static/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    43192 2023-04-15 22:05:25.000000 talqual-0.0.3/talqual/static/org.transcrypt.__runtime__.js
+-rw-r--r--   0 root         (0) root         (0)     8178 2023-04-15 22:05:25.000000 talqual-0.0.3/talqual/static/scripts.js
+-rw-rw-rw-   0 root         (0) root         (0)    10153 2023-04-15 22:09:09.000000 talqual-0.0.3/talqual/templates.py
+-rw-rw-rw-   0 root         (0) root         (0)     2016 2023-04-15 22:09:09.000000 talqual-0.0.3/talqual/translation.py
+-rw-rw-rw-   0 root         (0) root         (0)     5279 2023-04-15 22:09:09.000000 talqual-0.0.3/talqual/views.py
+-rw-rw-rw-   0 root         (0) root         (0)     1197 2023-04-15 22:09:09.000000 talqual-0.0.3/talqual/zpt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 22:09:43.113677 talqual-0.0.3/talqual.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8078 2023-04-15 22:09:43.000000 talqual-0.0.3/talqual.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      547 2023-04-15 22:09:43.000000 talqual-0.0.3/talqual.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-15 22:09:43.000000 talqual-0.0.3/talqual.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-04-15 22:09:43.000000 talqual-0.0.3/talqual.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      284 2023-04-15 22:09:43.000000 talqual-0.0.3/talqual.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-15 22:09:43.000000 talqual-0.0.3/talqual.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `talqual-0.0.2/LICENSE` & `talqual-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `talqual-0.0.2/PKG-INFO` & `talqual-0.0.3/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,152 +1,201 @@
-Metadata-Version: 2.1
-Name: talqual
-Version: 0.0.2
-Summary: TAL Chameleon (static site generator)
-Home-page: https://gitlab.com/timbaler/talqual/
-Author: Aleix Llusà Serra
-Author-email: timbaler@timbaler.cat
-License: GPLv3+
-Description: talqual
-        =======
-        
-        |Test| |Coverage| |Pypi|
-        
-        .. |Test| image:: https://gitlab.com/timbaler/talqual/badges/master/pipeline.svg
-                :target: https://gitlab.com/timbaler/talqual/commits/master
-        .. |Coverage| image:: https://gitlab.com/timbaler/talqual/badges/master/coverage.svg
-                :target: https://gitlab.com/timbaler/talqual/commits/master
-        ..  |Pypi| image:: https://img.shields.io/pypi/v/talqual.svg
-            :target: https://pypi.python.org/pypi/talqual
-        
-        
-        TAL_ Chameleon_ static site generator.
-        
-        Simple structure: templates + data -> output html
-        
-        
-        .. _TAL: https://chameleon.readthedocs.io/en/latest/reference.html
-        .. _Chameleon: https://chameleon.readthedocs.io
-        
-        
-        
-        Installation
-        ------------
-        Install from PyPI::
-        
-            pip install talqual
-        
-        
-        Developing
-        ----------
-        
-        Install requirement and launch tests::
-        
-            pip install -r requirements-dev.txt
-            pytest tests
-        
-        
-        Selenium
-        --------
-        
-        Launch tests with driver option::
-        
-          pytest tests --driver firefox
-        
-        
-        Maybe you get the error::
-        
-         selenium.common.exceptions.WebDriverException: Message: 'geckodriver' executable needs to be in PATH.
-        
-        Then you need to download the latest `geckodriver` release from https://github.com/mozilla/geckodriver/releases (such as `geckodriver-v0.26.0-linux64.tar.gz`) and extract it to the correspongind directory (such as `/usr/local/bin/`).
-        
-        
-        
-        Usage
-        -----
-        
-        * talqual `templates_dir`
-        * talqual `templates_dir` `output_html` --data `data.yaml`
-        * python -m talqual `templates_dir` `output_html` --data `data.yaml`
-        
-        or from code::
-        
-         from talqual.main import run
-         run(templates_dir, html_dir, data_yaml_file)
-        
-        
-        Features
-        --------
-        
-        Template elements: Folder, File, TalTemplate/Html, NoView, TalCommand
-        Data elements: Python objects, yaml files
-        
-        
-        * Define a `data`.yaml file
-        * Define a `templates` directory
-        * A folder in the `templates` is created to the `html` directory
-        * A file (pdf, image, css, js, etc.) in the `templates` is copied to the `html` directory
-        * A no view element (file or directory starting by `_`) in the `templates` is not created to the `html` directory
-        * A TAL template in the `templates` gets rendered to the `html` directory
-        
-          - It can reference data from the `data` directory or from python objects
-          - It can be:
-        
-            - a static .html or .htm (with no templating)
-            - a simple template .html .htm or .pt (with TAL templating)
-            - a template with macros .html .htm or .pt (with TAL and METAL templating)
-        
-        * A TAL Command gets executed and rendered  to the `html` directory
-        
-          - a template with NAME.tal_repeat_VARIABLE.pt gets repeated by `data[VARIABLE]` (it must be an iterable). Results in `NAME.0.html`, `NAME.1.html`, `NAME.2.html`, etc.
-        
-          - a template with NAME.tal_batch_VARIABLE_PAGESIZE.pt gets rendered by a Batch of PAGESIZE for `data[VARIABLE]` (it must be an iterable). Results in `NAME.html`, `NAME.2.html`, `NAME.3.html`, etc.
-        
-          - a template with NAME.tal_replace_talqual_scripts.js gets rendered to a javascript file NAME.js with the faceted module.
-        
-        
-        * A template can include the faceted javascript module. See the `portfolio` example.
-        
-        
-        License
-        -------
-        
-        ``talqual`` is offered under the GPLv3 license.
-        
-        This program is free software: you can redistribute it and/or modify
-        it under the terms of the GNU General Public License as published by
-        the Free Software Foundation, either version 3 of the License, or
-        (at your option) any later version.
-        
-        This program is distributed in the hope that it will be useful,
-        but WITHOUT ANY WARRANTY; without even the implied warranty of
-        MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-        GNU General Public License for more details.
-        
-        You should have received a copy of the GNU General Public License
-        along with this program.  If not, see <http://www.gnu.org/licenses/>.
-        
-        CHANGES
-        =======
-        
-        0.0.2 (2020-4-7)
-        ----------------
-        
-        - Add faceted select features
-        - Add faceted+batch combination
-        
-        
-        0.0.1 (2020-2-2)
-        ----------------
-        
-        - Initial release.
-        
-        - Template structure + yaml data file = output html structure
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 1 - Planning
-Classifier: Topic :: Internet :: WWW/HTTP
-Requires-Python: >=3.5.3
-Provides-Extra: test
+talqual
+=======
+
+|Test| |Coverage| |Pypi| |Python| |Gpl|
+
+.. |Test| image:: https://gitlab.com/timbaler/talqual/badges/master/pipeline.svg
+        :target: https://gitlab.com/timbaler/talqual/commits/master
+.. |Coverage| image:: https://gitlab.com/timbaler/talqual/badges/master/coverage.svg
+        :target: https://gitlab.com/timbaler/talqual/commits/master
+.. |Pypi| image:: https://img.shields.io/pypi/v/talqual.svg
+    :target: https://pypi.python.org/pypi/talqual
+.. |Python| image:: https://img.shields.io/pypi/pyversions/talqual.svg
+            :alt: Python version
+.. |Gpl| image:: https://img.shields.io/pypi/l/talqual.svg
+         :target: https://www.gnu.org/licenses/gpl-3.0.html
+         :alt: Gplv3-License
+
+
+TAL_ Chameleon_ static site generator.
+
+Simple structure: templates + data -> output html
+
+
+.. _TAL: https://chameleon.readthedocs.io/en/latest/reference.html
+.. _Chameleon: https://chameleon.readthedocs.io
+.. _TALsyntax: https://chameleon.readthedocs.io/en/latest/reference.html
+.. _METALsyntax: https://chameleon.readthedocs.io/en/latest/reference.html#macros-metal
+.. _TALi18nsyntax: https://chameleon.readthedocs.io/en/latest/reference.html#id49
+
+
+Installation
+------------
+
+Install from PyPI::
+
+    pip install talqual
+
+
+Developing
+----------
+
+Install requirement and launch tests::
+
+    pip install -r requirements-dev.txt
+    pytest tests
+
+
+Selenium
+--------
+
+Launch tests with driver option::
+
+  pytest tests --driver firefox
+
+
+Maybe you get the error::
+
+ selenium.common.exceptions.WebDriverException: Message: 'geckodriver' executable needs to be in PATH.
+
+Then you need to download the latest `geckodriver` release from https://github.com/mozilla/geckodriver/releases (such as `geckodriver-v0.28.0-linux64.tar.gz`) and extract it to the correspongind directory (such as `/usr/local/bin/`).
+
+
+
+Usage
+-----
+
+* talqual `templates_dir`
+* talqual `templates_dir` `output_html` --data `data_dir`
+* python -m talqual `templates_dir` `output_html` --data `data_dir`
+
+or from code::
+
+ from talqual.main import build
+ build(templates_dir, html_dir, data_dir)
+
+
+Features
+--------
+
+Template elements: Folder, File, TalTemplate/Html, NoView, TalCommand
+Data elements: Python objects, Folder, yaml, json, rst
+
+
+* Define a `data` directory. Will be converted to dictionary structure:
+
+  * Subfolders
+  * Yaml files
+  * Json files
+  * ReestructuredText files (only variables)
+
+* Define a `templates` directory
+* A folder in the `templates` is created to the `html` directory
+* A file (pdf, image, css, js, etc.) in the `templates` is copied to the `html` directory
+* A no view element (file or directory starting by `_`) in the `templates` is not created to the `html` directory
+* A TAL template in the `templates` gets rendered to the `html` directory
+
+  - It can reference data from the `data` directory or from python objects
+  - It can be:
+
+    - a static .html or .htm (with no templating)
+    - a simple template .html .htm or .pt (with TAL templating, see TALsyntax_)
+    - a template with macros .html .htm or .pt (with TAL and METAL templating, see METALsyntax_)
+
+* A TAL Command gets executed and rendered  to the `html` directory
+
+  - a template with NAME.tal_repeat_VARIABLE.pt gets repeated by `data[VARIABLE]` (it must be an iterable such as `[ITEM0, ITEM1, ITEM2, ...]` ). Results in `NAME.0.html`, `NAME.1.html`, `NAME.2.html`, etc.
+
+    - a template with tal_.tal_repeat_VARIABLE.pt results in `ITEM0.html`, `ITEM1.html`, `ITEM2.html`, etc.
+    - inside each TAL template the expression `${tal_repeat_VARIABLE}` can be used. Contains the current index `${tal_repeat_VARIABLE.num}` and `ITEM` `${tal_repeat_VARIABLE.item}`.
+
+  - a template with NAME.tal_batch_VARIABLE_PAGESIZE.pt gets rendered by a Batch of PAGESIZE for `data[VARIABLE]` (it must be an iterable). Results in `NAME.html`, `NAME.2.html`, `NAME.3.html`, etc.
+
+  - a template with NAME.tal_replace_talqual_scripts.js gets rendered to a javascript file NAME.js with the faceted module.
+
+  - a template with NAME.tal_replace_DATA:VARIABLE.js gets rendered to the contents of file in `data[DATA][VARIABLE]`.
+
+  - VARIABLE can be generally expressed as `VAR1:VAR2:VAR3` meaning `data[VAR1][VAR2][VAR3]`
+
+* Inside TAL templates, there is the expression `url:` for computing links relatively to the root. For example: `href="${url: static/a.png}"`
+
+* HTML internal links integrity is checked. In case of broken links, a warning is shown when building.
+
+
+Extra
+=====
+
+* A template can include the faceted javascript module. See the `portfolio` example.
+
+* A template can include the calendar javascript module. See the `portfolio` example.
+
+
+Translation (i18n)
+==================
+
+See the `i18n` example.
+
+
+Install:
+
+* You need to `pip install babel-lingua-chameleon` or `pip install talqual[multilingual]`
+
+
+Usage:
+
+* talqual `templates_dir` (by default locales at `templates_dir/_locales`)
+* talqual `templates_dir` `output_html` --data `data_dir` --locales `locales_dir`
+
+
+Features:
+
+* Define a folder in the `templates` named `tal_.tal_repeat_LOCALES`
+* Define templates .html .htm or .pt with TAL templating that includes i18n, see TALi18nsyntax_.
+* Define inside `data` a `LOCALES` variable listing the enabled localizations (l10n). For exemple, a `data.yaml`::
+
+   LOCALES:
+   - ca
+   - en
+   - oc
+
+* Define the `locales_dir`. Recommended with `Babel command-line interface <https://babel.pocoo.org/en/latest/cmdline.html>`_
+
+  * First time:
+
+    * Define the `babel.cfg` to extract from TAL templates::
+
+       [python: **.py]
+       [lingua-chameleon: **.html]
+       [lingua-chameleon: **.htm]
+       [lingua-chameleon: **.pt]
+
+    * `mkdir locales`
+    * `pybabel extract -F babel.cfg -o locales/mydomain.pot .`
+    * `pybabel init -D mydomain -i locales/mydomain.pot -d locales -l ca`
+    * (init all languages)
+    * `pybabel compile -D mydomain -d locales`
+
+  * Updates:
+
+    * `pybabel extract -F babel.cfg -o locales/mydomain.pot .`
+    * `pybabel update -D mydomain -i locales/mydomain.pot -d locales`
+    * `pybabel compile -D mydomain -d locales`
+
+
+
+License
+-------
+
+``talqual`` is offered under the GPLv3 license.
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `talqual-0.0.2/talqual/batch.py` & `talqual-0.0.3/talqual/batch.py`

 * *Files identical despite different names*

### Comparing `talqual-0.0.2/talqual/cli.py` & `talqual-0.0.3/talqual/cli.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,46 +1,60 @@
 import logging
 from pathlib import Path
 
 import click
 
-from . import main
+from . import __version__, main
 
 
-VERSION = '0.0.1'
 _dir_existing = click.Path(exists=True, dir_okay=True, file_okay=False)
 _dir_optional = click.Path(exists=False)
-_file_existing = click.Path(exists=True, dir_okay=False, file_okay=True)
+_fileordir_existing = click.Path(exists=True, dir_okay=True, file_okay=True)
 verbose_help = 'Enable verbose output.'
 
 
 @click.group()
-@click.version_option(VERSION, '-V', '--version', prog_name='talqual')
+@click.version_option(__version__, '-V', '--version', prog_name='talqual')
 @click.option('-v', '--verbose', is_flag=True, help=verbose_help)
 def cli(verbose):
     if verbose:
         logging.basicConfig(level=logging.DEBUG)
+    else:
+        logging.basicConfig(level=logging.INFO)
 
 
 @cli.command()
 @click.argument('src', type=_dir_existing, required=True)
 @click.argument('dst', type=_dir_optional, required=False)
-@click.option('--data', type=_file_existing, required=False,
-              help='defaults to src/_data.yaml', metavar='data.yaml')
-def build(src, dst, data):
+@click.option('--data', type=_fileordir_existing, required=False,
+              help='defaults to src/_data or src/_data.yaml',
+              metavar='data_src')
+@click.option('--locales', type=_dir_existing, required=False,
+              help='defaults to src/_locales',
+              metavar='locales_src')
+def build(src, dst, data, locales):
     """Builds SRC to DST
 
     SRC is a directory of templates
 
     DST defaults to SRC/_build
     """
     src = Path(src)
     if dst is None:
         dst = src / '_build'
     else:
         dst = Path(dst)
     if data is None:
-        data = src / '_data.yaml'
+        data = src / '_data'
+        if not data.exists():
+            data = src / '_data.yaml'
+            if not data.exists():
+                data = None
     else:
         data = Path(data)
 
-    main.build(src, dst, data)
+    if locales is None:
+        locales = src / '_locales'
+        if not locales.exists():
+            locales = None
+
+    main.build(src, dst, data, locales)
```

### Comparing `talqual-0.0.2/talqual/static/org.transcrypt.__runtime__.js` & `talqual-0.0.3/talqual/static/org.transcrypt.__runtime__.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 'use strict';
 var __name__ = "org.transcrypt.__runtime__";
 export var __envir__ = {};
 __envir__.interpreter_name = "python";
 __envir__.transpiler_name = "transcrypt";
 __envir__.executor_name = __envir__.transpiler_name;
-__envir__.transpiler_version = "3.7.16";
+__envir__.transpiler_version = "3.9.0";
 export function __nest__(headObject, tailNames, value) {
     var current = headObject;
     if (tailNames != "") {
         var tailChain = tailNames.split(".");
         var firstNewIndex = tailChain.length;
         for (var index = 0; index < tailChain.length; index++) {
             if (!current.hasOwnProperty(tailChain[index])) {
@@ -34,46 +34,45 @@
 export function __init__(module) {
     if (!module.__inited__) {
         module.__all__.__init__(module.__all__);
         module.__inited__ = true
     }
     return module.__all__
 }
-export var __proxy__ = false;
-export function __get__(self,
-    func, quotedFuncName) {
-    if (self)
-        if (self.hasOwnProperty("__class__") || typeof self == "string" || self instanceof String) {
-            if (quotedFuncName) Object.defineProperty(self, quotedFuncName, {
+export function __get__(aThis, func, quotedFuncName) {
+    if (aThis)
+        if (aThis.hasOwnProperty("__class__") ||
+            typeof aThis == "string" || aThis instanceof String) {
+            if (quotedFuncName) Object.defineProperty(aThis, quotedFuncName, {
                 value: function() {
                     var args = [].slice.apply(arguments);
-                    return func.apply(null, [self].concat(args))
+                    return func.apply(null, [aThis].concat(args))
                 },
                 writable: true,
                 enumerable: true,
                 configurable: true
             });
             return function() {
                 var args = [].slice.apply(arguments);
-                return func.apply(null, [self].concat(args))
+                return func.apply(null, [aThis.__proxy__ ? aThis.__proxy__ : aThis].concat(args))
             }
         } else return func;
     else return func
 }
-export function __getcm__(self, func, quotedFuncName) {
-    if (self.hasOwnProperty("__class__")) return function() {
+export function __getcm__(aThis, func, quotedFuncName) {
+    if (aThis.hasOwnProperty("__class__")) return function() {
         var args = [].slice.apply(arguments);
-        return func.apply(null, [self.__class__].concat(args))
+        return func.apply(null, [aThis.__class__].concat(args))
     };
     else return function() {
         var args = [].slice.apply(arguments);
-        return func.apply(null, [self].concat(args))
+        return func.apply(null, [aThis].concat(args))
     }
 }
-export function __getsm__(self, func, quotedFuncName) {
+export function __getsm__(aThis, func, quotedFuncName) {
     return func
 }
 export var py_metatype = {
     __name__: "type",
     __bases__: [],
     __new__: function(meta, name, bases, attribs) {
         var cls = function() {
@@ -81,14 +80,15 @@
             return cls.__new__(args)
         };
         for (var index = bases.length - 1; index >= 0; index--) {
             var base = bases[index];
             for (var attrib in base) {
                 var descrip =
                     Object.getOwnPropertyDescriptor(base, attrib);
+                if (descrip == null) continue;
                 Object.defineProperty(cls, attrib, descrip)
             }
             for (let symbol of Object.getOwnPropertySymbols(base)) {
                 let descrip = Object.getOwnPropertyDescriptor(base, symbol);
                 Object.defineProperty(cls, symbol, descrip)
             }
         }
@@ -116,42 +116,45 @@
     __new__: function(args) {
         var instance = Object.create(this, {
             __class__: {
                 value: this,
                 enumerable: true
             }
         });
-        if ("__getattr__" in this || "__setattr__" in this) instance = new Proxy(instance, {
-            get: function(target, name) {
-                let result = target[name];
-                if (result == undefined) return target.__getattr__(name);
-                else return result
-            },
-            set: function(target, name, value) {
-                try {
-                    target.__setattr__(name, value)
-                } catch (exception) {
-                    target[name] = value
+        if ("__getattr__" in this || "__setattr__" in this) {
+            instance.__proxy__ = new Proxy(instance, {
+                get: function(target, name) {
+                    let result = target[name];
+                    if (result == undefined) return target.__getattr__(name);
+                    else return result
+                },
+                set: function(target, name, value) {
+                    try {
+                        target.__setattr__(name, value)
+                    } catch (exception) {
+                        target[name] = value
+                    }
+                    return true
                 }
-                return true
-            }
-        });
+            });
+            instance = instance.__proxy__
+        }
         this.__init__.apply(null, [instance].concat(args));
         return instance
     }
 };
 export function __class__(name, bases, attribs, meta) {
     if (meta === undefined) meta = bases[0].__metaclass__;
     return meta.__new__(meta, name, bases, attribs)
 }
 export function __pragma__() {}
 export function __call__() {
     var args = [].slice.apply(arguments);
-    if (typeof args[0] == "object" && "__call__" in args[0]) return args[0].__call__.apply(args[1],
-        args.slice(2));
+    if (typeof args[0] == "object" && "__call__" in
+        args[0]) return args[0].__call__.apply(args[1], args.slice(2));
     else return args[0].apply(args[1], args.slice(2))
 }
 __envir__.executor_name = __envir__.transpiler_name;
 var __main__ = {
     __file__: ""
 };
 var __except__ = null;
@@ -161,17 +164,17 @@
     return anObject
 }
 export function __super__(aClass, methodName) {
     for (let base of aClass.__bases__)
         if (methodName in base) return base[methodName];
     throw new Exception("Superclass method not found");
 }
-export function property(getter, setter) {
-    if (!setter) setter =
-        function() {};
+export function property(getter,
+    setter) {
+    if (!setter) setter = function() {};
     return {
         get: function() {
             return getter(this)
         },
         set: function(value) {
             setter(this, value)
         },
@@ -1328,45 +1331,42 @@
                             kwargs[__attrib0__] = __allkwargs0__[__attrib0__]
                     }
                     delete kwargs.__kwargtrans__
                 }
                 var args = tuple([].slice.apply(arguments).slice(1, __ilastarg0__ + 1))
             } else var args = tuple();
             self.__args__ = args;
-            try {
-                self.stack = kwargs.error.stack
-            } catch (__except0__) {
-                self.stack = "No stack trace available"
-            }
+            if (kwargs.error != null) self.stack = kwargs.error.stack;
+            else if (Error) self.stack = (new Error).stack;
+            else self.stack = "No stack trace available"
         })
     },
     get __repr__() {
-        return __get__(this, function(self) {
-            if (len(self.__args__) > 1) return "{}{}".format(self.__class__.__name__,
-                repr(tuple(self.__args__)));
-            else if (len(self.__args__)) return "{}({})".format(self.__class__.__name__, repr(self.__args__[0]));
-            else return "{}()".format(self.__class__.__name__)
-        })
+        return __get__(this,
+            function(self) {
+                if (len(self.__args__) > 1) return "{}{}".format(self.__class__.__name__, repr(tuple(self.__args__)));
+                else if (len(self.__args__)) return "{}({})".format(self.__class__.__name__, repr(self.__args__[0]));
+                else return "{}()".format(self.__class__.__name__)
+            })
     },
     get __str__() {
         return __get__(this, function(self) {
             if (len(self.__args__) > 1) return str(tuple(self.__args__));
             else if (len(self.__args__)) return str(self.__args__[0]);
             else return ""
         })
     }
 });
 export var IterableError = __class__("IterableError", [Exception], {
     __module__: __name__,
     get __init__() {
         return __get__(this, function(self, error) {
-            Exception.__init__(self,
-                "Can't iterate over non-iterable", __kwargtrans__({
-                    error: error
-                }))
+            Exception.__init__(self, "Can't iterate over non-iterable", __kwargtrans__({
+                error: error
+            }))
         })
     }
 });
 export var StopIteration = __class__("StopIteration", [Exception], {
     __module__: __name__,
     get __init__() {
         return __get__(this, function(self, error) {
@@ -1375,19 +1375,20 @@
             }))
         })
     }
 });
 export var ValueError = __class__("ValueError", [Exception], {
     __module__: __name__,
     get __init__() {
-        return __get__(this, function(self, message, error) {
-            Exception.__init__(self, message, __kwargtrans__({
-                error: error
-            }))
-        })
+        return __get__(this,
+            function(self, message, error) {
+                Exception.__init__(self, message, __kwargtrans__({
+                    error: error
+                }))
+            })
     }
 });
 export var KeyError = __class__("KeyError", [Exception], {
     __module__: __name__,
     get __init__() {
         return __get__(this, function(self, message, error) {
             Exception.__init__(self, message, __kwargtrans__({
@@ -1405,44 +1406,42 @@
             }));
             else Exception.__init__(self, __kwargtrans__({
                 error: error
             }))
         })
     }
 });
-export var NotImplementedError =
-    __class__("NotImplementedError", [Exception], {
-        __module__: __name__,
-        get __init__() {
-            return __get__(this, function(self, message, error) {
-                Exception.__init__(self, message, __kwargtrans__({
-                    error: error
-                }))
-            })
-        }
-    });
+export var NotImplementedError = __class__("NotImplementedError", [Exception], {
+    __module__: __name__,
+    get __init__() {
+        return __get__(this, function(self, message, error) {
+            Exception.__init__(self, message, __kwargtrans__({
+                error: error
+            }))
+        })
+    }
+});
 export var IndexError = __class__("IndexError", [Exception], {
     __module__: __name__,
     get __init__() {
         return __get__(this, function(self, message, error) {
             Exception.__init__(self, message, __kwargtrans__({
                 error: error
             }))
         })
     }
 });
 export var AttributeError = __class__("AttributeError", [Exception], {
     __module__: __name__,
     get __init__() {
-        return __get__(this,
-            function(self, message, error) {
-                Exception.__init__(self, message, __kwargtrans__({
-                    error: error
-                }))
-            })
+        return __get__(this, function(self, message, error) {
+            Exception.__init__(self, message, __kwargtrans__({
+                error: error
+            }))
+        })
     }
 });
 export var py_TypeError = __class__("py_TypeError", [Exception], {
     __module__: __name__,
     get __init__() {
         return __get__(this, function(self, message, error) {
             Exception.__init__(self, message, __kwargtrans__({
@@ -1453,29 +1452,27 @@
 });
 export var Warning = __class__("Warning", [Exception], {
     __module__: __name__
 });
 export var UserWarning = __class__("UserWarning", [Warning], {
     __module__: __name__
 });
-export var DeprecationWarning = __class__("DeprecationWarning",
-    [Warning], {
-        __module__: __name__
-    });
+export var DeprecationWarning = __class__("DeprecationWarning", [Warning], {
+    __module__: __name__
+});
 export var RuntimeWarning = __class__("RuntimeWarning", [Warning], {
     __module__: __name__
 });
 export var __sort__ = function(iterable, key, reverse) {
     if (typeof key == "undefined" || key != null && key.hasOwnProperty("__kwargtrans__")) var key = null;
     if (typeof reverse == "undefined" || reverse != null && reverse.hasOwnProperty("__kwargtrans__")) var reverse = false;
     if (arguments.length) {
         var __ilastarg0__ = arguments.length - 1;
         if (arguments[__ilastarg0__] && arguments[__ilastarg0__].hasOwnProperty("__kwargtrans__")) {
-            var __allkwargs0__ =
-                arguments[__ilastarg0__--];
+            var __allkwargs0__ = arguments[__ilastarg0__--];
             for (var __attrib0__ in __allkwargs0__) switch (__attrib0__) {
                 case "iterable":
                     var iterable = __allkwargs0__[__attrib0__];
                     break;
                 case "key":
                     var key = __allkwargs0__[__attrib0__];
                     break;
@@ -1483,15 +1480,16 @@
                     var reverse = __allkwargs0__[__attrib0__];
                     break
             }
         }
     } else;
     if (key) iterable.sort(function __lambda__(a, b) {
         if (arguments.length) {
-            var __ilastarg0__ = arguments.length - 1;
+            var __ilastarg0__ =
+                arguments.length - 1;
             if (arguments[__ilastarg0__] && arguments[__ilastarg0__].hasOwnProperty("__kwargtrans__")) {
                 var __allkwargs0__ = arguments[__ilastarg0__--];
                 for (var __attrib0__ in __allkwargs0__) switch (__attrib0__) {
                     case "a":
                         var a = __allkwargs0__[__attrib0__];
                         break;
                     case "b":
@@ -1502,38 +1500,38 @@
         } else;
         return key(a) > key(b) ? 1 : -1
     });
     else iterable.sort();
     if (reverse) iterable.reverse()
 };
 export var sorted = function(iterable, key, reverse) {
-    if (typeof key == "undefined" || key != null && key.hasOwnProperty("__kwargtrans__")) var key = null;
+    if (typeof key == "undefined" || key != null && key.hasOwnProperty("__kwargtrans__")) var key =
+        null;
     if (typeof reverse == "undefined" || reverse != null && reverse.hasOwnProperty("__kwargtrans__")) var reverse = false;
     if (arguments.length) {
-        var __ilastarg0__ =
-            arguments.length - 1;
+        var __ilastarg0__ = arguments.length - 1;
         if (arguments[__ilastarg0__] && arguments[__ilastarg0__].hasOwnProperty("__kwargtrans__")) {
             var __allkwargs0__ = arguments[__ilastarg0__--];
             for (var __attrib0__ in __allkwargs0__) switch (__attrib0__) {
                 case "iterable":
                     var iterable = __allkwargs0__[__attrib0__];
                     break;
                 case "key":
                     var key = __allkwargs0__[__attrib0__];
                     break;
                 case "reverse":
-                    var reverse = __allkwargs0__[__attrib0__];
+                    var reverse =
+                        __allkwargs0__[__attrib0__];
                     break
             }
         }
     } else;
     if (py_typeof(iterable) == dict) var result = copy(iterable.py_keys());
     else var result = copy(iterable);
-    __sort__(result,
-        key, reverse);
+    __sort__(result, key, reverse);
     return result
 };
 export var map = function(func, iterable) {
     return function() {
         var __accu0__ = [];
         for (var item of iterable) __accu0__.append(func(item));
         return __accu0__
@@ -1566,76 +1564,77 @@
                 self.element.style.boxSizing = "border-box";
                 self.element.style.padding = "5px";
                 self.element.innerHTML = "_"
             }
         })
     },
     get print() {
-        return __get__(this, function(self) {
-            var sep = " ";
-            var end = "\n";
-            if (arguments.length) {
-                var __ilastarg0__ = arguments.length - 1;
-                if (arguments[__ilastarg0__] && arguments[__ilastarg0__].hasOwnProperty("__kwargtrans__")) {
-                    var __allkwargs0__ =
-                        arguments[__ilastarg0__--];
-                    for (var __attrib0__ in __allkwargs0__) switch (__attrib0__) {
-                        case "self":
-                            var self = __allkwargs0__[__attrib0__];
-                            break;
-                        case "sep":
-                            var sep = __allkwargs0__[__attrib0__];
-                            break;
-                        case "end":
-                            var end = __allkwargs0__[__attrib0__];
-                            break
+        return __get__(this,
+            function(self) {
+                var sep = " ";
+                var end = "\n";
+                if (arguments.length) {
+                    var __ilastarg0__ = arguments.length - 1;
+                    if (arguments[__ilastarg0__] && arguments[__ilastarg0__].hasOwnProperty("__kwargtrans__")) {
+                        var __allkwargs0__ = arguments[__ilastarg0__--];
+                        for (var __attrib0__ in __allkwargs0__) switch (__attrib0__) {
+                            case "self":
+                                var self = __allkwargs0__[__attrib0__];
+                                break;
+                            case "sep":
+                                var sep = __allkwargs0__[__attrib0__];
+                                break;
+                            case "end":
+                                var end = __allkwargs0__[__attrib0__];
+                                break
+                        }
                     }
-                }
-                var args = tuple([].slice.apply(arguments).slice(1, __ilastarg0__ + 1))
-            } else var args = tuple();
-            self.buffer = "{}{}{}".format(self.buffer, sep.join(function() {
-                var __accu0__ = [];
-                for (var arg of args) __accu0__.append(str(arg));
-                return __accu0__
-            }()), end).__getslice__(-4096,
-                null, 1);
-            if (self.element) {
-                self.element.innerHTML = self.buffer.py_replace("\n", "<br>").py_replace(" ", "&nbsp");
-                self.element.scrollTop = self.element.scrollHeight
-            } else console.log(sep.join(function() {
-                var __accu0__ = [];
-                for (var arg of args) __accu0__.append(str(arg));
-                return __accu0__
-            }()))
-        })
+                    var args = tuple([].slice.apply(arguments).slice(1,
+                        __ilastarg0__ + 1))
+                } else var args = tuple();
+                self.buffer = "{}{}{}".format(self.buffer, sep.join(function() {
+                    var __accu0__ = [];
+                    for (var arg of args) __accu0__.append(str(arg));
+                    return __accu0__
+                }()), end).__getslice__(-4096, null, 1);
+                if (self.element) {
+                    self.element.innerHTML = self.buffer.py_replace("\n", "<br>").py_replace(" ", "&nbsp");
+                    self.element.scrollTop = self.element.scrollHeight
+                } else console.log(sep.join(function() {
+                    var __accu0__ = [];
+                    for (var arg of args) __accu0__.append(str(arg));
+                    return __accu0__
+                }()))
+            })
     },
     get input() {
-        return __get__(this, function(self, question) {
-            if (arguments.length) {
-                var __ilastarg0__ = arguments.length - 1;
-                if (arguments[__ilastarg0__] && arguments[__ilastarg0__].hasOwnProperty("__kwargtrans__")) {
-                    var __allkwargs0__ =
-                        arguments[__ilastarg0__--];
-                    for (var __attrib0__ in __allkwargs0__) switch (__attrib0__) {
-                        case "self":
-                            var self = __allkwargs0__[__attrib0__];
-                            break;
-                        case "question":
-                            var question = __allkwargs0__[__attrib0__];
-                            break
+        return __get__(this,
+            function(self, question) {
+                if (arguments.length) {
+                    var __ilastarg0__ = arguments.length - 1;
+                    if (arguments[__ilastarg0__] && arguments[__ilastarg0__].hasOwnProperty("__kwargtrans__")) {
+                        var __allkwargs0__ = arguments[__ilastarg0__--];
+                        for (var __attrib0__ in __allkwargs0__) switch (__attrib0__) {
+                            case "self":
+                                var self = __allkwargs0__[__attrib0__];
+                                break;
+                            case "question":
+                                var question = __allkwargs0__[__attrib0__];
+                                break
+                        }
                     }
-                }
-            } else;
-            self.print("{}".format(question), __kwargtrans__({
-                end: ""
-            }));
-            var answer = window.prompt("\n".join(self.buffer.py_split("\n").__getslice__(-8, null, 1)));
-            self.print(answer);
-            return answer
-        })
+                } else;
+                self.print("{}".format(question), __kwargtrans__({
+                    end: ""
+                }));
+                var answer = window.prompt("\n".join(self.buffer.py_split("\n").__getslice__(-8,
+                    null, 1)));
+                self.print(answer);
+                return answer
+            })
     }
 });
 export var __terminal__ = __Terminal__();
 export var print = __terminal__.print;
 export var input = __terminal__.input;
 
 //# sourceMappingURL=org.transcrypt.__runtime__.map
```

### Comparing `talqual-0.0.2/talqual/static/scripts.js` & `talqual-0.0.3/talqual/static/scripts.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -61,15 +61,14 @@
     __mul__,
     __ne__,
     __neg__,
     __nest__,
     __or__,
     __pow__,
     __pragma__,
-    __proxy__,
     __pyUseJsNext__,
     __rshift__,
     __setitem__,
     __setproperty__,
     __setslice__,
     __sort__,
     __specialattrib__,
@@ -129,33 +128,58 @@
     str,
     sum,
     tuple,
     zip
 } from "./org.transcrypt.__runtime__.js";
 var __name__ = "__main__";
 export var is_checked = function(element, filter_class) {
-    return " {} ".format(element.className).indexOf(" {} ".format(filter_class)) > -1
+    return (" " + element.className + " ").indexOf(" " + filter_class + " ") > -1
 };
 export var style_hide = function(element) {
     if (element.style) element.style.display = "none";
-    else element.style =
-        dict({
-            "display": "none"
-        })
+    else element.style = dict({
+        "display": "none"
+    })
 };
 export var style_display = function(element) {
     if (element.style) element.style.display = ""
 };
+export var Calendar = __class__("Calendar", [object], {
+    __module__: __name__,
+    get __init__() {
+        return __get__(this, function(self, data_class) {
+            self.data_class = data_class;
+            self.run()
+        })
+    },
+    get _get_data() {
+        return __get__(this, function(self) {
+            return document.getElementsByClassName(self.data_class)
+        })
+    },
+    get run() {
+        return __get__(this, function(self) {
+            var now = Date.now();
+            for (var calendar of self.data)
+                for (var entry of calendar.childNodes)
+                    if (__in__("date",
+                            entry.dataset))
+                        if (now < Date.parse(entry.dataset.date)) style_display(entry);
+                        else style_hide(entry)
+        })
+    }
+});
+Object.defineProperty(Calendar, "data", property.call(Calendar, Calendar._get_data));
 export var Faceted = __class__("Faceted", [object], {
     __module__: __name__,
     get __init__() {
         return __get__(this, function(self, data_class, batch_size, pagination_class) {
             if (typeof batch_size == "undefined" || batch_size != null && batch_size.hasOwnProperty("__kwargtrans__")) var batch_size = null;
-            if (typeof pagination_class == "undefined" || pagination_class != null && pagination_class.hasOwnProperty("__kwargtrans__")) var pagination_class =
-                null;
+            if (typeof pagination_class == "undefined" || pagination_class !=
+                null && pagination_class.hasOwnProperty("__kwargtrans__")) var pagination_class = null;
             self.data_class = data_class;
             self.batch_size = batch_size;
             self.size = 0;
             self.pagination_class = pagination_class;
             self.batch_faceted = null;
             self.batch_pagination = [];
             self.py_values = null;
@@ -167,38 +191,39 @@
         return __get__(this, function(self) {
             return document.getElementsByClassName(self.data_class)
         })
     },
     get next_callback() {
         return __get__(this, function(self) {
             if (self.next_url !== null) {
-                self.batch_faceted.innerHTML = "";
+                self.batch_faceted.innerHTML =
+                    "";
                 return self._next_faceted(self.next_url)
             }
         })
     },
     get _next_url() {
-        return __get__(this,
-            function(self, html) {
-                var a_next = html.querySelector('.{} [rel="next"]'.format(self.pagination_class));
-                if (bool(a_next)) return a_next.getAttribute("href")
-            })
+        return __get__(this, function(self, html) {
+            var a_next = html.querySelector("." + self.pagination_class + ' [rel="next"]');
+            if (bool(a_next)) return a_next.getAttribute("href")
+        })
     },
     get _next_faceted() {
         return __get__(this, function(self, next_url) {
             if (next_url === null) return;
             if (self.size >= self.batch_size) {
                 self.next_url = next_url;
                 self.size = 0;
                 return
             }
             self.next_url = null;
             var xhr = new XMLHttpRequest;
             var parse_faceted = function() {
-                if (xhr.readyState == 4 && xhr.status == 200) {
+                if (xhr.readyState == 4 && xhr.status ==
+                    200) {
                     var html = document.createElement("html");
                     html.innerHTML = xhr.responseText;
                     var faceted_html = html.getElementsByClassName(self.data_class);
                     self.filter_field(faceted_html);
                     self._next_faceted(self._next_url(html))
                 }
             };
@@ -210,44 +235,46 @@
     get init_filtering() {
         return __get__(this, function(self) {
             if (self.batch_faceted !== null) {
                 self.batch_faceted.innerHTML = "";
                 return
             }
             for (var faceted of self.data) style_hide(faceted);
-            var paginations = document.querySelectorAll(".{}".format(self.pagination_class));
+            var paginations = document.querySelectorAll("." +
+                self.pagination_class);
             for (var pagination of paginations) style_hide(pagination);
-            var original = self.data[0];
+            var original = self.data.item(0);
             var faceted = original.cloneNode(false);
             style_display(faceted);
             original.insertAdjacentElement("afterend", faceted);
             self.batch_faceted = faceted;
             for (var pagination of paginations) {
                 var pagination_clone = pagination.cloneNode(false);
                 style_display(pagination_clone);
                 pagination.insertAdjacentElement("afterend", pagination_clone);
                 for (var link_next of pagination.querySelectorAll('[rel="next"]')) {
-                    var next_clone = link_next.cloneNode(true);
+                    var next_clone =
+                        link_next.cloneNode(true);
                     next_clone.removeAttribute("href");
-                    next_clone.addEventListener("click",
-                        self.next_callback);
+                    next_clone.addEventListener("click", self.next_callback);
                     pagination_clone.insertAdjacentElement("beforeend", next_clone)
                 }
                 self.batch_pagination.append(pagination_clone)
             }
         })
     },
     get end_filtering() {
         return __get__(this, function(self) {
             self.batch_faceted.remove();
             self.batch_faceted = null;
             for (var pagination of self.batch_pagination) pagination.remove();
             self.batch_pagination = [];
             for (var faceted of self.data) style_display(faceted);
-            var paginations = document.querySelectorAll(".{}".format(self.pagination_class));
+            var paginations = document.querySelectorAll("." +
+                self.pagination_class);
             for (var pagination of paginations) style_display(pagination)
         })
     },
     get _select_element() {
         return __get__(this, function(self, element, select) {
             if (typeof select == "undefined" || select != null && select.hasOwnProperty("__kwargtrans__")) var select = true;
             if (self.batch_faceted !== null) {
@@ -256,19 +283,21 @@
                     self.batch_faceted.insertAdjacentElement("beforeend", clone)
                 }
             } else if (select) style_display(element);
             else style_hide(element)
         })
     },
     get _filter_one() {
-        return __get__(this, function(self, faceted) {
+        return __get__(this, function(self,
+            faceted) {
             for (var element of faceted.childNodes) {
+                if (element.nodeType != 1) continue;
                 var hide = bool(self.py_values);
                 for (var value of self.py_values) {
-                    var filter_class = "{}-{}".format(self.field_name, value);
+                    var filter_class = self.field_name + "-" + value;
                     if (is_checked(element, filter_class)) {
                         var hide = false;
                         self.size++;
                         break
                     }
                 }
                 self._select_element(element, !hide);
@@ -280,14 +309,15 @@
         return __get__(this, function(self, field) {
             if (len(field.selectedOptions) > 1) self.py_values = function() {
                 var __accu0__ = [];
                 for (var option of field.selectedOptions) __accu0__.append(option.value);
                 return __accu0__
             }();
             else if (field.value) self.py_values = [field.value];
+            else if (len(field.selected) > 0) self.py_values = field.selected;
             else self.py_values = [];
             if (self.batch_faceted !== null && !bool(self.py_values)) {
                 self.end_filtering();
                 return
             }
             if (self.batch_size) self.init_filtering();
             self.field_name = field.getAttribute("name");
@@ -298,16 +328,15 @@
     get filter_field() {
         return __get__(this, function(self, data) {
             for (var faceted of data)
                 if (!faceted.isEqualNode(self.batch_faceted)) self._filter_one(faceted)
         })
     }
 });
-Object.defineProperty(Faceted, "data",
-    property.call(Faceted, Faceted._get_data));
+Object.defineProperty(Faceted, "data", property.call(Faceted, Faceted._get_data));
 export var VirtualSelect = __class__("VirtualSelect", [object], {
     __module__: __name__,
     get __init__() {
         return __get__(this, function(self, py_name, faceted) {
             if (typeof faceted == "undefined" || faceted != null && faceted.hasOwnProperty("__kwargtrans__")) var faceted = null;
             self.py_name = py_name;
             self.faceted = faceted;
@@ -316,17 +345,18 @@
     },
     get _call_onchange() {
         return __get__(this, function(self) {
             if (self.faceted) self.faceted.filter(self)
         })
     },
     get _get_value() {
-        return __get__(this, function(self) {
-            if (self.selected) return self.selected[0]
-        })
+        return __get__(this,
+            function(self) {
+                if (self.selected) return self.selected[0]
+            })
     },
     get _get_selectedOptions() {
         return __get__(this, function(self) {
             return function() {
                 var __accu0__ = [];
                 for (var value of self.selected) __accu0__.append(dict({
                     "value": value
@@ -344,15 +374,16 @@
         return __get__(this, function(self) {
             self.selected = [];
             self._call_onchange()
         })
     },
     get toggle() {
         return __get__(this, function(self, value) {
-            if (__in__(value, self.selected)) self.selected.remove(value);
+            if (__in__(value,
+                    self.selected)) self.selected.remove(value);
             else self.selected.append(value);
             self._call_onchange()
         })
     }
 });
 Object.defineProperty(VirtualSelect, "selectedOptions", property.call(VirtualSelect, VirtualSelect._get_selectedOptions));
 Object.defineProperty(VirtualSelect, "value", property.call(VirtualSelect, VirtualSelect._get_value));
```

