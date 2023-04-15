# Comparing `tmp/hebi-0.1.1.0.9.9.tar.gz` & `tmp/hebi-0.2.0.0.12.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hebi-0.1.1.0.9.9.tar", last modified: Thu Mar  9 19:31:27 2023, max compression
+gzip compressed data, was "hebi-0.2.0.0.12.5.tar", max compression
```

## Comparing `hebi-0.1.1.0.9.9.tar` & `hebi-0.2.0.0.12.5.tar`

### file list

```diff
@@ -1,45 +1,49 @@
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-03-09 19:31:27.961910 hebi-0.1.1.0.9.9/
--rw-r--r--   0 travis    (1000) travis    (1000)     1077 2023-03-09 19:29:50.000000 hebi-0.1.1.0.9.9/LICENSE.txt
--rw-r--r--   0 travis    (1000) travis    (1000)    10639 2023-03-09 19:31:27.961910 hebi-0.1.1.0.9.9/PKG-INFO
--rw-r--r--   0 travis    (1000) travis    (1000)     9981 2023-03-09 19:29:50.000000 hebi-0.1.1.0.9.9/README.md
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-03-09 19:31:27.949910 hebi-0.1.1.0.9.9/hebi/
--rw-r--r--   0 travis    (1000) travis    (1000)      419 2023-03-09 19:29:50.000000 hebi-0.1.1.0.9.9/hebi/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)     8101 2023-03-09 19:29:50.000000 hebi-0.1.1.0.9.9/hebi/__main__.py
--rw-r--r--   0 travis    (1000) travis    (1000)    25391 2023-03-09 19:29:50.000000 hebi-0.1.1.0.9.9/hebi/compiler.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-03-09 19:31:27.953910 hebi-0.1.1.0.9.9/hebi/optimize/
--rw-r--r--   0 travis    (1000) travis    (1000)        1 2023-03-09 19:29:50.000000 hebi-0.1.1.0.9.9/hebi/optimize/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)     6451 2023-03-09 19:29:50.000000 hebi-0.1.1.0.9.9/hebi/optimize/optimize_remove_deadvars.py
--rw-r--r--   0 travis    (1000) travis    (1000)      253 2023-03-09 19:29:50.000000 hebi-0.1.1.0.9.9/hebi/optimize/optimize_remove_pass.py
--rw-r--r--   0 travis    (1000) travis    (1000)     2528 2023-03-09 19:29:50.000000 hebi-0.1.1.0.9.9/hebi/optimize/optimize_varlen.py
--rw-r--r--   0 travis    (1000) travis    (1000)    12190 2023-03-09 19:29:50.000000 hebi-0.1.1.0.9.9/hebi/prelude.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-03-09 19:31:27.957910 hebi-0.1.1.0.9.9/hebi/rewrite/
--rw-r--r--   0 travis    (1000) travis    (1000)        0 2023-03-09 19:29:50.000000 hebi-0.1.1.0.9.9/hebi/rewrite/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)     3710 2023-03-09 19:29:50.000000 hebi-0.1.1.0.9.9/hebi/rewrite/rewrite_duplicate_assignment.py
--rw-r--r--   0 travis    (1000) travis    (1000)      704 2023-03-09 19:29:50.000000 hebi-0.1.1.0.9.9/hebi/rewrite/rewrite_forbidden_overwrites.py
--rw-r--r--   0 travis    (1000) travis    (1000)     2791 2023-03-09 19:29:50.000000 hebi-0.1.1.0.9.9/hebi/rewrite/rewrite_import.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1763 2023-03-09 19:29:50.000000 hebi-0.1.1.0.9.9/hebi/rewrite/rewrite_import_dataclasses.py
--rw-r--r--   0 travis    (1000) travis    (1000)     2616 2023-03-09 19:29:50.000000 hebi-0.1.1.0.9.9/hebi/rewrite/rewrite_import_hashlib.py
--rw-r--r--   0 travis    (1000) travis    (1000)     2012 2023-03-09 19:29:50.000000 hebi-0.1.1.0.9.9/hebi/rewrite/rewrite_import_plutusdata.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1183 2023-03-09 19:29:50.000000 hebi-0.1.1.0.9.9/hebi/rewrite/rewrite_import_typing.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1107 2023-03-09 19:29:50.000000 hebi-0.1.1.0.9.9/hebi/rewrite/rewrite_inject_builtin_constr.py
--rw-r--r--   0 travis    (1000) travis    (1000)      942 2023-03-09 19:29:50.000000 hebi-0.1.1.0.9.9/hebi/rewrite/rewrite_inject_builtins.py
--rw-r--r--   0 travis    (1000) travis    (1000)      851 2023-03-09 19:29:50.000000 hebi-0.1.1.0.9.9/hebi/rewrite/rewrite_remove_type_stuff.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1104 2023-03-09 19:29:50.000000 hebi-0.1.1.0.9.9/hebi/rewrite/rewrite_tuple_assign.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-03-09 19:31:27.961910 hebi-0.1.1.0.9.9/hebi/tests/
--rw-r--r--   0 travis    (1000) travis    (1000)        0 2023-03-09 19:29:50.000000 hebi-0.1.1.0.9.9/hebi/tests/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)    14258 2023-03-09 19:29:50.000000 hebi-0.1.1.0.9.9/hebi/tests/test_builtins.py
--rw-r--r--   0 travis    (1000) travis    (1000)    26917 2023-03-09 19:29:50.000000 hebi-0.1.1.0.9.9/hebi/tests/test_misc.py
--rw-r--r--   0 travis    (1000) travis    (1000)    17495 2023-03-09 19:29:50.000000 hebi-0.1.1.0.9.9/hebi/tests/test_ops.py
--rw-r--r--   0 travis    (1000) travis    (1000)     6508 2023-03-09 19:29:50.000000 hebi-0.1.1.0.9.9/hebi/tests/test_stdlib.py
--rw-r--r--   0 travis    (1000) travis    (1000)    28559 2023-03-09 19:29:50.000000 hebi-0.1.1.0.9.9/hebi/type_inference.py
--rw-r--r--   0 travis    (1000) travis    (1000)    39420 2023-03-09 19:29:50.000000 hebi-0.1.1.0.9.9/hebi/typed_ast.py
--rw-r--r--   0 travis    (1000) travis    (1000)    21346 2023-03-09 19:29:50.000000 hebi-0.1.1.0.9.9/hebi/util.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-03-09 19:31:27.953910 hebi-0.1.1.0.9.9/hebi.egg-info/
--rw-r--r--   0 travis    (1000) travis    (1000)    10639 2023-03-09 19:31:27.000000 hebi-0.1.1.0.9.9/hebi.egg-info/PKG-INFO
--rw-r--r--   0 travis    (1000) travis    (1000)     1057 2023-03-09 19:31:27.000000 hebi-0.1.1.0.9.9/hebi.egg-info/SOURCES.txt
--rw-r--r--   0 travis    (1000) travis    (1000)        1 2023-03-09 19:31:27.000000 hebi-0.1.1.0.9.9/hebi.egg-info/dependency_links.txt
--rw-r--r--   0 travis    (1000) travis    (1000)       44 2023-03-09 19:31:27.000000 hebi-0.1.1.0.9.9/hebi.egg-info/entry_points.txt
--rw-r--r--   0 travis    (1000) travis    (1000)       78 2023-03-09 19:31:27.000000 hebi-0.1.1.0.9.9/hebi.egg-info/requires.txt
--rw-r--r--   0 travis    (1000) travis    (1000)        5 2023-03-09 19:31:27.000000 hebi-0.1.1.0.9.9/hebi.egg-info/top_level.txt
--rw-r--r--   0 travis    (1000) travis    (1000)       38 2023-03-09 19:31:27.961910 hebi-0.1.1.0.9.9/setup.cfg
--rw-r--r--   0 travis    (1000) travis    (1000)     1857 2023-03-09 19:29:50.000000 hebi-0.1.1.0.9.9/setup.py
+-rw-r--r--   0        0        0     1077 2023-04-15 22:33:12.424800 hebi-0.2.0.0.12.5/LICENSE.txt
+-rw-r--r--   0        0        0    11864 2023-04-15 22:33:12.424800 hebi-0.2.0.0.12.5/README.md
+-rw-r--r--   0        0        0      430 2023-04-15 22:33:12.436800 hebi-0.2.0.0.12.5/hebi/__init__.py
+-rw-r--r--   0        0        0     7306 2023-04-15 22:33:12.436800 hebi-0.2.0.0.12.5/hebi/__main__.py
+-rw-r--r--   0        0        0     2330 2023-04-15 22:33:12.436800 hebi-0.2.0.0.12.5/hebi/builder.py
+-rw-r--r--   0        0        0    29084 2023-04-15 22:33:12.436800 hebi-0.2.0.0.12.5/hebi/compiler.py
+-rw-r--r--   0        0        0        0 2023-04-15 22:33:12.436800 hebi-0.2.0.0.12.5/hebi/ledger/__init__.py
+-rw-r--r--   0        0        0    11048 2023-04-15 22:33:12.436800 hebi-0.2.0.0.12.5/hebi/ledger/api_v2.py
+-rw-r--r--   0        0        0     3142 2023-04-15 22:33:12.436800 hebi-0.2.0.0.12.5/hebi/ledger/interval.py
+-rw-r--r--   0        0        0        1 2023-04-15 22:33:12.436800 hebi-0.2.0.0.12.5/hebi/optimize/__init__.py
+-rw-r--r--   0        0        0      410 2023-04-15 22:33:12.436800 hebi-0.2.0.0.12.5/hebi/optimize/optimize_remove_comments.py
+-rw-r--r--   0        0        0     6641 2023-04-15 22:33:12.436800 hebi-0.2.0.0.12.5/hebi/optimize/optimize_remove_deadvars.py
+-rw-r--r--   0        0        0      253 2023-04-15 22:33:12.436800 hebi-0.2.0.0.12.5/hebi/optimize/optimize_remove_pass.py
+-rw-r--r--   0        0        0     2528 2023-04-15 22:33:12.436800 hebi-0.2.0.0.12.5/hebi/optimize/optimize_varlen.py
+-rw-r--r--   0        0        0     3090 2023-04-15 22:33:12.436800 hebi-0.2.0.0.12.5/hebi/prelude.py
+-rw-r--r--   0        0        0        0 2023-04-15 22:33:12.436800 hebi-0.2.0.0.12.5/hebi/rewrite/__init__.py
+-rw-r--r--   0        0        0     3710 2023-04-15 22:33:12.436800 hebi-0.2.0.0.12.5/hebi/rewrite/rewrite_duplicate_assignment.py
+-rw-r--r--   0        0        0      704 2023-04-15 22:33:12.436800 hebi-0.2.0.0.12.5/hebi/rewrite/rewrite_forbidden_overwrites.py
+-rw-r--r--   0        0        0     4737 2023-04-15 22:33:12.436800 hebi-0.2.0.0.12.5/hebi/rewrite/rewrite_guaranteed_variables.py
+-rw-r--r--   0        0        0     3228 2023-04-15 22:33:12.436800 hebi-0.2.0.0.12.5/hebi/rewrite/rewrite_import.py
+-rw-r--r--   0        0        0     1899 2023-04-15 22:33:12.436800 hebi-0.2.0.0.12.5/hebi/rewrite/rewrite_import_dataclasses.py
+-rw-r--r--   0        0        0     2689 2023-04-15 22:33:12.436800 hebi-0.2.0.0.12.5/hebi/rewrite/rewrite_import_hashlib.py
+-rw-r--r--   0        0        0     2012 2023-04-15 22:33:12.436800 hebi-0.2.0.0.12.5/hebi/rewrite/rewrite_import_plutusdata.py
+-rw-r--r--   0        0        0     1183 2023-04-15 22:33:12.436800 hebi-0.2.0.0.12.5/hebi/rewrite/rewrite_import_typing.py
+-rw-r--r--   0        0        0     1148 2023-04-15 22:33:12.436800 hebi-0.2.0.0.12.5/hebi/rewrite/rewrite_inject_builtin_constr.py
+-rw-r--r--   0        0        0      942 2023-04-15 22:33:12.436800 hebi-0.2.0.0.12.5/hebi/rewrite/rewrite_inject_builtins.py
+-rw-r--r--   0        0        0      851 2023-04-15 22:33:12.436800 hebi-0.2.0.0.12.5/hebi/rewrite/rewrite_remove_type_stuff.py
+-rw-r--r--   0        0        0      367 2023-04-15 22:33:12.436800 hebi-0.2.0.0.12.5/hebi/rewrite/rewrite_subscript38.py
+-rw-r--r--   0        0        0     2212 2023-04-15 22:33:12.436800 hebi-0.2.0.0.12.5/hebi/rewrite/rewrite_tuple_assign.py
+-rw-r--r--   0        0        0     1498 2023-04-15 22:33:12.436800 hebi-0.2.0.0.12.5/hebi/rewrite/rewrite_zero_ary.py
+-rw-r--r--   0        0        0        0 2023-04-15 22:33:12.436800 hebi-0.2.0.0.12.5/hebi/std/__init__.py
+-rw-r--r--   0        0        0     3181 2023-04-15 22:33:12.436800 hebi-0.2.0.0.12.5/hebi/std/fractions.py
+-rw-r--r--   0        0        0      445 2023-04-15 22:33:12.436800 hebi-0.2.0.0.12.5/hebi/std/math.py
+-rw-r--r--   0        0        0        0 2023-04-15 22:33:12.436800 hebi-0.2.0.0.12.5/hebi/tests/__init__.py
+-rw-r--r--   0        0        0    14906 2023-04-15 22:33:12.436800 hebi-0.2.0.0.12.5/hebi/tests/test_builtins.py
+-rw-r--r--   0        0        0        0 2023-04-15 22:33:12.436800 hebi-0.2.0.0.12.5/hebi/tests/test_ledger/__init__.py
+-rw-r--r--   0        0        0     3400 2023-04-15 22:33:12.436800 hebi-0.2.0.0.12.5/hebi/tests/test_ledger/test_api_v2.py
+-rw-r--r--   0        0        0     5947 2023-04-15 22:33:12.436800 hebi-0.2.0.0.12.5/hebi/tests/test_ledger/test_interval.py
+-rw-r--r--   0        0        0    29495 2023-04-15 22:33:12.436800 hebi-0.2.0.0.12.5/hebi/tests/test_misc.py
+-rw-r--r--   0        0        0    17394 2023-04-15 22:33:12.436800 hebi-0.2.0.0.12.5/hebi/tests/test_ops.py
+-rw-r--r--   0        0        0        0 2023-04-15 22:33:12.436800 hebi-0.2.0.0.12.5/hebi/tests/test_std/__init__.py
+-rw-r--r--   0        0        0     4580 2023-04-15 22:33:12.436800 hebi-0.2.0.0.12.5/hebi/tests/test_std/test_fractions.py
+-rw-r--r--   0        0        0      617 2023-04-15 22:33:12.436800 hebi-0.2.0.0.12.5/hebi/tests/test_std/test_math.py
+-rw-r--r--   0        0        0    10549 2023-04-15 22:33:12.436800 hebi-0.2.0.0.12.5/hebi/tests/test_stdlib.py
+-rw-r--r--   0        0        0    28901 2023-04-15 22:33:12.436800 hebi-0.2.0.0.12.5/hebi/type_inference.py
+-rw-r--r--   0        0        0    40596 2023-04-15 22:33:12.436800 hebi-0.2.0.0.12.5/hebi/typed_ast.py
+-rw-r--r--   0        0        0    21810 2023-04-15 22:33:12.436800 hebi-0.2.0.0.12.5/hebi/util.py
+-rw-r--r--   0        0        0     1364 2023-04-15 22:33:12.436800 hebi-0.2.0.0.12.5/pyproject.toml
+-rw-r--r--   0        0        0    13190 1970-01-01 00:00:00.000000 hebi-0.2.0.0.12.5/PKG-INFO
```

### Comparing `hebi-0.1.1.0.9.9/LICENSE.txt` & `hebi-0.2.0.0.12.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hebi-0.1.1.0.9.9/PKG-INFO` & `hebi-0.2.0.0.12.5/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,103 +1,96 @@
-Metadata-Version: 2.1
-Name: hebi
-Version: 0.1.1.0.9.9
-Summary: A simple pythonic programming language for Smart Contracts on Cardano 
-Home-page: https://github.com/imperatorlang/hebi
-Author: nielstron
-Author-email: n.muendler@web.de
-License: MIT
-Keywords: python cardano smart contract blockchain verification haskell
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Compilers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.8, <3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 
 <div align="center">
 
 <img  src="https://raw.githubusercontent.com/OpShin/hebi/master/hebi.png" width="240" />
 <h1 style="text-align: center;">hebi</h1></br>
 
 
-[![Build Status](https://app.travis-ci.com/OpShin/hebi.svg?branch=master)](https://app.travis-ci.com/OpShin/hebi)
-[![PyPI version](https://badge.fury.io/py/hebi.svg)](https://pypi.org/project/hebi/)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hebi.svg)
-[![PyPI - Status](https://img.shields.io/pypi/status/hebi.svg)](https://pypi.org/project/hebi/)
-[![Coverage Status](https://coveralls.io/repos/github/OpShin/hebi/badge.svg?branch=master)](https://coveralls.io/github/OpShin/hebi?branch=master)
+<a href="https://app.travis-ci.com/OpShin/hebi"><img alt="Build Status" src="https://app.travis-ci.com/OpShin/hebi.svg?branch=main"/></a>
+<a href="https://pypi.org/project/hebi/"><img alt="PyPI version" src="https://badge.fury.io/py/hebi.svg"/></a>
+<img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/hebi.svg" />
+<a href="https://pypi.org/project/hebi/"><img alt="PyPI - Status" src="https://img.shields.io/pypi/status/hebi.svg" /></a>
+<a href="https://coveralls.io/github/OpShin/hebi?branch=main"><img alt="Coverage Status" src="https://coveralls.io/repos/github/OpShin/hebi/badge.svg?branch=main" /></a>
 
 </div>
 
+> You are building what you want. Why not also build **how** you want?
+
+
 This is an implementation of smart contracts for Cardano which are written in a very strict subset of valid Python.
 The general philosophy of this project is to write a compiler that 
 ensure the following:
 
 If the program compiles then:
+
 1. it is a valid Python program
 2. the output running it with python is the same as running it on-chain.
 
+
+> Note this is the sister project of [eopsin](https://github.com/ImperatorLang/eopsin).
+It uses an even more restricted subset of python (for example no while loops).
+The benefit is that the resulting code is greatly reduced in size and cpu/memory consumption.
+
+
 ### Why hebi?
 - 100% valid Python. Leverage the existing tool stack for Python, syntax highlighting, linting, debugging, unit-testing, [property-based testing](https://hypothesis.readthedocs.io/), [verification](https://github.com/marcoeilers/nagini)
 - Intuitive. Just like Python.
-- Flexible. Imperative, functional, the way you want it.
+- Functional. Forces you to write elegant, functional code in Python.
 - Efficient & Secure. Static type inference ensures strict typing and optimized code
 
-Note this is the sister project of [eopsin](https://github.com/ImperatorLang/eopsin).
-It uses an even more restricted subset of python (for example no if & while).
-The benefit is that the resulting code is greatly reduced in size and cpu/memory consumption.
-
 Eopsin is more comfortable to use than hebi.
 If you want to start building, write your contract in eopsin first.
 Then, after everything works to your pleasing, try to port to hebi and enjoy the performance gains.
 
 ### Getting Started
 
+#### OpShin Pioneer Program
+
+Check out the [opshin-pioneer-program](
+https://github.com/OpShin/opshin-pioneer-program) for a host of educational example contracts, test cases and off-chain code.
+
 #### Example repository
 
-Check out this example repository for a quick start in setting up a development environment
-and compiling some sample contracts yours:
+Check out the [opshin-starter-kit](
+https://github.com/OpShin/opshin-starter-kit) repository for a quick start in setting up a development environment
+and compiling some sample contracts yourself.
 
-https://github.com/OpShin/eopsin-example
 
 You can replace the contracts in your local copy of the repository with code from the
 `examples` section here to start exploring different contracts.
 
 #### Developer Community and Questions
 
 The eopsin repository contains a discussions page.
 Feel free to open up a new discussion with questions regarding development using hebi and using certain features.
 Others may be able to help you and will also benefit from the previously shared questions.
 
-Check out the community [here](https://github.com/OpShin/eopsin/discussions)
+Check out the community [here](https://github.com/OpShin/opshin/discussions)
 
 You can also chat with other developers [in the welcoming discord
-community](https://discord.gg/2ETSZnQQH9) of OpShin
+community](https://discord.gg/umR3A2g4uw) of OpShin
 
 #### Installation
 
-Install Python 3.8. Then run
+Install Python 3.8, 3.9 or 3.10. Then run
 
 ```bash
-python3.8 -m pip install hebi
+python3 -m pip install hebi
 ```
 
 #### Writing a Smart Contract
 
 A short non-complete introduction in starting to write smart contracts follows.
 
 1. Make sure you understand EUTxOs, Addresses, Validators etc on Cardano. [There is a wonderful crashcourse by @KtorZ](https://aiken-lang.org/fundamentals/eutxo). The contract will work on these concepts
-2. Make sure you understand python. Eopsin works like python and uses python. There are tons of tutorials for python, choose what suits you best.
+2. Make sure you understand python. hebi works like python and uses python. There are tons of tutorials for python, choose what suits you best.
 3. Make sure your contract is valid python and the types check out. Write simple contracts first and run them using `hebi eval` to get a feeling for how they work.
 4. Make sure your contract is valid hebi code. Run `hebi compile` and look at the compiler erros for guidance along what works and doesn't work and why.
-5. Dig into the [`examples`](https://github.com/OpShin/hebi/tree/master/examples) to understand common patterns. Check out the [`prelude`](https://imperatorlang.github.io/hebi/hebi/prelude.html) for understanding how the Script Context is structured and how complex datums are defined.
-6. Check out the [sample repository](https://github.com/OpShin/eopsin-example) to find a sample setup for developing your own contract.
+5. Dig into the [`examples`](https://github.com/OpShin/hebi/tree/main/examples) to understand common patterns. Check out the [`prelude`](https://hebi.opshin.dev/hebi/prelude.html) for understanding how the Script Context is structured and how complex datums are defined.
+6. Check out the [sample repository](https://github.com/OpShin/opshin-starter-kit) to find a sample setup for developing your own contract.
 
 
 In summary, a smart contract in hebi is defined by the function `validator` in your contract file.
 The function validates that a specific value can be spent, minted, burned, withdrawn etc, depending
 on where it is invoked/used as a credential.
 If the function fails (i.e. raises an error of any kind such as a `KeyError` or `AssertionError`)
 the validation is denied, and the funds can not be spent, minted, burned etc.
@@ -109,30 +102,35 @@
 
 A simple contract called the "Gift Contract" verifies that only specific wallets can withdraw money.
 They are authenticated by a signature.
 If you don't understand what a pubkeyhash is and how this validates anything, check out [this gentle introduction into Cardanos EUTxO](https://aiken-lang.org/fundamentals/eutxo).
 Also see the [tutorial by `pycardano`](https://pycardano.readthedocs.io/en/latest/guides/plutus.html) for explanations on what each of the parameters to the validator means
 and how to build transactions with the contract.
 
-
 ```python3
 from hebi.prelude import *
 
-@dataclass()
-class CancelDatum(PlutusData):
+@dataclass
+class WithdrawDatum(PlutusData):
     pubkeyhash: bytes
 
 
-def validator(datum: CancelDatum, redeemer: None, context: ScriptContext) -> None:
+def validator(datum: WithdrawDatum, redeemer: None, context: ScriptContext) -> None:
     assert datum.pubkeyhash in context.tx_info.signatories, "Required signature missing"
 ```
 
 All contracts written in hebi are 100% valid python.
-Minting policies follow the same structure, but expect a value of type `None` as first argument.
-See the `examples` directory for more.
+Minting policies expect only a redeemer and script context as argument.
+Check out the [Architecture guide](https://github.com/OpShin/hebi/blob/main/ARCHITECTURE.md#minting-policy---spending-validator-double-function)
+for details on how to write double functioning contracts.
+The [`examples`](https://github.com/OpShin/hebi/blob/main/examples) folder contains more examples.
+Also check out the [opshin-pioneer-program](
+https://github.com/OpShin/opshin-pioneer-program)
+and [opshin-starter-kit](
+https://github.com/OpShin/opshin-starter-kit) repo.
 
 ### Compiling
 
 Write your program in python. You may start with the content of `examples`.
 Arguments to scripts are passed in as Plutus Data objects in JSON notation.
 
 You can run any of the following commands
@@ -149,16 +147,15 @@
 The deploy process generates all artifacts required for usage with common libraries like [pycardano](https://github.com/Python-Cardano/pycardano), [lucid](https://github.com/spacebudz/lucid) and the [cardano-cli](https://github.com/input-output-hk/cardano-node).
 
 ```bash
 # Automatically generate all artifacts needed for using this contract
 hebi build examples/smart_contracts/assert_sum.py
 ```
 
-See the [tutorial by `pycardano`](https://pycardano.readthedocs.io/en/latest/guides/plutus.html) for explanations how to build transactions with `eopsin` contracts.
-Contracts in hebi are invoked the same, so you can just follow the tutorial there.
+See the [tutorial by `pycardano`](https://pycardano.readthedocs.io/en/latest/guides/plutus.html) for explanations how to build transactions with `opshin` contracts.
 
 ### The small print
 
 _Not every valid python program is a valid smart contract_.
 Not all language features of python will or can be supported.
 The reasons are mainly of practical nature (i.e. we can't infer types when functions like `eval` are allowed).
 Specifically, only a pure subset of python is allowed.
@@ -180,14 +177,15 @@
 that a recent eopsin release is integrated that contains a security patch.
 
 ## Contributing
 
 ### Architecture
 
 This program consists of a few independent components:
+
 1. An aggressive static type inferencer
 2. Rewriting tools to simplify complex python expressions
 3. A compiler from a subset of python into UPLC
 
 ### Debugging artefacts
 
 For debugging purposes, you can also run
@@ -200,16 +198,23 @@
 python3 -m hebi compile_pluto examples/smart_contracts/assert_sum.py
 ```
 
 ### Sponsoring
 
 You can sponsor the development of hebi through GitHub or [Teiki](https://alpha.teiki.network/projects/opshin) or just by sending ADA. Drop me a message on social media and let me know what it is for.
 
-- **[Teiki](https://alpha.teiki.network/projects/opshin)** Stake your ada to support OpShin at [Teiki](https://alpha.teiki.network/projects/opshin)
+- **[Kreate](https://beta.kreate.community/projects/opshin)** Stake your ada to support OpShin at [Kreate](https://beta.kreate.community/projects/opshin)
 - **GitHub** Sponsor the developers of this project through the button "Sponsor" next to them
 - **ADA** Donation in ADA can be submitted to `$opshin` or `addr1qyz3vgd5xxevjy2rvqevz9n7n7dney8n6hqggp23479fm6vwpj9clsvsf85cd4xc59zjztr5zwpummwckmzr2myjwjns74lhmr`.
 
 ### Supporters
 
 <a href="https://github.com/inversion-dev"><img src="https://avatars.githubusercontent.com/u/127298233?s=200&v=4" width="50"></a>
 <a href="https://github.com/MuesliSwapTeam/"><img  src="https://avatars.githubusercontent.com/u/91151317?v=4" width="50" /></a>
 <a href="https://github.com/AadaFinance/"><img  src="https://avatars.githubusercontent.com/u/89693711?v=4" width="50" /></a>
+
+The main sponsor of this project is [Inversion](https://inversion.dev/cardano/). Here is a word from them!
+
+> At Inversion, we pride ourselves on our passion for life and our ability to create exceptional software solutions for our clients. Our team of experts, with over a century of cumulative experience, is dedicated to harnessing the power of the Cardano blockchain to bring innovative and scalable decentralized applications to life. We've successfully built applications for NFT management, staking and delegation, chain data monitoring, analytics, and web3 integrations, as well as countless non-blockchain systems. With a focus on security, transparency, and sustainability, our team is excited to contribute to the Cardano ecosystem, pushing the boundaries of decentralized technologies to improve lives worldwide. Trust Inversion to be your go-to partner for robust, effective, and forward-thinking solutions, whether blockchain based, traditional systems, or a mix of the two.
+
+They have recently started a podcast, called "Africa On Chain", which you can check out here:
+https://www.youtube.com/@africaonchain
```

### Comparing `hebi-0.1.1.0.9.9/README.md` & `hebi-0.2.0.0.12.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,85 +1,127 @@
+Metadata-Version: 2.1
+Name: hebi
+Version: 0.2.0.0.12.5
+Summary: A simple and fast pythonic programming language for Smart Contracts on Cardano
+Home-page: https://github.com/opshin/hebi
+License: MIT
+Keywords: python,language,programming-language,compiler,validator,smart-contracts,cardano
+Author: nielstron
+Author-email: n.muendler@web.de
+Requires-Python: >=3.8,<3.12
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Software Development :: Compilers
+Requires-Dist: frozenlist (>=1.3.3,<2.0.0)
+Requires-Dist: pluthon (>=0.3.3,<0.4.0)
+Requires-Dist: pycardano (>=0.8.0,<0.9.0)
+Requires-Dist: uplc (>=0.6.1,<0.7.0)
+Project-URL: Documentation, https://hebi.opshin.dev/
+Project-URL: Repository, https://github.com/opshin/hebi
+Description-Content-Type: text/markdown
+
 
 <div align="center">
 
 <img  src="https://raw.githubusercontent.com/OpShin/hebi/master/hebi.png" width="240" />
 <h1 style="text-align: center;">hebi</h1></br>
 
 
-[![Build Status](https://app.travis-ci.com/OpShin/hebi.svg?branch=master)](https://app.travis-ci.com/OpShin/hebi)
-[![PyPI version](https://badge.fury.io/py/hebi.svg)](https://pypi.org/project/hebi/)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hebi.svg)
-[![PyPI - Status](https://img.shields.io/pypi/status/hebi.svg)](https://pypi.org/project/hebi/)
-[![Coverage Status](https://coveralls.io/repos/github/OpShin/hebi/badge.svg?branch=master)](https://coveralls.io/github/OpShin/hebi?branch=master)
+<a href="https://app.travis-ci.com/OpShin/hebi"><img alt="Build Status" src="https://app.travis-ci.com/OpShin/hebi.svg?branch=main"/></a>
+<a href="https://pypi.org/project/hebi/"><img alt="PyPI version" src="https://badge.fury.io/py/hebi.svg"/></a>
+<img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/hebi.svg" />
+<a href="https://pypi.org/project/hebi/"><img alt="PyPI - Status" src="https://img.shields.io/pypi/status/hebi.svg" /></a>
+<a href="https://coveralls.io/github/OpShin/hebi?branch=main"><img alt="Coverage Status" src="https://coveralls.io/repos/github/OpShin/hebi/badge.svg?branch=main" /></a>
 
 </div>
 
+> You are building what you want. Why not also build **how** you want?
+
+
 This is an implementation of smart contracts for Cardano which are written in a very strict subset of valid Python.
 The general philosophy of this project is to write a compiler that 
 ensure the following:
 
 If the program compiles then:
+
 1. it is a valid Python program
 2. the output running it with python is the same as running it on-chain.
 
+
+> Note this is the sister project of [eopsin](https://github.com/ImperatorLang/eopsin).
+It uses an even more restricted subset of python (for example no while loops).
+The benefit is that the resulting code is greatly reduced in size and cpu/memory consumption.
+
+
 ### Why hebi?
 - 100% valid Python. Leverage the existing tool stack for Python, syntax highlighting, linting, debugging, unit-testing, [property-based testing](https://hypothesis.readthedocs.io/), [verification](https://github.com/marcoeilers/nagini)
 - Intuitive. Just like Python.
-- Flexible. Imperative, functional, the way you want it.
+- Functional. Forces you to write elegant, functional code in Python.
 - Efficient & Secure. Static type inference ensures strict typing and optimized code
 
-Note this is the sister project of [eopsin](https://github.com/ImperatorLang/eopsin).
-It uses an even more restricted subset of python (for example no if & while).
-The benefit is that the resulting code is greatly reduced in size and cpu/memory consumption.
-
 Eopsin is more comfortable to use than hebi.
 If you want to start building, write your contract in eopsin first.
 Then, after everything works to your pleasing, try to port to hebi and enjoy the performance gains.
 
 ### Getting Started
 
+#### OpShin Pioneer Program
+
+Check out the [opshin-pioneer-program](
+https://github.com/OpShin/opshin-pioneer-program) for a host of educational example contracts, test cases and off-chain code.
+
 #### Example repository
 
-Check out this example repository for a quick start in setting up a development environment
-and compiling some sample contracts yours:
+Check out the [opshin-starter-kit](
+https://github.com/OpShin/opshin-starter-kit) repository for a quick start in setting up a development environment
+and compiling some sample contracts yourself.
 
-https://github.com/OpShin/eopsin-example
 
 You can replace the contracts in your local copy of the repository with code from the
 `examples` section here to start exploring different contracts.
 
 #### Developer Community and Questions
 
 The eopsin repository contains a discussions page.
 Feel free to open up a new discussion with questions regarding development using hebi and using certain features.
 Others may be able to help you and will also benefit from the previously shared questions.
 
-Check out the community [here](https://github.com/OpShin/eopsin/discussions)
+Check out the community [here](https://github.com/OpShin/opshin/discussions)
 
 You can also chat with other developers [in the welcoming discord
-community](https://discord.gg/2ETSZnQQH9) of OpShin
+community](https://discord.gg/umR3A2g4uw) of OpShin
 
 #### Installation
 
-Install Python 3.8. Then run
+Install Python 3.8, 3.9 or 3.10. Then run
 
 ```bash
-python3.8 -m pip install hebi
+python3 -m pip install hebi
 ```
 
 #### Writing a Smart Contract
 
 A short non-complete introduction in starting to write smart contracts follows.
 
 1. Make sure you understand EUTxOs, Addresses, Validators etc on Cardano. [There is a wonderful crashcourse by @KtorZ](https://aiken-lang.org/fundamentals/eutxo). The contract will work on these concepts
-2. Make sure you understand python. Eopsin works like python and uses python. There are tons of tutorials for python, choose what suits you best.
+2. Make sure you understand python. hebi works like python and uses python. There are tons of tutorials for python, choose what suits you best.
 3. Make sure your contract is valid python and the types check out. Write simple contracts first and run them using `hebi eval` to get a feeling for how they work.
 4. Make sure your contract is valid hebi code. Run `hebi compile` and look at the compiler erros for guidance along what works and doesn't work and why.
-5. Dig into the [`examples`](https://github.com/OpShin/hebi/tree/master/examples) to understand common patterns. Check out the [`prelude`](https://imperatorlang.github.io/hebi/hebi/prelude.html) for understanding how the Script Context is structured and how complex datums are defined.
-6. Check out the [sample repository](https://github.com/OpShin/eopsin-example) to find a sample setup for developing your own contract.
+5. Dig into the [`examples`](https://github.com/OpShin/hebi/tree/main/examples) to understand common patterns. Check out the [`prelude`](https://hebi.opshin.dev/hebi/prelude.html) for understanding how the Script Context is structured and how complex datums are defined.
+6. Check out the [sample repository](https://github.com/OpShin/opshin-starter-kit) to find a sample setup for developing your own contract.
 
 
 In summary, a smart contract in hebi is defined by the function `validator` in your contract file.
 The function validates that a specific value can be spent, minted, burned, withdrawn etc, depending
 on where it is invoked/used as a credential.
 If the function fails (i.e. raises an error of any kind such as a `KeyError` or `AssertionError`)
 the validation is denied, and the funds can not be spent, minted, burned etc.
@@ -91,30 +133,35 @@
 
 A simple contract called the "Gift Contract" verifies that only specific wallets can withdraw money.
 They are authenticated by a signature.
 If you don't understand what a pubkeyhash is and how this validates anything, check out [this gentle introduction into Cardanos EUTxO](https://aiken-lang.org/fundamentals/eutxo).
 Also see the [tutorial by `pycardano`](https://pycardano.readthedocs.io/en/latest/guides/plutus.html) for explanations on what each of the parameters to the validator means
 and how to build transactions with the contract.
 
-
 ```python3
 from hebi.prelude import *
 
-@dataclass()
-class CancelDatum(PlutusData):
+@dataclass
+class WithdrawDatum(PlutusData):
     pubkeyhash: bytes
 
 
-def validator(datum: CancelDatum, redeemer: None, context: ScriptContext) -> None:
+def validator(datum: WithdrawDatum, redeemer: None, context: ScriptContext) -> None:
     assert datum.pubkeyhash in context.tx_info.signatories, "Required signature missing"
 ```
 
 All contracts written in hebi are 100% valid python.
-Minting policies follow the same structure, but expect a value of type `None` as first argument.
-See the `examples` directory for more.
+Minting policies expect only a redeemer and script context as argument.
+Check out the [Architecture guide](https://github.com/OpShin/hebi/blob/main/ARCHITECTURE.md#minting-policy---spending-validator-double-function)
+for details on how to write double functioning contracts.
+The [`examples`](https://github.com/OpShin/hebi/blob/main/examples) folder contains more examples.
+Also check out the [opshin-pioneer-program](
+https://github.com/OpShin/opshin-pioneer-program)
+and [opshin-starter-kit](
+https://github.com/OpShin/opshin-starter-kit) repo.
 
 ### Compiling
 
 Write your program in python. You may start with the content of `examples`.
 Arguments to scripts are passed in as Plutus Data objects in JSON notation.
 
 You can run any of the following commands
@@ -131,16 +178,15 @@
 The deploy process generates all artifacts required for usage with common libraries like [pycardano](https://github.com/Python-Cardano/pycardano), [lucid](https://github.com/spacebudz/lucid) and the [cardano-cli](https://github.com/input-output-hk/cardano-node).
 
 ```bash
 # Automatically generate all artifacts needed for using this contract
 hebi build examples/smart_contracts/assert_sum.py
 ```
 
-See the [tutorial by `pycardano`](https://pycardano.readthedocs.io/en/latest/guides/plutus.html) for explanations how to build transactions with `eopsin` contracts.
-Contracts in hebi are invoked the same, so you can just follow the tutorial there.
+See the [tutorial by `pycardano`](https://pycardano.readthedocs.io/en/latest/guides/plutus.html) for explanations how to build transactions with `opshin` contracts.
 
 ### The small print
 
 _Not every valid python program is a valid smart contract_.
 Not all language features of python will or can be supported.
 The reasons are mainly of practical nature (i.e. we can't infer types when functions like `eval` are allowed).
 Specifically, only a pure subset of python is allowed.
@@ -162,14 +208,15 @@
 that a recent eopsin release is integrated that contains a security patch.
 
 ## Contributing
 
 ### Architecture
 
 This program consists of a few independent components:
+
 1. An aggressive static type inferencer
 2. Rewriting tools to simplify complex python expressions
 3. A compiler from a subset of python into UPLC
 
 ### Debugging artefacts
 
 For debugging purposes, you can also run
@@ -182,16 +229,24 @@
 python3 -m hebi compile_pluto examples/smart_contracts/assert_sum.py
 ```
 
 ### Sponsoring
 
 You can sponsor the development of hebi through GitHub or [Teiki](https://alpha.teiki.network/projects/opshin) or just by sending ADA. Drop me a message on social media and let me know what it is for.
 
-- **[Teiki](https://alpha.teiki.network/projects/opshin)** Stake your ada to support OpShin at [Teiki](https://alpha.teiki.network/projects/opshin)
+- **[Kreate](https://beta.kreate.community/projects/opshin)** Stake your ada to support OpShin at [Kreate](https://beta.kreate.community/projects/opshin)
 - **GitHub** Sponsor the developers of this project through the button "Sponsor" next to them
 - **ADA** Donation in ADA can be submitted to `$opshin` or `addr1qyz3vgd5xxevjy2rvqevz9n7n7dney8n6hqggp23479fm6vwpj9clsvsf85cd4xc59zjztr5zwpummwckmzr2myjwjns74lhmr`.
 
 ### Supporters
 
 <a href="https://github.com/inversion-dev"><img src="https://avatars.githubusercontent.com/u/127298233?s=200&v=4" width="50"></a>
 <a href="https://github.com/MuesliSwapTeam/"><img  src="https://avatars.githubusercontent.com/u/91151317?v=4" width="50" /></a>
 <a href="https://github.com/AadaFinance/"><img  src="https://avatars.githubusercontent.com/u/89693711?v=4" width="50" /></a>
+
+The main sponsor of this project is [Inversion](https://inversion.dev/cardano/). Here is a word from them!
+
+> At Inversion, we pride ourselves on our passion for life and our ability to create exceptional software solutions for our clients. Our team of experts, with over a century of cumulative experience, is dedicated to harnessing the power of the Cardano blockchain to bring innovative and scalable decentralized applications to life. We've successfully built applications for NFT management, staking and delegation, chain data monitoring, analytics, and web3 integrations, as well as countless non-blockchain systems. With a focus on security, transparency, and sustainability, our team is excited to contribute to the Cardano ecosystem, pushing the boundaries of decentralized technologies to improve lives worldwide. Trust Inversion to be your go-to partner for robust, effective, and forward-thinking solutions, whether blockchain based, traditional systems, or a mix of the two.
+
+They have recently started a podcast, called "Africa On Chain", which you can check out here:
+https://www.youtube.com/@africaonchain
+
```

### Comparing `hebi-0.1.1.0.9.9/hebi/__main__.py` & `hebi-0.2.0.0.12.5/hebi/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,21 +3,19 @@
 import importlib
 import json
 import pathlib
 import sys
 import typing
 import ast
 
-import cbor2
-import pyaiken
 import pycardano
 import uplc
 import uplc.ast
 
-from hebi import __version__, compiler
+from hebi import compiler, builder
 from hebi.util import CompilerError, data_from_json
 
 
 class Command(enum.Enum):
     compile_pluto = "compile_pluto"
     compile = "compile"
     eval = "eval"
@@ -90,17 +88,17 @@
     command = Command(args.command)
     input_file = args.input_file if args.input_file != "-" else sys.stdin
     with open(input_file, "r") as f:
         source_code = f.read()
 
     if command == Command.eval:
         if args.input_file == "-":
-            with open("__tmp_eopsin.py", "w") as fp:
+            with open("__tmp_opshin.py", "w") as fp:
                 fp.write(source_code)
-            input_file = "__tmp_eopsin.py"
+            input_file = "__tmp_opshin.py"
         sys.path.append(str(pathlib.Path(input_file).parent.absolute()))
         sc = importlib.import_module(pathlib.Path(input_file).stem)
         sys.path.pop()
         print("Starting execution")
         print("------------------")
         try:
             parsed_args = [
@@ -157,15 +155,15 @@
     code = code.compile()
 
     # apply parameters from the command line to the contract (instantiates parameterized contract!)
     code = code.term
     # UPLC lambdas may only take one argument at a time, so we evaluate by repeatedly applying
     for d in map(data_from_json, map(json.loads, args.args)):
         code = uplc.ast.Apply(code, d)
-    code = uplc.ast.Program("1.0.0", code)
+    code = uplc.ast.Program((1, 0, 0), code)
 
     if command == Command.compile:
         print(code.dumps())
         return
 
     if command == Command.build:
         if args.output_directory == "":
@@ -174,46 +172,25 @@
                     "Please supply an output directory if no input file is specified."
                 )
                 exit(-1)
             target_dir = pathlib.Path("build") / pathlib.Path(input_file).stem
         else:
             target_dir = pathlib.Path(args.output_directory)
         target_dir.mkdir(exist_ok=True, parents=True)
-        uplc_dump = code.dumps()
-        cbor_hex = pyaiken.uplc.flat(uplc_dump)
-        # create cbor file for use with pycardano/lucid
+        artifacts = builder.generate_artifacts(builder._build(code))
         with (target_dir / "script.cbor").open("w") as fp:
-            fp.write(cbor_hex)
-        cbor = bytes.fromhex(cbor_hex)
-        # double wrap
-        cbor_wrapped = cbor2.dumps(cbor)
-        cbor_wrapped_hex = cbor_wrapped.hex()
-        # create plutus file
-        d = {
-            "type": "PlutusScriptV2",
-            "description": f"Eopsin {__version__} Smart Contract",
-            "cborHex": cbor_wrapped_hex,
-        }
+            fp.write(artifacts.cbor_hex)
         with (target_dir / "script.plutus").open("w") as fp:
-            json.dump(d, fp)
-        script_hash = pycardano.plutus_script_hash(pycardano.PlutusV2Script(cbor))
-        # generate policy ids
+            fp.write(artifacts.plutus_json)
         with (target_dir / "script.policy_id").open("w") as fp:
-            fp.write(script_hash.to_primitive().hex())
-        addr_mainnet = pycardano.Address(
-            script_hash, network=pycardano.Network.MAINNET
-        ).encode()
-        # generate addresses
+            fp.write(artifacts.policy_id)
         with (target_dir / "mainnet.addr").open("w") as fp:
-            fp.write(addr_mainnet)
-        addr_testnet = pycardano.Address(
-            script_hash, network=pycardano.Network.TESTNET
-        ).encode()
+            fp.write(artifacts.mainnet_addr)
         with (target_dir / "testnet.addr").open("w") as fp:
-            fp.write(addr_testnet)
+            fp.write(artifacts.testnet_addr)
 
         print(f"Wrote script artifacts to {target_dir}/")
         return
     if command == Command.eval_uplc:
         print("Starting execution")
         print("------------------")
         assert isinstance(code, uplc.ast.Program)
```

### Comparing `hebi-0.1.1.0.9.9/hebi/compiler.py` & `hebi-0.2.0.0.12.5/hebi/compiler.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 import logging
 from logging import getLogger
 from ast import fix_missing_locations
 
+from .optimize.optimize_remove_comments import OptimizeRemoveDeadconstants
 from .rewrite.rewrite_forbidden_overwrites import RewriteForbiddenOverwrites
+from .rewrite.rewrite_guaranteed_variables import RewriteGuaranteedVariables
 from .rewrite.rewrite_import import RewriteImport
 from .rewrite.rewrite_import_dataclasses import RewriteImportDataclasses
 from .rewrite.rewrite_import_hashlib import RewriteImportHashlib
 from .rewrite.rewrite_import_plutusdata import RewriteImportPlutusData
 from .rewrite.rewrite_import_typing import RewriteImportTyping
 from .rewrite.rewrite_inject_builtins import RewriteInjectBuiltins
 from .rewrite.rewrite_inject_builtin_constr import RewriteInjectBuiltinsConstr
 from .rewrite.rewrite_remove_type_stuff import RewriteRemoveTypeStuff
+from .rewrite.rewrite_subscript38 import RewriteSubscript38
 from .rewrite.rewrite_tuple_assign import RewriteTupleAssign
 from .rewrite.rewrite_duplicate_assignment import RewriteDuplicateAssignment
+from .rewrite.rewrite_zero_ary import RewriteZeroAry
 from .optimize.optimize_remove_pass import OptimizeRemovePass
 from .optimize.optimize_remove_deadvars import OptimizeRemoveDeadvars
-from .optimize.optimize_varlen import OptimizeVarlen
 from .type_inference import *
 from .util import CompilingNodeTransformer, PowImpl
 from .typed_ast import transform_ext_params_map, transform_output_map, RawPlutoExpr
 
 
 _LOGGER = logging.getLogger(__name__)
 
-STATEMONAD = "s"
-
-
 BinOpMap = {
     Add: {
         IntegerInstanceType: {
             IntegerInstanceType: plt.AddInteger,
         },
         ByteStringInstanceType: {
             ByteStringInstanceType: plt.AppendByteString,
@@ -116,16 +116,17 @@
 class UPLCCompiler(CompilingNodeTransformer):
     """
     Expects a TypedAST and returns UPLC/Pluto like code
     """
 
     step = "Compiling python statements to UPLC"
 
-    def __init__(self, force_three_params=False):
+    def __init__(self, force_three_params=False, validator_function_name="validator"):
         self.force_three_params = force_three_params
+        self.validator_function_name = validator_function_name
 
     def visit_sequence(
         self, node_seq: typing.List[typedstmt]
     ) -> typing.Callable[[plt.AST], plt.AST]:
         def g(s: plt.AST):
             for n in reversed(node_seq):
                 compiled_stmt = self.visit(n)
@@ -183,28 +184,29 @@
         )
 
     def visit_Module(self, node: TypedModule) -> plt.AST:
         # find main function
         # TODO can use more sophisiticated procedure here i.e. functions marked by comment
         main_fun: typing.Optional[InstanceType] = None
         for s in node.body:
-            if isinstance(s, FunctionDef) and s.name == "validator":
+            if isinstance(s, FunctionDef) and s.name == self.validator_function_name:
                 main_fun = s
-        assert main_fun is not None, "Could not find function named validator"
-        main_fun_typ = main_fun.typ
-        main_fun_typ_typ: FunctionType = main_fun_typ.typ
+        assert (
+            main_fun is not None
+        ), f"Could not find function named {self.validator_function_name}"
+        main_fun_typ: FunctionType = main_fun.typ.typ
         assert isinstance(
-            main_fun_typ_typ, FunctionType
-        ), "Variable named validator is not of type function"
+            main_fun_typ, FunctionType
+        ), f"Variable named {self.validator_function_name} is not of type function"
 
         # check if this is a contract written to double function
         enable_double_func_mint_spend = False
-        if len(main_fun_typ_typ.argtyps) >= 3 and self.force_three_params:
+        if len(main_fun_typ.argtyps) >= 3 and self.force_three_params:
             # check if is possible
-            second_last_arg = main_fun_typ_typ.argtyps[-2]
+            second_last_arg = main_fun_typ.argtyps[-2]
             assert isinstance(
                 second_last_arg, InstanceType
             ), "Can not pass Class into validator"
             if isinstance(second_last_arg.typ, UnionType):
                 possible_types = second_last_arg.typ.typs
             else:
                 possible_types = [second_last_arg.typ]
@@ -220,50 +222,56 @@
             if not enable_double_func_mint_spend:
                 _LOGGER.warning(
                     "The second argument to the validator function potentially has constructor id 0. The validator will not be able to double function as minting script and spending script."
                 )
 
         body = node.body + [
             TypedReturn(
-                value=Name(id="validator", typ=main_fun_typ, ctx=Load()),
-                typ=main_fun_typ_typ.rettyp,
+                value=Name(
+                    id=self.validator_function_name,
+                    typ=InstanceType(main_fun_typ),
+                    ctx=Load(),
+                ),
+                typ=InstanceType(main_fun_typ),
             )
         ]
 
         validator = plt.Lambda(
-            [f"p{i}" for i, _ in enumerate(main_fun_typ_typ.argtyps)],
-            transform_output_map(main_fun_typ_typ.rettyp)(
+            [f"p{i}" for i, _ in enumerate(main_fun_typ.argtyps)],
+            transform_output_map(main_fun_typ.rettyp)(
                 plt.Let(
                     [
                         (
                             "val",
-                            self.visit_sequence(body)(plt.Unit()),
+                            self.visit_sequence(body)(
+                                plt.ConstrData(plt.Integer(0), plt.EmptyDataList())
+                            ),
                         ),
                     ],
                     plt.Apply(
                         plt.Var("val"),
                         plt.Var("val"),
                         *[
                             transform_ext_params_map(a)(plt.Var(f"p{i}"))
-                            for i, a in enumerate(main_fun_typ_typ.argtyps)
+                            for i, a in enumerate(main_fun_typ.argtyps)
                         ],
                     ),
                 ),
             ),
         )
         if enable_double_func_mint_spend:
             validator = wrap_validator_double_function(
-                validator, pass_through=len(main_fun_typ_typ.argtyps) - 3
+                validator, pass_through=len(main_fun_typ.argtyps) - 3
             )
         elif self.force_three_params:
             # Error if the double function is enforced but not possible
             raise RuntimeError(
                 "The contract can not always detect if it was passed three or two parameters on-chain."
             )
-        cp = plt.Program("1.0.0", validator)
+        cp = plt.Program((1, 0, 0), validator)
         return cp
 
     def visit_Constant(self, node: TypedConstant) -> plt.AST:
         plt_type = ConstantMap.get(type(node.value))
         if plt_type is None:
             raise NotImplementedError(
                 f"Constants of type {type(node.value)} are not supported"
@@ -288,19 +296,29 @@
         assert isinstance(
             node.target, Name
         ), "Assignments to other things than names are not supported"
         assert isinstance(
             node.target.typ, InstanceType
         ), "Can only assign instances to instances"
         compiled_e = self.visit(node.value)
-        # we need to map this as it will originate from PlutusData
         # (\{STATEMONAD} -> (\x -> if (x ==b {self.visit(node.targets[0])}) then ({compiled_e} {STATEMONAD}) else ({STATEMONAD} x)))
-        return lambda x: plt.Let(
-            [(node.target.id, transform_ext_params_map(node.target.typ)(compiled_e))], x
-        )
+        val = compiled_e
+        if isinstance(node.value.typ, InstanceType) and isinstance(
+            node.value.typ.typ, AnyType
+        ):
+            # we need to map this as it will originate from PlutusData
+            # AnyType is the only type other than the builtin itself that can be cast to builtin values
+            val = transform_ext_params_map(node.target.typ)(val)
+        if isinstance(node.target.typ, InstanceType) and isinstance(
+            node.target.typ.typ, AnyType
+        ):
+            # we need to map this back as it will be treated as PlutusData
+            # AnyType is the only type other than the builtin itself that can be cast to from builtin values
+            val = transform_output_map(node.value.typ)(val)
+        return lambda x: plt.Let([(node.target.id, val)], x)
 
     def visit_Name(self, node: TypedName) -> plt.AST:
         # depending on load or store context, return the value of the variable or its name
         if not isinstance(node.ctx, Load):
             raise NotImplementedError(f"Context {node.ctx} not supported")
         if isinstance(node.typ, ClassType):
             # if this is not an instance but a class, call the constructor
@@ -340,15 +358,19 @@
         )
 
     def visit_FunctionDef(
         self, node: TypedFunctionDef
     ) -> typing.Callable[[plt.AST], plt.AST]:
         body = node.body.copy()
         # defaults to returning None if there is no return statement
-        compiled_body = self.visit_sequence(body)(plt.Unit())
+        if node.typ.typ.rettyp.typ == AnyType():
+            ret_val = plt.ConstrData(plt.Integer(0), plt.EmptyDataList())
+        else:
+            ret_val = plt.Unit()
+        compiled_body = self.visit_sequence(body)(ret_val)
         return lambda x: plt.Let(
             [
                 (
                     node.name,
                     plt.Lambda(
                         [node.name] + [a.arg for a in node.args.args],
                         compiled_body,
@@ -363,80 +385,128 @@
             self.visit(node.test),
             self.visit_sequence(node.body)(x),
             self.visit_sequence(node.orelse)(x),
         )
 
     def visit_Return(self, node: TypedReturn) -> typing.Callable[[plt.AST], plt.AST]:
         # Throw away the term we were passed, this is going to be the last!
-        return lambda x: self.visit(node.value)
+        compiled_return = self.visit(node.value)
+        if isinstance(node.typ.typ, AnyType):
+            # if the function returns generic data, wrap the function return value
+            compiled_return = transform_output_map(node.value.typ)(compiled_return)
+        return lambda _: compiled_return
 
     def visit_Pass(self, node: TypedPass) -> typing.Callable[[plt.AST], plt.AST]:
         return lambda x: x
 
     def visit_Subscript(self, node: TypedSubscript) -> plt.AST:
         assert isinstance(
             node.value.typ, InstanceType
         ), "Can only access elements of instances, not classes"
         if isinstance(node.value.typ.typ, TupleType):
             assert isinstance(
-                node.slice, Index
-            ), "Only single index slices for tuples are currently supported"
-            assert isinstance(
-                node.slice.value, Constant
+                node.slice, Constant
             ), "Only constant index access for tuples is supported"
             assert isinstance(
-                node.slice.value.value, int
+                node.slice.value, int
             ), "Only constant index integer access for tuples is supported"
-            index = node.slice.value.value
+            index = node.slice.value
             if index < 0:
                 index += len(node.value.typ.typ.typs)
             assert isinstance(node.ctx, Load), "Tuples are read-only"
             return plt.FunctionalTupleAccess(
                 self.visit(node.value),
                 index,
                 len(node.value.typ.typ.typs),
             )
-        if isinstance(node.value.typ.typ, ListType):
+        if isinstance(node.value.typ.typ, PairType):
+            assert isinstance(
+                node.slice, Constant
+            ), "Only constant index access for pairs is supported"
             assert isinstance(
-                node.slice, Index
-            ), "Only single index slices for lists are currently supported"
+                node.slice.value, int
+            ), "Only constant index integer access for pairs is supported"
+            index = node.slice.value
+            if index < 0:
+                index += 2
+            assert isinstance(node.ctx, Load), "Pairs are read-only"
             assert (
-                node.slice.value.typ == IntegerInstanceType
+                0 <= index < 2
+            ), f"Pairs only have 2 elements, index should be 0 or 1, is {node.slice.value}"
+            member_func = plt.FstPair if index == 0 else plt.SndPair
+            # the content of pairs is always Data, so we need to unwrap
+            member_typ = node.typ
+            return transform_ext_params_map(member_typ)(
+                member_func(
+                    self.visit(node.value),
+                ),
+            )
+        if isinstance(node.value.typ.typ, ListType):
+            assert (
+                node.slice.typ == IntegerInstanceType
             ), "Only single element list index access supported"
             return plt.Let(
                 [
                     ("l", self.visit(node.value)),
                     (
                         "raw_i",
-                        self.visit(node.slice.value),
+                        self.visit(node.slice),
                     ),
                     (
                         "i",
                         plt.Ite(
                             plt.LessThanInteger(plt.Var("raw_i"), plt.Integer(0)),
                             plt.AddInteger(
                                 plt.Var("raw_i"), plt.LengthList(plt.Var("l"))
                             ),
                             plt.Var("raw_i"),
                         ),
                     ),
                 ],
                 plt.IndexAccessList(plt.Var("l"), plt.Var("i")),
             )
+        elif isinstance(node.value.typ.typ, DictType):
+            dict_typ = node.value.typ.typ
+            if not isinstance(node.slice, Slice):
+                return plt.Let(
+                    [
+                        (
+                            "key",
+                            self.visit(node.slice),
+                        )
+                    ],
+                    transform_ext_params_map(dict_typ.value_typ)(
+                        plt.SndPair(
+                            plt.FindList(
+                                self.visit(node.value),
+                                plt.Lambda(
+                                    ["x"],
+                                    plt.EqualsData(
+                                        transform_output_map(dict_typ.key_typ)(
+                                            plt.Var("key")
+                                        ),
+                                        plt.FstPair(plt.Var("x")),
+                                    ),
+                                ),
+                                plt.TraceError("KeyError"),
+                            ),
+                        ),
+                    ),
+                )
         elif isinstance(node.value.typ.typ, ByteStringType):
-            if isinstance(node.slice, Index):
+            if not isinstance(node.slice, Slice):
                 return plt.Let(
                     [
                         (
                             "bs",
                             self.visit(node.value),
                         ),
                         (
                             "raw_ix",
-                            self.visit(node.slice.value),
+                            self.visit(node.slice),
                         ),
                         (
                             "ix",
                             plt.Ite(
                                 plt.LessThanInteger(plt.Var("raw_ix"), plt.Integer(0)),
                                 plt.AddInteger(
                                     plt.Var("raw_ix"),
@@ -504,15 +574,17 @@
                         plt.SliceByteString(
                             plt.Var("drop"),
                             plt.Var("take"),
                             plt.Var("bs"),
                         ),
                     ),
                 )
-        raise NotImplementedError(f"Could not implement subscript of {node}")
+        raise NotImplementedError(
+            f'Could not implement subscript "{node.slice}" of "{node.value}"'
+        )
 
     def visit_Tuple(self, node: TypedTuple) -> plt.AST:
         return plt.FunctionalTuple(*(self.visit(e) for e in node.elts))
 
     def visit_ClassDef(
         self, node: TypedClassDef
     ) -> typing.Callable[[plt.AST], plt.AST]:
@@ -610,43 +682,54 @@
                 empty_list_con,
             )
 
     def generic_visit(self, node: AST) -> plt.AST:
         raise NotImplementedError(f"Can not compile {node}")
 
 
-def compile(prog: AST, filename=None, force_three_params=False):
+def compile(
+    prog: AST,
+    filename=None,
+    force_three_params=False,
+    validator_function_name="validator",
+):
     rewrite_steps = [
         # Important to call this one first - it imports all further files
         RewriteImport(filename=filename),
         # Rewrites that simplify the python code
+        RewriteSubscript38(),
         RewriteTupleAssign(),
         RewriteImportPlutusData(),
         RewriteImportHashlib(),
         RewriteImportTyping(),
         RewriteForbiddenOverwrites(),
         RewriteImportDataclasses(),
         RewriteInjectBuiltins(),
         RewriteDuplicateAssignment(),
+        RewriteGuaranteedVariables(),
         # The type inference needs to be run after complex python operations were rewritten
         AggressiveTypeInferencer(),
         # Rewrites that circumvent the type inference or use its results
+        RewriteZeroAry(),
         RewriteInjectBuiltinsConstr(),
         RewriteRemoveTypeStuff(),
     ]
     for s in rewrite_steps:
         prog = s.visit(prog)
         prog = fix_missing_locations(prog)
 
     # from here on raw uplc may occur, so we dont attempt to fix locations
     compile_pipeline = [
         # Apply optimizations
         OptimizeRemoveDeadvars(),
-        # OptimizeVarlen(),
+        OptimizeRemoveDeadconstants(),
         OptimizeRemovePass(),
         # the compiler runs last
-        UPLCCompiler(force_three_params=force_three_params),
+        UPLCCompiler(
+            force_three_params=force_three_params,
+            validator_function_name=validator_function_name,
+        ),
     ]
     for s in compile_pipeline:
         prog = s.visit(prog)
 
     return prog
```

### Comparing `hebi-0.1.1.0.9.9/hebi/optimize/optimize_remove_deadvars.py` & `hebi-0.2.0.0.12.5/hebi/optimize/optimize_remove_deadvars.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from ast import *
 from copy import copy
 from collections import defaultdict
 
 from ..util import CompilingNodeVisitor, CompilingNodeTransformer
 from ..type_inference import INITIAL_SCOPE
+from ..typed_ast import TypedAnnAssign
 
 """
 Removes assignments to variables that are never read
 """
 
 
 class NameLoadCollector(CompilingNodeVisitor):
@@ -58,15 +59,17 @@
 
 class OptimizeRemoveDeadvars(CompilingNodeTransformer):
     step = "Removing unused variables"
 
     loaded_vars = None
     # names that are guaranteed to be available to the current node
     # this acts differently to the type inferencer! in particular, ite/while/for all produce their own scope
-    guaranteed_avail_names = [list(INITIAL_SCOPE.keys())]
+    guaranteed_avail_names = [
+        list(INITIAL_SCOPE.keys()) + ["isinstance", "Union", "Dict", "List"]
+    ]
 
     def guaranteed(self, name: str) -> bool:
         name = name
         for scope in reversed(self.guaranteed_avail_names):
             if name in scope:
                 return True
         return False
@@ -148,21 +151,23 @@
                 assert isinstance(
                     t, Name
                 ), "Need to have name for dead var remover to work"
                 self.set_guaranteed(t.id)
             return self.generic_visit(node)
         return Pass()
 
-    def visit_AnnAssign(self, node: AnnAssign):
+    def visit_AnnAssign(self, node: TypedAnnAssign):
         if (
             not isinstance(node.target, Name)
             or node.target.id in self.loaded_vars
             or not SafeOperationVisitor(sum(self.guaranteed_avail_names, [])).visit(
                 node.value
             )
+            # only upcasts are safe!
+            or not node.target.typ >= node.value.typ
         ):
             assert isinstance(
                 node.target, Name
             ), "Need to have assignments to name for dead var remover to work"
             self.set_guaranteed(node.target.id)
             return self.generic_visit(node)
         return Pass()
```

### Comparing `hebi-0.1.1.0.9.9/hebi/optimize/optimize_varlen.py` & `hebi-0.2.0.0.12.5/hebi/optimize/optimize_varlen.py`

 * *Files identical despite different names*

### Comparing `hebi-0.1.1.0.9.9/hebi/prelude.py` & `hebi-0.2.0.0.12.5/hebi/ledger/api_v2.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,50 +1,53 @@
+"""
+The PlutusV2 ledger API
+"""
 from dataclasses import dataclass
 from typing import Dict, List, Union
-from hashlib import sha256, sha3_256, blake2b
 
 from pycardano import Datum as Anything, PlutusData
 
+
 # Plutus V2
-@dataclass()
+@dataclass(unsafe_hash=True)
 class TxId(PlutusData):
     """
     A transaction id, a 64 bytes long hash of the transaction body (also called transaction hash).
 
     Example value: TxId(bytes.fromhex("842a4d37b036da6ab3c04331240e67d81746beb44f23ad79703e026705361956"))
     """
 
     tx_id: bytes
 
 
-@dataclass()
+@dataclass(unsafe_hash=True)
 class Nothing(PlutusData):
     """
     Nothing, can be used to signify non-importance of a parameter to a function
 
     Example value: Nothing()
     """
 
     # The maximimum constructor ID for simple cbor types, chosen to minimize probability of collision while keeping the corresponding cbor small
     CONSTR_ID = 6
 
 
-@dataclass()
+@dataclass(unsafe_hash=True)
 class TrueData(PlutusData):
     """
     A Datum that represents True in Haskell implementations.
     It is thus used as an encoding for True in the ScriptContext.
 
     Example value: TrueData()
     """
 
     CONSTR_ID = 0
 
 
-@dataclass()
+@dataclass(unsafe_hash=True)
 class FalseData(PlutusData):
     """
     A Datum that represents False in Haskell implementations.
     It is thus used as an encoding for False in the ScriptContext.
 
     Example value: FalseData()
     """
@@ -55,29 +58,29 @@
 # A Datum that represents a boolean value in Haskell implementations.
 # It is thus used as an encoding for booleans in the ScriptContext.
 #
 # Example value: TrueData()
 BoolData = Union[TrueData, FalseData]
 
 
-@dataclass()
+@dataclass(unsafe_hash=True)
 class TxOutRef(PlutusData):
     """
     A reference to a transaction output (hash/id + index)
     """
 
     id: TxId
     idx: int
 
 
 # A public key hash, used to identify signatures provided by a wallet
 PubKeyHash = bytes
 
 
-@dataclass()
+@dataclass(unsafe_hash=True)
 class PubKeyCredential(PlutusData):
     """
     Part of an address that is authenticated by a public key hash
 
     Example value: PubKeyCredential(bytes.fromhex("c06ddaad12fc4ded18e56feac72957c1aa75fce6096b40e63ec88274"))
     """
 
@@ -85,15 +88,15 @@
     credential_hash: PubKeyHash
 
 
 # A validator hash, used to identify signatures provided by a smart contract
 ValidatorHash = bytes
 
 
-@dataclass()
+@dataclass(unsafe_hash=True)
 class ScriptCredential(PlutusData):
     """
     Part of an address that is authenticated by a smart cotnract
 
     Example value: ScriptCredential(bytes.fromhex("c06ddaad12fc4ded18e56feac72957c1aa75fce6096b40e63ec88274"))
     """
 
@@ -101,25 +104,25 @@
     credential_hash: ValidatorHash
 
 
 # A credential, either smart contract or public key hash
 Credential = Union[PubKeyCredential, ScriptCredential]
 
 
-@dataclass()
+@dataclass(unsafe_hash=True)
 class StakingHash(PlutusData):
     """
     Indicates that the stake of this address is controlled by the associated credential
     """
 
     CONSTR_ID = 0
     value: Credential
 
 
-@dataclass()
+@dataclass(unsafe_hash=True)
 class StakingPtr(PlutusData):
     """
     Indicates that the stake of this address is controlled by the associated pointer.
 
     In an address, a chain pointer refers to a point of the chain containing a stake key registration certificate.
     A point is identified by the 3 coordinates in this object.
     """
@@ -133,36 +136,36 @@
     cert_index: int
 
 
 # Part of an address that controls who can delegate the stake associated with an address
 StakingCredential = Union[StakingHash, StakingPtr]
 
 
-@dataclass()
+@dataclass(unsafe_hash=True)
 class NoStakingCredential(PlutusData):
     """
     Indicates that this address has no staking credentials.
     Its funds can not be delegated.
     """
 
     CONSTR_ID = 1
 
 
-@dataclass()
+@dataclass(unsafe_hash=True)
 class SomeStakingCredential(PlutusData):
     """
     Indicates that this address has staking credentials.
     Its funds can be delegated by the credentialed user.
     """
 
     CONSTR_ID = 0
     staking_credential: StakingCredential
 
 
-@dataclass()
+@dataclass(unsafe_hash=True)
 class Address(PlutusData):
     """
     A Shelley address, consisting of a payment and staking credential
     """
 
     payment_credential: Credential
     staking_credential: Union[NoStakingCredential, SomeStakingCredential]
@@ -181,90 +184,90 @@
 # Lovelace is represented with policy id b"" and token name b""
 Value = Dict[PolicyId, Dict[TokenName, int]]
 
 # A hash of a Datum
 DatumHash = bytes
 
 
-@dataclass()
+@dataclass(unsafe_hash=True)
 class SomeDatumHash(PlutusData):
     """
     Indicates that there is a datum associated with this output, which has the given hash.
     """
 
     CONSTR_ID = 1
     datum_hash: DatumHash
 
 
-@dataclass()
+@dataclass(unsafe_hash=True)
 class SomeScriptHash(PlutusData):
     """
     Indicates that there is a script associated with this output, which has the given hash.
     """
 
     CONSTR_ID = 0
     script_hash: DatumHash
 
 
-# The abstract super type of any object in eopsin.
+# The abstract super type of any object in opshin.
 # Use if you don't know what kind of object is being passed or if it doesn't matter.
 BuiltinData = Anything
 
 
 # An abstract type annotation that something is supposed to be used as a redeemer.
 Redeemer = BuiltinData
 
 
 # An abstract type annotation that something is supposed to be used as a datum.
 Datum = BuiltinData
 
 
-@dataclass()
+@dataclass(unsafe_hash=True)
 class NoOutputDatum(PlutusData):
     """
     Indicates that there is no datum associated with an output
     """
 
     CONSTR_ID = 0
 
 
-@dataclass()
+@dataclass(unsafe_hash=True)
 class SomeOutputDatumHash(PlutusData):
     """
     Indicates that there is an datum associated with an output, which has the attached hash
     """
 
     CONSTR_ID = 1
     datum_hash: DatumHash
 
 
-@dataclass()
+@dataclass(unsafe_hash=True)
 class SomeOutputDatum(PlutusData):
     """
     Indicates that there is an datum associated with an output, which is inlined and equal to the attached datum
     """
 
     CONSTR_ID = 2
     datum: Datum
 
 
 # Possible cases of datum association with an output
 OutputDatum = Union[NoOutputDatum, SomeOutputDatumHash, SomeOutputDatum]
 
 
-@dataclass()
+@dataclass(unsafe_hash=True)
 class NoScriptHash(PlutusData):
     """
     Indicates that there is no script associated with an output
     """
 
     CONSTR_ID = 1
 
 
-@dataclass()
+@dataclass(unsafe_hash=True)
 class TxOut(PlutusData):
     """
     The plutus representation of an transaction output, consisting of
     - address: address owning this output
     - value: tokens associated with this output
     - datum: datum associated with this output
     - reference_script: reference script associated with this output
@@ -272,63 +275,63 @@
 
     address: Address
     value: Value
     datum: OutputDatum
     reference_script: Union[NoScriptHash, SomeScriptHash]
 
 
-@dataclass()
+@dataclass(unsafe_hash=True)
 class TxInInfo(PlutusData):
     """
     The plutus representation of an transaction output, that is consumed by the transaction.
     """
 
     out_ref: TxOutRef
     resolved: TxOut
 
 
-@dataclass()
+@dataclass(unsafe_hash=True)
 class DCertDelegRegKey(PlutusData):
     CONSTR_ID = 0
     value: StakingCredential
 
 
-@dataclass()
+@dataclass(unsafe_hash=True)
 class DCertDelegDeRegKey(PlutusData):
     CONSTR_ID = 1
     value: StakingCredential
 
 
-@dataclass()
+@dataclass(unsafe_hash=True)
 class DCertDelegDelegate(PlutusData):
     CONSTR_ID = 2
     delegator: StakingCredential
     delegatee: PubKeyHash
 
 
-@dataclass()
+@dataclass(unsafe_hash=True)
 class DCertPoolRegister(PlutusData):
     CONSTR_ID = 3
     pool_id: PubKeyHash
     pool_vfr: PubKeyHash
 
 
-@dataclass()
+@dataclass(unsafe_hash=True)
 class DCertPoolRetire(PlutusData):
     CONSTR_ID = 4
     retirement_certificate: PubKeyHash
     epoch: int
 
 
-@dataclass()
+@dataclass(unsafe_hash=True)
 class DCertGenesis(PlutusData):
     CONSTR_ID = 5
 
 
-@dataclass()
+@dataclass(unsafe_hash=True)
 class DCertMir(PlutusData):
     CONSTR_ID = 6
 
 
 DCert = Union[
     DCertDelegRegKey,
     DCertDelegDeRegKey,
@@ -339,115 +342,115 @@
     DCertMir,
 ]
 
 
 POSIXTime = int
 
 
-@dataclass()
+@dataclass(unsafe_hash=True)
 class NegInfPOSIXTime(PlutusData):
     """
     Negative infinite POSIX time, used to indicate that there is no lower bound for the execution of this transaction
     """
 
     CONSTR_ID = 0
 
 
-@dataclass()
+@dataclass(unsafe_hash=True)
 class FinitePOSIXTime(PlutusData):
     """
     Finite POSIX time, used to indicate that there is a lower or upper bound for the execution of this transaction
     """
 
     CONSTR_ID = 1
     time: POSIXTime
 
 
-@dataclass()
+@dataclass(unsafe_hash=True)
 class PosInfPOSIXTime(PlutusData):
     """
     Infinite POSIX time, used to indicate that there is no upper bound for the execution of this transaction
     """
 
     CONSTR_ID = 2
 
 
 ExtendedPOSIXTime = Union[NegInfPOSIXTime, FinitePOSIXTime, PosInfPOSIXTime]
 
 
-@dataclass()
+@dataclass(unsafe_hash=True)
 class UpperBoundPOSIXTime(PlutusData):
     """
     Upper bound for the execution of this transaction
     """
 
     CONSTR_ID = 0
     limit: ExtendedPOSIXTime
     closed: BoolData
 
 
-@dataclass()
+@dataclass(unsafe_hash=True)
 class LowerBoundPOSIXTime(PlutusData):
     """
     Lower bound for the execution of this transaction
     """
 
     CONSTR_ID = 0
     limit: ExtendedPOSIXTime
     closed: BoolData
 
 
-@dataclass()
+@dataclass(unsafe_hash=True)
 class POSIXTimeRange(PlutusData):
     """
     Time range in which this transaction can be executed
     """
 
     lower_bound: LowerBoundPOSIXTime
     upper_bound: UpperBoundPOSIXTime
 
 
-@dataclass()
+@dataclass(unsafe_hash=True)
 class Minting(PlutusData):
     """
     Script purpose indicating that the given policy id is being minted or burned
     """
 
     CONSTR_ID = 0
     policy_id: PolicyId
 
 
-@dataclass()
+@dataclass(unsafe_hash=True)
 class Spending(PlutusData):
     """
     Script purpose indicating that the given transaction output is being spent, which is
     owned by the invoked contract
     """
 
     CONSTR_ID = 1
     tx_out_ref: TxOutRef
 
 
-@dataclass()
+@dataclass(unsafe_hash=True)
 class Rewarding(PlutusData):
     CONSTR_ID = 2
     staking_credential: StakingCredential
 
 
-@dataclass()
+@dataclass(unsafe_hash=True)
 class Certifying(PlutusData):
     CONSTR_ID = 3
     d_cert: DCert
 
 
 # The reason that this script is being invoked
 ScriptPurpose = Union[Minting, Spending, Rewarding, Certifying]
 
 
-@dataclass()
+@dataclass(unsafe_hash=True)
 class TxInfo(PlutusData):
     """
     A complex agglomeration of everything that could be of interest to the executed script, regarding the transaction
     that invoked the script
     """
 
     inputs: List[TxInInfo]
@@ -460,75 +463,15 @@
     valid_range: POSIXTimeRange
     signatories: List[PubKeyHash]
     redeemers: Dict[ScriptPurpose, Redeemer]
     data: Dict[DatumHash, Datum]
     id: TxId
 
 
-@dataclass()
+@dataclass(unsafe_hash=True)
 class ScriptContext(PlutusData):
     """
     Auxiliary information about the transaction and reason for invocation of the called script.
     """
 
     tx_info: TxInfo
     purpose: ScriptPurpose
-
-
-@dataclass()
-class Token(PlutusData):
-    """
-    A token, represented by policy id and token name
-    """
-
-    policy_id: PolicyId
-    token_name: TokenName
-
-
-# Used to indicate that this contract does not expect a redeemer
-NoRedeemer = Nothing
-
-### Optimized methods for handling tokens at addresses
-
-
-def all_tokens_unlocked_from_address(
-    txins: List[TxInInfo], address: Address, token: Token
-) -> int:
-    """Returns how many tokens of specified type are unlocked from given address"""
-    return sum(
-        [
-            txi.resolved.value.get(token.policy_id, {b"": 0}).get(token.token_name, 0)
-            for txi in txins
-            if txi.resolved.address == address
-        ]
-    )
-
-
-def all_tokens_locked_at_address_with_datum(
-    txouts: List[TxOut], address: Address, token: Token, output_datum: OutputDatum
-) -> int:
-    """Returns how many tokens of specified type are locked at then given address with the specified datum"""
-    return sum(
-        [
-            txo.value.get(token.policy_id, {b"": 0}).get(token.token_name, 0)
-            for txo in txouts
-            if txo.address == address and txo.datum == output_datum
-        ]
-    )
-
-
-def all_tokens_locked_at_address(
-    txouts: List[TxOut], address: Address, token: Token
-) -> int:
-    """Returns how many tokens of specified type are locked at the given address"""
-    return sum(
-        [
-            txo.value.get(token.policy_id, {b"": 0}).get(token.token_name, 0)
-            for txo in txouts
-            if txo.address == address
-        ]
-    )
-
-
-def resolve_spent_utxo(txins: List[TxInInfo], p: Spending) -> TxOut:
-    """Returns the UTxO whose spending should be validated"""
-    return [txi.resolved for txi in txins if txi.out_ref == p.tx_out_ref][0]
```

### Comparing `hebi-0.1.1.0.9.9/hebi/rewrite/rewrite_duplicate_assignment.py` & `hebi-0.2.0.0.12.5/hebi/rewrite/rewrite_duplicate_assignment.py`

 * *Files identical despite different names*

### Comparing `hebi-0.1.1.0.9.9/hebi/rewrite/rewrite_forbidden_overwrites.py` & `hebi-0.2.0.0.12.5/hebi/rewrite/rewrite_forbidden_overwrites.py`

 * *Files identical despite different names*

### Comparing `hebi-0.1.1.0.9.9/hebi/rewrite/rewrite_import.py` & `hebi-0.2.0.0.12.5/hebi/rewrite/rewrite_import.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import ast
+
 import importlib
 import importlib.util
 import pathlib
 import typing
 import sys
 from ast import *
 
@@ -36,14 +38,23 @@
     sys.modules[absolute_name] = module
     spec.loader.exec_module(module)
     if path is not None:
         setattr(parent_module, child_name, module)
     return module
 
 
+class RewriteLocation(CompilingNodeTransformer):
+    def __init__(self, orig_node):
+        self.orig_node = orig_node
+
+    def visit(self, node):
+        node = ast.copy_location(node, self.orig_node)
+        return super().visit(node)
+
+
 class RewriteImport(CompilingNodeTransformer):
     step = "Resolving imports"
 
     def __init__(self, filename=None, package=None):
         self.filename = filename
         self.package = package
 
@@ -70,11 +81,15 @@
         module_file = pathlib.Path(module.__file__)
         assert (
             module_file.suffix == ".py"
         ), "The import must import a single python file."
         # visit the imported file again - make sure that recursive imports are resolved accordingly
         with module_file.open("r") as fp:
             module_content = fp.read()
+        resolved = parse(module_content, filename=module_file.name)
+        # annotate this to point to the original line number!
+        RewriteLocation(node).visit(resolved)
+        # recursively import all statements there
         recursively_resolved: Module = RewriteImport(
             filename=str(module_file), package=module.__package__
-        ).visit(parse(module_content, filename=module_file.name))
+        ).visit(resolved)
         return recursively_resolved.body
```

### Comparing `hebi-0.1.1.0.9.9/hebi/rewrite/rewrite_import_dataclasses.py` & `hebi-0.2.0.0.12.5/hebi/rewrite/rewrite_import_dataclasses.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,18 +31,21 @@
 
     def visit_ClassDef(self, node: ClassDef) -> ClassDef:
         assert (
             self.imports_dataclasses
         ), "dataclasses must be imported in order to use datum classes"
         assert (
             len(node.decorator_list) == 1
-        ), "Class definitions must have no decorators but @dataclass()"
+        ), "Class definitions must have the decorator @dataclass"
+        if isinstance(node.decorator_list[0], Call):
+            node_decorator = node.decorator_list[0].func
+        elif isinstance(node.decorator_list[0], Name):
+            node_decorator = node.decorator_list[0]
+        else:
+            raise AssertionError("Class definitions must have the decorator @dataclass")
         assert isinstance(
-            node.decorator_list[0], Call
-        ), "Class definitions must have no decorators but @dataclass()"
-        assert isinstance(
-            node.decorator_list[0].func, Name
-        ), "Class definitions must have no decorators but @dataclass()"
+            node_decorator, Name
+        ), "Class definitions must have the decorator @dataclass"
         assert (
-            node.decorator_list[0].func.id == "dataclass"
-        ), "Class definitions must have no decorators but @dataclass()"
+            node_decorator.id == "dataclass"
+        ), "Class definitions must have the decorator @dataclass"
         return node
```

### Comparing `hebi-0.1.1.0.9.9/hebi/rewrite/rewrite_import_hashlib.py` & `hebi-0.2.0.0.12.5/hebi/rewrite/rewrite_import_hashlib.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,17 @@
         raise NotImplementedError("HashType only has attribute 'digest'")
 
     def attribute(self, attr) -> plt.AST:
         if attr == "digest":
             return plt.Lambda(["self"], plt.Var("self"))
         raise NotImplementedError("HashType only has attribute 'digest'")
 
+    def __ge__(self, other):
+        return isinstance(other, HashType)
+
 
 HashInstanceType = InstanceType(HashType())
 
 
 class PythonHashlib(Enum):
     sha256 = plt.Lambda(["_", "x"], plt.Lambda(["_"], plt.Sha2_256(plt.Var("x"))))
     sha3_256 = plt.Lambda(["_", "x"], plt.Lambda(["_"], plt.Sha3_256(plt.Var("x"))))
```

### Comparing `hebi-0.1.1.0.9.9/hebi/rewrite/rewrite_import_plutusdata.py` & `hebi-0.2.0.0.12.5/hebi/rewrite/rewrite_import_plutusdata.py`

 * *Files identical despite different names*

### Comparing `hebi-0.1.1.0.9.9/hebi/rewrite/rewrite_import_typing.py` & `hebi-0.2.0.0.12.5/hebi/rewrite/rewrite_import_typing.py`

 * *Files identical despite different names*

### Comparing `hebi-0.1.1.0.9.9/hebi/rewrite/rewrite_inject_builtin_constr.py` & `hebi-0.2.0.0.12.5/hebi/rewrite/rewrite_inject_builtin_constr.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
     def visit_Module(self, node: TypedModule) -> TypedModule:
         additional_assigns = []
         for t, tname in [
             (ByteStringType(), bytes.__name__),
             (IntegerType(), int.__name__),
             (StringType(), str.__name__),
+            (BoolType(), bool.__name__),
         ]:
             typ = t.constr_type()
             if isinstance(typ.typ, PolymorphicFunctionType):
                 # skip polymorphic functions
                 continue
             additional_assigns.append(
                 TypedAssign(
```

### Comparing `hebi-0.1.1.0.9.9/hebi/rewrite/rewrite_inject_builtins.py` & `hebi-0.2.0.0.12.5/hebi/rewrite/rewrite_inject_builtins.py`

 * *Files identical despite different names*

### Comparing `hebi-0.1.1.0.9.9/hebi/rewrite/rewrite_remove_type_stuff.py` & `hebi-0.2.0.0.12.5/hebi/rewrite/rewrite_remove_type_stuff.py`

 * *Files identical despite different names*

### Comparing `hebi-0.1.1.0.9.9/hebi/rewrite/rewrite_tuple_assign.py` & `hebi-0.2.0.0.12.5/hebi/rewrite/rewrite_tuple_assign.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from copy import copy
+
 import typing
 from ast import *
 
 from ..util import CompilingNodeTransformer
 
 """
 Rewrites all occurences of assignments to tuples to assignments to single values
@@ -21,15 +23,43 @@
         assignments = [Assign([Name(f"{uid}_tup", Store())], self.visit(node.value))]
         for i, t in enumerate(node.targets[0].elts):
             assignments.append(
                 Assign(
                     [t],
                     Subscript(
                         value=Name(f"{uid}_tup", Load()),
-                        slice=Index(value=Constant(i)),
+                        slice=Constant(i),
                         ctx=Load(),
                     ),
                 )
             )
         # recursively resolve multiple layers of tuples
         transformed = sum([self.visit(a) for a in assignments], [])
         return transformed
+
+    def visit_For(self, node: For) -> For:
+        # rewrite deconstruction in for loops
+        if not isinstance(node.target, Tuple):
+            return self.generic_visit(node)
+        new_for = copy(node)
+        new_for.iter = self.visit(node.iter)
+        uid = self.unique_id
+        self.unique_id += 1
+        # write the tuple into a singleton variable
+        new_for.target = Name(f"{uid}_tup", Store())
+        assignments = []
+        # iteratively assign the deconstructed parts to the original variable names
+        for i, t in enumerate(node.target.elts):
+            assignments.append(
+                Assign(
+                    [t],
+                    Subscript(
+                        value=Name(f"{uid}_tup", Load()),
+                        slice=Constant(i),
+                        ctx=Load(),
+                    ),
+                )
+            )
+        new_for.body = assignments + node.body
+        # recursively resolve multiple layers of tuples
+        # further layers should be handled by the normal tuple assignment though
+        return self.visit(new_for)
```

### Comparing `hebi-0.1.1.0.9.9/hebi/tests/test_builtins.py` & `hebi-0.2.0.0.12.5/hebi/tests/test_builtins.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-import frozendict
-import hypothesis
 import unittest
 
-from uplc import ast as uplc, eval as uplc_eval
+import parameterized
 from hypothesis import example, given
 from hypothesis import strategies as st
-import parameterized
+from uplc import ast as uplc, eval as uplc_eval
 
 from .. import compiler
 
 
 class BuiltinTest(unittest.TestCase):
     @given(xs=st.lists(st.booleans()))
     def test_all(self, xs):
@@ -382,7 +380,24 @@
         code = code.compile()
         f = code.term
         # UPLC lambdas may only take one argument at a time, so we evaluate by repeatedly applying
         for d in [uplc.PlutusList([uplc.PlutusInteger(x) for x in xs])]:
             f = uplc.Apply(f, d)
         ret = [x.value for x in uplc_eval(f).value]
         self.assertEqual(ret, list(reversed(xs)), "reversed returned wrong value")
+
+    @given(x=st.integers())
+    def test_bool_constr_int(self, x):
+        # this tests that errors that are caused by assignments are actually triggered at the time of assigning
+        source_code = """
+def validator(x: int) -> bool:
+    return bool(x)
+        """
+        ast = compiler.parse(source_code)
+        code = compiler.compile(ast)
+        code = code.compile()
+        f = code.term
+        # UPLC lambdas may only take one argument at a time, so we evaluate by repeatedly applying
+        for d in [uplc.PlutusInteger(x)]:
+            f = uplc.Apply(f, d)
+        ret = bool(uplc_eval(f).value)
+        self.assertEqual(ret, bool(x), "reversed returned wrong value")
```

### Comparing `hebi-0.1.1.0.9.9/hebi/tests/test_misc.py` & `hebi-0.2.0.0.12.5/hebi/tests/test_misc.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-import frozendict
-import hypothesis
 import unittest
 
-from uplc import ast as uplc, eval as uplc_eval
-from hypothesis import example, given
+import frozendict
+from hypothesis import given
 from hypothesis import strategies as st
 from parameterized import parameterized
+from uplc import ast as uplc, eval as uplc_eval
 
-from .. import compiler, prelude, type_inference
 from ..util import CompilerError
+from .. import compiler, prelude
 
 
 def fib(n):
     a, b = 0, 1
     for _ in range(n):
         a, b = b, a + b
     return a
@@ -27,15 +26,15 @@
         code = compiler.compile(ast)
         code = code.compile()
         f = code.term
         # UPLC lambdas may only take one argument at a time, so we evaluate by repeatedly applying
         for d in [uplc.PlutusInteger(20), uplc.PlutusInteger(22), uplc.BuiltinUnit()]:
             f = uplc.Apply(f, d)
         ret = uplc_eval(f)
-        self.assertEqual(ret, uplc.BuiltinUnit())
+        self.assertEqual(ret, uplc.PlutusConstr(0, []))
 
     def test_assert_sum_contract_fail(self):
         input_file = "examples/smart_contracts/assert_sum.py"
         with open(input_file) as fp:
             source_code = fp.read()
         ast = compiler.parse(source_code)
         code = compiler.compile(ast)
@@ -161,33 +160,14 @@
             f = uplc.Apply(f, d)
         ret = uplc_eval(f)
         self.assertEqual(
             uplc.PlutusInteger(fib(n)),
             ret,
         )
 
-    @parameterized.expand(
-        [
-            (
-                "d8799fd8799f9fd8799fd8799fd8799f582055d353acacaab6460b37ed0f0e3a1a0aabf056df4a7fa1e265d21149ccacc527ff01ffd8799fd8799fd87a9f581cdbe769758f26efb21f008dc097bb194cffc622acc37fcefc5372eee3ffd87a80ffa140a1401a00989680d87a9f5820dfab81872ce2bbe6ee5af9bbfee4047f91c1f57db5e30da727d5fef1e7f02f4dffd87a80ffffff809fd8799fd8799fd8799f581cdc315c289fee4484eda07038393f21dc4e572aff292d7926018725c2ffd87a80ffa140a14000d87980d87a80ffffa140a14000a140a1400080a0d8799fd8799fd87980d87a80ffd8799fd87b80d87a80ffff80a1d87a9fd8799fd8799f582055d353acacaab6460b37ed0f0e3a1a0aabf056df4a7fa1e265d21149ccacc527ff01ffffd87980a15820dfab81872ce2bbe6ee5af9bbfee4047f91c1f57db5e30da727d5fef1e7f02f4dd8799f581cdc315c289fee4484eda07038393f21dc4e572aff292d7926018725c2ffd8799f5820746957f0eb57f2b11119684e611a98f373afea93473fefbb7632d579af2f6259ffffd87a9fd8799fd8799f582055d353acacaab6460b37ed0f0e3a1a0aabf056df4a7fa1e265d21149ccacc527ff01ffffff"
-            ),
-            (
-                "d8799fd8799f9fd8799fd8799fd8799f582055d353acacaab6460b37ed0f0e3a1a0aabf056df4a7fa1e265d21149ccacc527ff01ffd8799fd8799fd87a9f581cdbe769758f26efb21f008dc097bb194cffc622acc37fcefc5372eee3ffd87a80ffa140a1401a00989680d87a9f5820dfab81872ce2bbe6ee5af9bbfee4047f91c1f57db5e30da727d5fef1e7f02f4dffd87a80ffffff809fd8799fd8799fd8799f581cdc315c289fee4484eda07038393f21dc4e572aff292d7926018725c2ffd87a80ffa140a14000d87980d87a80ffffa140a14000a140a1400080a0d8799fd8799fd87a9f1b000001836ac117d8ffd87a80ffd8799fd87b80d87a80ffff80a1d87a9fd8799fd8799f582055d353acacaab6460b37ed0f0e3a1a0aabf056df4a7fa1e265d21149ccacc527ff01ffffd87980a15820dfab81872ce2bbe6ee5af9bbfee4047f91c1f57db5e30da727d5fef1e7f02f4dd8799f581cdc315c289fee4484eda07038393f21dc4e572aff292d7926018725c2ffd8799f5820797a1e1720b63621c6b185088184cb8e23af6e46b55bd83e7a91024c823a6c2affffd87a9fd8799fd8799f582055d353acacaab6460b37ed0f0e3a1a0aabf056df4a7fa1e265d21149ccacc527ff01ffffff"
-            ),
-            (
-                "d8799fd8799f9fd8799fd8799fd8799f582055d353acacaab6460b37ed0f0e3a1a0aabf056df4a7fa1e265d21149ccacc527ff01ffd8799fd8799fd87a9f581cdbe769758f26efb21f008dc097bb194cffc622acc37fcefc5372eee3ffd87a80ffa140a1401a00989680d87a9f5820dfab81872ce2bbe6ee5af9bbfee4047f91c1f57db5e30da727d5fef1e7f02f4dffd87a80ffffff809fd8799fd8799fd8799f581cdc315c289fee4484eda07038393f21dc4e572aff292d7926018725c2ffd87a80ffa140a14000d87980d87a80ffd8799fd8799fd8799f581cdc315c289fee4484eda07038393f21dc4e572aff292d7926018725c2ffd87a80ffa140a1401a000f4240d87980d87a80ffffa140a14000a140a1400080a0d8799fd8799fd87a9f1b000001836ac117d8ffd87a80ffd8799fd87b80d87a80ffff9f581cdc315c289fee4484eda07038393f21dc4e572aff292d7926018725c2ffa1d87a9fd8799fd8799f582055d353acacaab6460b37ed0f0e3a1a0aabf056df4a7fa1e265d21149ccacc527ff01ffffd87980a15820dfab81872ce2bbe6ee5af9bbfee4047f91c1f57db5e30da727d5fef1e7f02f4dd8799f581cdc315c289fee4484eda07038393f21dc4e572aff292d7926018725c2ffd8799f5820c17c32f6433ae22c2acaebfb796bbfaee3993ff7ebb58a2bac6b4a3bdd2f6d28ffffd87a9fd8799fd8799f582055d353acacaab6460b37ed0f0e3a1a0aabf056df4a7fa1e265d21149ccacc527ff01ffffff"
-            ),
-        ]
-    )
-    def test_script_context_repr_correct(self, p):
-        # Make sure that this parses correctly and does not throw an error
-        # Note that this was extracted from a PlutusV2 invocation
-        # in increasing complexity...
-        prelude.ScriptContext.from_cbor(p)
-
     def test_gift_contract_succeed(self):
         input_file = "examples/smart_contracts/gift.py"
         with open(input_file) as fp:
             source_code = fp.read()
         ast = compiler.parse(source_code)
         code = compiler.compile(ast)
         code = code.compile()
@@ -211,15 +191,15 @@
                         "d8799fd8799f9fd8799fd8799fd8799f582055d353acacaab6460b37ed0f0e3a1a0aabf056df4a7fa1e265d21149ccacc527ff01ffd8799fd8799fd87a9f581cdbe769758f26efb21f008dc097bb194cffc622acc37fcefc5372eee3ffd87a80ffa140a1401a00989680d87a9f5820dfab81872ce2bbe6ee5af9bbfee4047f91c1f57db5e30da727d5fef1e7f02f4dffd87a80ffffff809fd8799fd8799fd8799f581cdc315c289fee4484eda07038393f21dc4e572aff292d7926018725c2ffd87a80ffa140a14000d87980d87a80ffd8799fd8799fd8799f581cdc315c289fee4484eda07038393f21dc4e572aff292d7926018725c2ffd87a80ffa140a1401a000f4240d87980d87a80ffffa140a14000a140a1400080a0d8799fd8799fd87a9f1b000001836ac117d8ffd87a80ffd8799fd87b80d87a80ffff9f581cdc315c289fee4484eda07038393f21dc4e572aff292d7926018725c2ffa1d87a9fd8799fd8799f582055d353acacaab6460b37ed0f0e3a1a0aabf056df4a7fa1e265d21149ccacc527ff01ffffd87980a15820dfab81872ce2bbe6ee5af9bbfee4047f91c1f57db5e30da727d5fef1e7f02f4dd8799f581cdc315c289fee4484eda07038393f21dc4e572aff292d7926018725c2ffd8799f5820c17c32f6433ae22c2acaebfb796bbfaee3993ff7ebb58a2bac6b4a3bdd2f6d28ffffd87a9fd8799fd8799f582055d353acacaab6460b37ed0f0e3a1a0aabf056df4a7fa1e265d21149ccacc527ff01ffffff"
                     )
                 )
             ),
         ]:
             f = uplc.Apply(f, d)
         ret = uplc_eval(f)
-        self.assertEqual(ret, uplc.BuiltinUnit())
+        self.assertEqual(ret, uplc.PlutusConstr(0, []))
 
     def test_gift_contract_fail(self):
         input_file = "examples/smart_contracts/gift.py"
         with open(input_file) as fp:
             source_code = fp.read()
         ast = compiler.parse(source_code)
         code = compiler.compile(ast)
@@ -393,43 +373,17 @@
             failed = True
         self.assertTrue(failed, "Machine did validate the content")
 
     def test_overopt_removedeadvar(self):
         # this tests that errors that are caused by assignments are actually triggered at the time of assigning
         source_code = """
 from hebi.prelude import *
-def validator(x: Token) -> bool:
-    a = x.policy_id
-    return True
-        """
-        ast = compiler.parse(source_code)
-        code = compiler.compile(ast)
-        code = code.compile()
-        f = code.term
-        # UPLC lambdas may only take one argument at a time, so we evaluate by repeatedly applying
-        try:
-            for d in [
-                uplc.PlutusConstr(0, []),
-            ]:
-                f = uplc.Apply(f, d)
-            ret = uplc_eval(f)
-            failed = False
-        except Exception as e:
-            failed = True
-        self.assertTrue(failed, "Machine did validate the content")
 
-    def test_opt_shared_var(self):
-        # this tests that errors that are caused by assignments are actually triggered at the time of assigning
-        source_code = """
-from hebi.prelude import *
 def validator(x: Token) -> bool:
-    if False:
-        y = x
-    else:
-        a = y
+    a = x.policy_id
     return True
         """
         ast = compiler.parse(source_code)
         code = compiler.compile(ast)
         code = code.compile()
         f = code.term
         # UPLC lambdas may only take one argument at a time, so we evaluate by repeatedly applying
@@ -664,7 +618,239 @@
         """
         ast = compiler.parse(source_code)
         try:
             code = compiler.compile(ast)
             self.fail("Compilation passed")
         except CompilerError:
             pass
+
+    def test_typecast_anything_int(self):
+        source_code = """
+def validator(x: Anything) -> int:
+    b: int = x
+    return b
+"""
+        ast = compiler.parse(source_code)
+        code = compiler.compile(ast).compile()
+        res = uplc_eval(uplc.Apply(code, uplc.PlutusInteger(0))).value
+        self.assertEqual(res, 0)
+
+    def test_typecast_int_anything(self):
+        # this should compile, it happens implicitly anyways when calling a function with Any parameters
+        source_code = """
+def validator(x: int) -> Anything:
+    b: Anything = x
+    return b
+"""
+        ast = compiler.parse(source_code)
+        code = compiler.compile(ast).compile()
+        res = uplc_eval(uplc.Apply(code, uplc.PlutusInteger(0))).value
+        self.assertEqual(res, 0)
+
+    def test_typecast_int_anything_int(self):
+        source_code = """
+def validator(x: int) -> Anything:
+    b: Anything = x
+    c: int = b
+    return c + 1
+"""
+        ast = compiler.parse(source_code)
+        code = compiler.compile(ast).compile()
+        res = uplc_eval(uplc.Apply(code, uplc.PlutusInteger(0))).value
+        self.assertEqual(res, 1)
+
+    def test_typecast_anything_int_anything(self):
+        source_code = """
+def validator(x: Anything) -> Anything:
+    b: int = x
+    c: Anything = b + 1
+    return c
+"""
+        ast = compiler.parse(source_code)
+        code = compiler.compile(ast).compile()
+        res = uplc_eval(uplc.Apply(code, uplc.PlutusInteger(0))).value
+        self.assertEqual(res, 1)
+
+    @unittest.expectedFailure
+    def test_typecast_int_str(self):
+        # this should compile, the two types are unrelated and there is no meaningful way to cast them either direction
+        source_code = """
+def validator(x: int) -> str:
+    b: str = x
+    return b
+"""
+        ast = compiler.parse(source_code)
+        code = compiler.compile(ast)
+
+    def test_typecast_int_int(self):
+        source_code = """
+def validator(x: int) -> int:
+    b: int = x
+    return b
+"""
+        ast = compiler.parse(source_code)
+        code = compiler.compile(ast).compile()
+        res = uplc_eval(uplc.Apply(code, uplc.PlutusInteger(0))).value
+        self.assertEqual(res, 0)
+
+    def test_zero_ary(self):
+        source_code = """
+def a() -> None:
+    assert False, "Executed a"
+
+def validator(x: None) -> None:
+    b = a
+    if False:
+        b()
+"""
+        ast = compiler.parse(source_code)
+        code = compiler.compile(ast).compile()
+        res = uplc_eval(uplc.Apply(code, uplc.PlutusInteger(0)))
+
+    @unittest.expectedFailure
+    def test_zero_ary_exec(self):
+        source_code = """
+def a() -> None:
+    assert False, "Executed a"
+
+def validator(x: None) -> None:
+    b = a
+    if True:
+        b()
+"""
+        ast = compiler.parse(source_code)
+        code = compiler.compile(ast).compile()
+        res = uplc_eval(uplc.Apply(code, uplc.PlutusInteger(0)))
+
+    def test_zero_ary_method(self):
+        source_code = """
+def validator(x: None) -> None:
+    b = b"\\xFF".decode
+    if False:
+        b()
+"""
+        ast = compiler.parse(source_code)
+        code = compiler.compile(ast).compile()
+        res = uplc_eval(uplc.Apply(code, uplc.PlutusInteger(0)))
+
+    @unittest.expectedFailure
+    def test_zero_ary_method_exec(self):
+        source_code = """
+def validator(x: None) -> None:
+    b = b"\\xFF".decode
+    if True:
+        b()
+"""
+        ast = compiler.parse(source_code)
+        code = compiler.compile(ast).compile()
+        res = uplc_eval(uplc.Apply(code, uplc.PlutusInteger(0)))
+
+    def test_return_anything(self):
+        source_code = """
+from hebi.prelude import *
+
+def validator() -> Anything:
+    return b""
+"""
+        ast = compiler.parse(source_code)
+        code = compiler.compile(ast).compile()
+        res = uplc_eval(uplc.Apply(code, uplc.PlutusConstr(0, [])))
+        self.assertEqual(res, uplc.PlutusByteString(b""))
+
+    def test_no_return_annotation(self):
+        source_code = """
+from hebi.prelude import *
+
+def validator():
+    return b""
+"""
+        ast = compiler.parse(source_code)
+        code = compiler.compile(ast).compile()
+        res = uplc_eval(uplc.Apply(code, uplc.PlutusConstr(0, [])))
+        self.assertEqual(res, uplc.PlutusByteString(b""))
+
+    def test_no_parameter_annotation(self):
+        source_code = """
+from hebi.prelude import *
+
+def validator(a) -> bytes:
+    b: bytes = a
+    return b
+"""
+        ast = compiler.parse(source_code)
+        code = compiler.compile(ast).compile()
+        res = uplc_eval(uplc.Apply(code, uplc.PlutusByteString(b"")))
+        self.assertEqual(res, uplc.PlutusByteString(b""))
+
+    def test_nested_deconstruction(self):
+        source_code = """
+def validator(xs) -> int:
+    a, ((b, c), d) = (1, ((2, 3), 4))
+    return a + b + c + d
+"""
+        ast = compiler.parse(source_code)
+        code = compiler.compile(ast)
+        code = code.compile()
+        f = code.term
+        # UPLC lambdas may only take one argument at a time, so we evaluate by repeatedly applying
+        f = uplc.Apply(f, uplc.PlutusConstr(0, []))
+        ret = uplc_eval(f).value
+        self.assertEqual(
+            ret,
+            1 + 2 + 3 + 4,
+            "for loop deconstruction did not behave as expected",
+        )
+
+    def test_different_return_types_anything(self):
+        source_code = """
+from hebi.prelude import *
+
+def validator(a: int) -> Anything:
+    if a > 0:
+        return b""
+    else:
+        return 0
+"""
+        ast = compiler.parse(source_code)
+        code = compiler.compile(ast).compile()
+        res = uplc_eval(uplc.Apply(code, uplc.PlutusInteger(1)))
+        self.assertEqual(res, uplc.PlutusByteString(b""))
+        res = uplc_eval(uplc.Apply(code, uplc.PlutusInteger(-1)))
+        self.assertEqual(res, uplc.PlutusInteger(0))
+
+    def test_no_return_annotation_no_return(self):
+        source_code = """
+from hebi.prelude import *
+
+def validator(a):
+    pass
+"""
+        ast = compiler.parse(source_code)
+        code = compiler.compile(ast).compile()
+        res = uplc_eval(uplc.Apply(code, uplc.PlutusConstr(0, [])))
+        self.assertEqual(res, uplc.PlutusConstr(0, []))
+
+    def test_opt_unsafe_cast(self):
+        # test that unsafe casts are not optimized away
+        source_code = """
+from hebi.prelude import *
+
+def validator(x: Token) -> bool:
+    b: Anything = x
+    a: int = b
+    return True
+        """
+        ast = compiler.parse(source_code)
+        code = compiler.compile(ast)
+        code = code.compile()
+        f = code.term
+        # UPLC lambdas may only take one argument at a time, so we evaluate by repeatedly applying
+        try:
+            for d in [
+                uplc.PlutusConstr(0, []),
+            ]:
+                f = uplc.Apply(f, d)
+            ret = uplc_eval(f)
+            failed = False
+        except Exception as e:
+            failed = True
+        self.assertTrue(failed, "Machine did validate the content")
```

### Comparing `hebi-0.1.1.0.9.9/hebi/tests/test_ops.py` & `hebi-0.2.0.0.12.5/hebi/tests/test_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,14 @@
-import frozendict
-import hypothesis
 import unittest
 
-from uplc import ast as uplc, eval as uplc_eval
 from hypothesis import example, given
 from hypothesis import strategies as st
-from parameterized import parameterized
+from uplc import ast as uplc, eval as uplc_eval
 
-from .. import compiler, prelude, type_inference
+from .. import compiler
 
 
 class OpTest(unittest.TestCase):
     @given(x=st.booleans(), y=st.booleans())
     def test_and_bool(self, x, y):
         # this tests that errors that are caused by assignments are actually triggered at the time of assigning
         source_code = """
```

### Comparing `hebi-0.1.1.0.9.9/hebi/tests/test_stdlib.py` & `hebi-0.2.0.0.12.5/hebi/tests/test_stdlib.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,76 @@
-import frozendict
-import hypothesis
 import unittest
 
-from uplc import ast as uplc, eval as uplc_eval
 from hypothesis import example, given
 from hypothesis import strategies as st
+from uplc import ast as uplc, eval as uplc_eval
 
 from .. import compiler
 
 
 class StdlibTest(unittest.TestCase):
+    @given(st.data())
+    def test_dict_get(self, data):
+        # this tests that errors that are caused by assignments are actually triggered at the time of assigning
+        source_code = """
+def validator(x: Dict[int, bytes], y: int, z: bytes) -> bytes:
+    return x.get(y, z)
+            """
+        ast = compiler.parse(source_code)
+        code = compiler.compile(ast)
+        code = code.compile()
+        f = code.term
+
+        x = data.draw(st.dictionaries(st.integers(), st.binary()))
+        y = data.draw(st.one_of(st.sampled_from(sorted(x.keys()) + [0]), st.integers()))
+        z = data.draw(st.binary())
+        # UPLC lambdas may only take one argument at a time, so we evaluate by repeatedly applying
+        for d in [
+            uplc.PlutusMap(
+                {uplc.PlutusInteger(k): uplc.PlutusByteString(v) for k, v in x.items()}
+            ),
+            uplc.PlutusInteger(y),
+            uplc.PlutusByteString(z),
+        ]:
+            f = uplc.Apply(f, d)
+        ret = uplc_eval(f).value
+        self.assertEqual(ret, x.get(y, z), "dict.get returned wrong value")
+
+    @given(st.data())
+    def test_dict_subscript(self, data):
+        # this tests that errors that are caused by assignments are actually triggered at the time of assigning
+        source_code = """
+def validator(x: Dict[int, bytes], y: int) -> bytes:
+    return x[y]
+            """
+        ast = compiler.parse(source_code)
+        code = compiler.compile(ast)
+        code = code.compile()
+        f = code.term
+
+        x = data.draw(st.dictionaries(st.integers(), st.binary()))
+        y = data.draw(st.one_of(st.sampled_from(sorted(x.keys()) + [0]), st.integers()))
+        # UPLC lambdas may only take one argument at a time, so we evaluate by repeatedly applying
+        for d in [
+            uplc.PlutusMap(
+                {uplc.PlutusInteger(k): uplc.PlutusByteString(v) for k, v in x.items()}
+            ),
+            uplc.PlutusInteger(y),
+        ]:
+            f = uplc.Apply(f, d)
+        try:
+            ret = uplc_eval(f).value
+        except RuntimeError:
+            ret = None
+        try:
+            exp = x[y]
+        except KeyError:
+            exp = None
+        self.assertEqual(ret, exp, "dict[] returned wrong value")
+
     @given(xs=st.dictionaries(st.integers(), st.binary()))
     def test_dict_keys(self, xs):
         # this tests that errors that are caused by assignments are actually triggered at the time of assigning
         source_code = """
 def validator(x: Dict[int, bytes]) -> List[int]:
     return x.keys()
             """
@@ -48,14 +105,58 @@
                 {uplc.PlutusInteger(k): uplc.PlutusByteString(v) for k, v in xs.items()}
             )
         ]:
             f = uplc.Apply(f, d)
         ret = [x.value for x in uplc_eval(f).value]
         self.assertEqual(ret, list(xs.values()), "dict.keys returned wrong value")
 
+    @given(xs=st.dictionaries(st.integers(), st.binary()))
+    def test_dict_items_keys_sum(self, xs):
+        # this tests that errors that are caused by assignments are actually triggered at the time of assigning
+        source_code = """
+def validator(xs: Dict[int, bytes]) -> int:
+    sum_keys = sum([x[0] for x in xs.items()])
+    return sum_keys
+"""
+        ast = compiler.parse(source_code)
+        code = compiler.compile(ast)
+        code = code.compile()
+        f = code.term
+        # UPLC lambdas may only take one argument at a time, so we evaluate by repeatedly applying
+        for d in [
+            uplc.PlutusMap(
+                {uplc.PlutusInteger(k): uplc.PlutusByteString(v) for k, v in xs.items()}
+            )
+        ]:
+            f = uplc.Apply(f, d)
+        ret = uplc_eval(f).value
+        self.assertEqual(ret, sum(xs.keys()), "dict.items returned wrong value")
+
+    @given(xs=st.dictionaries(st.binary(), st.integers()))
+    def test_dict_items_values_sum(self, xs):
+        # this tests that errors that are caused by assignments are actually triggered at the time of assigning
+        source_code = """
+def validator(xs: Dict[bytes, int]) -> int:
+    sum_values = sum([x[1] for x in xs.items()])
+    return sum_values
+"""
+        ast = compiler.parse(source_code)
+        code = compiler.compile(ast)
+        code = code.compile()
+        f = code.term
+        # UPLC lambdas may only take one argument at a time, so we evaluate by repeatedly applying
+        for d in [
+            uplc.PlutusMap(
+                {uplc.PlutusByteString(k): uplc.PlutusInteger(v) for k, v in xs.items()}
+            )
+        ]:
+            f = uplc.Apply(f, d)
+        ret = uplc_eval(f).value
+        self.assertEqual(ret, sum(xs.values()), "dict.items returned wrong value")
+
     @given(xs=st.text())
     def test_str_encode(self, xs):
         # this tests that errors that are caused by assignments are actually triggered at the time of assigning
         source_code = """
 def validator(x: str) -> bytes:
     return x.encode()
             """
@@ -151,15 +252,17 @@
         code = compiler.compile(ast)
         code = code.compile()
         f = code.term
         # UPLC lambdas may only take one argument at a time, so we evaluate by repeatedly applying
         for d in [uplc.BuiltinUnit()]:
             f = uplc.Apply(f, d)
         ret = uplc_eval(f)
-        self.assertEqual(ret, uplc.BuiltinUnit(), "literal None returned wrong value")
+        self.assertEqual(
+            ret, uplc.PlutusConstr(0, []), "literal None returned wrong value"
+        )
 
     @given(st.booleans())
     def test_constant_bool(self, x: bool):
         source_code = f"""
 def validator(x: None) -> bool:
     return {repr(x)}
             """
```

### Comparing `hebi-0.1.1.0.9.9/hebi/type_inference.py` & `hebi-0.2.0.0.12.5/hebi/type_inference.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from copy import copy
 import ast
 
 from .typed_ast import *
-from .util import PythonBuiltInTypes, CompilingNodeTransformer
+from .util import PythonBuiltInTypes, CompilingNodeTransformer, ReturnExtractor
 
 # from frozendict import frozendict
 
 
 """
 An aggressive type inference based on the work of Aycock [1].
 It only allows a subset of legal python operations which
@@ -38,29 +38,20 @@
         name.name: typ
         for name, typ in PythonBuiltInTypes.items()
         if isinstance(typ.typ, PolymorphicFunctionType)
     }
 )
 
 
-class ReturnExtractor(NodeVisitor):
-    """Utility to find all Return statements in an AST subtree"""
-
-    def __init__(self):
-        self.returns = []
-
-    def visit_Return(self, node: Return) -> None:
-        self.returns.append(node)
-
-
 class AggressiveTypeInferencer(CompilingNodeTransformer):
     step = "Static Type Inference"
 
     # A stack of dictionaries for storing scoped knowledge of variable types
     scopes = [INITIAL_SCOPE]
+    current_ret_type = []
 
     # Obtain the type of a variable name in the current scope
     def variable_type(self, name: str) -> Type:
         name = name
         for scope in reversed(self.scopes):
             if name in scope:
                 return scope[name]
@@ -69,15 +60,18 @@
     def enter_scope(self):
         self.scopes.append({})
 
     def exit_scope(self):
         self.scopes.pop()
 
     def set_variable_type(self, name: str, typ: Type, force=False):
-        if not force and name in self.scopes[-1] and typ != self.scopes[-1][name]:
+        if not force and name in self.scopes[-1] and self.scopes[-1][name] != typ:
+            if self.scopes[-1][name] >= typ:
+                # the specified type is broader, we pass on this
+                return
             raise TypeInferenceError(
                 f"Type {self.scopes[-1][name]} of variable {name} in local scope does not match inferred type {typ}"
             )
         self.scopes[-1][name] = typ
 
     def type_from_annotation(self, ann: expr):
         if isinstance(ann, Constant):
@@ -92,67 +86,62 @@
             raise TypeInferenceError(
                 f"Class name {ann.id} not initialized before annotating variable"
             )
         if isinstance(ann, Subscript):
             assert isinstance(
                 ann.value, Name
             ), "Only Union, Dict and List are allowed as Generic types"
-            assert isinstance(ann.slice, Index), "Generic types must be parameterized"
             if ann.value.id == "Union":
                 assert isinstance(
-                    ann.slice.value, Tuple
+                    ann.slice, Tuple
                 ), "Union must combine multiple classes"
-                ann_types = [self.type_from_annotation(e) for e in ann.slice.value.elts]
+                ann_types = [self.type_from_annotation(e) for e in ann.slice.elts]
                 assert all(
                     isinstance(e, RecordType) for e in ann_types
                 ), "Union must combine multiple PlutusData classes"
                 assert distinct(
                     [e.record.constructor for e in ann_types]
                 ), "Union must combine PlutusData classes with unique constructors"
                 return UnionType(FrozenFrozenList(ann_types))
             if ann.value.id == "List":
-                ann_type = self.type_from_annotation(ann.slice.value)
+                ann_type = self.type_from_annotation(ann.slice)
                 assert isinstance(
                     ann_type, ClassType
                 ), "List must have a single type as parameter"
                 assert not isinstance(
                     ann_type, TupleType
                 ), "List can currently not hold tuples"
                 return ListType(InstanceType(ann_type))
             if ann.value.id == "Dict":
-                assert isinstance(
-                    ann.slice.value, Tuple
-                ), "Dict must combine two classes"
-                assert len(ann.slice.value.elts) == 2, "Dict must combine two classes"
+                assert isinstance(ann.slice, Tuple), "Dict must combine two classes"
+                assert len(ann.slice.elts) == 2, "Dict must combine two classes"
                 ann_types = self.type_from_annotation(
-                    ann.slice.value.elts[0]
-                ), self.type_from_annotation(ann.slice.value.elts[1])
+                    ann.slice.elts[0]
+                ), self.type_from_annotation(ann.slice.elts[1])
                 assert all(
                     isinstance(e, ClassType) for e in ann_types
                 ), "Dict must combine two classes"
                 assert not any(
                     isinstance(e, TupleType) for e in ann_types
                 ), "Dict can currently not hold tuples"
                 return DictType(*(InstanceType(a) for a in ann_types))
             if ann.value.id == "Tuple":
                 assert isinstance(
-                    ann.slice.value, Tuple
+                    ann.slice, Tuple
                 ), "Tuple must combine several classes"
-                ann_types = [self.type_from_annotation(e) for e in ann.slice.value.elts]
+                ann_types = [self.type_from_annotation(e) for e in ann.slice.elts]
                 assert all(
                     isinstance(e, ClassType) for e in ann_types
                 ), "Tuple must combine classes"
                 return TupleType(FrozenFrozenList([InstanceType(a) for a in ann_types]))
             raise NotImplementedError(
                 "Only Union, Dict and List are allowed as Generic types"
             )
         if ann is None:
-            raise TypeInferenceError(
-                "Type annotation is missing for a function argument or return value"
-            )
+            return AnyType()
         raise NotImplementedError(f"Annotation type {ann.__class__} is not supported")
 
     def visit_ClassDef(self, node: ClassDef) -> TypedClassDef:
         class_record = RecordReader.extract(node, self)
         typ = RecordType(class_record)
         self.set_variable_type(node.name, typ)
         typed_node = copy(node)
@@ -220,17 +209,18 @@
         assert isinstance(
             node.target, Name
         ), "Can only assign to variable names, no type deconstruction"
         self.set_variable_type(
             node.target.id, InstanceType(typed_ass.annotation), force=True
         )
         typed_ass.target = self.visit(node.target)
-        assert typed_ass.value.typ >= InstanceType(
-            typed_ass.annotation
-        ), "Can only downcast to a specialized type"
+        assert (
+            typed_ass.value.typ >= InstanceType(typed_ass.annotation)
+            or InstanceType(typed_ass.annotation) >= typed_ass.value.typ
+        ), "Can only cast between related types"
         return typed_ass
 
     def visit_If(self, node: If) -> TypedIf:
         typed_if = copy(node)
         if (
             isinstance(typed_if.test, Call)
             and (typed_if.test.func, Name)
@@ -347,38 +337,41 @@
         ta = copy(node)
         ta.args = [self.visit(a) for a in node.args]
         return ta
 
     def visit_FunctionDef(self, node: FunctionDef) -> TypedFunctionDef:
         tfd = copy(node)
         assert not node.decorator_list, "Functions may not have decorators"
+        rettyp = InstanceType(self.type_from_annotation(tfd.returns))
         self.enter_scope()
+        self.current_ret_type.append(rettyp)
         tfd.args = self.visit(node.args)
         functyp = FunctionType(
             [t.typ for t in tfd.args.args],
-            InstanceType(self.type_from_annotation(tfd.returns)),
+            rettyp,
         )
         tfd.typ = InstanceType(functyp)
         # We need the function type inside for recursion
         self.set_variable_type(node.name, tfd.typ)
         tfd.body = [self.visit(s) for s in node.body]
         rets_extractor = ReturnExtractor()
         for b in tfd.body:
             rets_extractor.visit(b)
         rets = rets_extractor.returns
         # Check that return type and annotated return type match
         if not rets:
             assert (
-                functyp.rettyp == NoneInstanceType
+                functyp.rettyp >= NoneInstanceType
             ), f"Function '{node.name}' has no return statement but is supposed to return not-None value"
         else:
             assert all(
                 functyp.rettyp >= r.typ for r in rets
             ), f"Function '{node.name}' annotated return type does not match actual return type"
         self.exit_scope()
+        self.current_ret_type.pop(-1)
         # We need the function type outside for usage
         self.set_variable_type(node.name, tfd.typ)
         return tfd
 
     def visit_Module(self, node: Module) -> TypedModule:
         self.enter_scope()
         tm = copy(node)
@@ -421,54 +414,52 @@
         ts = copy(node)
         # special case: Subscript of Union / Dict / List and atomic types
         if isinstance(ts.value, Name) and ts.value.id in [
             "Union",
             "Dict",
             "List",
         ]:
-            assert isinstance(
-                ts.slice, Index
-            ), "Only single index slices for generic types are currently supported"
             ts.value = ts.typ = self.type_from_annotation(ts)
             return ts
 
         ts.value = self.visit(node.value)
         assert isinstance(ts.value.typ, InstanceType), "Can only subscript instances"
         if isinstance(ts.value.typ.typ, TupleType):
             assert (
                 ts.value.typ.typ.typs
             ), "Accessing elements from the empty tuple is not allowed"
-            assert isinstance(
-                ts.slice, Index
-            ), "Only single index slices for tuples are currently supported"
             if all(ts.value.typ.typ.typs[0] == t for t in ts.value.typ.typ.typs):
                 ts.typ = ts.value.typ.typ.typs[0]
-            elif isinstance(ts.slice.value, Constant) and isinstance(
-                ts.slice.value.value, int
-            ):
-                ts.typ = ts.value.typ.typ.typs[ts.slice.value.value]
+            elif isinstance(ts.slice, Constant) and isinstance(ts.slice.value, int):
+                ts.typ = ts.value.typ.typ.typs[ts.slice.value]
             else:
                 raise TypeInferenceError(
-                    f"Could not infer type of subscript of typ {ts.value.typ.__class__}"
+                    f"Could not infer type of subscript of typ {ts.value.typ.typ.__class__}"
+                )
+        elif isinstance(ts.value.typ.typ, PairType):
+            if isinstance(ts.slice, Constant) and isinstance(ts.slice.value, int):
+                ts.typ = (
+                    ts.value.typ.typ.l_typ
+                    if ts.slice.value == 0
+                    else ts.value.typ.typ.r_typ
+                )
+            else:
+                raise TypeInferenceError(
+                    f"Could not infer type of subscript of typ {ts.value.typ.typ.__class__}"
                 )
         elif isinstance(ts.value.typ.typ, ListType):
-            assert isinstance(
-                ts.slice, Index
-            ), "Only single index slices for lists are currently supported"
             ts.typ = ts.value.typ.typ.typ
-            ts.slice.value = self.visit(node.slice.value)
-            assert (
-                ts.slice.value.typ == IntegerInstanceType
-            ), "List indices must be integers"
+            ts.slice = self.visit(node.slice)
+            assert ts.slice.typ == IntegerInstanceType, "List indices must be integers"
         elif isinstance(ts.value.typ.typ, ByteStringType):
-            if isinstance(ts.slice, Index):
+            if not isinstance(ts.slice, Slice):
                 ts.typ = IntegerInstanceType
-                ts.slice.value = self.visit(node.slice.value)
+                ts.slice = self.visit(node.slice)
                 assert (
-                    ts.slice.value.typ == IntegerInstanceType
+                    ts.slice.typ == IntegerInstanceType
                 ), "bytes indices must be integers"
             elif isinstance(ts.slice, Slice):
                 ts.typ = ByteStringInstanceType
                 if ts.slice.lower is None:
                     ts.slice.lower = Constant(0)
                 ts.slice.lower = self.visit(node.slice.lower)
                 assert (
@@ -484,17 +475,24 @@
                 ), "upper slice indices for bytes must be integers"
             else:
                 raise TypeInferenceError(
                     f"Could not infer type of subscript of typ {ts.value.typ.__class__}"
                 )
         elif isinstance(ts.value.typ.typ, DictType):
             # TODO could be implemented with potentially just erroring. It might be desired to avoid this though.
-            raise TypeInferenceError(
-                f"Could not infer type of subscript of dict. Use 'get' with a default value instead."
-            )
+            if not isinstance(ts.slice, Slice):
+                ts.slice = self.visit(node.slice)
+                assert (
+                    ts.slice.typ == ts.value.typ.typ.key_typ
+                ), f"Dict subscript must have dict key type {ts.value.typ.typ.key_typ} but has type {ts.slice.typ}"
+                ts.typ = ts.value.typ.typ.value_typ
+            else:
+                raise TypeInferenceError(
+                    f"Could not infer type of subscript of dict with a slice."
+                )
         else:
             raise TypeInferenceError(
                 f"Could not infer type of subscript of typ {ts.value.typ.__class__}"
             )
         return ts
 
     def visit_Call(self, node: Call) -> TypedCall:
@@ -517,31 +515,33 @@
             )
         if isinstance(tc.func.typ, InstanceType) and isinstance(
             tc.func.typ.typ, FunctionType
         ):
             functyp = tc.func.typ.typ
             assert len(tc.args) == len(
                 functyp.argtyps
-            ), f"Signature of function {ast.dump(node)} does not match number of arguments"
+            ), f"Signature of function does not match number of arguments. Expected {len(functyp.argtyps)} arguments with these types: {functyp.argtyps}"
             # all arguments need to be supertypes of the given type
             assert all(
                 ap >= a.typ for a, ap in zip(tc.args, functyp.argtyps)
-            ), f"Signature of function {ast.dump(node)} does not match arguments"
+            ), f"Signature of function does not match arguments. Expected {len(functyp.argtyps)} arguments with these types: {functyp.argtyps}"
             tc.typ = functyp.rettyp
             return tc
         raise TypeInferenceError("Could not infer type of call")
 
     def visit_Pass(self, node: Pass) -> TypedPass:
         tp = copy(node)
         return tp
 
     def visit_Return(self, node: Return) -> TypedReturn:
         tp = copy(node)
         tp.value = self.visit(node.value)
-        tp.typ = tp.value.typ
+        tp.typ = (
+            tp.value.typ if not self.current_ret_type else self.current_ret_type[-1]
+        )
         return tp
 
     def visit_Attribute(self, node: Attribute) -> TypedAttribute:
         tp = copy(node)
         tp.value = self.visit(node.value)
         owner = tp.value.typ
         # accesses to field
```

### Comparing `hebi-0.1.1.0.9.9/hebi/typed_ast.py` & `hebi-0.2.0.0.12.5/hebi/typed_ast.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,14 +277,28 @@
     def __ge__(self, other):
         return isinstance(other, TupleType) and all(
             t >= ot for t, ot in zip(self.typs, other.typs)
         )
 
 
 @dataclass(frozen=True, unsafe_hash=True)
+class PairType(ClassType):
+    """An internal type representing built-in PlutusData pairs"""
+
+    l_typ: Type
+    r_typ: Type
+
+    def __ge__(self, other):
+        return isinstance(other, PairType) and all(
+            t >= ot
+            for t, ot in zip((self.l_typ, self.r_typ), (other.l_typ, other.r_typ))
+        )
+
+
+@dataclass(frozen=True, unsafe_hash=True)
 class ListType(ClassType):
     typ: Type
 
     def __ge__(self, other):
         return isinstance(other, ListType) and self.typ >= other.typ
 
 
@@ -300,14 +314,23 @@
             )
         if attr == "keys":
             return InstanceType(FunctionType([], InstanceType(ListType(self.key_typ))))
         if attr == "values":
             return InstanceType(
                 FunctionType([], InstanceType(ListType(self.value_typ)))
             )
+        if attr == "items":
+            return InstanceType(
+                FunctionType(
+                    [],
+                    InstanceType(
+                        ListType(InstanceType(PairType(self.key_typ, self.value_typ)))
+                    ),
+                )
+            )
         raise TypeInferenceError(
             f"Type of attribute '{attr}' is unknown for type Dict."
         )
 
     def attribute(self, attr) -> plt.AST:
         if attr == "get":
             return plt.Lambda(
@@ -358,14 +381,19 @@
                         transform_ext_params_map(self.value_typ)(
                             plt.SndPair(plt.Var("x"))
                         ),
                     ),
                     empty_list(self.value_typ),
                 ),
             )
+        if attr == "items":
+            return plt.Lambda(
+                ["self", "_"],
+                plt.Var("self"),
+            )
         raise NotImplementedError(f"Attribute '{attr}' of Dict is unknown.")
 
     def __ge__(self, other):
         return (
             isinstance(other, DictType)
             and self.key_typ >= other.key_typ
             and self.value_typ >= other.value_typ
@@ -757,14 +785,23 @@
                     ),
                 )
         return super().cmp(op, o)
 
 
 @dataclass(frozen=True, unsafe_hash=True)
 class BoolType(AtomicType):
+    def constr_type(self) -> "InstanceType":
+        return InstanceType(FunctionType([IntegerInstanceType], BoolInstanceType))
+
+    def constr(self) -> plt.AST:
+        # constructs a boolean from an integer
+        return plt.Lambda(
+            ["_", "x"], plt.Not(plt.EqualsInteger(plt.Var("x"), plt.Integer(0)))
+        )
+
     def cmp(self, op: cmpop, o: "Type") -> plt.AST:
         if isinstance(o, IntegerType):
             if isinstance(op, Eq):
                 # 1 == True
                 # 0 == False
                 # all other comparisons are False
                 return plt.Lambda(
@@ -1066,15 +1103,17 @@
     return lambda x: x
 
 
 TransformOutputMap = {
     StringInstanceType: lambda x: plt.BData(plt.EncodeUtf8(x)),
     IntegerInstanceType: lambda x: plt.IData(x),
     ByteStringInstanceType: lambda x: plt.BData(x),
-    UnitInstanceType: lambda x: plt.Apply(plt.Lambda(["_"], plt.Unit()), x),
+    UnitInstanceType: lambda x: plt.Apply(
+        plt.Lambda(["_"], plt.ConstrData(plt.Integer(0), plt.EmptyDataList())), x
+    ),
     BoolInstanceType: lambda x: plt.IData(
         plt.IfThenElse(x, plt.Integer(1), plt.Integer(0))
     ),
 }
 
 
 def transform_output_map(p: Type):
```

### Comparing `hebi-0.1.1.0.9.9/hebi/util.py` & `hebi-0.2.0.0.12.5/hebi/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import ast
+import pycardano
 from enum import Enum, auto
 
 from .typed_ast import *
 
 import pluthon as plt
 import uplc.ast as uplc
 
@@ -545,7 +546,25 @@
     if "map" in j:
         return uplc.PlutusMap({d["k"]: d["v"] for d in j["map"]})
     if "constructor" in j and "fields" in j:
         return uplc.PlutusConstr(
             j["constructor"], list(map(data_from_json, j["fields"]))
         )
     raise NotImplementedError(f"Unknown datum representation {j}")
+
+
+def datum_to_cbor(d: pycardano.Datum) -> bytes:
+    return pycardano.PlutusData.to_cbor(d, encoding="bytes")
+
+
+def datum_to_json(d: pycardano.Datum) -> str:
+    return pycardano.PlutusData.to_json(d)
+
+
+class ReturnExtractor(TypedNodeVisitor):
+    """Utility to find all Return statements in an AST subtree"""
+
+    def __init__(self):
+        self.returns = []
+
+    def visit_Return(self, node: Return) -> None:
+        self.returns.append(node)
```

