# Comparing `tmp/senor-octopus-0.1.9.tar.gz` & `tmp/senor-octopus-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "senor-octopus-0.1.9.tar", last modified: Thu Mar 25 20:56:07 2021, max compression
+gzip compressed data, was "senor-octopus-0.2.0.tar", last modified: Sun Apr 16 19:23:03 2023, max compression
```

## Comparing `senor-octopus-0.1.9.tar` & `senor-octopus-0.2.0.tar`

### file list

```diff
@@ -1,73 +1,143 @@
-drwxr-xr-x   0 beto       (501) staff       (20)        0 2021-03-25 20:56:07.575872 senor-octopus-0.1.9/
--rw-r--r--   0 beto       (501) staff       (20)      596 2021-03-22 23:11:01.000000 senor-octopus-0.1.9/.coveragerc
--rw-r--r--   0 beto       (501) staff       (20)      567 2021-03-23 01:18:54.000000 senor-octopus-0.1.9/.gitignore
--rw-r--r--   0 beto       (501) staff       (20)      608 2021-03-23 01:36:30.000000 senor-octopus-0.1.9/.pre-commit-config.yaml
--rw-r--r--   0 beto       (501) staff       (20)      461 2021-03-22 23:11:01.000000 senor-octopus-0.1.9/.readthedocs.yml
--rw-r--r--   0 beto       (501) staff       (20)     1416 2021-03-22 23:11:01.000000 senor-octopus-0.1.9/.travis.yml
--rw-r--r--   0 beto       (501) staff       (20)       81 2021-03-22 23:11:01.000000 senor-octopus-0.1.9/AUTHORS.rst
--rw-r--r--   0 beto       (501) staff       (20)     1117 2021-03-25 20:55:40.000000 senor-octopus-0.1.9/CHANGELOG.rst
--rw-r--r--   0 beto       (501) staff       (20)     1081 2021-03-22 23:11:01.000000 senor-octopus-0.1.9/LICENSE.txt
--rw-r--r--   0 beto       (501) staff       (20)     4548 2021-03-25 20:56:07.576090 senor-octopus-0.1.9/PKG-INFO
--rw-r--r--   0 beto       (501) staff       (20)     3336 2021-03-25 04:27:02.000000 senor-octopus-0.1.9/README.rst
-drwxr-xr-x   0 beto       (501) staff       (20)        0 2021-03-25 20:56:07.565435 senor-octopus-0.1.9/docs/
--rw-r--r--   0 beto       (501) staff       (20)     1153 2021-03-22 23:11:01.000000 senor-octopus-0.1.9/docs/Makefile
-drwxr-xr-x   0 beto       (501) staff       (20)        0 2021-03-25 20:56:07.565715 senor-octopus-0.1.9/docs/_static/
--rw-r--r--   0 beto       (501) staff       (20)       18 2021-03-22 23:11:01.000000 senor-octopus-0.1.9/docs/_static/.gitignore
--rw-r--r--   0 beto       (501) staff       (20)       41 2021-03-22 23:11:01.000000 senor-octopus-0.1.9/docs/authors.rst
--rw-r--r--   0 beto       (501) staff       (20)       43 2021-03-22 23:11:01.000000 senor-octopus-0.1.9/docs/changelog.rst
--rw-r--r--   0 beto       (501) staff       (20)     9504 2021-03-22 23:11:01.000000 senor-octopus-0.1.9/docs/conf.py
--rw-r--r--   0 beto       (501) staff       (20)     2266 2021-03-22 23:11:01.000000 senor-octopus-0.1.9/docs/index.rst
--rw-r--r--   0 beto       (501) staff       (20)       67 2021-03-22 23:11:01.000000 senor-octopus-0.1.9/docs/license.rst
--rw-r--r--   0 beto       (501) staff       (20)       39 2021-03-22 23:11:01.000000 senor-octopus-0.1.9/docs/readme.rst
--rw-r--r--   0 beto       (501) staff       (20)      233 2021-03-22 23:11:01.000000 senor-octopus-0.1.9/docs/requirements.txt
--rw-r--r--   0 beto       (501) staff       (20)      311 2021-03-22 23:11:01.000000 senor-octopus-0.1.9/pyproject.toml
--rw-r--r--   0 beto       (501) staff       (20)     1992 2021-03-25 20:56:07.577153 senor-octopus-0.1.9/setup.cfg
--rw-r--r--   0 beto       (501) staff       (20)      711 2021-03-22 23:17:27.000000 senor-octopus-0.1.9/setup.py
--rw-r--r--   0 beto       (501) staff       (20)      288 2021-03-25 04:27:02.000000 senor-octopus-0.1.9/simple.ini
-drwxr-xr-x   0 beto       (501) staff       (20)        0 2021-03-25 20:56:07.557996 senor-octopus-0.1.9/src/
-drwxr-xr-x   0 beto       (501) staff       (20)        0 2021-03-25 20:56:07.567527 senor-octopus-0.1.9/src/senor_octopus/
--rw-r--r--   0 beto       (501) staff       (20)      584 2021-03-23 23:59:41.000000 senor-octopus-0.1.9/src/senor_octopus/__init__.py
--rw-r--r--   0 beto       (501) staff       (20)     2234 2021-03-25 20:17:59.000000 senor-octopus-0.1.9/src/senor_octopus/cli.py
-drwxr-xr-x   0 beto       (501) staff       (20)        0 2021-03-25 20:56:07.570040 senor-octopus-0.1.9/src/senor_octopus/filters/
--rw-r--r--   0 beto       (501) staff       (20)      413 2021-03-25 19:25:35.000000 senor-octopus-0.1.9/src/senor_octopus/filters/jpath.py
--rw-r--r--   0 beto       (501) staff       (20)     7600 2021-03-25 19:53:12.000000 senor-octopus-0.1.9/src/senor_octopus/graph.py
--rw-r--r--   0 beto       (501) staff       (20)     1602 2021-03-25 20:41:16.000000 senor-octopus-0.1.9/src/senor_octopus/lib.py
--rw-r--r--   0 beto       (501) staff       (20)     1229 2021-03-25 20:14:17.000000 senor-octopus-0.1.9/src/senor_octopus/scheduler.py
-drwxr-xr-x   0 beto       (501) staff       (20)        0 2021-03-25 20:56:07.570569 senor-octopus-0.1.9/src/senor_octopus/sinks/
-drwxr-xr-x   0 beto       (501) staff       (20)        0 2021-03-25 20:56:07.570872 senor-octopus-0.1.9/src/senor_octopus/sinks/db/
--rw-r--r--   0 beto       (501) staff       (20)     2554 2021-03-25 19:25:35.000000 senor-octopus-0.1.9/src/senor_octopus/sinks/db/postgresql.py
--rw-r--r--   0 beto       (501) staff       (20)      247 2021-03-25 17:44:43.000000 senor-octopus-0.1.9/src/senor_octopus/sinks/log.py
--rw-r--r--   0 beto       (501) staff       (20)      694 2021-03-25 19:25:35.000000 senor-octopus-0.1.9/src/senor_octopus/sinks/pushover.py
-drwxr-xr-x   0 beto       (501) staff       (20)        0 2021-03-25 20:56:07.571905 senor-octopus-0.1.9/src/senor_octopus/sources/
--rw-r--r--   0 beto       (501) staff       (20)     1202 2021-03-25 19:25:35.000000 senor-octopus-0.1.9/src/senor_octopus/sources/awair.py
--rw-r--r--   0 beto       (501) staff       (20)      339 2021-03-25 04:27:02.000000 senor-octopus-0.1.9/src/senor_octopus/sources/rand.py
--rw-r--r--   0 beto       (501) staff       (20)      567 2021-03-25 19:25:35.000000 senor-octopus-0.1.9/src/senor_octopus/sources/speed.py
--rw-r--r--   0 beto       (501) staff       (20)     1117 2021-03-25 19:25:35.000000 senor-octopus-0.1.9/src/senor_octopus/sources/weatherapi.py
--rw-r--r--   0 beto       (501) staff       (20)      658 2021-03-25 17:13:45.000000 senor-octopus-0.1.9/src/senor_octopus/types.py
-drwxr-xr-x   0 beto       (501) staff       (20)        0 2021-03-25 20:56:07.569764 senor-octopus-0.1.9/src/senor_octopus.egg-info/
--rw-r--r--   0 beto       (501) staff       (20)     4548 2021-03-25 20:56:07.000000 senor-octopus-0.1.9/src/senor_octopus.egg-info/PKG-INFO
--rw-r--r--   0 beto       (501) staff       (20)     1432 2021-03-25 20:56:07.000000 senor-octopus-0.1.9/src/senor_octopus.egg-info/SOURCES.txt
--rw-r--r--   0 beto       (501) staff       (20)        1 2021-03-25 20:56:07.000000 senor-octopus-0.1.9/src/senor_octopus.egg-info/dependency_links.txt
--rw-r--r--   0 beto       (501) staff       (20)      503 2021-03-25 20:56:07.000000 senor-octopus-0.1.9/src/senor_octopus.egg-info/entry_points.txt
--rw-r--r--   0 beto       (501) staff       (20)        1 2021-03-22 23:58:27.000000 senor-octopus-0.1.9/src/senor_octopus.egg-info/not-zip-safe
--rw-r--r--   0 beto       (501) staff       (20)      390 2021-03-25 20:56:07.000000 senor-octopus-0.1.9/src/senor_octopus.egg-info/requires.txt
--rw-r--r--   0 beto       (501) staff       (20)       14 2021-03-25 20:56:07.000000 senor-octopus-0.1.9/src/senor_octopus.egg-info/top_level.txt
-drwxr-xr-x   0 beto       (501) staff       (20)        0 2021-03-25 20:56:07.573651 senor-octopus-0.1.9/tests/
--rw-r--r--   0 beto       (501) staff       (20)        0 2021-03-23 22:24:11.000000 senor-octopus-0.1.9/tests/__init__.py
--rw-r--r--   0 beto       (501) staff       (20)      908 2021-03-25 20:17:59.000000 senor-octopus-0.1.9/tests/conftest.py
-drwxr-xr-x   0 beto       (501) staff       (20)        0 2021-03-25 20:56:07.573901 senor-octopus-0.1.9/tests/sinks/
-drwxr-xr-x   0 beto       (501) staff       (20)        0 2021-03-25 20:56:07.574337 senor-octopus-0.1.9/tests/sinks/db/
--rw-r--r--   0 beto       (501) staff       (20)        0 2021-03-23 22:52:47.000000 senor-octopus-0.1.9/tests/sinks/db/__init__.py
--rw-r--r--   0 beto       (501) staff       (20)     3259 2021-03-23 23:55:41.000000 senor-octopus-0.1.9/tests/sinks/db/test_postgresql.py
--rw-r--r--   0 beto       (501) staff       (20)      969 2021-03-23 23:55:03.000000 senor-octopus-0.1.9/tests/sinks/test_pushover.py
-drwxr-xr-x   0 beto       (501) staff       (20)        0 2021-03-25 20:56:07.575511 senor-octopus-0.1.9/tests/sources/
--rw-r--r--   0 beto       (501) staff       (20)     2265 2021-03-23 23:55:03.000000 senor-octopus-0.1.9/tests/sources/test_awair.py
--rw-r--r--   0 beto       (501) staff       (20)     3685 2021-03-24 01:09:24.000000 senor-octopus-0.1.9/tests/sources/test_speed.py
--rw-r--r--   0 beto       (501) staff       (20)     8055 2021-03-25 15:46:49.000000 senor-octopus-0.1.9/tests/sources/test_weatherapi.py
--rw-r--r--   0 beto       (501) staff       (20)    84077 2021-03-25 15:45:55.000000 senor-octopus-0.1.9/tests/sources/weatherapi_response.json
--rw-r--r--   0 beto       (501) staff       (20)     1811 2021-03-23 22:46:52.000000 senor-octopus-0.1.9/tests/test_cli.py
--rw-r--r--   0 beto       (501) staff       (20)     5637 2021-03-25 19:26:05.000000 senor-octopus-0.1.9/tests/test_graph.py
--rw-r--r--   0 beto       (501) staff       (20)     1296 2021-03-25 20:51:24.000000 senor-octopus-0.1.9/tests/test_lib.py
--rw-r--r--   0 beto       (501) staff       (20)     1020 2021-03-25 15:45:55.000000 senor-octopus-0.1.9/tests/test_scheduler.py
--rw-r--r--   0 beto       (501) staff       (20)     2758 2021-03-22 23:11:01.000000 senor-octopus-0.1.9/tests/travis_install.sh
--rw-r--r--   0 beto       (501) staff       (20)     2010 2021-03-24 01:12:12.000000 senor-octopus-0.1.9/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:23:03.854480 senor-octopus-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:23:03.838479 senor-octopus-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:23:03.842480 senor-octopus-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/.github/workflows/python-package-daily.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    15075 2023-04-16 19:23:03.854480 senor-octopus-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13945 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/config.yaml.example
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:23:03.842480 senor-octopus-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:23:03.842480 senor-octopus-0.2.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9504 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:23:03.842480 senor-octopus-0.2.0/recipes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/recipes/beer.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/recipes/co2_alert.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/recipes/lights.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:23:03.842480 senor-octopus-0.2.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-04-16 19:23:03.854480 senor-octopus-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/simple.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:23:03.838479 senor-octopus-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:23:03.842480 senor-octopus-0.2.0/src/senor_octopus/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/src/senor_octopus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/src/senor_octopus/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/src/senor_octopus/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:23:03.846480 senor-octopus-0.2.0/src/senor_octopus/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/src/senor_octopus/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/src/senor_octopus/filters/deserialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/src/senor_octopus/filters/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/src/senor_octopus/filters/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/src/senor_octopus/filters/jpath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/src/senor_octopus/filters/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10268 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/src/senor_octopus/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/src/senor_octopus/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/src/senor_octopus/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:23:03.846480 senor-octopus-0.2.0/src/senor_octopus/sinks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/src/senor_octopus/sinks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:23:03.846480 senor-octopus-0.2.0/src/senor_octopus/sinks/db/
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/src/senor_octopus/sinks/db/postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/src/senor_octopus/sinks/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/src/senor_octopus/sinks/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/src/senor_octopus/sinks/pushover.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/src/senor_octopus/sinks/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/src/senor_octopus/sinks/sms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/src/senor_octopus/sinks/tuya.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:23:03.846480 senor-octopus-0.2.0/src/senor_octopus/sources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/src/senor_octopus/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/src/senor_octopus/sources/awair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/src/senor_octopus/sources/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/src/senor_octopus/sources/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/src/senor_octopus/sources/rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/src/senor_octopus/sources/speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/src/senor_octopus/sources/sqla.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/src/senor_octopus/sources/static.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/src/senor_octopus/sources/stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/src/senor_octopus/sources/sun.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:23:03.846480 senor-octopus-0.2.0/src/senor_octopus/sources/udp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/src/senor_octopus/sources/udp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/src/senor_octopus/sources/udp/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:23:03.846480 senor-octopus-0.2.0/src/senor_octopus/sources/udp/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/src/senor_octopus/sources/udp/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/src/senor_octopus/sources/udp/protocols/micron_bolt_mini_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/src/senor_octopus/sources/weatherapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/src/senor_octopus/sources/whistle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/src/senor_octopus/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:23:03.846480 senor-octopus-0.2.0/src/senor_octopus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15075 2023-04-16 19:23:03.000000 senor-octopus-0.2.0/src/senor_octopus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-04-16 19:23:03.000000 senor-octopus-0.2.0/src/senor_octopus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 19:23:03.000000 senor-octopus-0.2.0/src/senor_octopus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-16 19:23:03.000000 senor-octopus-0.2.0/src/senor_octopus.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 19:23:03.000000 senor-octopus-0.2.0/src/senor_octopus.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-16 19:23:03.000000 senor-octopus-0.2.0/src/senor_octopus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-16 19:23:03.000000 senor-octopus-0.2.0/src/senor_octopus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:23:03.850480 senor-octopus-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/tests/cli_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:23:03.850480 senor-octopus-0.2.0/tests/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/tests/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/tests/filters/deserialize_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/tests/filters/format_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/tests/filters/jinja_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/tests/filters/jpath_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/tests/filters/serialize_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/tests/graph_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/tests/lib_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/tests/scheduler_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:23:03.850480 senor-octopus-0.2.0/tests/sinks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/tests/sinks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:23:03.850480 senor-octopus-0.2.0/tests/sinks/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/tests/sinks/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/tests/sinks/db/postgresql_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/tests/sinks/log_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/tests/sinks/mqtt_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/tests/sinks/pushover_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/tests/sinks/slack_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/tests/sinks/sms_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/tests/sinks/tuya_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:23:03.850480 senor-octopus-0.2.0/tests/sources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/tests/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/tests/sources/awair_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/tests/sources/crypto_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/tests/sources/mqtt_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/tests/sources/rand_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/tests/sources/speed_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/tests/sources/sqla_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/tests/sources/static_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/tests/sources/stock_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/tests/sources/sun_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:23:03.854480 senor-octopus-0.2.0/tests/sources/udp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/tests/sources/udp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/tests/sources/udp/main_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:23:03.854480 senor-octopus-0.2.0/tests/sources/udp/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/tests/sources/udp/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/tests/sources/udp/protocols/micron_bolt_mini_2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84078 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/tests/sources/weatherapi_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9323 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/tests/sources/weatherapi_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/tests/sources/whistle_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-16 19:22:52.000000 senor-octopus-0.2.0/tests/travis_install.sh
```

### Comparing `senor-octopus-0.1.9/.gitignore` & `senor-octopus-0.2.0/.gitignore`

 * *Files 18% similar despite different names*

```diff
@@ -48,9 +48,10 @@
 cover/*
 MANIFEST
 
 # Per-project virtualenvs
 .venv*/
 .conda*/
 
-config.ini
+config.yaml
 venv
+.python-version
```

### Comparing `senor-octopus-0.1.9/LICENSE.txt` & `senor-octopus-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `senor-octopus-0.1.9/docs/Makefile` & `senor-octopus-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `senor-octopus-0.1.9/docs/conf.py` & `senor-octopus-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `senor-octopus-0.1.9/docs/index.rst` & `senor-octopus-0.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `senor-octopus-0.1.9/setup.py` & `senor-octopus-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `senor-octopus-0.1.9/src/senor_octopus/cli.py` & `senor-octopus-0.2.0/src/senor_octopus/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,18 @@
+"""
+A simple CLI for running the scheduler.
+"""
+
 import argparse
 import asyncio
-import configparser
 import logging
 import sys
 
+import yaml
+
 from senor_octopus import __version__
 from senor_octopus.graph import build_dag
 from senor_octopus.lib import render_dag
 from senor_octopus.scheduler import Scheduler
 
 __author__ = "Beto Dealmeida"
 __copyright__ = "Beto Dealmeida"
@@ -26,15 +31,15 @@
     Returns:
       :obj:`argparse.Namespace`: command line parameters namespace
     """
     parser = argparse.ArgumentParser(description="Schedule pipelines")
     parser.add_argument(
         "--version",
         action="version",
-        version="senor-octopus {ver}".format(ver=__version__),
+        version=f"senor-octopus {__version__}",
     )
     parser.add_argument(
         dest="f",
         help="Location of the config file",
         type=str,
         metavar="PATH",
     )
@@ -50,48 +55,68 @@
         "-vv",
         "--very-verbose",
         dest="loglevel",
         help="set loglevel to DEBUG",
         action="store_const",
         const=logging.DEBUG,
     )
+    parser.add_argument(
+        "-n",
+        "--dry-run",
+        dest="dryrun",
+        help="Dry run, print the DAG and exit",
+        action="store_true",
+    )
     return parser.parse_args(args)
 
 
 def setup_logging(loglevel):
+    """
+    Setup basic logging at the specified level.
+    """
     logformat = "[%(asctime)s] %(levelname)s:%(name)s:%(message)s"
     logging.basicConfig(
         level=loglevel,
         stream=sys.stdout,
         format=logformat,
         datefmt="%Y-%m-%d %H:%M:%S",
     )
 
 
-class CaseConfigParser(configparser.RawConfigParser):
-    def optionxform(self, optionstr):
-        return optionstr
-
-
 async def main(args):
+    """
+    Main entry point allowing external calls.
+    """
     args = parse_args(args)
     setup_logging(args.loglevel)
 
     _logger.info("Reading configuration")
-    config = CaseConfigParser()
-    config.read(args.f)
+    with open(args.f, encoding="utf-8") as inp:
+        config = yaml.load(inp, Loader=yaml.SafeLoader)
     _logger.info("Building DAG")
     dag = build_dag(config)
-    _logger.info("\n%s", render_dag(dag))
+    sys.stdout.write(render_dag(dag))
 
-    _logger.info("Running Sr. Octopus")
-    await Scheduler(dag).run()
+    if not args.dryrun:
+        _logger.info("Running Sr. Octopus")
+        scheduler = Scheduler(dag)
+        try:
+            await scheduler.run()
+        except asyncio.CancelledError:
+            _logger.info("Canceled")
+            scheduler.cancel()
 
     _logger.info("Done")
 
 
 def run():
-    asyncio.run(main(sys.argv[1:]))
+    """
+    Entry point for ``console_scripts``.
+    """
+    try:
+        asyncio.run(main(sys.argv[1:]))
+    except KeyboardInterrupt:
+        _logger.info("Stopping Sr. Octopus")
 
 
 if __name__ == "__main__":
     run()
```

### Comparing `senor-octopus-0.1.9/src/senor_octopus/sinks/db/postgresql.py` & `senor-octopus-0.2.0/src/senor_octopus/sinks/db/postgresql.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,56 @@
+"""
+A Postgres sink.
+"""
+
 import logging
-import os
 import textwrap
 
 import aiopg
 from psycopg2 import sql
 from psycopg2.extras import Json
+
 from senor_octopus.types import Stream
 
 _logger = logging.getLogger(__name__)
 
 
-async def postgresql(stream: Stream, table: str = "events") -> None:
-    dbname = os.environ["POSTGRES_DBNAME"]
-    host = os.environ["POSTGRES_HOST"]
-    port = os.environ["POSTGRES_PORT"]
-    user = os.environ["POSTGRES_USER"]
-    password = os.environ["POSTGRES_PASSWORD"]
+async def postgresql(  # pylint: disable=too-many-arguments
+    stream: Stream,
+    user: str,
+    password: str,
+    host: str,
+    port: int,
+    dbname: str,
+    table: str = "events",
+) -> None:
+    """
+    Write events into a Postgres database.
+
+    This sink can be used to write events into a Postgres database.
+    It will create a table with 3 columns, `timestamp`, `name` and
+    `event`, where to events will be stored.
 
+    Parameters
+    ----------
+    stream
+        The incoming stream of events
+    user
+        The username to use when connecting to the DB
+    password
+        The password to use when connecting to the DB
+    host
+        Host where the database is running
+    post
+        Port which the database is listening to
+    dbname
+        Name of the database to connect to
+    table
+        Name of the table where the events will be stored
+    """
     dsn = f"dbname={dbname} user={user} password={password} host={host} port={port}"
     async with aiopg.create_pool(dsn) as pool:
         async with pool.acquire() as conn:
             async with conn.cursor() as cur:
                 _logger.debug("Trying to create table `%s`", table)
                 await cur.execute(
                     sql.SQL(
```

### Comparing `senor-octopus-0.1.9/tests/sinks/test_pushover.py` & `senor-octopus-0.2.0/tests/sinks/pushover_test.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,42 +1,38 @@
-import os
+"""
+Tests for ``sink.pushover``.
+"""
+
 import random
 
 import pytest
+
 from senor_octopus.sinks.pushover import pushover
 from senor_octopus.sources.rand import rand
 
 
 @pytest.mark.asyncio
-async def test_pushover(mocker, httpx_mock) -> None:
-    mocker.patch.dict(
-        os.environ,
-        {
-            "PUSHOVER_APP_TOKEN": "XXX",
-            "PUSHOVER_USER_TOKEN": "alice",
-        },
-    )
+async def test_pushover(httpx_mock) -> None:
+    """
+    Test the source.
+    """
     httpx_mock.add_response()
     random.seed(42)
 
-    await pushover(rand(2))
+    await pushover(rand(2), "XXX", "alice")
     requests = httpx_mock.get_requests()
     assert len(requests) == 2
-    assert (
-        requests[0].read()
-        == b"token=XXX&user=alice&message=hub.random%3A+0.6394267984578837"
+    assert requests[0].read() == (
+        b"token=XXX&user=alice&message=%7Bevent%5B%27name%27%5D%7D%3A+"
+        b"%7Bevent%5B%27value%27%5D%7D"
     )
 
 
 @pytest.mark.asyncio
-async def test_pushover_empty_stream(mocker, httpx_mock) -> None:
-    mocker.patch.dict(
-        os.environ,
-        {
-            "PUSHOVER_APP_TOKEN": "XXX",
-            "PUSHOVER_USER_TOKEN": "alice",
-        },
-    )
+async def test_pushover_empty_stream(httpx_mock) -> None:
+    """
+    Test that nothing is sent when the stream is empty.
+    """
     random.seed(42)
 
-    await pushover(rand(0))
+    await pushover(rand(0), "XXX", "alice")
     assert not httpx_mock.get_request()
```

### Comparing `senor-octopus-0.1.9/tests/sources/test_awair.py` & `senor-octopus-0.2.0/tests/sources/awair_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,15 @@
-import os
-from datetime import datetime
-from datetime import timezone
+"""
+Tests for the Awair source.
+"""
+
+from datetime import datetime, timezone
 
 import pytest
+
 from senor_octopus.sources.awair import awair
 
 mock_payload = {
     "data": [
         {
             "timestamp": "2021-03-23T22:26:51.000Z",
             "score": 95.0,
@@ -26,26 +29,21 @@
             ],
         },
     ],
 }
 
 
 @pytest.mark.asyncio
-async def test_awair(mocker, httpx_mock) -> None:
-    mocker.patch.dict(
-        os.environ,
-        {
-            "AWAIR_ACCESS_TOKEN": "XXX",
-            "AWAIR_DEVICE_TYPE": "awair-element",
-            "AWAIR_DEVICE_ID": "12345",
-        },
-    )
+async def test_awair(httpx_mock) -> None:
+    """
+    Tests for the source.
+    """
     httpx_mock.add_response(json=mock_payload)
 
-    events = [event async for event in awair()]
+    events = [event async for event in awair("XXX", 12345)]
     assert events == [
         {
             "timestamp": datetime(2021, 3, 23, 22, 26, 51, tzinfo=timezone.utc),
             "name": "hub.awair.score",
             "value": 95.0,
         },
         {
```

### Comparing `senor-octopus-0.1.9/tests/sources/test_speed.py` & `senor-octopus-0.2.0/tests/sources/speed_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,17 @@
-from datetime import datetime
+"""
+Tests for the ``speedtest`` source.
+"""
+
+from datetime import datetime, timezone
 from unittest import mock
 
 import pytest
 from freezegun import freeze_time
+
 from senor_octopus.sources.speed import speed
 
 mock_payload = {
     "download": 20932433.00558606,
     "upload": 6068322.252775613,
     "ping": 50.377,
     "server": {
@@ -40,38 +45,40 @@
     },
 }
 
 
 @freeze_time("2021-01-01")
 @pytest.mark.asyncio
 async def test_speed(mocker) -> None:
+    """
+    Tests for the source.
+    """
     mock_speedtest = mock.MagicMock()
     mock_speedtest.Speedtest.return_value.results.dict.return_value = mock_payload
     mocker.patch("senor_octopus.sources.speed.speedtest", mock_speedtest)
 
     events = [event async for event in speed()]
-    print(events)
     assert events == [
         {
-            "timestamp": datetime(2021, 1, 1, 0, 0),
+            "timestamp": datetime(2021, 1, 1, 0, 0, tzinfo=timezone.utc),
             "name": "hub.speedtest.download",
             "value": 20932433.00558606,
         },
         {
-            "timestamp": datetime(2021, 1, 1, 0, 0),
+            "timestamp": datetime(2021, 1, 1, 0, 0, tzinfo=timezone.utc),
             "name": "hub.speedtest.upload",
             "value": 6068322.252775613,
         },
         {
-            "timestamp": datetime(2021, 1, 1, 0, 0),
+            "timestamp": datetime(2021, 1, 1, 0, 0, tzinfo=timezone.utc),
             "name": "hub.speedtest.ping",
             "value": 50.377,
         },
         {
-            "timestamp": datetime(2021, 1, 1, 0, 0),
+            "timestamp": datetime(2021, 1, 1, 0, 0, tzinfo=timezone.utc),
             "name": "hub.speedtest.server",
             "value": {
                 "url": "http://speedtest1.st-tel.net:8080/speedtest/upload.php",
                 "lat": "39.3958",
                 "lon": "-101.0519",
                 "name": "Colby, KS",
                 "country": "United States",
@@ -80,35 +87,35 @@
                 "id": "3434",
                 "host": "speedtest1.st-tel.net:8080",
                 "d": 1896.6996055651487,
                 "latency": 50.377,
             },
         },
         {
-            "timestamp": datetime(2021, 1, 1, 0, 0),
+            "timestamp": datetime(2021, 1, 1, 0, 0, tzinfo=timezone.utc),
             "name": "hub.speedtest.timestamp",
             "value": "2021-03-24T00:56:23.048266Z",
         },
         {
-            "timestamp": datetime(2021, 1, 1, 0, 0),
+            "timestamp": datetime(2021, 1, 1, 0, 0, tzinfo=timezone.utc),
             "name": "hub.speedtest.bytes_sent",
             "value": 8364032,
         },
         {
-            "timestamp": datetime(2021, 1, 1, 0, 0),
+            "timestamp": datetime(2021, 1, 1, 0, 0, tzinfo=timezone.utc),
             "name": "hub.speedtest.bytes_received",
             "value": 26295792,
         },
         {
-            "timestamp": datetime(2021, 1, 1, 0, 0),
+            "timestamp": datetime(2021, 1, 1, 0, 0, tzinfo=timezone.utc),
             "name": "hub.speedtest.share",
             "value": None,
         },
         {
-            "timestamp": datetime(2021, 1, 1, 0, 0),
+            "timestamp": datetime(2021, 1, 1, 0, 0, tzinfo=timezone.utc),
             "name": "hub.speedtest.client",
             "value": {
                 "ip": "66.220.13.38",
                 "lat": "38.3479",
                 "lon": "-122.9737",
                 "isp": "Hurricane Electric",
                 "isprating": "3.7",
```

### Comparing `senor-octopus-0.1.9/tests/sources/weatherapi_response.json` & `senor-octopus-0.2.0/tests/sources/weatherapi_response.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -5248,8 +5248,8 @@
 000147f0: 2020 2267 7573 745f 6b70 6822 3a20 3231    "gust_kph": 21
 00014800: 2e32 2c0a 2020 2020 2020 2020 2020 2020  .2,.            
 00014810: 2020 2020 2020 2020 2020 2020 2275 7622              "uv"
 00014820: 3a20 312e 300a 2020 2020 2020 2020 2020  : 1.0.          
 00014830: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
 00014840: 2020 2020 2020 2020 2020 2020 5d0a 2020              ].  
 00014850: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
-00014860: 2020 2020 5d0a 2020 2020 7d0a 7d             ].    }.}
+00014860: 2020 2020 5d0a 2020 2020 7d0a 7d0a           ].    }.}.
```

### Comparing `senor-octopus-0.1.9/tests/test_cli.py` & `senor-octopus-0.2.0/tests/cli_test.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,42 @@
+"""
+Tests for the CLI.
+"""
+
+import asyncio
 import logging
 import sys
 from unittest import mock
 
 import pytest
-from asynctest import CoroutineMock
-from senor_octopus.cli import main
-from senor_octopus.cli import parse_args
-from senor_octopus.cli import run
-from senor_octopus.cli import setup_logging
+
+from senor_octopus.cli import main, parse_args, run, setup_logging
 
 
 def test_parse_args() -> None:
+    """
+    Test ``parse_args``.
+    """
     with pytest.raises(SystemExit) as excinfo:
         parse_args(["--version"])
     assert str(excinfo.value) == "0"
 
-    parser = parse_args(["config.ini", "-vv"])
-    assert parser.f == "config.ini"
+    parser = parse_args(["config.yaml", "-vv"])
+    assert parser.f == "config.yaml"
     assert parser.loglevel == logging.DEBUG
 
-    parser = parse_args(["config.ini", "-v"])
-    assert parser.f == "config.ini"
+    parser = parse_args(["config.yaml", "-v"])
+    assert parser.f == "config.yaml"
     assert parser.loglevel == logging.INFO
 
 
-def test_setup_logging(mocker, capfd) -> None:
+def test_setup_logging(mocker) -> None:
+    """
+    Test ``setup_logging``.
+    """
     mock_logging = mock.MagicMock()
     mocker.patch("senor_octopus.cli.logging", mock_logging)
 
     setup_logging(logging.WARNING)
 
     mock_logging.basicConfig.assert_called_with(
         level=logging.WARNING,
@@ -36,28 +44,86 @@
         format="[%(asctime)s] %(levelname)s:%(name)s:%(message)s",
         datefmt="%Y-%m-%d %H:%M:%S",
     )
 
 
 @pytest.mark.asyncio
 async def test_main(mocker) -> None:
-    mocker.patch("senor_octopus.cli.CaseConfigParser")
+    """
+    Test ``main``.
+    """
+    mocker.patch("senor_octopus.cli.yaml")
     mocker.patch("senor_octopus.cli.build_dag")
+    mocker.patch("senor_octopus.cli.open")
 
     mock_scheduler = mock.MagicMock()
-    mock_scheduler.return_value.run = CoroutineMock()
-    mock_scheduler.return_value.run.side_effect = [None, Exception("Stopped")]
+    mock_scheduler.return_value.run = mocker.AsyncMock()
     mocker.patch("senor_octopus.cli.Scheduler", mock_scheduler)
 
-    await main(["config.ini"])
+    await main(["config.yaml"])
 
     mock_scheduler.return_value.run.assert_called()
 
 
+@pytest.mark.asyncio
+async def test_main_dryrun(mocker) -> None:
+    """
+    Test a dry run.
+    """
+    mocker.patch("senor_octopus.cli.yaml")
+    mocker.patch("senor_octopus.cli.build_dag")
+    mocker.patch("senor_octopus.cli.open")
+
+    mock_scheduler = mock.MagicMock()
+    mock_scheduler.return_value.run = mocker.AsyncMock()
+    mocker.patch("senor_octopus.cli.Scheduler", mock_scheduler)
+
+    await main(["config.yaml", "--dry-run"])
+
+    mock_scheduler.return_value.run.assert_not_called()
+
+
+@pytest.mark.asyncio
+async def test_main_canceled(mocker) -> None:
+    """
+    Test canceling the `main` function.
+    """
+    mocker.patch("senor_octopus.cli.yaml")
+    mocker.patch("senor_octopus.cli.build_dag")
+    mocker.patch("senor_octopus.cli.open")
+
+    mock_scheduler = mock.MagicMock()
+    mock_scheduler.return_value.run = mocker.AsyncMock()
+    mock_scheduler.return_value.run.side_effect = asyncio.CancelledError("Canceled")
+    mocker.patch("senor_octopus.cli.Scheduler", mock_scheduler)
+
+    await main(["config.yaml"])
+
+    mock_scheduler.return_value.cancel.assert_called()
+
+
 def test_run(mocker) -> None:
-    mock_main = CoroutineMock()
+    """
+    Test `run`.
+    """
+    mock_main = mocker.AsyncMock()
+    mocker.patch("senor_octopus.cli.main", mock_main)
+    mocker.patch("senor_octopus.cli.sys.argv", ["srocto", "config.yaml", "-vv"])
+
+    run()
+
+    mock_main.assert_called_with(["config.yaml", "-vv"])
+
+
+def test_interrupt(mocker) -> None:
+    """
+    Test interrupting `run`.
+    """
+    mock_main = mocker.AsyncMock()
+    mock_main.side_effect = KeyboardInterrupt()
     mocker.patch("senor_octopus.cli.main", mock_main)
-    mocker.patch("senor_octopus.cli.sys.argv", ["srocto", "config.ini", "-vv"])
+    mocker.patch("senor_octopus.cli.sys.argv", ["srocto", "config.yaml", "-vv"])
+    mock_logger = mocker.patch("senor_octopus.cli._logger")
 
     run()
 
-    mock_main.assert_called_with(["config.ini", "-vv"])
+    mock_logger.info.assert_called_with("Stopping Sr. Octopus")
```

### Comparing `senor-octopus-0.1.9/tests/travis_install.sh` & `senor-octopus-0.2.0/tests/travis_install.sh`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     conda create -p ./.venv  -c conda-forge --yes python=${PYTHON_VERSION} pip setuptools virtualenv tox
     conda activate ./.venv
 else
     pip install -U pip setuptools virtualenv tox
 fi
 
 if [[ "$COVERAGE" == "true" ]]; then
-    pip install -U pytest-cov pytest-virtualenv coverage coveralls flake8 pre-commit
+    pip install -U pytest-cov pytest-virtualenv coverage coveralls codecov flake8 pre-commit
 fi
 
 travis-cleanup() {
     printf "** Cleaning up environments ... "  # printf avoids new lines
     if [[ "$DISTRIB" == "conda" ]]; then
         # Force the env to be recreated next time, for build consistency
         conda deactivate
```

