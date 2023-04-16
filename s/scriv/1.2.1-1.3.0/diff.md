# Comparing `tmp/scriv-1.2.1.tar.gz` & `tmp/scriv-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/nedbatchelder/scriv/dist/.tmp-d1q66d6k/scriv-1.2.1.tar", last modified: Sun Feb 19 00:15:06 2023, max compression
+gzip compressed data, was "/Users/nedbatchelder/scriv/dist/.tmp-ksbcjues/scriv-1.3.0.tar", last modified: Sun Apr 16 12:26:11 2023, max compression
```

## Comparing `scriv-1.2.1.tar` & `scriv-1.3.0.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-02-19 00:15:06.000000 scriv-1.2.1/
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      493 2020-12-13 20:45:13.000000 scriv-1.2.1/.editorconfig
--rw-r--r--   0 nedbatchelder   (503) staff       (20)    14330 2023-02-19 00:14:09.000000 scriv-1.2.1/CHANGELOG.rst
--rw-r--r--   0 nedbatchelder   (503) staff       (20)    10177 2019-12-28 02:05:02.000000 scriv-1.2.1/LICENSE.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      331 2022-06-18 14:29:36.000000 scriv-1.2.1/MANIFEST.in
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     4947 2023-02-18 12:34:22.000000 scriv-1.2.1/Makefile
--rw-r--r--   0 nedbatchelder   (503) staff       (20)    18428 2023-02-19 00:15:06.000000 scriv-1.2.1/PKG-INFO
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     2997 2023-02-17 13:40:13.000000 scriv-1.2.1/README.rst
-drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-02-19 00:15:06.000000 scriv-1.2.1/changelog.d/
--rw-r--r--   0 nedbatchelder   (503) staff       (20)       65 2020-05-22 21:40:30.000000 scriv-1.2.1/changelog.d/README.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      182 2023-01-16 17:50:15.000000 scriv-1.2.1/changelog.d/ghrel_template.md.j2
-drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-02-19 00:15:06.000000 scriv-1.2.1/docs/
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     2024 2020-05-27 17:38:52.000000 scriv-1.2.1/docs/Makefile
-drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-02-19 00:15:06.000000 scriv-1.2.1/docs/_static/
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      334 2019-12-28 02:05:02.000000 scriv-1.2.1/docs/_static/theme_overrides.css
--rw-r--r--   0 nedbatchelder   (503) staff       (20)       30 2019-12-28 02:05:02.000000 scriv-1.2.1/docs/changelog.rst
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     8159 2023-01-18 10:44:55.000000 scriv-1.2.1/docs/commands.rst
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     1261 2020-08-29 17:11:39.000000 scriv-1.2.1/docs/concepts.rst
--rw-r--r--   0 nedbatchelder   (503) staff       (20)    13076 2023-01-16 16:40:15.000000 scriv-1.2.1/docs/conf.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     9152 2023-02-18 23:51:51.000000 scriv-1.2.1/docs/configuration.rst
-drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-02-19 00:15:06.000000 scriv-1.2.1/docs/include/
--rw-r--r--   0 nedbatchelder   (503) staff       (20)       88 2020-08-29 17:11:39.000000 scriv-1.2.1/docs/include/links.rst
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     1556 2022-06-18 14:29:36.000000 scriv-1.2.1/docs/index.rst
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     2636 2022-06-18 14:29:36.000000 scriv-1.2.1/docs/philosophy.rst
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     6343 2023-02-03 17:12:09.000000 scriv-1.2.1/pylintrc
-drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-02-19 00:15:06.000000 scriv-1.2.1/requirements/
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      106 2022-04-24 21:45:49.000000 scriv-1.2.1/requirements/base.in
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      704 2023-02-03 16:04:16.000000 scriv-1.2.1/requirements/base.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      793 2022-09-19 10:39:52.000000 scriv-1.2.1/requirements/constraints.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      336 2023-01-13 13:09:34.000000 scriv-1.2.1/requirements/dev.in
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     9215 2023-02-03 16:05:04.000000 scriv-1.2.1/requirements/dev.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      317 2022-03-23 11:43:56.000000 scriv-1.2.1/requirements/doc.in
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     3639 2023-02-03 16:04:30.000000 scriv-1.2.1/requirements/doc.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      189 2020-12-13 14:37:10.000000 scriv-1.2.1/requirements/pip-tools.in
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      659 2023-02-03 16:04:13.000000 scriv-1.2.1/requirements/pip-tools.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      719 2022-12-03 01:20:37.000000 scriv-1.2.1/requirements/quality.in
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     7734 2023-02-03 16:04:45.000000 scriv-1.2.1/requirements/quality.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      371 2022-12-03 01:20:37.000000 scriv-1.2.1/requirements/test.in
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     2016 2023-02-03 16:04:23.000000 scriv-1.2.1/requirements/test.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      194 2023-01-16 15:46:20.000000 scriv-1.2.1/requirements/tox.in
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      904 2023-02-03 16:04:48.000000 scriv-1.2.1/requirements/tox.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     2135 2023-02-19 00:15:06.000000 scriv-1.2.1/setup.cfg
--rwxr-xr-x   0 nedbatchelder   (503) staff       (20)       82 2022-12-07 12:50:29.000000 scriv-1.2.1/setup.py
-drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-02-19 00:15:06.000000 scriv-1.2.1/src/
-drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-02-19 00:15:06.000000 scriv-1.2.1/src/scriv/
--rw-r--r--   0 nedbatchelder   (503) staff       (20)       64 2023-02-19 00:12:33.000000 scriv-1.2.1/src/scriv/__init__.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)       78 2023-01-16 16:40:28.000000 scriv-1.2.1/src/scriv/__main__.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     3879 2023-01-16 14:08:01.000000 scriv-1.2.1/src/scriv/changelog.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      589 2023-01-16 14:08:01.000000 scriv-1.2.1/src/scriv/cli.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     2673 2023-01-18 11:41:57.000000 scriv-1.2.1/src/scriv/collect.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)    13820 2023-02-18 23:51:51.000000 scriv-1.2.1/src/scriv/config.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     1429 2023-01-16 14:08:01.000000 scriv-1.2.1/src/scriv/create.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      116 2023-01-16 16:35:31.000000 scriv-1.2.1/src/scriv/exceptions.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     2057 2022-11-29 12:13:06.000000 scriv-1.2.1/src/scriv/format.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     3253 2023-01-16 14:08:01.000000 scriv-1.2.1/src/scriv/format_md.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     5448 2023-01-18 12:46:04.000000 scriv-1.2.1/src/scriv/format_rst.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     3567 2023-01-18 10:44:55.000000 scriv-1.2.1/src/scriv/ghrel.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     2864 2023-01-16 14:08:01.000000 scriv-1.2.1/src/scriv/github.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     2388 2023-01-18 10:44:55.000000 scriv-1.2.1/src/scriv/gitinfo.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     3513 2023-02-19 00:03:12.000000 scriv-1.2.1/src/scriv/literals.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      494 2023-02-18 12:34:22.000000 scriv-1.2.1/src/scriv/optional.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     3524 2023-01-16 14:08:01.000000 scriv-1.2.1/src/scriv/scriv.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     1128 2023-01-16 14:08:01.000000 scriv-1.2.1/src/scriv/shell.py
-drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-02-19 00:15:06.000000 scriv-1.2.1/src/scriv/templates/
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      233 2020-08-10 09:51:42.000000 scriv-1.2.1/src/scriv/templates/new_fragment.md.j2
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      369 2020-08-10 09:51:42.000000 scriv-1.2.1/src/scriv/templates/new_fragment.rst.j2
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     2144 2022-09-11 23:44:19.000000 scriv-1.2.1/src/scriv/util.py
-drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-02-19 00:15:06.000000 scriv-1.2.1/src/scriv.egg-info/
--rw-r--r--   0 nedbatchelder   (503) staff       (20)    18428 2023-02-19 00:15:06.000000 scriv-1.2.1/src/scriv.egg-info/PKG-INFO
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     1726 2023-02-19 00:15:06.000000 scriv-1.2.1/src/scriv.egg-info/SOURCES.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)        1 2023-02-19 00:15:06.000000 scriv-1.2.1/src/scriv.egg-info/dependency_links.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)       40 2023-02-19 00:15:06.000000 scriv-1.2.1/src/scriv.egg-info/entry_points.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)       87 2023-02-19 00:15:06.000000 scriv-1.2.1/src/scriv.egg-info/requires.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)        6 2023-02-19 00:15:06.000000 scriv-1.2.1/src/scriv.egg-info/top_level.txt
-drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-02-19 00:15:06.000000 scriv-1.2.1/tests/
--rw-r--r--   0 nedbatchelder   (503) staff       (20)       27 2020-02-08 15:08:43.000000 scriv-1.2.1/tests/__init__.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     1855 2022-04-24 21:45:49.000000 scriv-1.2.1/tests/conftest.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     3923 2023-01-18 12:46:04.000000 scriv-1.2.1/tests/faker.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      558 2021-07-26 10:44:33.000000 scriv-1.2.1/tests/helpers.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     1364 2022-09-13 23:31:05.000000 scriv-1.2.1/tests/test_changelog.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)    16696 2023-01-18 12:46:03.000000 scriv-1.2.1/tests/test_collect.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)    10674 2023-02-18 23:51:51.000000 scriv-1.2.1/tests/test_config.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)    11237 2023-01-16 14:08:01.000000 scriv-1.2.1/tests/test_create.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      573 2022-04-24 21:45:49.000000 scriv-1.2.1/tests/test_faker.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     6938 2023-01-18 12:46:04.000000 scriv-1.2.1/tests/test_format_md.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     9205 2023-01-18 12:46:04.000000 scriv-1.2.1/tests/test_format_rst.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     6497 2023-01-18 10:44:55.000000 scriv-1.2.1/tests/test_ghrel.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     4110 2023-01-16 14:08:01.000000 scriv-1.2.1/tests/test_github.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     2485 2023-01-18 10:44:55.000000 scriv-1.2.1/tests/test_gitinfo.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     3694 2023-02-18 23:56:21.000000 scriv-1.2.1/tests/test_literals.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      331 2020-08-31 18:41:11.000000 scriv-1.2.1/tests/test_process.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     1299 2022-09-11 23:31:27.000000 scriv-1.2.1/tests/test_util.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     1648 2023-02-18 12:34:22.000000 scriv-1.2.1/tox.ini
+drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-04-16 12:26:11.000000 scriv-1.3.0/
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      493 2020-12-13 20:45:13.000000 scriv-1.3.0/.editorconfig
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)    14950 2023-04-16 12:24:12.000000 scriv-1.3.0/CHANGELOG.rst
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)    10177 2019-12-28 02:05:02.000000 scriv-1.3.0/LICENSE.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      331 2022-06-18 14:29:36.000000 scriv-1.3.0/MANIFEST.in
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     4947 2023-02-18 12:34:22.000000 scriv-1.3.0/Makefile
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)    19048 2023-04-16 12:26:11.000000 scriv-1.3.0/PKG-INFO
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     2997 2023-02-17 13:40:13.000000 scriv-1.3.0/README.rst
+drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-04-16 12:26:11.000000 scriv-1.3.0/changelog.d/
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)       65 2020-05-22 21:40:30.000000 scriv-1.3.0/changelog.d/README.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      182 2023-01-16 17:50:15.000000 scriv-1.3.0/changelog.d/ghrel_template.md.j2
+drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-04-16 12:26:11.000000 scriv-1.3.0/docs/
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     2024 2020-05-27 17:38:52.000000 scriv-1.3.0/docs/Makefile
+drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-04-16 12:26:11.000000 scriv-1.3.0/docs/_static/
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      334 2019-12-28 02:05:02.000000 scriv-1.3.0/docs/_static/theme_overrides.css
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)       30 2019-12-28 02:05:02.000000 scriv-1.3.0/docs/changelog.rst
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     8159 2023-01-18 10:44:55.000000 scriv-1.3.0/docs/commands.rst
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     1261 2020-08-29 17:11:39.000000 scriv-1.3.0/docs/concepts.rst
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)    13076 2023-01-16 16:40:15.000000 scriv-1.3.0/docs/conf.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     9158 2023-03-28 08:42:53.000000 scriv-1.3.0/docs/configuration.rst
+drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-04-16 12:26:11.000000 scriv-1.3.0/docs/include/
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)       88 2020-08-29 17:11:39.000000 scriv-1.3.0/docs/include/links.rst
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     1556 2022-06-18 14:29:36.000000 scriv-1.3.0/docs/index.rst
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     2636 2022-06-18 14:29:36.000000 scriv-1.3.0/docs/philosophy.rst
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     6343 2023-02-03 17:12:09.000000 scriv-1.3.0/pylintrc
+drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-04-16 12:26:11.000000 scriv-1.3.0/requirements/
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      106 2022-04-24 21:45:49.000000 scriv-1.3.0/requirements/base.in
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      704 2023-04-15 16:36:33.000000 scriv-1.3.0/requirements/base.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      793 2022-09-19 10:39:52.000000 scriv-1.3.0/requirements/constraints.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      336 2023-01-13 13:09:34.000000 scriv-1.3.0/requirements/dev.in
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     9269 2023-04-15 16:36:33.000000 scriv-1.3.0/requirements/dev.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      317 2022-03-23 11:43:56.000000 scriv-1.3.0/requirements/doc.in
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     3650 2023-04-15 16:36:33.000000 scriv-1.3.0/requirements/doc.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      189 2020-12-13 14:37:10.000000 scriv-1.3.0/requirements/pip-tools.in
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      659 2023-04-15 16:36:33.000000 scriv-1.3.0/requirements/pip-tools.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      719 2022-12-03 01:20:37.000000 scriv-1.3.0/requirements/quality.in
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     7753 2023-04-15 16:36:33.000000 scriv-1.3.0/requirements/quality.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      371 2022-12-03 01:20:37.000000 scriv-1.3.0/requirements/test.in
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     1988 2023-04-15 16:36:33.000000 scriv-1.3.0/requirements/test.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      194 2023-01-16 15:46:20.000000 scriv-1.3.0/requirements/tox.in
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      906 2023-04-15 16:36:33.000000 scriv-1.3.0/requirements/tox.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     2140 2023-04-16 12:26:11.000000 scriv-1.3.0/setup.cfg
+-rwxr-xr-x   0 nedbatchelder   (503) staff       (20)       82 2022-12-07 12:50:29.000000 scriv-1.3.0/setup.py
+drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-04-16 12:26:11.000000 scriv-1.3.0/src/
+drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-04-16 12:26:11.000000 scriv-1.3.0/src/scriv/
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)       64 2023-04-16 12:23:44.000000 scriv-1.3.0/src/scriv/__init__.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)       78 2023-01-16 16:40:28.000000 scriv-1.3.0/src/scriv/__main__.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     3879 2023-01-16 14:08:01.000000 scriv-1.3.0/src/scriv/changelog.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      589 2023-01-16 14:08:01.000000 scriv-1.3.0/src/scriv/cli.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     2711 2023-04-16 12:20:46.000000 scriv-1.3.0/src/scriv/collect.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)    13820 2023-02-18 23:51:51.000000 scriv-1.3.0/src/scriv/config.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     1429 2023-01-16 14:08:01.000000 scriv-1.3.0/src/scriv/create.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      116 2023-01-16 16:35:31.000000 scriv-1.3.0/src/scriv/exceptions.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     2057 2022-11-29 12:13:06.000000 scriv-1.3.0/src/scriv/format.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     3253 2023-01-16 14:08:01.000000 scriv-1.3.0/src/scriv/format_md.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     5448 2023-01-18 12:46:04.000000 scriv-1.3.0/src/scriv/format_rst.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     3453 2023-04-16 12:20:46.000000 scriv-1.3.0/src/scriv/ghrel.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     2864 2023-01-16 14:08:01.000000 scriv-1.3.0/src/scriv/github.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     2388 2023-01-18 10:44:55.000000 scriv-1.3.0/src/scriv/gitinfo.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     3700 2023-03-28 08:36:54.000000 scriv-1.3.0/src/scriv/literals.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      494 2023-03-24 12:26:03.000000 scriv-1.3.0/src/scriv/optional.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     3524 2023-01-16 14:08:01.000000 scriv-1.3.0/src/scriv/scriv.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     1128 2023-01-16 14:08:01.000000 scriv-1.3.0/src/scriv/shell.py
+drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-04-16 12:26:11.000000 scriv-1.3.0/src/scriv/templates/
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      233 2020-08-10 09:51:42.000000 scriv-1.3.0/src/scriv/templates/new_fragment.md.j2
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      369 2020-08-10 09:51:42.000000 scriv-1.3.0/src/scriv/templates/new_fragment.rst.j2
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     2975 2023-04-16 12:20:46.000000 scriv-1.3.0/src/scriv/util.py
+drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-04-16 12:26:11.000000 scriv-1.3.0/src/scriv.egg-info/
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)    19048 2023-04-16 12:26:11.000000 scriv-1.3.0/src/scriv.egg-info/PKG-INFO
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     1726 2023-04-16 12:26:11.000000 scriv-1.3.0/src/scriv.egg-info/SOURCES.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)        1 2023-04-16 12:26:11.000000 scriv-1.3.0/src/scriv.egg-info/dependency_links.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)       40 2023-04-16 12:26:11.000000 scriv-1.3.0/src/scriv.egg-info/entry_points.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)       87 2023-04-16 12:26:11.000000 scriv-1.3.0/src/scriv.egg-info/requires.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)        6 2023-04-16 12:26:11.000000 scriv-1.3.0/src/scriv.egg-info/top_level.txt
+drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-04-16 12:26:11.000000 scriv-1.3.0/tests/
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)       27 2020-02-08 15:08:43.000000 scriv-1.3.0/tests/__init__.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     2344 2023-03-24 12:55:52.000000 scriv-1.3.0/tests/conftest.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     3923 2023-01-18 12:46:04.000000 scriv-1.3.0/tests/faker.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      558 2021-07-26 10:44:33.000000 scriv-1.3.0/tests/helpers.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     1364 2022-09-13 23:31:05.000000 scriv-1.3.0/tests/test_changelog.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)    17637 2023-04-16 12:20:46.000000 scriv-1.3.0/tests/test_collect.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)    10674 2023-02-18 23:51:51.000000 scriv-1.3.0/tests/test_config.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)    11237 2023-01-16 14:08:01.000000 scriv-1.3.0/tests/test_create.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      573 2022-04-24 21:45:49.000000 scriv-1.3.0/tests/test_faker.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     6938 2023-01-18 12:46:04.000000 scriv-1.3.0/tests/test_format_md.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     9205 2023-01-18 12:46:04.000000 scriv-1.3.0/tests/test_format_rst.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     6497 2023-01-18 10:44:55.000000 scriv-1.3.0/tests/test_ghrel.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     4110 2023-01-16 14:08:01.000000 scriv-1.3.0/tests/test_github.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     2485 2023-01-18 10:44:55.000000 scriv-1.3.0/tests/test_gitinfo.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     5046 2023-03-28 08:36:54.000000 scriv-1.3.0/tests/test_literals.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      349 2023-03-24 12:55:52.000000 scriv-1.3.0/tests/test_process.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     1975 2023-04-16 12:20:46.000000 scriv-1.3.0/tests/test_util.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     1688 2023-03-24 12:55:52.000000 scriv-1.3.0/tox.ini
```

### Comparing `scriv-1.2.1/CHANGELOG.rst` & `scriv-1.3.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,38 @@
 See the fragment files in the `changelog.d directory`_.
 
 .. _changelog.d directory: https://github.com/nedbat/scriv/tree/master/changelog.d
 
 
 .. scriv-insert-here
 
+.. _changelog-1.3.0:
+
+1.3.0 — 2023-04-16
+------------------
+
+Added
+.....
+
+- ``.cfg`` files can now be read with ``literal:`` settings, thanks to `Matias
+  Guijarro <pull 88_>`_.
+
+.. _pull 88: https://github.com/nedbat/scriv/pull/88
+
+Fixed
+.....
+
+- In compliance with `PEP 440`_, comparing version numbers now ignores a
+  leading "v" character.  This makes scriv more flexible about how you present
+  version numbers in various places (code literals, changelog entries, git
+  tags, and so on).  Fixes `issue 89`_.
+
+.. _PEP 440: https://peps.python.org/pep-0440/
+.. _issue 89: https://github.com/nedbat/scriv/issues/89
+
 .. _changelog-1.2.1:
 
 1.2.1 — 2023-02-18
 ------------------
 
 Fixed
 .....
```

### Comparing `scriv-1.2.1/LICENSE.txt` & `scriv-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scriv-1.2.1/Makefile` & `scriv-1.3.0/Makefile`

 * *Files identical despite different names*

### Comparing `scriv-1.2.1/PKG-INFO` & `scriv-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scriv
-Version: 1.2.1
+Version: 1.3.0
 Summary: Scriv changelog management tool
 Home-page: https://github.com/nedbat/scriv
 Author: Ned Batchelder
 Author-email: ned@nedbatchelder.com
 License: Apache-2.0
 Project-URL: Mastodon, https://hachyderm.io/@nedbat
 Project-URL: Funding, https://github.com/sponsors/nedbat
@@ -128,14 +128,38 @@
 See the fragment files in the `changelog.d directory`_.
 
 .. _changelog.d directory: https://github.com/nedbat/scriv/tree/master/changelog.d
 
 
 .. scriv-insert-here
 
+.. _changelog-1.3.0:
+
+1.3.0 — 2023-04-16
+------------------
+
+Added
+.....
+
+- ``.cfg`` files can now be read with ``literal:`` settings, thanks to `Matias
+  Guijarro <pull 88_>`_.
+
+.. _pull 88: https://github.com/nedbat/scriv/pull/88
+
+Fixed
+.....
+
+- In compliance with `PEP 440`_, comparing version numbers now ignores a
+  leading "v" character.  This makes scriv more flexible about how you present
+  version numbers in various places (code literals, changelog entries, git
+  tags, and so on).  Fixes `issue 89`_.
+
+.. _PEP 440: https://peps.python.org/pep-0440/
+.. _issue 89: https://github.com/nedbat/scriv/issues/89
+
 .. _changelog-1.2.1:
 
 1.2.1 — 2023-02-18
 ------------------
 
 Fixed
 .....
```

### Comparing `scriv-1.2.1/README.rst` & `scriv-1.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `scriv-1.2.1/docs/Makefile` & `scriv-1.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `scriv-1.2.1/docs/commands.rst` & `scriv-1.3.0/docs/commands.rst`

 * *Files identical despite different names*

### Comparing `scriv-1.2.1/docs/concepts.rst` & `scriv-1.3.0/docs/concepts.rst`

 * *Files identical despite different names*

### Comparing `scriv-1.2.1/docs/conf.py` & `scriv-1.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `scriv-1.2.1/docs/configuration.rst` & `scriv-1.3.0/docs/configuration.rst`

 * *Files 0% similar despite different names*

```diff
@@ -123,16 +123,16 @@
 
     [scriv]
     version = literal: myproj/__init__.py: __version__
 
 In this case, the file ``myproj/__init__.py`` will be read, and the
 ``__version__`` value will be found and used as the version setting.
 
-Currently Python, TOML and YAML files are supported for literals, but other
-syntaxes can be supported in the future.
+Currently Python, .cfg, TOML and YAML files are supported for literals, but
+other syntaxes can be supported in the future.
 
 When using a TOML file, the value is specified using periods to separate the
 sections and key names::
 
     [scriv]
     version = literal: pyproject.toml: project.version
```

### Comparing `scriv-1.2.1/docs/index.rst` & `scriv-1.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `scriv-1.2.1/docs/philosophy.rst` & `scriv-1.3.0/docs/philosophy.rst`

 * *Files identical despite different names*

### Comparing `scriv-1.2.1/pylintrc` & `scriv-1.3.0/pylintrc`

 * *Files identical despite different names*

### Comparing `scriv-1.2.1/requirements/base.txt` & `scriv-1.3.0/requirements/base.txt`

 * *Files 14% similar despite different names*

```diff
@@ -4,31 +4,31 @@
 #
 #    make upgrade
 #
 attrs==22.2.0
     # via -r requirements/base.in
 certifi==2022.12.7
     # via requests
-charset-normalizer==3.0.1
+charset-normalizer==3.1.0
     # via requests
 click==8.1.3
     # via
     #   -r requirements/base.in
     #   click-log
 click-log==0.4.0
     # via -r requirements/base.in
 idna==3.4
     # via requests
-importlib-metadata==6.0.0
+importlib-metadata==6.4.1
     # via click
 jinja2==3.1.2
     # via -r requirements/base.in
 markupsafe==2.1.2
     # via jinja2
 requests==2.28.2
     # via -r requirements/base.in
-typing-extensions==4.4.0
+typing-extensions==4.5.0
     # via importlib-metadata
-urllib3==1.26.14
+urllib3==1.26.15
     # via requests
-zipp==3.12.0
+zipp==3.15.0
     # via importlib-metadata
```

### Comparing `scriv-1.2.1/requirements/constraints.txt` & `scriv-1.3.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `scriv-1.2.1/requirements/dev.txt` & `scriv-1.3.0/requirements/dev.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,27 +4,25 @@
 #
 #    make upgrade
 #
 alabaster==0.7.13
     # via
     #   -r requirements/quality.txt
     #   sphinx
-astroid==2.14.1
+astroid==2.15.2
     # via
     #   -r requirements/quality.txt
     #   pylint
 attrs==22.2.0
-    # via
-    #   -r requirements/quality.txt
-    #   pytest
-babel==2.11.0
+    # via -r requirements/quality.txt
+babel==2.12.1
     # via
     #   -r requirements/quality.txt
     #   sphinx
-black==23.1.0
+black==23.3.0
     # via -r requirements/quality.txt
 bleach==6.0.0
     # via
     #   -r requirements/quality.txt
     #   readme-renderer
 build==0.10.0
     # via
@@ -40,15 +38,15 @@
     # via
     #   -r requirements/quality.txt
     #   requests
 chardet==5.1.0
     # via
     #   -r requirements/tox.txt
     #   tox
-charset-normalizer==3.0.1
+charset-normalizer==3.1.0
     # via
     #   -r requirements/quality.txt
     #   requests
 check-manifest==0.49
     # via -r requirements/quality.txt
 click==8.1.3
     # via
@@ -61,68 +59,68 @@
     # via -r requirements/quality.txt
 cogapp==3.3.0
     # via -r requirements/quality.txt
 colorama==0.4.6
     # via
     #   -r requirements/tox.txt
     #   tox
-coverage==7.1.0
+coverage==7.2.3
     # via -r requirements/quality.txt
 dill==0.3.6
     # via
     #   -r requirements/quality.txt
     #   pylint
 distlib==0.3.6
     # via
     #   -r requirements/tox.txt
     #   virtualenv
 doc8==0.11.2
     # via -r requirements/quality.txt
-docutils==0.17.1
+docutils==0.18.1
     # via
     #   -r requirements/quality.txt
     #   doc8
     #   readme-renderer
     #   restructuredtext-lint
     #   sphinx
     #   sphinx-rtd-theme
-exceptiongroup==1.1.0
+exceptiongroup==1.1.1
     # via
     #   -r requirements/quality.txt
     #   pytest
-filelock==3.9.0
+filelock==3.11.0
     # via
     #   -r requirements/tox.txt
     #   tox
     #   virtualenv
 freezegun==1.2.2
     # via -r requirements/quality.txt
 idna==3.4
     # via
     #   -r requirements/quality.txt
     #   requests
 imagesize==1.4.1
     # via
     #   -r requirements/quality.txt
     #   sphinx
-importlib-metadata==6.0.0
+importlib-metadata==6.4.1
     # via
     #   -r requirements/pip-tools.txt
     #   -r requirements/tox.txt
     #   build
     #   click
     #   keyring
     #   pluggy
     #   pytest
     #   sphinx
     #   stevedore
     #   tox
     #   twine
     #   virtualenv
-importlib-resources==5.10.2
+importlib-resources==5.12.0
     # via
     #   -r requirements/quality.txt
     #   keyring
 iniconfig==2.0.0
     # via
     #   -r requirements/quality.txt
     #   pytest
@@ -146,15 +144,15 @@
     # via
     #   -r requirements/quality.txt
     #   twine
 lazy-object-proxy==1.9.0
     # via
     #   -r requirements/quality.txt
     #   astroid
-markdown-it-py==2.1.0
+markdown-it-py==2.2.0
     # via
     #   -r requirements/quality.txt
     #   rich
 markupsafe==2.1.2
     # via
     #   -r requirements/quality.txt
     #   jinja2
@@ -162,55 +160,55 @@
     # via
     #   -r requirements/quality.txt
     #   pylint
 mdurl==0.1.2
     # via
     #   -r requirements/quality.txt
     #   markdown-it-py
-more-itertools==9.0.0
+more-itertools==9.1.0
     # via
     #   -r requirements/quality.txt
     #   jaraco-classes
-mypy==0.991
+mypy==1.2.0
     # via -r requirements/quality.txt
-mypy-extensions==0.4.3
+mypy-extensions==1.0.0
     # via
     #   -r requirements/quality.txt
     #   black
     #   mypy
-packaging==23.0
+packaging==23.1
     # via
     #   -r requirements/pip-tools.txt
     #   -r requirements/tox.txt
     #   black
     #   build
     #   pudb
     #   pyproject-api
     #   pytest
     #   sphinx
     #   tox
 parso==0.8.3
     # via
     #   -r requirements/quality.txt
     #   jedi
-pathspec==0.11.0
+pathspec==0.11.1
     # via
     #   -r requirements/quality.txt
     #   black
 pbr==5.11.1
     # via
     #   -r requirements/quality.txt
     #   stevedore
-pip-tools==6.12.2
+pip-tools==6.13.0
     # via -r requirements/pip-tools.txt
 pkginfo==1.9.6
     # via
     #   -r requirements/quality.txt
     #   twine
-platformdirs==2.6.2
+platformdirs==3.2.0
     # via
     #   -r requirements/quality.txt
     #   -r requirements/tox.txt
     #   black
     #   pylint
     #   tox
     #   virtualenv
@@ -222,54 +220,56 @@
     #   tox
 pudb==2022.1.3
     # via -r requirements/quality.txt
 pycodestyle==2.10.0
     # via -r requirements/quality.txt
 pydocstyle==6.1.1
     # via -r requirements/quality.txt
-pygments==2.14.0
+pygments==2.15.0
     # via
     #   -r requirements/quality.txt
     #   doc8
     #   pudb
     #   readme-renderer
     #   rich
     #   sphinx
-pylint==2.16.1
+pylint==2.17.2
     # via
     #   -r requirements/quality.txt
     #   pylint-pytest
 pylint-pytest==1.0.3
     # via -r requirements/quality.txt
-pyproject-api==1.5.0
+pyproject-api==1.5.1
     # via
     #   -r requirements/tox.txt
     #   tox
 pyproject-hooks==1.0.0
     # via
     #   -r requirements/pip-tools.txt
     #   -r requirements/quality.txt
     #   build
-pytest==7.2.1
+pytest==7.3.1
     # via
     #   -r requirements/quality.txt
     #   pylint-pytest
     #   pytest-mock
 pytest-mock==3.10.0
     # via -r requirements/quality.txt
 python-dateutil==2.8.2
     # via
     #   -r requirements/quality.txt
     #   freezegun
-pytz==2022.7.1
+pytz==2023.3
     # via
     #   -r requirements/quality.txt
     #   babel
 pyyaml==6.0
-    # via -r requirements/quality.txt
+    # via
+    #   -r requirements/quality.txt
+    #   responses
 readme-renderer==37.3
     # via
     #   -r requirements/quality.txt
     #   twine
 requests==2.28.2
     # via
     #   -r requirements/quality.txt
@@ -277,25 +277,25 @@
     #   responses
     #   sphinx
     #   twine
 requests-toolbelt==0.10.1
     # via
     #   -r requirements/quality.txt
     #   twine
-responses==0.22.0
+responses==0.23.1
     # via -r requirements/quality.txt
 restructuredtext-lint==1.4.0
     # via
     #   -r requirements/quality.txt
     #   doc8
 rfc3986==2.0.0
     # via
     #   -r requirements/quality.txt
     #   twine
-rich==13.3.1
+rich==13.3.4
     # via
     #   -r requirements/quality.txt
     #   twine
 six==1.16.0
     # via
     #   -r requirements/quality.txt
     #   bleach
@@ -305,28 +305,33 @@
     #   -r requirements/quality.txt
     #   pydocstyle
     #   sphinx
 sphinx==5.3.0
     # via
     #   -r requirements/quality.txt
     #   sphinx-rtd-theme
-sphinx-rtd-theme==1.1.1
+    #   sphinxcontrib-jquery
+sphinx-rtd-theme==1.2.0
     # via -r requirements/quality.txt
 sphinxcontrib-applehelp==1.0.2
     # via
     #   -r requirements/quality.txt
     #   sphinx
 sphinxcontrib-devhelp==1.0.2
     # via
     #   -r requirements/quality.txt
     #   sphinx
 sphinxcontrib-htmlhelp==2.0.0
     # via
     #   -r requirements/quality.txt
     #   sphinx
+sphinxcontrib-jquery==4.1
+    # via
+    #   -r requirements/quality.txt
+    #   sphinx-rtd-theme
 sphinxcontrib-jsmath==1.0.1
     # via
     #   -r requirements/quality.txt
     #   sphinx
 sphinxcontrib-qthelp==1.0.3
     # via
     #   -r requirements/quality.txt
@@ -335,36 +340,32 @@
     # via
     #   -r requirements/quality.txt
     #   sphinx
 stevedore==3.5.2
     # via
     #   -r requirements/quality.txt
     #   doc8
-toml==0.10.2
-    # via
-    #   -r requirements/quality.txt
-    #   responses
 tomli==2.0.1
     # via
     #   -r requirements/pip-tools.txt
     #   -r requirements/tox.txt
     #   black
     #   build
     #   check-manifest
     #   mypy
     #   pylint
     #   pyproject-api
     #   pyproject-hooks
     #   pytest
     #   tox
-tomlkit==0.11.6
+tomlkit==0.11.7
     # via
     #   -r requirements/quality.txt
     #   pylint
-tox==4.4.4
+tox==4.4.12
     # via
     #   -r requirements/tox.txt
     #   tox-gh
 tox-gh==1.0.0
     # via -r requirements/tox.txt
 twine==4.0.2
     # via -r requirements/quality.txt
@@ -372,72 +373,72 @@
     # via
     #   -r requirements/quality.txt
     #   astroid
     #   black
     #   mypy
 types-freezegun==1.1.10
     # via -r requirements/quality.txt
-types-pyyaml==6.0.12.4
-    # via -r requirements/quality.txt
-types-requests==2.28.11.8
-    # via -r requirements/quality.txt
-types-toml==0.10.8.2
+types-pyyaml==6.0.12.9
     # via
     #   -r requirements/quality.txt
     #   responses
-types-urllib3==1.26.25.4
+types-requests==2.28.11.17
+    # via -r requirements/quality.txt
+types-toml==0.10.8.6
+    # via -r requirements/quality.txt
+types-urllib3==1.26.25.10
     # via
     #   -r requirements/quality.txt
     #   types-requests
-typing-extensions==4.4.0
+typing-extensions==4.5.0
     # via
     #   -r requirements/pip-tools.txt
     #   -r requirements/tox.txt
     #   astroid
     #   black
     #   importlib-metadata
     #   markdown-it-py
     #   mypy
     #   platformdirs
     #   pylint
     #   responses
     #   rich
     #   tox
-urllib3==1.26.14
+urllib3==1.26.15
     # via
     #   -r requirements/quality.txt
     #   requests
     #   responses
     #   twine
 urwid==2.1.2
     # via
     #   -r requirements/quality.txt
     #   pudb
     #   urwid-readline
 urwid-readline==0.13
     # via
     #   -r requirements/quality.txt
     #   pudb
-virtualenv==20.17.1
+virtualenv==20.21.0
     # via
     #   -r requirements/tox.txt
     #   tox
 webencodings==0.5.1
     # via
     #   -r requirements/quality.txt
     #   bleach
-wheel==0.38.4
+wheel==0.40.0
     # via
     #   -r requirements/pip-tools.txt
     #   pip-tools
-wrapt==1.14.1
+wrapt==1.15.0
     # via
     #   -r requirements/quality.txt
     #   astroid
-zipp==3.12.0
+zipp==3.15.0
     # via
     #   -r requirements/pip-tools.txt
     #   -r requirements/tox.txt
     #   importlib-metadata
     #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
```

### Comparing `scriv-1.2.1/requirements/doc.txt` & `scriv-1.3.0/requirements/doc.txt`

 * *Files 17% similar despite different names*

```diff
@@ -3,58 +3,56 @@
 # by the following command:
 #
 #    make upgrade
 #
 alabaster==0.7.13
     # via sphinx
 attrs==22.2.0
-    # via
-    #   -r requirements/test.txt
-    #   pytest
-babel==2.11.0
+    # via -r requirements/test.txt
+babel==2.12.1
     # via sphinx
 certifi==2022.12.7
     # via
     #   -r requirements/test.txt
     #   requests
-charset-normalizer==3.0.1
+charset-normalizer==3.1.0
     # via
     #   -r requirements/test.txt
     #   requests
 click==8.1.3
     # via
     #   -r requirements/test.txt
     #   click-log
 click-log==0.4.0
     # via -r requirements/test.txt
 cogapp==3.3.0
     # via -r requirements/doc.in
-coverage==7.1.0
+coverage==7.2.3
     # via -r requirements/test.txt
 doc8==0.11.2
     # via -r requirements/doc.in
-docutils==0.17.1
+docutils==0.18.1
     # via
     #   doc8
     #   restructuredtext-lint
     #   sphinx
     #   sphinx-rtd-theme
-exceptiongroup==1.1.0
+exceptiongroup==1.1.1
     # via
     #   -r requirements/test.txt
     #   pytest
 freezegun==1.2.2
     # via -r requirements/test.txt
 idna==3.4
     # via
     #   -r requirements/test.txt
     #   requests
 imagesize==1.4.1
     # via sphinx
-importlib-metadata==6.0.0
+importlib-metadata==6.4.1
     # via
     #   -r requirements/test.txt
     #   click
     #   pluggy
     #   pytest
     #   sphinx
     #   stevedore
@@ -70,15 +68,15 @@
     # via
     #   -r requirements/test.txt
     #   sphinx
 markupsafe==2.1.2
     # via
     #   -r requirements/test.txt
     #   jinja2
-packaging==23.0
+packaging==23.1
     # via
     #   -r requirements/test.txt
     #   pudb
     #   pytest
     #   sphinx
 parso==0.8.3
     # via
@@ -88,97 +86,98 @@
     # via stevedore
 pluggy==1.0.0
     # via
     #   -r requirements/test.txt
     #   pytest
 pudb==2022.1.3
     # via -r requirements/test.txt
-pygments==2.14.0
+pygments==2.15.0
     # via
     #   -r requirements/test.txt
     #   doc8
     #   pudb
     #   sphinx
-pytest==7.2.1
+pytest==7.3.1
     # via
     #   -r requirements/test.txt
     #   pytest-mock
 pytest-mock==3.10.0
     # via -r requirements/test.txt
 python-dateutil==2.8.2
     # via
     #   -r requirements/test.txt
     #   freezegun
-pytz==2022.7.1
+pytz==2023.3
     # via babel
 pyyaml==6.0
-    # via -r requirements/test.txt
+    # via
+    #   -r requirements/test.txt
+    #   responses
 requests==2.28.2
     # via
     #   -r requirements/test.txt
     #   responses
     #   sphinx
-responses==0.22.0
+responses==0.23.1
     # via -r requirements/test.txt
 restructuredtext-lint==1.4.0
     # via doc8
 six==1.16.0
     # via
     #   -r requirements/test.txt
     #   python-dateutil
 snowballstemmer==2.2.0
     # via sphinx
 sphinx==5.3.0
     # via
     #   -r requirements/doc.in
     #   sphinx-rtd-theme
-sphinx-rtd-theme==1.1.1
+    #   sphinxcontrib-jquery
+sphinx-rtd-theme==1.2.0
     # via -r requirements/doc.in
 sphinxcontrib-applehelp==1.0.2
     # via sphinx
 sphinxcontrib-devhelp==1.0.2
     # via sphinx
 sphinxcontrib-htmlhelp==2.0.0
     # via sphinx
+sphinxcontrib-jquery==4.1
+    # via sphinx-rtd-theme
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.3
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.5
     # via sphinx
 stevedore==3.5.2
     # via doc8
-toml==0.10.2
-    # via
-    #   -r requirements/test.txt
-    #   responses
 tomli==2.0.1
     # via
     #   -r requirements/test.txt
     #   pytest
-types-toml==0.10.8.2
+types-pyyaml==6.0.12.9
     # via
     #   -r requirements/test.txt
     #   responses
-typing-extensions==4.4.0
+typing-extensions==4.5.0
     # via
     #   -r requirements/test.txt
     #   importlib-metadata
     #   responses
-urllib3==1.26.14
+urllib3==1.26.15
     # via
     #   -r requirements/test.txt
     #   requests
     #   responses
 urwid==2.1.2
     # via
     #   -r requirements/test.txt
     #   pudb
     #   urwid-readline
 urwid-readline==0.13
     # via
     #   -r requirements/test.txt
     #   pudb
-zipp==3.12.0
+zipp==3.15.0
     # via
     #   -r requirements/test.txt
     #   importlib-metadata
```

### Comparing `scriv-1.2.1/requirements/pip-tools.txt` & `scriv-1.3.0/requirements/pip-tools.txt`

 * *Files 17% similar despite different names*

```diff
@@ -4,31 +4,31 @@
 #
 #    make upgrade
 #
 build==0.10.0
     # via pip-tools
 click==8.1.3
     # via pip-tools
-importlib-metadata==6.0.0
+importlib-metadata==6.4.1
     # via
     #   build
     #   click
-packaging==23.0
+packaging==23.1
     # via build
-pip-tools==6.12.2
+pip-tools==6.13.0
     # via -r requirements/pip-tools.in
 pyproject-hooks==1.0.0
     # via build
 tomli==2.0.1
     # via
     #   build
     #   pyproject-hooks
-typing-extensions==4.4.0
+typing-extensions==4.5.0
     # via importlib-metadata
-wheel==0.38.4
+wheel==0.40.0
     # via pip-tools
-zipp==3.12.0
+zipp==3.15.0
     # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `scriv-1.2.1/requirements/quality.in` & `scriv-1.3.0/requirements/quality.in`

 * *Files identical despite different names*

### Comparing `scriv-1.2.1/requirements/quality.txt` & `scriv-1.3.0/requirements/quality.txt`

 * *Files 5% similar despite different names*

```diff
@@ -4,37 +4,36 @@
 #
 #    make upgrade
 #
 alabaster==0.7.13
     # via
     #   -r requirements/doc.txt
     #   sphinx
-astroid==2.14.1
+astroid==2.15.2
     # via pylint
 attrs==22.2.0
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test.txt
-    #   pytest
-babel==2.11.0
+babel==2.12.1
     # via
     #   -r requirements/doc.txt
     #   sphinx
-black==23.1.0
+black==23.3.0
     # via -r requirements/quality.in
 bleach==6.0.0
     # via readme-renderer
 build==0.10.0
     # via check-manifest
 certifi==2022.12.7
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test.txt
     #   requests
-charset-normalizer==3.0.1
+charset-normalizer==3.1.0
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test.txt
     #   requests
 check-manifest==0.49
     # via -r requirements/quality.in
 click==8.1.3
@@ -45,31 +44,31 @@
     #   click-log
 click-log==0.4.0
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test.txt
 cogapp==3.3.0
     # via -r requirements/doc.txt
-coverage==7.1.0
+coverage==7.2.3
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test.txt
 dill==0.3.6
     # via pylint
 doc8==0.11.2
     # via -r requirements/doc.txt
-docutils==0.17.1
+docutils==0.18.1
     # via
     #   -r requirements/doc.txt
     #   doc8
     #   readme-renderer
     #   restructuredtext-lint
     #   sphinx
     #   sphinx-rtd-theme
-exceptiongroup==1.1.0
+exceptiongroup==1.1.1
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test.txt
     #   pytest
 freezegun==1.2.2
     # via
     #   -r requirements/doc.txt
@@ -79,27 +78,27 @@
     #   -r requirements/doc.txt
     #   -r requirements/test.txt
     #   requests
 imagesize==1.4.1
     # via
     #   -r requirements/doc.txt
     #   sphinx
-importlib-metadata==6.0.0
+importlib-metadata==6.4.1
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test.txt
     #   build
     #   click
     #   keyring
     #   pluggy
     #   pytest
     #   sphinx
     #   stevedore
     #   twine
-importlib-resources==5.10.2
+importlib-resources==5.12.0
     # via keyring
 iniconfig==2.0.0
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test.txt
     #   pytest
 isort==5.11.5
@@ -118,56 +117,56 @@
     #   -r requirements/doc.txt
     #   -r requirements/test.txt
     #   sphinx
 keyring==23.13.1
     # via twine
 lazy-object-proxy==1.9.0
     # via astroid
-markdown-it-py==2.1.0
+markdown-it-py==2.2.0
     # via rich
 markupsafe==2.1.2
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test.txt
     #   jinja2
 mccabe==0.7.0
     # via pylint
 mdurl==0.1.2
     # via markdown-it-py
-more-itertools==9.0.0
+more-itertools==9.1.0
     # via jaraco-classes
-mypy==0.991
+mypy==1.2.0
     # via -r requirements/quality.in
-mypy-extensions==0.4.3
+mypy-extensions==1.0.0
     # via
     #   black
     #   mypy
-packaging==23.0
+packaging==23.1
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test.txt
     #   black
     #   build
     #   pudb
     #   pytest
     #   sphinx
 parso==0.8.3
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test.txt
     #   jedi
-pathspec==0.11.0
+pathspec==0.11.1
     # via black
 pbr==5.11.1
     # via
     #   -r requirements/doc.txt
     #   stevedore
 pkginfo==1.9.6
     # via twine
-platformdirs==2.6.2
+platformdirs==3.2.0
     # via
     #   black
     #   pylint
 pluggy==1.0.0
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test.txt
@@ -176,77 +175,78 @@
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test.txt
 pycodestyle==2.10.0
     # via -r requirements/quality.in
 pydocstyle==6.1.1
     # via -r requirements/quality.in
-pygments==2.14.0
+pygments==2.15.0
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test.txt
     #   doc8
     #   pudb
     #   readme-renderer
     #   rich
     #   sphinx
-pylint==2.16.1
+pylint==2.17.2
     # via
     #   -r requirements/quality.in
     #   pylint-pytest
 pylint-pytest==1.0.3
     # via -r requirements/quality.in
 pyproject-hooks==1.0.0
     # via build
-pytest==7.2.1
+pytest==7.3.1
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test.txt
     #   pylint-pytest
     #   pytest-mock
 pytest-mock==3.10.0
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test.txt
 python-dateutil==2.8.2
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test.txt
     #   freezegun
-pytz==2022.7.1
+pytz==2023.3
     # via
     #   -r requirements/doc.txt
     #   babel
 pyyaml==6.0
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test.txt
+    #   responses
 readme-renderer==37.3
     # via twine
 requests==2.28.2
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test.txt
     #   requests-toolbelt
     #   responses
     #   sphinx
     #   twine
 requests-toolbelt==0.10.1
     # via twine
-responses==0.22.0
+responses==0.23.1
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test.txt
 restructuredtext-lint==1.4.0
     # via
     #   -r requirements/doc.txt
     #   doc8
 rfc3986==2.0.0
     # via twine
-rich==13.3.1
+rich==13.3.4
     # via twine
 six==1.16.0
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test.txt
     #   bleach
     #   python-dateutil
@@ -255,28 +255,33 @@
     #   -r requirements/doc.txt
     #   pydocstyle
     #   sphinx
 sphinx==5.3.0
     # via
     #   -r requirements/doc.txt
     #   sphinx-rtd-theme
-sphinx-rtd-theme==1.1.1
+    #   sphinxcontrib-jquery
+sphinx-rtd-theme==1.2.0
     # via -r requirements/doc.txt
 sphinxcontrib-applehelp==1.0.2
     # via
     #   -r requirements/doc.txt
     #   sphinx
 sphinxcontrib-devhelp==1.0.2
     # via
     #   -r requirements/doc.txt
     #   sphinx
 sphinxcontrib-htmlhelp==2.0.0
     # via
     #   -r requirements/doc.txt
     #   sphinx
+sphinxcontrib-jquery==4.1
+    # via
+    #   -r requirements/doc.txt
+    #   sphinx-rtd-theme
 sphinxcontrib-jsmath==1.0.1
     # via
     #   -r requirements/doc.txt
     #   sphinx
 sphinxcontrib-qthelp==1.0.3
     # via
     #   -r requirements/doc.txt
@@ -285,66 +290,61 @@
     # via
     #   -r requirements/doc.txt
     #   sphinx
 stevedore==3.5.2
     # via
     #   -r requirements/doc.txt
     #   doc8
-toml==0.10.2
-    # via
-    #   -r requirements/doc.txt
-    #   -r requirements/test.txt
-    #   responses
 tomli==2.0.1
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test.txt
     #   black
     #   build
     #   check-manifest
     #   mypy
     #   pylint
     #   pyproject-hooks
     #   pytest
-tomlkit==0.11.6
+tomlkit==0.11.7
     # via pylint
 twine==4.0.2
     # via -r requirements/quality.in
 typed-ast==1.5.4
     # via
     #   astroid
     #   black
     #   mypy
 types-freezegun==1.1.10
     # via -r requirements/quality.in
-types-pyyaml==6.0.12.4
-    # via -r requirements/quality.in
-types-requests==2.28.11.8
-    # via -r requirements/quality.in
-types-toml==0.10.8.2
+types-pyyaml==6.0.12.9
     # via
     #   -r requirements/quality.in
     #   -r requirements/test.txt
     #   responses
-types-urllib3==1.26.25.4
+types-requests==2.28.11.17
+    # via -r requirements/quality.in
+types-toml==0.10.8.6
+    # via -r requirements/quality.in
+types-urllib3==1.26.25.10
     # via types-requests
-typing-extensions==4.4.0
+typing-extensions==4.5.0
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test.txt
     #   astroid
     #   black
     #   importlib-metadata
     #   markdown-it-py
     #   mypy
     #   platformdirs
     #   pylint
     #   responses
     #   rich
-urllib3==1.26.14
+urllib3==1.26.15
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test.txt
     #   requests
     #   responses
     #   twine
 urwid==2.1.2
@@ -356,17 +356,17 @@
 urwid-readline==0.13
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test.txt
     #   pudb
 webencodings==0.5.1
     # via bleach
-wrapt==1.14.1
+wrapt==1.15.0
     # via astroid
-zipp==3.12.0
+zipp==3.15.0
     # via
     #   -r requirements/doc.txt
     #   -r requirements/test.txt
     #   importlib-metadata
     #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
```

### Comparing `scriv-1.2.1/requirements/test.txt` & `scriv-1.3.0/requirements/test.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,40 @@
 #
 # This file is autogenerated by pip-compile with Python 3.7
 # by the following command:
 #
 #    make upgrade
 #
 attrs==22.2.0
-    # via
-    #   -r requirements/base.txt
-    #   pytest
+    # via -r requirements/base.txt
 certifi==2022.12.7
     # via
     #   -r requirements/base.txt
     #   requests
-charset-normalizer==3.0.1
+charset-normalizer==3.1.0
     # via
     #   -r requirements/base.txt
     #   requests
 click==8.1.3
     # via
     #   -r requirements/base.txt
     #   click-log
 click-log==0.4.0
     # via -r requirements/base.txt
-coverage==7.1.0
+coverage==7.2.3
     # via -r requirements/test.in
-exceptiongroup==1.1.0
+exceptiongroup==1.1.1
     # via pytest
 freezegun==1.2.2
     # via -r requirements/test.in
 idna==3.4
     # via
     #   -r requirements/base.txt
     #   requests
-importlib-metadata==6.0.0
+importlib-metadata==6.4.1
     # via
     #   -r requirements/base.txt
     #   click
     #   pluggy
     #   pytest
 iniconfig==2.0.0
     # via pytest
@@ -44,61 +42,61 @@
     # via pudb
 jinja2==3.1.2
     # via -r requirements/base.txt
 markupsafe==2.1.2
     # via
     #   -r requirements/base.txt
     #   jinja2
-packaging==23.0
+packaging==23.1
     # via
     #   pudb
     #   pytest
 parso==0.8.3
     # via jedi
 pluggy==1.0.0
     # via pytest
 pudb==2022.1.3
     # via -r requirements/test.in
-pygments==2.14.0
+pygments==2.15.0
     # via pudb
-pytest==7.2.1
+pytest==7.3.1
     # via pytest-mock
 pytest-mock==3.10.0
     # via -r requirements/test.in
 python-dateutil==2.8.2
     # via freezegun
 pyyaml==6.0
-    # via -r requirements/test.in
+    # via
+    #   -r requirements/test.in
+    #   responses
 requests==2.28.2
     # via
     #   -r requirements/base.txt
     #   responses
-responses==0.22.0
+responses==0.23.1
     # via -r requirements/test.in
 six==1.16.0
     # via python-dateutil
-toml==0.10.2
-    # via responses
 tomli==2.0.1
     # via pytest
-types-toml==0.10.8.2
+types-pyyaml==6.0.12.9
     # via responses
-typing-extensions==4.4.0
+typing-extensions==4.5.0
     # via
     #   -r requirements/base.txt
     #   importlib-metadata
     #   responses
-urllib3==1.26.14
+urllib3==1.26.15
     # via
     #   -r requirements/base.txt
     #   requests
     #   responses
 urwid==2.1.2
     # via
     #   pudb
     #   urwid-readline
 urwid-readline==0.13
     # via pudb
-zipp==3.12.0
+zipp==3.15.0
     # via
     #   -r requirements/base.txt
     #   importlib-metadata
```

### Comparing `scriv-1.2.1/requirements/tox.txt` & `scriv-1.3.0/requirements/tox.txt`

 * *Files 4% similar despite different names*

```diff
@@ -8,47 +8,47 @@
     # via tox
 chardet==5.1.0
     # via tox
 colorama==0.4.6
     # via tox
 distlib==0.3.6
     # via virtualenv
-filelock==3.9.0
+filelock==3.11.0
     # via
     #   tox
     #   virtualenv
-importlib-metadata==6.0.0
+importlib-metadata==6.4.1
     # via
     #   pluggy
     #   tox
     #   virtualenv
-packaging==23.0
+packaging==23.1
     # via
     #   pyproject-api
     #   tox
-platformdirs==2.6.2
+platformdirs==3.2.0
     # via
     #   tox
     #   virtualenv
 pluggy==1.0.0
     # via tox
-pyproject-api==1.5.0
+pyproject-api==1.5.1
     # via tox
 tomli==2.0.1
     # via
     #   pyproject-api
     #   tox
-tox==4.4.4
+tox==4.4.12
     # via
     #   -r requirements/tox.in
     #   tox-gh
 tox-gh==1.0.0
     # via -r requirements/tox.in
-typing-extensions==4.4.0
+typing-extensions==4.5.0
     # via
     #   importlib-metadata
     #   platformdirs
     #   tox
-virtualenv==20.17.1
+virtualenv==20.21.0
     # via tox
-zipp==3.12.0
+zipp==3.15.0
     # via importlib-metadata
```

### Comparing `scriv-1.2.1/setup.cfg` & `scriv-1.3.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -101,13 +101,13 @@
 
 [pycodestyle]
 exclude = .git,.tox
 max-line-length = 80
 ignore = E203,W503
 
 [pydocstyle]
-ignore = D200,D203,D212,D406,D407,D413
+ignore = D105,D200,D203,D212,D406,D407,D413
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `scriv-1.2.1/src/scriv/changelog.py` & `scriv-1.3.0/src/scriv/changelog.py`

 * *Files identical despite different names*

### Comparing `scriv-1.2.1/src/scriv/cli.py` & `scriv-1.3.0/src/scriv/cli.py`

 * *Files identical despite different names*

### Comparing `scriv-1.2.1/src/scriv/collect.py` & `scriv-1.3.0/src/scriv/collect.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Optional
 
 import click
 import click_log
 
 from .gitinfo import git_add, git_config_bool, git_edit, git_rm
 from .scriv import Scriv
-from .util import extract_version
+from .util import Version
 
 logger = logging.getLogger(__name__)
 
 
 @click.command()
 @click.option(
     "--add/--no-add",
@@ -60,24 +60,25 @@
         logger.info("No changelog fragments to collect")
         return
 
     changelog = scriv.changelog()
     changelog.read()
 
     if title is None:
-        version = version or scriv.config.version
+        version = Version(version or scriv.config.version)
         if version:
             # Check that we haven't used this version before.
             for etitle in changelog.entries().keys():
                 if etitle is None:
                     continue
-                eversion = extract_version(etitle)
+                eversion = Version.from_text(etitle)
                 if eversion == version:
                     sys.exit(
-                        f"Entry {etitle!r} already uses version {version!r}."
+                        f"Entry {etitle!r} already uses "
+                        + f"version {str(version)!r}."
                     )
         new_header = changelog.entry_header(version=version)
     else:
         new_header = changelog.format_tools().format_header(title)
 
     new_text = changelog.entry_text(scriv.combine_fragments(frags))
     changelog.add_entry(new_header, new_text)
```

### Comparing `scriv-1.2.1/src/scriv/config.py` & `scriv-1.3.0/src/scriv/config.py`

 * *Files identical despite different names*

### Comparing `scriv-1.2.1/src/scriv/create.py` & `scriv-1.3.0/src/scriv/create.py`

 * *Files identical despite different names*

### Comparing `scriv-1.2.1/src/scriv/format.py` & `scriv-1.3.0/src/scriv/format.py`

 * *Files identical despite different names*

### Comparing `scriv-1.2.1/src/scriv/format_md.py` & `scriv-1.3.0/src/scriv/format_md.py`

 * *Files identical despite different names*

### Comparing `scriv-1.2.1/src/scriv/format_rst.py` & `scriv-1.3.0/src/scriv/format_rst.py`

 * *Files identical despite different names*

### Comparing `scriv-1.2.1/src/scriv/ghrel.py` & `scriv-1.3.0/src/scriv/ghrel.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import click_log
 import jinja2
 
 from .github import create_release, get_releases, update_release
 from .gitinfo import get_github_repos
 from .scriv import Scriv
 from .shell import run_simple_command
-from .util import extract_version, is_prerelease_version
+from .util import Version
 
 logger = logging.getLogger(__name__)
 
 
 @click.command()
 @click.option(
     "--all",
@@ -59,64 +59,65 @@
             sys.exit(f"More than one GitHub repo found: {repo_list}")
 
         repo = repos.pop()
 
     if not re.fullmatch(r"[^ /]+/[^ /]+", repo):
         sys.exit(f"Repo must be owner/reponame: {repo!r}")
 
-    tags = set(run_simple_command("git tag").split())
-    releases = get_releases(repo)
+    tags = set(map(Version, run_simple_command("git tag").split()))
+    releases = {Version(k): v for k, v in get_releases(repo).items()}
 
     for title, sections in changelog.entries().items():
         if title is None:
             continue
-        version = extract_version(title)
+        version = Version.from_text(title)
         if version is None:
             logger.warning(f"Entry {title!r} has no version, skipping.")
             continue
 
-        if version in tags:
-            section_text = "\n\n".join(sections)
-            md = changelog.format_tools().convert_to_markdown(section_text)
-
-            release_data = {
-                "body": md,
-                "name": version,
-                "tag_name": version,
-                "draft": False,
-                "prerelease": is_prerelease_version(version),
-            }
-
-            ghrel_template = jinja2.Template(scriv.config.ghrel_template)
-            md = ghrel_template.render(
-                body=md,
-                version=version,
-                release=release_data,
-                config=scriv.config,
+        if version not in tags:
+            logger.warning(
+                f"Version {version} has no tag. No release will be made."
             )
-            release_data["body"] = md
+            continue
 
-            if version in releases:
-                release = releases[version]
-                if release["body"] != md:
-                    logger.debug(
-                        f"Updating release {version}, data = {release_data}"
-                    )
-                    if dry_run:
-                        logger.info(f"Would update release {version}")
-                        logger.info(f"Body:\n{md}")
-                    else:
-                        update_release(release, release_data)
-            else:
-                logger.debug(f"Creating release, data = {release_data}")
+        section_text = "\n\n".join(sections)
+        md = changelog.format_tools().convert_to_markdown(section_text)
+
+        release_data = {
+            "body": md,
+            "name": version,
+            "tag_name": version,
+            "draft": False,
+            "prerelease": version.is_prerelease(),
+        }
+
+        ghrel_template = jinja2.Template(scriv.config.ghrel_template)
+        md = ghrel_template.render(
+            body=md,
+            version=version,
+            release=release_data,
+            config=scriv.config,
+        )
+        release_data["body"] = md
+
+        if version in releases:
+            release = releases[version]
+            if release["body"] != md:
+                logger.debug(
+                    f"Updating release {version}, data = {release_data}"
+                )
                 if dry_run:
-                    logger.info(f"Would create release {version}")
+                    logger.info(f"Would update release {version}")
                     logger.info(f"Body:\n{md}")
                 else:
-                    create_release(repo, release_data)
+                    update_release(release, release_data)
         else:
-            logger.warning(
-                f"Version {version} has no tag. No release will be made."
-            )
+            logger.debug(f"Creating release, data = {release_data}")
+            if dry_run:
+                logger.info(f"Would create release {version}")
+                logger.info(f"Body:\n{md}")
+            else:
+                create_release(repo, release_data)
 
         if not all_entries:
             break
```

### Comparing `scriv-1.2.1/src/scriv/github.py` & `scriv-1.3.0/src/scriv/github.py`

 * *Files identical despite different names*

### Comparing `scriv-1.2.1/src/scriv/gitinfo.py` & `scriv-1.3.0/src/scriv/gitinfo.py`

 * *Files identical despite different names*

### Comparing `scriv-1.2.1/src/scriv/literals.py` & `scriv-1.3.0/src/scriv/literals.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Find literals in various kinds of files.
 """
 
 import ast
+import configparser
 import os.path
 from typing import Any, MutableMapping, Optional
 
 from .exceptions import ScrivException
 from .optional import tomllib, yaml
 
 
@@ -39,14 +40,18 @@
                 "Can't read {!r} without YAML support. "
                 + "Install with [yaml] extra"
             ).format(file_name)
             raise ScrivException(msg)
         with open(file_name, encoding="utf-8") as f:
             data = yaml.safe_load(f)
         return find_nested_value(data, literal_name)
+    elif ext == ".cfg":
+        cfg_parser = configparser.ConfigParser()
+        cfg_parser.read(file_name)
+        return find_nested_value(cfg_parser, literal_name)
     else:
         raise ScrivException(
             f"Can't read literals from files like {file_name!r}"
         )
 
 
 class PythonLiteralFinder(ast.NodeVisitor):
```

### Comparing `scriv-1.2.1/src/scriv/scriv.py` & `scriv-1.3.0/src/scriv/scriv.py`

 * *Files identical despite different names*

### Comparing `scriv-1.2.1/src/scriv/shell.py` & `scriv-1.3.0/src/scriv/shell.py`

 * *Files identical despite different names*

### Comparing `scriv-1.2.1/src/scriv.egg-info/PKG-INFO` & `scriv-1.3.0/src/scriv.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scriv
-Version: 1.2.1
+Version: 1.3.0
 Summary: Scriv changelog management tool
 Home-page: https://github.com/nedbat/scriv
 Author: Ned Batchelder
 Author-email: ned@nedbatchelder.com
 License: Apache-2.0
 Project-URL: Mastodon, https://hachyderm.io/@nedbat
 Project-URL: Funding, https://github.com/sponsors/nedbat
@@ -128,14 +128,38 @@
 See the fragment files in the `changelog.d directory`_.
 
 .. _changelog.d directory: https://github.com/nedbat/scriv/tree/master/changelog.d
 
 
 .. scriv-insert-here
 
+.. _changelog-1.3.0:
+
+1.3.0 — 2023-04-16
+------------------
+
+Added
+.....
+
+- ``.cfg`` files can now be read with ``literal:`` settings, thanks to `Matias
+  Guijarro <pull 88_>`_.
+
+.. _pull 88: https://github.com/nedbat/scriv/pull/88
+
+Fixed
+.....
+
+- In compliance with `PEP 440`_, comparing version numbers now ignores a
+  leading "v" character.  This makes scriv more flexible about how you present
+  version numbers in various places (code literals, changelog entries, git
+  tags, and so on).  Fixes `issue 89`_.
+
+.. _PEP 440: https://peps.python.org/pep-0440/
+.. _issue 89: https://github.com/nedbat/scriv/issues/89
+
 .. _changelog-1.2.1:
 
 1.2.1 — 2023-02-18
 ------------------
 
 Fixed
 .....
```

### Comparing `scriv-1.2.1/src/scriv.egg-info/SOURCES.txt` & `scriv-1.3.0/src/scriv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scriv-1.2.1/tests/conftest.py` & `scriv-1.3.0/tests/conftest.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,29 @@
 """Fixture definitions."""
 
 import os
+import sys
 import traceback
 from pathlib import Path
 from typing import Iterable
 
 import pytest
 import responses
 from click.testing import CliRunner
 
+# We want to be able to test scriv without any extras installed.  But responses
+# installs PyYaml.  If we are testing the no-extras scenario, then: after we've
+# imported responses above, and before we import any scriv modules below,
+# clobber the yaml module so that scriv's import will fail, simulating PyYaml
+# not being available.
+if os.getenv("SCRIV_TEST_NO_EXTRAS", ""):
+    sys.modules["yaml"] = None  # type: ignore[assignment]
+
+# pylint: disable=wrong-import-position
+
 from scriv.cli import cli as scriv_cli
 
 from .faker import FakeGit, FakeRunCommand
 
 
 @pytest.fixture()
 def fake_run_command(mocker):
```

### Comparing `scriv-1.2.1/tests/faker.py` & `scriv-1.3.0/tests/faker.py`

 * *Files identical despite different names*

### Comparing `scriv-1.2.1/tests/helpers.py` & `scriv-1.3.0/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `scriv-1.2.1/tests/test_changelog.py` & `scriv-1.3.0/tests/test_changelog.py`

 * *Files identical despite different names*

### Comparing `scriv-1.2.1/tests/test_collect.py` & `scriv-1.3.0/tests/test_collect.py`

 * *Files 2% similar despite different names*

```diff
@@ -509,7 +509,39 @@
     with freezegun.freeze_time("2022-09-18T16:18:19"):
         result = cli_invoke(["collect"], expect_ok=False)
     assert result.exit_code == 1
     assert (
         str(result.exception)
         == "Entry '12.34.56 — 2022-09-18' already uses version '12.34.56'."
     )
+
+
+def test_duplicate_version_with_v(cli_invoke, changelog_d, temp_dir):
+    (changelog_d / "scriv.ini").write_text("[scriv]\nversion = 12.34.56\n")
+    (temp_dir / "CHANGELOG.rst").write_text(
+        textwrap.dedent(
+            """\
+            Preamble that doesn't count
+
+            v12.34.57 — 2022-09-19
+            ======================
+
+            A quick fix.
+
+            v12.34.56 — 2022-09-18
+            ======================
+
+            Good stuff.
+            """
+        ),
+        encoding="utf-8",
+    )
+
+    # Make a new fragment, and collect again without changing the version.
+    (changelog_d / "20170617_nedbat.rst").write_text(FRAG2)
+    with freezegun.freeze_time("2022-09-18T16:18:19"):
+        result = cli_invoke(["collect"], expect_ok=False)
+    assert result.exit_code == 1
+    assert (
+        str(result.exception)
+        == "Entry 'v12.34.56 — 2022-09-18' already uses version '12.34.56'."
+    )
```

### Comparing `scriv-1.2.1/tests/test_config.py` & `scriv-1.3.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `scriv-1.2.1/tests/test_create.py` & `scriv-1.3.0/tests/test_create.py`

 * *Files identical despite different names*

### Comparing `scriv-1.2.1/tests/test_faker.py` & `scriv-1.3.0/tests/test_faker.py`

 * *Files identical despite different names*

### Comparing `scriv-1.2.1/tests/test_format_md.py` & `scriv-1.3.0/tests/test_format_md.py`

 * *Files identical despite different names*

### Comparing `scriv-1.2.1/tests/test_format_rst.py` & `scriv-1.3.0/tests/test_format_rst.py`

 * *Files identical despite different names*

### Comparing `scriv-1.2.1/tests/test_ghrel.py` & `scriv-1.3.0/tests/test_ghrel.py`

 * *Files identical despite different names*

### Comparing `scriv-1.2.1/tests/test_github.py` & `scriv-1.3.0/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `scriv-1.2.1/tests/test_gitinfo.py` & `scriv-1.3.0/tests/test_gitinfo.py`

 * *Files identical despite different names*

### Comparing `scriv-1.2.1/tests/test_literals.py` & `scriv-1.3.0/tests/test_literals.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,32 @@
 """Tests of literals.py"""
 
+import os
+import sys
+
 import pytest
 
 import scriv.literals
 from scriv.exceptions import ScrivException
 from scriv.literals import find_literal
 from scriv.optional import tomllib, yaml
 
+
+def test_no_extras_craziness():
+    # Check that if we're testing no-extras we didn't get the modules, and if we
+    # aren't, then we did get the modules.
+    if os.getenv("SCRIV_TEST_NO_EXTRAS", ""):
+        if sys.version_info < (3, 11):
+            assert tomllib is None
+        assert yaml is None
+    else:
+        assert tomllib is not None
+        assert yaml is not None
+
+
 PYTHON_CODE = """\
 # A string we should get.
 version = "1.2.3"
 
 typed_version: Final[str] = "2.3.4"
 
 # Numbers don't count.
@@ -151,7 +167,51 @@
 
 def test_find_yaml_literal_fail_if_unavailable(monkeypatch):
     monkeypatch.setattr(scriv.literals, "yaml", None)
     with pytest.raises(
         ScrivException, match="Can't read .+ without YAML support"
     ):
         find_literal("foo.yml", "fail")
+
+
+CFG_LITERAL = """\
+
+[metadata]
+name = myproduct
+version = 1.2.3
+url = https://github.com/nedbat/scriv
+description = A nice description
+long_description = file: README.md
+long_description_content_type = text/markdown
+license = MIT
+
+[options]
+zip_safe = false
+include_package_data = true
+
+[bdist_wheel]
+universal = true
+
+[coverage:report]
+show_missing = true
+
+[flake8]
+max-line-length = 99
+doctests = True
+exclude =  .git, .eggs, __pycache__, tests/, docs/, build/, dist/
+"""
+
+
+@pytest.mark.parametrize(
+    "name, value",
+    [
+        ("metadata.version", "1.2.3"),
+        ("options.zip_safe", "false"),
+        ("coverage:report", None),  # find_literal only supports string values
+        ("metadata.myVersion", None),
+        ("unexisting", None),
+    ],
+)
+def test_find_cfg_literal(name, value, temp_dir):
+    with open("foo.cfg", "w", encoding="utf-8") as f:
+        f.write(CFG_LITERAL)
+    assert find_literal("foo.cfg", name) == value
```

### Comparing `scriv-1.2.1/tox.ini` & `scriv-1.3.0/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,19 @@
 extras =
     !no_extras: toml,yaml
 allowlist_externals =
     make
     rm
 passenv =
     COVERAGE_*
+setenv =
+    no_extras: SCRIV_TEST_NO_EXTRAS=1
 commands =
     python -V
-    no_extras: python -m pip uninstall -q -y tomli pyyaml
+    no_extras: python -m pip uninstall -q -y tomli
     coverage run -p -m pytest -Wd {posargs}
 
 [testenv:coverage]
 depends = py37,py38,py39,py310,py311,pypy3
 basepython = python3.11
 commands =
     coverage combine -q
```

