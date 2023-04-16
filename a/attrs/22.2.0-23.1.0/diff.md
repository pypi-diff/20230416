# Comparing `tmp/attrs-22.2.0.tar.gz` & `tmp/attrs-23.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "attrs-22.2.0.tar", last modified: Wed Dec 21 09:10:26 2022, max compression
+gzip compressed data, last modified: Sun Apr 16 10:22:15 2023, max compression
```

## Comparing `attrs-22.2.0.tar` & `attrs-23.1.0.tar`

### file list

```diff
@@ -1,130 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 09:10:25.996807 attrs-22.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 09:10:25.936806 attrs-22.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2022-12-21 09:10:16.000000 attrs-22.2.0/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)    10183 2022-12-21 09:10:16.000000 attrs-22.2.0/.github/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)       59 2022-12-21 09:10:16.000000 attrs-22.2.0/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2022-12-21 09:10:16.000000 attrs-22.2.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      378 2022-12-21 09:10:16.000000 attrs-22.2.0/.github/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)      119 2022-12-21 09:10:16.000000 attrs-22.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 09:10:25.936806 attrs-22.2.0/.github/sponsors/
--rw-r--r--   0 runner    (1001) docker     (123)     5189 2022-12-21 09:10:16.000000 attrs-22.2.0/.github/sponsors/FilePreviews.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2022-12-21 09:10:16.000000 attrs-22.2.0/.github/sponsors/Sentry.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2022-12-21 09:10:16.000000 attrs-22.2.0/.github/sponsors/Tidelift.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2022-12-21 09:10:16.000000 attrs-22.2.0/.github/sponsors/Variomedia.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 09:10:25.936806 attrs-22.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2022-12-21 09:10:16.000000 attrs-22.2.0/.github/workflows/build-docset.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5630 2022-12-21 09:10:16.000000 attrs-22.2.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2022-12-21 09:10:16.000000 attrs-22.2.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2022-12-21 09:10:16.000000 attrs-22.2.0/.github/workflows/pypi-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2022-12-21 09:10:16.000000 attrs-22.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    56547 2022-12-21 09:10:16.000000 attrs-22.2.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      215 2022-12-21 09:10:16.000000 attrs-22.2.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2022-12-21 09:10:16.000000 attrs-22.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      620 2022-12-21 09:10:16.000000 attrs-22.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11727 2022-12-21 09:10:25.996807 attrs-22.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6892 2022-12-21 09:10:16.000000 attrs-22.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 09:10:25.936806 attrs-22.2.0/changelog.d/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2022-12-21 09:10:16.000000 attrs-22.2.0/changelog.d/towncrier_template.md.jinja
--rw-r--r--   0 runner    (1001) docker     (123)      685 2022-12-21 09:10:16.000000 attrs-22.2.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 09:10:25.944806 attrs-22.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6758 2022-12-21 09:10:16.000000 attrs-22.2.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 09:10:25.948806 attrs-22.2.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     7639 2022-12-21 09:10:16.000000 attrs-22.2.0/docs/_static/attrs_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     8313 2022-12-21 09:10:16.000000 attrs-22.2.0/docs/_static/attrs_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5577 2022-12-21 09:10:16.000000 attrs-22.2.0/docs/_static/attrs_logo_white.png
--rw-r--r--   0 runner    (1001) docker     (123)     8313 2022-12-21 09:10:16.000000 attrs-22.2.0/docs/_static/attrs_logo_white.svg
--rw-r--r--   0 runner    (1001) docker     (123)      637 2022-12-21 09:10:16.000000 attrs-22.2.0/docs/_static/docset-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2022-12-21 09:10:16.000000 attrs-22.2.0/docs/_static/docset-icon@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)    26851 2022-12-21 09:10:16.000000 attrs-22.2.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      215 2022-12-21 09:10:16.000000 attrs-22.2.0/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2022-12-21 09:10:16.000000 attrs-22.2.0/docs/comparison.md
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2022-12-21 09:10:16.000000 attrs-22.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    19063 2022-12-21 09:10:16.000000 attrs-22.2.0/docs/examples.md
--rw-r--r--   0 runner    (1001) docker     (123)    10180 2022-12-21 09:10:16.000000 attrs-22.2.0/docs/extending.md
--rw-r--r--   0 runner    (1001) docker     (123)     5319 2022-12-21 09:10:16.000000 attrs-22.2.0/docs/glossary.md
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2022-12-21 09:10:16.000000 attrs-22.2.0/docs/hashing.md
--rw-r--r--   0 runner    (1001) docker     (123)     4622 2022-12-21 09:10:16.000000 attrs-22.2.0/docs/how-does-it-work.md
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2022-12-21 09:10:16.000000 attrs-22.2.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)    16576 2022-12-21 09:10:16.000000 attrs-22.2.0/docs/init.md
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2022-12-21 09:10:16.000000 attrs-22.2.0/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)     7679 2022-12-21 09:10:16.000000 attrs-22.2.0/docs/names.md
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2022-12-21 09:10:16.000000 attrs-22.2.0/docs/overview.md
--rw-r--r--   0 runner    (1001) docker     (123)     4837 2022-12-21 09:10:16.000000 attrs-22.2.0/docs/types.md
--rw-r--r--   0 runner    (1001) docker     (123)    12895 2022-12-21 09:10:16.000000 attrs-22.2.0/docs/why.md
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2022-12-21 09:10:16.000000 attrs-22.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      238 2022-12-21 09:10:16.000000 attrs-22.2.0/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-21 09:10:26.000807 attrs-22.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5049 2022-12-21 09:10:16.000000 attrs-22.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 09:10:25.928806 attrs-22.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 09:10:25.968806 attrs-22.2.0/src/attr/
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2022-12-21 09:10:16.000000 attrs-22.2.0/src/attr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15831 2022-12-21 09:10:16.000000 attrs-22.2.0/src/attr/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2022-12-21 09:10:16.000000 attrs-22.2.0/src/attr/_cmp.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2022-12-21 09:10:16.000000 attrs-22.2.0/src/attr/_cmp.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5435 2022-12-21 09:10:16.000000 attrs-22.2.0/src/attr/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2022-12-21 09:10:16.000000 attrs-22.2.0/src/attr/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14545 2022-12-21 09:10:16.000000 attrs-22.2.0/src/attr/_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    96087 2022-12-21 09:10:16.000000 attrs-22.2.0/src/attr/_make.py
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2022-12-21 09:10:16.000000 attrs-22.2.0/src/attr/_next_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2022-12-21 09:10:16.000000 attrs-22.2.0/src/attr/_typing_compat.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2022-12-21 09:10:16.000000 attrs-22.2.0/src/attr/_version_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2022-12-21 09:10:16.000000 attrs-22.2.0/src/attr/_version_info.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2022-12-21 09:10:16.000000 attrs-22.2.0/src/attr/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2022-12-21 09:10:16.000000 attrs-22.2.0/src/attr/converters.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2022-12-21 09:10:16.000000 attrs-22.2.0/src/attr/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2022-12-21 09:10:16.000000 attrs-22.2.0/src/attr/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2022-12-21 09:10:16.000000 attrs-22.2.0/src/attr/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2022-12-21 09:10:16.000000 attrs-22.2.0/src/attr/filters.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 09:10:16.000000 attrs-22.2.0/src/attr/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2022-12-21 09:10:16.000000 attrs-22.2.0/src/attr/setters.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2022-12-21 09:10:16.000000 attrs-22.2.0/src/attr/setters.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    20501 2022-12-21 09:10:16.000000 attrs-22.2.0/src/attr/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2022-12-21 09:10:16.000000 attrs-22.2.0/src/attr/validators.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 09:10:25.972807 attrs-22.2.0/src/attrs/
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2022-12-21 09:10:16.000000 attrs-22.2.0/src/attrs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2022-12-21 09:10:16.000000 attrs-22.2.0/src/attrs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       70 2022-12-21 09:10:16.000000 attrs-22.2.0/src/attrs/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2022-12-21 09:10:16.000000 attrs-22.2.0/src/attrs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2022-12-21 09:10:16.000000 attrs-22.2.0/src/attrs/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 09:10:16.000000 attrs-22.2.0/src/attrs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       67 2022-12-21 09:10:16.000000 attrs-22.2.0/src/attrs/setters.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2022-12-21 09:10:16.000000 attrs-22.2.0/src/attrs/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 09:10:25.976806 attrs-22.2.0/src/attrs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11727 2022-12-21 09:10:25.000000 attrs-22.2.0/src/attrs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2022-12-21 09:10:25.000000 attrs-22.2.0/src/attrs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-21 09:10:25.000000 attrs-22.2.0/src/attrs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-21 09:10:25.000000 attrs-22.2.0/src/attrs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      783 2022-12-21 09:10:25.000000 attrs-22.2.0/src/attrs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2022-12-21 09:10:25.000000 attrs-22.2.0/src/attrs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 09:10:25.996807 attrs-22.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2022-12-21 09:10:16.000000 attrs-22.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2022-12-21 09:10:16.000000 attrs-22.2.0/tests/attr_import_star.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2022-12-21 09:10:16.000000 attrs-22.2.0/tests/dataclass_transform_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     5738 2022-12-21 09:10:16.000000 attrs-22.2.0/tests/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2022-12-21 09:10:16.000000 attrs-22.2.0/tests/test_3rd_party.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2022-12-21 09:10:16.000000 attrs-22.2.0/tests/test_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)    17443 2022-12-21 09:10:16.000000 attrs-22.2.0/tests/test_annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)    14762 2022-12-21 09:10:16.000000 attrs-22.2.0/tests/test_cmp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2022-12-21 09:10:16.000000 attrs-22.2.0/tests/test_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2022-12-21 09:10:16.000000 attrs-22.2.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2022-12-21 09:10:16.000000 attrs-22.2.0/tests/test_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)    27565 2022-12-21 09:10:16.000000 attrs-22.2.0/tests/test_dunders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2022-12-21 09:10:16.000000 attrs-22.2.0/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    19853 2022-12-21 09:10:16.000000 attrs-22.2.0/tests/test_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18951 2022-12-21 09:10:16.000000 attrs-22.2.0/tests/test_functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     6116 2022-12-21 09:10:16.000000 attrs-22.2.0/tests/test_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2022-12-21 09:10:16.000000 attrs-22.2.0/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2022-12-21 09:10:16.000000 attrs-22.2.0/tests/test_init_subclass.py
--rw-r--r--   0 runner    (1001) docker     (123)    65399 2022-12-21 09:10:16.000000 attrs-22.2.0/tests/test_make.py
--rw-r--r--   0 runner    (1001) docker     (123)    38642 2022-12-21 09:10:16.000000 attrs-22.2.0/tests/test_mypy.yml
--rw-r--r--   0 runner    (1001) docker     (123)    10085 2022-12-21 09:10:16.000000 attrs-22.2.0/tests/test_next_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2022-12-21 09:10:16.000000 attrs-22.2.0/tests/test_pattern_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2022-12-21 09:10:16.000000 attrs-22.2.0/tests/test_pyright.py
--rw-r--r--   0 runner    (1001) docker     (123)    11122 2022-12-21 09:10:16.000000 attrs-22.2.0/tests/test_setattr.py
--rw-r--r--   0 runner    (1001) docker     (123)    19236 2022-12-21 09:10:16.000000 attrs-22.2.0/tests/test_slots.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2022-12-21 09:10:16.000000 attrs-22.2.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    35768 2022-12-21 09:10:16.000000 attrs-22.2.0/tests/test_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2022-12-21 09:10:16.000000 attrs-22.2.0/tests/test_version_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     8594 2022-12-21 09:10:16.000000 attrs-22.2.0/tests/typing_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2022-12-21 09:10:16.000000 attrs-22.2.0/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2022-12-21 09:10:16.000000 attrs-22.2.0/tox.ini
+-rw-r--r--   0        0        0      125 2023-04-16 10:22:15.000000 attrs-23.1.0/.git_archival.txt
+-rw-r--r--   0        0        0      131 2023-04-16 10:22:15.000000 attrs-23.1.0/.gitattributes
+-rw-r--r--   0        0        0     1042 2023-04-16 10:22:15.000000 attrs-23.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      238 2023-04-16 10:22:15.000000 attrs-23.1.0/.readthedocs.yaml
+-rw-r--r--   0        0        0    59511 2023-04-16 10:22:15.000000 attrs-23.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0      215 2023-04-16 10:22:15.000000 attrs-23.1.0/CITATION.cff
+-rw-r--r--   0        0        0     6873 2023-04-16 10:22:15.000000 attrs-23.1.0/README.md
+-rw-r--r--   0        0        0      685 2023-04-16 10:22:15.000000 attrs-23.1.0/conftest.py
+-rw-r--r--   0        0        0     2620 2023-04-16 10:22:15.000000 attrs-23.1.0/tox.ini
+-rw-r--r--   0        0        0     5483 2023-04-16 10:22:15.000000 attrs-23.1.0/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0    10999 2023-04-16 10:22:15.000000 attrs-23.1.0/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0       41 2023-04-16 10:22:15.000000 attrs-23.1.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0     2567 2023-04-16 10:22:15.000000 attrs-23.1.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      378 2023-04-16 10:22:15.000000 attrs-23.1.0/.github/SECURITY.md
+-rw-r--r--   0        0        0      119 2023-04-16 10:22:15.000000 attrs-23.1.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     5189 2023-04-16 10:22:15.000000 attrs-23.1.0/.github/sponsors/FilePreviews.svg
+-rw-r--r--   0        0        0     1901 2023-04-16 10:22:15.000000 attrs-23.1.0/.github/sponsors/Sentry.svg
+-rw-r--r--   0        0        0     2082 2023-04-16 10:22:15.000000 attrs-23.1.0/.github/sponsors/Tidelift.svg
+-rw-r--r--   0        0        0     1932 2023-04-16 10:22:15.000000 attrs-23.1.0/.github/sponsors/Variomedia.svg
+-rw-r--r--   0        0        0      555 2023-04-16 10:22:15.000000 attrs-23.1.0/.github/workflows/build-docset.yml
+-rw-r--r--   0        0        0     4798 2023-04-16 10:22:15.000000 attrs-23.1.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      753 2023-04-16 10:22:15.000000 attrs-23.1.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0     1748 2023-04-16 10:22:15.000000 attrs-23.1.0/.github/workflows/pypi-package.yml
+-rw-r--r--   0        0        0        0 2023-04-16 10:22:15.000000 attrs-23.1.0/changelog.d/.gitignore
+-rw-r--r--   0        0        0      798 2023-04-16 10:22:15.000000 attrs-23.1.0/changelog.d/towncrier_template.md.jinja
+-rw-r--r--   0        0        0     6758 2023-04-16 10:22:15.000000 attrs-23.1.0/docs/Makefile
+-rw-r--r--   0        0        0     5268 2023-04-16 10:22:15.000000 attrs-23.1.0/docs/api-attr.rst
+-rw-r--r--   0        0        0    22685 2023-04-16 10:22:15.000000 attrs-23.1.0/docs/api.rst
+-rw-r--r--   0        0        0      215 2023-04-16 10:22:15.000000 attrs-23.1.0/docs/changelog.md
+-rw-r--r--   0        0        0     1864 2023-04-16 10:22:15.000000 attrs-23.1.0/docs/comparison.md
+-rw-r--r--   0        0        0     5158 2023-04-16 10:22:15.000000 attrs-23.1.0/docs/conf.py
+-rw-r--r--   0        0        0    20163 2023-04-16 10:22:15.000000 attrs-23.1.0/docs/examples.md
+-rw-r--r--   0        0        0     9857 2023-04-16 10:22:15.000000 attrs-23.1.0/docs/extending.md
+-rw-r--r--   0        0        0     5319 2023-04-16 10:22:15.000000 attrs-23.1.0/docs/glossary.md
+-rw-r--r--   0        0        0     5127 2023-04-16 10:22:15.000000 attrs-23.1.0/docs/hashing.md
+-rw-r--r--   0        0        0     4622 2023-04-16 10:22:15.000000 attrs-23.1.0/docs/how-does-it-work.md
+-rw-r--r--   0        0        0     3056 2023-04-16 10:22:15.000000 attrs-23.1.0/docs/index.md
+-rw-r--r--   0        0        0    16635 2023-04-16 10:22:15.000000 attrs-23.1.0/docs/init.md
+-rw-r--r--   0        0        0     1201 2023-04-16 10:22:15.000000 attrs-23.1.0/docs/license.md
+-rw-r--r--   0        0        0     7679 2023-04-16 10:22:15.000000 attrs-23.1.0/docs/names.md
+-rw-r--r--   0        0        0     2448 2023-04-16 10:22:15.000000 attrs-23.1.0/docs/overview.md
+-rw-r--r--   0        0        0     4569 2023-04-16 10:22:15.000000 attrs-23.1.0/docs/types.md
+-rw-r--r--   0        0        0    12901 2023-04-16 10:22:15.000000 attrs-23.1.0/docs/why.md
+-rw-r--r--   0        0        0     7639 2023-04-16 10:22:15.000000 attrs-23.1.0/docs/_static/attrs_logo.png
+-rw-r--r--   0        0        0     8313 2023-04-16 10:22:15.000000 attrs-23.1.0/docs/_static/attrs_logo.svg
+-rw-r--r--   0        0        0     5577 2023-04-16 10:22:15.000000 attrs-23.1.0/docs/_static/attrs_logo_white.png
+-rw-r--r--   0        0        0     8313 2023-04-16 10:22:15.000000 attrs-23.1.0/docs/_static/attrs_logo_white.svg
+-rw-r--r--   0        0        0     1833 2023-04-16 10:22:15.000000 attrs-23.1.0/docs/_static/docset-icon.png
+-rw-r--r--   0        0        0     2273 2023-04-16 10:22:15.000000 attrs-23.1.0/docs/_static/docset-icon@2x.png
+-rw-r--r--   0        0        0     3241 2023-04-16 10:22:15.000000 attrs-23.1.0/src/attr/__init__.py
+-rw-r--r--   0        0        0    17609 2023-04-16 10:22:15.000000 attrs-23.1.0/src/attr/__init__.pyi
+-rw-r--r--   0        0        0     4098 2023-04-16 10:22:15.000000 attrs-23.1.0/src/attr/_cmp.py
+-rw-r--r--   0        0        0      399 2023-04-16 10:22:15.000000 attrs-23.1.0/src/attr/_cmp.pyi
+-rw-r--r--   0        0        0     5803 2023-04-16 10:22:15.000000 attrs-23.1.0/src/attr/_compat.py
+-rw-r--r--   0        0        0      826 2023-04-16 10:22:15.000000 attrs-23.1.0/src/attr/_config.py
+-rw-r--r--   0        0        0    16730 2023-04-16 10:22:15.000000 attrs-23.1.0/src/attr/_funcs.py
+-rw-r--r--   0        0        0    96979 2023-04-16 10:22:15.000000 attrs-23.1.0/src/attr/_make.py
+-rw-r--r--   0        0        0     6271 2023-04-16 10:22:15.000000 attrs-23.1.0/src/attr/_next_gen.py
+-rw-r--r--   0        0        0      469 2023-04-16 10:22:15.000000 attrs-23.1.0/src/attr/_typing_compat.pyi
+-rw-r--r--   0        0        0     2121 2023-04-16 10:22:15.000000 attrs-23.1.0/src/attr/_version_info.py
+-rw-r--r--   0        0        0      209 2023-04-16 10:22:15.000000 attrs-23.1.0/src/attr/_version_info.pyi
+-rw-r--r--   0        0        0     3602 2023-04-16 10:22:15.000000 attrs-23.1.0/src/attr/converters.py
+-rw-r--r--   0        0        0      406 2023-04-16 10:22:15.000000 attrs-23.1.0/src/attr/converters.pyi
+-rw-r--r--   0        0        0     1890 2023-04-16 10:22:15.000000 attrs-23.1.0/src/attr/exceptions.py
+-rw-r--r--   0        0        0      539 2023-04-16 10:22:15.000000 attrs-23.1.0/src/attr/exceptions.pyi
+-rw-r--r--   0        0        0     1470 2023-04-16 10:22:15.000000 attrs-23.1.0/src/attr/filters.py
+-rw-r--r--   0        0        0      225 2023-04-16 10:22:15.000000 attrs-23.1.0/src/attr/filters.pyi
+-rw-r--r--   0        0        0        0 2023-04-16 10:22:15.000000 attrs-23.1.0/src/attr/py.typed
+-rw-r--r--   0        0        0     1400 2023-04-16 10:22:15.000000 attrs-23.1.0/src/attr/setters.py
+-rw-r--r--   0        0        0      567 2023-04-16 10:22:15.000000 attrs-23.1.0/src/attr/setters.pyi
+-rw-r--r--   0        0        0    20702 2023-04-16 10:22:15.000000 attrs-23.1.0/src/attr/validators.py
+-rw-r--r--   0        0        0     2580 2023-04-16 10:22:15.000000 attrs-23.1.0/src/attr/validators.pyi
+-rw-r--r--   0        0        0     1039 2023-04-16 10:22:15.000000 attrs-23.1.0/src/attrs/__init__.py
+-rw-r--r--   0        0        0     2168 2023-04-16 10:22:15.000000 attrs-23.1.0/src/attrs/__init__.pyi
+-rw-r--r--   0        0        0       70 2023-04-16 10:22:15.000000 attrs-23.1.0/src/attrs/converters.py
+-rw-r--r--   0        0        0       70 2023-04-16 10:22:15.000000 attrs-23.1.0/src/attrs/exceptions.py
+-rw-r--r--   0        0        0       67 2023-04-16 10:22:15.000000 attrs-23.1.0/src/attrs/filters.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:22:15.000000 attrs-23.1.0/src/attrs/py.typed
+-rw-r--r--   0        0        0       67 2023-04-16 10:22:15.000000 attrs-23.1.0/src/attrs/setters.py
+-rw-r--r--   0        0        0       70 2023-04-16 10:22:15.000000 attrs-23.1.0/src/attrs/validators.py
+-rw-r--r--   0        0        0       31 2023-04-16 10:22:15.000000 attrs-23.1.0/tests/__init__.py
+-rw-r--r--   0        0        0      255 2023-04-16 10:22:15.000000 attrs-23.1.0/tests/attr_import_star.py
+-rw-r--r--   0        0        0      821 2023-04-16 10:22:15.000000 attrs-23.1.0/tests/dataclass_transform_example.py
+-rw-r--r--   0        0        0     5738 2023-04-16 10:22:15.000000 attrs-23.1.0/tests/strategies.py
+-rw-r--r--   0        0        0      673 2023-04-16 10:22:15.000000 attrs-23.1.0/tests/test_3rd_party.py
+-rw-r--r--   0        0        0     1618 2023-04-16 10:22:15.000000 attrs-23.1.0/tests/test_abc.py
+-rw-r--r--   0        0        0    18138 2023-04-16 10:22:15.000000 attrs-23.1.0/tests/test_annotations.py
+-rw-r--r--   0        0        0    14762 2023-04-16 10:22:15.000000 attrs-23.1.0/tests/test_cmp.py
+-rw-r--r--   0        0        0     1405 2023-04-16 10:22:15.000000 attrs-23.1.0/tests/test_compat.py
+-rw-r--r--   0        0        0     1123 2023-04-16 10:22:15.000000 attrs-23.1.0/tests/test_config.py
+-rw-r--r--   0        0        0     3969 2023-04-16 10:22:15.000000 attrs-23.1.0/tests/test_converters.py
+-rw-r--r--   0        0        0    27565 2023-04-16 10:22:15.000000 attrs-23.1.0/tests/test_dunders.py
+-rw-r--r--   0        0        0     2877 2023-04-16 10:22:15.000000 attrs-23.1.0/tests/test_filters.py
+-rw-r--r--   0        0        0    21175 2023-04-16 10:22:15.000000 attrs-23.1.0/tests/test_funcs.py
+-rw-r--r--   0        0        0    18951 2023-04-16 10:22:15.000000 attrs-23.1.0/tests/test_functional.py
+-rw-r--r--   0        0        0     6116 2023-04-16 10:22:15.000000 attrs-23.1.0/tests/test_hooks.py
+-rw-r--r--   0        0        0      347 2023-04-16 10:22:15.000000 attrs-23.1.0/tests/test_import.py
+-rw-r--r--   0        0        0      916 2023-04-16 10:22:15.000000 attrs-23.1.0/tests/test_init_subclass.py
+-rw-r--r--   0        0        0    66291 2023-04-16 10:22:15.000000 attrs-23.1.0/tests/test_make.py
+-rw-r--r--   0        0        0    40478 2023-04-16 10:22:15.000000 attrs-23.1.0/tests/test_mypy.yml
+-rw-r--r--   0        0        0    11236 2023-04-16 10:22:15.000000 attrs-23.1.0/tests/test_next_gen.py
+-rw-r--r--   0        0        0     3701 2023-04-16 10:22:15.000000 attrs-23.1.0/tests/test_packaging.py
+-rw-r--r--   0        0        0     2296 2023-04-16 10:22:15.000000 attrs-23.1.0/tests/test_pattern_matching.py
+-rw-r--r--   0        0        0     3087 2023-04-16 10:22:15.000000 attrs-23.1.0/tests/test_pyright.py
+-rw-r--r--   0        0        0    11122 2023-04-16 10:22:15.000000 attrs-23.1.0/tests/test_setattr.py
+-rw-r--r--   0        0        0    19571 2023-04-16 10:22:15.000000 attrs-23.1.0/tests/test_slots.py
+-rw-r--r--   0        0        0      440 2023-04-16 10:22:15.000000 attrs-23.1.0/tests/test_utils.py
+-rw-r--r--   0        0        0    36235 2023-04-16 10:22:15.000000 attrs-23.1.0/tests/test_validators.py
+-rw-r--r--   0        0        0     1465 2023-04-16 10:22:15.000000 attrs-23.1.0/tests/test_version_info.py
+-rw-r--r--   0        0        0     8965 2023-04-16 10:22:15.000000 attrs-23.1.0/tests/typing_example.py
+-rw-r--r--   0        0        0     1228 2023-04-16 10:22:15.000000 attrs-23.1.0/tests/utils.py
+-rw-r--r--   0        0        0      186 2023-04-16 10:22:15.000000 attrs-23.1.0/.gitignore
+-rw-r--r--   0        0        0     1109 2023-04-16 10:22:15.000000 attrs-23.1.0/LICENSE
+-rw-r--r--   0        0        0     4930 2023-04-16 10:22:15.000000 attrs-23.1.0/pyproject.toml
+-rw-r--r--   0        0        0    11348 2023-04-16 10:22:15.000000 attrs-23.1.0/PKG-INFO
```

### Comparing `attrs-22.2.0/.github/CODE_OF_CONDUCT.md` & `attrs-23.1.0/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `attrs-22.2.0/.github/CONTRIBUTING.md` & `attrs-23.1.0/.github/CONTRIBUTING.md`

 * *Files 8% similar despite different names*

```diff
@@ -38,35 +38,50 @@
 
 
 ## Local Development Environment
 
 You can (and should) run our test suite using [*tox*].
 However, you’ll probably want a more traditional environment as well.
 We highly recommend to develop using the latest Python release because we try to take advantage of modern features whenever possible.
+Also, running [*pre-commit*] later on will require the latest Python version.
 
-First create a [virtual environment](https://virtualenv.pypa.io/) so you don't break your system-wide Python installation.
-It’s out of scope for this document to list all the ways to manage virtual environments in Python, but if you don’t already have a pet way, take some time to look at tools like [*direnv*](https://hynek.me/til/python-project-local-venvs/), [*virtualfish*](https://virtualfish.readthedocs.io/), and [*virtualenvwrapper*](https://virtualenvwrapper.readthedocs.io/).
+First [fork](https://github.com/python-attrs/attrs/fork) the repository on GitHub.
 
-Next, get an up-to-date checkout of the *attrs* repository:
+Clone the fork to your computer:
 
 ```console
-$ git clone git@github.com:python-attrs/attrs.git
+$ git clone git@github.com:<your-username>/attrs.git
 ```
 
-or if you prefer to use *Git* via `https`:
+Or if you prefer to use Git via HTTPS:
 
 ```console
-$ git clone https://github.com/python-attrs/attrs.git
+$ git clone https://github.com/<your-username>/attrs.git
 ```
 
-Change into the newly created directory and **after activating your virtual environment** install an editable version of *attrs* along with its tests and docs requirements:
+Then add the *attrs* repository as *upstream* remote:
+
+```console
+$ git remote add -t main -m main --tags upstream https://github.com/python-attrs/attrs.git
+```
+
+The next step is to sync your local copy with the upstream repository:
+
+```console
+$ git fetch upstream
+```
+
+This is important to obtain eventually missing tags, which are needed to install the development version later on.
+See [#1104](https://github.com/python-attrs/attrs/issues/1104) for more information.
+
+Change into the newly created directory and after activating a virtual environment install an editable version of *attrs* along with its tests and docs requirements:
 
 ```console
 $ cd attrs
-$ python -m pip install --upgrade pip wheel setuptools  # PLEASE don't skip this step
+$ python -m pip install --upgrade pip wheel  # PLEASE don't skip this step
 $ python -m pip install -e '.[dev]'
 ```
 
 At this point,
 
 ```console
 $ python -m pytest
@@ -80,14 +95,42 @@
 ```console
 $ cd docs
 $ make html
 ```
 
 The built documentation can then be found in `docs/_build/html/`.
 
+To file a pull request, create a new branch on top of the upstream repository's `main` branch:
+
+```console
+$ git fetch upstream
+$ git checkout -b my_topical_branch upstream/main
+```
+
+Make your changes, push them to your fork (the remote *origin*):
+
+```console
+$ git push -u origin
+```
+
+and publish the PR in GitHub's web interface!
+
+After your pull request is merged and the branch is no longer needed, delete it:
+
+```console
+$ git checkout main
+$ git push --delete origin my_topical_branch && git branch -D my_topical_branch
+```
+
+Before starting to work on your next pull request, run the following command to sync your local repository with the remote *upstream*:
+
+```console
+$ git fetch upstream -u main:main
+```
+
 ---
 
 To avoid committing code that violates our style guide, we strongly advise you to install [*pre-commit*] and its hooks:
 
 ```console
 $ pre-commit install
 ```
@@ -164,15 +207,15 @@
 
   Header of New Section
   ^^^^^^^^^^^^^^^^^^^^^
 
   First line of new section.
   ```
 
-- If you add a new feature, demonstrate its awesomeness on the [examples page](https://github.com/python-attrs/attrs/blob/main/docs/examples.rst)!
+- If you add a new feature, demonstrate its awesomeness on the [examples page](https://github.com/python-attrs/attrs/blob/main/docs/examples.md)!
 
 
 ### Changelog
 
 If your change is noteworthy, there needs to be a changelog entry so our users can learn about it!
 
 To avoid merge conflicts, we use the [*Towncrier*](https://pypi.org/project/towncrier) package to manage our changelog.
```

### Comparing `attrs-22.2.0/.github/PULL_REQUEST_TEMPLATE.md` & `attrs-23.1.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files 10% similar despite different names*

```diff
@@ -20,15 +20,18 @@
 - [ ] Changes or additions to public APIs are reflected in our type stubs (files ending in ``.pyi``).
     - [ ] ...and used in the stub test file `tests/typing_example.py`.
     - [ ] If they've been added to `attr/__init__.pyi`, they've *also* been re-imported in `attrs/__init__.pyi`.
 - [ ] Updated **documentation** for changed code.
     - [ ] New functions/classes have to be added to `docs/api.rst` by hand.
     - [ ] Changes to the signature of `@attr.s()` have to be added by hand too.
     - [ ] Changed/added classes/methods/functions have appropriate `versionadded`, `versionchanged`, or `deprecated` [directives](http://www.sphinx-doc.org/en/stable/markup/para.html#directive-versionadded).
-          Find the appropriate next version in our [``__init__.py``](https://github.com/python-attrs/attrs/blob/main/src/attr/__init__.py) file.
+          The next version is the second number in the current release + 1.
+          The first number represents the current year.
+          So if the current version on PyPI is 22.2.0, the next version is gonna be 22.3.0.
+          If the next version is the first in the new year, it'll be 23.1.0.
 - [ ] Documentation in `.rst` files is written using [semantic newlines](https://rhodesmill.org/brandon/2012/one-sentence-per-line/).
 - [ ] Changes (and possible deprecations) have news fragments in [`changelog.d`](https://github.com/python-attrs/attrs/blob/main/changelog.d).
 - [ ] Consider granting [push permissions to the PR branch](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/allowing-changes-to-a-pull-request-branch-created-from-a-fork), so maintainers can fix minor issues themselves without pestering you.
 
 <!--
 If you have *any* questions to *any* of the points above, just **submit and ask**!
 This checklist is here to *help* you, not to deter you from contributing!
```

### Comparing `attrs-22.2.0/.github/sponsors/FilePreviews.svg` & `attrs-23.1.0/.github/sponsors/FilePreviews.svg`

 * *Files identical despite different names*

### Comparing `attrs-22.2.0/.github/sponsors/Sentry.svg` & `attrs-23.1.0/.github/sponsors/Sentry.svg`

 * *Files identical despite different names*

### Comparing `attrs-22.2.0/.github/sponsors/Tidelift.svg` & `attrs-23.1.0/.github/sponsors/Tidelift.svg`

 * *Files identical despite different names*

### Comparing `attrs-22.2.0/.github/sponsors/Variomedia.svg` & `attrs-23.1.0/.github/sponsors/Variomedia.svg`

 * *Files identical despite different names*

### Comparing `attrs-22.2.0/.pre-commit-config.yaml` & `attrs-23.1.0/.pre-commit-config.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 ---
 ci:
   autoupdate_schedule: monthly
 
 default_language_version:
-  python: python3.10  # needed for match
+  # Keep in sync with ci.yml/PYTHON_LATEST
+  python: python3.11
 
 repos:
   - repo: https://github.com/psf/black
-    rev: 22.10.0
+    rev: 23.3.0
     hooks:
       - id: black
 
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.0
+    rev: v3.3.1
     hooks:
       - id: pyupgrade
-        args: [--py36-plus, --keep-percent-format]
+        args: [--py37-plus, --keep-percent-format]
         exclude: "tests/test_slots.py"
 
   - repo: https://github.com/PyCQA/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
       - id: isort
-        additional_dependencies: [toml]
         files: \.py$
 
   - repo: https://github.com/asottile/yesqa
     rev: v1.4.0
     hooks:
       - id: yesqa
```

### Comparing `attrs-22.2.0/CHANGELOG.md` & `attrs-23.1.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,64 @@
 > However if you intend to build extensions on top of `attrs` you have to anticipate that.
 
 
 Changes for the upcoming release can be found in the ["changelog.d" directory](https://github.com/python-attrs/attrs/tree/main/changelog.d) in our repository.
 
 <!-- towncrier release notes start -->
 
+## [23.1.0](https://github.com/python-attrs/attrs/tree/23.1.0) - 2023-04-16
+
+### Backwards-incompatible Changes
+
+- Python 3.6 has been dropped and packaging switched to static package data using [Hatch](https://hatch.pypa.io/latest/).
+  [#993](https://github.com/python-attrs/attrs/issues/993)
+
+
+### Deprecations
+
+- The support for *zope-interface* via the `attrs.validators.provides` validator is now deprecated and will be removed in, or after, April 2024.
+
+  The presence of a C-based package in our developement dependencies has caused headaches and we're not under the impression it's used a lot.
+
+  Let us know if you're using it and we might publish it as a separate package.
+  [#1120](https://github.com/python-attrs/attrs/issues/1120)
+
+
+### Changes
+
+- `attrs.filters.exclude()` and `attrs.filters.include()` now support the passing of attribute names as strings.
+  [#1068](https://github.com/python-attrs/attrs/issues/1068)
+- `attrs.has()` and `attrs.fields()` now handle generic classes correctly.
+  [#1079](https://github.com/python-attrs/attrs/issues/1079)
+- Fix frozen exception classes when raised within e.g. `contextlib.contextmanager`, which mutates their `__traceback__` attributes.
+  [#1081](https://github.com/python-attrs/attrs/issues/1081)
+- `@frozen` now works with type checkers that implement [PEP-681](https://peps.python.org/pep-0681/) (ex. [pyright](https://github.com/microsoft/pyright/)).
+  [#1084](https://github.com/python-attrs/attrs/issues/1084)
+- Restored ability to unpickle instances pickled before 22.2.0.
+  [#1085](https://github.com/python-attrs/attrs/issues/1085)
+- `attrs.asdict()`'s and `attrs.astuple()`'s type stubs now accept the `attrs.AttrsInstance` protocol.
+  [#1090](https://github.com/python-attrs/attrs/issues/1090)
+- Fix slots class cellvar updating closure in CPython 3.8+ even when `__code__` introspection is unavailable.
+  [#1092](https://github.com/python-attrs/attrs/issues/1092)
+- `attrs.resolve_types()` can now pass `include_extras` to `typing.get_type_hints()` on Python 3.9+, and does so by default.
+  [#1099](https://github.com/python-attrs/attrs/issues/1099)
+- Added instructions for pull request workflow to `CONTRIBUTING.md`.
+  [#1105](https://github.com/python-attrs/attrs/issues/1105)
+- Added *type* parameter to `attrs.field()` function for use with `attrs.make_class()`.
+
+  Please note that type checkers ignore type metadata passed into `make_class()`, but it can be useful if you're wrapping _attrs_.
+  [#1107](https://github.com/python-attrs/attrs/issues/1107)
+- It is now possible for `attrs.evolve()` (and `attr.evolve()`) to change fields named `inst` if the instance is passed as a positional argument.
+
+  Passing the instance using the `inst` keyword argument is now deprecated and will be removed in, or after, April 2024.
+  [#1117](https://github.com/python-attrs/attrs/issues/1117)
+- `attrs.validators.optional()` now also accepts a tuple of validators (in addition to lists of validators).
+  [#1122](https://github.com/python-attrs/attrs/issues/1122)
+
+
 ## [22.2.0](https://github.com/python-attrs/attrs/tree/22.2.0) - 2022-12-21
 
 ### Backwards-incompatible Changes
 
 - Python 3.5 is not supported anymore.
   [#988](https://github.com/python-attrs/attrs/issues/988)
 
@@ -273,15 +323,15 @@
   [#782](https://github.com/python-attrs/attrs/issues/782)
 
 - To make it easier to customize attribute comparison (#435), we have added the `attr.cmp_with()` helper.
 
   See the [new docs on comparison](https://www.attrs.org/en/stable/comparison.html) for more details.
   [#787](https://github.com/python-attrs/attrs/issues/787)
 
-- Added **provisional** support for static typing in `pyright` via the [dataclass_transforms specification](https://github.com/microsoft/pyright/blob/main/specs/dataclass_transforms.md).
+- Added **provisional** support for static typing in `pyright` via [PEP 681](https://peps.python.org/pep-0681/).
   Both the `pyright` specification and `attrs` implementation may change in future versions of both projects.
 
   Your constructive feedback is welcome in both [attrs#795](https://github.com/python-attrs/attrs/issues/795) and [pyright#1782](https://github.com/microsoft/pyright/discussions/1782).
   [#796](https://github.com/python-attrs/attrs/issues/796)
 
 
 ## [20.3.0](https://github.com/python-attrs/attrs/tree/20.3.0) - 2020-11-05
```

### Comparing `attrs-22.2.0/LICENSE` & `attrs-23.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `attrs-22.2.0/PKG-INFO` & `attrs-23.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,77 +1,68 @@
 Metadata-Version: 2.1
 Name: attrs
-Version: 22.2.0
+Version: 23.1.0
 Summary: Classes Without Boilerplate
-Home-page: https://www.attrs.org/
-Author: Hynek Schlawack
-Author-email: hs@ox.cx
-Maintainer: Hynek Schlawack
-Maintainer-email: hs@ox.cx
-License: MIT
 Project-URL: Documentation, https://www.attrs.org/
 Project-URL: Changelog, https://www.attrs.org/en/stable/changelog.html
 Project-URL: Bug Tracker, https://github.com/python-attrs/attrs/issues
 Project-URL: Source Code, https://github.com/python-attrs/attrs
 Project-URL: Funding, https://github.com/sponsors/hynek
 Project-URL: Tidelift, https://tidelift.com/subscription/pkg/pypi-attrs?utm_source=pypi-attrs&utm_medium=pypi
-Project-URL: Ko-fi, https://ko-fi.com/the_hynek
-Keywords: class,attribute,boilerplate,dataclass
+Author-email: Hynek Schlawack <hs@ox.cx>
+License-Expression: MIT
+License-File: LICENSE
+Keywords: attribute,boilerplate,class
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: docs
-Provides-Extra: tests-no-zope
-Provides-Extra: tests
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Requires-Dist: importlib-metadata; python_version < '3.8'
 Provides-Extra: cov
+Requires-Dist: attrs[tests]; extra == 'cov'
+Requires-Dist: coverage[toml]>=5.3; extra == 'cov'
 Provides-Extra: dev
-Provides-Extra: tests_no_zope
-License-File: LICENSE
+Requires-Dist: attrs[docs,tests]; extra == 'dev'
+Requires-Dist: pre-commit; extra == 'dev'
+Provides-Extra: docs
+Requires-Dist: furo; extra == 'docs'
+Requires-Dist: myst-parser; extra == 'docs'
+Requires-Dist: sphinx; extra == 'docs'
+Requires-Dist: sphinx-notfound-page; extra == 'docs'
+Requires-Dist: sphinxcontrib-towncrier; extra == 'docs'
+Requires-Dist: towncrier; extra == 'docs'
+Requires-Dist: zope-interface; extra == 'docs'
+Provides-Extra: tests
+Requires-Dist: attrs[tests-no-zope]; extra == 'tests'
+Requires-Dist: zope-interface; extra == 'tests'
+Provides-Extra: tests-no-zope
+Requires-Dist: cloudpickle; platform_python_implementation == 'CPython' and extra == 'tests-no-zope'
+Requires-Dist: hypothesis; extra == 'tests-no-zope'
+Requires-Dist: mypy>=1.1.1; platform_python_implementation == 'CPython' and extra == 'tests-no-zope'
+Requires-Dist: pympler; extra == 'tests-no-zope'
+Requires-Dist: pytest-mypy-plugins; platform_python_implementation == 'CPython' and python_version < '3.11' and extra == 'tests-no-zope'
+Requires-Dist: pytest-xdist[psutil]; extra == 'tests-no-zope'
+Requires-Dist: pytest>=4.3.0; extra == 'tests-no-zope'
+Description-Content-Type: text/markdown
 
 <p align="center">
   <a href="https://www.attrs.org/">
     <img src="https://raw.githubusercontent.com/python-attrs/attrs/main/docs/_static/attrs_logo.svg" width="35%" alt="attrs" />
   </a>
 </p>
 
 
-<p align="center">
-   <a href="https://www.attrs.org/en/stable/">
-       <img src="https://img.shields.io/badge/Docs-RTD-black" alt="Documentation" />
-   </a>
-   <a href="https://github.com/python-attrs/attrs/blob/main/LICENSE">
-      <img src="https://img.shields.io/badge/license-MIT-C06524" alt="License: MIT" />
-   </a>
-   <a href="https://bestpractices.coreinfrastructure.org/projects/6482"><img src="https://bestpractices.coreinfrastructure.org/projects/6482/badge"></a>
-   <a href="https://pypi.org/project/attrs/">
-      <img src="https://img.shields.io/pypi/v/attrs" />
-   </a>
-   <a href="https://pepy.tech/project/attrs">
-      <img src="https://static.pepy.tech/personalized-badge/attrs?period=month&units=international_system&left_color=grey&right_color=blue&left_text=Downloads%20/%20Month" alt="Downloads per month" />
-   </a>
-   <a href="https://zenodo.org/badge/latestdoi/29918975"><img src="https://zenodo.org/badge/29918975.svg" alt="DOI"></a>
-</p>
-
-<!-- teaser-begin -->
-
 *attrs* is the Python package that will bring back the **joy** of **writing classes** by relieving you from the drudgery of implementing object protocols (aka [dunder methods](https://www.attrs.org/en/latest/glossary.html#term-dunder-methods)).
 [Trusted by NASA](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-github-profile/customizing-your-profile/personalizing-your-profile#list-of-qualifying-repositories-for-mars-2020-helicopter-contributor-achievement) for Mars missions since 2020!
 
 Its main goal is to help you to write **concise** and **correct** software without slowing down your code.
 
 
 ## Sponsors
@@ -181,71 +172,72 @@
 - [**Documentation**](https://www.attrs.org/)
 - [**PyPI**](https://pypi.org/project/attrs/)
 - [**Source Code**](https://github.com/python-attrs/attrs)
 - [**Contributing**](https://github.com/python-attrs/attrs/blob/main/.github/CONTRIBUTING.md)
 - [**Third-party Extensions**](https://github.com/python-attrs/attrs/wiki/Extensions-to-attrs)
 - **License**: [MIT](https://www.attrs.org/en/latest/license.html)
 - **Get Help**: please use the `python-attrs` tag on [StackOverflow](https://stackoverflow.com/questions/tagged/python-attrs)
-- **Supported Python Versions**: 3.6 and later
+- **Supported Python Versions**: 3.7 and later
 
 
 ### *attrs* for Enterprise
 
 Available as part of the Tidelift Subscription.
 
 The maintainers of *attrs* and thousands of other packages are working with Tidelift to deliver commercial support and maintenance for the open source packages you use to build your applications.
 Save time, reduce risk, and improve code health, while paying the maintainers of the exact packages you use.
 [Learn more.](https://tidelift.com/subscription/pkg/pypi-attrs?utm_source=pypi-attrs&utm_medium=referral&utm_campaign=enterprise&utm_term=repo)
 
-
-## Changes in This Release
+## Release Information
 
 ### Backwards-incompatible Changes
 
-- Python 3.5 is not supported anymore.
-  [#988](https://github.com/python-attrs/attrs/issues/988)
+- Python 3.6 has been dropped and packaging switched to static package data using [Hatch](https://hatch.pypa.io/latest/).
+  [#993](https://github.com/python-attrs/attrs/issues/993)
 
 
 ### Deprecations
 
-- Python 3.6 is now deprecated and support will be removed in the next release.
-  [#1017](https://github.com/python-attrs/attrs/issues/1017)
+- The support for *zope-interface* via the `attrs.validators.provides` validator is now deprecated and will be removed in, or after, April 2024.
+
+  The presence of a C-based package in our developement dependencies has caused headaches and we're not under the impression it's used a lot.
+
+  Let us know if you're using it and we might publish it as a separate package.
+  [#1120](https://github.com/python-attrs/attrs/issues/1120)
 
 
 ### Changes
 
-- `attrs.field()` now supports an *alias* option for explicit `__init__` argument names.
+- `attrs.filters.exclude()` and `attrs.filters.include()` now support the passing of attribute names as strings.
+  [#1068](https://github.com/python-attrs/attrs/issues/1068)
+- `attrs.has()` and `attrs.fields()` now handle generic classes correctly.
+  [#1079](https://github.com/python-attrs/attrs/issues/1079)
+- Fix frozen exception classes when raised within e.g. `contextlib.contextmanager`, which mutates their `__traceback__` attributes.
+  [#1081](https://github.com/python-attrs/attrs/issues/1081)
+- `@frozen` now works with type checkers that implement [PEP-681](https://peps.python.org/pep-0681/) (ex. [pyright](https://github.com/microsoft/pyright/)).
+  [#1084](https://github.com/python-attrs/attrs/issues/1084)
+- Restored ability to unpickle instances pickled before 22.2.0.
+  [#1085](https://github.com/python-attrs/attrs/issues/1085)
+- `attrs.asdict()`'s and `attrs.astuple()`'s type stubs now accept the `attrs.AttrsInstance` protocol.
+  [#1090](https://github.com/python-attrs/attrs/issues/1090)
+- Fix slots class cellvar updating closure in CPython 3.8+ even when `__code__` introspection is unavailable.
+  [#1092](https://github.com/python-attrs/attrs/issues/1092)
+- `attrs.resolve_types()` can now pass `include_extras` to `typing.get_type_hints()` on Python 3.9+, and does so by default.
+  [#1099](https://github.com/python-attrs/attrs/issues/1099)
+- Added instructions for pull request workflow to `CONTRIBUTING.md`.
+  [#1105](https://github.com/python-attrs/attrs/issues/1105)
+- Added *type* parameter to `attrs.field()` function for use with `attrs.make_class()`.
+
+  Please note that type checkers ignore type metadata passed into `make_class()`, but it can be useful if you're wrapping _attrs_.
+  [#1107](https://github.com/python-attrs/attrs/issues/1107)
+- It is now possible for `attrs.evolve()` (and `attr.evolve()`) to change fields named `inst` if the instance is passed as a positional argument.
+
+  Passing the instance using the `inst` keyword argument is now deprecated and will be removed in, or after, April 2024.
+  [#1117](https://github.com/python-attrs/attrs/issues/1117)
+- `attrs.validators.optional()` now also accepts a tuple of validators (in addition to lists of validators).
+  [#1122](https://github.com/python-attrs/attrs/issues/1122)
+
 
-  Get `__init__` signatures matching any taste, peculiar or plain!
-  The [PEP 681 compatible](https://peps.python.org/pep-0681/#field-specifier-parameters) *alias* option can be use to override private attribute name mangling, or add other arbitrary field argument name overrides.
-  [#950](https://github.com/python-attrs/attrs/issues/950)
-- `attrs.NOTHING` is now an enum value, making it possible to use with e.g. [`typing.Literal`](https://docs.python.org/3/library/typing.html#typing.Literal).
-  [#983](https://github.com/python-attrs/attrs/issues/983)
-- Added missing re-import of `attr.AttrsInstance` to the `attrs` namespace.
-  [#987](https://github.com/python-attrs/attrs/issues/987)
-- Fix slight performance regression in classes with custom `__setattr__` and speedup even more.
-  [#991](https://github.com/python-attrs/attrs/issues/991)
-- Class-creation performance improvements by switching performance-sensitive templating operations to f-strings.
-
-  You can expect an improvement of about 5% -- even for very simple classes.
-  [#995](https://github.com/python-attrs/attrs/issues/995)
-- `attrs.has()` is now a [`TypeGuard`](https://docs.python.org/3/library/typing.html#typing.TypeGuard) for `AttrsInstance`.
-  That means that type checkers know a class is an instance of an `attrs` class if you check it using `attrs.has()` (or `attr.has()`) first.
-  [#997](https://github.com/python-attrs/attrs/issues/997)
-- Made `attrs.AttrsInstance` stub available at runtime and fixed type errors related to the usage of `attrs.AttrsInstance` in *Pyright*.
-  [#999](https://github.com/python-attrs/attrs/issues/999)
-- On Python 3.10 and later, call [`abc.update_abstractmethods()`](https://docs.python.org/3/library/abc.html#abc.update_abstractmethods) on dict classes after creation.
-  This improves the detection of abstractness.
-  [#1001](https://github.com/python-attrs/attrs/issues/1001)
-- *attrs*'s pickling methods now use dicts instead of tuples.
-  That is safer and more robust across different versions of a class.
-  [#1009](https://github.com/python-attrs/attrs/issues/1009)
-- Added `attrs.validators.not_(wrapped_validator)` to logically invert *wrapped_validator* by accepting only values where *wrapped_validator* rejects the value with a `ValueError` or `TypeError` (by default, exception types configurable).
-  [#1010](https://github.com/python-attrs/attrs/issues/1010)
-- The type stubs for `attrs.cmp_using()` now have default values.
-  [#1027](https://github.com/python-attrs/attrs/issues/1027)
-- To conform with [PEP 681](https://peps.python.org/pep-0681/), `attr.s()` and `attrs.define()` now accept *unsafe_hash* in addition to *hash*.
-  [#1065](https://github.com/python-attrs/attrs/issues/1065)
 
 ---
 
 [Full changelog](https://www.attrs.org/en/stable/changelog.html)
```

#### html2text {}

```diff
@@ -1,36 +1,44 @@
-Metadata-Version: 2.1 Name: attrs Version: 22.2.0 Summary: Classes Without
-Boilerplate Home-page: https://www.attrs.org/ Author: Hynek Schlawack Author-
-email: hs@ox.cx Maintainer: Hynek Schlawack Maintainer-email: hs@ox.cx License:
-MIT Project-URL: Documentation, https://www.attrs.org/ Project-URL: Changelog,
-https://www.attrs.org/en/stable/changelog.html Project-URL: Bug Tracker, https:
-//github.com/python-attrs/attrs/issues Project-URL: Source Code, https://
-github.com/python-attrs/attrs Project-URL: Funding, https://github.com/
+Metadata-Version: 2.1 Name: attrs Version: 23.1.0 Summary: Classes Without
+Boilerplate Project-URL: Documentation, https://www.attrs.org/ Project-URL:
+Changelog, https://www.attrs.org/en/stable/changelog.html Project-URL: Bug
+Tracker, https://github.com/python-attrs/attrs/issues Project-URL: Source Code,
+https://github.com/python-attrs/attrs Project-URL: Funding, https://github.com/
 sponsors/hynek Project-URL: Tidelift, https://tidelift.com/subscription/pkg/
-pypi-attrs?utm_source=pypi-attrs&utm_medium=pypi Project-URL: Ko-fi, https://
-ko-fi.com/the_hynek Keywords: class,attribute,boilerplate,dataclass Classifier:
-Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
-Developers Classifier: Natural Language :: English Classifier: License :: OSI
-Approved :: MIT License Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.6 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Programming Language :: Python :: Implementation ::
-CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6 Description-Content-Type: text/markdown Provides-Extra:
-docs Provides-Extra: tests-no-zope Provides-Extra: tests Provides-Extra: cov
-Provides-Extra: dev Provides-Extra: tests_no_zope License-File: LICENSE
+pypi-attrs?utm_source=pypi-attrs&utm_medium=pypi Author-email: Hynek Schlawack
+ox.cx> License-Expression: MIT License-File: LICENSE Keywords:
+attribute,boilerplate,class Classifier: Development Status :: 5 - Production/
+Stable Classifier: Intended Audience :: Developers Classifier: License :: OSI
+Approved :: MIT License Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: Implementation :: CPython Classifier: Programming
+Language :: Python :: Implementation :: PyPy Classifier: Typing :: Typed
+Requires-Python: >=3.7 Requires-Dist: importlib-metadata; python_version <
+'3.8' Provides-Extra: cov Requires-Dist: attrs[tests]; extra == 'cov' Requires-
+Dist: coverage[toml]>=5.3; extra == 'cov' Provides-Extra: dev Requires-Dist:
+attrs[docs,tests]; extra == 'dev' Requires-Dist: pre-commit; extra == 'dev'
+Provides-Extra: docs Requires-Dist: furo; extra == 'docs' Requires-Dist: myst-
+parser; extra == 'docs' Requires-Dist: sphinx; extra == 'docs' Requires-Dist:
+sphinx-notfound-page; extra == 'docs' Requires-Dist: sphinxcontrib-towncrier;
+extra == 'docs' Requires-Dist: towncrier; extra == 'docs' Requires-Dist: zope-
+interface; extra == 'docs' Provides-Extra: tests Requires-Dist: attrs[tests-no-
+zope]; extra == 'tests' Requires-Dist: zope-interface; extra == 'tests'
+Provides-Extra: tests-no-zope Requires-Dist: cloudpickle;
+platform_python_implementation == 'CPython' and extra == 'tests-no-zope'
+Requires-Dist: hypothesis; extra == 'tests-no-zope' Requires-Dist: mypy>=1.1.1;
+platform_python_implementation == 'CPython' and extra == 'tests-no-zope'
+Requires-Dist: pympler; extra == 'tests-no-zope' Requires-Dist: pytest-mypy-
+plugins; platform_python_implementation == 'CPython' and python_version <
+'3.11' and extra == 'tests-no-zope' Requires-Dist: pytest-xdist[psutil]; extra
+== 'tests-no-zope' Requires-Dist: pytest>=4.3.0; extra == 'tests-no-zope'
+Description-Content-Type: text/markdown
                                     [attrs]
- [Documentation] [License:_MIT] [https://bestpractices.coreinfrastructure.org/
-   projects/6482/badge] [https://img.shields.io/pypi/v/attrs] [Downloads_per
-                                 month] [DOI]
- *attrs* is the Python package that will bring back the **joy** of **writing
+*attrs* is the Python package that will bring back the **joy** of **writing
 classes** by relieving you from the drudgery of implementing object protocols
 (aka [dunder methods](https://www.attrs.org/en/latest/glossary.html#term-
 dunder-methods)). [Trusted by NASA](https://docs.github.com/en/account-and-
 profile/setting-up-and-managing-your-github-profile/customizing-your-profile/
 personalizing-your-profile#list-of-qualifying-repositories-for-mars-2020-
 helicopter-contributor-achievement) for Mars missions since 2020! Its main goal
 is to help you to write **concise** and **correct** software without slowing
@@ -80,58 +88,55 @@
 changelog.html) - [**Documentation**](https://www.attrs.org/) - [**PyPI**]
 (https://pypi.org/project/attrs/) - [**Source Code**](https://github.com/
 python-attrs/attrs) - [**Contributing**](https://github.com/python-attrs/attrs/
 blob/main/.github/CONTRIBUTING.md) - [**Third-party Extensions**](https://
 github.com/python-attrs/attrs/wiki/Extensions-to-attrs) - **License**: [MIT]
 (https://www.attrs.org/en/latest/license.html) - **Get Help**: please use the
 `python-attrs` tag on [StackOverflow](https://stackoverflow.com/questions/
-tagged/python-attrs) - **Supported Python Versions**: 3.6 and later ### *attrs*
+tagged/python-attrs) - **Supported Python Versions**: 3.7 and later ### *attrs*
 for Enterprise Available as part of the Tidelift Subscription. The maintainers
 of *attrs* and thousands of other packages are working with Tidelift to deliver
 commercial support and maintenance for the open source packages you use to
 build your applications. Save time, reduce risk, and improve code health, while
 paying the maintainers of the exact packages you use. [Learn more.](https://
 tidelift.com/subscription/pkg/pypi-attrs?utm_source=pypi-
-attrs&utm_medium=referral&utm_campaign=enterprise&utm_term=repo) ## Changes in
-This Release ### Backwards-incompatible Changes - Python 3.5 is not supported
-anymore. [#988](https://github.com/python-attrs/attrs/issues/988) ###
-Deprecations - Python 3.6 is now deprecated and support will be removed in the
-next release. [#1017](https://github.com/python-attrs/attrs/issues/1017) ###
-Changes - `attrs.field()` now supports an *alias* option for explicit
-`__init__` argument names. Get `__init__` signatures matching any taste,
-peculiar or plain! The [PEP 681 compatible](https://peps.python.org/pep-0681/
-#field-specifier-parameters) *alias* option can be use to override private
-attribute name mangling, or add other arbitrary field argument name overrides.
-[#950](https://github.com/python-attrs/attrs/issues/950) - `attrs.NOTHING` is
-now an enum value, making it possible to use with e.g. [`typing.Literal`]
-(https://docs.python.org/3/library/typing.html#typing.Literal). [#983](https://
-github.com/python-attrs/attrs/issues/983) - Added missing re-import of
-`attr.AttrsInstance` to the `attrs` namespace. [#987](https://github.com/
-python-attrs/attrs/issues/987) - Fix slight performance regression in classes
-with custom `__setattr__` and speedup even more. [#991](https://github.com/
-python-attrs/attrs/issues/991) - Class-creation performance improvements by
-switching performance-sensitive templating operations to f-strings. You can
-expect an improvement of about 5% -- even for very simple classes. [#995]
-(https://github.com/python-attrs/attrs/issues/995) - `attrs.has()` is now a
-[`TypeGuard`](https://docs.python.org/3/library/typing.html#typing.TypeGuard)
-for `AttrsInstance`. That means that type checkers know a class is an instance
-of an `attrs` class if you check it using `attrs.has()` (or `attr.has()`)
-first. [#997](https://github.com/python-attrs/attrs/issues/997) - Made
-`attrs.AttrsInstance` stub available at runtime and fixed type errors related
-to the usage of `attrs.AttrsInstance` in *Pyright*. [#999](https://github.com/
-python-attrs/attrs/issues/999) - On Python 3.10 and later, call
-[`abc.update_abstractmethods()`](https://docs.python.org/3/library/
-abc.html#abc.update_abstractmethods) on dict classes after creation. This
-improves the detection of abstractness. [#1001](https://github.com/python-
-attrs/attrs/issues/1001) - *attrs*'s pickling methods now use dicts instead of
-tuples. That is safer and more robust across different versions of a class.
-[#1009](https://github.com/python-attrs/attrs/issues/1009) - Added
-`attrs.validators.not_(wrapped_validator)` to logically invert
-*wrapped_validator* by accepting only values where *wrapped_validator* rejects
-the value with a `ValueError` or `TypeError` (by default, exception types
-configurable). [#1010](https://github.com/python-attrs/attrs/issues/1010) - The
-type stubs for `attrs.cmp_using()` now have default values. [#1027](https://
-github.com/python-attrs/attrs/issues/1027) - To conform with [PEP 681](https://
-peps.python.org/pep-0681/), `attr.s()` and `attrs.define()` now accept
-*unsafe_hash* in addition to *hash*. [#1065](https://github.com/python-attrs/
-attrs/issues/1065) --- [Full changelog](https://www.attrs.org/en/stable/
-changelog.html)
+attrs&utm_medium=referral&utm_campaign=enterprise&utm_term=repo) ## Release
+Information ### Backwards-incompatible Changes - Python 3.6 has been dropped
+and packaging switched to static package data using [Hatch](https://
+hatch.pypa.io/latest/). [#993](https://github.com/python-attrs/attrs/issues/
+993) ### Deprecations - The support for *zope-interface* via the
+`attrs.validators.provides` validator is now deprecated and will be removed in,
+or after, April 2024. The presence of a C-based package in our developement
+dependencies has caused headaches and we're not under the impression it's used
+a lot. Let us know if you're using it and we might publish it as a separate
+package. [#1120](https://github.com/python-attrs/attrs/issues/1120) ### Changes
+- `attrs.filters.exclude()` and `attrs.filters.include()` now support the
+passing of attribute names as strings. [#1068](https://github.com/python-attrs/
+attrs/issues/1068) - `attrs.has()` and `attrs.fields()` now handle generic
+classes correctly. [#1079](https://github.com/python-attrs/attrs/issues/1079) -
+Fix frozen exception classes when raised within e.g.
+`contextlib.contextmanager`, which mutates their `__traceback__` attributes.
+[#1081](https://github.com/python-attrs/attrs/issues/1081) - `@frozen` now
+works with type checkers that implement [PEP-681](https://peps.python.org/pep-
+0681/) (ex. [pyright](https://github.com/microsoft/pyright/)). [#1084](https://
+github.com/python-attrs/attrs/issues/1084) - Restored ability to unpickle
+instances pickled before 22.2.0. [#1085](https://github.com/python-attrs/attrs/
+issues/1085) - `attrs.asdict()`'s and `attrs.astuple()`'s type stubs now accept
+the `attrs.AttrsInstance` protocol. [#1090](https://github.com/python-attrs/
+attrs/issues/1090) - Fix slots class cellvar updating closure in CPython 3.8+
+even when `__code__` introspection is unavailable. [#1092](https://github.com/
+python-attrs/attrs/issues/1092) - `attrs.resolve_types()` can now pass
+`include_extras` to `typing.get_type_hints()` on Python 3.9+, and does so by
+default. [#1099](https://github.com/python-attrs/attrs/issues/1099) - Added
+instructions for pull request workflow to `CONTRIBUTING.md`. [#1105](https://
+github.com/python-attrs/attrs/issues/1105) - Added *type* parameter to
+`attrs.field()` function for use with `attrs.make_class()`. Please note that
+type checkers ignore type metadata passed into `make_class()`, but it can be
+useful if you're wrapping _attrs_. [#1107](https://github.com/python-attrs/
+attrs/issues/1107) - It is now possible for `attrs.evolve()` (and `attr.evolve
+()`) to change fields named `inst` if the instance is passed as a positional
+argument. Passing the instance using the `inst` keyword argument is now
+deprecated and will be removed in, or after, April 2024. [#1117](https://
+github.com/python-attrs/attrs/issues/1117) - `attrs.validators.optional()` now
+also accepts a tuple of validators (in addition to lists of validators).
+[#1122](https://github.com/python-attrs/attrs/issues/1122) --- [Full changelog]
+(https://www.attrs.org/en/stable/changelog.html)
```

### Comparing `attrs-22.2.0/README.md` & `attrs-23.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,14 @@
       <picture>
          <source srcset="https://raw.githubusercontent.com/python-attrs/attrs/main/docs/_static/attrs_logo_white.svg" media="(prefers-color-scheme: dark)">
          <img src="https://raw.githubusercontent.com/python-attrs/attrs/main/docs/_static/attrs_logo.svg" width="35%" alt="attrs" />
       </picture>
    </a>
 </p>
 
-<!-- logo-end -->
-
 <p align="center">
    <a href="https://www.attrs.org/en/stable/">
        <img src="https://img.shields.io/badge/Docs-RTD-black" alt="Documentation" />
    </a>
    <a href="https://github.com/python-attrs/attrs/blob/main/LICENSE">
       <img src="https://img.shields.io/badge/license-MIT-C06524" alt="License: MIT" />
    </a>
@@ -141,15 +139,15 @@
 - [**Documentation**](https://www.attrs.org/)
 - [**PyPI**](https://pypi.org/project/attrs/)
 - [**Source Code**](https://github.com/python-attrs/attrs)
 - [**Contributing**](https://github.com/python-attrs/attrs/blob/main/.github/CONTRIBUTING.md)
 - [**Third-party Extensions**](https://github.com/python-attrs/attrs/wiki/Extensions-to-attrs)
 - **License**: [MIT](https://www.attrs.org/en/latest/license.html)
 - **Get Help**: please use the `python-attrs` tag on [StackOverflow](https://stackoverflow.com/questions/tagged/python-attrs)
-- **Supported Python Versions**: 3.6 and later
+- **Supported Python Versions**: 3.7 and later
 
 
 ### *attrs* for Enterprise
 
 Available as part of the Tidelift Subscription.
 
 The maintainers of *attrs* and thousands of other packages are working with Tidelift to deliver commercial support and maintenance for the open source packages you use to build your applications.
```

#### html2text {}

```diff
@@ -56,15 +56,15 @@
 changelog.html) - [**Documentation**](https://www.attrs.org/) - [**PyPI**]
 (https://pypi.org/project/attrs/) - [**Source Code**](https://github.com/
 python-attrs/attrs) - [**Contributing**](https://github.com/python-attrs/attrs/
 blob/main/.github/CONTRIBUTING.md) - [**Third-party Extensions**](https://
 github.com/python-attrs/attrs/wiki/Extensions-to-attrs) - **License**: [MIT]
 (https://www.attrs.org/en/latest/license.html) - **Get Help**: please use the
 `python-attrs` tag on [StackOverflow](https://stackoverflow.com/questions/
-tagged/python-attrs) - **Supported Python Versions**: 3.6 and later ### *attrs*
+tagged/python-attrs) - **Supported Python Versions**: 3.7 and later ### *attrs*
 for Enterprise Available as part of the Tidelift Subscription. The maintainers
 of *attrs* and thousands of other packages are working with Tidelift to deliver
 commercial support and maintenance for the open source packages you use to
 build your applications. Save time, reduce risk, and improve code health, while
 paying the maintainers of the exact packages you use. [Learn more.](https://
 tidelift.com/subscription/pkg/pypi-attrs?utm_source=pypi-
 attrs&utm_medium=referral&utm_campaign=enterprise&utm_term=repo)
```

### Comparing `attrs-22.2.0/changelog.d/towncrier_template.md.jinja` & `attrs-23.1.0/changelog.d/towncrier_template.md.jinja`

 * *Files identical despite different names*

### Comparing `attrs-22.2.0/conftest.py` & `attrs-23.1.0/conftest.py`

 * *Files identical despite different names*

### Comparing `attrs-22.2.0/docs/Makefile` & `attrs-23.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `attrs-22.2.0/docs/_static/attrs_logo.png` & `attrs-23.1.0/docs/_static/attrs_logo.png`

 * *Files identical despite different names*

### Comparing `attrs-22.2.0/docs/_static/attrs_logo.svg` & `attrs-23.1.0/docs/_static/attrs_logo.svg`

 * *Files identical despite different names*

### Comparing `attrs-22.2.0/docs/_static/attrs_logo_white.png` & `attrs-23.1.0/docs/_static/attrs_logo_white.png`

 * *Files identical despite different names*

### Comparing `attrs-22.2.0/docs/_static/attrs_logo_white.svg` & `attrs-23.1.0/docs/_static/attrs_logo_white.svg`

 * *Files identical despite different names*

### Comparing `attrs-22.2.0/docs/api.rst` & `attrs-23.1.0/docs/api.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,223 +1,129 @@
 API Reference
 =============
 
-.. currentmodule:: attr
+.. module:: attrs
 
-*attrs* works by decorating a class using `attrs.define` or `attr.s` and then optionally defining attributes on the class using `attrs.field`, `attr.ib`, or a type annotation.
+*attrs* works by decorating a class using `attrs.define` or `attr.s` and then defining attributes on the class using `attrs.field`, `attr.ib`, or type annotations.
 
-If you're confused by the many names, please check out `names` for clarification.
+What follows is the API explanation, if you'd like a more hands-on tutorial, have a look at `examples`.
 
-What follows is the API explanation, if you'd like a more hands-on introduction, have a look at `examples`.
+If you're confused by the many names, please check out `names` for clarification, but the `TL;DR <https://en.wikipedia.org/wiki/TL;DR>`_ is that as of version 21.3.0, *attrs* consists of **two** top-level package names:
 
-As of version 21.3.0, *attrs* consists of **two** top-level package names:
-
-- The classic ``attr`` that powered the venerable `attr.s` and `attr.ib`
-- The modern ``attrs`` that only contains most modern APIs and relies on `attrs.define` and `attrs.field` to define your classes.
+- The classic ``attr`` that powers the venerable `attr.s` and `attr.ib`.
+- The newer ``attrs`` that only contains most modern APIs and relies on `attrs.define` and `attrs.field` to define your classes.
   Additionally it offers some ``attr`` APIs with nicer defaults (e.g. `attrs.asdict`).
 
-The ``attrs`` namespace is built *on top of* ``attr`` which will *never* go away.
+The ``attrs`` namespace is built *on top of* ``attr`` -- which will *never* go away -- and is just as stable, since it doesn't constitute a rewrite.
+To keep repetition low and this document at a reasonable size, the ``attr`` namespace is `documented on a separate page <api-attr>`, though.
 
 
 Core
 ----
 
-.. note::
-
-  Please note that the ``attrs`` namespace has been added in version 21.3.0.
-  Most of the objects are simply re-imported from ``attr``.
-  Therefore if a class, method, or function claims that it has been added in an older version, it is only available in the ``attr`` namespace.
-
 .. autodata:: attrs.NOTHING
    :no-value:
 
 .. autofunction:: attrs.define
 
-.. function:: attrs.mutable(same_as_define)
+.. function:: mutable(same_as_define)
 
-   Alias for `attrs.define`.
+   Same as `attrs.define`.
 
    .. versionadded:: 20.1.0
 
-.. function:: attrs.frozen(same_as_define)
+.. function:: frozen(same_as_define)
 
    Behaves the same as `attrs.define` but sets *frozen=True* and *on_setattr=None*.
 
    .. versionadded:: 20.1.0
 
-.. autofunction:: attrs.field
-
-.. function:: define
-
-   Old import path for `attrs.define`.
-
-.. function:: mutable
+.. autofunction:: field
 
-   Old import path for `attrs.mutable`.
-
-.. function:: frozen
-
-   Old import path for `attrs.frozen`.
-
-.. function:: field
-
-   Old import path for `attrs.field`.
-
-.. autoclass:: attrs.Attribute
+.. autoclass:: Attribute
    :members: evolve
 
    For example:
 
    .. doctest::
 
-      >>> import attr
-      >>> @attr.s
+      >>> import attrs
+      >>> from attrs import define, field
+
+      >>> @define
       ... class C:
-      ...     x = attr.ib()
-      >>> attr.fields(C).x
+      ...     x = field()
+      >>> attrs.fields(C).x
       Attribute(name='x', default=NOTHING, validator=None, repr=True, eq=True, eq_key=None, order=True, order_key=None, hash=None, init=True, metadata=mappingproxy({}), type=None, converter=None, kw_only=False, inherited=False, on_setattr=None, alias='x')
 
 
-.. autofunction:: attrs.make_class
+.. autofunction:: make_class
 
    This is handy if you want to programmatically create classes.
 
    For example:
 
    .. doctest::
 
-      >>> C1 = attr.make_class("C1", ["x", "y"])
+      >>> C1 = attrs.make_class("C1", ["x", "y"])
       >>> C1(1, 2)
       C1(x=1, y=2)
-      >>> C2 = attr.make_class("C2", {"x": attr.ib(default=42),
-      ...                             "y": attr.ib(default=attr.Factory(list))})
+      >>> C2 = attrs.make_class("C2", {
+      ...     "x": field(default=42),
+      ...     "y": field(factory=list)
+      ... })
       >>> C2()
       C2(x=42, y=[])
 
 
-.. autoclass:: attrs.Factory
+.. autoclass:: Factory
 
    For example:
 
    .. doctest::
 
-      >>> @attr.s
+      >>> @define
       ... class C:
-      ...     x = attr.ib(default=attr.Factory(list))
-      ...     y = attr.ib(default=attr.Factory(
+      ...     x = field(default=attrs.Factory(list))
+      ...     y = field(default=attrs.Factory(
       ...         lambda self: set(self.x),
       ...         takes_self=True)
       ...     )
       >>> C()
       C(x=[], y=set())
       >>> C([1, 2, 3])
       C(x=[1, 2, 3], y={1, 2, 3})
 
 
-Classic
-~~~~~~~
-
-.. data:: attr.NOTHING
-
-   Same as `attrs.NOTHING`.
-
-.. autofunction:: attr.s(these=None, repr_ns=None, repr=None, cmp=None, hash=None, init=None, slots=False, frozen=False, weakref_slot=True, str=False, auto_attribs=False, kw_only=False, cache_hash=False, auto_exc=False, eq=None, order=None, auto_detect=False, collect_by_mro=False, getstate_setstate=None, on_setattr=None, field_transformer=None, match_args=True, unsafe_hash=None)
-
-   .. note::
-
-      *attrs* also comes with a serious-business alias ``attr.attrs``.
-
-   For example:
-
-   .. doctest::
-
-      >>> import attr
-      >>> @attr.s
-      ... class C:
-      ...     _private = attr.ib()
-      >>> C(private=42)
-      C(_private=42)
-      >>> class D:
-      ...     def __init__(self, x):
-      ...         self.x = x
-      >>> D(1)
-      <D object at ...>
-      >>> D = attr.s(these={"x": attr.ib()}, init=False)(D)
-      >>> D(1)
-      D(x=1)
-      >>> @attr.s(auto_exc=True)
-      ... class Error(Exception):
-      ...     x = attr.ib()
-      ...     y = attr.ib(default=42, init=False)
-      >>> Error("foo")
-      Error(x='foo', y=42)
-      >>> raise Error("foo")
-      Traceback (most recent call last):
-         ...
-      Error: ('foo', 42)
-      >>> raise ValueError("foo", 42)   # for comparison
-      Traceback (most recent call last):
-         ...
-      ValueError: ('foo', 42)
-
-
-.. autofunction:: attr.ib
-
-   .. note::
-
-      *attrs* also comes with a serious-business alias ``attr.attrib``.
-
-   The object returned by `attr.ib` also allows for setting the default and the validator using decorators:
-
-   .. doctest::
-
-      >>> @attr.s
-      ... class C:
-      ...     x = attr.ib()
-      ...     y = attr.ib()
-      ...     @x.validator
-      ...     def _any_name_except_a_name_of_an_attribute(self, attribute, value):
-      ...         if value < 0:
-      ...             raise ValueError("x must be positive")
-      ...     @y.default
-      ...     def _any_name_except_a_name_of_an_attribute(self):
-      ...         return self.x + 1
-      >>> C(1)
-      C(x=1, y=2)
-      >>> C(-1)
-      Traceback (most recent call last):
-          ...
-      ValueError: x must be positive
-
-
-
 Exceptions
 ----------
 
+.. module:: attrs.exceptions
+
 All exceptions are available from both ``attr.exceptions`` and ``attrs.exceptions`` and are the same thing.
 That means that it doesn't matter from from which namespace they've been raised and/or caught:
 
 .. doctest::
 
    >>> import attrs, attr
    >>> try:
    ...     raise attrs.exceptions.FrozenError()
    ... except attr.exceptions.FrozenError:
    ...     print("this works!")
    this works!
 
-.. autoexception:: attrs.exceptions.PythonTooOldError
-.. autoexception:: attrs.exceptions.FrozenError
-.. autoexception:: attrs.exceptions.FrozenInstanceError
-.. autoexception:: attrs.exceptions.FrozenAttributeError
-.. autoexception:: attrs.exceptions.AttrsAttributeNotFoundError
-.. autoexception:: attrs.exceptions.NotAnAttrsClassError
-.. autoexception:: attrs.exceptions.DefaultAlreadySetError
-.. autoexception:: attrs.exceptions.UnannotatedAttributeError
-.. autoexception:: attrs.exceptions.NotCallableError
+.. autoexception:: PythonTooOldError
+.. autoexception:: FrozenError
+.. autoexception:: FrozenInstanceError
+.. autoexception:: FrozenAttributeError
+.. autoexception:: AttrsAttributeNotFoundError
+.. autoexception:: NotAnAttrsClassError
+.. autoexception:: DefaultAlreadySetError
+.. autoexception:: NotCallableError
+.. autoexception:: UnannotatedAttributeError
 
    For example::
 
        @attr.s(auto_attribs=True)
        class C:
            x: int
            y = attr.ib()  # <- ERROR!
@@ -226,40 +132,35 @@
 .. _helpers:
 
 Helpers
 -------
 
 *attrs* comes with a bunch of helper methods that make working with it easier:
 
-.. autofunction:: attrs.cmp_using
-.. function:: attr.cmp_using
+.. currentmodule:: attrs
 
-   Same as `attrs.cmp_using`.
+.. autofunction:: attrs.cmp_using
 
 .. autofunction:: attrs.fields
 
    For example:
 
    .. doctest::
 
-      >>> @attr.s
+      >>> @define
       ... class C:
-      ...     x = attr.ib()
-      ...     y = attr.ib()
+      ...     x = field()
+      ...     y = field()
       >>> attrs.fields(C)
       (Attribute(name='x', default=NOTHING, validator=None, repr=True, eq=True, eq_key=None, order=True, order_key=None, hash=None, init=True, metadata=mappingproxy({}), type=None, converter=None, kw_only=False, inherited=False, on_setattr=None, alias='x'), Attribute(name='y', default=NOTHING, validator=None, repr=True, eq=True, eq_key=None, order=True, order_key=None, hash=None, init=True, metadata=mappingproxy({}), type=None, converter=None, kw_only=False, inherited=False, on_setattr=None, alias='y'))
       >>> attrs.fields(C)[1]
       Attribute(name='y', default=NOTHING, validator=None, repr=True, eq=True, eq_key=None, order=True, order_key=None, hash=None, init=True, metadata=mappingproxy({}), type=None, converter=None, kw_only=False, inherited=False, on_setattr=None, alias='y')
       >>> attrs.fields(C).y is attrs.fields(C)[1]
       True
 
-.. function:: attr.fields
-
-   Same as `attrs.fields`.
-
 .. autofunction:: attrs.fields_dict
 
    For example:
 
    .. doctest::
 
       >>> @attr.s
@@ -269,125 +170,104 @@
       >>> attrs.fields_dict(C)
       {'x': Attribute(name='x', default=NOTHING, validator=None, repr=True, eq=True, eq_key=None, order=True, order_key=None, hash=None, init=True, metadata=mappingproxy({}), type=None, converter=None, kw_only=False, inherited=False, on_setattr=None, alias='x'), 'y': Attribute(name='y', default=NOTHING, validator=None, repr=True, eq=True, eq_key=None, order=True, order_key=None, hash=None, init=True, metadata=mappingproxy({}), type=None, converter=None, kw_only=False, inherited=False, on_setattr=None, alias='y')}
       >>> attr.fields_dict(C)['y']
       Attribute(name='y', default=NOTHING, validator=None, repr=True, eq=True, eq_key=None, order=True, order_key=None, hash=None, init=True, metadata=mappingproxy({}), type=None, converter=None, kw_only=False, inherited=False, on_setattr=None, alias='y')
       >>> attrs.fields_dict(C)['y'] is attrs.fields(C).y
       True
 
-.. function:: attr.fields_dict
-
-   Same as `attrs.fields_dict`.
-
 .. autofunction:: attrs.has
 
    For example:
 
    .. doctest::
 
       >>> @attr.s
       ... class C:
       ...     pass
       >>> attr.has(C)
       True
       >>> attr.has(object)
       False
 
-.. function:: attr.has
-
-   Same as `attrs.has`.
-
 .. autofunction:: attrs.resolve_types
 
     For example:
 
     .. doctest::
 
         >>> import typing
-        >>> @attrs.define
+        >>> @define
         ... class A:
         ...     a: typing.List['A']
         ...     b: 'B'
         ...
-        >>> @attrs.define
+        >>> @define
         ... class B:
         ...     a: A
         ...
         >>> attrs.fields(A).a.type
         typing.List[ForwardRef('A')]
         >>> attrs.fields(A).b.type
         'B'
         >>> attrs.resolve_types(A, globals(), locals())
         <class 'A'>
         >>> attrs.fields(A).a.type
         typing.List[A]
         >>> attrs.fields(A).b.type
         <class 'B'>
 
-.. function:: attr.resolve_types
-
-   Same as `attrs.resolve_types`.
-
 .. autofunction:: attrs.asdict
 
    For example:
 
    .. doctest::
 
-      >>> @attrs.define
+      >>> @define
       ... class C:
       ...     x: int
       ...     y: int
       >>> attrs.asdict(C(1, C(2, 3)))
       {'x': 1, 'y': {'x': 2, 'y': 3}}
 
-.. autofunction:: attr.asdict
-
 .. autofunction:: attrs.astuple
 
    For example:
 
    .. doctest::
 
-      >>> @attrs.define
+      >>> @define
       ... class C:
-      ...     x = attr.field()
-      ...     y = attr.field()
+      ...     x = field()
+      ...     y = field()
       >>> attrs.astuple(C(1,2))
       (1, 2)
 
-.. autofunction:: attr.astuple
-
-
-*attrs* includes some handy helpers for filtering the attributes in `attrs.asdict` and `attrs.astuple`:
+.. module:: attrs.filters
 
-.. autofunction:: attrs.filters.include
+*attrs* includes helpers for filtering the attributes in `attrs.asdict` and `attrs.astuple`:
 
-.. autofunction:: attrs.filters.exclude
+.. autofunction:: include
 
-.. function:: attr.filters.include
-
-   Same as `attrs.filters.include`.
-
-.. function:: attr.filters.exclude
-
-   Same as `attrs.filters.exclude`.
+.. autofunction:: exclude
 
 See :func:`attrs.asdict` for examples.
 
-All objects from ``attrs.filters`` are also available from ``attr.filters``.
+All objects from ``attrs.filters`` are also available from ``attr.filters`` (it's the same module in a different namespace).
 
 ----
 
+.. currentmodule:: attrs
+
 .. autofunction:: attrs.evolve
 
    For example:
 
    .. doctest::
 
-      >>> @attrs.define
+      >>> @define
       ... class C:
       ...     x: int
       ...     y: int
       >>> i1 = C(1, 2)
       >>> i1
       C(x=1, y=2)
       >>> i2 = attrs.evolve(i1, y=3)
@@ -399,94 +279,80 @@
    ``evolve`` creates a new instance using ``__init__``.
    This fact has several implications:
 
    * private attributes should be specified without the leading underscore, just like in ``__init__``.
    * attributes with ``init=False`` can't be set with ``evolve``.
    * the usual ``__init__`` validators will validate the new values.
 
-.. function:: attr.evolve
-
-   Same as `attrs.evolve`.
-
 .. autofunction:: attrs.validate
 
    For example:
 
    .. doctest::
 
-      >>> @attrs.define(on_setattr=attrs.setters.NO_OP)
+      >>> @define(on_setattr=attrs.setters.NO_OP)
       ... class C:
-      ...     x = attrs.field(validator=attrs.validators.instance_of(int))
+      ...     x = field(validator=attrs.validators.instance_of(int))
       >>> i = C(1)
       >>> i.x = "1"
       >>> attrs.validate(i)
       Traceback (most recent call last):
          ...
       TypeError: ("'x' must be <class 'int'> (got '1' that is a <class 'str'>).", ...)
 
-.. function:: attr.validate
-
-   Same as `attrs.validate`.
-
-
-Validators can be globally disabled if you want to run them only in development and tests but not in production because you fear their performance impact:
-
-.. autofunction:: set_run_validators
-
-.. autofunction:: get_run_validators
-
 
 .. _api-validators:
 
 Validators
 ----------
 
-*attrs* comes with some common validators in the ``attrs.validators`` module.
-All objects from ``attrs.validators`` are also available from ``attr.validators``.
+.. module:: attrs.validators
 
+*attrs* comes with some common validators in the ``attrs.validators`` module.
+All objects from ``attrs.validators`` are also available from ``attr.validators`` (it's the same module in a different namespace).
 
 .. autofunction:: attrs.validators.lt
 
    For example:
 
    .. doctest::
 
-      >>> @attrs.define
+      >>> @define
       ... class C:
-      ...     x = attrs.field(validator=attrs.validators.lt(42))
+      ...     x = field(validator=attrs.validators.lt(42))
       >>> C(41)
       C(x=41)
       >>> C(42)
       Traceback (most recent call last):
          ...
       ValueError: ("'x' must be < 42: 42")
 
 .. autofunction:: attrs.validators.le
 
    For example:
 
    .. doctest::
 
-      >>> @attrs.define
+      >>> @define
       ... class C:
-      ...     x = attrs.field(validator=attr.validators.le(42))
+      ...     x = field(validator=attrs.validators.le(42))
       >>> C(42)
       C(x=42)
       >>> C(43)
       Traceback (most recent call last):
          ...
       ValueError: ("'x' must be <= 42: 43")
 
 .. autofunction:: attrs.validators.ge
 
    For example:
 
    .. doctest::
 
-      >>> @attrs.define
+      >>> @define
       ... class C:
       ...     x = attrs.field(validator=attrs.validators.ge(42))
       >>> C(42)
       C(x=42)
       >>> C(41)
       Traceback (most recent call last):
          ...
@@ -494,65 +360,65 @@
 
 .. autofunction:: attrs.validators.gt
 
    For example:
 
    .. doctest::
 
-      >>> @attrs.define
+      >>> @define
       ... class C:
-      ...     x = attr.field(validator=attrs.validators.gt(42))
+      ...     x = field(validator=attrs.validators.gt(42))
       >>> C(43)
       C(x=43)
       >>> C(42)
       Traceback (most recent call last):
          ...
       ValueError: ("'x' must be > 42: 42")
 
 .. autofunction:: attrs.validators.max_len
 
    For example:
 
    .. doctest::
 
-      >>> @attrs.define
+      >>> @define
       ... class C:
-      ...     x = attrs.field(validator=attrs.validators.max_len(4))
+      ...     x = field(validator=attrs.validators.max_len(4))
       >>> C("spam")
       C(x='spam')
       >>> C("bacon")
       Traceback (most recent call last):
          ...
       ValueError: ("Length of 'x' must be <= 4: 5")
 
 .. autofunction:: attrs.validators.min_len
 
    For example:
 
    .. doctest::
 
-      >>> @attrs.define
+      >>> @define
       ... class C:
-      ...     x = attrs.field(validator=attrs.validators.min_len(1))
+      ...     x = field(validator=attrs.validators.min_len(1))
       >>> C("bacon")
       C(x='bacon')
       >>> C("")
       Traceback (most recent call last):
          ...
       ValueError: ("Length of 'x' must be => 1: 0")
 
 .. autofunction:: attrs.validators.instance_of
 
    For example:
 
    .. doctest::
 
-      >>> @attrs.define
+      >>> @define
       ... class C:
-      ...     x = attrs.field(validator=attrs.validators.instance_of(int))
+      ...     x = field(validator=attrs.validators.instance_of(int))
       >>> C(42)
       C(x=42)
       >>> C("42")
       Traceback (most recent call last):
          ...
       TypeError: ("'x' must be <type 'int'> (got '42' that is a <type 'str'>).", Attribute(name='x', default=NOTHING, validator=<instance_of validator for type <type 'int'>>, type=None, kw_only=False), <type 'int'>, '42')
       >>> C(None)
@@ -566,18 +432,18 @@
 
    .. doctest::
 
       >>> import enum
       >>> class State(enum.Enum):
       ...     ON = "on"
       ...     OFF = "off"
-      >>> @attrs.define
+      >>> @define
       ... class C:
-      ...     state = attrs.field(validator=attrs.validators.in_(State))
-      ...     val = attrs.field(validator=attrs.validators.in_([1, 2, 3]))
+      ...     state = field(validator=attrs.validators.in_(State))
+      ...     val = field(validator=attrs.validators.in_([1, 2, 3]))
       >>> C(State.ON, 1)
       C(state=<State.ON: 'on'>, val=1)
       >>> C("on", 1)
       Traceback (most recent call last):
          ...
       ValueError: 'state' must be in <enum 'State'> (got 'on'), Attribute(name='state', default=NOTHING, validator=<in_ validator with options <enum 'State'>>, repr=True, eq=True, eq_key=None, order=True, order_key=None, hash=None, init=True, metadata=mappingproxy({}), type=None, converter=None, kw_only=False, inherited=False, on_setattr=None), <enum 'State'>, 'on')
       >>> C(State.ON, 4)
@@ -589,27 +455,27 @@
 
 .. autofunction:: attrs.validators.and_
 
    For convenience, it's also possible to pass a list to `attrs.field`'s validator argument.
 
    Thus the following two statements are equivalent::
 
-      x = attrs.field(validator=attrs.validators.and_(v1, v2, v3))
-      x = attrs.field(validator=[v1, v2, v3])
+      x = field(validator=attrs.validators.and_(v1, v2, v3))
+      x = field(validator=[v1, v2, v3])
 
 .. autofunction:: attrs.validators.not_
 
    For example:
 
    .. doctest::
 
       >>> reserved_names = {"id", "time", "source"}
-      >>> @attrs.define
+      >>> @define
       ... class Measurement:
-      ...     tags = attrs.field(
+      ...     tags = field(
       ...         validator=attrs.validators.deep_mapping(
       ...             key_validator=attrs.validators.not_(
       ...                 attrs.validators.in_(reserved_names),
       ...                 msg="reserved tag key",
       ...             ),
       ...             value_validator=attrs.validators.instance_of((str, int)),
       ...         )
@@ -624,17 +490,20 @@
 
 .. autofunction:: attrs.validators.optional
 
    For example:
 
    .. doctest::
 
-      >>> @attrs.define
+      >>> @define
       ... class C:
-      ...     x = attrs.field(validator=attrs.validators.optional(attr.validators.instance_of(int)))
+      ...     x = field(
+      ...         validator=attrs.validators.optional(
+      ...             attrs.validators.instance_of(int)
+      ...         ))
       >>> C(42)
       C(x=42)
       >>> C("42")
       Traceback (most recent call last):
          ...
       TypeError: ("'x' must be <type 'int'> (got '42' that is a <type 'str'>).", Attribute(name='x', default=NOTHING, validator=<instance_of validator for type <type 'int'>>, type=None, kw_only=False), <type 'int'>, '42')
       >>> C(None)
@@ -643,34 +512,34 @@
 
 .. autofunction:: attrs.validators.is_callable
 
     For example:
 
     .. doctest::
 
-        >>> @attrs.define
+        >>> @define
         ... class C:
-        ...     x = attrs.field(validator=attrs.validators.is_callable())
+        ...     x = field(validator=attrs.validators.is_callable())
         >>> C(isinstance)
         C(x=<built-in function isinstance>)
         >>> C("not a callable")
         Traceback (most recent call last):
             ...
         attr.exceptions.NotCallableError: 'x' must be callable (got 'not a callable' that is a <class 'str'>).
 
 
 .. autofunction:: attrs.validators.matches_re
 
     For example:
 
     .. doctest::
 
-        >>> @attrs.define
+        >>> @define
         ... class User:
-        ...     email = attrs.field(validator=attrs.validators.matches_re(
+        ...     email = field(validator=attrs.validators.matches_re(
         ...         "(^[a-zA-Z0-9_.+-]+@[a-zA-Z0-9-]+\.[a-zA-Z0-9-.]+$)"))
         >>> User(email="user@example.com")
         User(email='user@example.com')
         >>> User(email="user@example.com@test.com")
         Traceback (most recent call last):
             ...
         ValueError: ("'email' must match regex '(^[a-zA-Z0-9_.+-]+@[a-zA-Z0-9-]+\\\\.[a-zA-Z0-9-.]+$)' ('user@example.com@test.com' doesn't)", Attribute(name='email', default=NOTHING, validator=<matches_re validator for pattern re.compile('(^[a-zA-Z0-9_.+-]+@[a-zA-Z0-9-]+\\.[a-zA-Z0-9-.]+$)')>, repr=True, cmp=True, hash=None, init=True, metadata=mappingproxy({}), type=None, converter=None, kw_only=False), re.compile('(^[a-zA-Z0-9_.+-]+@[a-zA-Z0-9-]+\\.[a-zA-Z0-9-.]+$)'), 'user@example.com@test.com')
@@ -678,19 +547,19 @@
 
 .. autofunction:: attrs.validators.deep_iterable
 
     For example:
 
     .. doctest::
 
-        >>> @attrs.define
+        >>> @define
         ... class C:
-        ...     x = attrs.field(validator=attrs.validators.deep_iterable(
-        ...     member_validator=attrs.validators.instance_of(int),
-        ...     iterable_validator=attrs.validators.instance_of(list)
+        ...     x = field(validator=attrs.validators.deep_iterable(
+        ...             member_validator=attrs.validators.instance_of(int),
+        ...             iterable_validator=attrs.validators.instance_of(list)
         ...     ))
         >>> C(x=[1, 2, 3])
         C(x=[1, 2, 3])
         >>> C(x=set([1, 2, 3]))
         Traceback (most recent call last):
             ...
         TypeError: ("'x' must be <class 'list'> (got {1, 2, 3} that is a <class 'set'>).", Attribute(name='x', default=NOTHING, validator=<deep_iterable validator for <instance_of validator for type <class 'list'>> iterables of <instance_of validator for type <class 'int'>>>, repr=True, cmp=True, hash=None, init=True, metadata=mappingproxy({}), type=None, converter=None, kw_only=False), <class 'list'>, {1, 2, 3})
@@ -702,20 +571,20 @@
 
 .. autofunction:: attrs.validators.deep_mapping
 
     For example:
 
     .. doctest::
 
-        >>> @attrs.define
+        >>> @define
         ... class C:
-        ...     x = attrs.field(validator=attrs.validators.deep_mapping(
-        ...         key_validator=attrs.validators.instance_of(str),
-        ...         value_validator=attrs.validators.instance_of(int),
-        ...         mapping_validator=attrs.validators.instance_of(dict)
+        ...     x = field(validator=attrs.validators.deep_mapping(
+        ...             key_validator=attrs.validators.instance_of(str),
+        ...             value_validator=attrs.validators.instance_of(int),
+        ...             mapping_validator=attrs.validators.instance_of(dict)
         ...     ))
         >>> C(x={"a": 1, "b": 2})
         C(x={'a': 1, 'b': 2})
         >>> C(x=None)
         Traceback (most recent call last):
             ...
         TypeError: ("'x' must be <class 'dict'> (got None that is a <class 'NoneType'>).", Attribute(name='x', default=NOTHING, validator=<deep_mapping validator for objects mapping <instance_of validator for type <class 'str'>> to <instance_of validator for type <class 'int'>>>, repr=True, cmp=True, hash=None, init=True, metadata=mappingproxy({}), type=None, converter=None, kw_only=False), <class 'dict'>, None)
@@ -736,65 +605,67 @@
 
 .. autofunction:: attrs.validators.disabled
 
 
 Converters
 ----------
 
-All objects from ``attrs.converters`` are also available from ``attr.converters``.
+.. module:: attrs.converters
+
+All objects from ``attrs.converters`` are also available from ``attr.converters`` (it's the same module in a different namespace).
 
 .. autofunction:: attrs.converters.pipe
 
-   For convenience, it's also possible to pass a list to `attr.ib`'s converter argument.
+   For convenience, it's also possible to pass a list to `attrs.field` / `attr.ib`'s converter arguments.
 
    Thus the following two statements are equivalent::
 
-      x = attr.ib(converter=attr.converter.pipe(c1, c2, c3))
-      x = attr.ib(converter=[c1, c2, c3])
+      x = attrs.field(converter=attrs.converter.pipe(c1, c2, c3))
+      x = attrs.field(converter=[c1, c2, c3])
 
 .. autofunction:: attrs.converters.optional
 
    For example:
 
    .. doctest::
 
-      >>> @attr.s
+      >>> @define
       ... class C:
-      ...     x = attr.ib(converter=attr.converters.optional(int))
+      ...     x = field(converter=attrs.converters.optional(int))
       >>> C(None)
       C(x=None)
       >>> C(42)
       C(x=42)
 
 
 .. autofunction:: attrs.converters.default_if_none
 
    For example:
 
    .. doctest::
 
-      >>> @attr.s
+      >>> @define
       ... class C:
-      ...     x = attr.ib(
-      ...         converter=attr.converters.default_if_none("")
+      ...     x = field(
+      ...         converter=attrs.converters.default_if_none("")
       ...     )
       >>> C(None)
       C(x='')
 
 
 .. autofunction:: attrs.converters.to_bool
 
    For example:
 
    .. doctest::
 
-      >>> @attr.s
+      >>> @define
       ... class C:
-      ...     x = attr.ib(
-      ...         converter=attr.converters.to_bool
+      ...     x = field(
+      ...         converter=attrs.converters.to_bool
       ...     )
       >>> C("yes")
       C(x=True)
       >>> C(0)
       C(x=False)
       >>> C("foo")
       Traceback (most recent call last):
@@ -804,71 +675,43 @@
 
 
 .. _api_setters:
 
 Setters
 -------
 
+.. module:: attrs.setters
+
 These are helpers that you can use together with `attrs.define`'s and `attrs.fields`'s ``on_setattr`` arguments.
-All setters in ``attrs.setters`` are also available from ``attr.setters``.
+All setters in ``attrs.setters`` are also available from ``attr.setters`` (it's the same module in a different namespace).
+
+.. autofunction:: frozen
+.. autofunction:: validate
+.. autofunction:: convert
+.. autofunction:: pipe
 
-.. autofunction:: attrs.setters.frozen
-.. autofunction:: attrs.setters.validate
-.. autofunction:: attrs.setters.convert
-.. autofunction:: attrs.setters.pipe
-.. data:: attrs.setters.NO_OP
+.. data:: NO_OP
 
    Sentinel for disabling class-wide *on_setattr* hooks for certain attributes.
 
    Does not work in `attrs.setters.pipe` or within lists.
 
    .. versionadded:: 20.1.0
 
    For example, only ``x`` is frozen here:
 
    .. doctest::
 
-     >>> @attrs.define(on_setattr=attr.setters.frozen)
+     >>> @define(on_setattr=attr.setters.frozen)
      ... class C:
-     ...     x = attr.field()
-     ...     y = attr.field(on_setattr=attr.setters.NO_OP)
+     ...     x = field()
+     ...     y = field(on_setattr=attr.setters.NO_OP)
      >>> c = C(1, 2)
      >>> c.y = 3
      >>> c.y
      3
      >>> c.x = 4
      Traceback (most recent call last):
          ...
      attrs.exceptions.FrozenAttributeError: ()
 
    N.B. Please use `attrs.define`'s *frozen* argument (or `attrs.frozen`) to freeze whole classes; it is more efficient.
-
-
-Deprecated APIs
----------------
-
-.. _version-info:
-
-To help you write backward compatible code that doesn't throw warnings on modern releases, the ``attr`` module has an ``__version_info__`` attribute as of version 19.2.0.
-It behaves similarly to `sys.version_info` and is an instance of `VersionInfo`:
-
-.. autoclass:: VersionInfo
-
-   With its help you can write code like this:
-
-   >>> if getattr(attr, "__version_info__", (0,)) >= (19, 2):
-   ...     cmp_off = {"eq": False}
-   ... else:
-   ...     cmp_off = {"cmp": False}
-   >>> cmp_off == {"eq":  False}
-   True
-   >>> @attr.s(**cmp_off)
-   ... class C:
-   ...     pass
-
-
-----
-
-The serious-business aliases used to be called ``attr.attributes`` and ``attr.attr``.
-There are no plans to remove them but they shouldn't be used in new code.
-
-.. autofunction:: assoc
```

### Comparing `attrs-22.2.0/docs/comparison.md` & `attrs-23.1.0/docs/comparison.md`

 * *Files identical despite different names*

### Comparing `attrs-22.2.0/docs/conf.py` & `attrs-23.1.0/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,17 +16,14 @@
 """
 
 linkcheck_ignore = [
     # We run into GitHub's rate limits.
     r"https://github.com/.*/(issues|pull)/\d+",
     # Rate limits and the latest tag is missing anyways on release.
     "https://github.com/python-attrs/attrs/tree/.*",
-    # It never finds the anchor even though it's there.
-    "https://github.com/microsoft/pyright/blob/main/specs/"
-    "dataclass_transforms.md#attrs",
 ]
 
 # In nitpick mode (-n), still ignore any of the following "broken" references
 # to non-types.
 nitpick_ignore = [
     ("py:class", "Any value"),
     ("py:class", "callable"),
```

### Comparing `attrs-22.2.0/docs/examples.md` & `attrs-23.1.0/docs/examples.md`

 * *Files 6% similar despite different names*

```diff
@@ -211,41 +211,68 @@
 
 >>> asdict(UserList([User("jane@doe.invalid", "s33kred"),
 ...                  User("joe@doe.invalid", "p4ssw0rd")]),
 ...        filter=lambda attr, value: attr.name != "password")
 {'users': [{'email': 'jane@doe.invalid'}, {'email': 'joe@doe.invalid'}]}
 ```
 
-For the common case where you want to [`include`](attrs.filters.include) or [`exclude`](attrs.filters.exclude) certain types or attributes, *attrs* ships with a few helpers:
+For the common case where you want to [`include`](attrs.filters.include) or [`exclude`](attrs.filters.exclude) certain types, string name or attributes, *attrs* ships with a few helpers:
 
 ```{doctest}
 >>> from attrs import asdict, filters, fields
 
 >>> @define
 ... class User:
 ...     login: str
 ...     password: str
+...     email: str
 ...     id: int
 
 >>> asdict(
-...     User("jane", "s33kred", 42),
-...     filter=filters.exclude(fields(User).password, int))
+...     User("jane", "s33kred", "jane@example.com", 42),
+...     filter=filters.exclude(fields(User).password, "email", int))
 {'login': 'jane'}
 
 >>> @define
 ... class C:
 ...     x: str
 ...     y: str
 ...     z: int
 
 >>> asdict(C("foo", "2", 3),
 ...        filter=filters.include(int, fields(C).x))
 {'x': 'foo', 'z': 3}
+
+>>> asdict(C("foo", "2", 3),
+...        filter=filters.include(fields(C).x, "z"))
+{'x': 'foo', 'z': 3}
 ```
 
+:::{note}
+Though using string names directly is convenient, mistyping attribute names will silently do the wrong thing and neither Python nor your type checker can help you.
+{func}`attrs.fields()` will raise an `AttributeError` when the field doesn't exist while literal string names won't.
+Using {func}`attrs.fields()` to get attributes is worth being recommended in most cases.
+
+```{doctest}
+>>> asdict(
+...     User("jane", "s33kred", "jane@example.com", 42),
+...     filter=filters.exclude("passwd")
+... )
+{'login': 'jane', 'password': 's33kred', 'email': 'jane@example.com', 'id': 42}
+
+>>> asdict(
+...     User("jane", "s33kred", "jane@example.com", 42),
+...     filter=fields(User).passwd
+... )
+Traceback (most recent call last):
+...
+AttributeError: 'UserAttributes' object has no attribute 'passwd'. Did you mean: 'password'?
+```
+:::
+
 Other times, all you want is a tuple and *attrs* won't let you down:
 
 ```{doctest}
 >>> import sqlite3
 >>> from attrs import astuple
 
 >>> @define
@@ -467,15 +494,15 @@
 Keys need to be hashable, and both keys and values are recommended to be immutable.
 
 If you're the author of a third-party library with *attrs* integration, please see [*Extending Metadata*](extending-metadata).
 
 
 ## Types
 
-*attrs* also allows you to associate a type with an attribute using either the *type* argument to {func}`attr.ib` or using {pep}`526`-annotations:
+*attrs* also allows you to associate a type with an attribute using either the *type* argument to {func}`attr.ib` and {func}`attr.field` or using {pep}`526`-annotations:
 
 ```{doctest}
 >>> @define
 ... class C:
 ...     x: int
 >>> fields(C).x.type
 <class 'int'>
@@ -622,19 +649,21 @@
 Sometimes you may want to create a class programmatically.
 *attrs* gives you {func}`attrs.make_class` for that:
 
 ```{doctest}
 >>> from attrs import make_class
 >>> @define
 ... class C1:
-...     x = field()
+...     x = field(type=int)
 ...     y = field()
->>> C2 = make_class("C2", ["x", "y"])
+>>> C2 = make_class("C2", {"x": field(type=int), "y": field()})
 >>> fields(C1) == fields(C2)
 True
+>>> fields(C1).x.type
+<class 'int'>
 ```
 
 You can still have power over the attributes if you pass a dictionary of name: {func}`~attrs.field` mappings and can pass arguments to `@attr.s`:
 
 ```{doctest}
 >>> C = make_class("C", {"x": field(default=42),
 ...                      "y": field(default=Factory(list))},
```

### Comparing `attrs-22.2.0/docs/extending.md` & `attrs-23.1.0/docs/extending.md`

 * *Files 3% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 Please note that it is currently *impossible* to let mypy know that you've changed defaults like *eq* or *order*.
 You can only use this trick to tell *Mypy* that a class is actually an *attrs* class.
 :::
 
 
 ### Pyright
 
-Generic decorator wrapping is supported in [*Pyright*](https://github.com/microsoft/pyright) via their [`dataclass_transform`] specification.
+Generic decorator wrapping is supported in [*Pyright*](https://github.com/microsoft/pyright) via `dataclass_transform` / {pep}`689`.
 
 For a custom wrapping of the form:
 
 ```
 def custom_define(f):
     return attr.define(f)
 ```
@@ -114,19 +114,14 @@
     field_descriptors: Tuple[Union[type, Callable[..., Any]], ...] = (()),
 ) -> Callable[[_T], _T]: ...
 
 @__dataclass_transform__(field_descriptors=(attr.attrib, attr.field))
 def custom_define(f): ...
 ```
 
-:::{warning}
-`dataclass_transform` is supported **provisionally** as of `pyright` 1.1.135.
-
-Both the *Pyright* [`dataclass_transform`] specification and *attrs* implementation may change in future versions.
-:::
 
 ## Types
 
 *attrs* offers two ways of attaching type information to attributes:
 
 - {pep}`526` annotations,
 - and the *type* argument to {func}`attr.ib`.
@@ -328,9 +323,7 @@
 ...     value_serializer=serialize,
 ... )
 >>> data
 {'dt': '2020-05-04T13:37:00'}
 >>> json.dumps(data)
 '{"dt": "2020-05-04T13:37:00"}'
 ```
-
-[`dataclass_transform`]: https://github.com/microsoft/pyright/blob/main/specs/dataclass_transforms.md
```

### Comparing `attrs-22.2.0/docs/glossary.md` & `attrs-23.1.0/docs/glossary.md`

 * *Files identical despite different names*

### Comparing `attrs-22.2.0/docs/hashing.md` & `attrs-23.1.0/docs/hashing.md`

 * *Files identical despite different names*

### Comparing `attrs-22.2.0/docs/how-does-it-work.md` & `attrs-23.1.0/docs/how-does-it-work.md`

 * *Files identical despite different names*

### Comparing `attrs-22.2.0/docs/index.md` & `attrs-23.1.0/docs/index.md`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 why
 examples
 types
 init
 comparison
 hashing
 api
+api-attr
 extending
 how-does-it-work
 names
 glossary
 ```
 
 ```{toctree}
```

### Comparing `attrs-22.2.0/docs/init.md` & `attrs-23.1.0/docs/init.md`

 * *Files 2% similar despite different names*

```diff
@@ -209,18 +209,20 @@
 C(x=3, y=4)
 >>> C(x=4, y=3)
 Traceback (most recent call last):
    ...
 ValueError: 'x' has to be smaller than 'y'!
 ```
 
-This example also shows of some syntactic sugar for using the {obj}`attrs.validators.and_` validator: if you pass a list, all validators have to pass.
+This example demonstrates a convenience shortcut:
+Passing a list of validators directly is equivalent to passing them wrapped in the {obj}`attrs.validators.and_` validator and all validators must pass.
 
 *attrs* won't intercept your changes to those attributes but you can always call {func}`attrs.validate` on any instance to verify that it's still valid:
-When using {func}`attrs.define` or [`attrs.frozen`](attrs.frozen), *attrs* will run the validators even when setting the attribute.
+
+When using {func}`attrs.define` or [`attrs.frozen`](attrs.frozen), however, *attrs* will run the validators even when setting the attribute.
 
 ```{doctest}
 >>> i = C(4, 5)
 >>> i.x = 5
 Traceback (most recent call last):
    ...
 ValueError: 'x' has to be smaller than 'y'!
@@ -237,15 +239,15 @@
 >>> C("42")
 Traceback (most recent call last):
    ...
 TypeError: ("'x' must be <type 'int'> (got '42' that is a <type 'str'>).", Attribute(name='x', default=NOTHING, factory=NOTHING, validator=<instance_of validator for type <type 'int'>>, type=None), <type 'int'>, '42')
 ```
 
 Of course you can mix and match the two approaches at your convenience.
-If you define validators both ways for an attribute, they are both ran:
+If you use both ways to define validators for an attribute, they are both ran:
 
 ```{doctest}
 >>> @define
 ... class C:
 ...     x = field(validator=attrs.validators.instance_of(int))
 ...     @x.validator
 ...     def fits_byte(self, attribute, value):
@@ -259,28 +261,28 @@
 TypeError: ("'x' must be <class 'int'> (got '128' that is a <class 'str'>).", Attribute(name='x', default=NOTHING, validator=[<instance_of validator for type <class 'int'>>, <function fits_byte at 0x10fd7a0d0>], repr=True, cmp=True, hash=True, init=True, metadata=mappingproxy({}), type=None, converter=one), <class 'int'>, '128')
 >>> C(256)
 Traceback (most recent call last):
    ...
 ValueError: value out of bounds
 ```
 
-And finally you can disable validators globally:
+Finally, validators can be globally disabled:
 
 ```{doctest}
 >>> attrs.validators.set_disabled(True)
 >>> C("128")
 C(x='128')
 >>> attrs.validators.set_disabled(False)
 >>> C("128")
 Traceback (most recent call last):
    ...
 TypeError: ("'x' must be <class 'int'> (got '128' that is a <class 'str'>).", Attribute(name='x', default=NOTHING, validator=[<instance_of validator for type <class 'int'>>, <function fits_byte at 0x10fd7a0d0>], repr=True, cmp=True, hash=True, init=True, metadata=mappingproxy({}), type=None, converter=None), <class 'int'>, '128')
 ```
 
-You can achieve the same by using the context manager:
+... or within a context manager:
 
 ```{doctest}
 >>> with attrs.validators.disabled():
 ...     C("128")
 C(x='128')
 >>> C("128")
 Traceback (most recent call last):
@@ -288,16 +290,15 @@
 TypeError: ("'x' must be <class 'int'> (got '128' that is a <class 'str'>).", Attribute(name='x', default=NOTHING, validator=[<instance_of validator for type <class 'int'>>, <function fits_byte at 0x10fd7a0d0>], repr=True, cmp=True, hash=True, init=True, metadata=mappingproxy({}), type=None, converter=None), <class 'int'>, '128')
 ```
 
 (converters)=
 
 ## Converters
 
-Finally, sometimes you may want to normalize the values coming in.
-For that *attrs* comes with converters.
+Sometimes, it is necessary to normalize the values coming in, therefore *attrs* comes with converters.
 
 Attributes can have a `converter` function specified, which will be called with the attribute's passed-in value to get a new value to use.
 This can be useful for doing type-conversions on values that you don't want to force your callers to do.
 
 ```{doctest}
 >>> @define
 ... class C:
@@ -346,18 +347,18 @@
 >>> C.__init__.__annotations__
 {'return': None, 'x': <class 'str'>}
 ```
 
 
 ## Hooking Yourself Into Initialization
 
-Generally speaking, the moment you think that you need finer control over how your class is instantiated than what *attrs* offers, it's usually best to use a {obj}`classmethod` factory or to apply the [builder pattern](https://en.wikipedia.org/wiki/Builder_pattern).
+Generally speaking, the moment you realize the need of finer control – than what *attrs* offers – over how a class is instantiated, it's usually best to use a {obj}`classmethod` factory or to apply the [builder pattern](https://en.wikipedia.org/wiki/Builder_pattern).
 
 However, sometimes you need to do that one quick thing before or after your class is initialized.
-And for that *attrs* offers three means:
+For that purpose, *attrs* offers the following options:
 
 - `__attrs_pre_init__` is automatically detected and run *before* *attrs* starts initializing.
   This is useful if you need to inject a call to `super().__init__()`.
 
 - `__attrs_post_init__` is automatically detected and run *after* *attrs* is done initializing your instance.
   This is useful if you want to derive some attribute from others or perform some kind of validation over the whole instance.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `attrs-22.2.0/docs/license.md` & `attrs-23.1.0/docs/license.md`

 * *Files identical despite different names*

### Comparing `attrs-22.2.0/docs/names.md` & `attrs-23.1.0/docs/names.md`

 * *Files identical despite different names*

### Comparing `attrs-22.2.0/docs/overview.md` & `attrs-23.1.0/docs/overview.md`

 * *Files identical despite different names*

### Comparing `attrs-22.2.0/docs/types.md` & `attrs-23.1.0/docs/types.md`

 * *Files 7% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     a_number = attr.ib(default=42)  # type: int
     list_of_numbers = attr.ib(factory=list, type=list[int])
 ```
 
 
 ## Pyright
 
-*attrs* provides support for [*Pyright*] though the [`dataclass_transform`] specification.
+*attrs* provides support for [*Pyright*] through the `dataclass_transform` / {pep}`681` specification.
 This provides static type inference for a subset of *attrs* equivalent to standard-library {mod}`dataclasses`,
 and requires explicit type annotations using the {func}`attrs.define` or `@attr.s(auto_attribs=True)` API.
 
 Given the following definition, *Pyright* will generate static type signatures for `SomeClass` attribute access, `__init__`, `__eq__`, and comparison methods:
 
 ```
 @attr.define
@@ -90,17 +90,14 @@
 The *Pyright* inferred types are a tiny subset of those supported by *Mypy*, including:
 
 - The generated `__init__` signature only includes the attribute type annotations.
   It currently does not include attribute `converter` types.
 
 - The `attrs.frozen` decorator is not typed with frozen attributes, which are properly typed via `attrs.define(frozen=True)`.
 
-  A [full list](https://github.com/microsoft/pyright/blob/main/specs/dataclass_transforms.md#attrs) of limitations and incompatibilities can be found in *Pyright*'s repository.
-
 Your constructive feedback is welcome in both [attrs#795](https://github.com/python-attrs/attrs/issues/795) and [pyright#1782](https://github.com/microsoft/pyright/discussions/1782).
 Generally speaking, the decision on improving *attrs* support in *Pyright* is entirely Microsoft's prerogative, though.
 :::
 
-[`dataclass_transform`]: https://github.com/microsoft/pyright/blob/main/specs/dataclass_transforms.md
 [*Mypy*]: http://mypy-lang.org
 [*Pyright*]: https://github.com/microsoft/pyright
 [*pytype*]: https://google.github.io/pytype/
```

### Comparing `attrs-22.2.0/docs/why.md` & `attrs-23.1.0/docs/why.md`

 * *Files 2% similar despite different names*

```diff
@@ -265,15 +265,15 @@
 ...
 ...     def __hash__(self):
 ...         return hash((self.__class__, self.a, self.b))
 >>> ArtisanalClass(a=1, b=2)
 ArtisanalClass(a=1, b=2)
 ```
 
-which is quite a mouthful and it doesn't even use any of *attrs*'s more advanced features like validators or defaults values.
+which is quite a mouthful and it doesn't even use any of *attrs*'s more advanced features like validators or default values.
 Also: no tests whatsoever.
 And who will guarantee you, that you don't accidentally flip the `<` in your tenth implementation of `__gt__`?
 
 It also should be noted that *attrs* is not an all-or-nothing solution.
 You can freely choose which features you want and disable those that you want more control over:
 
 ```{doctest}
@@ -289,9 +289,9 @@
 ```
 
 :::{admonition} Summary
 If you don't care and like typing, we're not gonna stop you.
 
 However it takes a lot of bias and determined rationalization to claim that *attrs* raises the mental burden on a project given how difficult it is to find the important bits in a hand-written class and how annoying it is to ensure you've copy-pasted your code correctly over all your classes.
 
-In any case, if you ever get sick of the repetitiveness and drowning important code in a sea of boilerplate, *attrs* will be waiting for you.
+In any case, if you ever get sick of the repetitiveness and the drowning of important code in a sea of boilerplate, *attrs* will be waiting for you.
 :::
```

### Comparing `attrs-22.2.0/setup.py` & `attrs-23.1.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,316 +1,309 @@
 00000000: 2320 5350 4458 2d4c 6963 656e 7365 2d49  # SPDX-License-I
 00000010: 6465 6e74 6966 6965 723a 204d 4954 0a0a  dentifier: MIT..
-00000020: 696d 706f 7274 2063 6f64 6563 730a 696d  import codecs.im
-00000030: 706f 7274 206f 730a 696d 706f 7274 2072  port os.import r
-00000040: 650a 0a66 726f 6d20 7365 7475 7074 6f6f  e..from setuptoo
-00000050: 6c73 2069 6d70 6f72 7420 6669 6e64 5f70  ls import find_p
-00000060: 6163 6b61 6765 732c 2073 6574 7570 0a0a  ackages, setup..
-00000070: 0a23 2323 2323 2323 2323 2323 2323 2323  .###############
-00000080: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000090: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000000a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000000b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000000c0: 0a0a 4e41 4d45 203d 2022 6174 7472 7322  ..NAME = "attrs"
-000000d0: 0a50 4143 4b41 4745 5320 3d20 6669 6e64  .PACKAGES = find
-000000e0: 5f70 6163 6b61 6765 7328 7768 6572 653d  _packages(where=
-000000f0: 2273 7263 2229 0a4d 4554 415f 5041 5448  "src").META_PATH
-00000100: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
-00000110: 2273 7263 222c 2022 6174 7472 222c 2022  "src", "attr", "
-00000120: 5f5f 696e 6974 5f5f 2e70 7922 290a 4b45  __init__.py").KE
-00000130: 5957 4f52 4453 203d 205b 2263 6c61 7373  YWORDS = ["class
-00000140: 222c 2022 6174 7472 6962 7574 6522 2c20  ", "attribute", 
-00000150: 2262 6f69 6c65 7270 6c61 7465 222c 2022  "boilerplate", "
-00000160: 6461 7461 636c 6173 7322 5d0a 5052 4f4a  dataclass"].PROJ
-00000170: 4543 545f 5552 4c53 203d 207b 0a20 2020  ECT_URLS = {.   
-00000180: 2022 446f 6375 6d65 6e74 6174 696f 6e22   "Documentation"
-00000190: 3a20 2268 7474 7073 3a2f 2f77 7777 2e61  : "https://www.a
-000001a0: 7474 7273 2e6f 7267 2f22 2c0a 2020 2020  ttrs.org/",.    
-000001b0: 2243 6861 6e67 656c 6f67 223a 2022 6874  "Changelog": "ht
-000001c0: 7470 733a 2f2f 7777 772e 6174 7472 732e  tps://www.attrs.
-000001d0: 6f72 672f 656e 2f73 7461 626c 652f 6368  org/en/stable/ch
-000001e0: 616e 6765 6c6f 672e 6874 6d6c 222c 0a20  angelog.html",. 
-000001f0: 2020 2022 4275 6720 5472 6163 6b65 7222     "Bug Tracker"
-00000200: 3a20 2268 7474 7073 3a2f 2f67 6974 6875  : "https://githu
-00000210: 622e 636f 6d2f 7079 7468 6f6e 2d61 7474  b.com/python-att
-00000220: 7273 2f61 7474 7273 2f69 7373 7565 7322  rs/attrs/issues"
-00000230: 2c0a 2020 2020 2253 6f75 7263 6520 436f  ,.    "Source Co
-00000240: 6465 223a 2022 6874 7470 733a 2f2f 6769  de": "https://gi
-00000250: 7468 7562 2e63 6f6d 2f70 7974 686f 6e2d  thub.com/python-
-00000260: 6174 7472 732f 6174 7472 7322 2c0a 2020  attrs/attrs",.  
-00000270: 2020 2246 756e 6469 6e67 223a 2022 6874    "Funding": "ht
-00000280: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000290: 2f73 706f 6e73 6f72 732f 6879 6e65 6b22  /sponsors/hynek"
-000002a0: 2c0a 2020 2020 2254 6964 656c 6966 7422  ,.    "Tidelift"
-000002b0: 3a20 2268 7474 7073 3a2f 2f74 6964 656c  : "https://tidel
-000002c0: 6966 742e 636f 6d2f 7375 6273 6372 6970  ift.com/subscrip
-000002d0: 7469 6f6e 2f70 6b67 2f70 7970 692d 6174  tion/pkg/pypi-at
-000002e0: 7472 733f 220a 2020 2020 2275 746d 5f73  trs?".    "utm_s
-000002f0: 6f75 7263 653d 7079 7069 2d61 7474 7273  ource=pypi-attrs
-00000300: 2675 746d 5f6d 6564 6975 6d3d 7079 7069  &utm_medium=pypi
-00000310: 222c 0a20 2020 2022 4b6f 2d66 6922 3a20  ",.    "Ko-fi": 
-00000320: 2268 7474 7073 3a2f 2f6b 6f2d 6669 2e63  "https://ko-fi.c
-00000330: 6f6d 2f74 6865 5f68 796e 656b 222c 0a7d  om/the_hynek",.}
-00000340: 0a43 4c41 5353 4946 4945 5253 203d 205b  .CLASSIFIERS = [
-00000350: 0a20 2020 2022 4465 7665 6c6f 706d 656e  .    "Developmen
-00000360: 7420 5374 6174 7573 203a 3a20 3520 2d20  t Status :: 5 - 
-00000370: 5072 6f64 7563 7469 6f6e 2f53 7461 626c  Production/Stabl
-00000380: 6522 2c0a 2020 2020 2249 6e74 656e 6465  e",.    "Intende
-00000390: 6420 4175 6469 656e 6365 203a 3a20 4465  d Audience :: De
-000003a0: 7665 6c6f 7065 7273 222c 0a20 2020 2022  velopers",.    "
-000003b0: 4e61 7475 7261 6c20 4c61 6e67 7561 6765  Natural Language
-000003c0: 203a 3a20 456e 676c 6973 6822 2c0a 2020   :: English",.  
-000003d0: 2020 224c 6963 656e 7365 203a 3a20 4f53    "License :: OS
-000003e0: 4920 4170 7072 6f76 6564 203a 3a20 4d49  I Approved :: MI
-000003f0: 5420 4c69 6365 6e73 6522 2c0a 2020 2020  T License",.    
-00000400: 224f 7065 7261 7469 6e67 2053 7973 7465  "Operating Syste
-00000410: 6d20 3a3a 204f 5320 496e 6465 7065 6e64  m :: OS Independ
-00000420: 656e 7422 2c0a 2020 2020 2250 726f 6772  ent",.    "Progr
-00000430: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000440: 3a3a 2050 7974 686f 6e22 2c0a 2020 2020  :: Python",.    
-00000450: 2250 726f 6772 616d 6d69 6e67 204c 616e  "Programming Lan
-00000460: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-00000470: 3a3a 2033 222c 0a20 2020 2022 5072 6f67  :: 3",.    "Prog
-00000480: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000490: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-000004a0: 3622 2c0a 2020 2020 2250 726f 6772 616d  6",.    "Program
-000004b0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-000004c0: 2050 7974 686f 6e20 3a3a 2033 2e37 222c   Python :: 3.7",
-000004d0: 0a20 2020 2022 5072 6f67 7261 6d6d 696e  .    "Programmin
-000004e0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-000004f0: 7468 6f6e 203a 3a20 332e 3822 2c0a 2020  thon :: 3.8",.  
-00000500: 2020 2250 726f 6772 616d 6d69 6e67 204c    "Programming L
-00000510: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000520: 6e20 3a3a 2033 2e39 222c 0a20 2020 2022  n :: 3.9",.    "
-00000530: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00000540: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000550: 3a20 332e 3130 222c 0a20 2020 2022 5072  : 3.10",.    "Pr
-00000560: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000570: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000580: 332e 3131 222c 0a20 2020 2022 5072 6f67  3.11",.    "Prog
-00000590: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-000005a0: 203a 3a20 5079 7468 6f6e 203a 3a20 496d   :: Python :: Im
-000005b0: 706c 656d 656e 7461 7469 6f6e 203a 3a20  plementation :: 
-000005c0: 4350 7974 686f 6e22 2c0a 2020 2020 2250  CPython",.    "P
-000005d0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-000005e0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-000005f0: 2049 6d70 6c65 6d65 6e74 6174 696f 6e20   Implementation 
-00000600: 3a3a 2050 7950 7922 2c0a 2020 2020 2254  :: PyPy",.    "T
-00000610: 6f70 6963 203a 3a20 536f 6674 7761 7265  opic :: Software
-00000620: 2044 6576 656c 6f70 6d65 6e74 203a 3a20   Development :: 
-00000630: 4c69 6272 6172 6965 7320 3a3a 2050 7974  Libraries :: Pyt
-00000640: 686f 6e20 4d6f 6475 6c65 7322 2c0a 5d0a  hon Modules",.].
-00000650: 494e 5354 414c 4c5f 5245 5155 4952 4553  INSTALL_REQUIRES
-00000660: 203d 205b 5d0a 4558 5452 4153 5f52 4551   = [].EXTRAS_REQ
-00000670: 5549 5245 203d 207b 0a20 2020 2022 646f  UIRE = {.    "do
-00000680: 6373 223a 205b 0a20 2020 2020 2020 2022  cs": [.        "
-00000690: 6675 726f 222c 0a20 2020 2020 2020 2022  furo",.        "
-000006a0: 7370 6869 6e78 222c 0a20 2020 2020 2020  sphinx",.       
-000006b0: 2022 6d79 7374 2d70 6172 7365 7222 2c0a   "myst-parser",.
-000006c0: 2020 2020 2020 2020 227a 6f70 652e 696e          "zope.in
-000006d0: 7465 7266 6163 6522 2c0a 2020 2020 2020  terface",.      
-000006e0: 2020 2273 7068 696e 782d 6e6f 7466 6f75    "sphinx-notfou
-000006f0: 6e64 2d70 6167 6522 2c0a 2020 2020 2020  nd-page",.      
-00000700: 2020 2273 7068 696e 7863 6f6e 7472 6962    "sphinxcontrib
-00000710: 2d74 6f77 6e63 7269 6572 222c 0a20 2020  -towncrier",.   
-00000720: 2020 2020 2022 746f 776e 6372 6965 7222       "towncrier"
-00000730: 2c0a 2020 2020 5d2c 0a20 2020 2022 7465  ,.    ],.    "te
-00000740: 7374 732d 6e6f 2d7a 6f70 6522 3a20 5b0a  sts-no-zope": [.
-00000750: 2020 2020 2020 2020 2320 466f 7220 7265          # For re
-00000760: 6772 6573 7369 6f6e 2074 6573 7420 746f  gression test to
-00000770: 2065 6e73 7572 6520 636c 6f75 6470 6963   ensure cloudpic
-00000780: 6b6c 6520 636f 6d70 6174 2064 6f65 736e  kle compat doesn
-00000790: 2774 2062 7265 616b 2e0a 2020 2020 2020  't break..      
-000007a0: 2020 2763 6c6f 7564 7069 636b 6c65 3b20    'cloudpickle; 
-000007b0: 7079 7468 6f6e 5f69 6d70 6c65 6d65 6e74  python_implement
-000007c0: 6174 696f 6e20 3d3d 2022 4350 7974 686f  ation == "CPytho
-000007d0: 6e22 272c 0a20 2020 2020 2020 2022 6879  n"',.        "hy
-000007e0: 706f 7468 6573 6973 222c 0a20 2020 2020  pothesis",.     
-000007f0: 2020 2022 7079 6d70 6c65 7222 2c0a 2020     "pympler",.  
-00000800: 2020 2020 2020 2320 342e 332e 3020 6472        # 4.3.0 dr
-00000810: 6f70 7065 6420 6c61 7374 2075 7365 206f  opped last use o
-00000820: 6620 6063 6f6e 7665 7274 600a 2020 2020  f `convert`.    
-00000830: 2020 2020 2270 7974 6573 743e 3d34 2e33      "pytest>=4.3
-00000840: 2e30 222c 0a20 2020 2020 2020 2023 2070  .0",.        # p
-00000850: 7375 7469 6c20 6578 7472 6120 6973 206e  sutil extra is n
-00000860: 6565 6465 6420 666f 7220 636f 7272 6563  eeded for correc
-00000870: 7420 636f 7265 2063 6f75 6e74 2064 6574  t core count det
-00000880: 6563 7469 6f6e 2e0a 2020 2020 2020 2020  ection..        
-00000890: 2270 7974 6573 742d 7864 6973 745b 7073  "pytest-xdist[ps
-000008a0: 7574 696c 5d22 2c0a 2020 2020 2020 2020  util]",.        
-000008b0: 2320 5369 6e63 6520 7468 6520 6d79 7079  # Since the mypy
-000008c0: 2065 7272 6f72 206d 6573 7361 6765 7320   error messages 
-000008d0: 6b65 6570 2063 6861 6e67 696e 672c 2077  keep changing, w
-000008e0: 6520 6861 7665 2074 6f20 6b65 6570 2075  e have to keep u
-000008f0: 7064 6174 696e 670a 2020 2020 2020 2020  pdating.        
-00000900: 2320 7468 6973 2070 696e 2e0a 2020 2020  # this pin..    
-00000910: 2020 2020 226d 7970 793e 3d30 2e39 3731      "mypy>=0.971
-00000920: 2c3c 302e 3939 303b 2070 7974 686f 6e5f  ,<0.990; python_
-00000930: 696d 706c 656d 656e 7461 7469 6f6e 203d  implementation =
-00000940: 3d20 2743 5079 7468 6f6e 2722 2c0a 2020  = 'CPython'",.  
-00000950: 2020 2020 2020 2270 7974 6573 742d 6d79        "pytest-my
-00000960: 7079 2d70 6c75 6769 6e73 3b20 7079 7468  py-plugins; pyth
-00000970: 6f6e 5f69 6d70 6c65 6d65 6e74 6174 696f  on_implementatio
-00000980: 6e20 3d3d 2027 4350 7974 686f 6e27 2061  n == 'CPython' a
-00000990: 6e64 2022 0a20 2020 2020 2020 2022 7079  nd ".        "py
-000009a0: 7468 6f6e 5f76 6572 7369 6f6e 3c27 332e  thon_version<'3.
-000009b0: 3131 2722 2c0a 2020 2020 5d2c 0a20 2020  11'",.    ],.   
-000009c0: 2022 7465 7374 7322 3a20 5b0a 2020 2020   "tests": [.    
-000009d0: 2020 2020 2261 7474 7273 5b74 6573 7473      "attrs[tests
-000009e0: 2d6e 6f2d 7a6f 7065 5d22 2c0a 2020 2020  -no-zope]",.    
-000009f0: 2020 2020 227a 6f70 652e 696e 7465 7266      "zope.interf
-00000a00: 6163 6522 2c0a 2020 2020 5d2c 0a20 2020  ace",.    ],.   
-00000a10: 2022 636f 7622 3a20 5b0a 2020 2020 2020   "cov": [.      
-00000a20: 2020 2261 7474 7273 5b74 6573 7473 5d22    "attrs[tests]"
-00000a30: 2c0a 2020 2020 2020 2020 2263 6f76 6572  ,.        "cover
-00000a40: 6167 652d 656e 6162 6c65 2d73 7562 7072  age-enable-subpr
-00000a50: 6f63 6573 7322 2c0a 2020 2020 2020 2020  ocess",.        
-00000a60: 2320 456e 7375 7265 2063 6f76 6572 6167  # Ensure coverag
-00000a70: 6520 6973 206e 6577 2065 6e6f 7567 6820  e is new enough 
-00000a80: 666f 7220 6073 6f75 7263 655f 706b 6773  for `source_pkgs
-00000a90: 602e 0a20 2020 2020 2020 2022 636f 7665  `..        "cove
-00000aa0: 7261 6765 5b74 6f6d 6c5d 3e3d 352e 3322  rage[toml]>=5.3"
-00000ab0: 2c0a 2020 2020 5d2c 0a20 2020 2022 6465  ,.    ],.    "de
-00000ac0: 7622 3a20 5b22 6174 7472 735b 7465 7374  v": ["attrs[test
-00000ad0: 732c 646f 6373 5d22 5d2c 0a7d 0a23 2044  s,docs]"],.}.# D
-00000ae0: 6f6e 2774 2062 7265 616b 2050 6175 6c20  on't break Paul 
-00000af0: 756e 6e65 6365 7373 6172 696c 7920 6a75  unnecessarily ju
-00000b00: 7374 2079 6574 2e20 432e 662e 2023 3638  st yet. C.f. #68
-00000b10: 350a 4558 5452 4153 5f52 4551 5549 5245  5.EXTRAS_REQUIRE
-00000b20: 5b22 7465 7374 735f 6e6f 5f7a 6f70 6522  ["tests_no_zope"
-00000b30: 5d20 3d20 4558 5452 4153 5f52 4551 5549  ] = EXTRAS_REQUI
-00000b40: 5245 5b22 7465 7374 732d 6e6f 2d7a 6f70  RE["tests-no-zop
-00000b50: 6522 5d0a 0a0a 2323 2323 2323 2323 2323  e"]...##########
-00000b60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000b70: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000b80: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000b90: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000ba0: 2323 2323 230a 0a48 4552 4520 3d20 6f73  #####..HERE = os
-00000bb0: 2e70 6174 682e 6162 7370 6174 6828 6f73  .path.abspath(os
-00000bc0: 2e70 6174 682e 6469 726e 616d 6528 5f5f  .path.dirname(__
-00000bd0: 6669 6c65 5f5f 2929 0a0a 0a64 6566 2072  file__))...def r
-00000be0: 6561 6428 2a70 6172 7473 293a 0a20 2020  ead(*parts):.   
-00000bf0: 2022 2222 0a20 2020 2042 7569 6c64 2061   """.    Build a
-00000c00: 6e20 6162 736f 6c75 7465 2070 6174 6820  n absolute path 
-00000c10: 6672 6f6d 202a 7061 7274 732a 2061 6e64  from *parts* and
-00000c20: 2072 6574 7572 6e20 7468 6520 636f 6e74   return the cont
-00000c30: 656e 7473 206f 6620 7468 650a 2020 2020  ents of the.    
-00000c40: 7265 7375 6c74 696e 6720 6669 6c65 2e20  resulting file. 
-00000c50: 2041 7373 756d 6520 5554 462d 3820 656e   Assume UTF-8 en
-00000c60: 636f 6469 6e67 2e0a 2020 2020 2222 220a  coding..    """.
-00000c70: 2020 2020 7769 7468 2063 6f64 6563 732e      with codecs.
-00000c80: 6f70 656e 286f 732e 7061 7468 2e6a 6f69  open(os.path.joi
-00000c90: 6e28 4845 5245 2c20 2a70 6172 7473 292c  n(HERE, *parts),
-00000ca0: 2022 7262 222c 2022 7574 662d 3822 2920   "rb", "utf-8") 
-00000cb0: 6173 2066 3a0a 2020 2020 2020 2020 7265  as f:.        re
-00000cc0: 7475 726e 2066 2e72 6561 6428 290a 0a0a  turn f.read()...
-00000cd0: 4d45 5441 5f46 494c 4520 3d20 7265 6164  META_FILE = read
-00000ce0: 284d 4554 415f 5041 5448 290a 0a0a 6465  (META_PATH)...de
-00000cf0: 6620 6669 6e64 5f6d 6574 6128 6d65 7461  f find_meta(meta
-00000d00: 293a 0a20 2020 2022 2222 0a20 2020 2045  ):.    """.    E
-00000d10: 7874 7261 6374 205f 5f2a 6d65 7461 2a5f  xtract __*meta*_
-00000d20: 5f20 6672 6f6d 204d 4554 415f 4649 4c45  _ from META_FILE
-00000d30: 2e0a 2020 2020 2222 220a 2020 2020 6d65  ..    """.    me
-00000d40: 7461 5f6d 6174 6368 203d 2072 652e 7365  ta_match = re.se
-00000d50: 6172 6368 280a 2020 2020 2020 2020 7266  arch(.        rf
-00000d60: 225e 5f5f 7b6d 6574 617d 5f5f 203d 205b  "^__{meta}__ = [
-00000d70: 275c 225d 285b 5e27 5c22 5d2a 295b 275c  '\"]([^'\"]*)['\
-00000d80: 225d 222c 204d 4554 415f 4649 4c45 2c20  "]", META_FILE, 
-00000d90: 7265 2e4d 0a20 2020 2029 0a20 2020 2069  re.M.    ).    i
-00000da0: 6620 6d65 7461 5f6d 6174 6368 3a0a 2020  f meta_match:.  
-00000db0: 2020 2020 2020 7265 7475 726e 206d 6574        return met
-00000dc0: 615f 6d61 7463 682e 6772 6f75 7028 3129  a_match.group(1)
-00000dd0: 0a20 2020 2072 6169 7365 2052 756e 7469  .    raise Runti
-00000de0: 6d65 4572 726f 7228 6622 556e 6162 6c65  meError(f"Unable
-00000df0: 2074 6f20 6669 6e64 205f 5f7b 6d65 7461   to find __{meta
-00000e00: 7d5f 5f20 7374 7269 6e67 2e22 290a 0a0a  }__ string.")...
-00000e10: 5645 5253 494f 4e20 3d20 6669 6e64 5f6d  VERSION = find_m
-00000e20: 6574 6128 2276 6572 7369 6f6e 2229 0a55  eta("version").U
-00000e30: 524c 203d 2066 696e 645f 6d65 7461 2822  RL = find_meta("
-00000e40: 7572 6c22 290a 0a23 2050 7950 4920 646f  url")..# PyPI do
-00000e50: 6573 6e27 7420 7375 7070 6f72 7420 7468  esn't support th
-00000e60: 6520 3c70 6963 7475 7265 3e20 7461 672e  e <picture> tag.
-00000e70: 0a4c 4f47 4f20 3d20 2222 223c 7020 616c  .LOGO = """<p al
-00000e80: 6967 6e3d 2263 656e 7465 7222 3e0a 2020  ign="center">.  
-00000e90: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00000ea0: 2f77 7777 2e61 7474 7273 2e6f 7267 2f22  /www.attrs.org/"
-00000eb0: 3e0a 2020 2020 3c69 6d67 2073 7263 3d22  >.    <img src="
-00000ec0: 6874 7470 733a 2f2f 7261 772e 6769 7468  https://raw.gith
-00000ed0: 7562 7573 6572 636f 6e74 656e 742e 636f  ubusercontent.co
-00000ee0: 6d2f 7079 7468 6f6e 2d61 7474 7273 2f61  m/python-attrs/a
-00000ef0: 7474 7273 2f6d 6169 6e2f 646f 6373 2f5f  ttrs/main/docs/_
-00000f00: 7374 6174 6963 2f61 7474 7273 5f6c 6f67  static/attrs_log
-00000f10: 6f2e 7376 6722 2077 6964 7468 3d22 3335  o.svg" width="35
-00000f20: 2522 2061 6c74 3d22 6174 7472 7322 202f  %" alt="attrs" /
-00000f30: 3e0a 2020 3c2f 613e 0a3c 2f70 3e0a 2222  >.  </a>.</p>.""
-00000f40: 2220 2023 206e 6f71 610a 0a4c 4f4e 4720  "  # noqa..LONG 
-00000f50: 3d20 280a 2020 2020 4c4f 474f 0a20 2020  = (.    LOGO.   
-00000f60: 202b 2072 6561 6428 2252 4541 444d 452e   + read("README.
-00000f70: 6d64 2229 2e73 706c 6974 2822 3c21 2d2d  md").split("<!--
-00000f80: 206c 6f67 6f2d 656e 6420 2d2d 3e22 2c20   logo-end -->", 
-00000f90: 3129 5b31 5d0a 2020 2020 2b20 225c 6e5c  1)[1].    + "\n\
-00000fa0: 6e23 2320 4368 616e 6765 7320 696e 2054  n## Changes in T
-00000fb0: 6869 7320 5265 6c65 6173 655c 6e22 0a20  his Release\n". 
-00000fc0: 2020 202b 2072 6561 6428 2243 4841 4e47     + read("CHANG
-00000fd0: 454c 4f47 2e6d 6422 290a 2020 2020 2e73  ELOG.md").    .s
-00000fe0: 706c 6974 2822 746f 776e 6372 6965 7220  plit("towncrier 
-00000ff0: 7265 6c65 6173 6520 6e6f 7465 7320 7374  release notes st
-00001000: 6172 7420 2d2d 3e22 2c20 3129 5b31 5d0a  art -->", 1)[1].
-00001010: 2020 2020 2e73 7472 6970 2829 0a20 2020      .strip().   
-00001020: 202e 7370 6c69 7428 225c 6e23 2320 222c   .split("\n## ",
-00001030: 2031 295b 305d 0a20 2020 202e 7374 7269   1)[0].    .stri
-00001040: 7028 290a 2020 2020 2e73 706c 6974 2822  p().    .split("
-00001050: 5c6e 222c 2031 295b 315d 0a20 2020 202b  \n", 1)[1].    +
-00001060: 2022 5c6e 5c6e 2d2d 2d5c 6e5c 6e5b 4675   "\n\n---\n\n[Fu
-00001070: 6c6c 2063 6861 6e67 656c 6f67 5d22 0a20  ll changelog]". 
-00001080: 2020 2022 2868 7474 7073 3a2f 2f77 7777     "(https://www
-00001090: 2e61 7474 7273 2e6f 7267 2f65 6e2f 7374  .attrs.org/en/st
-000010a0: 6162 6c65 2f63 6861 6e67 656c 6f67 2e68  able/changelog.h
-000010b0: 746d 6c29 5c6e 220a 290a 0a69 6620 5f5f  tml)\n".)..if __
-000010c0: 6e61 6d65 5f5f 203d 3d20 225f 5f6d 6169  name__ == "__mai
-000010d0: 6e5f 5f22 3a0a 2020 2020 7365 7475 7028  n__":.    setup(
-000010e0: 0a20 2020 2020 2020 206e 616d 653d 4e41  .        name=NA
-000010f0: 4d45 2c0a 2020 2020 2020 2020 6465 7363  ME,.        desc
-00001100: 7269 7074 696f 6e3d 6669 6e64 5f6d 6574  ription=find_met
-00001110: 6128 2264 6573 6372 6970 7469 6f6e 2229  a("description")
-00001120: 2c0a 2020 2020 2020 2020 6c69 6365 6e73  ,.        licens
-00001130: 653d 6669 6e64 5f6d 6574 6128 226c 6963  e=find_meta("lic
-00001140: 656e 7365 2229 2c0a 2020 2020 2020 2020  ense"),.        
-00001150: 7572 6c3d 5552 4c2c 0a20 2020 2020 2020  url=URL,.       
-00001160: 2070 726f 6a65 6374 5f75 726c 733d 5052   project_urls=PR
-00001170: 4f4a 4543 545f 5552 4c53 2c0a 2020 2020  OJECT_URLS,.    
-00001180: 2020 2020 7665 7273 696f 6e3d 5645 5253      version=VERS
-00001190: 494f 4e2c 0a20 2020 2020 2020 2061 7574  ION,.        aut
-000011a0: 686f 723d 6669 6e64 5f6d 6574 6128 2261  hor=find_meta("a
-000011b0: 7574 686f 7222 292c 0a20 2020 2020 2020  uthor"),.       
-000011c0: 2061 7574 686f 725f 656d 6169 6c3d 6669   author_email=fi
-000011d0: 6e64 5f6d 6574 6128 2265 6d61 696c 2229  nd_meta("email")
-000011e0: 2c0a 2020 2020 2020 2020 6d61 696e 7461  ,.        mainta
-000011f0: 696e 6572 3d66 696e 645f 6d65 7461 2822  iner=find_meta("
-00001200: 6175 7468 6f72 2229 2c0a 2020 2020 2020  author"),.      
-00001210: 2020 6d61 696e 7461 696e 6572 5f65 6d61    maintainer_ema
-00001220: 696c 3d66 696e 645f 6d65 7461 2822 656d  il=find_meta("em
-00001230: 6169 6c22 292c 0a20 2020 2020 2020 206b  ail"),.        k
-00001240: 6579 776f 7264 733d 4b45 5957 4f52 4453  eywords=KEYWORDS
-00001250: 2c0a 2020 2020 2020 2020 6c6f 6e67 5f64  ,.        long_d
-00001260: 6573 6372 6970 7469 6f6e 3d4c 4f4e 472c  escription=LONG,
-00001270: 0a20 2020 2020 2020 206c 6f6e 675f 6465  .        long_de
-00001280: 7363 7269 7074 696f 6e5f 636f 6e74 656e  scription_conten
-00001290: 745f 7479 7065 3d22 7465 7874 2f6d 6172  t_type="text/mar
-000012a0: 6b64 6f77 6e22 2c0a 2020 2020 2020 2020  kdown",.        
-000012b0: 7061 636b 6167 6573 3d50 4143 4b41 4745  packages=PACKAGE
-000012c0: 532c 0a20 2020 2020 2020 2070 6163 6b61  S,.        packa
-000012d0: 6765 5f64 6972 3d7b 2222 3a20 2273 7263  ge_dir={"": "src
-000012e0: 227d 2c0a 2020 2020 2020 2020 7079 7468  "},.        pyth
-000012f0: 6f6e 5f72 6571 7569 7265 733d 223e 3d33  on_requires=">=3
-00001300: 2e36 222c 0a20 2020 2020 2020 207a 6970  .6",.        zip
-00001310: 5f73 6166 653d 4661 6c73 652c 0a20 2020  _safe=False,.   
-00001320: 2020 2020 2063 6c61 7373 6966 6965 7273       classifiers
-00001330: 3d43 4c41 5353 4946 4945 5253 2c0a 2020  =CLASSIFIERS,.  
-00001340: 2020 2020 2020 696e 7374 616c 6c5f 7265        install_re
-00001350: 7175 6972 6573 3d49 4e53 5441 4c4c 5f52  quires=INSTALL_R
-00001360: 4551 5549 5245 532c 0a20 2020 2020 2020  EQUIRES,.       
-00001370: 2065 7874 7261 735f 7265 7175 6972 653d   extras_require=
-00001380: 4558 5452 4153 5f52 4551 5549 5245 2c0a  EXTRAS_REQUIRE,.
-00001390: 2020 2020 2020 2020 696e 636c 7564 655f          include_
-000013a0: 7061 636b 6167 655f 6461 7461 3d54 7275  package_data=Tru
-000013b0: 652c 0a20 2020 2029 0a                   e,.    ).
+00000020: 5b62 7569 6c64 2d73 7973 7465 6d5d 0a72  [build-system].r
+00000030: 6571 7569 7265 7320 3d20 5b22 6861 7463  equires = ["hatc
+00000040: 686c 696e 6722 2c20 2268 6174 6368 2d76  hling", "hatch-v
+00000050: 6373 222c 2022 6861 7463 682d 6661 6e63  cs", "hatch-fanc
+00000060: 792d 7079 7069 2d72 6561 646d 6522 5d0a  y-pypi-readme"].
+00000070: 6275 696c 642d 6261 636b 656e 6420 3d20  build-backend = 
+00000080: 2268 6174 6368 6c69 6e67 2e62 7569 6c64  "hatchling.build
+00000090: 220a 0a0a 5b70 726f 6a65 6374 5d0a 6e61  "...[project].na
+000000a0: 6d65 203d 2022 6174 7472 7322 0a61 7574  me = "attrs".aut
+000000b0: 686f 7273 203d 205b 7b20 6e61 6d65 203d  hors = [{ name =
+000000c0: 2022 4879 6e65 6b20 5363 686c 6177 6163   "Hynek Schlawac
+000000d0: 6b22 2c20 656d 6169 6c20 3d20 2268 7340  k", email = "hs@
+000000e0: 6f78 2e63 7822 207d 5d0a 6c69 6365 6e73  ox.cx" }].licens
+000000f0: 6520 3d20 224d 4954 220a 7265 7175 6972  e = "MIT".requir
+00000100: 6573 2d70 7974 686f 6e20 3d20 223e 3d33  es-python = ">=3
+00000110: 2e37 220a 6465 7363 7269 7074 696f 6e20  .7".description 
+00000120: 3d20 2243 6c61 7373 6573 2057 6974 686f  = "Classes Witho
+00000130: 7574 2042 6f69 6c65 7270 6c61 7465 220a  ut Boilerplate".
+00000140: 6b65 7977 6f72 6473 203d 205b 2263 6c61  keywords = ["cla
+00000150: 7373 222c 2022 6174 7472 6962 7574 6522  ss", "attribute"
+00000160: 2c20 2262 6f69 6c65 7270 6c61 7465 225d  , "boilerplate"]
+00000170: 0a63 6c61 7373 6966 6965 7273 203d 205b  .classifiers = [
+00000180: 0a20 2020 2022 4465 7665 6c6f 706d 656e  .    "Developmen
+00000190: 7420 5374 6174 7573 203a 3a20 3520 2d20  t Status :: 5 - 
+000001a0: 5072 6f64 7563 7469 6f6e 2f53 7461 626c  Production/Stabl
+000001b0: 6522 2c0a 2020 2020 2249 6e74 656e 6465  e",.    "Intende
+000001c0: 6420 4175 6469 656e 6365 203a 3a20 4465  d Audience :: De
+000001d0: 7665 6c6f 7065 7273 222c 0a20 2020 2022  velopers",.    "
+000001e0: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
+000001f0: 7070 726f 7665 6420 3a3a 204d 4954 204c  pproved :: MIT L
+00000200: 6963 656e 7365 222c 0a20 2020 2022 5072  icense",.    "Pr
+00000210: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+00000220: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+00000230: 332e 3722 2c0a 2020 2020 2250 726f 6772  3.7",.    "Progr
+00000240: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000250: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e38  :: Python :: 3.8
+00000260: 222c 0a20 2020 2022 5072 6f67 7261 6d6d  ",.    "Programm
+00000270: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000280: 5079 7468 6f6e 203a 3a20 332e 3922 2c0a  Python :: 3.9",.
+00000290: 2020 2020 2250 726f 6772 616d 6d69 6e67      "Programming
+000002a0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+000002b0: 686f 6e20 3a3a 2033 2e31 3022 2c0a 2020  hon :: 3.10",.  
+000002c0: 2020 2250 726f 6772 616d 6d69 6e67 204c    "Programming L
+000002d0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+000002e0: 6e20 3a3a 2033 2e31 3122 2c0a 2020 2020  n :: 3.11",.    
+000002f0: 2250 726f 6772 616d 6d69 6e67 204c 616e  "Programming Lan
+00000300: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000310: 3a3a 2049 6d70 6c65 6d65 6e74 6174 696f  :: Implementatio
+00000320: 6e20 3a3a 2043 5079 7468 6f6e 222c 0a20  n :: CPython",. 
+00000330: 2020 2022 5072 6f67 7261 6d6d 696e 6720     "Programming 
+00000340: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000350: 6f6e 203a 3a20 496d 706c 656d 656e 7461  on :: Implementa
+00000360: 7469 6f6e 203a 3a20 5079 5079 222c 0a20  tion :: PyPy",. 
+00000370: 2020 2022 5479 7069 6e67 203a 3a20 5479     "Typing :: Ty
+00000380: 7065 6422 2c0a 5d0a 6465 7065 6e64 656e  ped",.].dependen
+00000390: 6369 6573 203d 205b 2269 6d70 6f72 746c  cies = ["importl
+000003a0: 6962 5f6d 6574 6164 6174 613b 7079 7468  ib_metadata;pyth
+000003b0: 6f6e 5f76 6572 7369 6f6e 3c27 332e 3827  on_version<'3.8'
+000003c0: 225d 0a64 796e 616d 6963 203d 205b 2276  "].dynamic = ["v
+000003d0: 6572 7369 6f6e 222c 2022 7265 6164 6d65  ersion", "readme
+000003e0: 225d 0a0a 5b70 726f 6a65 6374 2e6f 7074  "]..[project.opt
+000003f0: 696f 6e61 6c2d 6465 7065 6e64 656e 6369  ional-dependenci
+00000400: 6573 5d0a 7465 7374 732d 6e6f 2d7a 6f70  es].tests-no-zop
+00000410: 6520 3d20 5b0a 2020 2020 2320 466f 7220  e = [.    # For 
+00000420: 7265 6772 6573 7369 6f6e 2074 6573 7420  regression test 
+00000430: 746f 2065 6e73 7572 6520 636c 6f75 6470  to ensure cloudp
+00000440: 6963 6b6c 6520 636f 6d70 6174 2064 6f65  ickle compat doe
+00000450: 736e 2774 2062 7265 616b 2e0a 2020 2020  sn't break..    
+00000460: 2763 6c6f 7564 7069 636b 6c65 3b20 7079  'cloudpickle; py
+00000470: 7468 6f6e 5f69 6d70 6c65 6d65 6e74 6174  thon_implementat
+00000480: 696f 6e20 3d3d 2022 4350 7974 686f 6e22  ion == "CPython"
+00000490: 272c 0a20 2020 2022 6879 706f 7468 6573  ',.    "hypothes
+000004a0: 6973 222c 0a20 2020 2022 7079 6d70 6c65  is",.    "pymple
+000004b0: 7222 2c0a 2020 2020 2320 342e 332e 3020  r",.    # 4.3.0 
+000004c0: 6472 6f70 7065 6420 6c61 7374 2075 7365  dropped last use
+000004d0: 206f 6620 6063 6f6e 7665 7274 600a 2020   of `convert`.  
+000004e0: 2020 2270 7974 6573 743e 3d34 2e33 2e30    "pytest>=4.3.0
+000004f0: 222c 0a20 2020 2022 7079 7465 7374 2d78  ",.    "pytest-x
+00000500: 6469 7374 5b70 7375 7469 6c5d 222c 0a20  dist[psutil]",. 
+00000510: 2020 2023 2053 696e 6365 2074 6865 206d     # Since the m
+00000520: 7970 7920 6572 726f 7220 6d65 7373 6167  ypy error messag
+00000530: 6573 206b 6565 7020 6368 616e 6769 6e67  es keep changing
+00000540: 2c20 7765 2068 6176 6520 746f 206b 6565  , we have to kee
+00000550: 7020 7570 6461 7469 6e67 2074 6869 730a  p updating this.
+00000560: 2020 2020 2320 7069 6e2e 0a20 2020 2027      # pin..    '
+00000570: 6d79 7079 3e3d 312e 312e 313b 2070 7974  mypy>=1.1.1; pyt
+00000580: 686f 6e5f 696d 706c 656d 656e 7461 7469  hon_implementati
+00000590: 6f6e 203d 3d20 2243 5079 7468 6f6e 2227  on == "CPython"'
+000005a0: 2c0a 2020 2020 2770 7974 6573 742d 6d79  ,.    'pytest-my
+000005b0: 7079 2d70 6c75 6769 6e73 3b20 7079 7468  py-plugins; pyth
+000005c0: 6f6e 5f69 6d70 6c65 6d65 6e74 6174 696f  on_implementatio
+000005d0: 6e20 3d3d 2022 4350 7974 686f 6e22 2061  n == "CPython" a
+000005e0: 6e64 2070 7974 686f 6e5f 7665 7273 696f  nd python_versio
+000005f0: 6e3c 2233 2e31 3122 272c 0a5d 0a74 6573  n<"3.11"',.].tes
+00000600: 7473 203d 205b 2261 7474 7273 5b74 6573  ts = ["attrs[tes
+00000610: 7473 2d6e 6f2d 7a6f 7065 5d22 2c20 227a  ts-no-zope]", "z
+00000620: 6f70 652e 696e 7465 7266 6163 6522 5d0a  ope.interface"].
+00000630: 636f 7620 3d20 5b0a 2020 2020 2261 7474  cov = [.    "att
+00000640: 7273 5b74 6573 7473 5d22 2c0a 2020 2020  rs[tests]",.    
+00000650: 2320 456e 7375 7265 2063 6f76 6572 6167  # Ensure coverag
+00000660: 6520 6973 206e 6577 2065 6e6f 7567 6820  e is new enough 
+00000670: 666f 7220 6073 6f75 7263 655f 706b 6773  for `source_pkgs
+00000680: 602e 0a20 2020 2022 636f 7665 7261 6765  `..    "coverage
+00000690: 5b74 6f6d 6c5d 3e3d 352e 3322 2c0a 5d0a  [toml]>=5.3",.].
+000006a0: 646f 6373 203d 205b 0a20 2020 2022 6675  docs = [.    "fu
+000006b0: 726f 222c 0a20 2020 2022 6d79 7374 2d70  ro",.    "myst-p
+000006c0: 6172 7365 7222 2c0a 2020 2020 2273 7068  arser",.    "sph
+000006d0: 696e 7822 2c0a 2020 2020 227a 6f70 652e  inx",.    "zope.
+000006e0: 696e 7465 7266 6163 6522 2c0a 2020 2020  interface",.    
+000006f0: 2273 7068 696e 782d 6e6f 7466 6f75 6e64  "sphinx-notfound
+00000700: 2d70 6167 6522 2c0a 2020 2020 2273 7068  -page",.    "sph
+00000710: 696e 7863 6f6e 7472 6962 2d74 6f77 6e63  inxcontrib-townc
+00000720: 7269 6572 222c 0a20 2020 2022 746f 776e  rier",.    "town
+00000730: 6372 6965 7222 2c0a 5d0a 6465 7620 3d20  crier",.].dev = 
+00000740: 5b22 6174 7472 735b 7465 7374 732c 646f  ["attrs[tests,do
+00000750: 6373 5d22 2c20 2270 7265 2d63 6f6d 6d69  cs]", "pre-commi
+00000760: 7422 5d0a 0a5b 7072 6f6a 6563 742e 7572  t"]..[project.ur
+00000770: 6c73 5d0a 446f 6375 6d65 6e74 6174 696f  ls].Documentatio
+00000780: 6e20 3d20 2268 7474 7073 3a2f 2f77 7777  n = "https://www
+00000790: 2e61 7474 7273 2e6f 7267 2f22 0a43 6861  .attrs.org/".Cha
+000007a0: 6e67 656c 6f67 203d 2022 6874 7470 733a  ngelog = "https:
+000007b0: 2f2f 7777 772e 6174 7472 732e 6f72 672f  //www.attrs.org/
+000007c0: 656e 2f73 7461 626c 652f 6368 616e 6765  en/stable/change
+000007d0: 6c6f 672e 6874 6d6c 220a 2242 7567 2054  log.html"."Bug T
+000007e0: 7261 636b 6572 2220 3d20 2268 7474 7073  racker" = "https
+000007f0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7079  ://github.com/py
+00000800: 7468 6f6e 2d61 7474 7273 2f61 7474 7273  thon-attrs/attrs
+00000810: 2f69 7373 7565 7322 0a22 536f 7572 6365  /issues"."Source
+00000820: 2043 6f64 6522 203d 2022 6874 7470 733a   Code" = "https:
+00000830: 2f2f 6769 7468 7562 2e63 6f6d 2f70 7974  //github.com/pyt
+00000840: 686f 6e2d 6174 7472 732f 6174 7472 7322  hon-attrs/attrs"
+00000850: 0a46 756e 6469 6e67 203d 2022 6874 7470  .Funding = "http
+00000860: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
+00000870: 706f 6e73 6f72 732f 6879 6e65 6b22 0a54  ponsors/hynek".T
+00000880: 6964 656c 6966 7420 3d20 2268 7474 7073  idelift = "https
+00000890: 3a2f 2f74 6964 656c 6966 742e 636f 6d2f  ://tidelift.com/
+000008a0: 7375 6273 6372 6970 7469 6f6e 2f70 6b67  subscription/pkg
+000008b0: 2f70 7970 692d 6174 7472 733f 7574 6d5f  /pypi-attrs?utm_
+000008c0: 736f 7572 6365 3d70 7970 692d 6174 7472  source=pypi-attr
+000008d0: 7326 7574 6d5f 6d65 6469 756d 3d70 7970  s&utm_medium=pyp
+000008e0: 6922 0a0a 0a5b 746f 6f6c 2e68 6174 6368  i"...[tool.hatch
+000008f0: 2e76 6572 7369 6f6e 5d0a 736f 7572 6365  .version].source
+00000900: 203d 2022 7663 7322 0a72 6177 2d6f 7074   = "vcs".raw-opt
+00000910: 696f 6e73 203d 207b 206c 6f63 616c 5f73  ions = { local_s
+00000920: 6368 656d 6520 3d20 226e 6f2d 6c6f 6361  cheme = "no-loca
+00000930: 6c2d 7665 7273 696f 6e22 207d 0a0a 5b74  l-version" }..[t
+00000940: 6f6f 6c2e 6861 7463 682e 6275 696c 642e  ool.hatch.build.
+00000950: 7461 7267 6574 732e 7768 6565 6c5d 0a70  targets.wheel].p
+00000960: 6163 6b61 6765 7320 3d20 5b22 7372 632f  ackages = ["src/
+00000970: 6174 7472 222c 2022 7372 632f 6174 7472  attr", "src/attr
+00000980: 7322 5d0a 0a5b 746f 6f6c 2e68 6174 6368  s"]..[tool.hatch
+00000990: 2e6d 6574 6164 6174 612e 686f 6f6b 732e  .metadata.hooks.
+000009a0: 6661 6e63 792d 7079 7069 2d72 6561 646d  fancy-pypi-readm
+000009b0: 655d 0a63 6f6e 7465 6e74 2d74 7970 6520  e].content-type 
+000009c0: 3d20 2274 6578 742f 6d61 726b 646f 776e  = "text/markdown
+000009d0: 220a 0a23 2050 7950 4920 646f 6573 6e27  "..# PyPI doesn'
+000009e0: 7420 7375 7070 6f72 7420 7468 6520 3c70  t support the <p
+000009f0: 6963 7475 7265 3e20 7461 672e 0a5b 5b74  icture> tag..[[t
+00000a00: 6f6f 6c2e 6861 7463 682e 6d65 7461 6461  ool.hatch.metada
+00000a10: 7461 2e68 6f6f 6b73 2e66 616e 6379 2d70  ta.hooks.fancy-p
+00000a20: 7970 692d 7265 6164 6d65 2e66 7261 676d  ypi-readme.fragm
+00000a30: 656e 7473 5d5d 0a74 6578 7420 3d20 2222  ents]].text = ""
+00000a40: 223c 7020 616c 6967 6e3d 2263 656e 7465  "<p align="cente
+00000a50: 7222 3e0a 2020 3c61 2068 7265 663d 2268  r">.  <a href="h
+00000a60: 7474 7073 3a2f 2f77 7777 2e61 7474 7273  ttps://www.attrs
+00000a70: 2e6f 7267 2f22 3e0a 2020 2020 3c69 6d67  .org/">.    <img
+00000a80: 2073 7263 3d22 6874 7470 733a 2f2f 7261   src="https://ra
+00000a90: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
+00000aa0: 656e 742e 636f 6d2f 7079 7468 6f6e 2d61  ent.com/python-a
+00000ab0: 7474 7273 2f61 7474 7273 2f6d 6169 6e2f  ttrs/attrs/main/
+00000ac0: 646f 6373 2f5f 7374 6174 6963 2f61 7474  docs/_static/att
+00000ad0: 7273 5f6c 6f67 6f2e 7376 6722 2077 6964  rs_logo.svg" wid
+00000ae0: 7468 3d22 3335 2522 2061 6c74 3d22 6174  th="35%" alt="at
+00000af0: 7472 7322 202f 3e0a 2020 3c2f 613e 0a3c  trs" />.  </a>.<
+00000b00: 2f70 3e0a 2222 220a 0a5b 5b74 6f6f 6c2e  /p>."""..[[tool.
+00000b10: 6861 7463 682e 6d65 7461 6461 7461 2e68  hatch.metadata.h
+00000b20: 6f6f 6b73 2e66 616e 6379 2d70 7970 692d  ooks.fancy-pypi-
+00000b30: 7265 6164 6d65 2e66 7261 676d 656e 7473  readme.fragments
+00000b40: 5d5d 0a70 6174 6820 3d20 2252 4541 444d  ]].path = "READM
+00000b50: 452e 6d64 220a 7374 6172 742d 6166 7465  E.md".start-afte
+00000b60: 7220 3d20 223c 212d 2d20 7465 6173 6572  r = "<!-- teaser
+00000b70: 2d62 6567 696e 202d 2d3e 220a 0a5b 5b74  -begin -->"..[[t
+00000b80: 6f6f 6c2e 6861 7463 682e 6d65 7461 6461  ool.hatch.metada
+00000b90: 7461 2e68 6f6f 6b73 2e66 616e 6379 2d70  ta.hooks.fancy-p
+00000ba0: 7970 692d 7265 6164 6d65 2e66 7261 676d  ypi-readme.fragm
+00000bb0: 656e 7473 5d5d 0a74 6578 7420 3d20 2222  ents]].text = ""
+00000bc0: 220a 0a23 2320 5265 6c65 6173 6520 496e  "..## Release In
+00000bd0: 666f 726d 6174 696f 6e0a 0a22 2222 0a0a  formation.."""..
+00000be0: 5b5b 746f 6f6c 2e68 6174 6368 2e6d 6574  [[tool.hatch.met
+00000bf0: 6164 6174 612e 686f 6f6b 732e 6661 6e63  adata.hooks.fanc
+00000c00: 792d 7079 7069 2d72 6561 646d 652e 6672  y-pypi-readme.fr
+00000c10: 6167 6d65 6e74 735d 5d0a 7061 7468 203d  agments]].path =
+00000c20: 2022 4348 414e 4745 4c4f 472e 6d64 220a   "CHANGELOG.md".
+00000c30: 7061 7474 6572 6e20 3d20 225c 6e28 2323  pattern = "\n(##
+00000c40: 232e 2b3f 5c6e 2923 2320 220a 0a5b 5b74  #.+?\n)## "..[[t
+00000c50: 6f6f 6c2e 6861 7463 682e 6d65 7461 6461  ool.hatch.metada
+00000c60: 7461 2e68 6f6f 6b73 2e66 616e 6379 2d70  ta.hooks.fancy-p
+00000c70: 7970 692d 7265 6164 6d65 2e66 7261 676d  ypi-readme.fragm
+00000c80: 656e 7473 5d5d 0a74 6578 7420 3d20 2222  ents]].text = ""
+00000c90: 220a 0a2d 2d2d 0a0a 5b46 756c 6c20 6368  "..---..[Full ch
+00000ca0: 616e 6765 6c6f 675d 2868 7474 7073 3a2f  angelog](https:/
+00000cb0: 2f77 7777 2e61 7474 7273 2e6f 7267 2f65  /www.attrs.org/e
+00000cc0: 6e2f 7374 6162 6c65 2f63 6861 6e67 656c  n/stable/changel
+00000cd0: 6f67 2e68 746d 6c29 0a22 2222 0a0a 0a23  og.html)."""...#
+00000ce0: 204d 616b 6520 636f 7665 7261 6765 2070   Make coverage p
+00000cf0: 6c61 7920 6e69 6365 6c79 2077 6974 6820  lay nicely with 
+00000d00: 7079 7465 7374 2d78 6469 7374 2e0a 5b74  pytest-xdist..[t
+00000d10: 6f6f 6c2e 6861 7463 682e 6275 696c 642e  ool.hatch.build.
+00000d20: 7461 7267 6574 732e 7768 6565 6c2e 686f  targets.wheel.ho
+00000d30: 6f6b 732e 6175 746f 7275 6e5d 0a64 6570  oks.autorun].dep
+00000d40: 656e 6465 6e63 6965 7320 3d20 5b22 6861  endencies = ["ha
+00000d50: 7463 682d 6175 746f 7275 6e22 5d0a 636f  tch-autorun"].co
+00000d60: 6465 203d 2022 2222 0a69 6d70 6f72 7420  de = """.import 
+00000d70: 636f 7665 7261 6765 0a63 6f76 6572 6167  coverage.coverag
+00000d80: 652e 7072 6f63 6573 735f 7374 6172 7475  e.process_startu
+00000d90: 7028 290a 2222 220a 656e 6162 6c65 2d62  p().""".enable-b
+00000da0: 792d 6465 6661 756c 7420 3d20 6661 6c73  y-default = fals
+00000db0: 650a 0a0a 5b74 6f6f 6c2e 7079 7465 7374  e...[tool.pytest
+00000dc0: 2e69 6e69 5f6f 7074 696f 6e73 5d0a 6164  .ini_options].ad
+00000dd0: 646f 7074 7320 3d20 5b22 2d72 6122 2c20  dopts = ["-ra", 
+00000de0: 222d 2d73 7472 6963 742d 6d61 726b 6572  "--strict-marker
+00000df0: 7322 2c20 222d 2d73 7472 6963 742d 636f  s", "--strict-co
+00000e00: 6e66 6967 225d 0a78 6661 696c 5f73 7472  nfig"].xfail_str
+00000e10: 6963 7420 3d20 7472 7565 0a74 6573 7470  ict = true.testp
+00000e20: 6174 6873 203d 2022 7465 7374 7322 0a66  aths = "tests".f
+00000e30: 696c 7465 7277 6172 6e69 6e67 7320 3d20  ilterwarnings = 
+00000e40: 5b22 6f6e 6365 3a3a 5761 726e 696e 6722  ["once::Warning"
+00000e50: 2c20 2269 676e 6f72 653a 3a3a 7079 6d70  , "ignore:::pymp
+00000e60: 6c65 725b 2e2a 5d22 5d0a 0a0a 5b74 6f6f  ler[.*]"]...[too
+00000e70: 6c2e 636f 7665 7261 6765 2e72 756e 5d0a  l.coverage.run].
+00000e80: 7061 7261 6c6c 656c 203d 2074 7275 650a  parallel = true.
+00000e90: 6272 616e 6368 203d 2074 7275 650a 736f  branch = true.so
+00000ea0: 7572 6365 5f70 6b67 7320 3d20 5b22 6174  urce_pkgs = ["at
+00000eb0: 7472 222c 2022 6174 7472 7322 5d0a 0a5b  tr", "attrs"]..[
+00000ec0: 746f 6f6c 2e63 6f76 6572 6167 652e 7061  tool.coverage.pa
+00000ed0: 7468 735d 0a73 6f75 7263 6520 3d20 5b22  ths].source = ["
+00000ee0: 7372 6322 2c20 222e 746f 782f 7079 2a2f  src", ".tox/py*/
+00000ef0: 2a2a 2f73 6974 652d 7061 636b 6167 6573  **/site-packages
+00000f00: 225d 0a0a 5b74 6f6f 6c2e 636f 7665 7261  "]..[tool.covera
+00000f10: 6765 2e72 6570 6f72 745d 0a73 686f 775f  ge.report].show_
+00000f20: 6d69 7373 696e 6720 3d20 7472 7565 0a73  missing = true.s
+00000f30: 6b69 705f 636f 7665 7265 6420 3d20 7472  kip_covered = tr
+00000f40: 7565 0a65 7863 6c75 6465 5f6c 696e 6573  ue.exclude_lines
+00000f50: 203d 205b 0a20 2020 2022 7072 6167 6d61   = [.    "pragma
+00000f60: 3a20 6e6f 2063 6f76 6572 222c 0a20 2020  : no cover",.   
+00000f70: 2023 2050 7950 7920 6973 2075 6e61 6363   # PyPy is unacc
+00000f80: 6570 7461 626c 7920 736c 6f77 2075 6e64  eptably slow und
+00000f90: 6572 2063 6f76 6572 6167 652e 0a20 2020  er coverage..   
+00000fa0: 2022 6966 2050 5950 593a 222c 0a5d 0a0a   "if PYPY:",.]..
+00000fb0: 0a5b 746f 6f6c 2e62 6c61 636b 5d0a 6c69  .[tool.black].li
+00000fc0: 6e65 2d6c 656e 6774 6820 3d20 3739 0a0a  ne-length = 79..
+00000fd0: 0a5b 746f 6f6c 2e69 736f 7274 5d0a 7072  .[tool.isort].pr
+00000fe0: 6f66 696c 6520 3d20 2261 7474 7273 220a  ofile = "attrs".
+00000ff0: 0a0a 5b74 6f6f 6c2e 696e 7465 7272 6f67  ..[tool.interrog
+00001000: 6174 655d 0a76 6572 626f 7365 203d 2032  ate].verbose = 2
+00001010: 0a66 6169 6c2d 756e 6465 7220 3d20 3130  .fail-under = 10
+00001020: 300a 7768 6974 656c 6973 742d 7265 6765  0.whitelist-rege
+00001030: 7820 3d20 5b22 7465 7374 5f2e 2a22 5d0a  x = ["test_.*"].
+00001040: 0a0a 5b74 6f6f 6c2e 6368 6563 6b2d 7768  ..[tool.check-wh
+00001050: 6565 6c2d 636f 6e74 656e 7473 5d0a 746f  eel-contents].to
+00001060: 706c 6576 656c 203d 205b 2261 7474 7222  plevel = ["attr"
+00001070: 2c20 2261 7474 7273 225d 0a0a 0a5b 746f  , "attrs"]...[to
+00001080: 6f6c 2e74 6f77 6e63 7269 6572 5d0a 6e61  ol.towncrier].na
+00001090: 6d65 203d 2022 6174 7472 7322 0a64 6972  me = "attrs".dir
+000010a0: 6563 746f 7279 203d 2022 6368 616e 6765  ectory = "change
+000010b0: 6c6f 672e 6422 0a66 696c 656e 616d 6520  log.d".filename 
+000010c0: 3d20 2243 4841 4e47 454c 4f47 2e6d 6422  = "CHANGELOG.md"
+000010d0: 0a73 7461 7274 5f73 7472 696e 6720 3d20  .start_string = 
+000010e0: 223c 212d 2d20 746f 776e 6372 6965 7220  "<!-- towncrier 
+000010f0: 7265 6c65 6173 6520 6e6f 7465 7320 7374  release notes st
+00001100: 6172 7420 2d2d 3e5c 6e22 0a74 656d 706c  art -->\n".templ
+00001110: 6174 6520 3d20 2263 6861 6e67 656c 6f67  ate = "changelog
+00001120: 2e64 2f74 6f77 6e63 7269 6572 5f74 656d  .d/towncrier_tem
+00001130: 706c 6174 652e 6d64 2e6a 696e 6a61 220a  plate.md.jinja".
+00001140: 7469 746c 655f 666f 726d 6174 203d 2022  title_format = "
+00001150: 220a 6973 7375 655f 666f 726d 6174 203d  ".issue_format =
+00001160: 2022 5b23 7b69 7373 7565 7d5d 2868 7474   "[#{issue}](htt
+00001170: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00001180: 7079 7468 6f6e 2d61 7474 7273 2f61 7474  python-attrs/att
+00001190: 7273 2f69 7373 7565 732f 7b69 7373 7565  rs/issues/{issue
+000011a0: 7d29 220a 756e 6465 726c 696e 6573 203d  })".underlines =
+000011b0: 205b 2222 2c20 2222 2c20 2222 5d0a 0a5b   ["", "", ""]..[
+000011c0: 5b74 6f6f 6c2e 746f 776e 6372 6965 722e  [tool.towncrier.
+000011d0: 7365 6374 696f 6e5d 5d0a 7061 7468 203d  section]].path =
+000011e0: 2022 220a 0a5b 5b74 6f6f 6c2e 746f 776e   ""..[[tool.town
+000011f0: 6372 6965 722e 7479 7065 5d5d 0a64 6972  crier.type]].dir
+00001200: 6563 746f 7279 203d 2022 6272 6561 6b69  ectory = "breaki
+00001210: 6e67 220a 6e61 6d65 203d 2022 4261 636b  ng".name = "Back
+00001220: 7761 7264 732d 696e 636f 6d70 6174 6962  wards-incompatib
+00001230: 6c65 2043 6861 6e67 6573 220a 7368 6f77  le Changes".show
+00001240: 636f 6e74 656e 7420 3d20 7472 7565 0a0a  content = true..
+00001250: 5b5b 746f 6f6c 2e74 6f77 6e63 7269 6572  [[tool.towncrier
+00001260: 2e74 7970 655d 5d0a 6469 7265 6374 6f72  .type]].director
+00001270: 7920 3d20 2264 6570 7265 6361 7469 6f6e  y = "deprecation
+00001280: 220a 6e61 6d65 203d 2022 4465 7072 6563  ".name = "Deprec
+00001290: 6174 696f 6e73 220a 7368 6f77 636f 6e74  ations".showcont
+000012a0: 656e 7420 3d20 7472 7565 0a0a 5b5b 746f  ent = true..[[to
+000012b0: 6f6c 2e74 6f77 6e63 7269 6572 2e74 7970  ol.towncrier.typ
+000012c0: 655d 5d0a 6469 7265 6374 6f72 7920 3d20  e]].directory = 
+000012d0: 2263 6861 6e67 6522 0a6e 616d 6520 3d20  "change".name = 
+000012e0: 2243 6861 6e67 6573 220a 7368 6f77 636f  "Changes".showco
+000012f0: 6e74 656e 7420 3d20 7472 7565 0a0a 0a5b  ntent = true...[
+00001300: 746f 6f6c 2e6d 7970 795d 0a64 6973 616c  tool.mypy].disal
+00001310: 6c6f 775f 756e 7479 7065 645f 6465 6673  low_untyped_defs
+00001320: 203d 2074 7275 650a 6368 6563 6b5f 756e   = true.check_un
+00001330: 7479 7065 645f 6465 6673 203d 2074 7275  typed_defs = tru
+00001340: 650a                                     e.
```

### Comparing `attrs-22.2.0/src/attr/__init__.pyi` & `attrs-23.1.0/src/attr/__init__.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -65,14 +65,15 @@
 # _ValidatorType from working when passed in a list or tuple.
 _ValidatorArgType = Union[_ValidatorType[_T], Sequence[_ValidatorType[_T]]]
 
 # We subclass this here to keep the protocol's qualified name clean.
 class AttrsInstance(AttrsInstance_, Protocol):
     pass
 
+_A = TypeVar("_A", bound=AttrsInstance)
 # _make --
 
 class _Nothing(enum.Enum):
     NOTHING = enum.auto()
 
 NOTHING = _Nothing.NOTHING
 
@@ -112,14 +113,15 @@
 # signature in the extension module using the specification linked above to
 # provide pyright support.
 def __dataclass_transform__(
     *,
     eq_default: bool = True,
     order_default: bool = False,
     kw_only_default: bool = False,
+    frozen_default: bool = False,
     field_descriptors: Tuple[Union[type, Callable[..., Any]], ...] = (()),
 ) -> Callable[[_T], _T]: ...
 
 class Attribute(Generic[_T]):
     name: str
     default: Optional[_T]
     validator: Optional[_ValidatorType[_T]]
@@ -253,14 +255,15 @@
     converter: None = ...,
     factory: None = ...,
     kw_only: bool = ...,
     eq: Optional[bool] = ...,
     order: Optional[bool] = ...,
     on_setattr: Optional[_OnSetAttrArgType] = ...,
     alias: Optional[str] = ...,
+    type: Optional[type] = ...,
 ) -> Any: ...
 
 # This form catches an explicit None or no default and infers the type from the
 # other arguments.
 @overload
 def field(
     *,
@@ -273,14 +276,15 @@
     converter: Optional[_ConverterType] = ...,
     factory: Optional[Callable[[], _T]] = ...,
     kw_only: bool = ...,
     eq: Optional[_EqOrderType] = ...,
     order: Optional[_EqOrderType] = ...,
     on_setattr: Optional[_OnSetAttrArgType] = ...,
     alias: Optional[str] = ...,
+    type: Optional[type] = ...,
 ) -> _T: ...
 
 # This form catches an explicit default argument.
 @overload
 def field(
     *,
     default: _T,
@@ -292,14 +296,15 @@
     converter: Optional[_ConverterType] = ...,
     factory: Optional[Callable[[], _T]] = ...,
     kw_only: bool = ...,
     eq: Optional[_EqOrderType] = ...,
     order: Optional[_EqOrderType] = ...,
     on_setattr: Optional[_OnSetAttrArgType] = ...,
     alias: Optional[str] = ...,
+    type: Optional[type] = ...,
 ) -> _T: ...
 
 # This form covers type=non-Type: e.g. forward references (str), Any
 @overload
 def field(
     *,
     default: Optional[_T] = ...,
@@ -311,14 +316,15 @@
     converter: Optional[_ConverterType] = ...,
     factory: Optional[Callable[[], _T]] = ...,
     kw_only: bool = ...,
     eq: Optional[_EqOrderType] = ...,
     order: Optional[_EqOrderType] = ...,
     on_setattr: Optional[_OnSetAttrArgType] = ...,
     alias: Optional[str] = ...,
+    type: Optional[type] = ...,
 ) -> Any: ...
 @overload
 @__dataclass_transform__(order_default=True, field_descriptors=(attrib, field))
 def attrs(
     maybe_cls: _C,
     these: Optional[Dict[str, Any]] = ...,
     repr_ns: Optional[str] = ...,
@@ -422,25 +428,81 @@
     getstate_setstate: Optional[bool] = ...,
     on_setattr: Optional[_OnSetAttrArgType] = ...,
     field_transformer: Optional[_FieldTransformer] = ...,
     match_args: bool = ...,
 ) -> Callable[[_C], _C]: ...
 
 mutable = define
-frozen = define  # they differ only in their defaults
 
+@overload
+@__dataclass_transform__(
+    frozen_default=True, field_descriptors=(attrib, field)
+)
+def frozen(
+    maybe_cls: _C,
+    *,
+    these: Optional[Dict[str, Any]] = ...,
+    repr: bool = ...,
+    unsafe_hash: Optional[bool] = ...,
+    hash: Optional[bool] = ...,
+    init: bool = ...,
+    slots: bool = ...,
+    frozen: bool = ...,
+    weakref_slot: bool = ...,
+    str: bool = ...,
+    auto_attribs: bool = ...,
+    kw_only: bool = ...,
+    cache_hash: bool = ...,
+    auto_exc: bool = ...,
+    eq: Optional[bool] = ...,
+    order: Optional[bool] = ...,
+    auto_detect: bool = ...,
+    getstate_setstate: Optional[bool] = ...,
+    on_setattr: Optional[_OnSetAttrArgType] = ...,
+    field_transformer: Optional[_FieldTransformer] = ...,
+    match_args: bool = ...,
+) -> _C: ...
+@overload
+@__dataclass_transform__(
+    frozen_default=True, field_descriptors=(attrib, field)
+)
+def frozen(
+    maybe_cls: None = ...,
+    *,
+    these: Optional[Dict[str, Any]] = ...,
+    repr: bool = ...,
+    unsafe_hash: Optional[bool] = ...,
+    hash: Optional[bool] = ...,
+    init: bool = ...,
+    slots: bool = ...,
+    frozen: bool = ...,
+    weakref_slot: bool = ...,
+    str: bool = ...,
+    auto_attribs: bool = ...,
+    kw_only: bool = ...,
+    cache_hash: bool = ...,
+    auto_exc: bool = ...,
+    eq: Optional[bool] = ...,
+    order: Optional[bool] = ...,
+    auto_detect: bool = ...,
+    getstate_setstate: Optional[bool] = ...,
+    on_setattr: Optional[_OnSetAttrArgType] = ...,
+    field_transformer: Optional[_FieldTransformer] = ...,
+    match_args: bool = ...,
+) -> Callable[[_C], _C]: ...
 def fields(cls: Type[AttrsInstance]) -> Any: ...
 def fields_dict(cls: Type[AttrsInstance]) -> Dict[str, Attribute[Any]]: ...
 def validate(inst: AttrsInstance) -> None: ...
 def resolve_types(
-    cls: _C,
+    cls: _A,
     globalns: Optional[Dict[str, Any]] = ...,
     localns: Optional[Dict[str, Any]] = ...,
     attribs: Optional[List[Attribute[Any]]] = ...,
-) -> _C: ...
+    include_extras: bool = ...,
+) -> _A: ...
 
 # TODO: add support for returning a proper attrs class from the mypy plugin
 # we use Any instead of _CountingAttr so that e.g. `make_class('Foo',
 # [attr.ib()])` is valid
 def make_class(
     name: str,
     attrs: Union[List[str], Tuple[str, ...], Dict[str, Any]],
```

### Comparing `attrs-22.2.0/src/attr/_cmp.py` & `attrs-23.1.0/src/attr/_cmp.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,30 +16,30 @@
     le=None,
     gt=None,
     ge=None,
     require_same_type=True,
     class_name="Comparable",
 ):
     """
-    Create a class that can be passed into `attr.ib`'s ``eq``, ``order``, and
-    ``cmp`` arguments to customize field comparison.
+    Create a class that can be passed into `attrs.field`'s ``eq``, ``order``,
+    and ``cmp`` arguments to customize field comparison.
 
-    The resulting class will have a full set of ordering methods if
-    at least one of ``{lt, le, gt, ge}`` and ``eq``  are provided.
+    The resulting class will have a full set of ordering methods if at least
+    one of ``{lt, le, gt, ge}`` and ``eq``  are provided.
 
-    :param Optional[callable] eq: `callable` used to evaluate equality
-        of two objects.
-    :param Optional[callable] lt: `callable` used to evaluate whether
-        one object is less than another object.
-    :param Optional[callable] le: `callable` used to evaluate whether
-        one object is less than or equal to another object.
-    :param Optional[callable] gt: `callable` used to evaluate whether
-        one object is greater than another object.
-    :param Optional[callable] ge: `callable` used to evaluate whether
-        one object is greater than or equal to another object.
+    :param Optional[callable] eq: `callable` used to evaluate equality of two
+        objects.
+    :param Optional[callable] lt: `callable` used to evaluate whether one
+        object is less than another object.
+    :param Optional[callable] le: `callable` used to evaluate whether one
+        object is less than or equal to another object.
+    :param Optional[callable] gt: `callable` used to evaluate whether one
+        object is greater than another object.
+    :param Optional[callable] ge: `callable` used to evaluate whether one
+        object is greater than or equal to another object.
 
     :param bool require_same_type: When `True`, equality and ordering methods
         will return `NotImplemented` if objects are not of the same type.
 
     :param Optional[str] class_name: Name of class. Defaults to 'Comparable'.
 
     See `comparison` for more details.
```

### Comparing `attrs-22.2.0/src/attr/_compat.py` & `attrs-23.1.0/src/attr/_compat.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,17 +5,19 @@
 import platform
 import sys
 import threading
 import types
 import warnings
 
 from collections.abc import Mapping, Sequence  # noqa
+from typing import _GenericAlias
 
 
 PYPY = platform.python_implementation() == "PyPy"
+PY_3_9_PLUS = sys.version_info[:2] >= (3, 9)
 PY310 = sys.version_info[:2] >= (3, 10)
 PY_3_12_PLUS = sys.version_info[:2] >= (3, 12)
 
 
 def just_warn(*args, **kw):
     warnings.warn(
         "Running interpreter doesn't sufficiently support code object "
@@ -77,40 +79,40 @@
         def set_closure_cell(cell, value):
             cell.__setstate__((value,))
 
         return set_closure_cell
 
     # Otherwise gotta do it the hard way.
 
-    # Create a function that will set its first cellvar to `value`.
-    def set_first_cellvar_to(value):
-        x = value
-        return
-
-        # This function will be eliminated as dead code, but
-        # not before its reference to `x` forces `x` to be
-        # represented as a closure cell rather than a local.
-        def force_x_to_be_a_cell():  # pragma: no cover
-            return x
-
     try:
-        # Extract the code object and make sure our assumptions about
-        # the closure behavior are correct.
-        co = set_first_cellvar_to.__code__
-        if co.co_cellvars != ("x",) or co.co_freevars != ():
-            raise AssertionError  # pragma: no cover
-
-        # Convert this code object to a code object that sets the
-        # function's first _freevar_ (not cellvar) to the argument.
         if sys.version_info >= (3, 8):
 
             def set_closure_cell(cell, value):
                 cell.cell_contents = value
 
         else:
+            # Create a function that will set its first cellvar to `value`.
+            def set_first_cellvar_to(value):
+                x = value
+                return
+
+                # This function will be eliminated as dead code, but
+                # not before its reference to `x` forces `x` to be
+                # represented as a closure cell rather than a local.
+                def force_x_to_be_a_cell():  # pragma: no cover
+                    return x
+
+            # Extract the code object and make sure our assumptions about
+            # the closure behavior are correct.
+            co = set_first_cellvar_to.__code__
+            if co.co_cellvars != ("x",) or co.co_freevars != ():
+                raise AssertionError  # pragma: no cover
+
+            # Convert this code object to a code object that sets the
+            # function's first _freevar_ (not cellvar) to the argument.
             args = [co.co_argcount]
             args.append(co.co_kwonlyargcount)
             args.extend(
                 [
                     co.co_nlocals,
                     co.co_stacksize,
                     co.co_flags,
@@ -170,7 +172,14 @@
 # we need to know that we're already repr'ing the outside instance from within
 # the dict's repr() call.
 #
 # This lives here rather than in _make.py so that the functions in _make.py
 # don't have a direct reference to the thread-local in their globals dict.
 # If they have such a reference, it breaks cloudpickle.
 repr_context = threading.local()
+
+
+def get_generic_base(cl):
+    """If this is a generic class (A[str]), return the generic base for it."""
+    if cl.__class__ is _GenericAlias:
+        return cl.__origin__
+    return None
```

### Comparing `attrs-22.2.0/src/attr/_config.py` & `attrs-23.1.0/src/attr/_config.py`

 * *Files identical despite different names*

### Comparing `attrs-22.2.0/src/attr/_funcs.py` & `attrs-23.1.0/src/attr/_funcs.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 # SPDX-License-Identifier: MIT
 
 
 import copy
 
+from ._compat import PY_3_9_PLUS, get_generic_base
 from ._make import NOTHING, _obj_setattr, fields
 from .exceptions import AttrsAttributeNotFoundError
 
 
 def asdict(
     inst,
     recurse=True,
     filter=None,
     dict_factory=dict,
     retain_collection_types=False,
     value_serializer=None,
 ):
     """
-    Return the ``attrs`` attribute values of *inst* as a dict.
+    Return the *attrs* attribute values of *inst* as a dict.
 
-    Optionally recurse into other ``attrs``-decorated classes.
+    Optionally recurse into other *attrs*-decorated classes.
 
-    :param inst: Instance of an ``attrs``-decorated class.
+    :param inst: Instance of an *attrs*-decorated class.
     :param bool recurse: Recurse into classes that are also
-        ``attrs``-decorated.
+        *attrs*-decorated.
     :param callable filter: A callable whose return code determines whether an
         attribute or element is included (``True``) or dropped (``False``).  Is
         called with the `attrs.Attribute` as the first argument and the
         value as the second argument.
     :param callable dict_factory: A callable to produce dictionaries from.  For
         example, to produce ordered dictionaries instead of normal Python
         dictionaries, pass in ``collections.OrderedDict``.
@@ -36,15 +37,15 @@
     :param Optional[callable] value_serializer: A hook that is called for every
         attribute or dict key/value.  It receives the current instance, field
         and value and must return the (updated) value.  The hook is run *after*
         the optional *filter* has been applied.
 
     :rtype: return type of *dict_factory*
 
-    :raise attr.exceptions.NotAnAttrsClassError: If *cls* is not an ``attrs``
+    :raise attrs.exceptions.NotAnAttrsClassError: If *cls* is not an *attrs*
         class.
 
     ..  versionadded:: 16.0.0 *dict_factory*
     ..  versionadded:: 16.1.0 *retain_collection_types*
     ..  versionadded:: 20.3.0 *value_serializer*
     ..  versionadded:: 21.3.0 If a dict has a collection for a key, it is
         serialized as a tuple.
@@ -191,35 +192,35 @@
     inst,
     recurse=True,
     filter=None,
     tuple_factory=tuple,
     retain_collection_types=False,
 ):
     """
-    Return the ``attrs`` attribute values of *inst* as a tuple.
+    Return the *attrs* attribute values of *inst* as a tuple.
 
-    Optionally recurse into other ``attrs``-decorated classes.
+    Optionally recurse into other *attrs*-decorated classes.
 
-    :param inst: Instance of an ``attrs``-decorated class.
+    :param inst: Instance of an *attrs*-decorated class.
     :param bool recurse: Recurse into classes that are also
-        ``attrs``-decorated.
+        *attrs*-decorated.
     :param callable filter: A callable whose return code determines whether an
         attribute or element is included (``True``) or dropped (``False``).  Is
         called with the `attrs.Attribute` as the first argument and the
         value as the second argument.
     :param callable tuple_factory: A callable to produce tuples from.  For
         example, to produce lists instead of tuples.
     :param bool retain_collection_types: Do not convert to ``list``
         or ``dict`` when encountering an attribute which type is
         ``tuple``, ``dict`` or ``set``.  Only meaningful if ``recurse`` is
         ``True``.
 
     :rtype: return type of *tuple_factory*
 
-    :raise attr.exceptions.NotAnAttrsClassError: If *cls* is not an ``attrs``
+    :raise attrs.exceptions.NotAnAttrsClassError: If *cls* is not an *attrs*
         class.
 
     ..  versionadded:: 16.2.0
     """
     attrs = fields(inst.__class__)
     rv = []
     retain = retain_collection_types  # Very long. :/
@@ -285,92 +286,140 @@
             rv.append(v)
 
     return rv if tuple_factory is list else tuple_factory(rv)
 
 
 def has(cls):
     """
-    Check whether *cls* is a class with ``attrs`` attributes.
+    Check whether *cls* is a class with *attrs* attributes.
 
     :param type cls: Class to introspect.
     :raise TypeError: If *cls* is not a class.
 
     :rtype: bool
     """
-    return getattr(cls, "__attrs_attrs__", None) is not None
+    attrs = getattr(cls, "__attrs_attrs__", None)
+    if attrs is not None:
+        return True
+
+    # No attrs, maybe it's a specialized generic (A[str])?
+    generic_base = get_generic_base(cls)
+    if generic_base is not None:
+        generic_attrs = getattr(generic_base, "__attrs_attrs__", None)
+        if generic_attrs is not None:
+            # Stick it on here for speed next time.
+            cls.__attrs_attrs__ = generic_attrs
+        return generic_attrs is not None
+    return False
 
 
 def assoc(inst, **changes):
     """
     Copy *inst* and apply *changes*.
 
-    :param inst: Instance of a class with ``attrs`` attributes.
+    This is different from `evolve` that applies the changes to the arguments
+    that create the new instance.
+
+    `evolve`'s behavior is preferable, but there are `edge cases`_ where it
+    doesn't work. Therefore `assoc` is deprecated, but will not be removed.
+
+    .. _`edge cases`: https://github.com/python-attrs/attrs/issues/251
+
+    :param inst: Instance of a class with *attrs* attributes.
     :param changes: Keyword changes in the new copy.
 
     :return: A copy of inst with *changes* incorporated.
 
-    :raise attr.exceptions.AttrsAttributeNotFoundError: If *attr_name* couldn't
-        be found on *cls*.
-    :raise attr.exceptions.NotAnAttrsClassError: If *cls* is not an ``attrs``
+    :raise attrs.exceptions.AttrsAttributeNotFoundError: If *attr_name*
+        couldn't be found on *cls*.
+    :raise attrs.exceptions.NotAnAttrsClassError: If *cls* is not an *attrs*
         class.
 
     ..  deprecated:: 17.1.0
         Use `attrs.evolve` instead if you can.
         This function will not be removed du to the slightly different approach
         compared to `attrs.evolve`.
     """
-    import warnings
-
-    warnings.warn(
-        "assoc is deprecated and will be removed after 2018/01.",
-        DeprecationWarning,
-        stacklevel=2,
-    )
     new = copy.copy(inst)
     attrs = fields(inst.__class__)
     for k, v in changes.items():
         a = getattr(attrs, k, NOTHING)
         if a is NOTHING:
             raise AttrsAttributeNotFoundError(
                 f"{k} is not an attrs attribute on {new.__class__}."
             )
         _obj_setattr(new, k, v)
     return new
 
 
-def evolve(inst, **changes):
+def evolve(*args, **changes):
     """
-    Create a new instance, based on *inst* with *changes* applied.
+    Create a new instance, based on the first positional argument with
+    *changes* applied.
 
-    :param inst: Instance of a class with ``attrs`` attributes.
+    :param inst: Instance of a class with *attrs* attributes.
     :param changes: Keyword changes in the new copy.
 
     :return: A copy of inst with *changes* incorporated.
 
     :raise TypeError: If *attr_name* couldn't be found in the class
         ``__init__``.
-    :raise attr.exceptions.NotAnAttrsClassError: If *cls* is not an ``attrs``
+    :raise attrs.exceptions.NotAnAttrsClassError: If *cls* is not an *attrs*
         class.
 
-    ..  versionadded:: 17.1.0
-    """
+    .. versionadded:: 17.1.0
+    .. deprecated:: 23.1.0
+       It is now deprecated to pass the instance using the keyword argument
+       *inst*. It will raise a warning until at least April 2024, after which
+       it will become an error. Always pass the instance as a positional
+       argument.
+    """
+    # Try to get instance by positional argument first.
+    # Use changes otherwise and warn it'll break.
+    if args:
+        try:
+            (inst,) = args
+        except ValueError:
+            raise TypeError(
+                f"evolve() takes 1 positional argument, but {len(args)} "
+                "were given"
+            ) from None
+    else:
+        try:
+            inst = changes.pop("inst")
+        except KeyError:
+            raise TypeError(
+                "evolve() missing 1 required positional argument: 'inst'"
+            ) from None
+
+        import warnings
+
+        warnings.warn(
+            "Passing the instance per keyword argument is deprecated and "
+            "will stop working in, or after, April 2024.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+
     cls = inst.__class__
     attrs = fields(cls)
     for a in attrs:
         if not a.init:
             continue
         attr_name = a.name  # To deal with private attributes.
         init_name = a.alias
         if init_name not in changes:
             changes[init_name] = getattr(inst, attr_name)
 
     return cls(**changes)
 
 
-def resolve_types(cls, globalns=None, localns=None, attribs=None):
+def resolve_types(
+    cls, globalns=None, localns=None, attribs=None, include_extras=True
+):
     """
     Resolve any strings and forward annotations in type annotations.
 
     This is only required if you need concrete types in `Attribute`'s *type*
     field. In other words, you don't need to resolve your types if you only
     use them for static type checking.
 
@@ -381,35 +430,45 @@
     `typing.get_type_hints` for more details.
 
     :param type cls: Class to resolve.
     :param Optional[dict] globalns: Dictionary containing global variables.
     :param Optional[dict] localns: Dictionary containing local variables.
     :param Optional[list] attribs: List of attribs for the given class.
         This is necessary when calling from inside a ``field_transformer``
-        since *cls* is not an ``attrs`` class yet.
+        since *cls* is not an *attrs* class yet.
+    :param bool include_extras: Resolve more accurately, if possible.
+        Pass ``include_extras`` to ``typing.get_hints``, if supported by the
+        typing module. On supported Python versions (3.9+), this resolves the
+        types more accurately.
 
     :raise TypeError: If *cls* is not a class.
-    :raise attr.exceptions.NotAnAttrsClassError: If *cls* is not an ``attrs``
+    :raise attrs.exceptions.NotAnAttrsClassError: If *cls* is not an *attrs*
         class and you didn't pass any attribs.
     :raise NameError: If types cannot be resolved because of missing variables.
 
     :returns: *cls* so you can use this function also as a class decorator.
         Please note that you have to apply it **after** `attrs.define`. That
         means the decorator has to come in the line **before** `attrs.define`.
 
     ..  versionadded:: 20.1.0
     ..  versionadded:: 21.1.0 *attribs*
+    ..  versionadded:: 23.1.0 *include_extras*
 
     """
     # Since calling get_type_hints is expensive we cache whether we've
     # done it already.
     if getattr(cls, "__attrs_types_resolved__", None) != cls:
         import typing
 
-        hints = typing.get_type_hints(cls, globalns=globalns, localns=localns)
+        kwargs = {"globalns": globalns, "localns": localns}
+
+        if PY_3_9_PLUS:
+            kwargs["include_extras"] = include_extras
+
+        hints = typing.get_type_hints(cls, **kwargs)
         for field in fields(cls) if attribs is None else attribs:
             if field.name in hints:
                 # Since fields have been frozen we must work around it.
                 _obj_setattr(field, "type", hints[field.name])
         # We store the class we resolved so that subclasses know they haven't
         # been resolved.
         cls.__attrs_types_resolved__ = cls
```

### Comparing `attrs-22.2.0/src/attr/_make.py` & `attrs-23.1.0/src/attr/_make.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,20 @@
 import typing
 
 from operator import itemgetter
 
 # We need to import _compat itself in addition to the _compat members to avoid
 # having the thread-local in the globals here.
 from . import _compat, _config, setters
-from ._compat import PY310, PYPY, _AnnotationExtractor, set_closure_cell
+from ._compat import (
+    PY310,
+    _AnnotationExtractor,
+    get_generic_base,
+    set_closure_cell,
+)
 from .exceptions import (
     DefaultAlreadySetError,
     FrozenInstanceError,
     NotAnAttrsClassError,
     UnannotatedAttributeError,
 )
 
@@ -105,17 +110,20 @@
 ):
     """
     Create a new attribute on a class.
 
     ..  warning::
 
         Does *not* do anything unless the class is also decorated with
-        `attr.s`!
+        `attr.s` / `attrs.define` / et cetera!
+
+    Please consider using `attrs.field` in new code (``attr.ib`` will *never*
+    go away, though).
 
-    :param default: A value that is used if an ``attrs``-generated ``__init__``
+    :param default: A value that is used if an *attrs*-generated ``__init__``
         is used and no value is passed while instantiating or the attribute is
         excluded using ``init=False``.
 
         If the value is an instance of `attrs.Factory`, its callable will be
         used to construct a new value (useful for mutable data types like lists
         or dicts).
 
@@ -126,27 +134,27 @@
         The default can also be set using decorator notation as shown below.
 
     :type default: Any value
 
     :param callable factory: Syntactic sugar for
         ``default=attr.Factory(factory)``.
 
-    :param validator: `callable` that is called by ``attrs``-generated
+    :param validator: `callable` that is called by *attrs*-generated
         ``__init__`` methods after the instance has been initialized.  They
         receive the initialized instance, the :func:`~attrs.Attribute`, and the
         passed value.
 
         The return value is *not* inspected so the validator has to throw an
         exception itself.
 
         If a `list` is passed, its items are treated as validators and must
         all pass.
 
         Validators can be globally disabled and re-enabled using
-        `get_run_validators`.
+        `attrs.validators.get_disabled` / `attrs.validators.set_disabled`.
 
         The validator can also be set using decorator notation as shown below.
 
     :type validator: `callable` or a `list` of `callable`\\ s.
 
     :param repr: Include this attribute in the generated ``__repr__``
         method. If ``True``, include the attribute; if ``False``, omit it. By
@@ -180,28 +188,28 @@
         is the correct behavior according the Python spec.  Setting this value
         to anything else than ``None`` is *discouraged*.
     :param bool init: Include this attribute in the generated ``__init__``
         method.  It is possible to set this to ``False`` and set a default
         value.  In that case this attributed is unconditionally initialized
         with the specified default value or factory.
     :param callable converter: `callable` that is called by
-        ``attrs``-generated ``__init__`` methods to convert attribute's value
+        *attrs*-generated ``__init__`` methods to convert attribute's value
         to the desired format.  It is given the passed-in value, and the
         returned value will be used as the new value of the attribute.  The
         value is converted before being passed to the validator, if any.
     :param metadata: An arbitrary mapping, to be used by third-party
         components.  See `extending-metadata`.
 
     :param type: The type of the attribute. Nowadays, the preferred method to
         specify the type is using a variable annotation (see :pep:`526`).
         This argument is provided for backward compatibility.
         Regardless of the approach used, the type will be stored on
         ``Attribute.type``.
 
-        Please note that ``attrs`` doesn't do anything with this metadata by
+        Please note that *attrs* doesn't do anything with this metadata by
         itself. You can use it as part of your own code or for
         `static type checking <types>`.
     :param kw_only: Make this attribute keyword-only in the generated
         ``__init__`` (if ``init`` is ``False``, this parameter is ignored).
     :param on_setattr: Allows to overwrite the *on_setattr* setting from
         `attr.s`. If left `None`, the *on_setattr* value from `attr.s` is used.
         Set to `attrs.setters.NO_OP` to run **no** `setattr` hooks for this
@@ -578,36 +586,27 @@
     # add or remove attributes!
     attr_names = [a.name for a in attrs]
     AttrsClass = _make_attr_tuple_class(cls.__name__, attr_names)
 
     return _Attributes((AttrsClass(attrs), base_attrs, base_attr_map))
 
 
-if PYPY:
-
-    def _frozen_setattrs(self, name, value):
-        """
-        Attached to frozen classes as __setattr__.
-        """
-        if isinstance(self, BaseException) and name in (
-            "__cause__",
-            "__context__",
-        ):
-            BaseException.__setattr__(self, name, value)
-            return
-
-        raise FrozenInstanceError()
-
-else:
+def _frozen_setattrs(self, name, value):
+    """
+    Attached to frozen classes as __setattr__.
+    """
+    if isinstance(self, BaseException) and name in (
+        "__cause__",
+        "__context__",
+        "__traceback__",
+    ):
+        BaseException.__setattr__(self, name, value)
+        return
 
-    def _frozen_setattrs(self, name, value):
-        """
-        Attached to frozen classes as __setattr__.
-        """
-        raise FrozenInstanceError()
+    raise FrozenInstanceError()
 
 
 def _frozen_delattrs(self, name):
     """
     Attached to frozen classes as __delattr__.
     """
     raise FrozenInstanceError()
@@ -936,17 +935,23 @@
         hash_caching_enabled = self._cache_hash
 
         def slots_setstate(self, state):
             """
             Automatically created by attrs.
             """
             __bound_setattr = _obj_setattr.__get__(self)
-            for name in state_attr_names:
-                if name in state:
-                    __bound_setattr(name, state[name])
+            if isinstance(state, tuple):
+                # Backward compatibility with attrs instances pickled with
+                # attrs versions before v22.2.0 which stored tuples.
+                for name, value in zip(state_attr_names, state):
+                    __bound_setattr(name, value)
+            else:
+                for name in state_attr_names:
+                    if name in state:
+                        __bound_setattr(name, state[name])
 
             # The hash code cache is not included when the object is
             # serialized, but it still needs to be initialized to None to
             # indicate that the first call to __hash__ should be a cache
             # miss.
             if hash_caching_enabled:
                 __bound_setattr(_hash_cache_field, None)
@@ -1216,20 +1221,23 @@
     match_args=True,
     unsafe_hash=None,
 ):
     r"""
     A class decorator that adds :term:`dunder methods` according to the
     specified attributes using `attr.ib` or the *these* argument.
 
+    Please consider using `attrs.define` / `attrs.frozen` in new code
+    (``attr.s`` will *never* go away, though).
+
     :param these: A dictionary of name to `attr.ib` mappings.  This is
         useful to avoid the definition of your attributes within the class body
         because you can't (e.g. if you want to add ``__repr__`` methods to
         Django models) or don't want to.
 
-        If *these* is not ``None``, ``attrs`` will *not* search the class body
+        If *these* is not ``None``, *attrs* will *not* search the class body
         for attributes and will *not* remove any attributes from it.
 
         The order is deduced from the order of the attributes inside *these*.
 
     :type these: `dict` of `str` to `attr.ib`
 
     :param str repr_ns: When using nested classes, there's no way in Python 2
@@ -1238,69 +1246,69 @@
     :param bool auto_detect: Instead of setting the *init*, *repr*, *eq*,
         *order*, and *hash* arguments explicitly, assume they are set to
         ``True`` **unless any** of the involved methods for one of the
         arguments is implemented in the *current* class (i.e. it is *not*
         inherited from some base class).
 
         So for example by implementing ``__eq__`` on a class yourself,
-        ``attrs`` will deduce ``eq=False`` and will create *neither*
+        *attrs* will deduce ``eq=False`` and will create *neither*
         ``__eq__`` *nor* ``__ne__`` (but Python classes come with a sensible
         ``__ne__`` by default, so it *should* be enough to only implement
         ``__eq__`` in most cases).
 
         .. warning::
 
-           If you prevent ``attrs`` from creating the ordering methods for you
+           If you prevent *attrs* from creating the ordering methods for you
            (``order=False``, e.g. by implementing ``__le__``), it becomes
            *your* responsibility to make sure its ordering is sound. The best
            way is to use the `functools.total_ordering` decorator.
 
 
         Passing ``True`` or ``False`` to *init*, *repr*, *eq*, *order*,
         *cmp*, or *hash* overrides whatever *auto_detect* would determine.
 
     :param bool repr: Create a ``__repr__`` method with a human readable
-        representation of ``attrs`` attributes..
+        representation of *attrs* attributes..
     :param bool str: Create a ``__str__`` method that is identical to
         ``__repr__``.  This is usually not necessary except for
         `Exception`\ s.
     :param Optional[bool] eq: If ``True`` or ``None`` (default), add ``__eq__``
         and ``__ne__`` methods that check two instances for equality.
 
-        They compare the instances as if they were tuples of their ``attrs``
+        They compare the instances as if they were tuples of their *attrs*
         attributes if and only if the types of both classes are *identical*!
     :param Optional[bool] order: If ``True``, add ``__lt__``, ``__le__``,
         ``__gt__``, and ``__ge__`` methods that behave like *eq* above and
         allow instances to be ordered. If ``None`` (default) mirror value of
         *eq*.
     :param Optional[bool] cmp: Setting *cmp* is equivalent to setting *eq*
         and *order* to the same value. Must not be mixed with *eq* or *order*.
     :param Optional[bool] unsafe_hash: If ``None`` (default), the ``__hash__``
         method is generated according how *eq* and *frozen* are set.
 
-        1. If *both* are True, ``attrs`` will generate a ``__hash__`` for you.
+        1. If *both* are True, *attrs* will generate a ``__hash__`` for you.
         2. If *eq* is True and *frozen* is False, ``__hash__`` will be set to
            None, marking it unhashable (which it is).
         3. If *eq* is False, ``__hash__`` will be left untouched meaning the
            ``__hash__`` method of the base class will be used (if base class is
            ``object``, this means it will fall back to id-based hashing.).
 
         Although not recommended, you can decide for yourself and force
-        ``attrs`` to create one (e.g. if the class is immutable even though you
+        *attrs* to create one (e.g. if the class is immutable even though you
         didn't freeze it programmatically) by passing ``True`` or not.  Both of
         these cases are rather special and should be used carefully.
 
         See our documentation on `hashing`, Python's documentation on
         `object.__hash__`, and the `GitHub issue that led to the default \
         behavior <https://github.com/python-attrs/attrs/issues/136>`_ for more
         details.
     :param Optional[bool] hash: Alias for *unsafe_hash*. *unsafe_hash* takes
         precedence.
     :param bool init: Create a ``__init__`` method that initializes the
-        ``attrs`` attributes. Leading underscores are stripped for the argument
+        *attrs* attributes. Leading underscores are stripped for the argument
         name. If a ``__attrs_pre_init__`` method exists on the class, it will
         be called before the class is initialized. If a ``__attrs_post_init__``
         method exists on the class, it will be called after the class is fully
         initialized.
 
         If ``init`` is ``False``, an ``__attrs_init__`` method will be
         injected instead. This allows you to define a custom ``__init__``
@@ -1308,15 +1316,15 @@
         and then call ``__attrs_init__()`` and ``__attrs_post_init__()``.
     :param bool slots: Create a :term:`slotted class <slotted classes>` that's
         more memory-efficient. Slotted classes are generally superior to the
         default dict classes, but have some gotchas you should know about, so
         we encourage you to read the :term:`glossary entry <slotted classes>`.
     :param bool frozen: Make instances immutable after initialization.  If
         someone attempts to modify a frozen instance,
-        `attr.exceptions.FrozenInstanceError` is raised.
+        `attrs.exceptions.FrozenInstanceError` is raised.
 
         .. note::
 
             1. This is achieved by installing a custom ``__setattr__`` method
                on your class, so you can't implement your own.
 
             2. True immutability is impossible in Python.
@@ -1333,15 +1341,15 @@
             5. Subclasses of a frozen class are frozen too.
 
     :param bool weakref_slot: Make instances weak-referenceable.  This has no
         effect unless ``slots`` is also enabled.
     :param bool auto_attribs: If ``True``, collect :pep:`526`-annotated
         attributes from the class body.
 
-        In this case, you **must** annotate every field.  If ``attrs``
+        In this case, you **must** annotate every field.  If *attrs*
         encounters a field that is set to an `attr.ib` but lacks a type
         annotation, an `attr.exceptions.UnannotatedAttributeError` is
         raised.  Use ``field_name: typing.Any = attr.ib(...)`` if you don't
         want to set a type.
 
         If you assign a value to those attributes (e.g. ``x: int = 42``), that
         value becomes the default value like if it were passed using
@@ -1349,17 +1357,17 @@
         works as expected in most cases (see warning below).
 
         Attributes annotated as `typing.ClassVar`, and attributes that are
         neither annotated nor set to an `attr.ib` are **ignored**.
 
         .. warning::
            For features that use the attribute name to create decorators (e.g.
-           `validators <validators>`), you still *must* assign `attr.ib` to
-           them. Otherwise Python will either not find the name or try to use
-           the default value to call e.g. ``validator`` on it.
+           :ref:`validators <validators>`), you still *must* assign `attr.ib`
+           to them. Otherwise Python will either not find the name or try to
+           use the default value to call e.g. ``validator`` on it.
 
            These errors can be quite confusing and probably the most common bug
            report on our bug tracker.
 
     :param bool kw_only: Make all attributes keyword-only
         in the generated ``__init__`` (if ``init`` is ``False``, this
         parameter is ignored).
@@ -1372,22 +1380,22 @@
         the behavior of the object's hash code is undefined.
     :param bool auto_exc: If the class subclasses `BaseException`
         (which implicitly includes any subclass of any exception), the
         following happens to behave like a well-behaved Python exceptions
         class:
 
         - the values for *eq*, *order*, and *hash* are ignored and the
-          instances compare and hash by the instance's ids (N.B. ``attrs`` will
+          instances compare and hash by the instance's ids (N.B. *attrs* will
           *not* remove existing implementations of ``__hash__`` or the equality
           methods. It just won't add own ones.),
         - all attributes that are either passed into ``__init__`` or have a
           default value are additionally available as a tuple in the ``args``
           attribute,
         - the value of *str* is ignored leaving ``__str__`` to base classes.
-    :param bool collect_by_mro: Setting this to `True` fixes the way ``attrs``
+    :param bool collect_by_mro: Setting this to `True` fixes the way *attrs*
        collects attributes from base classes.  The default behavior is
        incorrect in certain cases of multiple inheritance.  It should be on by
        default but is kept off for backward-compatibility.
 
        See issue `#428 <https://github.com/python-attrs/attrs/issues/428>`_ for
        more details.
 
@@ -1418,15 +1426,15 @@
         If a list of callables is passed, they're automatically wrapped in an
         `attrs.setters.pipe`.
     :type on_setattr: `callable`, or a list of callables, or `None`, or
         `attrs.setters.NO_OP`
 
     :param Optional[callable] field_transformer:
         A function that is called with the original class object and all
-        fields right before ``attrs`` finalizes the class.  You can use
+        fields right before *attrs* finalizes the class.  You can use
         this, e.g., to automatically add converters or validators to
         fields based on their types.  See `transform-fields` for more details.
 
     :param bool match_args:
         If `True` (default), set ``__match_args__`` on the class to support
         :pep:`634` (Structural Pattern Matching). It is a tuple of all
         non-keyword-only ``__init__`` parameter names on Python 3.10 and later.
@@ -1896,47 +1904,61 @@
 
     cls.__repr__ = _make_repr(attrs, ns, cls)
     return cls
 
 
 def fields(cls):
     """
-    Return the tuple of ``attrs`` attributes for a class.
+    Return the tuple of *attrs* attributes for a class.
 
     The tuple also allows accessing the fields by their names (see below for
     examples).
 
     :param type cls: Class to introspect.
 
     :raise TypeError: If *cls* is not a class.
-    :raise attr.exceptions.NotAnAttrsClassError: If *cls* is not an ``attrs``
+    :raise attrs.exceptions.NotAnAttrsClassError: If *cls* is not an *attrs*
         class.
 
     :rtype: tuple (with name accessors) of `attrs.Attribute`
 
-    ..  versionchanged:: 16.2.0 Returned tuple allows accessing the fields
-        by name.
+    .. versionchanged:: 16.2.0 Returned tuple allows accessing the fields
+       by name.
+    .. versionchanged:: 23.1.0 Add support for generic classes.
     """
-    if not isinstance(cls, type):
+    generic_base = get_generic_base(cls)
+
+    if generic_base is None and not isinstance(cls, type):
         raise TypeError("Passed object must be a class.")
+
     attrs = getattr(cls, "__attrs_attrs__", None)
+
     if attrs is None:
+        if generic_base is not None:
+            attrs = getattr(generic_base, "__attrs_attrs__", None)
+            if attrs is not None:
+                # Even though this is global state, stick it on here to speed
+                # it up. We rely on `cls` being cached for this to be
+                # efficient.
+                cls.__attrs_attrs__ = attrs
+                return attrs
         raise NotAnAttrsClassError(f"{cls!r} is not an attrs-decorated class.")
+
     return attrs
 
 
 def fields_dict(cls):
     """
-    Return an ordered dictionary of ``attrs`` attributes for a class, whose
+    Return an ordered dictionary of *attrs* attributes for a class, whose
     keys are the attribute names.
 
     :param type cls: Class to introspect.
 
     :raise TypeError: If *cls* is not a class.
-    :raise attr.exceptions.NotAnAttrsClassError: If *cls* is not an ``attrs``
+    :raise attrs.exceptions.NotAnAttrsClassError: If *cls* is not an *attrs*
         class.
 
     :rtype: dict
 
     .. versionadded:: 18.1.0
     """
     if not isinstance(cls, type):
@@ -1949,15 +1971,15 @@
 
 def validate(inst):
     """
     Validate all attributes on *inst* that have a validator.
 
     Leaves all exceptions through.
 
-    :param inst: Instance of a class with ``attrs`` attributes.
+    :param inst: Instance of a class with *attrs* attributes.
     """
     if _config._run_validators is False:
         return
 
     for a in fields(inst.__class__):
         v = a.validator
         if v is not None:
@@ -2387,14 +2409,18 @@
     return name.lstrip("_")
 
 
 class Attribute:
     """
     *Read-only* representation of an attribute.
 
+    .. warning::
+
+       You should never instantiate this class yourself.
+
     The class has *all* arguments of `attr.ib` (except for ``factory``
     which is only syntactic sugar for ``default=Factory(...)`` plus the
     following:
 
     - ``name`` (`str`): The name of the attribute.
     - ``alias`` (`str`): The __init__ parameter name of the attribute, after
       any explicit overrides and default private-attribute-name handling.
@@ -2532,21 +2558,21 @@
             default=ca._default,
             type=type,
             cmp=None,
             inherited=False,
             **inst_dict,
         )
 
-    # Don't use attr.evolve since fields(Attribute) doesn't work
+    # Don't use attrs.evolve since fields(Attribute) doesn't work
     def evolve(self, **changes):
         """
         Copy *self* and apply *changes*.
 
-        This works similarly to `attr.evolve` but that function does not work
-        with ``Attribute``.
+        This works similarly to `attrs.evolve` but that function does not work
+        with `Attribute`.
 
         It is mainly meant to be used for `transform-fields`.
 
         .. versionadded:: 20.3.0
         """
         new = copy.copy(self)
 
@@ -2773,18 +2799,14 @@
 
     .. versionadded:: 17.1.0  *takes_self*
     """
 
     __slots__ = ("factory", "takes_self")
 
     def __init__(self, factory, takes_self=False):
-        """
-        `Factory` is part of the default machinery so if we want a default
-        value here, we have to implement it ourselves.
-        """
         self.factory = factory
         self.takes_self = takes_self
 
     def __getstate__(self):
         """
         Play nice with pickle.
         """
@@ -2814,21 +2836,21 @@
     for name in Factory.__slots__
 ]
 
 Factory = _add_hash(_add_eq(_add_repr(Factory, attrs=_f), attrs=_f), attrs=_f)
 
 
 def make_class(name, attrs, bases=(object,), **attributes_arguments):
-    """
+    r"""
     A quick way to create a new class called *name* with *attrs*.
 
     :param str name: The name for the new class.
 
     :param attrs: A list of names or a dictionary of mappings of names to
-        attributes.
+        `attr.ib`\ s / `attrs.field`\ s.
 
         The order is deduced from the order of the names or attributes inside
         *attrs*.  Otherwise the order of the definition of the attributes is
         used.
     :type attrs: `list` or `dict`
 
     :param tuple bases: Classes that the new class will subclass.
```

### Comparing `attrs-22.2.0/src/attr/_next_gen.py` & `attrs-23.1.0/src/attr/_next_gen.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     auto_detect=True,
     getstate_setstate=None,
     on_setattr=None,
     field_transformer=None,
     match_args=True,
 ):
     r"""
-    Define an ``attrs`` class.
+    Define an *attrs* class.
 
     Differences to the classic `attr.s` that it uses underneath:
 
     - Automatically detect whether or not *auto_attribs* should be `True` (c.f.
       *auto_attribs* parameter).
     - If *frozen* is `False`, run converters and validators when setting an
       attribute by default.
@@ -163,35 +163,41 @@
     *,
     default=NOTHING,
     validator=None,
     repr=True,
     hash=None,
     init=True,
     metadata=None,
+    type=None,
     converter=None,
     factory=None,
     kw_only=False,
     eq=None,
     order=None,
     on_setattr=None,
     alias=None,
 ):
     """
     Identical to `attr.ib`, except keyword-only and with some arguments
     removed.
 
+    .. versionadded:: 23.1.0
+       The *type* parameter has been re-added; mostly for
+       {func}`attrs.make_class`. Please note that type checkers ignore this
+       metadata.
     .. versionadded:: 20.1.0
     """
     return attrib(
         default=default,
         validator=validator,
         repr=repr,
         hash=hash,
         init=init,
         metadata=metadata,
+        type=type,
         converter=converter,
         factory=factory,
         kw_only=kw_only,
         eq=eq,
         order=order,
         on_setattr=on_setattr,
         alias=alias,
```

### Comparing `attrs-22.2.0/src/attr/_version_info.py` & `attrs-23.1.0/src/attr/_version_info.py`

 * *Files identical despite different names*

### Comparing `attrs-22.2.0/src/attr/converters.py` & `attrs-23.1.0/src/attr/converters.py`

 * *Files identical despite different names*

### Comparing `attrs-22.2.0/src/attr/exceptions.py` & `attrs-23.1.0/src/attr/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,59 +30,58 @@
 
     .. versionadded:: 20.1.0
     """
 
 
 class AttrsAttributeNotFoundError(ValueError):
     """
-    An ``attrs`` function couldn't find an attribute that the user asked for.
+    An *attrs* function couldn't find an attribute that the user asked for.
 
     .. versionadded:: 16.2.0
     """
 
 
 class NotAnAttrsClassError(ValueError):
     """
-    A non-``attrs`` class has been passed into an ``attrs`` function.
+    A non-*attrs* class has been passed into an *attrs* function.
 
     .. versionadded:: 16.2.0
     """
 
 
 class DefaultAlreadySetError(RuntimeError):
     """
-    A default has been set using ``attr.ib()`` and is attempted to be reset
+    A default has been set when defining the field and is attempted to be reset
     using the decorator.
 
     .. versionadded:: 17.1.0
     """
 
 
 class UnannotatedAttributeError(RuntimeError):
     """
-    A class with ``auto_attribs=True`` has an ``attr.ib()`` without a type
-    annotation.
+    A class with ``auto_attribs=True`` has a field without a type annotation.
 
     .. versionadded:: 17.3.0
     """
 
 
 class PythonTooOldError(RuntimeError):
     """
-    It was attempted to use an ``attrs`` feature that requires a newer Python
+    It was attempted to use an *attrs* feature that requires a newer Python
     version.
 
     .. versionadded:: 18.2.0
     """
 
 
 class NotCallableError(TypeError):
     """
-    A ``attr.ib()`` requiring a callable has been set with a value
-    that is not callable.
+    A field requiring a callable has been set with a value that is not
+    callable.
 
     .. versionadded:: 19.2.0
     """
 
     def __init__(self, msg, value):
         super(TypeError, self).__init__(msg, value)
         self.msg = msg
```

### Comparing `attrs-22.2.0/src/attr/exceptions.pyi` & `attrs-23.1.0/src/attr/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `attrs-22.2.0/src/attr/filters.py` & `attrs-23.1.0/src/attr/filters.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,43 +9,58 @@
 
 def _split_what(what):
     """
     Returns a tuple of `frozenset`s of classes and attributes.
     """
     return (
         frozenset(cls for cls in what if isinstance(cls, type)),
+        frozenset(cls for cls in what if isinstance(cls, str)),
         frozenset(cls for cls in what if isinstance(cls, Attribute)),
     )
 
 
 def include(*what):
     """
     Include *what*.
 
     :param what: What to include.
-    :type what: `list` of `type` or `attrs.Attribute`\\ s
+    :type what: `list` of classes `type`, field names `str` or
+        `attrs.Attribute`\\ s
 
     :rtype: `callable`
+
+    .. versionchanged:: 23.1.0 Accept strings with field names.
     """
-    cls, attrs = _split_what(what)
+    cls, names, attrs = _split_what(what)
 
     def include_(attribute, value):
-        return value.__class__ in cls or attribute in attrs
+        return (
+            value.__class__ in cls
+            or attribute.name in names
+            or attribute in attrs
+        )
 
     return include_
 
 
 def exclude(*what):
     """
     Exclude *what*.
 
     :param what: What to exclude.
-    :type what: `list` of classes or `attrs.Attribute`\\ s.
+    :type what: `list` of classes `type`, field names `str` or
+        `attrs.Attribute`\\ s.
 
     :rtype: `callable`
+
+    .. versionchanged:: 23.3.0 Accept field name string as input argument
     """
-    cls, attrs = _split_what(what)
+    cls, names, attrs = _split_what(what)
 
     def exclude_(attribute, value):
-        return value.__class__ not in cls and attribute not in attrs
+        return not (
+            value.__class__ in cls
+            or attribute.name in names
+            or attribute in attrs
+        )
 
     return exclude_
```

### Comparing `attrs-22.2.0/src/attr/setters.py` & `attrs-23.1.0/src/attr/setters.py`

 * *Files identical despite different names*

### Comparing `attrs-22.2.0/src/attr/setters.pyi` & `attrs-23.1.0/src/attr/setters.pyi`

 * *Files identical despite different names*

### Comparing `attrs-22.2.0/src/attr/validators.py` & `attrs-23.1.0/src/attr/validators.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,27 +5,22 @@
 """
 
 
 import operator
 import re
 
 from contextlib import contextmanager
+from re import Pattern
 
 from ._config import get_run_validators, set_run_validators
 from ._make import _AndValidator, and_, attrib, attrs
 from .converters import default_if_none
 from .exceptions import NotCallableError
 
 
-try:
-    Pattern = re.Pattern
-except AttributeError:  # Python <3.7 lacks a Pattern type.
-    Pattern = type(re.compile(""))
-
-
 __all__ = [
     "and_",
     "deep_iterable",
     "deep_mapping",
     "disabled",
     "ge",
     "get_disabled",
@@ -245,15 +240,25 @@
 
     :param interface: The interface to check for.
     :type interface: ``zope.interface.Interface``
 
     :raises TypeError: With a human readable error message, the attribute
         (of type `attrs.Attribute`), the expected interface, and the
         value it got.
+
+    .. deprecated:: 23.1.0
     """
+    import warnings
+
+    warnings.warn(
+        "attrs's zope-interface support is deprecated and will be removed in, "
+        "or after, April 2024.",
+        DeprecationWarning,
+        stacklevel=2,
+    )
     return _ProvidesValidator(interface)
 
 
 @attrs(repr=False, slots=True, hash=True)
 class _OptionalValidator:
     validator = attrib()
 
@@ -271,23 +276,24 @@
 
 def optional(validator):
     """
     A validator that makes an attribute optional.  An optional attribute is one
     which can be set to ``None`` in addition to satisfying the requirements of
     the sub-validator.
 
-    :param validator: A validator (or a list of validators) that is used for
-        non-``None`` values.
-    :type validator: callable or `list` of callables.
+    :param Callable | tuple[Callable] | list[Callable] validator: A validator
+        (or validators) that is used for non-``None`` values.
 
     .. versionadded:: 15.1.0
     .. versionchanged:: 17.1.0 *validator* can be a list of validators.
+    .. versionchanged:: 23.1.0 *validator* can also be a tuple of validators.
     """
-    if isinstance(validator, list):
+    if isinstance(validator, (list, tuple)):
         return _OptionalValidator(_AndValidator(validator))
+
     return _OptionalValidator(validator)
 
 
 @attrs(repr=False, slots=True, hash=True)
 class _InValidator:
     options = attrib()
 
@@ -355,21 +361,21 @@
 
     def __repr__(self):
         return "<is_callable validator>"
 
 
 def is_callable():
     """
-    A validator that raises a `attr.exceptions.NotCallableError` if the
+    A validator that raises a `attrs.exceptions.NotCallableError` if the
     initializer is called with a value for this particular attribute
     that is not callable.
 
     .. versionadded:: 19.1.0
 
-    :raises `attr.exceptions.NotCallableError`: With a human readable error
+    :raises attrs.exceptions.NotCallableError: With a human readable error
         message containing the attribute (`attrs.Attribute`) name,
         and the value it got.
     """
     return _IsCallableValidator()
 
 
 @attrs(repr=False, slots=True, hash=True)
```

### Comparing `attrs-22.2.0/src/attr/validators.pyi` & `attrs-23.1.0/src/attr/validators.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,17 @@
 def instance_of(
     type: Tuple[Type[_T1], Type[_T2], Type[_T3]]
 ) -> _ValidatorType[Union[_T1, _T2, _T3]]: ...
 @overload
 def instance_of(type: Tuple[type, ...]) -> _ValidatorType[Any]: ...
 def provides(interface: Any) -> _ValidatorType[Any]: ...
 def optional(
-    validator: Union[_ValidatorType[_T], List[_ValidatorType[_T]]]
+    validator: Union[
+        _ValidatorType[_T], List[_ValidatorType[_T]], Tuple[_ValidatorType[_T]]
+    ]
 ) -> _ValidatorType[Optional[_T]]: ...
 def in_(options: Container[_T]) -> _ValidatorType[_T]: ...
 def and_(*validators: _ValidatorType[_T]) -> _ValidatorType[_T]: ...
 def matches_re(
     regex: Union[Pattern[AnyStr], AnyStr],
     flags: int = ...,
     func: Optional[
@@ -78,9 +80,9 @@
 def gt(val: _T) -> _ValidatorType[_T]: ...
 def max_len(length: int) -> _ValidatorType[_T]: ...
 def min_len(length: int) -> _ValidatorType[_T]: ...
 def not_(
     validator: _ValidatorType[_T],
     *,
     msg: Optional[str] = None,
-    exc_types: Union[Type[Exception], Iterable[Type[Exception]]] = ...
+    exc_types: Union[Type[Exception], Iterable[Type[Exception]]] = ...,
 ) -> _ValidatorType[_T]: ...
```

### Comparing `attrs-22.2.0/src/attrs/__init__.pyi` & `attrs-23.1.0/src/attrs/__init__.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -42,26 +42,26 @@
 from attr import resolve_types as resolve_types
 from attr import setters as setters
 from attr import validate as validate
 from attr import validators as validators
 
 # TODO: see definition of attr.asdict/astuple
 def asdict(
-    inst: Any,
+    inst: AttrsInstance,
     recurse: bool = ...,
     filter: Optional[_FilterType[Any]] = ...,
     dict_factory: Type[Mapping[Any, Any]] = ...,
     retain_collection_types: bool = ...,
     value_serializer: Optional[
         Callable[[type, Attribute[Any], Any], Any]
     ] = ...,
     tuple_keys: bool = ...,
 ) -> Dict[str, Any]: ...
 
 # TODO: add support for returning NamedTuple from the mypy plugin
 def astuple(
-    inst: Any,
+    inst: AttrsInstance,
     recurse: bool = ...,
     filter: Optional[_FilterType[Any]] = ...,
     tuple_factory: Type[Sequence[Any]] = ...,
     retain_collection_types: bool = ...,
 ) -> Tuple[Any, ...]: ...
```

### Comparing `attrs-22.2.0/tests/dataclass_transform_example.py` & `attrs-23.1.0/tests/dataclass_transform_example.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,27 +18,25 @@
     # mypy plugin adapts the "int" method signature, pyright does not
     with_converter: int = attr.field(converter=int)
 
 
 reveal_type(DefineConverter.__init__)  # noqa
 
 
-# mypy plugin supports attr.frozen, pyright does not
 @attr.frozen()
 class Frozen:
     a: str
 
 
 d = Frozen("a")
 d.a = "new"
 
 reveal_type(d.a)  # noqa
 
 
-# but pyright supports attr.define(frozen)
 @attr.define(frozen=True)
 class FrozenDefine:
     a: str
 
 
 d2 = FrozenDefine("a")
 d2.a = "new"
```

### Comparing `attrs-22.2.0/tests/strategies.py` & `attrs-23.1.0/tests/strategies.py`

 * *Files identical despite different names*

### Comparing `attrs-22.2.0/tests/test_3rd_party.py` & `attrs-23.1.0/tests/test_3rd_party.py`

 * *Files identical despite different names*

### Comparing `attrs-22.2.0/tests/test_abc.py` & `attrs-23.1.0/tests/test_abc.py`

 * *Files identical despite different names*

### Comparing `attrs-22.2.0/tests/test_annotations.py` & `attrs-23.1.0/tests/test_annotations.py`

 * *Files 2% similar despite different names*

```diff
@@ -512,14 +512,42 @@
 
         attr.resolve_types(C)
 
         assert int is attr.fields(C).x.type
         assert str is attr.fields(C).y.type
         assert None is attr.fields(C).z.type
 
+    @pytest.mark.skipif(
+        sys.version_info[:2] < (3, 9),
+        reason="Incompatible behavior on older Pythons",
+    )
+    def test_extra_resolve(self):
+        """
+        `get_type_hints` returns extra type hints.
+        """
+        from typing import Annotated
+
+        globals = {"Annotated": Annotated}
+
+        @attr.define
+        class C:
+            x: 'Annotated[float, "test"]'
+
+        attr.resolve_types(C, globals)
+
+        assert attr.fields(C).x.type == Annotated[float, "test"]
+
+        @attr.define
+        class D:
+            x: 'Annotated[float, "test"]'
+
+        attr.resolve_types(D, globals, include_extras=False)
+
+        assert attr.fields(D).x.type == float
+
     def test_resolve_types_auto_attrib(self, slots):
         """
         Types can be resolved even when strings are involved.
         """
 
         @attr.s(slots=slots, auto_attribs=True)
         class A:
```

### Comparing `attrs-22.2.0/tests/test_cmp.py` & `attrs-23.1.0/tests/test_cmp.py`

 * *Files identical despite different names*

### Comparing `attrs-22.2.0/tests/test_compat.py` & `attrs-23.1.0/tests/test_compat.py`

 * *Files identical despite different names*

### Comparing `attrs-22.2.0/tests/test_config.py` & `attrs-23.1.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `attrs-22.2.0/tests/test_converters.py` & `attrs-23.1.0/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `attrs-22.2.0/tests/test_dunders.py` & `attrs-23.1.0/tests/test_dunders.py`

 * *Files identical despite different names*

### Comparing `attrs-22.2.0/tests/test_filters.py` & `attrs-23.1.0/tests/test_filters.py`

 * *Files 15% similar despite different names*

```diff
@@ -26,30 +26,35 @@
 
     def test_splits(self):
         """
         Splits correctly.
         """
         assert (
             frozenset((int, str)),
+            frozenset(("abcd", "123")),
             frozenset((fields(C).a,)),
-        ) == _split_what((str, fields(C).a, int))
+        ) == _split_what((str, "123", fields(C).a, int, "abcd"))
 
 
 class TestInclude:
     """
     Tests for `include`.
     """
 
     @pytest.mark.parametrize(
         "incl,value",
         [
             ((int,), 42),
             ((str,), "hello"),
             ((str, fields(C).a), 42),
             ((str, fields(C).b), "hello"),
+            (("a",), 42),
+            (("a",), "hello"),
+            (("a", str), 42),
+            (("a", fields(C).b), "hello"),
         ],
     )
     def test_allow(self, incl, value):
         """
         Return True if a class or attribute is included.
         """
         i = include(*incl)
@@ -58,14 +63,18 @@
     @pytest.mark.parametrize(
         "incl,value",
         [
             ((str,), 42),
             ((int,), "hello"),
             ((str, fields(C).b), 42),
             ((int, fields(C).b), "hello"),
+            (("b",), 42),
+            (("b",), "hello"),
+            (("b", str), 42),
+            (("b", fields(C).b), "hello"),
         ],
     )
     def test_drop_class(self, incl, value):
         """
         Return False on non-included classes and attributes.
         """
         i = include(*incl)
@@ -80,14 +89,18 @@
     @pytest.mark.parametrize(
         "excl,value",
         [
             ((str,), 42),
             ((int,), "hello"),
             ((str, fields(C).b), 42),
             ((int, fields(C).b), "hello"),
+            (("b",), 42),
+            (("b",), "hello"),
+            (("b", str), 42),
+            (("b", fields(C).b), "hello"),
         ],
     )
     def test_allow(self, excl, value):
         """
         Return True if class or attribute is not excluded.
         """
         e = exclude(*excl)
@@ -96,14 +109,18 @@
     @pytest.mark.parametrize(
         "excl,value",
         [
             ((int,), 42),
             ((str,), "hello"),
             ((str, fields(C).a), 42),
             ((str, fields(C).b), "hello"),
+            (("a",), 42),
+            (("a",), "hello"),
+            (("a", str), 42),
+            (("a", fields(C).b), "hello"),
         ],
     )
     def test_drop_class(self, excl, value):
         """
         Return True on non-excluded classes and attributes.
         """
         e = exclude(*excl)
```

### Comparing `attrs-22.2.0/tests/test_funcs.py` & `attrs-23.1.0/tests/test_funcs.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
 Tests for `attr._funcs`.
 """
 
 
 from collections import OrderedDict
+from typing import Generic, TypeVar
 
 import pytest
 
 from hypothesis import assume, given
 from hypothesis import strategies as st
 
 import attr
@@ -414,14 +415,45 @@
 
     def test_negative(self):
         """
         Returns `False` on non-decorated classes.
         """
         assert not has(object)
 
+    def test_generics(self):
+        """
+        Works with generic classes.
+        """
+        T = TypeVar("T")
+
+        @attr.define
+        class A(Generic[T]):
+            a: T
+
+        assert has(A)
+
+        assert has(A[str])
+        # Verify twice, since there's caching going on.
+        assert has(A[str])
+
+    def test_generics_negative(self):
+        """
+        Returns `False` on non-decorated generic classes.
+        """
+        T = TypeVar("T")
+
+        class A(Generic[T]):
+            a: T
+
+        assert not has(A)
+
+        assert not has(A[str])
+        # Verify twice, since there's caching going on.
+        assert not has(A[str])
+
 
 class TestAssoc:
     """
     Tests for `assoc`.
     """
 
     @given(slots=st.booleans(), frozen=st.booleans())
@@ -431,28 +463,26 @@
         """
 
         @attr.s(slots=slots, frozen=frozen)
         class C:
             pass
 
         i1 = C()
-        with pytest.deprecated_call():
-            i2 = assoc(i1)
+        i2 = assoc(i1)
 
         assert i1 is not i2
         assert i1 == i2
 
     @given(simple_classes())
     def test_no_changes(self, C):
         """
         No changes means a verbatim copy.
         """
         i1 = C()
-        with pytest.deprecated_call():
-            i2 = assoc(i1)
+        i2 = assoc(i1)
 
         assert i1 is not i2
         assert i1 == i2
 
     @given(simple_classes(), st.data())
     def test_change(self, C, data):
         """
@@ -461,16 +491,15 @@
         # Take the first attribute, and change it.
         assume(fields(C))  # Skip classes with no attributes.
         field_names = [a.name for a in fields(C)]
         original = C()
         chosen_names = data.draw(st.sets(st.sampled_from(field_names)))
         change_dict = {name: data.draw(st.integers()) for name in chosen_names}
 
-        with pytest.deprecated_call():
-            changed = assoc(original, **change_dict)
+        changed = assoc(original, **change_dict)
 
         for k, v in change_dict.items():
             assert getattr(changed, k) == v
 
     @given(simple_classes())
     def test_unknown(self, C):
         """
@@ -491,30 +520,15 @@
         """
 
         @attr.s(frozen=True)
         class C:
             x = attr.ib()
             y = attr.ib()
 
-        with pytest.deprecated_call():
-            assert C(3, 2) == assoc(C(1, 2), x=3)
-
-    def test_warning(self):
-        """
-        DeprecationWarning points to the correct file.
-        """
-
-        @attr.s
-        class C:
-            x = attr.ib()
-
-        with pytest.warns(DeprecationWarning) as wi:
-            assert C(2) == assoc(C(1), x=2)
-
-        assert __file__ == wi.list[0].filename
+        assert C(3, 2) == assoc(C(1, 2), x=3)
 
 
 class TestEvolve:
     """
     Tests for `evolve`.
     """
 
@@ -671,7 +685,51 @@
         obj2b = {"foo": 42, "param2": 42}
 
         obj1a = Cls1(param1=obj2a)
 
         assert Cls1({"foo": 42, "param2": 42}) == attr.evolve(
             obj1a, param1=obj2b
         )
+
+    def test_inst_kw(self):
+        """
+        If `inst` is passed per kw argument, a warning is raised.
+        See #1109
+        """
+
+        @attr.s
+        class C:
+            pass
+
+        with pytest.warns(DeprecationWarning) as wi:
+            evolve(inst=C())
+
+        assert __file__ == wi.list[0].filename
+
+    def test_no_inst(self):
+        """
+        Missing inst argument raises a TypeError like Python would.
+        """
+        with pytest.raises(TypeError, match=r"evolve\(\) missing 1"):
+            evolve(x=1)
+
+    def test_too_many_pos_args(self):
+        """
+        More than one positional argument raises a TypeError like Python would.
+        """
+        with pytest.raises(
+            TypeError,
+            match=r"evolve\(\) takes 1 positional argument, but 2 were given",
+        ):
+            evolve(1, 2)
+
+    def test_can_change_inst(self):
+        """
+        If the instance is passed by positional argument, a field named `inst`
+        can be changed.
+        """
+
+        @attr.define
+        class C:
+            inst: int
+
+        assert C(42) == evolve(C(23), inst=42)
```

### Comparing `attrs-22.2.0/tests/test_functional.py` & `attrs-23.1.0/tests/test_functional.py`

 * *Files identical despite different names*

### Comparing `attrs-22.2.0/tests/test_hooks.py` & `attrs-23.1.0/tests/test_hooks.py`

 * *Files identical despite different names*

### Comparing `attrs-22.2.0/tests/test_init_subclass.py` & `attrs-23.1.0/tests/test_init_subclass.py`

 * *Files identical despite different names*

### Comparing `attrs-22.2.0/tests/test_make.py` & `attrs-23.1.0/tests/test_make.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import functools
 import gc
 import inspect
 import itertools
 import sys
 
 from operator import attrgetter
+from typing import Generic, TypeVar
 
 import pytest
 
 from hypothesis import assume, given
 from hypothesis.strategies import booleans, integers, lists, sampled_from, text
 
 import attr
@@ -397,15 +398,14 @@
         Attributes and methods are looked up the same way.
 
         See #428
         """
 
         @attr.s(collect_by_mro=True)
         class A:
-
             x = attr.ib(10)
 
             def xx(self):
                 return 10
 
         @attr.s(collect_by_mro=True)
         class B(A):
@@ -1102,23 +1102,39 @@
         with pytest.raises(TypeError) as e:
             fields(C())
 
         assert "Passed object must be a class." == e.value.args[0]
 
     def test_handler_non_attrs_class(self):
         """
-        Raises `ValueError` if passed a non-``attrs`` instance.
+        Raises `ValueError` if passed a non-*attrs* instance.
         """
         with pytest.raises(NotAnAttrsClassError) as e:
             fields(object)
 
         assert (
             f"{object!r} is not an attrs-decorated class."
         ) == e.value.args[0]
 
+    def test_handler_non_attrs_generic_class(self):
+        """
+        Raises `ValueError` if passed a non-*attrs* generic class.
+        """
+        T = TypeVar("T")
+
+        class B(Generic[T]):
+            pass
+
+        with pytest.raises(NotAnAttrsClassError) as e:
+            fields(B[str])
+
+        assert (
+            f"{B[str]!r} is not an attrs-decorated class."
+        ) == e.value.args[0]
+
     @given(simple_classes())
     def test_fields(self, C):
         """
         Returns a list of `Attribute`a.
         """
         assert all(isinstance(a, Attribute) for a in fields(C))
 
@@ -1126,14 +1142,32 @@
     def test_fields_properties(self, C):
         """
         Fields returns a tuple with properties.
         """
         for attribute in fields(C):
             assert getattr(fields(C), attribute.name) is attribute
 
+    def test_generics(self):
+        """
+        Fields work with generic classes.
+        """
+        T = TypeVar("T")
+
+        @attr.define
+        class A(Generic[T]):
+            a: T
+
+        assert len(fields(A)) == 1
+        assert fields(A).a.name == "a"
+        assert fields(A).a.default is attr.NOTHING
+
+        assert len(fields(A[str])) == 1
+        assert fields(A[str]).a.name == "a"
+        assert fields(A[str]).a.default is attr.NOTHING
+
 
 class TestFieldsDict:
     """
     Tests for `fields_dict`.
     """
 
     @given(simple_classes())
@@ -1144,15 +1178,15 @@
         with pytest.raises(TypeError) as e:
             fields_dict(C())
 
         assert "Passed object must be a class." == e.value.args[0]
 
     def test_handler_non_attrs_class(self):
         """
-        Raises `ValueError` if passed a non-``attrs`` instance.
+        Raises `ValueError` if passed a non-*attrs* instance.
         """
         with pytest.raises(NotAnAttrsClassError) as e:
             fields_dict(object)
 
         assert (
             f"{object!r} is not an attrs-decorated class."
         ) == e.value.args[0]
```

### Comparing `attrs-22.2.0/tests/test_mypy.yml` & `attrs-23.1.0/tests/test_mypy.yml`

 * *Files 16% similar despite different names*

```diff
@@ -3,28 +3,28 @@
     - val: "a = attr.ib(type=int)"
     - val: "a: int = attr.ib()"
   main: |
     import attr
     @attr.s
     class C:
         {{ val }}
-    C()  # E: Missing positional argument "a" in call to "C"
+    C()  # E: Missing positional argument "a" in call to "C"  [call-arg]
     C(1)
     C(a=1)
-    C(a="hi")  # E: Argument "a" to "C" has incompatible type "str"; expected "int"
+    C(a="hi")  # E: Argument "a" to "C" has incompatible type "str"; expected "int"  [arg-type]
 - case: attr_s_with_type_annotations
   main: |
     import attr
     @attr.s
     class C:
       a: int = attr.ib()
-    C()  # E: Missing positional argument "a" in call to "C"
+    C()  # E: Missing positional argument "a" in call to "C"  [call-arg]
     C(1)
     C(a=1)
-    C(a="hi")  # E: Argument "a" to "C" has incompatible type "str"; expected "int"
+    C(a="hi")  # E: Argument "a" to "C" has incompatible type "str"; expected "int"  [arg-type]
 
 - case: testAttrsSimple
   main: |
     import attr
     @attr.s
     class A:
         a = attr.ib()
@@ -35,15 +35,15 @@
 
         def foo(self):
             return self.a
     reveal_type(A)  # N: Revealed type is "def (a: Any, b: Any, c: Any =, d: Any =) -> main.A"
     A(1, [2])
     A(1, [2], '3', 4)
     A(1, 2, 3, 4)
-    A(1, [2], '3', 4, 5)  # E: Too many arguments for "A"
+    A(1, [2], '3', 4, 5)  # E: Too many arguments for "A"  [call-arg]
 
 - case: testAttrsAnnotated
   main: |
     import attr
     from typing import List, ClassVar
     @attr.s
     class A:
@@ -52,16 +52,16 @@
         c: str = attr.ib('18')
         _d: int = attr.ib(validator=None, default=18)
         E = 7
         F: ClassVar[int] = 22
     reveal_type(A)  # N: Revealed type is "def (a: builtins.int, b: builtins.list[builtins.int], c: builtins.str =, d: builtins.int =) -> main.A"
     A(1, [2])
     A(1, [2], '3', 4)
-    A(1, 2, 3, 4)  # E: Argument 2 to "A" has incompatible type "int"; expected "List[int]" # E: Argument 3 to "A" has incompatible type "int"; expected "str"
-    A(1, [2], '3', 4, 5)  # E: Too many arguments for "A"
+    A(1, 2, 3, 4)  # E: Argument 2 to "A" has incompatible type "int"; expected "List[int]"  [arg-type] # E: Argument 3 to "A" has incompatible type "int"; expected "str"  [arg-type]
+    A(1, [2], '3', 4, 5)  # E: Too many arguments for "A"  [call-arg]
 
 - case: testAttrsPython2Annotations
   main: |
     import attr
     from typing import List, ClassVar
     @attr.s
     class A:
@@ -70,16 +70,16 @@
         c = attr.ib('18') # type: str
         _d = attr.ib(validator=None, default=18) # type: int
         E = 7
         F: ClassVar[int] = 22
     reveal_type(A)  # N: Revealed type is "def (a: builtins.int, b: builtins.list[builtins.int], c: builtins.str =, d: builtins.int =) -> main.A"
     A(1, [2])
     A(1, [2], '3', 4)
-    A(1, 2, 3, 4)  # E: Argument 2 to "A" has incompatible type "int"; expected "List[int]" # E: Argument 3 to "A" has incompatible type "int"; expected "str"
-    A(1, [2], '3', 4, 5)  # E: Too many arguments for "A"
+    A(1, 2, 3, 4)  # E: Argument 2 to "A" has incompatible type "int"; expected "List[int]"  [arg-type] # E: Argument 3 to "A" has incompatible type "int"; expected "str"  [arg-type]
+    A(1, [2], '3', 4, 5)  # E: Too many arguments for "A"  [call-arg]
 
 - case: testAttrsAutoAttribs
   main: |
     import attr
     from typing import List, ClassVar
     @attr.s(auto_attribs=True)
     class A:
@@ -88,53 +88,53 @@
         c: str = '18'
         _d: int = attr.ib(validator=None, default=18)
         E = 7
         F: ClassVar[int] = 22
     reveal_type(A)  # N: Revealed type is "def (a: builtins.int, b: builtins.list[builtins.int], c: builtins.str =, d: builtins.int =) -> main.A"
     A(1, [2])
     A(1, [2], '3', 4)
-    A(1, 2, 3, 4)  # E: Argument 2 to "A" has incompatible type "int"; expected "List[int]" # E: Argument 3 to "A" has incompatible type "int"; expected "str"
-    A(1, [2], '3', 4, 5)  # E: Too many arguments for "A"
+    A(1, 2, 3, 4)  # E: Argument 2 to "A" has incompatible type "int"; expected "List[int]"  [arg-type] # E: Argument 3 to "A" has incompatible type "int"; expected "str"  [arg-type]
+    A(1, [2], '3', 4, 5)  # E: Too many arguments for "A"  [call-arg]
 
 - case: testAttrsUntypedNoUntypedDefs
   mypy_config: |
     disallow_untyped_defs = True
   main: |
     import attr
     @attr.s
     class A:
-        a = attr.ib()  # E: Need type annotation for "a"
-        _b = attr.ib()  # E: Need type annotation for "_b"
-        c = attr.ib(18)  # E: Need type annotation for "c"
-        _d = attr.ib(validator=None, default=18)   # E: Need type annotation for "_d"
+        a = attr.ib()  # E: Need type annotation for "a"  [var-annotated]
+        _b = attr.ib()  # E: Need type annotation for "_b"  [var-annotated]
+        c = attr.ib(18)  # E: Need type annotation for "c"  [var-annotated]
+        _d = attr.ib(validator=None, default=18)   # E: Need type annotation for "_d"  [var-annotated]
         E = 18
 
 - case: testAttrsWrongReturnValue
   main: |
     import attr
     @attr.s
     class A:
         x: int = attr.ib(8)
         def foo(self) -> str:
-            return self.x  # E: Incompatible return value type (got "int", expected "str")
+            return self.x  # E: Incompatible return value type (got "int", expected "str")  [return-value]
     @attr.s
     class B:
         x = attr.ib(8)  # type: int
         def foo(self) -> str:
-            return self.x  # E: Incompatible return value type (got "int", expected "str")
+            return self.x  # E: Incompatible return value type (got "int", expected "str")  [return-value]
     @attr.dataclass
     class C:
         x: int = 8
         def foo(self) -> str:
-            return self.x  # E: Incompatible return value type (got "int", expected "str")
+            return self.x  # E: Incompatible return value type (got "int", expected "str")  [return-value]
     @attr.s
     class D:
         x = attr.ib(8, type=int)
         def foo(self) -> str:
-            return self.x  # E: Incompatible return value type (got "int", expected "str")
+            return self.x  # E: Incompatible return value type (got "int", expected "str")  [return-value]
 
 - case: testAttrsSeriousNames
   main: |
     from attr import attrib, attrs
     from typing import List
     @attrs(init=True)
     class A:
@@ -142,62 +142,62 @@
         _b: List[int] = attrib()
         c = attrib(18)
         _d = attrib(validator=None, default=18)
         CLASS_VAR = 18
     reveal_type(A)  # N: Revealed type is "def (a: Any, b: builtins.list[builtins.int], c: Any =, d: Any =) -> main.A"
     A(1, [2])
     A(1, [2], '3', 4)
-    A(1, 2, 3, 4)  # E: Argument 2 to "A" has incompatible type "int"; expected "List[int]"
-    A(1, [2], '3', 4, 5)  # E: Too many arguments for "A"
+    A(1, 2, 3, 4)  # E: Argument 2 to "A" has incompatible type "int"; expected "List[int]"  [arg-type]
+    A(1, [2], '3', 4, 5)  # E: Too many arguments for "A"  [call-arg]
 
 - case: testAttrsDefaultErrors
   main: |
     import attr
     @attr.s
     class A:
         x = attr.ib(default=17)
-        y = attr.ib()  # E: Non-default attributes not allowed after default attributes.
+        y = attr.ib()  # E: Non-default attributes not allowed after default attributes.  [misc]
     @attr.s(auto_attribs=True)
     class B:
         x: int = 17
-        y: int # E: Non-default attributes not allowed after default attributes.
+        y: int # E: Non-default attributes not allowed after default attributes.  [misc]
     @attr.s(auto_attribs=True)
     class C:
         x: int = attr.ib(default=17)
-        y: int # E: Non-default attributes not allowed after default attributes.
+        y: int # E: Non-default attributes not allowed after default attributes.  [misc]
     @attr.s
     class D:
         x = attr.ib()
-        y = attr.ib() # E: Non-default attributes not allowed after default attributes.
+        y = attr.ib() # E: Non-default attributes not allowed after default attributes.  [misc]
 
         @x.default
         def foo(self):
             return 17
 
 - case: testAttrsNotBooleans
   main: |
     import attr
     x = True
-    @attr.s(cmp=x)  # E: "cmp" argument must be True or False.
+    @attr.s(cmp=x)  # E: "cmp" argument must be a True, False, or None literal  [literal-required]
     class A:
-        a = attr.ib(init=x)  # E: "init" argument must be True or False.
+        a = attr.ib(init=x)  # E: "init" argument must be a True or False literal  [literal-required]
 
 - case: testAttrsInitFalse
   main: |
     from attr import attrib, attrs
     @attrs(auto_attribs=True, init=False)
     class A:
         a: int
         _b: int
         c: int = 18
         _d: int = attrib(validator=None, default=18)
     reveal_type(A)  # N: Revealed type is "def () -> main.A"
     A()
-    A(1, [2])  # E: Too many arguments for "A"
-    A(1, [2], '3', 4)  # E: Too many arguments for "A"
+    A(1, [2])  # E: Too many arguments for "A"  [call-arg]
+    A(1, [2], '3', 4)  # E: Too many arguments for "A"  [call-arg]
 
 - case: testAttrsInitAttribFalse
   main: |
     from attr import attrib, attrs
     @attrs
     class A:
         a = attrib(init=False)
@@ -219,104 +219,104 @@
     A(1) < A(2)
     A(1) <= A(2)
     A(1) > A(2)
     A(1) >= A(2)
     A(1) == A(2)
     A(1) != A(2)
 
-    A(1) < 1  # E: Unsupported operand types for < ("A" and "int")
-    A(1) <= 1  # E: Unsupported operand types for <= ("A" and "int")
-    A(1) > 1  # E: Unsupported operand types for > ("A" and "int")
-    A(1) >= 1  # E: Unsupported operand types for >= ("A" and "int")
+    A(1) < 1  # E: Unsupported operand types for < ("A" and "int")  [operator]
+    A(1) <= 1  # E: Unsupported operand types for <= ("A" and "int")  [operator]
+    A(1) > 1  # E: Unsupported operand types for > ("A" and "int")  [operator]
+    A(1) >= 1  # E: Unsupported operand types for >= ("A" and "int")  [operator]
     A(1) == 1
     A(1) != 1
 
-    1 < A(1)  # E: Unsupported operand types for < ("int" and "A")
-    1 <= A(1)  # E: Unsupported operand types for <= ("int" and "A")
-    1 > A(1)  # E: Unsupported operand types for > ("int" and "A")
-    1 >= A(1)  # E: Unsupported operand types for >= ("int" and "A")
+    1 < A(1)  # E: Unsupported operand types for < ("int" and "A")  [operator]
+    1 <= A(1)  # E: Unsupported operand types for <= ("int" and "A")  [operator]
+    1 > A(1)  # E: Unsupported operand types for > ("int" and "A")  [operator]
+    1 >= A(1)  # E: Unsupported operand types for >= ("int" and "A")  [operator]
     1 == A(1)
     1 != A(1)
 
 - case: testAttrsEqFalse
   main: |
     from attr import attrib, attrs
     @attrs(auto_attribs=True, eq=False)
     class A:
         a: int
     reveal_type(A)  # N: Revealed type is "def (a: builtins.int) -> main.A"
     reveal_type(A.__eq__)  # N: Revealed type is "def (builtins.object, builtins.object) -> builtins.bool"
     reveal_type(A.__ne__)  # N: Revealed type is "def (builtins.object, builtins.object) -> builtins.bool"
 
-    A(1) < A(2)  # E: Unsupported left operand type for < ("A")
-    A(1) <= A(2)  # E: Unsupported left operand type for <= ("A")
-    A(1) > A(2)  # E: Unsupported left operand type for > ("A")
-    A(1) >= A(2)  # E: Unsupported left operand type for >= ("A")
+    A(1) < A(2)  # E: Unsupported left operand type for < ("A")  [operator]
+    A(1) <= A(2)  # E: Unsupported left operand type for <= ("A")  [operator]
+    A(1) > A(2)  # E: Unsupported left operand type for > ("A")  [operator]
+    A(1) >= A(2)  # E: Unsupported left operand type for >= ("A")  [operator]
     A(1) == A(2)
     A(1) != A(2)
 
-    A(1) < 1  # E: Unsupported operand types for > ("int" and "A")
-    A(1) <= 1  # E: Unsupported operand types for >= ("int" and "A")
-    A(1) > 1  # E: Unsupported operand types for < ("int" and "A")
-    A(1) >= 1  # E: Unsupported operand types for <= ("int" and "A")
+    A(1) < 1  # E: Unsupported operand types for > ("int" and "A")  [operator]
+    A(1) <= 1  # E: Unsupported operand types for >= ("int" and "A")  [operator]
+    A(1) > 1  # E: Unsupported operand types for < ("int" and "A")  [operator]
+    A(1) >= 1  # E: Unsupported operand types for <= ("int" and "A")  [operator]
     A(1) == 1
     A(1) != 1
 
-    1 < A(1)  # E: Unsupported operand types for < ("int" and "A")
-    1 <= A(1)  # E: Unsupported operand types for <= ("int" and "A")
-    1 > A(1)  # E: Unsupported operand types for > ("int" and "A")
-    1 >= A(1)  # E: Unsupported operand types for >= ("int" and "A")
+    1 < A(1)  # E: Unsupported operand types for < ("int" and "A")  [operator]
+    1 <= A(1)  # E: Unsupported operand types for <= ("int" and "A")  [operator]
+    1 > A(1)  # E: Unsupported operand types for > ("int" and "A")  [operator]
+    1 >= A(1)  # E: Unsupported operand types for >= ("int" and "A")  [operator]
     1 == A(1)
     1 != A(1)
 
 - case: testAttrsOrderFalse
   main: |
     from attr import attrib, attrs
     @attrs(auto_attribs=True, order=False)
     class A:
         a: int
     reveal_type(A)  # N: Revealed type is "def (a: builtins.int) -> main.A"
 
-    A(1) < A(2)  # E: Unsupported left operand type for < ("A")
-    A(1) <= A(2)  # E: Unsupported left operand type for <= ("A")
-    A(1) > A(2)  # E: Unsupported left operand type for > ("A")
-    A(1) >= A(2)  # E: Unsupported left operand type for >= ("A")
+    A(1) < A(2)  # E: Unsupported left operand type for < ("A")  [operator]
+    A(1) <= A(2)  # E: Unsupported left operand type for <= ("A")  [operator]
+    A(1) > A(2)  # E: Unsupported left operand type for > ("A")  [operator]
+    A(1) >= A(2)  # E: Unsupported left operand type for >= ("A")  [operator]
     A(1) == A(2)
     A(1) != A(2)
 
-    A(1) < 1  # E: Unsupported operand types for > ("int" and "A")
-    A(1) <= 1  # E: Unsupported operand types for >= ("int" and "A")
-    A(1) > 1  # E: Unsupported operand types for < ("int" and "A")
-    A(1) >= 1  # E: Unsupported operand types for <= ("int" and "A")
+    A(1) < 1  # E: Unsupported operand types for > ("int" and "A")  [operator]
+    A(1) <= 1  # E: Unsupported operand types for >= ("int" and "A")  [operator]
+    A(1) > 1  # E: Unsupported operand types for < ("int" and "A")  [operator]
+    A(1) >= 1  # E: Unsupported operand types for <= ("int" and "A")  [operator]
     A(1) == 1
     A(1) != 1
 
-    1 < A(1)  # E: Unsupported operand types for < ("int" and "A")
-    1 <= A(1)  # E: Unsupported operand types for <= ("int" and "A")
-    1 > A(1)  # E: Unsupported operand types for > ("int" and "A")
-    1 >= A(1)  # E: Unsupported operand types for >= ("int" and "A")
+    1 < A(1)  # E: Unsupported operand types for < ("int" and "A")  [operator]
+    1 <= A(1)  # E: Unsupported operand types for <= ("int" and "A")  [operator]
+    1 > A(1)  # E: Unsupported operand types for > ("int" and "A")  [operator]
+    1 >= A(1)  # E: Unsupported operand types for >= ("int" and "A")  [operator]
     1 == A(1)
     1 != A(1)
 
 - case: testAttrsCmpEqOrderValues
   main: |
     from attr import attrib, attrs
     @attrs(cmp=True)
     class DeprecatedTrue:
        ...
 
     @attrs(cmp=False)
     class DeprecatedFalse:
        ...
 
-    @attrs(cmp=False, eq=True)  # E: Don't mix "cmp" with "eq" and "order"
+    @attrs(cmp=False, eq=True)  # E: Don't mix "cmp" with "eq" and "order"  [misc]
     class Mixed:
        ...
 
-    @attrs(order=True, eq=False)  # E: eq must be True if order is True
+    @attrs(order=True, eq=False)  # E: eq must be True if order is True  [misc]
     class Confused:
        ...
 
 - case: testAttrsInheritance
   main: |
     import attr
     @attr.s
@@ -380,25 +380,25 @@
     import attr
 
     @attr.s(frozen=True)
     class A:
         a = attr.ib()
 
     a = A(5)
-    a.a = 16  # E: Property "a" defined in "A" is read-only
+    a.a = 16  # E: Property "a" defined in "A" is read-only  [misc]
 - case: testAttrsNextGenFrozen
   main: |
     from attr import frozen, field
 
     @frozen
     class A:
         a = field()
 
     a = A(5)
-    a.a = 16  # E: Property "a" defined in "A" is read-only
+    a.a = 16  # E: Property "a" defined in "A" is read-only  [misc]
 
 - case: testAttrsNextGenDetect
   main: |
     from attr import define, field
 
     @define
     class A:
@@ -460,23 +460,23 @@
         x: List[T]
         y: T = attr.ib()
         def foo(self) -> List[T]:
             return [self.y]
         def bar(self) -> T:
             return self.x[0]
         def problem(self) -> T:
-            return self.x  # E: Incompatible return value type (got "List[T]", expected "T")
+            return self.x  # E: Incompatible return value type (got "List[T]", expected "T")  [return-value]
     reveal_type(A) # N: Revealed type is "def [T] (x: builtins.list[T`1], y: T`1) -> main.A[T`1]"
     a = A([1], 2)
     reveal_type(a)  # N: Revealed type is "main.A[builtins.int]"
     reveal_type(a.x)  # N: Revealed type is "builtins.list[builtins.int]"
     reveal_type(a.y)  # N: Revealed type is "builtins.int"
 
-    A(['str'], 7)  # E: Cannot infer type argument 1 of "A"
-    A([1], '2')  # E: Cannot infer type argument 1 of "A"
+    A(['str'], 7)  # E: Cannot infer type argument 1 of "A"  [misc]
+    A([1], '2')  # E: Cannot infer type argument 1 of "A"  [misc]
 
 - case: testAttrsUntypedGenericInheritance
   main: |
     from typing import Generic, TypeVar
     import attr
 
     T = TypeVar("T")
@@ -639,15 +639,15 @@
         b: str = attr.ib()
         @classmethod
         def new(cls) -> A:
            reveal_type(cls)  # N: Revealed type is "Type[main.A]"
            return cls(6, 'hello')
         @classmethod
         def bad(cls) -> A:
-            return cls(17)  # E: Missing positional argument "b" in call to "A"
+            return cls(17)  # E: Missing positional argument "b" in call to "A"  [call-arg]
         def foo(self) -> int:
            return self.a
     reveal_type(A)  # N: Revealed type is "def (a: builtins.int, b: builtins.str) -> main.A"
     a = A.new()
     reveal_type(a.foo) # N: Revealed type is "def () -> builtins.int"
 
 - case: testAttrsOtherOverloads
@@ -777,18 +777,18 @@
         return ''
     @attr.dataclass
     class A:
         bad: str = attr.ib(converter=bad_converter)
         bad_overloaded: int = attr.ib(converter=bad_overloaded_converter)
     reveal_type(A)
   out: |
-    main:15: error: Cannot determine __init__ type from converter
-    main:15: error: Argument "converter" has incompatible type "Callable[[], str]"; expected "Callable[[Any], Any]"
-    main:16: error: Cannot determine __init__ type from converter
-    main:16: error: Argument "converter" has incompatible type overloaded function; expected "Callable[[Any], Any]"
+    main:15: error: Cannot determine __init__ type from converter  [misc]
+    main:15: error: Argument "converter" has incompatible type "Callable[[], str]"; expected "Callable[[Any], Any]"  [arg-type]
+    main:16: error: Cannot determine __init__ type from converter  [misc]
+    main:16: error: Argument "converter" has incompatible type overloaded function; expected "Callable[[Any], Any]"  [arg-type]
     main:17: note: Revealed type is "def (bad: Any, bad_overloaded: Any) -> main.A"
 
 - case: testAttrsUsingBadConverterReprocess
   mypy_config: strict_optional = False
   main: |
     import attr
     from typing import overload
@@ -805,34 +805,34 @@
         return ''
     @attr.dataclass
     class A:
         bad: str = attr.ib(converter=bad_converter)
         bad_overloaded: int = attr.ib(converter=bad_overloaded_converter)
     reveal_type(A)
   out: |
-    main:16: error: Cannot determine __init__ type from converter
-    main:16: error: Argument "converter" has incompatible type "Callable[[], str]"; expected "Callable[[Any], Any]"
-    main:17: error: Cannot determine __init__ type from converter
-    main:17: error: Argument "converter" has incompatible type overloaded function; expected "Callable[[Any], Any]"
+    main:16: error: Cannot determine __init__ type from converter  [misc]
+    main:16: error: Argument "converter" has incompatible type "Callable[[], str]"; expected "Callable[[Any], Any]"  [arg-type]
+    main:17: error: Cannot determine __init__ type from converter  [misc]
+    main:17: error: Argument "converter" has incompatible type overloaded function; expected "Callable[[Any], Any]"  [arg-type]
     main:18: note: Revealed type is "def (bad: Any, bad_overloaded: Any) -> main.A"
 
 - case: testAttrsUsingUnsupportedConverter
   main: |
     import attr
     class Thing:
         def do_it(self, int) -> str:
-            ...
+            return ""
     thing = Thing()
     def factory(default: int):
-       ...
+       return 1
     @attr.s
     class C:
-        x: str = attr.ib(converter=thing.do_it)  # E: Unsupported converter, only named functions, types and lambdas are currently supported
+        x: str = attr.ib(converter=thing.do_it)  # E: Unsupported converter, only named functions, types and lambdas are currently supported  [misc]
         y: str = attr.ib(converter=lambda x: x)
-        z: str = attr.ib(converter=factory(8))   # E: Unsupported converter, only named functions, types and lambdas are currently supported
+        z: str = attr.ib(converter=factory(8))   # E: Unsupported converter, only named functions, types and lambdas are currently supported  [misc]
     reveal_type(C)  # N: Revealed type is "def (x: Any, y: Any, z: Any) -> main.C"
 
 - case: testAttrsUsingConverterAndSubclass
   main: |
     import attr
 
     def converter(s:int) -> str:
@@ -883,30 +883,30 @@
     reveal_type(A.__lt__)  # N: Revealed type is "def [_AT] (self: _AT`-1, other: _AT`-1) -> builtins.bool"
     reveal_type(B.__lt__)  # N: Revealed type is "def [_AT] (self: _AT`-1, other: _AT`-1) -> builtins.bool"
     reveal_type(C.__lt__)  # N: Revealed type is "def [_AT] (self: _AT`-1, other: _AT`-1) -> builtins.bool"
     reveal_type(D.__lt__)  # N: Revealed type is "def [_AT] (self: _AT`-1, other: _AT`-1) -> builtins.bool"
 
     A() < A()
     B() < B()
-    A() < B() # E: Unsupported operand types for < ("A" and "B")
+    A() < B() # E: Unsupported operand types for < ("A" and "B")  [operator]
 
     C() > A()
     C() > B()
     C() > C()
-    C() > D() # E: Unsupported operand types for > ("C" and "D")
+    C() > D() # E: Unsupported operand types for > ("C" and "D")  [operator]
 
     D() >= A()
-    D() >= B()  # E: Unsupported operand types for >= ("D" and "B")
-    D() >= C()  # E: Unsupported operand types for >= ("D" and "C")
+    D() >= B()  # E: Unsupported operand types for >= ("D" and "B")  [operator]
+    D() >= C()  # E: Unsupported operand types for >= ("D" and "C")  [operator]
     D() >= D()
 
-    A() <= 1  # E: Unsupported operand types for <= ("A" and "int")
-    B() <= 1  # E: Unsupported operand types for <= ("B" and "int")
-    C() <= 1  # E: Unsupported operand types for <= ("C" and "int")
-    D() <= 1  # E: Unsupported operand types for <= ("D" and "int")
+    A() <= 1  # E: Unsupported operand types for <= ("A" and "int")  [operator]
+    B() <= 1  # E: Unsupported operand types for <= ("B" and "int")  [operator]
+    C() <= 1  # E: Unsupported operand types for <= ("C" and "int")  [operator]
+    D() <= 1  # E: Unsupported operand types for <= ("D" and "int")  [operator]
 
 - case: testAttrsComplexSuperclass
   main: |
     import attr
     @attr.s
     class C:
         x: int = attr.ib(default=1)
@@ -929,57 +929,57 @@
     reveal_type(A) # N: Revealed type is "def (x: Any, y: builtins.int, z: Any =) -> main.A"
 
 - case: testAttrsMultiAssign2
   main: |
     import attr
     @attr.s
     class A:
-       x = y = z = attr.ib()  # E: Too many names for one attribute
+       x = y = z = attr.ib()  # E: Too many names for one attribute  [misc]
 
 - case: testAttrsPrivateInit
   main: |
     import attr
     @attr.s
     class C:
         _x = attr.ib(init=False, default=42)
     C()
-    C(_x=42)  # E: Unexpected keyword argument "_x" for "C"
+    C(_x=42)  # E: Unexpected keyword argument "_x" for "C"  [call-arg]
 
 - case: testAttrsAutoMustBeAll
   main: |
     import attr
     @attr.s(auto_attribs=True)
     class A:
        a: int
        b = 17
        # The following forms are not allowed with auto_attribs=True
-       c = attr.ib()  # E: Need type annotation for "c"
-       d, e = attr.ib(), attr.ib() # E: Need type annotation for "d" # E: Need type annotation for "e"
-       f = g = attr.ib()  # E: Need type annotation for "f" # E: Need type annotation for "g"
+       c = attr.ib()  # E: Need type annotation for "c"  [var-annotated]
+       d, e = attr.ib(), attr.ib() # E: Need type annotation for "d"  [var-annotated] # E: Need type annotation for "e"  [var-annotated]
+       f = g = attr.ib()  # E: Need type annotation for "f"  [var-annotated] # E: Need type annotation for "g"  [var-annotated]
 
 - case: testAttrsRepeatedName
   main: |
     import attr
     @attr.s
     class A:
        a = attr.ib(default=8)
        b = attr.ib()
        a = attr.ib()
     reveal_type(A)  # N: Revealed type is "def (b: Any, a: Any) -> main.A"
     @attr.s
     class B:
        a: int = attr.ib(default=8)
        b: int = attr.ib()
-       a: int = attr.ib()  # E: Name "a" already defined on line 10
+       a: int = attr.ib()  # E: Name "a" already defined on line 10  [no-redef]
     reveal_type(B)  # N: Revealed type is "def (b: builtins.int, a: builtins.int) -> main.B"
     @attr.s(auto_attribs=True)
     class C:
        a: int = 8
        b: int
-       a: int = attr.ib()  # E: Name "a" already defined on line 16
+       a: int = attr.ib()  # E: Name "a" already defined on line 16  [no-redef]
     reveal_type(C)  # N: Revealed type is "def (a: builtins.int, b: builtins.int) -> main.C"
 
 - case: testAttrsFrozenSubclass
   main: |
     import attr
 
     @attr.dataclass
@@ -1002,27 +1002,27 @@
     class NonFrozenFrozen(FrozenBase):
         b: int
 
     # Make sure these are untouched
     non_frozen_base = NonFrozenBase(1)
     non_frozen_base.a = 17
     frozen_base = FrozenBase(1)
-    frozen_base.a = 17  # E: Property "a" defined in "FrozenBase" is read-only
+    frozen_base.a = 17  # E: Property "a" defined in "FrozenBase" is read-only  [misc]
 
     a = FrozenNonFrozen(1, 2)
-    a.a = 17  # E: Property "a" defined in "FrozenNonFrozen" is read-only
-    a.b = 17  # E: Property "b" defined in "FrozenNonFrozen" is read-only
+    a.a = 17  # E: Property "a" defined in "FrozenNonFrozen" is read-only  [misc]
+    a.b = 17  # E: Property "b" defined in "FrozenNonFrozen" is read-only  [misc]
 
     b = FrozenFrozen(1, 2)
-    b.a = 17  # E: Property "a" defined in "FrozenFrozen" is read-only
-    b.b = 17  # E: Property "b" defined in "FrozenFrozen" is read-only
+    b.a = 17  # E: Property "a" defined in "FrozenFrozen" is read-only  [misc]
+    b.b = 17  # E: Property "b" defined in "FrozenFrozen" is read-only  [misc]
 
     c = NonFrozenFrozen(1, 2)
-    c.a = 17  # E: Property "a" defined in "NonFrozenFrozen" is read-only
-    c.b = 17  # E: Property "b" defined in "NonFrozenFrozen" is read-only
+    c.a = 17  # E: Property "a" defined in "NonFrozenFrozen" is read-only  [misc]
+    c.b = 17  # E: Property "b" defined in "NonFrozenFrozen" is read-only  [misc]
 - case: testAttrsCallableAttributes
   main: |
     from typing import Callable
     import attr
     def blah(a: int, b: int) -> bool:
         return True
 
@@ -1056,37 +1056,37 @@
     A()
 
 - case: testAttrsFactoryAndDefault
   main: |
     import attr
     @attr.s
     class A:
-        x: int = attr.ib(factory=int, default=7)  # E: Can't pass both "default" and "factory".
+        x: int = attr.ib(factory=int, default=7)  # E: Can't pass both "default" and "factory".  [misc]
 
 - case: testAttrsFactoryBadReturn
   main: |
     import attr
     def my_factory() -> int:
         return 7
     @attr.s
     class A:
-        x: int = attr.ib(factory=list)  # E: Incompatible types in assignment (expression has type "List[_T]", variable has type "int")
-        y: str = attr.ib(factory=my_factory) # E: Incompatible types in assignment (expression has type "int", variable has type "str")
+        x: int = attr.ib(factory=list)  # E: Incompatible types in assignment (expression has type "List[_T]", variable has type "int")  [assignment]
+        y: str = attr.ib(factory=my_factory) # E: Incompatible types in assignment (expression has type "int", variable has type "str")  [assignment]
 
 - case: testAttrsDefaultAndInit
   main: |
     import attr
 
     @attr.s
     class C:
        a = attr.ib(init=False, default=42)
        b = attr.ib()  # Ok because previous attribute is init=False
        c = attr.ib(default=44)
        d = attr.ib(init=False)  # Ok because this attribute is init=False
-       e = attr.ib()  # E: Non-default attributes not allowed after default attributes.
+       e = attr.ib()  # E: Non-default attributes not allowed after default attributes.  [misc]
 
 - case: testAttrsOptionalConverter
   main: |
     # flags: --strict-optional
     import attr
     from attr.converters import optional
     from typing import Optional
@@ -1117,26 +1117,26 @@
 
 - case: testAttrsKwOnlyAttrib
   main: |
     import attr
     @attr.s
     class A:
         a = attr.ib(kw_only=True)
-    A()  # E: Missing named argument "a" for "A"
-    A(15) # E: Too many positional arguments for "A"
+    A()  # E: Missing named argument "a" for "A"  [call-arg]
+    A(15) # E: Too many positional arguments for "A"  [misc]
     A(a=15)
 
 - case: testAttrsKwOnlyClass
   main: |
     import attr
     @attr.s(kw_only=True, auto_attribs=True)
     class A:
         a: int
         b: bool
-    A()  # E: Missing named argument "a" for "A" # E: Missing named argument "b" for "A"
+    A()  # E: Missing named argument "a" for "A"  [call-arg] # E: Missing named argument "b" for "A"  [call-arg]
     A(b=True, a=15)
 
 - case: testAttrsKwOnlyClassNoInit
   main: |
     import attr
     @attr.s(kw_only=True)
     class B:
@@ -1207,15 +1207,15 @@
 - case: testDisallowUntypedWorksForwardBad
   mypy_config: disallow_untyped_defs = True
   main: |
     import attr
 
     @attr.s
     class B:
-        x = attr.ib()  # E: Need type annotation for "x"
+        x = attr.ib()  # E: Need type annotation for "x"  [var-annotated]
 
     reveal_type(B)  # N: Revealed type is "def (x: Any) -> main.B"
 
 - case: testAttrsDefaultDecoratorDeferred
   main: |
     defer: Yes
 
@@ -1249,51 +1249,51 @@
 
 - case: testTypeInAttrUndefined
   main: |
     import attr
 
     @attr.s
     class C:
-        total = attr.ib(type=Bad)  # E: Name "Bad" is not defined
+        total = attr.ib(type=Bad)  # E: Name "Bad" is not defined  [name-defined]
 
 - case: testTypeInAttrForwardInRuntime
   main: |
     import attr
 
     @attr.s
     class C:
         total = attr.ib(type=Forward)
 
     reveal_type(C.total)  # N: Revealed type is "main.Forward"
-    C('no')  # E: Argument 1 to "C" has incompatible type "str"; expected "Forward"
+    C('no')  # E: Argument 1 to "C" has incompatible type "str"; expected "Forward"  [arg-type]
     class Forward: ...
 
 - case: testDefaultInAttrForward
   main: |
     import attr
 
     @attr.s
     class C:
         total = attr.ib(default=func())
 
-    def func() -> int: ...
+    def func() -> int: return 5
 
     C()
     C(1)
-    C(1, 2)  # E: Too many arguments for "C"
+    C(1, 2)  # E: Too many arguments for "C"  [call-arg]
 
 - case: testTypeInAttrUndefinedFrozen
   main: |
     import attr
 
     @attr.s(frozen=True)
     class C:
-        total = attr.ib(type=Bad)  # E: Name "Bad" is not defined
+        total = attr.ib(type=Bad)  # E: Name "Bad" is not defined  [name-defined]
 
-    C(0).total = 1  # E: Property "total" defined in "C" is read-only
+    C(0).total = 1  # E: Property "total" defined in "C" is read-only  [misc]
 
 - case: testTypeInAttrDeferredStar
   main: |
     import lib
   files:
     - path: lib.py
       content: |
@@ -1302,31 +1302,31 @@
         if MYPY:  # Force deferral
             from other import *
 
         @attr.s
         class C:
             total = attr.ib(type=int)
 
-        C()  # E: Missing positional argument "total" in call to "C"
-        C('no')  # E: Argument 1 to "C" has incompatible type "str"; expected "int"
+        C()  # E: Missing positional argument "total" in call to "C"  [call-arg]
+        C('no')  # E: Argument 1 to "C" has incompatible type "str"; expected "int"  [arg-type]
     - path: other.py
       content: |
         import lib
 
 - case: testAttrsDefaultsMroOtherFile
   main: |
     import a
   files:
     - path: a.py
       content: |
         import attr
         from b import A1, A2
 
         @attr.s
-        class Asdf(A1, A2):  # E: Non-default attributes not allowed after default attributes.
+        class Asdf(A1, A2):  # E: Non-default attributes not allowed after default attributes.  [misc]
             pass
     - path: b.py
       content: |
         import attr
 
         @attr.s
         class A1:
@@ -1366,15 +1366,34 @@
   main: |
     from attrs import fields
 
     class A:
       a: int
       b: str
 
-    fields(A)  # E: Argument 1 to "fields" has incompatible type "Type[A]"; expected "Type[AttrsInstance]"
+    fields(A)  # E: Argument 1 to "fields" has incompatible type "Type[A]"; expected "Type[AttrsInstance]"  [arg-type]
+
+- case: testAsDict
+  main: |
+    from attrs import asdict, define
+
+    @define
+    class A:
+      a: int
+
+    asdict(A(1))
+
+- case: testAsDictError
+  main: |
+    from attrs import asdict
+
+    class A:
+      a: int
+
+    asdict(A())  # E: Argument 1 to "asdict" has incompatible type "A"; expected "AttrsInstance"  [arg-type]
 
 - case: testHasTypeGuard
   main: |
     from attrs import define, has
 
     @define
     class A:
```

### Comparing `attrs-22.2.0/tests/test_next_gen.py` & `attrs-23.1.0/tests/test_next_gen.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
 Integration tests for next-generation APIs.
 """
 
 import re
 
+from contextlib import contextmanager
 from functools import partial
 
 import pytest
 
 import attr as _attr  # don't use it by accident
 import attrs
 
@@ -23,14 +24,24 @@
 class TestNextGen:
     def test_simple(self):
         """
         Instantiation works.
         """
         C("1", 2)
 
+    def test_field_type(self):
+        """
+        Make class with attrs.field and type parameter.
+        """
+        classFields = {"testint": attrs.field(type=int)}
+
+        A = attrs.make_class("A", classFields)
+
+        assert int == attrs.fields(A).testint.type
+
     def test_no_slots(self):
         """
         slots can be deactivated.
         """
 
         @attrs.define(slots=False)
         class NoSlots:
@@ -308,14 +319,46 @@
                 raise ValueError()
             except ValueError:
                 raise MyException("foo") from None
 
         assert "foo" == ei.value.x
         assert ei.value.__cause__ is None
 
+    @pytest.mark.parametrize(
+        "decorator",
+        [
+            partial(_attr.s, frozen=True, slots=True, auto_exc=True),
+            attrs.frozen,
+            attrs.define,
+            attrs.mutable,
+        ],
+    )
+    def test_setting_traceback_on_exception(self, decorator):
+        """
+        contextlib.contextlib (re-)sets __traceback__ on raised exceptions.
+
+        Ensure that works, as well as if done explicitly
+        """
+
+        @decorator
+        class MyException(Exception):
+            pass
+
+        @contextmanager
+        def do_nothing():
+            yield
+
+        with do_nothing(), pytest.raises(MyException) as ei:
+            raise MyException()
+
+        assert isinstance(ei.value, MyException)
+
+        # this should not raise an exception either
+        ei.value.__traceback__ = ei.value.__traceback__
+
     def test_converts_and_validates_by_default(self):
         """
         If no on_setattr is set, assume setters.convert, setters.validate.
         """
 
         @attrs.define
         class C:
@@ -342,15 +385,14 @@
         Attributes and methods are looked up the same way in NG by default.
 
         See #428
         """
 
         @attrs.define
         class A:
-
             x: int = 10
 
             def xx(self):
                 return 10
 
         @attrs.define
         class B(A):
```

### Comparing `attrs-22.2.0/tests/test_pattern_matching.py` & `attrs-23.1.0/tests/test_pattern_matching.py`

 * *Files identical despite different names*

### Comparing `attrs-22.2.0/tests/test_pyright.py` & `attrs-23.1.0/tests/test_pyright.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,14 +59,19 @@
         ),
         PyrightDiagnostic(
             severity="information",
             message='Type of "DefineConverter.__init__" is '
             '"(self: DefineConverter, with_converter: int) -> None"',
         ),
         PyrightDiagnostic(
+            severity="error",
+            message='Cannot assign member "a" for type '
+            '"Frozen"\n\xa0\xa0"Frozen" is frozen',
+        ),
+        PyrightDiagnostic(
             severity="information",
             message='Type of "d.a" is "Literal[\'new\']"',
         ),
         PyrightDiagnostic(
             severity="error",
             message='Cannot assign member "a" for type '
             '"FrozenDefine"\n\xa0\xa0"FrozenDefine" is frozen',
```

### Comparing `attrs-22.2.0/tests/test_setattr.py` & `attrs-23.1.0/tests/test_setattr.py`

 * *Files identical despite different names*

### Comparing `attrs-22.2.0/tests/test_slots.py` & `attrs-23.1.0/tests/test_slots.py`

 * *Files 2% similar despite different names*

```diff
@@ -750,21 +750,20 @@
 @attr.s(slots=True)
 class A:
     x = attr.ib()
     b = attr.ib()
     c = attr.ib()
 
 
-@pytest.mark.parametrize("cls", [A])
-def test_slots_unpickle_after_attr_removed(cls):
+def test_slots_unpickle_after_attr_removed():
     """
     We don't assign attributes we don't have anymore if the class has
     removed it.
     """
-    a = cls(1, 2, 3)
+    a = A(1, 2, 3)
     a_pickled = pickle.dumps(a)
     a_unpickled = pickle.loads(a_pickled)
     assert a_unpickled == a
 
     @attr.s(slots=True)
     class NEW_A:
         x = attr.ib()
@@ -774,20 +773,19 @@
         new_a = pickle.loads(a_pickled)
 
         assert new_a.x == 1
         assert new_a.c == 3
         assert not hasattr(new_a, "b")
 
 
-@pytest.mark.parametrize("cls", [A])
-def test_slots_unpickle_after_attr_added(cls, frozen):
+def test_slots_unpickle_after_attr_added(frozen):
     """
     We don't assign attribute we haven't had before if the class has one added.
     """
-    a = cls(1, 2, 3)
+    a = A(1, 2, 3)
     a_pickled = pickle.dumps(a)
     a_unpickled = pickle.loads(a_pickled)
 
     assert a_unpickled == a
 
     @attr.s(slots=True, frozen=frozen)
     class NEW_A:
@@ -799,7 +797,24 @@
     with mock.patch(f"{__name__}.A", NEW_A):
         new_a = pickle.loads(a_pickled)
 
         assert new_a.x == 1
         assert new_a.b == 2
         assert new_a.c == 3
         assert not hasattr(new_a, "d")
+
+
+def test_slots_unpickle_is_backward_compatible(frozen):
+    """
+    Ensure object pickled before v22.2.0 can still be unpickled.
+    """
+    a = A(1, 2, 3)
+
+    a_pickled = (
+        b"\x80\x04\x95&\x00\x00\x00\x00\x00\x00\x00\x8c\x10"
+        + a.__module__.encode()
+        + b"\x94\x8c\x01A\x94\x93\x94)\x81\x94K\x01K\x02K\x03\x87\x94b."
+    )
+
+    a_unpickled = pickle.loads(a_pickled)
+
+    assert a_unpickled == a
```

### Comparing `attrs-22.2.0/tests/test_validators.py` & `attrs-23.1.0/tests/test_validators.py`

 * *Files 2% similar despite different names*

```diff
@@ -345,50 +345,62 @@
         """
 
         @zope_interface.implementer(ifoo)
         class C:
             def f(self):
                 pass
 
-        v = provides(ifoo)
+        with pytest.deprecated_call():
+            v = provides(ifoo)
+
         v(None, simple_attr("x"), C())
 
     def test_fail(self, ifoo):
         """
         Raises `TypeError` if interfaces isn't provided by value.
         """
         value = object()
         a = simple_attr("x")
 
-        v = provides(ifoo)
+        with pytest.deprecated_call():
+            v = provides(ifoo)
+
         with pytest.raises(TypeError) as e:
             v(None, a, value)
+
         assert (
             "'x' must provide {interface!r} which {value!r} doesn't.".format(
                 interface=ifoo, value=value
             ),
             a,
             ifoo,
             value,
         ) == e.value.args
 
     def test_repr(self, ifoo):
         """
         Returned validator has a useful `__repr__`.
         """
-        v = provides(ifoo)
+        with pytest.deprecated_call():
+            v = provides(ifoo)
+
         assert (
             "<provides validator for interface {interface!r}>".format(
                 interface=ifoo
             )
         ) == repr(v)
 
 
 @pytest.mark.parametrize(
-    "validator", [instance_of(int), [always_pass, instance_of(int)]]
+    "validator",
+    [
+        instance_of(int),
+        [always_pass, instance_of(int)],
+        (always_pass, instance_of(int)),
+    ],
 )
 class TestOptional:
     """
     Tests for `optional`.
     """
 
     def test_in_all(self, validator):
@@ -433,14 +445,19 @@
         v = optional(validator)
 
         if isinstance(validator, list):
             repr_s = (
                 "<optional validator for _AndValidator(_validators=[{func}, "
                 "<instance_of validator for type <class 'int'>>]) or None>"
             ).format(func=repr(always_pass))
+        elif isinstance(validator, tuple):
+            repr_s = (
+                "<optional validator for _AndValidator(_validators=({func}, "
+                "<instance_of validator for type <class 'int'>>)) or None>"
+            ).format(func=repr(always_pass))
         else:
             repr_s = (
                 "<optional validator for <instance_of validator for type "
                 "<class 'int'>> or None>"
             )
 
         assert repr_s == repr(v)
```

### Comparing `attrs-22.2.0/tests/test_version_info.py` & `attrs-23.1.0/tests/test_version_info.py`

 * *Files identical despite different names*

### Comparing `attrs-22.2.0/tests/typing_example.py` & `attrs-23.1.0/tests/typing_example.py`

 * *Files 4% similar despite different names*

```diff
@@ -232,14 +232,23 @@
     )
     o: Any = attr.ib(
         validator=attr.validators.not_(attr.validators.in_("abc"), msg="spam")
     )
     p: Any = attr.ib(
         validator=attr.validators.not_(attr.validators.in_("abc"), msg=None)
     )
+    q: Any = attr.ib(
+        validator=attrs.validators.optional(attrs.validators.instance_of(C))
+    )
+    r: Any = attr.ib(
+        validator=attrs.validators.optional([attrs.validators.instance_of(C)])
+    )
+    s: Any = attr.ib(
+        validator=attrs.validators.optional((attrs.validators.instance_of(C),))
+    )
 
 
 @attr.define
 class Validated2:
     num: int = attr.field(validator=attr.validators.ge(0))
 
 
@@ -428,26 +437,28 @@
 def accessing_from_attr() -> None:
     """
     Use a function to keep the ns clean.
     """
     attr.converters.optional
     attr.exceptions.FrozenError
     attr.filters.include
+    attr.filters.exclude
     attr.setters.frozen
     attr.validators.and_
     attr.cmp_using
 
 
 def accessing_from_attrs() -> None:
     """
     Use a function to keep the ns clean.
     """
     attrs.converters.optional
     attrs.exceptions.FrozenError
     attrs.filters.include
+    attrs.filters.exclude
     attrs.setters.frozen
     attrs.validators.and_
     attrs.cmp_using
 
 
 foo = object
 if attrs.has(foo) or attr.has(foo):
```

### Comparing `attrs-22.2.0/tests/utils.py` & `attrs-23.1.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `attrs-22.2.0/tox.ini` & `attrs-23.1.0/tox.ini`

 * *Files 16% similar despite different names*

```diff
@@ -1,108 +1,63 @@
-# Keep docs in sync with docs env and .readthedocs.yml.
-[gh-actions]
-python =
-    3.6: py36, mypy
-    3.7: py37
-    3.8: py38, changelog
-    3.9: py39
-    3.10: py310, mypy
-    3.11: py311
-    3.12: py312
-    pypy-3: pypy3
-
-
 [tox]
-envlist = mypy,pre-commit,py36,py37,py38,py39,py310,py311,py312,pypy3,pyright,manifest,docs,pypi-description,changelog,coverage-report
+envlist = mypy,pre-commit,py37,py38,py39,py310,py311,py312,pypy3,pyright,docs,changelog,coverage-report
 isolated_build = True
 
 
 [testenv:docs]
-# Keep basepython in sync with ci.yml/docs and .readthedocs.yml.
-basepython = python3.10
+# Keep basepython in sync with ci.yml/docs and .readthedocs.yaml.
+basepython = python3.11
 extras = docs
 commands =
     sphinx-build -n -T -W -b html -d {envtmpdir}/doctrees docs docs/_build/html
     sphinx-build -n -T -W -b doctest -d {envtmpdir}/doctrees docs docs/_build/html
 
+
 [testenv]
 extras = tests
-commands = python -m pytest {posargs:-n auto}
-
-
-[testenv:py36]
-extras = cov
-setenv = COVERAGE_PROCESS_START={toxinidir}/pyproject.toml
-commands = coverage run -m pytest {posargs:-n auto}
-
-
-[testenv:py310]
-extras = cov
-setenv =
-    PYTHONWARNINGS=d
-    {[testenv:py36]setenv}
-commands = {[testenv:py36]commands}
+commands = pytest {posargs:-n auto}
+passenv = SETUPTOOLS_SCM_PRETEND_VERSION
 
 
-[testenv:py31{1,2}]
+[testenv:py3{7,10,11}]
 extras = cov
 # Python 3.6+ has a number of compile-time warnings on invalid string escapes.
 # PYTHONWARNINGS=d and --no-compile below make them visible during the Tox run.
-install_command = python -m pip install --no-compile {opts} {packages}
+install_command = python -Im pip install --no-compile {opts} {packages}
 setenv =
+    HATCH_BUILD_HOOK_ENABLE_AUTORUN=1
+    COVERAGE_PROCESS_START={toxinidir}/pyproject.toml
     PYTHONWARNINGS=d
-    {[testenv:py36]setenv}
-# xdist is currently broken on 3.11rc2
-commands = coverage run -m pytest {posargs}
+commands = coverage run -m pytest {posargs:-n auto}
 
 
 [testenv:coverage-report]
-basepython = python3.10
-depends = py36,py310
+basepython = python3.11
+depends = py3{7,10,11}
 skip_install = true
 deps = coverage[toml]>=5.3
 commands =
     coverage combine
     coverage report
 
 
 [testenv:pre-commit]
 skip_install = true
 deps = pre-commit
-passenv = HOMEPATH  # needed on Windows
-commands = pre-commit run --all-files --show-diff-on-failure
-
-
-[testenv:manifest]
-basepython = python3.10
-deps = check-manifest
-skip_install = true
-commands = check-manifest
-
-
-[testenv:pypi-description]
-basepython = python3.8
-skip_install = true
-deps =
-    twine
-    pip >= 18.0.0
-commands =
-    pip wheel -w {envtmpdir}/build --no-deps .
-    twine check {envtmpdir}/build/*
+commands = pre-commit run --all-files
 
 
 [testenv:changelog]
-basepython = python3.8
 deps = towncrier
 skip_install = true
 commands = towncrier build --version main --draft
 
 
 [testenv:mypy]
-deps = mypy>=0.902
+deps = mypy>=0.991
 commands =
     mypy src/attrs/__init__.pyi src/attr/__init__.pyi src/attr/_typing_compat.pyi src/attr/_version_info.pyi src/attr/converters.pyi src/attr/exceptions.pyi src/attr/filters.pyi src/attr/setters.pyi src/attr/validators.pyi
     mypy tests/typing_example.py
 
 
 [testenv:pyright]
 # Install and configure node and pyright
```

