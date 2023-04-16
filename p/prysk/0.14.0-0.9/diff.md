# Comparing `tmp/prysk-0.14.0.tar.gz` & `tmp/prysk-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prysk-0.14.0.tar", max compression
+gzip compressed data, was "prysk-0.9.tar", last modified: Sat Jan 29 10:05:38 2022, max compression
```

## Comparing `prysk-0.14.0.tar` & `prysk-0.9.tar`

### file list

```diff
@@ -1,38 +1,61 @@
--rw-r--r--   0        0        0    18092 2023-02-13 20:47:09.460930 prysk-0.14.0/COPYING.txt
--rw-r--r--   0        0        0     6397 2023-04-16 09:02:29.363158 prysk-0.14.0/README.rst
--rw-r--r--   0        0        0      462 2023-02-13 20:47:09.461930 prysk-0.14.0/contrib/PKGBUILD
--rw-r--r--   0        0        0     1342 2023-02-13 20:47:09.461930 prysk-0.14.0/contrib/cram.vim
--rw-r--r--   0        0        0      307 2023-02-13 20:47:09.462930 prysk-0.14.0/docs/_templates/versions.html
--rw-r--r--   0        0        0     2617 2023-02-13 20:47:09.462930 prysk-0.14.0/docs/conf.py
--rw-r--r--   0        0        0      835 2023-02-13 20:47:34.550274 prysk-0.14.0/docs/contributors.rst
--rw-r--r--   0        0        0     1118 2023-02-13 20:47:09.465930 prysk-0.14.0/docs/development.rst
--rw-r--r--   0        0        0     2026 2023-02-13 20:47:09.465930 prysk-0.14.0/docs/getting_started.rst
--rw-r--r--   0        0        0      392 2023-02-16 18:47:21.069606 prysk-0.14.0/docs/index.rst
--rw-r--r--   0        0        0     6584 2023-02-13 20:47:09.466930 prysk-0.14.0/docs/news.rst
--rw-r--r--   0        0        0     2516 2023-04-16 09:55:50.957857 prysk-0.14.0/docs/prysk_news.rst
--rw-r--r--   0        0        0     1190 2023-03-03 20:16:25.741872 prysk-0.14.0/docs/pytest-plugin.rst
--rw-r--r--   0        0        0       27 2023-02-13 20:47:09.467930 prysk-0.14.0/docs/readme.rst
--rw-r--r--   0        0        0       42 2023-02-13 20:47:09.467930 prysk-0.14.0/examples/.hidden/hidden.t
--rw-r--r--   0        0        0       42 2023-02-13 20:47:09.467930 prysk-0.14.0/examples/.hidden.t
--rw-r--r--   0        0        0        9 2023-02-13 20:47:09.467930 prysk-0.14.0/examples/bare.t
--rw-r--r--   0        0        0        0 2023-02-13 20:47:09.467930 prysk-0.14.0/examples/empty.t
--rw-r--r--   0        0        0      476 2023-04-16 09:02:29.363158 prysk-0.14.0/examples/env.t
--rw-r--r--   0        0        0      397 2023-02-13 20:47:09.468930 prysk-0.14.0/examples/fail.t
--rw-r--r--   0        0        0       29 2023-02-13 20:47:09.469930 prysk-0.14.0/examples/missingeol.t
--rw-r--r--   0        0        0      179 2023-02-13 20:47:09.469930 prysk-0.14.0/examples/skip.t
--rw-r--r--   0        0        0     1441 2023-04-16 09:02:29.364158 prysk-0.14.0/examples/test.t
--rw-r--r--   0        0        0     4054 2023-02-16 18:47:21.070606 prysk-0.14.0/noxfile.py
--rw-r--r--   0        0        0   107051 2023-04-16 09:42:24.991677 prysk-0.14.0/poetry.lock
--rw-r--r--   0        0        0      261 2023-02-13 20:47:09.475930 prysk-0.14.0/prysk/__init__.py
--rw-r--r--   0        0        0      177 2023-02-13 20:47:09.475930 prysk-0.14.0/prysk/__main__.py
--rw-r--r--   0        0        0    17100 2023-04-16 09:55:50.957857 prysk-0.14.0/prysk/cli.py
--rw-r--r--   0        0        0     5291 2023-02-13 20:47:09.477930 prysk-0.14.0/prysk/diff.py
--rw-r--r--   0        0        0     1750 2023-02-13 20:47:09.477930 prysk-0.14.0/prysk/process.py
--rw-r--r--   0        0        0     1507 2023-02-13 20:47:09.478930 prysk-0.14.0/prysk/settings.py
--rw-r--r--   0        0        0    10809 2023-04-16 09:02:29.364158 prysk-0.14.0/prysk/test.py
--rw-r--r--   0        0        0     5357 2023-02-13 20:47:09.479930 prysk-0.14.0/prysk/xunit.py
--rw-r--r--   0        0        0     2712 2023-04-16 09:55:50.957857 prysk-0.14.0/pyproject.toml
--rw-r--r--   0        0        0     4642 2023-03-04 17:56:46.398259 prysk-0.14.0/pytest_prysk/__init__.py
--rw-r--r--   0        0        0      694 2023-02-13 20:47:09.480930 prysk-0.14.0/scripts/md5.py
--rw-r--r--   0        0        0     7527 1970-01-01 00:00:00.000000 prysk-0.14.0/setup.py
--rw-r--r--   0        0        0     7887 1970-01-01 00:00:00.000000 prysk-0.14.0/PKG-INFO
+drwxr-xr-x   0 nicoretti  (1000) nicoretti  (1000)        0 2022-01-29 10:05:38.814325 prysk-0.9/
+-rw-r--r--   0 nicoretti  (1000) nicoretti  (1000)       21 2022-01-29 10:05:06.685780 prysk-0.9/.coveragerc
+-rw-r--r--   0 nicoretti  (1000) nicoretti  (1000)      965 2022-01-20 20:42:40.076459 prysk-0.9/.pylintrc
+-rw-r--r--   0 nicoretti  (1000) nicoretti  (1000)    18092 2022-01-20 20:42:40.076459 prysk-0.9/COPYING.txt
+-rw-r--r--   0 nicoretti  (1000) nicoretti  (1000)      217 2022-01-29 10:05:06.685780 prysk-0.9/MANIFEST.in
+-rw-r--r--   0 nicoretti  (1000) nicoretti  (1000)     8788 2022-01-29 10:05:38.815325 prysk-0.9/PKG-INFO
+-rw-r--r--   0 nicoretti  (1000) nicoretti  (1000)     6403 2022-01-29 10:05:06.686780 prysk-0.9/README.rst
+drwxr-xr-x   0 nicoretti  (1000) nicoretti  (1000)        0 2022-01-29 10:05:38.813325 prysk-0.9/contrib/
+-rw-r--r--   0 nicoretti  (1000) nicoretti  (1000)     1342 2022-01-20 20:42:40.076459 prysk-0.9/contrib/cram.vim
+drwxr-xr-x   0 nicoretti  (1000) nicoretti  (1000)        0 2022-01-29 10:05:38.813325 prysk-0.9/docs/
+-rw-r--r--   0 nicoretti  (1000) nicoretti  (1000)      634 2022-01-29 10:05:06.686780 prysk-0.9/docs/Makefile
+-rw-r--r--   0 nicoretti  (1000) nicoretti  (1000)     2512 2022-01-29 10:05:06.686780 prysk-0.9/docs/conf.py
+-rw-r--r--   0 nicoretti  (1000) nicoretti  (1000)      304 2022-01-29 10:05:06.686780 prysk-0.9/docs/development.rst
+-rw-r--r--   0 nicoretti  (1000) nicoretti  (1000)       21 2022-01-29 10:05:06.686780 prysk-0.9/docs/examples.rst
+-rw-r--r--   0 nicoretti  (1000) nicoretti  (1000)       17 2022-01-29 10:05:06.686780 prysk-0.9/docs/format.rst
+-rw-r--r--   0 nicoretti  (1000) nicoretti  (1000)      501 2022-01-29 10:05:06.686780 prysk-0.9/docs/index.rst
+-rw-r--r--   0 nicoretti  (1000) nicoretti  (1000)       72 2022-01-29 10:05:06.686780 prysk-0.9/docs/installation.rst
+-rw-r--r--   0 nicoretti  (1000) nicoretti  (1000)     7129 2022-01-29 10:05:06.687780 prysk-0.9/docs/news.rst
+-rw-r--r--   0 nicoretti  (1000) nicoretti  (1000)       27 2022-01-29 10:05:06.687780 prysk-0.9/docs/readme.rst
+drwxr-xr-x   0 nicoretti  (1000) nicoretti  (1000)        0 2022-01-29 10:05:38.814325 prysk-0.9/examples/
+drwxr-xr-x   0 nicoretti  (1000) nicoretti  (1000)        0 2022-01-29 10:05:38.814325 prysk-0.9/examples/.hidden/
+-rw-r--r--   0 nicoretti  (1000) nicoretti  (1000)       42 2022-01-20 20:42:40.077458 prysk-0.9/examples/.hidden/hidden.t
+-rw-r--r--   0 nicoretti  (1000) nicoretti  (1000)       42 2022-01-20 20:42:40.076459 prysk-0.9/examples/.hidden.t
+-rw-r--r--   0 nicoretti  (1000) nicoretti  (1000)        9 2022-01-20 20:42:40.077458 prysk-0.9/examples/bare.t
+-rw-r--r--   0 nicoretti  (1000) nicoretti  (1000)        0 2022-01-20 20:42:40.077458 prysk-0.9/examples/empty.t
+-rw-r--r--   0 nicoretti  (1000) nicoretti  (1000)      397 2022-01-25 20:58:26.710373 prysk-0.9/examples/env.t
+-rw-r--r--   0 nicoretti  (1000) nicoretti  (1000)      397 2022-01-20 20:42:40.077458 prysk-0.9/examples/fail.t
+-rw-r--r--   0 nicoretti  (1000) nicoretti  (1000)       29 2022-01-20 20:42:40.077458 prysk-0.9/examples/missingeol.t
+-rw-r--r--   0 nicoretti  (1000) nicoretti  (1000)      179 2022-01-20 20:42:40.077458 prysk-0.9/examples/skip.t
+-rw-r--r--   0 nicoretti  (1000) nicoretti  (1000)     1339 2022-01-20 20:42:40.077458 prysk-0.9/examples/test.t
+drwxr-xr-x   0 nicoretti  (1000) nicoretti  (1000)        0 2022-01-29 10:05:38.814325 prysk-0.9/prysk/
+-rw-r--r--   0 nicoretti  (1000) nicoretti  (1000)      180 2022-01-29 10:05:06.687780 prysk-0.9/prysk/__init__.py
+-rw-r--r--   0 nicoretti  (1000) nicoretti  (1000)      175 2022-01-25 20:58:26.710373 prysk-0.9/prysk/__main__.py
+-rw-r--r--   0 nicoretti  (1000) nicoretti  (1000)     5409 2022-01-25 20:58:26.711373 prysk-0.9/prysk/_diff.py
+-rw-r--r--   0 nicoretti  (1000) nicoretti  (1000)     1741 2022-01-29 10:05:06.687780 prysk-0.9/prysk/_process.py
+-rw-r--r--   0 nicoretti  (1000) nicoretti  (1000)     2452 2022-01-29 10:05:06.687780 prysk-0.9/prysk/_run.py
+-rw-r--r--   0 nicoretti  (1000) nicoretti  (1000)     7663 2022-01-29 10:05:06.687780 prysk-0.9/prysk/_test.py
+-rw-r--r--   0 nicoretti  (1000) nicoretti  (1000)     5933 2022-01-29 10:05:06.688780 prysk-0.9/prysk/_xunit.py
+-rw-r--r--   0 nicoretti  (1000) nicoretti  (1000)     7668 2022-01-29 10:05:06.688780 prysk-0.9/prysk/application.py
+-rw-r--r--   0 nicoretti  (1000) nicoretti  (1000)     4524 2022-01-29 10:05:06.688780 prysk-0.9/prysk/cli.py
+-rw-r--r--   0 nicoretti  (1000) nicoretti  (1000)       72 2022-01-29 10:05:06.688780 prysk-0.9/requirements.txt
+drwxr-xr-x   0 nicoretti  (1000) nicoretti  (1000)        0 2022-01-29 10:05:38.814325 prysk-0.9/scripts/
+-rw-r--r--   0 nicoretti  (1000) nicoretti  (1000)      591 2022-01-25 08:01:58.810960 prysk-0.9/scripts/md5.py
+-rw-r--r--   0 nicoretti  (1000) nicoretti  (1000)      301 2022-01-20 20:42:40.077458 prysk-0.9/setup.cfg
+-rwxr-xr-x   0 nicoretti  (1000) nicoretti  (1000)     1610 2022-01-29 10:05:06.688780 prysk-0.9/setup.py
+drwxr-xr-x   0 nicoretti  (1000) nicoretti  (1000)        0 2022-01-29 10:05:38.814325 prysk-0.9/tests/
+-rw-r--r--   0 nicoretti  (1000) nicoretti  (1000)      907 2022-01-25 20:58:26.712373 prysk-0.9/tests/config.t
+-rw-r--r--   0 nicoretti  (1000) nicoretti  (1000)     1416 2022-01-25 20:58:26.712373 prysk-0.9/tests/debug.t
+-rw-r--r--   0 nicoretti  (1000) nicoretti  (1000)      247 2022-01-20 20:42:40.077458 prysk-0.9/tests/dist.t
+-rw-r--r--   0 nicoretti  (1000) nicoretti  (1000)      113 2022-01-26 13:06:23.032621 prysk-0.9/tests/doctest.t
+-rw-r--r--   0 nicoretti  (1000) nicoretti  (1000)     1503 2022-01-25 20:58:26.712373 prysk-0.9/tests/encoding.t
+-rw-r--r--   0 nicoretti  (1000) nicoretti  (1000)     6792 2022-01-25 20:58:26.712373 prysk-0.9/tests/interactive.t
+-rw-r--r--   0 nicoretti  (1000) nicoretti  (1000)      669 2022-01-25 20:58:26.713373 prysk-0.9/tests/md5.t
+-rw-r--r--   0 nicoretti  (1000) nicoretti  (1000)      232 2022-01-26 13:06:23.032621 prysk-0.9/tests/pep8.t
+-rw-r--r--   0 nicoretti  (1000) nicoretti  (1000)      186 2022-01-26 13:06:23.033621 prysk-0.9/tests/pyflakes.t
+-rw-r--r--   0 nicoretti  (1000) nicoretti  (1000)     1186 2022-01-25 20:58:26.713373 prysk-0.9/tests/run-doctests.py
+-rw-r--r--   0 nicoretti  (1000) nicoretti  (1000)     1103 2022-01-29 10:05:06.689780 prysk-0.9/tests/setup.sh
+-rw-r--r--   0 nicoretti  (1000) nicoretti  (1000)     3205 2022-01-25 20:58:26.713373 prysk-0.9/tests/test.t
+-rw-r--r--   0 nicoretti  (1000) nicoretti  (1000)     1581 2022-01-25 20:58:26.713373 prysk-0.9/tests/usage.t
+-rw-r--r--   0 nicoretti  (1000) nicoretti  (1000)     2353 2022-01-25 20:58:26.714373 prysk-0.9/tests/xunit.t
+-rw-r--r--   0 nicoretti  (1000) nicoretti  (1000)      874 2022-01-29 10:05:06.689780 prysk-0.9/tox.ini
```

### Comparing `prysk-0.14.0/COPYING.txt` & `prysk-0.9/COPYING.txt`

 * *Files identical despite different names*

### Comparing `prysk-0.14.0/README.rst` & `prysk-0.9/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,32 @@
 Prysk
 ======================
-.. image:: https://img.shields.io/github/actions/workflow/status/nicoretti/prysk/verifier.yaml
-    :target: https://github.com/Nicoretti/prysk/actions
+.. image:: https://github.com/Nicoretti/prysk/actions/workflows/verifier.yaml/badge.svg
+    :target: https://github.com/Nicoretti/prysk/actions/workflows/verifier.yaml
 
-.. image:: https://img.shields.io/coverallsCoverage/github/Nicoretti/prysk
-    :target: https://coveralls.io/github/Nicoretti/prysk
+.. image:: https://coveralls.io/repos/github/Nicoretti/prysk/badge.svg?branch=master
+    :target: https://coveralls.io/github/Nicoretti/prysk?branch=master
 
-.. image:: https://img.shields.io/badge/imports-isort-ef8336.svg
-    :target: https://pycqa.github.io/isort/
-
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-   :target: https://github.com/psf/black
-
-.. image:: https://img.shields.io/pypi/v/prysk
+.. image:: https://img.shields.io/badge/pypi%20package-available-blue.svg
     :target: https://pypi.org/project/prysk/
 
 .. image:: https://img.shields.io/badge/docs-available-blue.svg
     :target: https://nicoretti.github.io/prysk/
 
 Prysk is a fork of the popular snapshot testing tool Cram_.
 Even though Cram_ is pretty complete and mature for everyday use,
-Prysk wants to continue pushing its development forward.
+Prysk want's to continue pushing it's development forward.
 
 .. _Cram: https://bitheap.org/cram
 
 Prysk tests look like snippets of interactive shell sessions. Prysk runs
 each command and compares the command output in the test with the
 command's actual output.
 
-Here's a snippet from `Prysk's own test suite`_:
-
-.. code-block:: console
+Here's a snippet from `Prysk's own test suite`_::
 
     Set up prysk alias and example tests:
 
       $ . "$TESTDIR"/setup.sh
 
     Usage:
 
@@ -57,18 +49,18 @@
         --indent=NUM        number of spaces to use for indentation (default: 2)
         --xunit-file=PATH   path to write xUnit XML output
 
 The format in a nutshell:
 
 * Prysk tests use the ``.t`` file extension.
 
-* Lines beginning with two spaces, a dollar sign (``$``), and a space are run
+* Lines beginning with two spaces, a dollar sign, and a space are run
   in the shell.
 
-* Lines beginning with two spaces, a greater than sign (``>``), and a space
+* Lines beginning with two spaces, a greater than sign, and a space
   allow multi-line commands.
 
 * All other lines beginning with two spaces are considered command
   output.
 
 * Output lines ending with a space and the keyword ``(re)`` are
   matched as `Perl-compatible regular expressions`_.
@@ -86,28 +78,26 @@
 
 * Actual output lines containing unprintable characters are escaped
   and suffixed with a space and the keyword ``(esc)``. Lines matching
   unprintable output must also contain the keyword.
 
 * Anything else is a comment.
 
-.. _Prysk's own test suite: https://github.com/Nicoretti/prysk/blob/master/test/integration/prysk/usage.t
+.. _Prysk's own test suite: https://github.com/nicoretti/prysk/blob/master/tests/usage.t
 .. _Perl-compatible regular expressions: https://en.wikipedia.org/wiki/Perl_Compatible_Regular_Expressions
 
 Usage
 -----
 
 Prysk will print a dot for each passing test. If a test fails, a
 `unified context diff`_ is printed showing the test's expected output
 and the actual output. Skipped tests (empty tests and tests that exit
 with return code ``80``) are marked with ``s`` instead of a dot.
 
-For example, if we run Prysk on `its own example tests`_:
-
-.. code-block:: diff
+For example, if we run Prysk on `its own example tests`_::
 
     .s.!
     --- examples/fail.t
     +++ examples/fail.t.err
     @@ -3,21 +3,22 @@
        $ echo 1
        1
@@ -142,22 +132,32 @@
 file is automatically removed the next time the test passes.
 
 When you're first writing a test, you might just write the commands
 and run the test to see what happens. If you run Prysk with ``-i`` or
 ``--interactive``, you'll be prompted to merge the actual output back
 into the test. This makes it easy to quickly prototype new tests.
 
+You can specify a default set of options by creating a ``.prysk``
+file. For example::
+
+    [prysk]
+    verbose = True
+    indent = 4
+
 Is the same as invoking Prysk with ``--verbose`` and ``--indent=4``.
 
+To change what configuration file Prysk loads, you can set the
+``PRYSKRC`` environment variable. You can also specify command line
+options in the ``PRYSK`` environment variable.
+
 Note that the following environment variables are reset before tests
 are run:
 
 * ``TMPDIR``, ``TEMP``, and ``TMP`` are set to the test runner's
-  ``tmp`` directory. In test output, occurrences of this directory are
-  replaced by ``$TMPDIR``.
+  ``tmp`` directory.
 
 * ``LANG``, ``LC_ALL``, and ``LANGUAGE`` are set to ``C``.
 
 * ``TZ`` is set to ``GMT``.
 
 * ``COLUMNS`` is set to ``80``. (Note: When using ``--shell=zsh``,
   this cannot be reset. It will reflect the actual terminal's width.)
```

### Comparing `prysk-0.14.0/contrib/cram.vim` & `prysk-0.9/contrib/cram.vim`

 * *Files identical despite different names*

### Comparing `prysk-0.14.0/docs/conf.py` & `prysk-0.9/docs/conf.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,70 +6,71 @@
 
 # -- Path setup --------------------------------------------------------------
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
-import sys
-from pathlib import Path
+# import os
+# import sys
+# sys.path.insert(0, os.path.abspath('.'))
 
-CURRENT_DIR = Path(__file__).parent.resolve()
-sys.path.insert(0, f"{CURRENT_DIR.parent}")
 
 # -- Project information -----------------------------------------------------
 
-project = "prysk"
-author = "Brodie Rao, Nicola Coretti & Contributors"
+project = 'prysk'
+author = 'Brodie Rao, Nicola Coretti & Contributors'
 copyright = author
-release = ""
 # The full version, including alpha/beta/rc tags
+release = '0.9.0'
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
-extensions = ["sphinx_copybutton", "sphinx_multiversion"]
-
-# configure multiverse whitelist
-smv_tag_whitelist = r"^.*$"  # Include all tags
-smv_branch_whitelist = r"master"  # Include master
+extensions = [
+    'sphinx_rtd_theme'
+]
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ["_templates"]
+templates_path = ['_templates']
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
-exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
+exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = "furo"
-html_title = f"Prysk {release}"
+html_theme = 'sphinx_rtd_theme'
+
 html_context = {
     "display_github": True,
     "github_user": "Nicoretti",
     "github_repo": project,
     "github_version": "master",
     "conf_py_path": "/docs/",
-    "source_suffix": "rst",
+    "source_suffix": 'rst',
 }
-html_sidebars = {
-    "**": [
-        "sidebar/scroll-start.html",
-        "sidebar/brand.html",
-        "sidebar/search.html",
-        "sidebar/navigation.html",
-        "versions.html",
-        "sidebar/scroll-end.html",
-    ]
+
+html_theme_options = {
+    'logo_only': False,
+    'display_version': True,
+    'prev_next_buttons_location': 'bottom',
+    'style_external_links': False,
+    'vcs_pageview_mode': '',
+    # Toc options
+    'collapse_navigation': True,
+    'sticky_navigation': True,
+    'navigation_depth': 4,
+    'includehidden': True,
+    'titles_only': False,
 }
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ["_static"]
+html_static_path = ['_static']
```

### Comparing `prysk-0.14.0/docs/news.rst` & `prysk-0.9/docs/news.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,31 @@
 ======
  News
 ======
 
 Prysk
 +++++
+Version 0.9 (Jan. 29, 2022)
+---------------------------
+* Add basic documentation
+* Release new version to account and cope with accidentally
+  deleted (untagged prysk version 0.8)
+
+    .. note::
+        once a version is published on pipy it can't be
+        reused even if it has been deleted
+        (see `file name reuse <https://pypi.org/help/#file-name-reuse>`_).
+
+Version 0.8 (Jan. 25, 2022)
+---------------------------
+* Rename cram to prysk
 
-.. include:: prysk_news.rst
+    .. warning::
+        Also semantically relevant names have been renamed,
+        e.g. env var CRAMTMP is now PRYSK_TMP
 
 Cram
 ++++
 Version 0.7 (Feb. 24, 2016)
 ---------------------------
 
 * Added the ``-d``/``--debug`` flag that disables diffing of
```

### Comparing `prysk-0.14.0/examples/test.t` & `prysk-0.9/examples/test.t`

 * *Files 4% similar despite different names*

```diff
@@ -67,18 +67,13 @@
   $ echo hi
   \x68\x69 (esc)
   $ echo '(esc) in output (esc)'
   (esc) in output (esc)
   $ echo '(esc) in output (esc)'
   (esc) in output \x28esc\x29 (esc)
 
-Temporary directory:
-
-  $ echo "The temporary directory: $TMPDIR"
-  The temporary directory: $TMPDIR
-
 Command that closes a pipe:
 
   $ cat /dev/urandom | head -1 > /dev/null
 
 If Cram let Python's SIGPIPE handler get inherited by this script, we
 might see broken pipe messages.
```

### Comparing `prysk-0.14.0/prysk/diff.py` & `prysk-0.9/prysk/_diff.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,90 +1,90 @@
 """Utilities for diffing test files and their output"""
 
 import codecs
 import difflib
 import re
 
-__all__ = ["esc", "glob", "regex", "unified_diff"]
+__all__ = ['esc', 'glob', 'regex', 'unified_diff']
 
 
 def _regex(pattern, s):
     """Match a regular expression or return False if invalid.
 
     >>> [bool(_regex(r, b'foobar')) for r in (b'foo.*', b'***')]
     [True, False]
     """
     try:
-        return re.match(pattern + rb"\Z", s)
+        return re.match(pattern + br'\Z', s)
     except re.error:
         return False
 
 
 def _glob(el, l):
     r"""Match a glob-like pattern.
 
     The only supported special characters are * and ?. Escaping is
     supported.
 
     >>> bool(_glob(br'\* \\ \? fo?b*', b'* \\ ? foobar'))
     True
     """
     i, n = 0, len(el)
-    res = b""
+    res = b''
     while i < n:
-        c = el[i : i + 1]
+        c = el[i:i + 1]
         i += 1
-        if c == b"\\" and el[i] in b"*?\\":
-            res += el[i - 1 : i + 1]
+        if c == b'\\' and el[i] in b'*?\\':
+            res += el[i - 1:i + 1]
             i += 1
-        elif c == b"*":
-            res += b".*"
-        elif c == b"?":
-            res += b"."
+        elif c == b'*':
+            res += b'.*'
+        elif c == b'?':
+            res += b'.'
         else:
             res += re.escape(c)
     return _regex(res, l)
 
 
 def _matchannotation(keyword, matchfunc, el, l):
     """Apply match function based on annotation keyword"""
-    ann = b" (%s)\n" % keyword
-    return el.endswith(ann) and matchfunc(el[: -len(ann)], l[:-1])
+    ann = b' (%s)\n' % keyword
+    return el.endswith(ann) and matchfunc(el[:-len(ann)], l[:-1])
 
 
 def regex(el, l):
     """Apply a regular expression match to a line annotated with '(re)'"""
-    return _matchannotation(b"re", _regex, el, l)
+    return _matchannotation(b're', _regex, el, l)
 
 
 def glob(el, l):
     """Apply a glob match to a line annotated with '(glob)'"""
-    return _matchannotation(b"glob", _glob, el, l)
+    return _matchannotation(b'glob', _glob, el, l)
 
 
 def esc(el, l):
     """Apply an escape match to a line annotated with '(esc)'"""
-    ann = b" (esc)\n"
+    ann = b' (esc)\n'
 
     if el.endswith(ann):
-        el = codecs.escape_decode(el[: -len(ann)])[0] + b"\n"
+        el = codecs.escape_decode(el[:-len(ann)])[0] + b'\n'
     if el == l:
         return True
 
     if l.endswith(ann):
-        l = codecs.escape_decode(l[: -len(ann)])[0] + b"\n"
+        l = codecs.escape_decode(l[:-len(ann)])[0] + b'\n'
     return el == l
 
 
-class _SequenceMatcher(difflib.SequenceMatcher):
+class _SequenceMatcher(difflib.SequenceMatcher, object):
     """Like difflib.SequenceMatcher, but supports custom match functions"""
 
     def __init__(self, *args, **kwargs):
-        self._matchers = kwargs.pop("matchers", [])
-        super().__init__(*args, **kwargs)
+        self._matchers = kwargs.pop('matchers', [])
+        super(_SequenceMatcher, self).__init__(*args, **kwargs)
 
     def _match(self, el, l):
         """Tests for matching lines using custom matchers"""
         for matcher in self._matchers:
             if matcher(el, l):
                 return True
         return False
@@ -98,72 +98,65 @@
         for n, (el, line) in enumerate(zip(self.a[alo:ahi], self.b[blo:bhi])):
             if el != line and self._match(el, line):
                 # This fools the superclass's method into thinking that the
                 # regex/glob in a is identical to b by replacing a's line (the
                 # expected output) with b's line (the actual output).
                 self.a[alo + n] = line
                 matches.append((n, el))
-        ret = super().find_longest_match(alo, ahi, blo, bhi)
+        ret = super(_SequenceMatcher, self).find_longest_match(alo, ahi,
+                                                               blo, bhi)
         # Restore the lines replaced above. Otherwise, the diff output
         # would seem to imply that the tests never had any regexes/globs.
         for n, el in matches:
             self.a[alo + n] = el
         return ret
 
 
-def unified_diff(
-    l1,
-    l2,
-    fromfile=b"",
-    tofile=b"",
-    fromfiledate=b"",
-    tofiledate=b"",
-    n=3,
-    lineterm=b"\n",
-    matchers=None,
-):
+def unified_diff(l1, l2, fromfile=b'', tofile=b'', fromfiledate=b'',
+                 tofiledate=b'', n=3, lineterm=b'\n', matchers=None):
     r"""Compare two sequences of lines; generate the delta as a unified diff.
 
     This is like difflib.unified_diff(), but allows custom matchers.
 
     >>> l1 = [b'a\n', b'? (glob)\n']
     >>> l2 = [b'a\n', b'b\n']
     >>> (list(unified_diff(l1, l2, b'f1', b'f2', b'1970-01-01',
     ...                    b'1970-01-02')) ==
     ...  [b'--- f1\t1970-01-01\n', b'+++ f2\t1970-01-02\n',
     ...   b'@@ -1,2 +1,2 @@\n', b' a\n', b'-? (glob)\n', b'+b\n'])
     True
 
-    >>> from prysk.diff import glob
+    >>> from prysk._diff import glob
     >>> list(unified_diff(l1, l2, matchers=[glob]))
     []
     """
     if matchers is None:
         matchers = []
     started = False
     matcher = _SequenceMatcher(None, l1, l2, matchers=matchers)
     for group in matcher.get_grouped_opcodes(n):
         if not started:
             if fromfiledate:
-                fromdate = b"\t" + fromfiledate
+                fromdate = b'\t' + fromfiledate
             else:
-                fromdate = b""
+                fromdate = b''
             if tofiledate:
-                todate = b"\t" + tofiledate
+                todate = b'\t' + tofiledate
             else:
-                todate = b""
-            yield b"--- " + fromfile + fromdate + lineterm
-            yield b"+++ " + tofile + todate + lineterm
+                todate = b''
+            yield b'--- ' + fromfile + fromdate + lineterm
+            yield b'+++ ' + tofile + todate + lineterm
             started = True
         i1, i2, j1, j2 = group[0][1], group[-1][2], group[0][3], group[-1][4]
-        yield b"@@ -%d,%d +%d,%d @@" % (i1 + 1, i2 - i1, j1 + 1, j2 - j1) + lineterm
+        yield (b'@@ -%d,%d +%d,%d @@' % (i1 + 1, i2 - i1, j1 + 1, j2 - j1) +
+               lineterm)
         for tag, i1, i2, j1, j2 in group:
-            if tag == "equal":
+            if tag == 'equal':
                 for line in l1[i1:i2]:
-                    yield b" " + line
+                    yield b' ' + line
                 continue
-            if tag in ("replace", "delete"):
+            if tag == 'replace' or tag == 'delete':
                 for line in l1[i1:i2]:
-                    yield b"-" + line
-            if tag in ("replace", "insert"):
+                    yield b'-' + line
+            if tag == 'replace' or tag == 'insert':
                 for line in l2[j1:j2]:
-                    yield b"+" + line
+                    yield b'+' + line
```

### Comparing `prysk-0.14.0/prysk/process.py` & `prysk-0.9/prysk/_process.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 """Utilities for running subprocesses"""
 
 import os
 import signal
 import subprocess
 import sys
 
-__all__ = ["PIPE", "STDOUT", "execute"]
+__all__ = ['PIPE', 'STDOUT', 'execute']
 
 PIPE = subprocess.PIPE
 STDOUT = subprocess.STDOUT
 
 
 def _makeresetsigpipe():
     """Make a function to reset SIGPIPE to SIG_DFL (for use in subprocesses).
 
     Doing subprocess.Popen(..., preexec_fn=makeresetsigpipe()) will prevent
     Python's SIGPIPE handler (SIG_IGN) from being inherited by the
     child process.
     """
-    if sys.platform == "win32" or getattr(signal, "SIGPIPE", None) is None:
+    if (sys.platform == 'win32' or
+            getattr(signal, 'SIGPIPE', None) is None):
         return None
     return lambda: signal.signal(signal.SIGPIPE, signal.SIG_DFL)
 
 
 def execute(args, stdin=None, stdout=None, stderr=None, cwd=None, env=None):
     """Run a process and return its output and return code.
 
@@ -38,23 +39,16 @@
     cwd sets the process's current working directory.
 
     env can be set to a dictionary to override the process's environment
     variables.
 
     This function returns a 2-tuple of (output, returncode).
     """
-    if sys.platform == "win32":
+    if sys.platform == 'win32':
         args = [os.fsdecode(arg) for arg in args]
 
-    process = subprocess.Popen(
-        args,
-        stdin=PIPE,
-        stdout=stdout,
-        stderr=stderr,
-        cwd=cwd,
-        env=env,
-        bufsize=-1,
-        preexec_fn=_makeresetsigpipe(),
-        close_fds=os.name == "posix",
-    )
-    out, _err = process.communicate(stdin)
-    return out, process.returncode
+    p = subprocess.Popen(args, stdin=PIPE, stdout=stdout, stderr=stderr,
+                         cwd=cwd, env=env, bufsize=-1,
+                         preexec_fn=_makeresetsigpipe(),
+                         close_fds=os.name == 'posix')
+    out, err = p.communicate(stdin)
+    return out, p.returncode
```

### Comparing `prysk-0.14.0/prysk/test.py` & `prysk-0.9/prysk/_test.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,105 +1,33 @@
 """Utilities for running individual tests"""
 
 import itertools
 import os
 import re
 import time
-from contextlib import contextmanager
-from pathlib import Path
 
-from prysk.diff import (
-    esc,
-    glob,
-    regex,
-    unified_diff,
-)
-from prysk.process import (
-    PIPE,
-    STDOUT,
-    execute,
-)
-
-__all__ = ["test", "testfile", "runtests"]
-
-_SKIP = 80
-_IS_ESCAPING_NEEDED = re.compile(rb"[\x00-\x09\x0b-\x1f\x7f-\xff]").search
-
-
-def is_hidden(path):
-    """Check if a path (file/dir) is hidden or not."""
-
-    def _is_hidden(part):
-        return (
-            part.startswith(".")
-            and not part == "."
-            and not part.startswith("..")
-            and not part.startswith("./")
-        )
-
-    return any(map(_is_hidden, path.parts))
-
-
-def is_testfile(path):
-    """Check if path is a valid prysk test file"""
-    return path.is_file() and path.suffix == ".t" and not is_hidden(path)
+from prysk._diff import esc, glob, regex, unified_diff
+from prysk._process import PIPE, STDOUT, execute
+
+__all__ = ['test', 'testfile']
+
+_needescape = re.compile(br'[\x00-\x09\x0b-\x1f\x7f-\xff]').search
+_escapesub = re.compile(br'[\x00-\x09\x0b-\x1f\\\x7f-\xff]').sub
+_escapemap = dict((bytes([i]), br'\x%02x' % i) for i in range(256))
+_escapemap.update({b'\\': b'\\\\', b'\r': br'\r', b'\t': br'\t'})
 
 
 def _escape(s):
     """Like the string-escape codec, but doesn't escape quotes"""
-    escape_sub = re.compile(rb"[\x00-\x09\x0b-\x1f\\\x7f-\xff]").sub
-    escape_map = dict((bytes([i]), rb"\x%02x" % i) for i in range(256))
-    escape_map.update({b"\\": b"\\\\", b"\r": rb"\r", b"\t": rb"\t"})
-    return escape_sub(lambda m: escape_map[m.group(0)], s[:-1]) + b" (esc)\n"
-
-
-def _findtests(paths):
-    """Yield tests in paths in sorted order"""
-
-    paths = list(map(Path, paths))
-
-    def is_test_dir(path):
-        """Check if the path is a valid prysk test dir"""
-        return path.is_dir() and not is_hidden(path)
-
-    def remove_duplicates(path):
-        """Stable duplication removal"""
-        return list(dict.fromkeys(path))
-
-    def collect(paths):
-        """Collect all test files compliant with cram collection order"""
-        for path in paths:
-            if is_testfile(path):
-                yield path
-            if is_test_dir(path):
-                yield from sorted((f for f in path.rglob("*.t") if is_testfile(f)))
-
-    yield from remove_duplicates(collect(paths))
-
-
-@contextmanager
-def cwd(path):
-    """Change the current working directory and restore it afterwards."""
-    _cwd = os.getcwd()
-    os.chdir(path)
-    try:
-        yield path
-    finally:
-        os.chdir(_cwd)
-
-
-def test(
-    lines,
-    shell="/bin/sh",
-    indent=2,
-    testname=None,
-    env=None,
-    cleanenv=True,
-    debug=False,
-):
+    return (_escapesub(lambda m: _escapemap[m.group(0)], s[:-1]) +
+            b' (esc)\n')
+
+
+def test(lines, shell='/bin/sh', indent=2, testname=None, env=None,
+         cleanenv=True, debug=False):
     r"""Run test lines and return input, output, and diff.
 
     This returns a 3-tuple containing the following:
 
         (list of lines in test, same list with actual output, diff)
 
     diff is a generator that yields the diff between the two lists.
@@ -149,125 +77,111 @@
     :param cleanenv: Whether or not to sanitize the environment
     :type cleanenv: bool
     :param debug: Whether or not to run in debug mode (don't capture stdout)
     :type debug: bool
     return: Input, output, and diff iterables
     :rtype: (list[bytes], list[bytes], collections.Iterable[bytes])
     """
-    indent = b" " * indent
-    cmdline = indent + b"$ "
-    conline = indent + b"> "
-    salt = b"PRYSK%.5f" % time.time()
+    indent = b' ' * indent
+    cmdline = indent + b'$ '
+    conline = indent + b'> '
+    salt = b'CRAM%.5f' % time.time()
 
     def create_environment(environment, shell, clean=False):
         _env = os.environ.copy() if environment is None else environment
-        _env["TESTSHELL"] = shell
+        _env['TESTSHELL'] = shell
         if clean:
-            _env.update({key: "C" for key in ["LANG", "LC_ALL", "LANGUAGE"]})
-            _env["TZ"] = "GMT"
-            _env["CDPATH"] = ""
-            _env["COLUMNS"] = "80"
-            _env["GREP_OPTIONS"] = ""
+            _env.update({key: 'C' for key in ['LANG', 'LC_ALL', 'LANGUAGE']})
+            _env['TZ'] = 'GMT'
+            _env['CDPATH'] = ''
+            _env['COLUMNS'] = '80'
+            _env['GREP_OPTIONS'] = ''
         return _env
 
     lines = lines.splitlines(True) if isinstance(lines, bytes) else lines
     shell = [shell] if isinstance(shell, (bytes, str)) else shell
     env = create_environment(env, shell[0], clean=cleanenv)
 
     if debug:
-        return _debug(cmdline, conline, env, lines, shell)
+        stdin = []
+        for line in lines:
+            if not line.endswith(b'\n'):
+                line += b'\n'
+            if line.startswith(cmdline):
+                stdin.append(line[len(cmdline):])
+            elif line.startswith(conline):
+                stdin.append(line[len(conline):])
+
+        execute(shell + ['-'], stdin=b''.join(stdin), env=env)
+        return ([], [], [])
 
     after = {}
     refout, postout = [], []
     i = pos = prepos = -1
     stdin = []
     for i, line in enumerate(lines):
-        if not line.endswith(b"\n"):
-            line += b"\n"
+        if not line.endswith(b'\n'):
+            line += b'\n'
         refout.append(line)
         if line.startswith(cmdline):
             after.setdefault(pos, []).append(line)
             prepos = pos
             pos = i
-            stdin.append(b"echo %s %d $?\n" % (salt, i))
-            stdin.append(line[len(cmdline) :])
+            stdin.append(b'echo %s %d $?\n' % (salt, i))
+            stdin.append(line[len(cmdline):])
         elif line.startswith(conline):
             after.setdefault(prepos, []).append(line)
-            stdin.append(line[len(conline) :])
+            stdin.append(line[len(conline):])
         elif not line.startswith(indent):
             after.setdefault(pos, []).append(line)
-    stdin.append(b"echo %s %d $?\n" % (salt, i + 1))
+    stdin.append(b'echo %s %d $?\n' % (salt, i + 1))
 
-    output, retcode = execute(
-        shell + ["-"], stdin=b"".join(stdin), stdout=PIPE, stderr=STDOUT, env=env
-    )
-    if retcode == _SKIP:
-        return refout, None, []
+    output, retcode = execute(shell + ['-'], stdin=b''.join(stdin),
+                              stdout=PIPE, stderr=STDOUT, env=env)
+    if retcode == 80:
+        return (refout, None, [])
 
     pos = -1
+    ret = 0
     for i, line in enumerate(output[:-1].splitlines(True)):
         out, cmd = line, None
         if salt in line:
             out, cmd = line.split(salt, 1)
 
         if out:
-            if not out.endswith(b"\n"):
-                out += b" (no-eol)\n"
+            if not out.endswith(b'\n'):
+                out += b' (no-eol)\n'
 
-            if _IS_ESCAPING_NEEDED(out):
+            if _needescape(out):
                 out = _escape(out)
-
-            try:
-                tmpdir = os.environb[b"TMPDIR"]
-            except KeyError:
-                pass
-            else:
-                out = re.sub(re.escape(tmpdir), b"$TMPDIR", out)
-
             postout.append(indent + out)
 
         if cmd:
             ret = int(cmd.split()[1])
             if ret != 0:
-                postout.append(indent + b"[%d]\n" % ret)
+                postout.append(indent + b'[%d]\n' % ret)
             postout += after.pop(pos, [])
             pos = int(cmd.split()[0])
 
     postout += after.pop(pos, [])
 
     if testname:
-        diff_path = bytes(testname)
-        error_path = bytes(Path(testname.parent, f"{testname.name}.err"))
+        diffpath = testname
+        errpath = diffpath + b'.err'
     else:
-        diff_path = error_path = b""
-
-    diff = unified_diff(
-        refout, postout, diff_path, error_path, matchers=[esc, glob, regex]
-    )
-    for line in diff:
-        return refout, postout, itertools.chain([line], diff)
+        diffpath = errpath = b''
+    diff = unified_diff(refout, postout, diffpath, errpath,
+                        matchers=[esc, glob, regex])
+    for firstline in diff:
+        return refout, postout, itertools.chain([firstline], diff)
     return refout, postout, []
 
 
-def _debug(cmdline, conline, env, lines, shell):
-    stdin = []
-    for line in lines:
-        if not line.endswith(b"\n"):
-            line += b"\n"
-        if line.startswith(cmdline):
-            stdin.append(line[len(cmdline) :])
-        elif line.startswith(conline):
-            stdin.append(line[len(conline) :])
-    execute(shell + ["-"], stdin=b"".join(stdin), env=env)
-    return [], [], []
-
-
-def testfile(
-    path, shell="/bin/sh", indent=2, env=None, cleanenv=True, debug=False, testname=None
-):
+def testfile(path, shell='/bin/sh', indent=2, env=None, cleanenv=True,
+             debug=False, testname=None):
     """Run test at path and return input, output, and diff.
 
     This returns a 3-tuple containing the following:
 
         (list of lines in test, same list with actual output, diff)
 
     diff is a generator that yields the diff between the two lists.
@@ -291,70 +205,16 @@
     :param debug: Whether or not to run in debug mode (don't capture stdout)
     :type debug: bool
     :param testname: Optional test file name (used in diff output)
     :type testname: bytes or None
     :return: Input, output, and diff iterables
     :rtype: (list[bytes], list[bytes], collections.Iterable[bytes])
     """
-    with open(path, "rb") as f:
-        abspath = path.resolve()
+    with open(path, 'rb') as f:
+        abspath = os.path.abspath(path)
         env = env or os.environ.copy()
-        env["TESTDIR"] = f"{abspath.parent}"
-        env["TESTFILE"] = f"{abspath.name}"
+        env['TESTDIR'] = os.fsdecode(os.path.dirname(abspath))
+        env['TESTFILE'] = os.fsdecode(os.path.basename(abspath))
         if testname is None:
-            testname = path
-        return test(
-            f,
-            shell,
-            indent=indent,
-            testname=testname,
-            env=env,
-            cleanenv=cleanenv,
-            debug=debug,
-        )
-
-
-def runtests(paths, tmpdir, shell, indent=2, cleanenv=True, debug=False):
-    """Run tests and yield results.
-
-    This yields a sequence of 2-tuples containing the following:
-
-        (test path, test function)
-
-    The test function, when called, runs the test in a temporary directory
-    and returns a 3-tuple:
-
-        (list of lines in the test, same list with actual output, diff)
-    """
-    basenames, seen = set(), set()
-    tests = _findtests(paths)
-    for i, path in enumerate(tests):
-        abspath = path.resolve()
-        if abspath in seen:
-            continue
-        seen.add(abspath)
-
-        if not path.stat().st_size:
-            yield path, lambda: (None, None, None)
-            continue
-
-        basename = path.name
-        if basename in basenames:
-            basename = f"{basename}-{i}"
-        else:
-            basenames.add(basename)
-
-        def test():
-            """Run test file"""
-            testdir = tmpdir / basename
-            os.mkdir(testdir)
-            with cwd(testdir):
-                return testfile(
-                    abspath,
-                    shell,
-                    indent=indent,
-                    cleanenv=cleanenv,
-                    debug=debug,
-                    testname=path,
-                )
-
-        yield path, test
+            testname = os.path.basename(abspath)
+        return test(f, shell, indent=indent, testname=testname, env=env,
+                    cleanenv=cleanenv, debug=debug)
```

### Comparing `prysk-0.14.0/prysk/xunit.py` & `prysk-0.9/prysk/_xunit.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,93 +1,88 @@
 """xUnit XML output"""
 
 import locale
+import os
 import re
 import socket
 import sys
 import time
-from inspect import cleandoc
 
-__all__ = ["runxunit"]
+__all__ = ['runxunit']
 
-_WIDE_CDATA_REGEX = (
-    r"(?:[^\x09\x0a\x0d\x20-\ud7ff\ue000-\ufffd" r"\U00010000-\U0010ffff]|]]>)"
-)
-_NARROW_CDATA_REGEX = r"(?:[^\x09\x0a\x0d\x20-\ud7ff\ue000-\ufffd]" r"|]]>)"
-_WIDE_QUOTE_ATTR_REGEX = (
-    r"[^\x20\x21\x23-\x25\x27-\x3b\x3d"
-    r"\x3f-\ud7ff\ue000-\ufffd"
-    r"\U00010000-\U0010ffff]"
-)
-_NARROW_QUOTE_ATTR_REGEX = (
-    r"[^\x20\x21\x23-\x25\x27-\x3b\x3d" r"\x3f-\ud7ff\ue000-\ufffd]"
-)
-_REPLACEMENT_CHAR = "\N{REPLACEMENT CHARACTER}"
-
-if sys.maxunicode >= 0x10FFFF:
-    _CDATASUB = re.compile(_WIDE_CDATA_REGEX).sub
-    _QUOTEATTRSUB = re.compile(_WIDE_QUOTE_ATTR_REGEX).sub
+_widecdataregex = (r'(?:[^\x09\x0a\x0d\x20-\ud7ff\ue000-\ufffd'
+                   r'\U00010000-\U0010ffff]|]]>)')
+_narrowcdataregex = (r'(?:[^\x09\x0a\x0d\x20-\ud7ff\ue000-\ufffd]'
+                     r'|]]>)')
+_widequoteattrregex = (r'[^\x20\x21\x23-\x25\x27-\x3b\x3d'
+                       r'\x3f-\ud7ff\ue000-\ufffd'
+                       r'\U00010000-\U0010ffff]')
+_narrowquoteattrregex = (r'[^\x20\x21\x23-\x25\x27-\x3b\x3d'
+                         r'\x3f-\ud7ff\ue000-\ufffd]')
+_replacementchar = '\N{REPLACEMENT CHARACTER}'
+
+if sys.maxunicode >= 0x10ffff:
+    _cdatasub = re.compile(_widecdataregex).sub
+    _quoteattrsub = re.compile(_widequoteattrregex).sub
 else:
-    _CDATASUB = re.compile(_NARROW_CDATA_REGEX).sub
-    _QUOTEATTRSUB = re.compile(_NARROW_QUOTE_ATTR_REGEX).sub
+    _cdatasub = re.compile(_narrowcdataregex).sub
+    _quoteattrsub = re.compile(_narrowquoteattrregex).sub
 
 
 def _cdatareplace(m):
-    """Replace _CDATASUB() regex match"""
-    if m.group(0) == "]]>":
-        return "]]>]]&gt;<![CDATA["
+    """Replace _cdatasub() regex match"""
+    if m.group(0) == ']]>':
+        return ']]>]]&gt;<![CDATA['
     else:
-        return _REPLACEMENT_CHAR
+        return _replacementchar
 
 
 def _cdata(s):
     r"""Escape a string as an XML CDATA block.
 
     >>> (_cdata('1<\'2\'>&"3\x00]]>\t\r\n') ==
     ...  '<![CDATA[1<\'2\'>&\"3\ufffd]]>]]&gt;<![CDATA[\t\r\n]]>')
     True
     """
-    return f"<![CDATA[{_CDATASUB(_cdatareplace, s)}]]>"
+    return '<![CDATA[%s]]>' % _cdatasub(_cdatareplace, s)
 
 
 def _quoteattrreplace(m):
-    """Replace _QUOTEATTRSUB() regex match"""
-    return {
-        "\t": "&#9;",
-        "\n": "&#10;",
-        "\r": "&#13;",
-        '"': "&quot;",
-        "&": "&amp;",
-        "<": "&lt;",
-        ">": "&gt;",
-    }.get(m.group(0), _REPLACEMENT_CHAR)
+    """Replace _quoteattrsub() regex match"""
+    return {'\t': '&#9;',
+            '\n': '&#10;',
+            '\r': '&#13;',
+            '"': '&quot;',
+            '&': '&amp;',
+            '<': '&lt;',
+            '>': '&gt;'}.get(m.group(0), _replacementchar)
 
 
 def _quoteattr(s):
     r"""Escape a string for use as an XML attribute value.
 
     >>> (_quoteattr('1<\'2\'>&"3\x00]]>\t\r\n') ==
     ...  '"1&lt;\'2\'&gt;&amp;&quot;3\ufffd]]&gt;&#9;&#13;&#10;"')
     True
     """
-    return f'"{_QUOTEATTRSUB(_quoteattrreplace, s)}"'
+    return '"%s"' % _quoteattrsub(_quoteattrreplace, s)
 
 
 def _timestamp():
     """Return the current time in ISO 8601 format"""
     tm = time.localtime()
     if tm.tm_isdst == 1:
         tz = time.altzone
     else:
         tz = time.timezone
 
-    timestamp = time.strftime("%Y-%m-%dT%H:%M:%S", tm)
-    hours = int(-tz / 60 / 60)
-    minutes = int(abs(tz) / 60 % 60)
-    timestamp += "%+03d:%02d" % (hours, minutes)
+    timestamp = time.strftime('%Y-%m-%dT%H:%M:%S', tm)
+    tzhours = int(-tz / 60 / 60)
+    tzmins = int(abs(tz) / 60 % 60)
+    timestamp += '%+03d:%02d' % (tzhours, tzmins)
     return timestamp
 
 
 def runxunit(tests, xmlpath):
     """Run tests with xUnit XML output.
 
     tests should be a sequence of 2-tuples containing the following:
@@ -100,82 +95,81 @@
     suitestart = time.time()
     timestamp = _timestamp()
     hostname = socket.gethostname()
     total, skipped, failed = [0], [0], [0]
     testcases = []
 
     for path, test in tests:
-
         def testwrapper():
             """Run test and collect XML output"""
             total[0] += 1
 
             start = time.time()
             refout, postout, diff = test()
             testtime = time.time() - start
 
-            classname = f"{path}"
-            name = path.name
+            classname = path.decode(locale.getpreferredencoding(), 'replace')
+            name = os.path.basename(classname)
 
             if postout is None:
                 skipped[0] += 1
-                testcase = "\n".join(
-                    [
-                        f"  <testcase classname={_quoteattr(classname)}",
-                        f"            name={_quoteattr(name)}",
-                        f'            time="{testtime:6f}">',
-                        "    <skipped/>",
-                        "  </testcase>",
-                        "",
-                    ]
-                )
+                testcase = (('  <testcase classname=%(classname)s\n'
+                             '            name=%(name)s\n'
+                             '            time="%(time).6f">\n'
+                             '    <skipped/>\n'
+                             '  </testcase>\n') %
+                            {'classname': _quoteattr(classname),
+                             'name': _quoteattr(name),
+                             'time': testtime})
             elif diff:
                 failed[0] += 1
                 diff = list(diff)
-                diffu = "".join(
-                    l.decode(locale.getpreferredencoding(), "replace") for l in diff
-                )
-                testcase = "\n".join(
-                    [
-                        f"  <testcase classname={_quoteattr(classname)}",
-                        f"            name={_quoteattr(name)}",
-                        f'            time="{testtime:6f}">',
-                        f"    <failure>{_cdata(diffu)}</failure>",
-                        "  </testcase>",
-                        "",
-                    ]
-                )
+                diffu = ''.join(l.decode(locale.getpreferredencoding(),
+                                         'replace')
+                                for l in diff)
+                testcase = (('  <testcase classname=%(classname)s\n'
+                             '            name=%(name)s\n'
+                             '            time="%(time).6f">\n'
+                             '    <failure>%(diff)s</failure>\n'
+                             '  </testcase>\n') %
+                            {'classname': _quoteattr(classname),
+                             'name': _quoteattr(name),
+                             'time': testtime,
+                             'diff': _cdata(diffu)})
             else:
-                testcase = "\n".join(
-                    [
-                        f"  <testcase classname={_quoteattr(classname)}",
-                        f"            name={_quoteattr(name)}",
-                        f'            time="{testtime:6f}"/>',
-                        "",
-                    ]
-                )
-
+                testcase = (('  <testcase classname=%(classname)s\n'
+                             '            name=%(name)s\n'
+                             '            time="%(time).6f"/>\n') %
+                            {'classname': _quoteattr(classname),
+                             'name': _quoteattr(name),
+                             'time': testtime})
             testcases.append(testcase)
+
             return refout, postout, diff
 
         yield path, testwrapper
 
     suitetime = time.time() - suitestart
-    # fmt: off
-    header = cleandoc(f"""
-         <?xml version="1.0" encoding="utf-8"?>
-         <testsuite name="prysk"
-                    tests="{total[0]}"
-                    failures="{failed[0]}"
-                    skipped="{skipped[0]}"
-                    timestamp={_quoteattr(timestamp)}
-                    hostname={_quoteattr(hostname)}
-                    time="{suitetime:6f}">
-    """) + "\n"
-    # fmt: on
-    footer = "</testsuite>\n"
-
-    with open(xmlpath, "wb") as xmlfile:
-        encoding = "utf-8"
-        xmlfile.write(header.encode(encoding))
-        [xmlfile.write(testcase.encode(encoding)) for testcase in testcases]
-        xmlfile.write(footer.encode(encoding))
+    header = (('<?xml version="1.0" encoding="utf-8"?>\n'
+               '<testsuite name="prysk"\n'
+               '           tests="%(total)d"\n'
+               '           failures="%(failed)d"\n'
+               '           skipped="%(skipped)d"\n'
+               '           timestamp=%(timestamp)s\n'
+               '           hostname=%(hostname)s\n'
+               '           time="%(time).6f">\n') %
+              {'total': total[0],
+               'failed': failed[0],
+               'skipped': skipped[0],
+               'timestamp': _quoteattr(timestamp),
+               'hostname': _quoteattr(hostname),
+               'time': suitetime})
+    footer = '</testsuite>\n'
+
+    xmlfile = open(xmlpath, 'wb')
+    try:
+        xmlfile.write(header.encode('utf-8'))
+        for testcase in testcases:
+            xmlfile.write(testcase.encode('utf-8'))
+        xmlfile.write(footer.encode('utf-8'))
+    finally:
+        xmlfile.close()
```

### Comparing `prysk-0.14.0/setup.py` & `prysk-0.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,206 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-packages = \
-['prysk', 'pytest_prysk']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['rich>=13.3.1,<14.0.0']
-
-extras_require = \
-{'pytest-plugin': ['pytest>=7.0.1']}
-
-entry_points = \
-{'console_scripts': ['prysk = prysk:main'],
- 'pytest11': ['prysk = pytest_prysk']}
-
-setup_kwargs = {
-    'name': 'prysk',
-    'version': '0.14.0',
-    'description': 'Functional tests for command line applications',
-    'long_description': 'Prysk\n======================\n.. image:: https://img.shields.io/github/actions/workflow/status/nicoretti/prysk/verifier.yaml\n    :target: https://github.com/Nicoretti/prysk/actions\n\n.. image:: https://img.shields.io/coverallsCoverage/github/Nicoretti/prysk\n    :target: https://coveralls.io/github/Nicoretti/prysk\n\n.. image:: https://img.shields.io/badge/imports-isort-ef8336.svg\n    :target: https://pycqa.github.io/isort/\n\n.. image:: https://img.shields.io/badge/code%20style-black-000000.svg\n   :target: https://github.com/psf/black\n\n.. image:: https://img.shields.io/pypi/v/prysk\n    :target: https://pypi.org/project/prysk/\n\n.. image:: https://img.shields.io/badge/docs-available-blue.svg\n    :target: https://nicoretti.github.io/prysk/\n\nPrysk is a fork of the popular snapshot testing tool Cram_.\nEven though Cram_ is pretty complete and mature for everyday use,\nPrysk wants to continue pushing its development forward.\n\n.. _Cram: https://bitheap.org/cram\n\nPrysk tests look like snippets of interactive shell sessions. Prysk runs\neach command and compares the command output in the test with the\ncommand\'s actual output.\n\nHere\'s a snippet from `Prysk\'s own test suite`_:\n\n.. code-block:: console\n\n    Set up prysk alias and example tests:\n\n      $ . "$TESTDIR"/setup.sh\n\n    Usage:\n\n      $ prysk -h\n      [Uu]sage: prysk \\[OPTIONS\\] TESTS\\.\\.\\. (re)\n\n      [Oo]ptions: (re)\n        -h, --help          show this help message and exit\n        -V, --version       show version information and exit\n        -q, --quiet         don\'t print diffs\n        -v, --verbose       show filenames and test status\n        -i, --interactive   interactively merge changed test output\n        -d, --debug         write script output directly to the terminal\n        -y, --yes           answer yes to all questions\n        -n, --no            answer no to all questions\n        -E, --preserve-env  don\'t reset common environment variables\n        --keep-tmpdir       keep temporary directories\n        --shell=PATH        shell to use for running tests (default: /bin/sh)\n        --shell-opts=OPTS   arguments to invoke shell with\n        --indent=NUM        number of spaces to use for indentation (default: 2)\n        --xunit-file=PATH   path to write xUnit XML output\n\nThe format in a nutshell:\n\n* Prysk tests use the ``.t`` file extension.\n\n* Lines beginning with two spaces, a dollar sign (``$``), and a space are run\n  in the shell.\n\n* Lines beginning with two spaces, a greater than sign (``>``), and a space\n  allow multi-line commands.\n\n* All other lines beginning with two spaces are considered command\n  output.\n\n* Output lines ending with a space and the keyword ``(re)`` are\n  matched as `Perl-compatible regular expressions`_.\n\n* Lines ending with a space and the keyword ``(glob)`` are matched\n  with a glob-like syntax. The only special characters supported are\n  ``*`` and ``?``. Both characters can be escaped using ``\\``, and the\n  backslash can be escaped itself.\n\n* Output lines ending with either of the above keywords are always\n  first matched literally with actual command output.\n\n* Lines ending with a space and the keyword ``(no-eol)`` will match\n  actual output that doesn\'t end in a newline.\n\n* Actual output lines containing unprintable characters are escaped\n  and suffixed with a space and the keyword ``(esc)``. Lines matching\n  unprintable output must also contain the keyword.\n\n* Anything else is a comment.\n\n.. _Prysk\'s own test suite: https://github.com/Nicoretti/prysk/blob/master/test/integration/prysk/usage.t\n.. _Perl-compatible regular expressions: https://en.wikipedia.org/wiki/Perl_Compatible_Regular_Expressions\n\nUsage\n-----\n\nPrysk will print a dot for each passing test. If a test fails, a\n`unified context diff`_ is printed showing the test\'s expected output\nand the actual output. Skipped tests (empty tests and tests that exit\nwith return code ``80``) are marked with ``s`` instead of a dot.\n\nFor example, if we run Prysk on `its own example tests`_:\n\n.. code-block:: diff\n\n    .s.!\n    --- examples/fail.t\n    +++ examples/fail.t.err\n    @@ -3,21 +3,22 @@\n       $ echo 1\n       1\n       $ echo 1\n    -  2\n    +  1\n       $ echo 1\n       1\n\n     Invalid regex:\n\n       $ echo 1\n    -  +++ (re)\n    +  1\n\n     Offset regular expression:\n\n       $ printf \'foo\\nbar\\nbaz\\n\\n1\\nA\\n@\\n\'\n       foo\n    +  bar\n       baz\n\n       \\d (re)\n       [A-Z] (re)\n    -  #\n    +  @\n    s.\n    # Ran 6 tests, 2 skipped, 1 failed.\n\nPrysk will also write the test with its actual output to\n``examples/fail.t.err``, allowing you to use other diff tools. This\nfile is automatically removed the next time the test passes.\n\nWhen you\'re first writing a test, you might just write the commands\nand run the test to see what happens. If you run Prysk with ``-i`` or\n``--interactive``, you\'ll be prompted to merge the actual output back\ninto the test. This makes it easy to quickly prototype new tests.\n\nIs the same as invoking Prysk with ``--verbose`` and ``--indent=4``.\n\nNote that the following environment variables are reset before tests\nare run:\n\n* ``TMPDIR``, ``TEMP``, and ``TMP`` are set to the test runner\'s\n  ``tmp`` directory. In test output, occurrences of this directory are\n  replaced by ``$TMPDIR``.\n\n* ``LANG``, ``LC_ALL``, and ``LANGUAGE`` are set to ``C``.\n\n* ``TZ`` is set to ``GMT``.\n\n* ``COLUMNS`` is set to ``80``. (Note: When using ``--shell=zsh``,\n  this cannot be reset. It will reflect the actual terminal\'s width.)\n\n* ``CDPATH`` and ``GREP_OPTIONS`` are set to an empty string.\n\nPrysk also provides the following environment variables to tests:\n\n* ``PRYSK_TEMP``, set to the test runner\'s temporary directory.\n\n* ``TESTDIR``, set to the directory containing the test file.\n\n* ``TESTFILE``, set to the basename of the current test file.\n\n* ``TESTSHELL``, set to the value specified by ``--shell``.\n\nAlso note that care should be taken with commands that close the test\nshell\'s ``stdin``. For example, if you\'re trying to invoke ``ssh`` in\na test, try adding the ``-n`` option to prevent it from closing\n``stdin``. Similarly, if you invoke a daemon process that inherits\n``stdout`` and fails to close it, it may cause Prysk to hang while\nwaiting for the test shell\'s ``stdout`` to be fully closed.\n\n.. _unified context diff: https://en.wikipedia.org/wiki/Diff#Unified_format\n.. _its own example tests: https://github.com/nicoretti/prysk/tree/master/examples\n',
-    'author': 'Nicola Coretti',
-    'author_email': 'nico.coretti@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://nicoretti.github.io/prysk/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0.0',
-}
-
-
-setup(**setup_kwargs)
+Metadata-Version: 1.1
+Name: prysk
+Version: 0.9
+Summary: Functional tests for command line applications
+Home-page: https://github.com/Nicoretti/prysk
+Author: Brodie Rao, Nicola Coretti
+Author-email: brodie@bitheap.org, nico.coretti@gmail.com
+License: GNU GPLv2 or any later version
+Description: Prysk
+        ======================
+        .. image:: https://github.com/Nicoretti/prysk/actions/workflows/verifier.yaml/badge.svg
+            :target: https://github.com/Nicoretti/prysk/actions/workflows/verifier.yaml
+        
+        .. image:: https://coveralls.io/repos/github/Nicoretti/prysk/badge.svg?branch=master
+            :target: https://coveralls.io/github/Nicoretti/prysk?branch=master
+        
+        .. image:: https://img.shields.io/badge/pypi%20package-available-blue.svg
+            :target: https://pypi.org/project/prysk/
+        
+        .. image:: https://img.shields.io/badge/docs-available-blue.svg
+            :target: https://nicoretti.github.io/prysk/
+        
+        Prysk is a fork of the popular snapshot testing tool Cram_.
+        Even though Cram_ is pretty complete and mature for everyday use,
+        Prysk want's to continue pushing it's development forward.
+        
+        .. _Cram: https://bitheap.org/cram
+        
+        Prysk tests look like snippets of interactive shell sessions. Prysk runs
+        each command and compares the command output in the test with the
+        command's actual output.
+        
+        Here's a snippet from `Prysk's own test suite`_::
+        
+            Set up prysk alias and example tests:
+        
+              $ . "$TESTDIR"/setup.sh
+        
+            Usage:
+        
+              $ prysk -h
+              [Uu]sage: prysk \[OPTIONS\] TESTS\.\.\. (re)
+        
+              [Oo]ptions: (re)
+                -h, --help          show this help message and exit
+                -V, --version       show version information and exit
+                -q, --quiet         don't print diffs
+                -v, --verbose       show filenames and test status
+                -i, --interactive   interactively merge changed test output
+                -d, --debug         write script output directly to the terminal
+                -y, --yes           answer yes to all questions
+                -n, --no            answer no to all questions
+                -E, --preserve-env  don't reset common environment variables
+                --keep-tmpdir       keep temporary directories
+                --shell=PATH        shell to use for running tests (default: /bin/sh)
+                --shell-opts=OPTS   arguments to invoke shell with
+                --indent=NUM        number of spaces to use for indentation (default: 2)
+                --xunit-file=PATH   path to write xUnit XML output
+        
+        The format in a nutshell:
+        
+        * Prysk tests use the ``.t`` file extension.
+        
+        * Lines beginning with two spaces, a dollar sign, and a space are run
+          in the shell.
+        
+        * Lines beginning with two spaces, a greater than sign, and a space
+          allow multi-line commands.
+        
+        * All other lines beginning with two spaces are considered command
+          output.
+        
+        * Output lines ending with a space and the keyword ``(re)`` are
+          matched as `Perl-compatible regular expressions`_.
+        
+        * Lines ending with a space and the keyword ``(glob)`` are matched
+          with a glob-like syntax. The only special characters supported are
+          ``*`` and ``?``. Both characters can be escaped using ``\``, and the
+          backslash can be escaped itself.
+        
+        * Output lines ending with either of the above keywords are always
+          first matched literally with actual command output.
+        
+        * Lines ending with a space and the keyword ``(no-eol)`` will match
+          actual output that doesn't end in a newline.
+        
+        * Actual output lines containing unprintable characters are escaped
+          and suffixed with a space and the keyword ``(esc)``. Lines matching
+          unprintable output must also contain the keyword.
+        
+        * Anything else is a comment.
+        
+        .. _Prysk's own test suite: https://github.com/nicoretti/prysk/blob/master/tests/usage.t
+        .. _Perl-compatible regular expressions: https://en.wikipedia.org/wiki/Perl_Compatible_Regular_Expressions
+        
+        Usage
+        -----
+        
+        Prysk will print a dot for each passing test. If a test fails, a
+        `unified context diff`_ is printed showing the test's expected output
+        and the actual output. Skipped tests (empty tests and tests that exit
+        with return code ``80``) are marked with ``s`` instead of a dot.
+        
+        For example, if we run Prysk on `its own example tests`_::
+        
+            .s.!
+            --- examples/fail.t
+            +++ examples/fail.t.err
+            @@ -3,21 +3,22 @@
+               $ echo 1
+               1
+               $ echo 1
+            -  2
+            +  1
+               $ echo 1
+               1
+        
+             Invalid regex:
+        
+               $ echo 1
+            -  +++ (re)
+            +  1
+        
+             Offset regular expression:
+        
+               $ printf 'foo\nbar\nbaz\n\n1\nA\n@\n'
+               foo
+            +  bar
+               baz
+        
+               \d (re)
+               [A-Z] (re)
+            -  #
+            +  @
+            s.
+            # Ran 6 tests, 2 skipped, 1 failed.
+        
+        Prysk will also write the test with its actual output to
+        ``examples/fail.t.err``, allowing you to use other diff tools. This
+        file is automatically removed the next time the test passes.
+        
+        When you're first writing a test, you might just write the commands
+        and run the test to see what happens. If you run Prysk with ``-i`` or
+        ``--interactive``, you'll be prompted to merge the actual output back
+        into the test. This makes it easy to quickly prototype new tests.
+        
+        You can specify a default set of options by creating a ``.prysk``
+        file. For example::
+        
+            [prysk]
+            verbose = True
+            indent = 4
+        
+        Is the same as invoking Prysk with ``--verbose`` and ``--indent=4``.
+        
+        To change what configuration file Prysk loads, you can set the
+        ``PRYSKRC`` environment variable. You can also specify command line
+        options in the ``PRYSK`` environment variable.
+        
+        Note that the following environment variables are reset before tests
+        are run:
+        
+        * ``TMPDIR``, ``TEMP``, and ``TMP`` are set to the test runner's
+          ``tmp`` directory.
+        
+        * ``LANG``, ``LC_ALL``, and ``LANGUAGE`` are set to ``C``.
+        
+        * ``TZ`` is set to ``GMT``.
+        
+        * ``COLUMNS`` is set to ``80``. (Note: When using ``--shell=zsh``,
+          this cannot be reset. It will reflect the actual terminal's width.)
+        
+        * ``CDPATH`` and ``GREP_OPTIONS`` are set to an empty string.
+        
+        Prysk also provides the following environment variables to tests:
+        
+        * ``PRYSK_TEMP``, set to the test runner's temporary directory.
+        
+        * ``TESTDIR``, set to the directory containing the test file.
+        
+        * ``TESTFILE``, set to the basename of the current test file.
+        
+        * ``TESTSHELL``, set to the value specified by ``--shell``.
+        
+        Also note that care should be taken with commands that close the test
+        shell's ``stdin``. For example, if you're trying to invoke ``ssh`` in
+        a test, try adding the ``-n`` option to prevent it from closing
+        ``stdin``. Similarly, if you invoke a daemon process that inherits
+        ``stdout`` and fails to close it, it may cause Prysk to hang while
+        waiting for the test shell's ``stdout`` to be fully closed.
+        
+        .. _unified context diff: https://en.wikipedia.org/wiki/Diff#Unified_format
+        .. _its own example tests: https://github.com/nicoretti/prysk/tree/master/examples
+        
+Keywords: automatic functional test framework,snapshot testing
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU General Public License (GPL)
+Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Unix Shell
+Classifier: Topic :: Software Development :: Testing
```

