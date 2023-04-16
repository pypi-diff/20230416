# Comparing `tmp/osw-0.5.2.tar.gz` & `tmp/osw-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osw-0.5.2.tar", last modified: Mon Mar 27 03:27:39 2023, max compression
+gzip compressed data, was "osw-0.6.0.tar", last modified: Sun Apr 16 02:50:59 2023, max compression
```

## Comparing `osw-0.5.2.tar` & `osw-0.6.0.tar`

### file list

```diff
@@ -1,99 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 03:27:39.870239 osw-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-03-27 03:27:08.000000 osw-0.5.2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 03:27:39.842239 osw-0.5.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 03:27:39.850239 osw-0.5.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-03-27 03:27:08.000000 osw-0.5.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-03-27 03:27:08.000000 osw-0.5.2/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-03-27 03:27:08.000000 osw-0.5.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-03-27 03:27:08.000000 osw-0.5.2/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-27 03:27:08.000000 osw-0.5.2/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-03-27 03:27:08.000000 osw-0.5.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-03-27 03:27:08.000000 osw-0.5.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-27 03:27:08.000000 osw-0.5.2/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-03-27 03:27:08.000000 osw-0.5.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    13425 2023-03-27 03:27:08.000000 osw-0.5.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    32387 2023-03-27 03:27:08.000000 osw-0.5.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-03-27 03:27:39.870239 osw-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-03-27 03:27:08.000000 osw-0.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-27 03:27:08.000000 osw-0.5.2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 03:27:39.854239 osw-0.5.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-03-27 03:27:08.000000 osw-0.5.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 03:27:39.854239 osw-0.5.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-27 03:27:08.000000 osw-0.5.2/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-27 03:27:08.000000 osw-0.5.2/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-27 03:27:08.000000 osw-0.5.2/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)    10000 2023-03-27 03:27:08.000000 osw-0.5.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-27 03:27:08.000000 osw-0.5.2/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-03-27 03:27:08.000000 osw-0.5.2/docs/dev.md
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-03-27 03:27:08.000000 osw-0.5.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-27 03:27:08.000000 osw-0.5.2/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-27 03:27:08.000000 osw-0.5.2/docs/model.md
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-03-27 03:27:08.000000 osw-0.5.2/docs/osw.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-27 03:27:08.000000 osw-0.5.2/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-03-27 03:27:08.000000 osw-0.5.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-27 03:27:08.000000 osw-0.5.2/docs/tools.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 03:27:39.858239 osw-0.5.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-27 03:27:08.000000 osw-0.5.2/examples/accounts.pwd.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-03-27 03:27:08.000000 osw-0.5.2/examples/controller_logic.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-03-27 03:27:08.000000 osw-0.5.2/examples/create_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-03-27 03:27:08.000000 osw-0.5.2/examples/create_page_package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 03:27:39.858239 osw-0.5.2/examples/data_processing/
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-03-27 03:27:08.000000 osw-0.5.2/examples/data_processing/local_jsonpath_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-03-27 03:27:08.000000 osw-0.5.2/examples/database_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-03-27 03:27:08.000000 osw-0.5.2/examples/entity_manipulation.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-03-27 03:27:08.000000 osw-0.5.2/examples/load_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    15311 2023-03-27 03:27:08.000000 osw-0.5.2/examples/local_editing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6444 2023-03-27 03:27:08.000000 osw-0.5.2/examples/page_manipulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-03-27 03:27:08.000000 osw-0.5.2/examples/register_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-03-27 03:27:08.000000 osw-0.5.2/examples/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-03-27 03:27:08.000000 osw-0.5.2/examples/store_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-03-27 03:27:08.000000 osw-0.5.2/examples/update_local_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-03-27 03:27:08.000000 osw-0.5.2/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 03:27:39.842239 osw-0.5.2/nb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 03:27:39.858239 osw-0.5.2/nb/quantities/
--rw-r--r--   0 runner    (1001) docker     (123)   123529 2023-03-27 03:27:08.000000 osw-0.5.2/nb/quantities/Quantities.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 03:27:39.862239 osw-0.5.2/nb/quantities/archive/
--rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-03-27 03:27:08.000000 osw-0.5.2/nb/quantities/archive/Onto2Wiki_qudtQuantities.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   107607 2023-03-27 03:27:08.000000 osw-0.5.2/nb/quantities/archive/broader.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    59112 2023-03-27 03:27:08.000000 osw-0.5.2/nb/quantities/archive/buildDictionaryTest.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   152865 2023-03-27 03:27:08.000000 osw-0.5.2/nb/quantities/archive/httpRequest.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    18955 2023-03-27 03:27:08.000000 osw-0.5.2/nb/quantities/archive/idea.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    18386 2023-03-27 03:27:08.000000 osw-0.5.2/nb/quantities/archive/querys.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    31162 2023-03-27 03:27:08.000000 osw-0.5.2/nb/quantities/archive/searchRunaways.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 03:27:39.862239 osw-0.5.2/nb/translations/
--rw-r--r--   0 runner    (1001) docker     (123)   404547 2023-03-27 03:27:08.000000 osw-0.5.2/nb/translations/DeeplTranslate.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-03-27 03:27:08.000000 osw-0.5.2/nb/translations/JsObjectToJson.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-03-27 03:27:08.000000 osw-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-03-27 03:27:39.870239 osw-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-03-27 03:27:08.000000 osw-0.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 03:27:39.842239 osw-0.5.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 03:27:39.862239 osw-0.5.2/src/osw/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-03-27 03:27:08.000000 osw-0.5.2/src/osw/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 03:27:39.866239 osw-0.5.2/src/osw/controller/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-27 03:27:08.000000 osw-0.5.2/src/osw/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-03-27 03:27:08.000000 osw-0.5.2/src/osw/controller/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    20235 2023-03-27 03:27:08.000000 osw-0.5.2/src/osw/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 03:27:39.866239 osw-0.5.2/src/osw/model/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-27 03:27:08.000000 osw-0.5.2/src/osw/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-03-27 03:27:08.000000 osw-0.5.2/src/osw/model/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     8563 2023-03-27 03:27:08.000000 osw-0.5.2/src/osw/model/page_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-03-27 03:27:08.000000 osw-0.5.2/src/osw/sparql_client_smw.py
--rw-r--r--   0 runner    (1001) docker     (123)    37219 2023-03-27 03:27:08.000000 osw-0.5.2/src/osw/wiki_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    20350 2023-03-27 03:27:08.000000 osw-0.5.2/src/osw/wtsite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 03:27:39.866239 osw-0.5.2/src/osw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-03-27 03:27:39.000000 osw-0.5.2/src/osw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-03-27 03:27:39.000000 osw-0.5.2/src/osw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 03:27:39.000000 osw-0.5.2/src/osw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 03:27:39.000000 osw-0.5.2/src/osw.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-03-27 03:27:39.000000 osw-0.5.2/src/osw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-03-27 03:27:39.000000 osw-0.5.2/src/osw.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 03:27:39.870239 osw-0.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-03-27 03:27:08.000000 osw-0.5.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-03-27 03:27:08.000000 osw-0.5.2/tests/controller_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 03:27:39.870239 osw-0.5.2/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-03-27 03:27:08.000000 osw-0.5.2/tests/integration/login_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-27 03:27:08.000000 osw-0.5.2/tests/integration/store_and_load_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-03-27 03:27:08.000000 osw-0.5.2/tests/sparql_client_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-03-27 03:27:08.000000 osw-0.5.2/tests/test_osl.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-03-27 03:27:08.000000 osw-0.5.2/tests/test_wiki_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-03-27 03:27:08.000000 osw-0.5.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:50:59.855885 osw-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-16 02:50:27.000000 osw-0.6.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:50:59.811885 osw-0.6.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:50:59.823885 osw-0.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-04-16 02:50:27.000000 osw-0.6.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-16 02:50:27.000000 osw-0.6.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-16 02:50:27.000000 osw-0.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-16 02:50:27.000000 osw-0.6.0/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-16 02:50:27.000000 osw-0.6.0/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-16 02:50:27.000000 osw-0.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-16 02:50:27.000000 osw-0.6.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-16 02:50:27.000000 osw-0.6.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-16 02:50:27.000000 osw-0.6.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-16 02:50:27.000000 osw-0.6.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)    13425 2023-04-16 02:50:27.000000 osw-0.6.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    32387 2023-04-16 02:50:27.000000 osw-0.6.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-04-16 02:50:59.855885 osw-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-16 02:50:27.000000 osw-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-16 02:50:27.000000 osw-0.6.0/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:50:59.831885 osw-0.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-16 02:50:27.000000 osw-0.6.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:50:59.831885 osw-0.6.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-16 02:50:27.000000 osw-0.6.0/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-16 02:50:27.000000 osw-0.6.0/docs/auth.md
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-16 02:50:27.000000 osw-0.6.0/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-16 02:50:27.000000 osw-0.6.0/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10000 2023-04-16 02:50:27.000000 osw-0.6.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-16 02:50:27.000000 osw-0.6.0/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-16 02:50:27.000000 osw-0.6.0/docs/controller.md
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-16 02:50:27.000000 osw-0.6.0/docs/dev.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-16 02:50:27.000000 osw-0.6.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-16 02:50:27.000000 osw-0.6.0/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-16 02:50:27.000000 osw-0.6.0/docs/model.md
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-16 02:50:27.000000 osw-0.6.0/docs/osw.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-16 02:50:27.000000 osw-0.6.0/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-16 02:50:27.000000 osw-0.6.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-16 02:50:27.000000 osw-0.6.0/docs/tools.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:50:59.835885 osw-0.6.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-16 02:50:27.000000 osw-0.6.0/examples/accounts.pwd.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-16 02:50:27.000000 osw-0.6.0/examples/controller_logic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-16 02:50:27.000000 osw-0.6.0/examples/create_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-04-16 02:50:27.000000 osw-0.6.0/examples/create_page_package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:50:59.835885 osw-0.6.0/examples/data_processing/
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-16 02:50:27.000000 osw-0.6.0/examples/data_processing/local_jsonpath_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-16 02:50:27.000000 osw-0.6.0/examples/database_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-04-16 02:50:27.000000 osw-0.6.0/examples/entity_manipulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-16 02:50:27.000000 osw-0.6.0/examples/load_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15311 2023-04-16 02:50:27.000000 osw-0.6.0/examples/local_editing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6444 2023-04-16 02:50:27.000000 osw-0.6.0/examples/page_manipulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-16 02:50:27.000000 osw-0.6.0/examples/register_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-16 02:50:27.000000 osw-0.6.0/examples/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-16 02:50:27.000000 osw-0.6.0/examples/store_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-16 02:50:27.000000 osw-0.6.0/examples/update_local_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-16 02:50:27.000000 osw-0.6.0/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:50:59.811885 osw-0.6.0/nb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:50:59.835885 osw-0.6.0/nb/quantities/
+-rw-r--r--   0 runner    (1001) docker     (123)   123529 2023-04-16 02:50:27.000000 osw-0.6.0/nb/quantities/Quantities.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:50:59.839885 osw-0.6.0/nb/quantities/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-04-16 02:50:27.000000 osw-0.6.0/nb/quantities/archive/Onto2Wiki_qudtQuantities.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   107607 2023-04-16 02:50:27.000000 osw-0.6.0/nb/quantities/archive/broader.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    59112 2023-04-16 02:50:27.000000 osw-0.6.0/nb/quantities/archive/buildDictionaryTest.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   152865 2023-04-16 02:50:27.000000 osw-0.6.0/nb/quantities/archive/httpRequest.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    18955 2023-04-16 02:50:27.000000 osw-0.6.0/nb/quantities/archive/idea.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    18386 2023-04-16 02:50:27.000000 osw-0.6.0/nb/quantities/archive/querys.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    31162 2023-04-16 02:50:27.000000 osw-0.6.0/nb/quantities/archive/searchRunaways.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:50:59.843885 osw-0.6.0/nb/translations/
+-rw-r--r--   0 runner    (1001) docker     (123)   404547 2023-04-16 02:50:27.000000 osw-0.6.0/nb/translations/DeeplTranslate.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-16 02:50:27.000000 osw-0.6.0/nb/translations/JsObjectToJson.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-16 02:50:27.000000 osw-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-04-16 02:50:59.855885 osw-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-16 02:50:27.000000 osw-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:50:59.815885 osw-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:50:59.843885 osw-0.6.0/src/osw/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-16 02:50:27.000000 osw-0.6.0/src/osw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-04-16 02:50:27.000000 osw-0.6.0/src/osw/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:50:59.847885 osw-0.6.0/src/osw/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-16 02:50:27.000000 osw-0.6.0/src/osw/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-16 02:50:27.000000 osw-0.6.0/src/osw/controller/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-16 02:50:27.000000 osw-0.6.0/src/osw/controller/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19603 2023-04-16 02:50:27.000000 osw-0.6.0/src/osw/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:50:59.851885 osw-0.6.0/src/osw/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-16 02:50:27.000000 osw-0.6.0/src/osw/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-04-16 02:50:27.000000 osw-0.6.0/src/osw/model/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8563 2023-04-16 02:50:27.000000 osw-0.6.0/src/osw/model/page_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-16 02:50:27.000000 osw-0.6.0/src/osw/model/static.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-04-16 02:50:27.000000 osw-0.6.0/src/osw/sparql_client_smw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37231 2023-04-16 02:50:27.000000 osw-0.6.0/src/osw/wiki_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20350 2023-04-16 02:50:27.000000 osw-0.6.0/src/osw/wtsite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:50:59.847885 osw-0.6.0/src/osw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-04-16 02:50:59.000000 osw-0.6.0/src/osw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-16 02:50:59.000000 osw-0.6.0/src/osw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 02:50:59.000000 osw-0.6.0/src/osw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 02:50:59.000000 osw-0.6.0/src/osw.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-16 02:50:59.000000 osw-0.6.0/src/osw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-16 02:50:59.000000 osw-0.6.0/src/osw.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:50:59.851885 osw-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-16 02:50:27.000000 osw-0.6.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-16 02:50:27.000000 osw-0.6.0/tests/controller_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:50:59.855885 osw-0.6.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-04-16 02:50:27.000000 osw-0.6.0/tests/integration/db_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-16 02:50:27.000000 osw-0.6.0/tests/integration/login_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-16 02:50:27.000000 osw-0.6.0/tests/integration/store_and_load_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-16 02:50:27.000000 osw-0.6.0/tests/sparql_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-04-16 02:50:27.000000 osw-0.6.0/tests/test_credential_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-16 02:50:27.000000 osw-0.6.0/tests/test_osl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-16 02:50:27.000000 osw-0.6.0/tests/test_wiki_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-04-16 02:50:27.000000 osw-0.6.0/tox.ini
```

### Comparing `osw-0.5.2/.coveragerc` & `osw-0.6.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `osw-0.5.2/.github/workflows/ci.yml` & `osw-0.6.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `osw-0.5.2/.github/workflows/docs.yml` & `osw-0.6.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `osw-0.5.2/.gitignore` & `osw-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `osw-0.5.2/.pre-commit-config.yaml` & `osw-0.6.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `osw-0.5.2/CHANGELOG.md` & `osw-0.6.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `osw-0.5.2/CONTRIBUTING.md` & `osw-0.6.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `osw-0.5.2/LICENSE.txt` & `osw-0.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `osw-0.5.2/PKG-INFO` & `osw-0.6.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: osw
-Version: 0.5.2
+Version: 0.6.0
 Summary: Python toolset for data processing, queries, wikicode generation and page manipulation
 Home-page: https://github.com/OpenSemanticLab/osw-python
 Author: "Simon Stier"
 Author-email: simon.stier@isc.fraunhofer.de
 License: AGPL-3.0-or-later
 Project-URL: Documentation, https://opensemanticlab.github.io/osw-python/
 Project-URL: Source, https://github.com/OpenSemanticLab/osw-python
 Project-URL: Changelog, https://github.com/OpenSemanticLab/osw-python/blob/main/CHANGELOG.md
 Project-URL: Download, https://pypi.org/project/osw/#files
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Provides-Extra: DB
 Provides-Extra: testing
 License-File: LICENSE.txt
 
 <!-- These are examples of badges you might want to add to your README:
      please update the URLs accordingly
 
 [![Built Status](https://api.cirrus-ci.com/github/<USER>/osw.svg?branch=main)](https://cirrus-ci.com/github/<USER>/osw)
@@ -26,14 +27,15 @@
 [![PyPI-Server](https://img.shields.io/pypi/v/osw.svg)](https://pypi.org/project/osw/)
 [![Conda-Forge](https://img.shields.io/conda/vn/conda-forge/osw.svg)](https://anaconda.org/conda-forge/osw)
 [![Monthly Downloads](https://pepy.tech/badge/osw/month)](https://pepy.tech/project/osw)
 [![Twitter](https://img.shields.io/twitter/url/http/shields.io.svg?style=social&label=Twitter)](https://twitter.com/osw)
 -->
 
 [![PyPI-Server](https://img.shields.io/pypi/v/osw.svg)](https://pypi.org/project/osw/)
+[![DOI](https://zenodo.org/badge/458130867.svg)](https://zenodo.org/badge/latestdoi/458130867)
 [![Coveralls](https://img.shields.io/coveralls/github/OpenSemanticLab/osw-python/main.svg)](https://coveralls.io/r/<USER>/osw)
 [![Project generated with PyScaffold](https://img.shields.io/badge/-PyScaffold-005CA0?logo=pyscaffold)](https://pyscaffold.org/)
 
 # osw
 
 > Python toolset for data processing, queries, wikicode generation and page manipulation
```

### Comparing `osw-0.5.2/README.md` & `osw-0.6.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 [![PyPI-Server](https://img.shields.io/pypi/v/osw.svg)](https://pypi.org/project/osw/)
 [![Conda-Forge](https://img.shields.io/conda/vn/conda-forge/osw.svg)](https://anaconda.org/conda-forge/osw)
 [![Monthly Downloads](https://pepy.tech/badge/osw/month)](https://pepy.tech/project/osw)
 [![Twitter](https://img.shields.io/twitter/url/http/shields.io.svg?style=social&label=Twitter)](https://twitter.com/osw)
 -->
 
 [![PyPI-Server](https://img.shields.io/pypi/v/osw.svg)](https://pypi.org/project/osw/)
+[![DOI](https://zenodo.org/badge/458130867.svg)](https://zenodo.org/badge/latestdoi/458130867)
 [![Coveralls](https://img.shields.io/coveralls/github/OpenSemanticLab/osw-python/main.svg)](https://coveralls.io/r/<USER>/osw)
 [![Project generated with PyScaffold](https://img.shields.io/badge/-PyScaffold-005CA0?logo=pyscaffold)](https://pyscaffold.org/)
 
 # osw
 
 > Python toolset for data processing, queries, wikicode generation and page manipulation
```

### Comparing `osw-0.5.2/docs/Makefile` & `osw-0.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `osw-0.5.2/docs/conf.py` & `osw-0.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `osw-0.5.2/docs/index.md` & `osw-0.6.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `osw-0.5.2/examples/controller_logic.py` & `osw-0.6.0/examples/controller_logic.py`

 * *Files identical despite different names*

### Comparing `osw-0.5.2/examples/create_page_package.py` & `osw-0.6.0/examples/create_page_package.py`

 * *Files identical despite different names*

### Comparing `osw-0.5.2/examples/data_processing/local_jsonpath_queries.py` & `osw-0.6.0/examples/data_processing/local_jsonpath_queries.py`

 * *Files identical despite different names*

### Comparing `osw-0.5.2/examples/database_access.py` & `osw-0.6.0/examples/database_access.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,64 +1,61 @@
 import os
 
-# import osw.controller.entity as controller
 import osw.model.entity as model
+from osw.auth import CredentialManager
 from osw.core import OSW
 from osw.wtsite import WtSite
 
 # create/update the password file under examples/accounts.pwd.yaml
 pwd_file_path = os.path.join(
     os.path.dirname(os.path.abspath(__file__)), "accounts.pwd.yaml"
 )
 # pwd_file_path = "./accounts.pwd.yaml"
 wtsite = WtSite.from_domain("wiki-dev.open-semantic-lab.org", pwd_file_path)
 osw = OSW(site=wtsite)
 
 wtsite.enable_cache()  # skip downloads on second request
 
 # osw.fetch_schema() #this will load the current entity schema from the OSW instance. You may have to re-run the script to get the updated schema extension. Requires 'pip install datamodel-code-generator'
-if False:
+if True:
     osw.fetch_schema(
         OSW.FetchSchemaParam(
-            schema_title="Category:OSW02590972aeba46d7864ed492c0c11384", mode="replace"
+            schema_title="Category:OSW02590972aeba46d7864ed492c0c11384",  # Host
+            mode="replace",
         )
     )
     osw.fetch_schema(
         OSW.FetchSchemaParam(
-            schema_title="Category:OSWacdb001c926c46b998af3e645d36b13f", mode="append"
+            schema_title="Category:OSWacdb001c926c46b998af3e645d36b13f",
+            # DatabaseServer
+            mode="append",
         )
     )
     osw.fetch_schema(
         OSW.FetchSchemaParam(
-            schema_title="Category:OSW51ad0d1716254c77a2b7a03217f23b43", mode="append"
+            schema_title="Category:OSW51ad0d1716254c77a2b7a03217f23b43",  # Database
+            mode="append",
+        )
+    )
+    osw.fetch_schema(
+        OSW.FetchSchemaParam(
+            schema_title="Category:OSW33c7c3a4076a4a58b20d818c162e84e6",  # DatabaseType
+            mode="append",
         )
     )
 
-# #explicit load host and server
-# host = osw.load_entity("Item:OSWb8625aedf4074b72a4fa9bcb11694e4d")
-# server = osw.load_entity("Item:OSW536e1417a0eb427887aeb267f47442fb")
-
-db = osw.load_entity("Item:OSW837099bdc67d4b7cb5ffcce713a7648b")
-db = db.cast(model.Database)
-
-# #load host and server from references
-# server = osw.load_entity(db.db_server)
-# server = server.cast(model.DatabaseServer)
-# host = osw.load_entity(server.host)
-# host = host.cast(model.Host)
-
-# #load host and server from semantic queries
-server_title = wtsite.semantic_search(
-    f"[[-HasDbServer::Item:{osw.get_osw_id(db.uuid)}]]"
-)
-server = osw.load_entity(server_title[0])
-
-host_title = wtsite.semantic_search(f"[[-HasHost::Item:{osw.get_osw_id(server.uuid)}]]")
-host = osw.load_entity(host_title[0])
 
+# make sure to import controllers after updating the model (ignore linter warning)
+import osw.controller as controller  # noqa: E402
 
-connect_str = f"{host.network_domain[0]}:{server.network_port[0]}/{db.db_name}"
-print(connect_str)
+# load database definition
+db = osw.load_entity("Item:OSWb8cc7705e17c47b19331fdb045bfbca8")  # postgres
+db = db.cast(model.Database)
 
 # cast into controller and execute function
-# db = db.cast(controller.DbController)
-# print(db.create_table())
+db = db.cast(controller.DatabaseController)
+db.connect(
+    controller.DatabaseController.ConnectionConfig(
+        cm=CredentialManager(cred_filepath=pwd_file_path), osw=osw
+    )
+)
+db.execute("SELECT * FROM public.sensors ORDER BY sensor_id ASC")
```

### Comparing `osw-0.5.2/examples/entity_manipulation.py` & `osw-0.6.0/examples/entity_manipulation.py`

 * *Files identical despite different names*

### Comparing `osw-0.5.2/examples/load_entity.py` & `osw-0.6.0/examples/load_entity.py`

 * *Files identical despite different names*

### Comparing `osw-0.5.2/examples/local_editing.py` & `osw-0.6.0/examples/local_editing.py`

 * *Files identical despite different names*

### Comparing `osw-0.5.2/examples/page_manipulation.py` & `osw-0.6.0/examples/page_manipulation.py`

 * *Files identical despite different names*

### Comparing `osw-0.5.2/examples/register_model.py` & `osw-0.6.0/examples/register_model.py`

 * *Files identical despite different names*

### Comparing `osw-0.5.2/examples/settings.json` & `osw-0.6.0/examples/settings.json`

 * *Files identical despite different names*

### Comparing `osw-0.5.2/examples/store_entity.py` & `osw-0.6.0/examples/store_entity.py`

 * *Files identical despite different names*

### Comparing `osw-0.5.2/nb/quantities/Quantities.ipynb` & `osw-0.6.0/nb/quantities/Quantities.ipynb`

 * *Files identical despite different names*

### Comparing `osw-0.5.2/nb/quantities/archive/Onto2Wiki_qudtQuantities.ipynb` & `osw-0.6.0/nb/quantities/archive/Onto2Wiki_qudtQuantities.ipynb`

 * *Files identical despite different names*

### Comparing `osw-0.5.2/nb/quantities/archive/broader.ipynb` & `osw-0.6.0/nb/quantities/archive/broader.ipynb`

 * *Files identical despite different names*

### Comparing `osw-0.5.2/nb/quantities/archive/buildDictionaryTest.ipynb` & `osw-0.6.0/nb/quantities/archive/buildDictionaryTest.ipynb`

 * *Files identical despite different names*

### Comparing `osw-0.5.2/nb/quantities/archive/httpRequest.ipynb` & `osw-0.6.0/nb/quantities/archive/httpRequest.ipynb`

 * *Files identical despite different names*

### Comparing `osw-0.5.2/nb/quantities/archive/idea.ipynb` & `osw-0.6.0/nb/quantities/archive/idea.ipynb`

 * *Files identical despite different names*

### Comparing `osw-0.5.2/nb/quantities/archive/querys.ipynb` & `osw-0.6.0/nb/quantities/archive/querys.ipynb`

 * *Files identical despite different names*

### Comparing `osw-0.5.2/nb/quantities/archive/searchRunaways.ipynb` & `osw-0.6.0/nb/quantities/archive/searchRunaways.ipynb`

 * *Files identical despite different names*

### Comparing `osw-0.5.2/nb/translations/DeeplTranslate.ipynb` & `osw-0.6.0/nb/translations/DeeplTranslate.ipynb`

 * *Files identical despite different names*

### Comparing `osw-0.5.2/nb/translations/JsObjectToJson.ipynb` & `osw-0.6.0/nb/translations/JsObjectToJson.ipynb`

 * *Files identical despite different names*

### Comparing `osw-0.5.2/setup.cfg` & `osw-0.6.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -45,18 +45,21 @@
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
+DB = sqlalchemy; psycopg2
 testing = 
 	setuptools~=63.4.1
 	pytest~=7.1.2
 	pytest-cov
+	sqlalchemy
+	psycopg2
 
 [options.entry_points]
 
 [tool:pytest]
 addopts = 
 	--cov osw --cov-report term-missing
 	--verbose
@@ -80,14 +83,16 @@
 exclude = 
 	.tox
 	build
 	dist
 	.eggs
 	docs/conf.py
 	src/osw/model/entity.py #autogenerated
+per-file-ignores = 
+	__init__.py:F401
 
 [pyscaffold]
 version = 4.3.1
 package = osw
 extensions = 
 	github_actions
 	markdown
```

### Comparing `osw-0.5.2/setup.py` & `osw-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `osw-0.5.2/src/osw/core.py` & `osw-0.6.0/src/osw/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -365,34 +365,22 @@
             )  # remove import statement
 
             if fetchSchemaParam.mode == "replace":
 
                 header = (
                     "from uuid import uuid4\n"
                     "from typing import TYPE_CHECKING, Type, TypeVar\n"
+                    "from osw.model.static import OswBaseModel\n"
                     "\n"
                     "if TYPE_CHECKING:\n"
                     "    from dataclasses import dataclass as _basemodel_decorator\n"
                     "else:\n"
                     "    _basemodel_decorator = lambda x: x  # noqa: E731\n"
                     "\n"
                 )
-                header += (
-                    '\nT = TypeVar("T", bound=BaseModel)\n'
-                    "\nclass OswBaseModel(BaseModel):\n"
-                    "    def full_dict(self, **kwargs): #extent BaseClass export function\n"
-                    "        d = super().dict(**kwargs)\n"
-                    "        for key in "
-                    + str(self._protected_keywords).replace("'", '"')
-                    + ":\n"
-                    "            if hasattr(self, key): d[key] = getattr(self, key) #include selected private properites. note: private properties are not considered as discriminator \n"
-                    "        return d\n\n"
-                    "    def cast(self, cls: Type[T]) -> T:\n"
-                    "       return cls(**self.dict())\n"
-                )
 
                 content = re.sub(
                     r"(class\s*\S*\s*\(\s*OswBaseModel\s*\)\s*:.*\n)",
                     header + r"\n\n\n\1",
                     content,
                     1,
                 )  # replace first match
@@ -418,15 +406,15 @@
                     r"class\s*([\S]*)\s*\(\s*\S*\s*\)\s*:.*\n"
                 )  # match class definition [\s\S]*(?:[^\S\n]*\n){2,}
                 for cls in re.findall(pattern, org_content):
                     print(cls)
                     content = re.sub(
                         r"(class\s*"
                         + cls
-                        + r"\s*\(\s*\S*\s*\)\s*:.*\n[\s\S]*?(?:[^\S\n]*\n){2,})",
+                        + r"\s*\(\s*\S*\s*\)\s*:.*\n[\s\S]*?(?:[^\S\n]*\n){3,})",
                         "",
                         content,
                         count=1,
                     )  # replace duplicated classes
 
                 content = re.sub(
                     r"(from __future__ import annotations)", "", content, 1
@@ -522,10 +510,12 @@
         """
         if isinstance(entity, model.Item):
             entity_title = "Item:" + OSW.get_osw_id(entity.uuid)
             page = self.site.get_WtPage(entity_title)
         else:
             print("Error: Unsupported entity type")
             return
-
-        page.delete(comment)
-        print("Entity deleted: " + page.get_url())
+        if page.exists:
+            page.delete(comment)
+            print("Entity deleted: " + page.get_url())
+        else:
+            print(f"Entity '{entity_title}' does not exist!")
```

### Comparing `osw-0.5.2/src/osw/model/entity.py` & `osw-0.6.0/src/osw/model/entity.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,75 +1,36 @@
 # generated by datamodel-codegen:
-#   filename:  Item.json
-#   timestamp: 2023-01-23T06:27:29+00:00
+#   filename:  Entity.json
+#   timestamp: 2023-04-14T02:20:12+00:00
 
 from __future__ import annotations
 
 from enum import Enum
-from typing import Any, List, Optional
+from typing import Any, List, Optional, Union
 from uuid import UUID
 
 from pydantic import BaseModel, Field
-from typing_extensions import Literal
 
 
 class LangCode(Enum):
     en = "en"
     de = "de"
 
 
 from typing import TYPE_CHECKING, Type, TypeVar
 from uuid import uuid4
 
+from osw.model.static import OswBaseModel
+
 if TYPE_CHECKING:
     from dataclasses import dataclass as _basemodel_decorator
 else:
     _basemodel_decorator = lambda x: x  # noqa: E731
 
 
-T = TypeVar("T", bound=BaseModel)
-
-
-class OswBaseModel(BaseModel):
-    def full_dict(self, **kwargs):  # extent BaseClass export function
-        d = super().dict(**kwargs)
-        for key in ("_osl_template", "_osl_footer"):
-            if hasattr(self, key):
-                d[key] = getattr(
-                    self, key
-                )  # include selected private properites. note: private properties are not considered as discriminator
-        return d
-
-    def cast(self, cls: Type[T]) -> T:
-        return cls(**self.dict())
-
-    def cast_none_to_default(self, cls: Type[T]) -> T:
-        """Casting self into target class. If the passed attribute is None or solely
-        includes None values, the attribute is not passed to the instance of the
-        target class, which will then fall back to the default."""
-
-        def test_if_empty_list_or_none(obj) -> bool:
-            if obj is None:
-                return True
-            elif isinstance(obj, list):
-                if len(obj) == 0:
-                    return True
-                elif len([item for item in obj if item is not None]) == 0:
-                    return True
-            return False
-
-        return cls(
-            **{
-                k: v
-                for k, v in self.dict().items()
-                if not test_if_empty_list_or_none(v)
-            }
-        )
-
-
 @_basemodel_decorator
 class Label(OswBaseModel):
     text: str = Field(..., title="Text")
     lang: Optional[LangCode] = Field("en", title="Lang code")
 
 
 class LangCode1(Enum):
@@ -80,42 +41,93 @@
 @_basemodel_decorator
 class Description(OswBaseModel):
     text: str = Field(..., title="Text")
     lang: Optional[LangCode1] = Field("en", title="Lang code")
 
 
 @_basemodel_decorator
-class Statement(OswBaseModel):
-    osl_template: Optional[Literal["OslTemplate:Statement"]] = "OslTemplate:Statement"
-    label: Optional[Label] = Field(None, title="Label")
-    """
-    Human readable name
-    """
-    uuid: UUID = Field(default_factory=uuid4, title="UUID")
-    subject: Optional[str] = None
-    predicate: str
-    object: Optional[str] = None
-    substatements: Optional[List[Statement]] = Field(None, title="Substatements")
+class CommonDefinitions(OswBaseModel):
+    __root__: Any
 
 
 @_basemodel_decorator
 class Entity(OswBaseModel):
     uuid: UUID = Field(default_factory=uuid4, title="UUID")
-    label: Label = Field(..., title="Label")
+    name: Optional[str] = Field(None, title="Name")
     """
-    Human readable name
+    Technical / Machine compatible name
+    """
+    label: List[Label] = Field(..., min_items=1, title="Labels")
+    """
+    Human readable names. You have to assign at least one.
+    """
+    short_name: Optional[List[Label]] = Field(None, title="Short name")
+    """
+    Abbreviation, Acronym, etc.
     """
     query_label: Optional[str] = Field(None, title="Label")
-    additional_labels: Optional[List[Label]] = Field(None, title="Additional Labels")
     description: Optional[List[Description]] = Field(None, title="Description")
     image: Optional[str] = Field(None, title="Image")
+    based_on: Optional[List[str]] = Field(None, title="Based on")
+    """
+    Other entities on which this one is based, e.g. when it is created by copying
+    """
     statements: Optional[List[Statement]] = Field(None, title="Statements")
-    extensions: Optional[List[Any]] = Field(None, title="Extensions")
+    attachments: Optional[List[str]] = Field(None, title="File attachments")
+
+
+@_basemodel_decorator
+class Statement1(OswBaseModel):
+    uuid: UUID = Field(default_factory=uuid4, title="UUID")
+    label: Optional[List[Label]] = Field(None, title="Label")
+    """
+    Human readable name
+    """
+    subject: Optional[str] = Field(None, title="Subject")
+    substatements: Optional[List[Statement]] = Field(None, title="Substatements")
+
+
+@_basemodel_decorator
+class Statement(OswBaseModel):
+    __root__: Union[Statement1, CommonDefinitions, CommonDefinitions, CommonDefinitions]
+
+
+Entity.update_forward_refs()
+Statement1.update_forward_refs()
+# generated by datamodel-codegen:
+#   filename:  Item.json
+#   timestamp: 2023-04-14T02:20:14+00:00
+
+
+from enum import Enum
+from typing import Any, List, Optional, Union
+from uuid import UUID
+
+from pydantic import BaseModel, Field
+
+
+class Level(Enum):
+    public = "public"
+    internal = "internal"
+    restricted = "restricted"
+
+
+class ReadAccess(OswBaseModel):
+    level: Optional[Level] = Field(None, title="Level")
+
+
+class AccessRestrictions(OswBaseModel):
+    read: Optional[ReadAccess] = Field(None, title="Read access")
 
 
 class Item(Entity):
     type: Optional[List[str]] = Field(
         ["Category:Item"], min_length=1, title="Types/Categories"
     )
+    entry_access: Optional[AccessRestrictions] = Field(
+        None, title="Access restrictions"
+    )
 
 
-Statement.update_forward_refs()
+Entity.update_forward_refs()
+Statement1.update_forward_refs()
+Item.update_forward_refs()
```

### Comparing `osw-0.5.2/src/osw/model/page_package.py` & `osw-0.6.0/src/osw/model/page_package.py`

 * *Files identical despite different names*

### Comparing `osw-0.5.2/src/osw/sparql_client_smw.py` & `osw-0.6.0/src/osw/sparql_client_smw.py`

 * *Files identical despite different names*

### Comparing `osw-0.5.2/src/osw/wiki_tools.py` & `osw-0.6.0/src/osw/wiki_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import copy
 import getpass
 from pathlib import Path
-from typing import Dict, List, Union
+from typing import Dict, List, Tuple, Union
 
 import mwclient
 import mwparserfromhell
 import numpy as np
 import yaml
 from jsonpath_ng.ext import parse
 
 
 def read_domains_from_credentials_file(
     credentials_file_path: Union[str, Path]
-) -> (List[str], Dict[str, Dict[str, str]]):
+) -> Tuple[List[str], Dict[str, Dict[str, str]]]:
     """Reads domains and credentials from a yaml file
 
     Parameters
     ----------
     credentials_file_path
         Path to the yaml file with the credentials
```

### Comparing `osw-0.5.2/src/osw/wtsite.py` & `osw-0.6.0/src/osw/wtsite.py`

 * *Files identical despite different names*

### Comparing `osw-0.5.2/src/osw.egg-info/PKG-INFO` & `osw-0.6.0/src/osw.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: osw
-Version: 0.5.2
+Version: 0.6.0
 Summary: Python toolset for data processing, queries, wikicode generation and page manipulation
 Home-page: https://github.com/OpenSemanticLab/osw-python
 Author: "Simon Stier"
 Author-email: simon.stier@isc.fraunhofer.de
 License: AGPL-3.0-or-later
 Project-URL: Documentation, https://opensemanticlab.github.io/osw-python/
 Project-URL: Source, https://github.com/OpenSemanticLab/osw-python
 Project-URL: Changelog, https://github.com/OpenSemanticLab/osw-python/blob/main/CHANGELOG.md
 Project-URL: Download, https://pypi.org/project/osw/#files
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Provides-Extra: DB
 Provides-Extra: testing
 License-File: LICENSE.txt
 
 <!-- These are examples of badges you might want to add to your README:
      please update the URLs accordingly
 
 [![Built Status](https://api.cirrus-ci.com/github/<USER>/osw.svg?branch=main)](https://cirrus-ci.com/github/<USER>/osw)
@@ -26,14 +27,15 @@
 [![PyPI-Server](https://img.shields.io/pypi/v/osw.svg)](https://pypi.org/project/osw/)
 [![Conda-Forge](https://img.shields.io/conda/vn/conda-forge/osw.svg)](https://anaconda.org/conda-forge/osw)
 [![Monthly Downloads](https://pepy.tech/badge/osw/month)](https://pepy.tech/project/osw)
 [![Twitter](https://img.shields.io/twitter/url/http/shields.io.svg?style=social&label=Twitter)](https://twitter.com/osw)
 -->
 
 [![PyPI-Server](https://img.shields.io/pypi/v/osw.svg)](https://pypi.org/project/osw/)
+[![DOI](https://zenodo.org/badge/458130867.svg)](https://zenodo.org/badge/latestdoi/458130867)
 [![Coveralls](https://img.shields.io/coveralls/github/OpenSemanticLab/osw-python/main.svg)](https://coveralls.io/r/<USER>/osw)
 [![Project generated with PyScaffold](https://img.shields.io/badge/-PyScaffold-005CA0?logo=pyscaffold)](https://pyscaffold.org/)
 
 # osw
 
 > Python toolset for data processing, queries, wikicode generation and page manipulation
```

### Comparing `osw-0.5.2/src/osw.egg-info/SOURCES.txt` & `osw-0.6.0/src/osw.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,30 +2,33 @@
 .gitignore
 .gitmodules
 .isort.cfg
 .pre-commit-config.yaml
 .readthedocs.yml
 AUTHORS.md
 CHANGELOG.md
+CITATION.cff
 CONTRIBUTING.md
 LICENSE.txt
 README.md
 __init__.py
 mkdocs.yml
 pyproject.toml
 setup.cfg
 setup.py
 tox.ini
 .github/workflows/ci.yml
 .github/workflows/docs.yml
 docs/Makefile
+docs/auth.md
 docs/authors.md
 docs/changelog.md
 docs/conf.py
 docs/contributing.md
+docs/controller.md
 docs/dev.md
 docs/index.md
 docs/license.md
 docs/model.md
 docs/osw.md
 docs/readme.md
 docs/requirements.txt
@@ -52,29 +55,34 @@
 nb/quantities/archive/httpRequest.ipynb
 nb/quantities/archive/idea.ipynb
 nb/quantities/archive/querys.ipynb
 nb/quantities/archive/searchRunaways.ipynb
 nb/translations/DeeplTranslate.ipynb
 nb/translations/JsObjectToJson.ipynb
 src/osw/__init__.py
+src/osw/auth.py
 src/osw/core.py
 src/osw/sparql_client_smw.py
 src/osw/wiki_tools.py
 src/osw/wtsite.py
 src/osw.egg-info/PKG-INFO
 src/osw.egg-info/SOURCES.txt
 src/osw.egg-info/dependency_links.txt
 src/osw.egg-info/not-zip-safe
 src/osw.egg-info/requires.txt
 src/osw.egg-info/top_level.txt
 src/osw/controller/__init__.py
+src/osw/controller/database.py
 src/osw/controller/entity.py
 src/osw/model/__init__.py
 src/osw/model/entity.py
 src/osw/model/page_package.py
+src/osw/model/static.py
 tests/conftest.py
 tests/controller_mixin.py
 tests/sparql_client_test.py
+tests/test_credential_manager.py
 tests/test_osl.py
 tests/test_wiki_tools.py
+tests/integration/db_test.py
 tests/integration/login_test.py
 tests/integration/store_and_load_test.py
```

### Comparing `osw-0.5.2/tests/conftest.py` & `osw-0.6.0/tests/conftest.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 import pytest
 
 
 def pytest_addoption(parser):
     parser.addoption("--wiki_domain", action="store")
     parser.addoption("--wiki_username", action="store")
     parser.addoption("--wiki_password", action="store")
+    parser.addoption("--db_username", action="store")
+    parser.addoption("--db_password", action="store")
 
 
 @pytest.fixture(scope="session")
 def wiki_domain(request):
     value = request.config.option.wiki_domain
     if value is None:
         pytest.skip()
@@ -34,7 +36,23 @@
 
 @pytest.fixture(scope="session")
 def wiki_password(request):
     value = request.config.option.wiki_password
     if value is None:
         pytest.skip()
     return value
+
+
+@pytest.fixture(scope="session")
+def db_username(request):
+    value = request.config.option.db_username
+    if value is None:
+        pytest.skip()
+    return value
+
+
+@pytest.fixture(scope="session")
+def db_password(request):
+    value = request.config.option.db_password
+    if value is None:
+        pytest.skip()
+    return value
```

### Comparing `osw-0.5.2/tests/controller_mixin.py` & `osw-0.6.0/tests/controller_mixin.py`

 * *Files identical despite different names*

### Comparing `osw-0.5.2/tests/integration/store_and_load_test.py` & `osw-0.6.0/tests/integration/store_and_load_test.py`

 * *Files identical despite different names*

### Comparing `osw-0.5.2/tests/sparql_client_test.py` & `osw-0.6.0/tests/sparql_client_test.py`

 * *Files identical despite different names*

### Comparing `osw-0.5.2/tox.ini` & `osw-0.6.0/tox.ini`

 * *Files identical despite different names*

