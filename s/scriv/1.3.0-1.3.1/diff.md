# Comparing `tmp/scriv-1.3.0.tar.gz` & `tmp/scriv-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/nedbatchelder/scriv/dist/.tmp-ksbcjues/scriv-1.3.0.tar", last modified: Sun Apr 16 12:26:11 2023, max compression
+gzip compressed data, was "/Users/nedbatchelder/scriv/dist/.tmp-8_1s_rxv/scriv-1.3.1.tar", last modified: Sun Apr 16 13:18:06 2023, max compression
```

## Comparing `scriv-1.3.0.tar` & `scriv-1.3.1.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-04-16 12:26:11.000000 scriv-1.3.0/
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      493 2020-12-13 20:45:13.000000 scriv-1.3.0/.editorconfig
--rw-r--r--   0 nedbatchelder   (503) staff       (20)    14950 2023-04-16 12:24:12.000000 scriv-1.3.0/CHANGELOG.rst
--rw-r--r--   0 nedbatchelder   (503) staff       (20)    10177 2019-12-28 02:05:02.000000 scriv-1.3.0/LICENSE.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      331 2022-06-18 14:29:36.000000 scriv-1.3.0/MANIFEST.in
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     4947 2023-02-18 12:34:22.000000 scriv-1.3.0/Makefile
--rw-r--r--   0 nedbatchelder   (503) staff       (20)    19048 2023-04-16 12:26:11.000000 scriv-1.3.0/PKG-INFO
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     2997 2023-02-17 13:40:13.000000 scriv-1.3.0/README.rst
-drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-04-16 12:26:11.000000 scriv-1.3.0/changelog.d/
--rw-r--r--   0 nedbatchelder   (503) staff       (20)       65 2020-05-22 21:40:30.000000 scriv-1.3.0/changelog.d/README.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      182 2023-01-16 17:50:15.000000 scriv-1.3.0/changelog.d/ghrel_template.md.j2
-drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-04-16 12:26:11.000000 scriv-1.3.0/docs/
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     2024 2020-05-27 17:38:52.000000 scriv-1.3.0/docs/Makefile
-drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-04-16 12:26:11.000000 scriv-1.3.0/docs/_static/
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      334 2019-12-28 02:05:02.000000 scriv-1.3.0/docs/_static/theme_overrides.css
--rw-r--r--   0 nedbatchelder   (503) staff       (20)       30 2019-12-28 02:05:02.000000 scriv-1.3.0/docs/changelog.rst
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     8159 2023-01-18 10:44:55.000000 scriv-1.3.0/docs/commands.rst
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     1261 2020-08-29 17:11:39.000000 scriv-1.3.0/docs/concepts.rst
--rw-r--r--   0 nedbatchelder   (503) staff       (20)    13076 2023-01-16 16:40:15.000000 scriv-1.3.0/docs/conf.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     9158 2023-03-28 08:42:53.000000 scriv-1.3.0/docs/configuration.rst
-drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-04-16 12:26:11.000000 scriv-1.3.0/docs/include/
--rw-r--r--   0 nedbatchelder   (503) staff       (20)       88 2020-08-29 17:11:39.000000 scriv-1.3.0/docs/include/links.rst
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     1556 2022-06-18 14:29:36.000000 scriv-1.3.0/docs/index.rst
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     2636 2022-06-18 14:29:36.000000 scriv-1.3.0/docs/philosophy.rst
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     6343 2023-02-03 17:12:09.000000 scriv-1.3.0/pylintrc
-drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-04-16 12:26:11.000000 scriv-1.3.0/requirements/
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      106 2022-04-24 21:45:49.000000 scriv-1.3.0/requirements/base.in
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      704 2023-04-15 16:36:33.000000 scriv-1.3.0/requirements/base.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      793 2022-09-19 10:39:52.000000 scriv-1.3.0/requirements/constraints.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      336 2023-01-13 13:09:34.000000 scriv-1.3.0/requirements/dev.in
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     9269 2023-04-15 16:36:33.000000 scriv-1.3.0/requirements/dev.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      317 2022-03-23 11:43:56.000000 scriv-1.3.0/requirements/doc.in
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     3650 2023-04-15 16:36:33.000000 scriv-1.3.0/requirements/doc.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      189 2020-12-13 14:37:10.000000 scriv-1.3.0/requirements/pip-tools.in
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      659 2023-04-15 16:36:33.000000 scriv-1.3.0/requirements/pip-tools.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      719 2022-12-03 01:20:37.000000 scriv-1.3.0/requirements/quality.in
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     7753 2023-04-15 16:36:33.000000 scriv-1.3.0/requirements/quality.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      371 2022-12-03 01:20:37.000000 scriv-1.3.0/requirements/test.in
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     1988 2023-04-15 16:36:33.000000 scriv-1.3.0/requirements/test.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      194 2023-01-16 15:46:20.000000 scriv-1.3.0/requirements/tox.in
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      906 2023-04-15 16:36:33.000000 scriv-1.3.0/requirements/tox.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     2140 2023-04-16 12:26:11.000000 scriv-1.3.0/setup.cfg
--rwxr-xr-x   0 nedbatchelder   (503) staff       (20)       82 2022-12-07 12:50:29.000000 scriv-1.3.0/setup.py
-drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-04-16 12:26:11.000000 scriv-1.3.0/src/
-drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-04-16 12:26:11.000000 scriv-1.3.0/src/scriv/
--rw-r--r--   0 nedbatchelder   (503) staff       (20)       64 2023-04-16 12:23:44.000000 scriv-1.3.0/src/scriv/__init__.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)       78 2023-01-16 16:40:28.000000 scriv-1.3.0/src/scriv/__main__.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     3879 2023-01-16 14:08:01.000000 scriv-1.3.0/src/scriv/changelog.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      589 2023-01-16 14:08:01.000000 scriv-1.3.0/src/scriv/cli.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     2711 2023-04-16 12:20:46.000000 scriv-1.3.0/src/scriv/collect.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)    13820 2023-02-18 23:51:51.000000 scriv-1.3.0/src/scriv/config.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     1429 2023-01-16 14:08:01.000000 scriv-1.3.0/src/scriv/create.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      116 2023-01-16 16:35:31.000000 scriv-1.3.0/src/scriv/exceptions.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     2057 2022-11-29 12:13:06.000000 scriv-1.3.0/src/scriv/format.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     3253 2023-01-16 14:08:01.000000 scriv-1.3.0/src/scriv/format_md.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     5448 2023-01-18 12:46:04.000000 scriv-1.3.0/src/scriv/format_rst.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     3453 2023-04-16 12:20:46.000000 scriv-1.3.0/src/scriv/ghrel.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     2864 2023-01-16 14:08:01.000000 scriv-1.3.0/src/scriv/github.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     2388 2023-01-18 10:44:55.000000 scriv-1.3.0/src/scriv/gitinfo.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     3700 2023-03-28 08:36:54.000000 scriv-1.3.0/src/scriv/literals.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      494 2023-03-24 12:26:03.000000 scriv-1.3.0/src/scriv/optional.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     3524 2023-01-16 14:08:01.000000 scriv-1.3.0/src/scriv/scriv.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     1128 2023-01-16 14:08:01.000000 scriv-1.3.0/src/scriv/shell.py
-drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-04-16 12:26:11.000000 scriv-1.3.0/src/scriv/templates/
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      233 2020-08-10 09:51:42.000000 scriv-1.3.0/src/scriv/templates/new_fragment.md.j2
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      369 2020-08-10 09:51:42.000000 scriv-1.3.0/src/scriv/templates/new_fragment.rst.j2
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     2975 2023-04-16 12:20:46.000000 scriv-1.3.0/src/scriv/util.py
-drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-04-16 12:26:11.000000 scriv-1.3.0/src/scriv.egg-info/
--rw-r--r--   0 nedbatchelder   (503) staff       (20)    19048 2023-04-16 12:26:11.000000 scriv-1.3.0/src/scriv.egg-info/PKG-INFO
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     1726 2023-04-16 12:26:11.000000 scriv-1.3.0/src/scriv.egg-info/SOURCES.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)        1 2023-04-16 12:26:11.000000 scriv-1.3.0/src/scriv.egg-info/dependency_links.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)       40 2023-04-16 12:26:11.000000 scriv-1.3.0/src/scriv.egg-info/entry_points.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)       87 2023-04-16 12:26:11.000000 scriv-1.3.0/src/scriv.egg-info/requires.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)        6 2023-04-16 12:26:11.000000 scriv-1.3.0/src/scriv.egg-info/top_level.txt
-drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-04-16 12:26:11.000000 scriv-1.3.0/tests/
--rw-r--r--   0 nedbatchelder   (503) staff       (20)       27 2020-02-08 15:08:43.000000 scriv-1.3.0/tests/__init__.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     2344 2023-03-24 12:55:52.000000 scriv-1.3.0/tests/conftest.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     3923 2023-01-18 12:46:04.000000 scriv-1.3.0/tests/faker.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      558 2021-07-26 10:44:33.000000 scriv-1.3.0/tests/helpers.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     1364 2022-09-13 23:31:05.000000 scriv-1.3.0/tests/test_changelog.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)    17637 2023-04-16 12:20:46.000000 scriv-1.3.0/tests/test_collect.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)    10674 2023-02-18 23:51:51.000000 scriv-1.3.0/tests/test_config.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)    11237 2023-01-16 14:08:01.000000 scriv-1.3.0/tests/test_create.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      573 2022-04-24 21:45:49.000000 scriv-1.3.0/tests/test_faker.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     6938 2023-01-18 12:46:04.000000 scriv-1.3.0/tests/test_format_md.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     9205 2023-01-18 12:46:04.000000 scriv-1.3.0/tests/test_format_rst.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     6497 2023-01-18 10:44:55.000000 scriv-1.3.0/tests/test_ghrel.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     4110 2023-01-16 14:08:01.000000 scriv-1.3.0/tests/test_github.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     2485 2023-01-18 10:44:55.000000 scriv-1.3.0/tests/test_gitinfo.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     5046 2023-03-28 08:36:54.000000 scriv-1.3.0/tests/test_literals.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      349 2023-03-24 12:55:52.000000 scriv-1.3.0/tests/test_process.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     1975 2023-04-16 12:20:46.000000 scriv-1.3.0/tests/test_util.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     1688 2023-03-24 12:55:52.000000 scriv-1.3.0/tox.ini
+drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-04-16 13:18:06.000000 scriv-1.3.1/
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      493 2020-12-13 20:45:13.000000 scriv-1.3.1/.editorconfig
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)    15133 2023-04-16 13:17:26.000000 scriv-1.3.1/CHANGELOG.rst
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)    10177 2019-12-28 02:05:02.000000 scriv-1.3.1/LICENSE.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      331 2022-06-18 14:29:36.000000 scriv-1.3.1/MANIFEST.in
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     4947 2023-02-18 12:34:22.000000 scriv-1.3.1/Makefile
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)    19231 2023-04-16 13:18:06.000000 scriv-1.3.1/PKG-INFO
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     2997 2023-02-17 13:40:13.000000 scriv-1.3.1/README.rst
+drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-04-16 13:18:06.000000 scriv-1.3.1/changelog.d/
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)       65 2020-05-22 21:40:30.000000 scriv-1.3.1/changelog.d/README.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      182 2023-01-16 17:50:15.000000 scriv-1.3.1/changelog.d/ghrel_template.md.j2
+drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-04-16 13:18:06.000000 scriv-1.3.1/docs/
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     2024 2020-05-27 17:38:52.000000 scriv-1.3.1/docs/Makefile
+drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-04-16 13:18:06.000000 scriv-1.3.1/docs/_static/
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      334 2019-12-28 02:05:02.000000 scriv-1.3.1/docs/_static/theme_overrides.css
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)       30 2019-12-28 02:05:02.000000 scriv-1.3.1/docs/changelog.rst
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     8159 2023-01-18 10:44:55.000000 scriv-1.3.1/docs/commands.rst
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     1261 2020-08-29 17:11:39.000000 scriv-1.3.1/docs/concepts.rst
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)    13076 2023-01-16 16:40:15.000000 scriv-1.3.1/docs/conf.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     9158 2023-03-28 08:42:53.000000 scriv-1.3.1/docs/configuration.rst
+drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-04-16 13:18:06.000000 scriv-1.3.1/docs/include/
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)       88 2020-08-29 17:11:39.000000 scriv-1.3.1/docs/include/links.rst
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     1556 2022-06-18 14:29:36.000000 scriv-1.3.1/docs/index.rst
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     2636 2022-06-18 14:29:36.000000 scriv-1.3.1/docs/philosophy.rst
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     6343 2023-02-03 17:12:09.000000 scriv-1.3.1/pylintrc
+drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-04-16 13:18:06.000000 scriv-1.3.1/requirements/
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      106 2022-04-24 21:45:49.000000 scriv-1.3.1/requirements/base.in
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      704 2023-04-15 16:36:33.000000 scriv-1.3.1/requirements/base.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      793 2022-09-19 10:39:52.000000 scriv-1.3.1/requirements/constraints.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      336 2023-01-13 13:09:34.000000 scriv-1.3.1/requirements/dev.in
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     9269 2023-04-15 16:36:33.000000 scriv-1.3.1/requirements/dev.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      317 2022-03-23 11:43:56.000000 scriv-1.3.1/requirements/doc.in
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     3650 2023-04-15 16:36:33.000000 scriv-1.3.1/requirements/doc.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      189 2020-12-13 14:37:10.000000 scriv-1.3.1/requirements/pip-tools.in
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      659 2023-04-15 16:36:33.000000 scriv-1.3.1/requirements/pip-tools.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      719 2022-12-03 01:20:37.000000 scriv-1.3.1/requirements/quality.in
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     7753 2023-04-15 16:36:33.000000 scriv-1.3.1/requirements/quality.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      371 2022-12-03 01:20:37.000000 scriv-1.3.1/requirements/test.in
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     1988 2023-04-15 16:36:33.000000 scriv-1.3.1/requirements/test.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      194 2023-01-16 15:46:20.000000 scriv-1.3.1/requirements/tox.in
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      906 2023-04-15 16:36:33.000000 scriv-1.3.1/requirements/tox.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     2140 2023-04-16 13:18:06.000000 scriv-1.3.1/setup.cfg
+-rwxr-xr-x   0 nedbatchelder   (503) staff       (20)       82 2022-12-07 12:50:29.000000 scriv-1.3.1/setup.py
+drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-04-16 13:18:06.000000 scriv-1.3.1/src/
+drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-04-16 13:18:06.000000 scriv-1.3.1/src/scriv/
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)       64 2023-04-16 13:17:17.000000 scriv-1.3.1/src/scriv/__init__.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)       78 2023-01-16 16:40:28.000000 scriv-1.3.1/src/scriv/__main__.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     3879 2023-01-16 14:08:01.000000 scriv-1.3.1/src/scriv/changelog.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      589 2023-01-16 14:08:01.000000 scriv-1.3.1/src/scriv/cli.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     2711 2023-04-16 12:20:46.000000 scriv-1.3.1/src/scriv/collect.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)    13820 2023-02-18 23:51:51.000000 scriv-1.3.1/src/scriv/config.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     1429 2023-01-16 14:08:01.000000 scriv-1.3.1/src/scriv/create.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      116 2023-01-16 16:35:31.000000 scriv-1.3.1/src/scriv/exceptions.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     2057 2022-11-29 12:13:06.000000 scriv-1.3.1/src/scriv/format.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     3253 2023-01-16 14:08:01.000000 scriv-1.3.1/src/scriv/format_md.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     5448 2023-01-18 12:46:04.000000 scriv-1.3.1/src/scriv/format_rst.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     3463 2023-04-16 13:09:18.000000 scriv-1.3.1/src/scriv/ghrel.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     2864 2023-01-16 14:08:01.000000 scriv-1.3.1/src/scriv/github.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     2388 2023-01-18 10:44:55.000000 scriv-1.3.1/src/scriv/gitinfo.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     3700 2023-03-28 08:36:54.000000 scriv-1.3.1/src/scriv/literals.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      494 2023-03-24 12:26:03.000000 scriv-1.3.1/src/scriv/optional.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     3524 2023-01-16 14:08:01.000000 scriv-1.3.1/src/scriv/scriv.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     1128 2023-01-16 14:08:01.000000 scriv-1.3.1/src/scriv/shell.py
+drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-04-16 13:18:06.000000 scriv-1.3.1/src/scriv/templates/
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      233 2020-08-10 09:51:42.000000 scriv-1.3.1/src/scriv/templates/new_fragment.md.j2
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      369 2020-08-10 09:51:42.000000 scriv-1.3.1/src/scriv/templates/new_fragment.rst.j2
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     2975 2023-04-16 12:20:46.000000 scriv-1.3.1/src/scriv/util.py
+drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-04-16 13:18:06.000000 scriv-1.3.1/src/scriv.egg-info/
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)    19231 2023-04-16 13:18:06.000000 scriv-1.3.1/src/scriv.egg-info/PKG-INFO
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     1726 2023-04-16 13:18:06.000000 scriv-1.3.1/src/scriv.egg-info/SOURCES.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)        1 2023-04-16 13:18:06.000000 scriv-1.3.1/src/scriv.egg-info/dependency_links.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)       40 2023-04-16 13:18:06.000000 scriv-1.3.1/src/scriv.egg-info/entry_points.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)       87 2023-04-16 13:18:06.000000 scriv-1.3.1/src/scriv.egg-info/requires.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)        6 2023-04-16 13:18:06.000000 scriv-1.3.1/src/scriv.egg-info/top_level.txt
+drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-04-16 13:18:06.000000 scriv-1.3.1/tests/
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)       27 2020-02-08 15:08:43.000000 scriv-1.3.1/tests/__init__.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     2344 2023-03-24 12:55:52.000000 scriv-1.3.1/tests/conftest.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     3923 2023-01-18 12:46:04.000000 scriv-1.3.1/tests/faker.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      558 2021-07-26 10:44:33.000000 scriv-1.3.1/tests/helpers.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     1364 2022-09-13 23:31:05.000000 scriv-1.3.1/tests/test_changelog.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)    17637 2023-04-16 12:20:46.000000 scriv-1.3.1/tests/test_collect.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)    10674 2023-02-18 23:51:51.000000 scriv-1.3.1/tests/test_config.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)    11237 2023-01-16 14:08:01.000000 scriv-1.3.1/tests/test_create.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      573 2022-04-24 21:45:49.000000 scriv-1.3.1/tests/test_faker.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     6938 2023-01-18 12:46:04.000000 scriv-1.3.1/tests/test_format_md.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     9205 2023-01-18 12:46:04.000000 scriv-1.3.1/tests/test_format_rst.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     6906 2023-04-16 13:08:38.000000 scriv-1.3.1/tests/test_ghrel.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     4110 2023-01-16 14:08:01.000000 scriv-1.3.1/tests/test_github.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     2485 2023-01-18 10:44:55.000000 scriv-1.3.1/tests/test_gitinfo.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     5046 2023-03-28 08:36:54.000000 scriv-1.3.1/tests/test_literals.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      349 2023-03-24 12:55:52.000000 scriv-1.3.1/tests/test_process.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     1975 2023-04-16 12:20:46.000000 scriv-1.3.1/tests/test_util.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     1688 2023-03-24 12:55:52.000000 scriv-1.3.1/tox.ini
```

### Comparing `scriv-1.3.0/CHANGELOG.rst` & `scriv-1.3.1/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,25 @@
 See the fragment files in the `changelog.d directory`_.
 
 .. _changelog.d directory: https://github.com/nedbat/scriv/tree/master/changelog.d
 
 
 .. scriv-insert-here
 
+.. _changelog-1.3.1:
+
+1.3.1 — 2023-04-16
+------------------
+
+Fixed
+.....
+
+- The Version class introduced in 1.3.0 broke the ``scriv github-release``
+  command.  This is now fixed.
+
 .. _changelog-1.3.0:
 
 1.3.0 — 2023-04-16
 ------------------
 
 Added
 .....
```

### Comparing `scriv-1.3.0/LICENSE.txt` & `scriv-1.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scriv-1.3.0/Makefile` & `scriv-1.3.1/Makefile`

 * *Files identical despite different names*

### Comparing `scriv-1.3.0/PKG-INFO` & `scriv-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scriv
-Version: 1.3.0
+Version: 1.3.1
 Summary: Scriv changelog management tool
 Home-page: https://github.com/nedbat/scriv
 Author: Ned Batchelder
 Author-email: ned@nedbatchelder.com
 License: Apache-2.0
 Project-URL: Mastodon, https://hachyderm.io/@nedbat
 Project-URL: Funding, https://github.com/sponsors/nedbat
@@ -128,14 +128,25 @@
 See the fragment files in the `changelog.d directory`_.
 
 .. _changelog.d directory: https://github.com/nedbat/scriv/tree/master/changelog.d
 
 
 .. scriv-insert-here
 
+.. _changelog-1.3.1:
+
+1.3.1 — 2023-04-16
+------------------
+
+Fixed
+.....
+
+- The Version class introduced in 1.3.0 broke the ``scriv github-release``
+  command.  This is now fixed.
+
 .. _changelog-1.3.0:
 
 1.3.0 — 2023-04-16
 ------------------
 
 Added
 .....
```

### Comparing `scriv-1.3.0/README.rst` & `scriv-1.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `scriv-1.3.0/docs/Makefile` & `scriv-1.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `scriv-1.3.0/docs/commands.rst` & `scriv-1.3.1/docs/commands.rst`

 * *Files identical despite different names*

### Comparing `scriv-1.3.0/docs/concepts.rst` & `scriv-1.3.1/docs/concepts.rst`

 * *Files identical despite different names*

### Comparing `scriv-1.3.0/docs/conf.py` & `scriv-1.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `scriv-1.3.0/docs/configuration.rst` & `scriv-1.3.1/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `scriv-1.3.0/docs/index.rst` & `scriv-1.3.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `scriv-1.3.0/docs/philosophy.rst` & `scriv-1.3.1/docs/philosophy.rst`

 * *Files identical despite different names*

### Comparing `scriv-1.3.0/pylintrc` & `scriv-1.3.1/pylintrc`

 * *Files identical despite different names*

### Comparing `scriv-1.3.0/requirements/base.txt` & `scriv-1.3.1/requirements/base.txt`

 * *Files identical despite different names*

### Comparing `scriv-1.3.0/requirements/constraints.txt` & `scriv-1.3.1/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `scriv-1.3.0/requirements/dev.txt` & `scriv-1.3.1/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `scriv-1.3.0/requirements/doc.txt` & `scriv-1.3.1/requirements/doc.txt`

 * *Files identical despite different names*

### Comparing `scriv-1.3.0/requirements/pip-tools.txt` & `scriv-1.3.1/requirements/pip-tools.txt`

 * *Files identical despite different names*

### Comparing `scriv-1.3.0/requirements/quality.in` & `scriv-1.3.1/requirements/quality.in`

 * *Files identical despite different names*

### Comparing `scriv-1.3.0/requirements/quality.txt` & `scriv-1.3.1/requirements/quality.txt`

 * *Files identical despite different names*

### Comparing `scriv-1.3.0/requirements/test.txt` & `scriv-1.3.1/requirements/test.txt`

 * *Files identical despite different names*

### Comparing `scriv-1.3.0/requirements/tox.txt` & `scriv-1.3.1/requirements/tox.txt`

 * *Files identical despite different names*

### Comparing `scriv-1.3.0/setup.cfg` & `scriv-1.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `scriv-1.3.0/src/scriv/changelog.py` & `scriv-1.3.1/src/scriv/changelog.py`

 * *Files identical despite different names*

### Comparing `scriv-1.3.0/src/scriv/cli.py` & `scriv-1.3.1/src/scriv/cli.py`

 * *Files identical despite different names*

### Comparing `scriv-1.3.0/src/scriv/collect.py` & `scriv-1.3.1/src/scriv/collect.py`

 * *Files identical despite different names*

### Comparing `scriv-1.3.0/src/scriv/config.py` & `scriv-1.3.1/src/scriv/config.py`

 * *Files identical despite different names*

### Comparing `scriv-1.3.0/src/scriv/create.py` & `scriv-1.3.1/src/scriv/create.py`

 * *Files identical despite different names*

### Comparing `scriv-1.3.0/src/scriv/format.py` & `scriv-1.3.1/src/scriv/format.py`

 * *Files identical despite different names*

### Comparing `scriv-1.3.0/src/scriv/format_md.py` & `scriv-1.3.1/src/scriv/format_md.py`

 * *Files identical despite different names*

### Comparing `scriv-1.3.0/src/scriv/format_rst.py` & `scriv-1.3.1/src/scriv/format_rst.py`

 * *Files identical despite different names*

### Comparing `scriv-1.3.0/src/scriv/ghrel.py` & `scriv-1.3.1/src/scriv/ghrel.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,16 +81,16 @@
             continue
 
         section_text = "\n\n".join(sections)
         md = changelog.format_tools().convert_to_markdown(section_text)
 
         release_data = {
             "body": md,
-            "name": version,
-            "tag_name": version,
+            "name": str(version),
+            "tag_name": str(version),
             "draft": False,
             "prerelease": version.is_prerelease(),
         }
 
         ghrel_template = jinja2.Template(scriv.config.ghrel_template)
         md = ghrel_template.render(
             body=md,
```

### Comparing `scriv-1.3.0/src/scriv/github.py` & `scriv-1.3.1/src/scriv/github.py`

 * *Files identical despite different names*

### Comparing `scriv-1.3.0/src/scriv/gitinfo.py` & `scriv-1.3.1/src/scriv/gitinfo.py`

 * *Files identical despite different names*

### Comparing `scriv-1.3.0/src/scriv/literals.py` & `scriv-1.3.1/src/scriv/literals.py`

 * *Files identical despite different names*

### Comparing `scriv-1.3.0/src/scriv/scriv.py` & `scriv-1.3.1/src/scriv/scriv.py`

 * *Files identical despite different names*

### Comparing `scriv-1.3.0/src/scriv/shell.py` & `scriv-1.3.1/src/scriv/shell.py`

 * *Files identical despite different names*

### Comparing `scriv-1.3.0/src/scriv/util.py` & `scriv-1.3.1/src/scriv/util.py`

 * *Files identical despite different names*

### Comparing `scriv-1.3.0/src/scriv.egg-info/PKG-INFO` & `scriv-1.3.1/src/scriv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scriv
-Version: 1.3.0
+Version: 1.3.1
 Summary: Scriv changelog management tool
 Home-page: https://github.com/nedbat/scriv
 Author: Ned Batchelder
 Author-email: ned@nedbatchelder.com
 License: Apache-2.0
 Project-URL: Mastodon, https://hachyderm.io/@nedbat
 Project-URL: Funding, https://github.com/sponsors/nedbat
@@ -128,14 +128,25 @@
 See the fragment files in the `changelog.d directory`_.
 
 .. _changelog.d directory: https://github.com/nedbat/scriv/tree/master/changelog.d
 
 
 .. scriv-insert-here
 
+.. _changelog-1.3.1:
+
+1.3.1 — 2023-04-16
+------------------
+
+Fixed
+.....
+
+- The Version class introduced in 1.3.0 broke the ``scriv github-release``
+  command.  This is now fixed.
+
 .. _changelog-1.3.0:
 
 1.3.0 — 2023-04-16
 ------------------
 
 Added
 .....
```

### Comparing `scriv-1.3.0/src/scriv.egg-info/SOURCES.txt` & `scriv-1.3.1/src/scriv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scriv-1.3.0/tests/conftest.py` & `scriv-1.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `scriv-1.3.0/tests/faker.py` & `scriv-1.3.1/tests/faker.py`

 * *Files identical despite different names*

### Comparing `scriv-1.3.0/tests/helpers.py` & `scriv-1.3.1/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `scriv-1.3.0/tests/test_changelog.py` & `scriv-1.3.1/tests/test_changelog.py`

 * *Files identical despite different names*

### Comparing `scriv-1.3.0/tests/test_collect.py` & `scriv-1.3.1/tests/test_collect.py`

 * *Files identical despite different names*

### Comparing `scriv-1.3.0/tests/test_config.py` & `scriv-1.3.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `scriv-1.3.0/tests/test_create.py` & `scriv-1.3.1/tests/test_create.py`

 * *Files identical despite different names*

### Comparing `scriv-1.3.0/tests/test_faker.py` & `scriv-1.3.1/tests/test_faker.py`

 * *Files identical despite different names*

### Comparing `scriv-1.3.0/tests/test_format_md.py` & `scriv-1.3.1/tests/test_format_md.py`

 * *Files identical despite different names*

### Comparing `scriv-1.3.0/tests/test_format_rst.py` & `scriv-1.3.1/tests/test_format_rst.py`

 * *Files identical despite different names*

### Comparing `scriv-1.3.0/tests/test_ghrel.py` & `scriv-1.3.1/tests/test_ghrel.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """Tests of scriv/ghrel.py."""
 
+import json
 import logging
+from typing import Any, Dict
 from unittest.mock import call
 
 import pytest
 
 CHANGELOG1 = """\
 Some text before
 
@@ -68,35 +70,63 @@
     fake_git.add_remote("origin", "git@github.com:joe/project.git")
     fake_git.add_tags(["v1.2.3", "v1.0", "v0.9a7"])
     (temp_dir / "CHANGELOG.rst").write_text(CHANGELOG1)
     mock_get_releases = mocker.patch("scriv.ghrel.get_releases")
     mock_get_releases.return_value = RELEASES1
 
 
-def test_default(cli_invoke, scenario1, mocker, caplog):
-    mock_create_release = mocker.patch("scriv.ghrel.create_release")
-    mock_update_release = mocker.patch("scriv.ghrel.update_release")
+@pytest.fixture()
+def mock_create_release(mocker):
+    """Create a mock create_release that checks arguments."""
+
+    def _create_release(repo: str, release_data: Dict[str, Any]) -> None:
+        assert repo
+        assert release_data["name"]
+        assert json.dumps(release_data)[0] == "{"
+
+    return mocker.patch(
+        "scriv.ghrel.create_release", side_effect=_create_release
+    )
+
+
+@pytest.fixture()
+def mock_update_release(mocker):
+    """Create a mock update_release that checks arguments."""
 
+    def _update_release(
+        release: Dict[str, Any], release_data: Dict[str, Any]
+    ) -> None:
+        assert release_data["name"]
+        assert release["url"]
+        assert json.dumps(release_data)[0] == "{"
+
+    return mocker.patch(
+        "scriv.ghrel.update_release", side_effect=_update_release
+    )
+
+
+def test_default(
+    cli_invoke, scenario1, mock_create_release, mock_update_release, caplog
+):
     cli_invoke(["github-release"])
 
     assert mock_create_release.mock_calls == [call("joe/project", V123_REL)]
     assert mock_update_release.mock_calls == []
     assert caplog.record_tuples == [
         (
             "scriv.changelog",
             logging.INFO,
             "Reading changelog CHANGELOG.rst",
         ),
     ]
 
 
-def test_dash_all(cli_invoke, scenario1, mocker, caplog):
-    mock_create_release = mocker.patch("scriv.ghrel.create_release")
-    mock_update_release = mocker.patch("scriv.ghrel.update_release")
-
+def test_dash_all(
+    cli_invoke, scenario1, mock_create_release, mock_update_release, caplog
+):
     cli_invoke(["github-release", "--all"])
 
     assert mock_create_release.mock_calls == [call("joe/project", V123_REL)]
     assert mock_update_release.mock_calls == [
         call(RELEASES1["v0.9a7"], V097_REL),
     ]
     assert caplog.record_tuples == [
@@ -114,21 +144,20 @@
             "scriv.ghrel",
             logging.WARNING,
             "Version v0.0.1 has no tag. No release will be made.",
         ),
     ]
 
 
-def test_explicit_repo(cli_invoke, scenario1, fake_git, mocker):
+def test_explicit_repo(
+    cli_invoke, scenario1, fake_git, mock_create_release, mock_update_release
+):
     # Add another GitHub remote, now there are two.
     fake_git.add_remote("upstream", "git@github.com:psf/project.git")
 
-    mock_create_release = mocker.patch("scriv.ghrel.create_release")
-    mock_update_release = mocker.patch("scriv.ghrel.update_release")
-
     cli_invoke(["github-release", "--repo=xyzzy/plugh"])
 
     assert mock_create_release.mock_calls == [call("xyzzy/plugh", V123_REL)]
     assert mock_update_release.mock_calls == []
 
 
 @pytest.mark.parametrize(
@@ -137,18 +166,16 @@
 def test_bad_explicit_repo(cli_invoke, repo):
     result = cli_invoke(["github-release", f"--repo={repo}"], expect_ok=False)
     assert result.exit_code == 1
     assert str(result.exception) == f"Repo must be owner/reponame: {repo!r}"
 
 
 @pytest.fixture()
-def no_actions(mocker, responses):
+def no_actions(mock_create_release, mock_update_release, responses):
     """Check that nothing really happened."""
-    mock_create_release = mocker.patch("scriv.ghrel.create_release")
-    mock_update_release = mocker.patch("scriv.ghrel.update_release")
 
     yield
 
     assert mock_create_release.mock_calls == []
     assert mock_update_release.mock_calls == []
     assert len(responses.calls) == 0
 
@@ -207,22 +234,20 @@
     assert result.exit_code == 1
     assert result.output == (
         "Reading changelog CHANGELOG.rst\n"
         + "More than one GitHub repo found: joe/project, psf/project\n"
     )
 
 
-def test_with_template(cli_invoke, temp_dir, scenario1, mocker):
+def test_with_template(cli_invoke, temp_dir, scenario1, mock_create_release):
     (temp_dir / "setup.cfg").write_text(
         """
         [scriv]
         ghrel_template = |{{body}}|{{config.format}}|{{version}}
         """
     )
-    mock_create_release = mocker.patch("scriv.ghrel.create_release")
-
     cli_invoke(["github-release"])
 
     expected = dict(V123_REL)
     expected["body"] = "|A good release\n|rst|v1.2.3"
 
     assert mock_create_release.mock_calls == [call("joe/project", expected)]
```

### Comparing `scriv-1.3.0/tests/test_github.py` & `scriv-1.3.1/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `scriv-1.3.0/tests/test_gitinfo.py` & `scriv-1.3.1/tests/test_gitinfo.py`

 * *Files identical despite different names*

### Comparing `scriv-1.3.0/tests/test_literals.py` & `scriv-1.3.1/tests/test_literals.py`

 * *Files identical despite different names*

### Comparing `scriv-1.3.0/tests/test_util.py` & `scriv-1.3.1/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `scriv-1.3.0/tox.ini` & `scriv-1.3.1/tox.ini`

 * *Files identical despite different names*

