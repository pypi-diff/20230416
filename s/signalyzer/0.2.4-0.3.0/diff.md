# Comparing `tmp/signalyzer-0.2.4.tar.gz` & `tmp/signalyzer-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signalyzer-0.2.4.tar", last modified: Tue Mar 15 14:01:00 2022, max compression
+gzip compressed data, was "signalyzer-0.3.0.tar", last modified: Sun Apr 16 07:54:59 2023, max compression
```

## Comparing `signalyzer-0.2.4.tar` & `signalyzer-0.3.0.tar`

### file list

```diff
@@ -1,126 +1,109 @@
-drwxrwxrwx   0        0        0        0 2022-03-15 14:01:00.869943 signalyzer-0.2.4/
--rw-rw-rw-   0        0        0      192 2022-01-06 19:41:26.000000 signalyzer-0.2.4/.editorconfig
--rw-rw-rw-   0        0        0       62 2022-01-28 05:29:40.000000 signalyzer-0.2.4/.gitattributes
--rw-rw-rw-   0        0        0      186 2022-01-06 19:45:17.000000 signalyzer-0.2.4/.gitignore
--rw-rw-rw-   0        0        0     1023 2022-02-19 02:54:25.000000 signalyzer-0.2.4/.gitlab-ci.yml
--rw-rw-rw-   0        0        0      176 2022-01-06 21:09:10.000000 signalyzer-0.2.4/.pypirc
--rw-rw-rw-   0        0        0      359 2022-01-06 19:25:31.000000 signalyzer-0.2.4/.readthedocs.yaml
--rw-rw-rw-   0        0        0     2780 2022-03-15 14:00:35.000000 signalyzer-0.2.4/CHANGELOG.rst
--rw-rw-rw-   0        0        0    11066 2022-01-22 07:29:06.000000 signalyzer-0.2.4/CONTRIBUTING.md
--rw-rw-rw-   0        0        0     1496 2022-01-15 05:25:35.000000 signalyzer-0.2.4/LICENSE
--rw-rw-rw-   0        0        0      231 2022-01-14 03:18:38.000000 signalyzer-0.2.4/MANIFEST.in
--rw-rw-rw-   0        0        0     8812 2022-03-15 14:01:00.870973 signalyzer-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     7072 2022-03-12 06:02:01.000000 signalyzer-0.2.4/README.md
-drwxrwxrwx   0        0        0        0 2022-03-15 14:00:59.584478 signalyzer-0.2.4/assets/
-drwxrwxrwx   0        0        0        0 2022-03-15 14:00:59.596459 signalyzer-0.2.4/assets/banner/
--rw-rw-rw-   0        0        0    32601 2022-01-07 14:07:01.000000 signalyzer-0.2.4/assets/banner/banner.png
-drwxrwxrwx   0        0        0        0 2022-03-15 14:00:59.691446 signalyzer-0.2.4/assets/icons/
--rw-rw-rw-   0        0        0     1150 2022-01-07 11:37:25.000000 signalyzer-0.2.4/assets/icons/favicon_16x16.ico
--rw-rw-rw-   0        0        0      994 2022-01-07 11:36:00.000000 signalyzer-0.2.4/assets/icons/favicon_16x16.png
--rw-rw-rw-   0        0        0     4286 2022-01-07 11:37:03.000000 signalyzer-0.2.4/assets/icons/favicon_32x32.ico
--rw-rw-rw-   0        0        0     2194 2022-01-07 11:35:46.000000 signalyzer-0.2.4/assets/icons/favicon_32x32.png
--rw-rw-rw-   0        0        0    16958 2022-01-07 11:33:07.000000 signalyzer-0.2.4/assets/icons/favicon_64x64.ico
--rw-rw-rw-   0        0        0     5487 2022-01-07 11:31:31.000000 signalyzer-0.2.4/assets/icons/favicon_64x64.png
-drwxrwxrwx   0        0        0        0 2022-03-15 14:00:59.720577 signalyzer-0.2.4/assets/logo/
--rw-rw-rw-   0        0        0    26733 2022-01-07 13:38:43.000000 signalyzer-0.2.4/assets/logo/logo.png
--rw-rw-rw-   0        0        0    22588 2022-01-07 14:02:53.000000 signalyzer-0.2.4/assets/logo/logo.svg
--rw-rw-rw-   0        0        0    19632 2022-01-07 14:08:14.000000 signalyzer-0.2.4/assets/signalyzer.svg
-drwxrwxrwx   0        0        0        0 2022-03-15 14:00:59.804505 signalyzer-0.2.4/docs/
--rw-rw-rw-   0        0        0      654 2021-05-02 07:55:52.000000 signalyzer-0.2.4/docs/Makefile
-drwxrwxrwx   0        0        0        0 2022-03-15 14:00:59.437460 signalyzer-0.2.4/docs/_static/
-drwxrwxrwx   0        0        0        0 2022-03-15 14:00:59.865428 signalyzer-0.2.4/docs/_static/images/
--rw-rw-rw-   0        0        0    32601 2022-01-07 14:07:01.000000 signalyzer-0.2.4/docs/_static/images/banner.png
--rw-rw-rw-   0        0        0     1150 2022-01-07 11:37:25.000000 signalyzer-0.2.4/docs/_static/images/favicon.ico
--rw-rw-rw-   0        0        0    26733 2022-01-07 13:38:43.000000 signalyzer-0.2.4/docs/_static/images/logo.png
--rw-rw-rw-   0        0        0    19632 2022-01-07 14:08:14.000000 signalyzer-0.2.4/docs/_static/images/signalyzer.svg
-drwxrwxrwx   0        0        0        0 2022-03-15 14:00:59.898398 signalyzer-0.2.4/docs/annex/
--rw-rw-rw-   0        0        0       64 2022-01-06 13:22:07.000000 signalyzer-0.2.4/docs/annex/changelog.rst
--rw-rw-rw-   0        0        0     1478 2022-01-08 06:02:32.000000 signalyzer-0.2.4/docs/annex/contributing.rst
--rw-rw-rw-   0        0        0      431 2022-01-06 13:23:28.000000 signalyzer-0.2.4/docs/annex/license.rst
-drwxrwxrwx   0        0        0        0 2022-03-15 14:00:59.911395 signalyzer-0.2.4/docs/api/
--rw-rw-rw-   0        0        0     2115 2022-03-05 15:49:15.000000 signalyzer-0.2.4/docs/api/index.rst
-drwxrwxrwx   0        0        0        0 2022-03-15 14:01:00.046431 signalyzer-0.2.4/docs/collections/
--rw-rw-rw-   0        0        0    10593 2022-02-01 04:03:27.000000 signalyzer-0.2.4/docs/collections/exponential-smoothing-traces.rst
--rw-rw-rw-   0        0        0     3942 2022-01-27 03:26:36.000000 signalyzer-0.2.4/docs/collections/index.rst
--rw-rw-rw-   0        0        0    10569 2022-01-06 13:22:08.000000 signalyzer-0.2.4/docs/collections/linear-regression-traces.rst
--rw-rw-rw-   0        0        0    12123 2022-01-27 05:06:11.000000 signalyzer-0.2.4/docs/collections/set-traces.rst
--rw-rw-rw-   0        0        0     2885 2022-01-15 11:24:22.000000 signalyzer-0.2.4/docs/collections/slew-rate-limiter-traces.rst
--rw-rw-rw-   0        0        0    12216 2022-01-27 04:43:01.000000 signalyzer-0.2.4/docs/collections/statistics-traces.rst
--rw-rw-rw-   0        0        0     7114 2022-01-09 07:15:15.000000 signalyzer-0.2.4/docs/collections/vector-traces.rst
--rw-rw-rw-   0        0        0     2887 2022-03-15 14:00:35.000000 signalyzer-0.2.4/docs/conf.py
--rw-rw-rw-   0        0        0       49 2021-05-02 07:55:52.000000 signalyzer-0.2.4/docs/genindex.rst
--rw-rw-rw-   0        0        0     4545 2022-03-12 07:56:17.000000 signalyzer-0.2.4/docs/index.rst
--rwxrwxrwx   0        0        0      791 2022-01-14 03:31:54.000000 signalyzer-0.2.4/docs/make.bat
-drwxrwxrwx   0        0        0        0 2022-03-15 14:01:00.304397 signalyzer-0.2.4/docs/processing/
--rw-rw-rw-   0        0        0     2711 2022-03-05 14:08:13.000000 signalyzer-0.2.4/docs/processing/change-rate-limiting.rst
--rw-rw-rw-   0        0        0     5849 2022-01-27 04:17:23.000000 signalyzer-0.2.4/docs/processing/clipping.rst
--rw-rw-rw-   0        0        0     2699 2022-01-16 10:04:58.000000 signalyzer-0.2.4/docs/processing/dt1-element.rst
--rw-rw-rw-   0        0        0     3691 2022-01-22 05:52:50.000000 signalyzer-0.2.4/docs/processing/exponential-smoothing.rst
--rw-rw-rw-   0        0        0     9291 2022-01-08 12:45:35.000000 signalyzer-0.2.4/docs/processing/iir-filters.rst
--rw-rw-rw-   0        0        0     3234 2022-03-13 06:23:06.000000 signalyzer-0.2.4/docs/processing/index.rst
--rw-rw-rw-   0        0        0     4306 2022-03-13 06:32:45.000000 signalyzer-0.2.4/docs/processing/logic-functions.rst
--rw-rw-rw-   0        0        0     3042 2022-01-08 12:32:58.000000 signalyzer-0.2.4/docs/processing/moving-averages.rst
--rw-rw-rw-   0        0        0     2205 2022-01-15 08:26:08.000000 signalyzer-0.2.4/docs/processing/moving-differentiation.rst
--rw-rw-rw-   0        0        0     1209 2022-03-12 07:03:27.000000 signalyzer-0.2.4/docs/processing/moving-events.rst
--rw-rw-rw-   0        0        0     3204 2022-01-07 12:16:22.000000 signalyzer-0.2.4/docs/processing/moving-linear-regression.rst
--rw-rw-rw-   0        0        0     2690 2022-01-16 09:54:44.000000 signalyzer-0.2.4/docs/processing/pt1-element.rst
--rw-rw-rw-   0        0        0     1609 2022-01-15 12:48:04.000000 signalyzer-0.2.4/docs/processing/slew-rate-limiter.rst
--rw-rw-rw-   0        0        0     5424 2022-01-30 07:38:17.000000 signalyzer-0.2.4/docs/processing/slew-rate-limiting.rst
--rw-rw-rw-   0        0        0      782 2022-01-06 13:22:08.000000 signalyzer-0.2.4/docs/processing/window-generator.rst
--rw-rw-rw-   0        0        0       47 2022-02-19 02:54:25.000000 signalyzer-0.2.4/docs/requirements.txt
-drwxrwxrwx   0        0        0        0 2022-03-15 14:01:00.322430 signalyzer-0.2.4/docs/statemachine/
--rw-rw-rw-   0        0        0    13704 2022-01-21 14:34:40.000000 signalyzer-0.2.4/docs/statemachine/index.rst
-drwxrwxrwx   0        0        0        0 2022-03-15 14:01:00.382369 signalyzer-0.2.4/docs/trace/
--rw-rw-rw-   0        0        0     1318 2022-01-07 16:00:38.000000 signalyzer-0.2.4/docs/trace/conversions.rst
--rw-rw-rw-   0        0        0     2986 2022-01-06 13:22:07.000000 signalyzer-0.2.4/docs/trace/creations.rst
--rw-rw-rw-   0        0        0      753 2022-01-14 03:40:14.000000 signalyzer-0.2.4/docs/trace/index.rst
--rw-rw-rw-   0        0        0     7530 2022-03-13 06:36:09.000000 signalyzer-0.2.4/docs/trace/operations.rst
-drwxrwxrwx   0        0        0        0 2022-03-15 14:01:00.587700 signalyzer-0.2.4/docs/transformations/
--rw-rw-rw-   0        0        0    18105 2022-03-13 09:08:56.000000 signalyzer-0.2.4/docs/transformations/arithmetic_operators.rst
--rw-rw-rw-   0        0        0    15687 2022-01-27 04:17:23.000000 signalyzer-0.2.4/docs/transformations/assignment_operators.rst
--rw-rw-rw-   0        0        0    12537 2022-03-05 16:29:29.000000 signalyzer-0.2.4/docs/transformations/bitwise_operators.rst
--rw-rw-rw-   0        0        0     9595 2022-01-27 04:17:23.000000 signalyzer-0.2.4/docs/transformations/comparison_operators.rst
--rw-rw-rw-   0        0        0     3985 2022-01-27 04:17:23.000000 signalyzer-0.2.4/docs/transformations/differentiating_functions.rst
--rw-rw-rw-   0        0        0     9312 2022-03-13 08:43:26.000000 signalyzer-0.2.4/docs/transformations/index.rst
--rw-rw-rw-   0        0        0     1988 2022-01-06 13:22:08.000000 signalyzer-0.2.4/docs/transformations/integrating_functions.rst
--rw-rw-rw-   0        0        0    11139 2022-01-30 05:15:37.000000 signalyzer-0.2.4/docs/transformations/mathematical_functions.rst
--rw-rw-rw-   0        0        0    21171 2022-01-15 05:10:36.000000 signalyzer-0.2.4/docs/transformations/statistics.rst
--rw-rw-rw-   0        0        0     7563 2022-01-06 13:22:07.000000 signalyzer-0.2.4/docs/transformations/trigonometric_functions.rst
--rw-rw-rw-   0        0        0     4303 2022-01-27 04:24:36.000000 signalyzer-0.2.4/docs/transformations/value_conversions.rst
--rw-rw-rw-   0        0        0     3416 2022-01-27 04:17:23.000000 signalyzer-0.2.4/docs/transformations/x-axis_transformations.rst
--rwxrwxrwx   0        0        0      794 2022-01-14 03:48:19.000000 signalyzer-0.2.4/make.bat
-drwxrwxrwx   0        0        0        0 2022-03-15 14:01:00.602686 signalyzer-0.2.4/notebooks/
--rw-rw-rw-   0        0        0     4328 2022-03-12 16:17:15.000000 signalyzer-0.2.4/notebooks/DFT.ipynb
-drwxrwxrwx   0        0        0        0 2022-03-15 14:01:00.661663 signalyzer-0.2.4/notebooks/chord/
-drwxrwxrwx   0        0        0        0 2022-03-15 14:01:00.719679 signalyzer-0.2.4/notebooks/chord/.ipynb_checkpoints/
--rw-rw-rw-   0        0        0    20443 2022-03-06 06:48:50.000000 signalyzer-0.2.4/notebooks/chord/.ipynb_checkpoints/chord-checkpoint.ipynb
--rw-rw-rw-   0        0        0   210460 2022-03-06 06:48:49.000000 signalyzer-0.2.4/notebooks/chord/.ipynb_checkpoints/chord-diagram-checkpoint.ipynb
--rw-rw-rw-   0        0        0   210460 2022-03-06 06:48:49.000000 signalyzer-0.2.4/notebooks/chord/chord-diagram.ipynb
--rw-rw-rw-   0        0        0    20443 2022-03-06 06:48:50.000000 signalyzer-0.2.4/notebooks/chord/chord.ipynb
-drwxrwxrwx   0        0        0        0 2022-03-15 14:01:00.734692 signalyzer-0.2.4/notebooks/statemachine/
--rw-rw-rw-   0        0        0    15978 2022-03-12 07:49:01.000000 signalyzer-0.2.4/notebooks/statemachine/statemachine.ipynb
-drwxrwxrwx   0        0        0        0 2022-03-15 14:01:00.762748 signalyzer-0.2.4/notebooks/statistics/
--rw-rw-rw-   0        0        0    28409 2022-03-12 07:49:54.000000 signalyzer-0.2.4/notebooks/statistics/statistics.ipynb
-drwxrwxrwx   0        0        0        0 2022-03-15 14:01:00.770700 signalyzer-0.2.4/notebooks/trace/
--rw-rw-rw-   0        0        0   224467 2022-03-12 07:48:21.000000 signalyzer-0.2.4/notebooks/trace/trace.ipynb
--rw-rw-rw-   0        0        0       90 2021-11-17 02:22:26.000000 signalyzer-0.2.4/pyproject.toml
--rw-rw-rw-   0        0        0       53 2022-01-06 13:01:52.000000 signalyzer-0.2.4/requirements.txt
--rw-rw-rw-   0        0        0       11 2022-01-08 10:02:35.000000 signalyzer-0.2.4/runtime.txt
--rw-rw-rw-   0        0        0     1687 2022-03-15 14:01:00.876924 signalyzer-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0       86 2022-01-14 03:10:52.000000 signalyzer-0.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2022-03-15 14:00:59.451470 signalyzer-0.2.4/src/
-drwxrwxrwx   0        0        0        0 2022-03-15 14:01:00.786664 signalyzer-0.2.4/src/signalyzer/
--rw-rw-rw-   0        0        0      856 2022-03-15 14:00:35.000000 signalyzer-0.2.4/src/signalyzer/__init__.py
--rw-rw-rw-   0        0        0      649 2021-05-02 07:55:52.000000 signalyzer-0.2.4/src/signalyzer/constants.py
-drwxrwxrwx   0        0        0        0 2022-03-15 14:01:00.839414 signalyzer-0.2.4/src/signalyzer/statemachine/
--rw-rw-rw-   0        0        0     8238 2022-01-21 14:58:09.000000 signalyzer-0.2.4/src/signalyzer/statemachine/__init__.py
-drwxrwxrwx   0        0        0        0 2022-03-15 14:01:00.866941 signalyzer-0.2.4/src/signalyzer/trace/
--rw-rw-rw-   0        0        0   141251 2022-03-13 10:34:19.000000 signalyzer-0.2.4/src/signalyzer/trace/__init__.py
--rw-rw-rw-   0        0        0      476 2021-11-14 07:02:04.000000 signalyzer-0.2.4/src/signalyzer/types.py
-drwxrwxrwx   0        0        0        0 2022-03-15 14:01:00.813666 signalyzer-0.2.4/src/signalyzer.egg-info/
--rw-rw-rw-   0        0        0     8812 2022-03-15 14:00:57.000000 signalyzer-0.2.4/src/signalyzer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2977 2022-03-15 14:00:59.000000 signalyzer-0.2.4/src/signalyzer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-03-15 14:00:57.000000 signalyzer-0.2.4/src/signalyzer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-03-13 08:25:49.000000 signalyzer-0.2.4/src/signalyzer.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       53 2022-03-15 14:00:57.000000 signalyzer-0.2.4/src/signalyzer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2022-03-15 14:00:57.000000 signalyzer-0.2.4/src/signalyzer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 07:54:59.143488 signalyzer-0.3.0/
+-rw-rw-rw-   0        0        0     3435 2023-04-16 07:45:08.000000 signalyzer-0.3.0/CHANGELOG.rst
+-rw-rw-rw-   0        0        0    11067 2023-04-16 06:14:32.000000 signalyzer-0.3.0/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0     1496 2023-01-14 05:33:16.000000 signalyzer-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0      231 2022-01-14 03:18:38.000000 signalyzer-0.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     8869 2023-04-16 07:54:59.143488 signalyzer-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7130 2023-04-16 06:16:52.000000 signalyzer-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-16 07:54:58.882347 signalyzer-0.3.0/docs/
+-rw-rw-rw-   0        0        0      654 2023-04-16 06:07:55.000000 signalyzer-0.3.0/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-04-16 07:54:58.829711 signalyzer-0.3.0/docs/_static/
+drwxrwxrwx   0        0        0        0 2023-04-16 07:54:58.891312 signalyzer-0.3.0/docs/_static/images/
+-rw-rw-rw-   0        0        0    32601 2023-04-16 06:16:59.000000 signalyzer-0.3.0/docs/_static/images/banner.png
+-rw-rw-rw-   0        0        0     1150 2023-04-16 06:17:33.000000 signalyzer-0.3.0/docs/_static/images/favicon.ico
+-rw-rw-rw-   0        0        0    26733 2023-04-16 06:16:11.000000 signalyzer-0.3.0/docs/_static/images/logo.png
+-rw-rw-rw-   0        0        0    19632 2023-04-16 06:07:55.000000 signalyzer-0.3.0/docs/_static/images/signalyzer.svg
+drwxrwxrwx   0        0        0        0 2023-04-16 07:54:58.897311 signalyzer-0.3.0/docs/annex/
+-rw-rw-rw-   0        0        0       67 2023-04-16 06:12:40.000000 signalyzer-0.3.0/docs/annex/changelog.rst
+-rw-rw-rw-   0        0        0     1512 2023-04-16 06:12:48.000000 signalyzer-0.3.0/docs/annex/contributing.rst
+-rw-rw-rw-   0        0        0      445 2023-04-16 06:13:03.000000 signalyzer-0.3.0/docs/annex/license.rst
+drwxrwxrwx   0        0        0        0 2023-04-16 07:54:58.899314 signalyzer-0.3.0/docs/api/
+-rw-rw-rw-   0        0        0     2411 2023-04-16 06:07:54.000000 signalyzer-0.3.0/docs/api/index.rst
+drwxrwxrwx   0        0        0        0 2023-04-16 07:54:58.917831 signalyzer-0.3.0/docs/collections/
+-rw-rw-rw-   0        0        0     7984 2023-04-16 07:27:08.000000 signalyzer-0.3.0/docs/collections/alpha-beta-filter-traces.rst
+-rw-rw-rw-   0        0        0    11599 2023-04-16 06:07:54.000000 signalyzer-0.3.0/docs/collections/exponential-smoothing-traces.rst
+-rw-rw-rw-   0        0        0     3970 2023-04-16 06:07:54.000000 signalyzer-0.3.0/docs/collections/index.rst
+-rw-rw-rw-   0        0        0    10569 2023-04-16 06:07:54.000000 signalyzer-0.3.0/docs/collections/linear-regression-traces.rst
+-rw-rw-rw-   0        0        0    12123 2023-04-16 06:07:54.000000 signalyzer-0.3.0/docs/collections/set-traces.rst
+-rw-rw-rw-   0        0        0     2885 2023-04-16 06:07:54.000000 signalyzer-0.3.0/docs/collections/slew-rate-limiter-traces.rst
+-rw-rw-rw-   0        0        0    12216 2023-04-16 06:07:54.000000 signalyzer-0.3.0/docs/collections/statistics-traces.rst
+-rw-rw-rw-   0        0        0     7964 2023-04-16 06:07:54.000000 signalyzer-0.3.0/docs/collections/vector-traces.rst
+-rw-rw-rw-   0        0        0     3953 2023-04-16 07:37:09.000000 signalyzer-0.3.0/docs/conf.py
+-rw-rw-rw-   0        0        0       49 2023-04-16 06:13:45.000000 signalyzer-0.3.0/docs/genindex.rst
+-rw-rw-rw-   0        0        0     4600 2023-04-16 07:38:43.000000 signalyzer-0.3.0/docs/index.rst
+-rwxrwxrwx   0        0        0      791 2023-04-16 06:37:33.000000 signalyzer-0.3.0/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-04-16 07:54:58.952344 signalyzer-0.3.0/docs/processing/
+-rw-rw-rw-   0        0        0     2438 2023-04-16 06:50:31.000000 signalyzer-0.3.0/docs/processing/alpha-beta-filter.rst
+-rw-rw-rw-   0        0        0     2711 2023-04-16 06:07:55.000000 signalyzer-0.3.0/docs/processing/change-rate-limiting.rst
+-rw-rw-rw-   0        0        0     5849 2023-04-16 06:07:54.000000 signalyzer-0.3.0/docs/processing/clipping.rst
+-rw-rw-rw-   0        0        0     2699 2023-04-16 06:07:55.000000 signalyzer-0.3.0/docs/processing/dt1-element.rst
+-rw-rw-rw-   0        0        0     3705 2023-04-16 06:07:55.000000 signalyzer-0.3.0/docs/processing/exponential-smoothing.rst
+-rw-rw-rw-   0        0        0     9291 2023-04-16 06:07:54.000000 signalyzer-0.3.0/docs/processing/iir-filters.rst
+-rw-rw-rw-   0        0        0     3351 2023-04-16 06:07:55.000000 signalyzer-0.3.0/docs/processing/index.rst
+-rw-rw-rw-   0        0        0     4310 2023-04-16 06:07:55.000000 signalyzer-0.3.0/docs/processing/logic-functions.rst
+-rw-rw-rw-   0        0        0     3042 2023-04-16 06:07:55.000000 signalyzer-0.3.0/docs/processing/moving-averages.rst
+-rw-rw-rw-   0        0        0     2205 2023-04-16 06:07:54.000000 signalyzer-0.3.0/docs/processing/moving-differentiation.rst
+-rw-rw-rw-   0        0        0     1209 2023-04-16 06:07:55.000000 signalyzer-0.3.0/docs/processing/moving-events.rst
+-rw-rw-rw-   0        0        0     3204 2023-04-16 06:07:54.000000 signalyzer-0.3.0/docs/processing/moving-linear-regression.rst
+-rw-rw-rw-   0        0        0     2690 2023-04-16 06:07:55.000000 signalyzer-0.3.0/docs/processing/pt1-element.rst
+-rw-rw-rw-   0        0        0     1609 2023-04-16 06:07:55.000000 signalyzer-0.3.0/docs/processing/slew-rate-limiter.rst
+-rw-rw-rw-   0        0        0     5424 2023-04-16 06:07:55.000000 signalyzer-0.3.0/docs/processing/slew-rate-limiting.rst
+-rw-rw-rw-   0        0        0      815 2023-04-16 06:20:01.000000 signalyzer-0.3.0/docs/processing/window-generator.rst
+-rw-rw-rw-   0        0        0       87 2023-04-16 06:07:55.000000 signalyzer-0.3.0/docs/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 07:54:58.954344 signalyzer-0.3.0/docs/statemachine/
+-rw-rw-rw-   0        0        0    13704 2023-04-16 06:07:54.000000 signalyzer-0.3.0/docs/statemachine/index.rst
+drwxrwxrwx   0        0        0        0 2023-04-16 07:54:58.961344 signalyzer-0.3.0/docs/trace/
+-rw-rw-rw-   0        0        0     1973 2023-04-16 06:07:55.000000 signalyzer-0.3.0/docs/trace/conversions.rst
+-rw-rw-rw-   0        0        0     3093 2023-04-16 06:14:56.000000 signalyzer-0.3.0/docs/trace/creations.rst
+-rw-rw-rw-   0        0        0      780 2023-04-16 06:17:50.000000 signalyzer-0.3.0/docs/trace/index.rst
+-rw-rw-rw-   0        0        0     7530 2023-04-16 06:07:55.000000 signalyzer-0.3.0/docs/trace/operations.rst
+drwxrwxrwx   0        0        0        0 2023-04-16 07:54:58.986344 signalyzer-0.3.0/docs/transformations/
+-rw-rw-rw-   0        0        0    18105 2023-04-16 06:07:55.000000 signalyzer-0.3.0/docs/transformations/arithmetic_operators.rst
+-rw-rw-rw-   0        0        0    15687 2023-04-16 06:07:55.000000 signalyzer-0.3.0/docs/transformations/assignment_operators.rst
+-rw-rw-rw-   0        0        0    12537 2023-04-16 06:07:54.000000 signalyzer-0.3.0/docs/transformations/bitwise_operators.rst
+-rw-rw-rw-   0        0        0     9595 2023-04-16 06:07:55.000000 signalyzer-0.3.0/docs/transformations/comparison_operators.rst
+-rw-rw-rw-   0        0        0     3985 2023-04-16 06:07:55.000000 signalyzer-0.3.0/docs/transformations/differentiating_functions.rst
+-rw-rw-rw-   0        0        0     9312 2023-04-16 06:07:54.000000 signalyzer-0.3.0/docs/transformations/index.rst
+-rw-rw-rw-   0        0        0     1988 2023-04-16 06:07:55.000000 signalyzer-0.3.0/docs/transformations/integrating_functions.rst
+-rw-rw-rw-   0        0        0    11139 2023-04-16 06:07:55.000000 signalyzer-0.3.0/docs/transformations/mathematical_functions.rst
+-rw-rw-rw-   0        0        0    21171 2023-04-16 06:07:54.000000 signalyzer-0.3.0/docs/transformations/statistics.rst
+-rw-rw-rw-   0        0        0     7562 2023-04-16 06:07:55.000000 signalyzer-0.3.0/docs/transformations/trigonometric_functions.rst
+-rw-rw-rw-   0        0        0     4303 2023-04-16 06:07:54.000000 signalyzer-0.3.0/docs/transformations/value_conversions.rst
+-rw-rw-rw-   0        0        0     3416 2023-04-16 06:07:55.000000 signalyzer-0.3.0/docs/transformations/x-axis_transformations.rst
+-rwxrwxrwx   0        0        0      794 2022-10-31 07:05:54.000000 signalyzer-0.3.0/make.bat
+drwxrwxrwx   0        0        0        0 2023-04-16 07:54:59.000345 signalyzer-0.3.0/notebooks/
+-rw-rw-rw-   0        0        0     4288 2022-08-07 05:20:13.000000 signalyzer-0.3.0/notebooks/DFT.ipynb
+drwxrwxrwx   0        0        0        0 2023-04-16 07:54:59.045304 signalyzer-0.3.0/notebooks/analyzer/
+-rw-rw-rw-   0        0        0  1440630 2022-08-19 15:29:03.000000 signalyzer-0.3.0/notebooks/analyzer/Slope-Velocity-Estimator.pdf
+-rw-rw-rw-   0        0        0   851566 2022-11-04 19:21:31.000000 signalyzer-0.3.0/notebooks/analyzer/analyzer.ipynb
+-rw-rw-rw-   0        0        0   502720 2021-05-02 07:50:32.000000 signalyzer-0.3.0/notebooks/analyzer/recording.csv
+-rw-rw-rw-   0        0        0   137795 2022-11-04 19:21:35.000000 signalyzer-0.3.0/notebooks/analyzer.ipynb
+drwxrwxrwx   0        0        0        0 2023-04-16 07:54:59.066771 signalyzer-0.3.0/notebooks/chord/
+-rw-rw-rw-   0        0        0   210460 2022-03-06 06:48:49.000000 signalyzer-0.3.0/notebooks/chord/chord-diagram.ipynb
+-rw-rw-rw-   0        0        0    20443 2022-03-06 06:48:50.000000 signalyzer-0.3.0/notebooks/chord/chord.ipynb
+drwxrwxrwx   0        0        0        0 2023-04-16 07:54:59.080866 signalyzer-0.3.0/notebooks/statemachine/
+-rw-rw-rw-   0        0        0    15978 2022-03-12 07:49:01.000000 signalyzer-0.3.0/notebooks/statemachine/statemachine.ipynb
+drwxrwxrwx   0        0        0        0 2023-04-16 07:54:59.093488 signalyzer-0.3.0/notebooks/statistics/
+-rw-rw-rw-   0        0        0    28409 2022-03-12 07:49:54.000000 signalyzer-0.3.0/notebooks/statistics/statistics.ipynb
+drwxrwxrwx   0        0        0        0 2023-04-16 07:54:59.103866 signalyzer-0.3.0/notebooks/trace/
+-rw-rw-rw-   0        0        0   225473 2022-10-31 07:03:51.000000 signalyzer-0.3.0/notebooks/trace/trace.ipynb
+-rw-rw-rw-   0        0        0       90 2021-11-17 02:22:26.000000 signalyzer-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       57 2023-04-15 07:00:47.000000 signalyzer-0.3.0/requirements.txt
+-rw-rw-rw-   0        0        0       12 2023-04-16 06:23:43.000000 signalyzer-0.3.0/runtime.txt
+-rw-rw-rw-   0        0        0     1693 2023-04-16 07:54:59.144949 signalyzer-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0       86 2022-01-14 03:10:52.000000 signalyzer-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 07:54:58.842738 signalyzer-0.3.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-16 07:54:59.123014 signalyzer-0.3.0/src/signalyzer/
+-rw-rw-rw-   0        0        0     1008 2023-04-16 07:34:22.000000 signalyzer-0.3.0/src/signalyzer/__init__.py
+-rw-rw-rw-   0        0        0      622 2022-08-25 18:11:34.000000 signalyzer-0.3.0/src/signalyzer/constants.py
+drwxrwxrwx   0        0        0        0 2023-04-16 07:54:59.138691 signalyzer-0.3.0/src/signalyzer/statemachine/
+-rw-rw-rw-   0        0        0     8398 2023-04-15 07:57:02.000000 signalyzer-0.3.0/src/signalyzer/statemachine/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 07:54:59.140709 signalyzer-0.3.0/src/signalyzer/trace/
+-rw-rw-rw-   0        0        0   154446 2023-04-16 07:34:22.000000 signalyzer-0.3.0/src/signalyzer/trace/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 07:54:59.135688 signalyzer-0.3.0/src/signalyzer.egg-info/
+-rw-rw-rw-   0        0        0     8869 2023-04-16 07:54:58.000000 signalyzer-0.3.0/src/signalyzer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2697 2023-04-16 07:54:58.000000 signalyzer-0.3.0/src/signalyzer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 07:54:58.000000 signalyzer-0.3.0/src/signalyzer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-16 06:46:52.000000 signalyzer-0.3.0/src/signalyzer.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       57 2023-04-16 07:54:58.000000 signalyzer-0.3.0/src/signalyzer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-16 07:54:58.000000 signalyzer-0.3.0/src/signalyzer.egg-info/top_level.txt
```

### Comparing `signalyzer-0.2.4/CHANGELOG.rst` & `signalyzer-0.3.0/CHANGELOG.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,51 @@
 Change Log
 **********
 
 These are the enhancements, breaking changes and bug fixes of note between each
 release.
 
+.. _v0.3.0:
+
+`0.3.0`_ - 2023-04-16
+=====================
+
+.. _0.3.0: https://gitlab.com/signalytics/signalyzer/compare/v0.2.4..._v0.3.0:
+
+Enhancements
+------------
+
+* Add method :meth:`~Trace.alpha_beta_filter` to filter a measured signal with
+  an alpha-beta filter.
+* Add dataclass :class:`AlphaBetaFilterTraces` for the trace collection produced
+  by an alpha-beta filter.
+* Add dataclass :class:`AlphaBetaFilter` for the results produced by the
+  alpha-beta filter.
+* Add :attr:`~VectorTraces.delta_phi` trace to the vector trace collection.
+* Upgrade type hints to new convention.
+
+
+Breaking Changes
+----------------
+
+* Drop support for Python 3.9.
+
 .. _v0.2.4:
 
 `0.2.4`_ - 2022-03-15
 =====================
 
 .. _0.2.4: https://gitlab.com/signalytics/signalyzer/compare/v0.2.3...v0.2.4
 
 Enhancements
 ------------
 
 * Add method :meth:`~Trace.moving_events` to count the occurrences of an event
   in form of a sample value within a moving window over the samples.
-* Add method :meth:`~Trace.fmod` to module divide the signal samples.
+* Add method :meth:`~Trace.fmod` to modulo divide the signal samples.
 
 .. _v0.2.3:
 
 `0.2.3`_ - 2022-03-06
 =====================
 
 .. _0.2.3: https://gitlab.com/signalytics/signalyzer/compare/v0.2.2...v0.2.3
```

### Comparing `signalyzer-0.2.4/CONTRIBUTING.md` & `signalyzer-0.3.0/CONTRIBUTING.md`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 ```shell
 > git config --global user.name "your user name"
 > git config --global user.email "your@email.com"
 ```
 
 #### Step 2: Build
 
-The `signalyzer` package requires at least [Python] 3.9 and depends on the
+The `signalyzer` package requires at least [Python] 3.10 and depends on the
 external packages:
 
 - [numpy](https://pypi.org/project/numpy)
 - [scipy](https://pypi.org/project/scipy)
 - [pandas](https://pypi.org/project/pandas)
 - [plotly](https://pypi.org/project/plotly)
```

### Comparing `signalyzer-0.2.4/LICENSE` & `signalyzer-0.3.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2021-2022 by Jochen Gerhaeusser.
+Copyright (c) 2021-2023 by Jochen Gerhaeusser.
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `signalyzer-0.2.4/PKG-INFO` & `signalyzer-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signalyzer
-Version: 0.2.4
+Version: 0.3.0
 Summary: Signal analyzer for time-discrete, equidistant measured signals
 Home-page: https://gitlab.com/signalytics/signalyzer/
 Download-URL: https://gitlab.com/signalytics/signalyzer/-/packages
 Author: Jochen Gerhaeusser
 Author-email: jochen_privat@gmx.de
 License: BSD-3-Clause
 Project-URL: Issue Tracker, https://gitlab.com/signalytics/signalyzer/-/issues/
@@ -17,21 +17,21 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Education
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Visualization
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
   <img src="https://signalytics.gitlab.io/signalyzer/_static/images/signalyzer.svg"><br>
 </div>
 
@@ -71,16 +71,16 @@
 * moving OLS linear regression with window statistics
 * shifting (moving) of the measured signal
 * slicing of the measured signal
 * evaluate statemachine transitions observed by measured state signal
 
 > **Important**: The **signalyzer** package is best used within [JupyterLab] a
 > web-based interactive development environment for [Jupyter] notebooks or with
-> Plotly [Dash] or Jupyter [voila] to build standalone web applications and
-> dashboards.
+> Plotly [Dash], [Streamlit] or Jupyter [voila] to build standalone web
+> applications and dashboards.
 
 ## Table of Contents
 [Back to top]: #table-of-contents
 
 1. [Project Status](#project-status)
 2. [Project Structure](#project-structure)
 3. [Getting Started](#getting-started)
@@ -96,36 +96,36 @@
 6. [Documentation](#documentation)
 7. [Contributing](#contributing)
 8. [License](#license)
 9. [Authors](#authors)
 
 ## Project Status
 
-This [project] is a work in progress and far away from stable.
-Feedback is always welcomed!
+This [project] is stable and active. Feedback is always welcomed!
 
 **[Back to top](#table-of-contents)**
 
 ## Project Structure
 
 The [project] is organized in sub-folders.
 
+- `assets`: [Project] assets files
 - `docs/`: [Sphinx] documentation
 - `notebooks/`: [Jupyter] notebooks
 - `src/signalyzer/`: Package sources
   - `signalyzer/trace`: Trace module sources
   - `signalyzer/statemachine`: Statemachine module sources
 
 **[Back to top](#table-of-contents)**
 
 ## Getting Started
 
 ### Dependencies
 
-The `signalyzer` package requires at least [Python] 3.9 and depends on the
+The `signalyzer` package requires at least [Python] 3.10 and depends on the
 external packages:
 
 - [numpy]
 - [scipy]
 - [pandas]
 - [plotly]
 
@@ -244,19 +244,18 @@
 [sphinx-plotly-directive]: https://pypi.org/project/sphinx-plotly-directive
 [numpy]: https://pypi.org/project/numpy
 [scipy]: https://pypi.org/project/scipy
 [pandas]: https://pypi.org/project/pandas
 [plotly]: https://pypi.org/project/plotly
 [voila]: https://voila.readthedocs.io
 [dash]: https://dash.plotly.com/
+[streamlit]: https://streamlit.io/
 [JupyterLab]: https://jupyter.org
 [Jupyter]: https://jupyter.org
 [gitlab]: https://gitlab.com
 [project]: https://gitlab.com/signalytics/signalyzer
 [PyPI package registry]: https://gitlab.com/signalytics/signalyzer/-/packages
 [repository tag list]: https://gitlab.com/signalytics/signalyzer/-/tags
 [contributors]: https://gitlab.com/signalytics/signalyzer/-/graphs/main
 [GitLab Pages]: https://signalytics.gitlab.io/signalyzer
 [installation guide]: https://signalytics.gitlab.io/signalyzer/intro.html#installation
 [Read The Docs]: https://signalyzer.readthedocs.io
-
-
```

### Comparing `signalyzer-0.2.4/README.md` & `signalyzer-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -38,16 +38,16 @@
 * moving OLS linear regression with window statistics
 * shifting (moving) of the measured signal
 * slicing of the measured signal
 * evaluate statemachine transitions observed by measured state signal
 
 > **Important**: The **signalyzer** package is best used within [JupyterLab] a
 > web-based interactive development environment for [Jupyter] notebooks or with
-> Plotly [Dash] or Jupyter [voila] to build standalone web applications and
-> dashboards.
+> Plotly [Dash], [Streamlit] or Jupyter [voila] to build standalone web
+> applications and dashboards.
 
 ## Table of Contents
 [Back to top]: #table-of-contents
 
 1. [Project Status](#project-status)
 2. [Project Structure](#project-structure)
 3. [Getting Started](#getting-started)
@@ -63,36 +63,36 @@
 6. [Documentation](#documentation)
 7. [Contributing](#contributing)
 8. [License](#license)
 9. [Authors](#authors)
 
 ## Project Status
 
-This [project] is a work in progress and far away from stable.
-Feedback is always welcomed!
+This [project] is stable and active. Feedback is always welcomed!
 
 **[Back to top](#table-of-contents)**
 
 ## Project Structure
 
 The [project] is organized in sub-folders.
 
+- `assets`: [Project] assets files
 - `docs/`: [Sphinx] documentation
 - `notebooks/`: [Jupyter] notebooks
 - `src/signalyzer/`: Package sources
   - `signalyzer/trace`: Trace module sources
   - `signalyzer/statemachine`: Statemachine module sources
 
 **[Back to top](#table-of-contents)**
 
 ## Getting Started
 
 ### Dependencies
 
-The `signalyzer` package requires at least [Python] 3.9 and depends on the
+The `signalyzer` package requires at least [Python] 3.10 and depends on the
 external packages:
 
 - [numpy]
 - [scipy]
 - [pandas]
 - [plotly]
 
@@ -211,14 +211,15 @@
 [sphinx-plotly-directive]: https://pypi.org/project/sphinx-plotly-directive
 [numpy]: https://pypi.org/project/numpy
 [scipy]: https://pypi.org/project/scipy
 [pandas]: https://pypi.org/project/pandas
 [plotly]: https://pypi.org/project/plotly
 [voila]: https://voila.readthedocs.io
 [dash]: https://dash.plotly.com/
+[streamlit]: https://streamlit.io/
 [JupyterLab]: https://jupyter.org
 [Jupyter]: https://jupyter.org
 [gitlab]: https://gitlab.com
 [project]: https://gitlab.com/signalytics/signalyzer
 [PyPI package registry]: https://gitlab.com/signalytics/signalyzer/-/packages
 [repository tag list]: https://gitlab.com/signalytics/signalyzer/-/tags
 [contributors]: https://gitlab.com/signalytics/signalyzer/-/graphs/main
```

### Comparing `signalyzer-0.2.4/assets/banner/banner.png` & `signalyzer-0.3.0/docs/_static/images/banner.png`

 * *Files identical despite different names*

### Comparing `signalyzer-0.2.4/assets/icons/favicon_16x16.ico` & `signalyzer-0.3.0/docs/_static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `signalyzer-0.2.4/assets/logo/logo.png` & `signalyzer-0.3.0/docs/_static/images/logo.png`

 * *Files identical despite different names*

### Comparing `signalyzer-0.2.4/assets/logo/logo.svg` & `signalyzer-0.3.0/docs/_static/images/signalyzer.svg`

 * *Files 9% similar despite different names*

```diff
@@ -2,1411 +2,1226 @@
 00000010: 2e30 2220 656e 636f 6469 6e67 3d22 5554  .0" encoding="UT
 00000020: 462d 3822 2073 7461 6e64 616c 6f6e 653d  F-8" standalone=
 00000030: 226e 6f22 3f3e 0a3c 212d 2d20 4372 6561  "no"?>.<!-- Crea
 00000040: 7465 6420 7769 7468 2049 6e6b 7363 6170  ted with Inkscap
 00000050: 6520 2868 7474 703a 2f2f 7777 772e 696e  e (http://www.in
 00000060: 6b73 6361 7065 2e6f 7267 2f29 202d 2d3e  kscape.org/) -->
 00000070: 0a0a 3c73 7667 0a20 2020 7769 6474 683d  ..<svg.   width=
-00000080: 2235 306d 6d22 0a20 2020 6865 6967 6874  "50mm".   height
-00000090: 3d22 3530 6d6d 220a 2020 2076 6965 7742  ="50mm".   viewB
-000000a0: 6f78 3d22 3020 3020 3530 2035 3022 0a20  ox="0 0 50 50". 
-000000b0: 2020 7665 7273 696f 6e3d 2231 2e31 220a    version="1.1".
-000000c0: 2020 2069 643d 2273 7667 3932 3222 0a20     id="svg922". 
-000000d0: 2020 696e 6b73 6361 7065 3a76 6572 7369    inkscape:versi
-000000e0: 6f6e 3d22 312e 312e 3120 2833 6266 3561  on="1.1.1 (3bf5a
-000000f0: 6530 6432 352c 2032 3032 312d 3039 2d32  e0d25, 2021-09-2
-00000100: 3029 220a 2020 2073 6f64 6970 6f64 693a  0)".   sodipodi:
-00000110: 646f 636e 616d 653d 226c 6f67 6f2e 7376  docname="logo.sv
-00000120: 6722 0a20 2020 696e 6b73 6361 7065 3a65  g".   inkscape:e
-00000130: 7870 6f72 742d 6669 6c65 6e61 6d65 3d22  xport-filename="
-00000140: 443a 5c57 6f72 6b73 7061 6365 5c44 7261  D:\Workspace\Dra
-00000150: 7769 6e67 735c 6c6f 676f 5f32 3030 7832  wings\logo_200x2
-00000160: 3030 2e70 6e67 220a 2020 2069 6e6b 7363  00.png".   inksc
-00000170: 6170 653a 6578 706f 7274 2d78 6470 693d  ape:export-xdpi=
-00000180: 2231 3031 2e36 220a 2020 2069 6e6b 7363  "101.6".   inksc
-00000190: 6170 653a 6578 706f 7274 2d79 6470 693d  ape:export-ydpi=
-000001a0: 2231 3031 2e36 220a 2020 2078 6d6c 6e73  "101.6".   xmlns
-000001b0: 3a69 6e6b 7363 6170 653d 2268 7474 703a  :inkscape="http:
-000001c0: 2f2f 7777 772e 696e 6b73 6361 7065 2e6f  //www.inkscape.o
-000001d0: 7267 2f6e 616d 6573 7061 6365 732f 696e  rg/namespaces/in
-000001e0: 6b73 6361 7065 220a 2020 2078 6d6c 6e73  kscape".   xmlns
-000001f0: 3a73 6f64 6970 6f64 693d 2268 7474 703a  :sodipodi="http:
-00000200: 2f2f 736f 6469 706f 6469 2e73 6f75 7263  //sodipodi.sourc
-00000210: 6566 6f72 6765 2e6e 6574 2f44 5444 2f73  eforge.net/DTD/s
-00000220: 6f64 6970 6f64 692d 302e 6474 6422 0a20  odipodi-0.dtd". 
-00000230: 2020 786d 6c6e 733d 2268 7474 703a 2f2f    xmlns="http://
-00000240: 7777 772e 7733 2e6f 7267 2f32 3030 302f  www.w3.org/2000/
-00000250: 7376 6722 0a20 2020 786d 6c6e 733a 7376  svg".   xmlns:sv
-00000260: 673d 2268 7474 703a 2f2f 7777 772e 7733  g="http://www.w3
-00000270: 2e6f 7267 2f32 3030 302f 7376 6722 0a20  .org/2000/svg". 
-00000280: 2020 786d 6c6e 733a 7264 663d 2268 7474    xmlns:rdf="htt
-00000290: 703a 2f2f 7777 772e 7733 2e6f 7267 2f31  p://www.w3.org/1
-000002a0: 3939 392f 3032 2f32 322d 7264 662d 7379  999/02/22-rdf-sy
-000002b0: 6e74 6178 2d6e 7323 220a 2020 2078 6d6c  ntax-ns#".   xml
-000002c0: 6e73 3a63 633d 2268 7474 703a 2f2f 6372  ns:cc="http://cr
-000002d0: 6561 7469 7665 636f 6d6d 6f6e 732e 6f72  eativecommons.or
-000002e0: 672f 6e73 2322 0a20 2020 786d 6c6e 733a  g/ns#".   xmlns:
-000002f0: 6463 3d22 6874 7470 3a2f 2f70 7572 6c2e  dc="http://purl.
-00000300: 6f72 672f 6463 2f65 6c65 6d65 6e74 732f  org/dc/elements/
-00000310: 312e 312f 223e 0a20 203c 7469 746c 650a  1.1/">.  <title.
-00000320: 2020 2020 2069 643d 2274 6974 6c65 3930       id="title90
-00000330: 3122 3e53 6967 6e61 6c79 7a65 7220 4c6f  1">Signalyzer Lo
-00000340: 676f 3c2f 7469 746c 653e 0a20 203c 736f  go</title>.  <so
-00000350: 6469 706f 6469 3a6e 616d 6564 7669 6577  dipodi:namedview
-00000360: 0a20 2020 2020 6964 3d22 6e61 6d65 6476  .     id="namedv
-00000370: 6965 7739 3234 220a 2020 2020 2070 6167  iew924".     pag
-00000380: 6563 6f6c 6f72 3d22 2366 6666 6666 6622  ecolor="#ffffff"
-00000390: 0a20 2020 2020 626f 7264 6572 636f 6c6f  .     bordercolo
-000003a0: 723d 2223 3939 3939 3939 220a 2020 2020  r="#999999".    
-000003b0: 2062 6f72 6465 726f 7061 6369 7479 3d22   borderopacity="
-000003c0: 3122 0a20 2020 2020 696e 6b73 6361 7065  1".     inkscape
-000003d0: 3a70 6167 6573 6861 646f 773d 2230 220a  :pageshadow="0".
-000003e0: 2020 2020 2069 6e6b 7363 6170 653a 7061       inkscape:pa
-000003f0: 6765 6f70 6163 6974 793d 2230 220a 2020  geopacity="0".  
-00000400: 2020 2069 6e6b 7363 6170 653a 7061 6765     inkscape:page
-00000410: 6368 6563 6b65 7262 6f61 7264 3d22 3022  checkerboard="0"
-00000420: 0a20 2020 2020 696e 6b73 6361 7065 3a64  .     inkscape:d
-00000430: 6f63 756d 656e 742d 756e 6974 733d 226d  ocument-units="m
-00000440: 6d22 0a20 2020 2020 7368 6f77 6772 6964  m".     showgrid
-00000450: 3d22 7472 7565 220a 2020 2020 2073 686f  ="true".     sho
-00000460: 7767 7569 6465 733d 2266 616c 7365 220a  wguides="false".
-00000470: 2020 2020 2069 6e6b 7363 6170 653a 6775       inkscape:gu
-00000480: 6964 652d 6262 6f78 3d22 7472 7565 220a  ide-bbox="true".
-00000490: 2020 2020 2069 6e6b 7363 6170 653a 7a6f       inkscape:zo
-000004a0: 6f6d 3d22 3222 0a20 2020 2020 696e 6b73  om="2".     inks
-000004b0: 6361 7065 3a63 783d 2232 3836 2e37 3522  cape:cx="286.75"
-000004c0: 0a20 2020 2020 696e 6b73 6361 7065 3a63  .     inkscape:c
-000004d0: 793d 2231 3135 2e37 3522 0a20 2020 2020  y="115.75".     
-000004e0: 696e 6b73 6361 7065 3a77 696e 646f 772d  inkscape:window-
-000004f0: 7769 6474 683d 2232 3536 3022 0a20 2020  width="2560".   
-00000500: 2020 696e 6b73 6361 7065 3a77 696e 646f    inkscape:windo
-00000510: 772d 6865 6967 6874 3d22 3133 3631 220a  w-height="1361".
-00000520: 2020 2020 2069 6e6b 7363 6170 653a 7769       inkscape:wi
-00000530: 6e64 6f77 2d78 3d22 2d39 220a 2020 2020  ndow-x="-9".    
-00000540: 2069 6e6b 7363 6170 653a 7769 6e64 6f77   inkscape:window
-00000550: 2d79 3d22 2d39 220a 2020 2020 2069 6e6b  -y="-9".     ink
-00000560: 7363 6170 653a 7769 6e64 6f77 2d6d 6178  scape:window-max
-00000570: 696d 697a 6564 3d22 3122 0a20 2020 2020  imized="1".     
-00000580: 696e 6b73 6361 7065 3a63 7572 7265 6e74  inkscape:current
-00000590: 2d6c 6179 6572 3d22 6c61 7965 7234 220a  -layer="layer4".
-000005a0: 2020 2020 2069 6e6b 7363 6170 653a 6c6f       inkscape:lo
-000005b0: 636b 6775 6964 6573 3d22 7472 7565 220a  ckguides="true".
-000005c0: 2020 2020 2069 6e6b 7363 6170 653a 6f62       inkscape:ob
-000005d0: 6a65 6374 2d70 6174 6873 3d22 7472 7565  ject-paths="true
-000005e0: 220a 2020 2020 2069 6e6b 7363 6170 653a  ".     inkscape:
-000005f0: 736e 6170 2d69 6e74 6572 7365 6374 696f  snap-intersectio
-00000600: 6e2d 7061 7468 733d 2274 7275 6522 0a20  n-paths="true". 
-00000610: 2020 2020 696e 6b73 6361 7065 3a73 6e61      inkscape:sna
-00000620: 702d 736d 6f6f 7468 2d6e 6f64 6573 3d22  p-smooth-nodes="
-00000630: 7472 7565 220a 2020 2020 2069 6e6b 7363  true".     inksc
-00000640: 6170 653a 736e 6170 2d6d 6964 706f 696e  ape:snap-midpoin
-00000650: 7473 3d22 7472 7565 220a 2020 2020 2069  ts="true".     i
-00000660: 6e6b 7363 6170 653a 736e 6170 2d6f 626a  nkscape:snap-obj
-00000670: 6563 742d 6d69 6470 6f69 6e74 733d 2274  ect-midpoints="t
-00000680: 7275 6522 0a20 2020 2020 696e 6b73 6361  rue".     inksca
-00000690: 7065 3a73 6e61 702d 6365 6e74 6572 3d22  pe:snap-center="
-000006a0: 7472 7565 220a 2020 2020 2069 6e6b 7363  true".     inksc
-000006b0: 6170 653a 736e 6170 2d62 626f 783d 2274  ape:snap-bbox="t
-000006c0: 7275 6522 0a20 2020 2020 696e 6b73 6361  rue".     inksca
-000006d0: 7065 3a62 626f 782d 7061 7468 733d 2274  pe:bbox-paths="t
-000006e0: 7275 6522 0a20 2020 2020 696e 6b73 6361  rue".     inksca
-000006f0: 7065 3a62 626f 782d 6e6f 6465 733d 2274  pe:bbox-nodes="t
-00000700: 7275 6522 0a20 2020 2020 696e 6b73 6361  rue".     inksca
-00000710: 7065 3a73 6e61 702d 6262 6f78 2d65 6467  pe:snap-bbox-edg
-00000720: 652d 6d69 6470 6f69 6e74 733d 2274 7275  e-midpoints="tru
-00000730: 6522 0a20 2020 2020 696e 6b73 6361 7065  e".     inkscape
-00000740: 3a73 6e61 702d 6262 6f78 2d6d 6964 706f  :snap-bbox-midpo
-00000750: 696e 7473 3d22 6661 6c73 6522 0a20 2020  ints="false".   
-00000760: 2020 696e 6b73 6361 7065 3a73 6e61 702d    inkscape:snap-
-00000770: 6772 6964 733d 2274 7275 6522 0a20 2020  grids="true".   
-00000780: 2020 696e 6b73 6361 7065 3a73 6e61 702d    inkscape:snap-
-00000790: 676c 6f62 616c 3d22 7472 7565 220a 2020  global="true".  
-000007a0: 2020 2069 6e6b 7363 6170 653a 736e 6170     inkscape:snap
-000007b0: 2d6e 6f64 6573 3d22 7472 7565 220a 2020  -nodes="true".  
-000007c0: 2020 2069 6e6b 7363 6170 653a 736e 6170     inkscape:snap
-000007d0: 2d6f 7468 6572 733d 2274 7275 6522 0a20  -others="true". 
-000007e0: 2020 2020 696e 6b73 6361 7065 3a73 6e61      inkscape:sna
-000007f0: 702d 746f 2d67 7569 6465 733d 2274 7275  p-to-guides="tru
-00000800: 6522 3e0a 2020 2020 3c73 6f64 6970 6f64  e">.    <sodipod
-00000810: 693a 6775 6964 650a 2020 2020 2020 2070  i:guide.       p
-00000820: 6f73 6974 696f 6e3d 2231 322e 352c 3530  osition="12.5,50
-00000830: 220a 2020 2020 2020 206f 7269 656e 7461  ".       orienta
-00000840: 7469 6f6e 3d22 2d31 2c30 220a 2020 2020  tion="-1,0".    
-00000850: 2020 2069 643d 2267 7569 6465 3333 3537     id="guide3357
-00000860: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
-00000870: 653a 6c61 6265 6c3d 2222 0a20 2020 2020  e:label="".     
-00000880: 2020 696e 6b73 6361 7065 3a6c 6f63 6b65    inkscape:locke
-00000890: 643d 2274 7275 6522 0a20 2020 2020 2020  d="true".       
-000008a0: 696e 6b73 6361 7065 3a63 6f6c 6f72 3d22  inkscape:color="
-000008b0: 7267 6228 302c 302c 3235 3529 2220 2f3e  rgb(0,0,255)" />
-000008c0: 0a20 2020 203c 736f 6469 706f 6469 3a67  .    <sodipodi:g
-000008d0: 7569 6465 0a20 2020 2020 2020 706f 7369  uide.       posi
-000008e0: 7469 6f6e 3d22 342e 3939 3939 3939 3965  tion="4.9999999e
-000008f0: 2d30 372c 3439 2e39 3939 3939 3922 0a20  -07,49.999999". 
-00000900: 2020 2020 2020 6f72 6965 6e74 6174 696f        orientatio
-00000910: 6e3d 2230 2c2d 3122 0a20 2020 2020 2020  n="0,-1".       
-00000920: 6964 3d22 6775 6964 6533 3335 3922 0a20  id="guide3359". 
-00000930: 2020 2020 2020 696e 6b73 6361 7065 3a6c        inkscape:l
-00000940: 6f63 6b65 643d 2274 7275 6522 202f 3e0a  ocked="true" />.
-00000950: 2020 2020 3c73 6f64 6970 6f64 693a 6775      <sodipodi:gu
-00000960: 6964 650a 2020 2020 2020 2070 6f73 6974  ide.       posit
-00000970: 696f 6e3d 2234 2e39 3939 3939 3939 652d  ion="4.9999999e-
-00000980: 3037 2c32 3522 0a20 2020 2020 2020 6f72  07,25".       or
-00000990: 6965 6e74 6174 696f 6e3d 2231 2c30 220a  ientation="1,0".
-000009a0: 2020 2020 2020 2069 643d 2267 7569 6465         id="guide
-000009b0: 3333 3631 220a 2020 2020 2020 2069 6e6b  3361".       ink
-000009c0: 7363 6170 653a 6c6f 636b 6564 3d22 7472  scape:locked="tr
-000009d0: 7565 2220 2f3e 0a20 2020 203c 736f 6469  ue" />.    <sodi
-000009e0: 706f 6469 3a67 7569 6465 0a20 2020 2020  podi:guide.     
-000009f0: 2020 706f 7369 7469 6f6e 3d22 3235 2c32    position="25,2
-00000a00: 3522 0a20 2020 2020 2020 6f72 6965 6e74  5".       orient
-00000a10: 6174 696f 6e3d 2231 2c30 220a 2020 2020  ation="1,0".    
-00000a20: 2020 2069 643d 2267 7569 6465 3333 3633     id="guide3363
-00000a30: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
-00000a40: 653a 6c6f 636b 6564 3d22 7472 7565 2220  e:locked="true" 
-00000a50: 2f3e 0a20 2020 203c 736f 6469 706f 6469  />.    <sodipodi
-00000a60: 3a67 7569 6465 0a20 2020 2020 2020 706f  :guide.       po
-00000a70: 7369 7469 6f6e 3d22 3530 2c32 3522 0a20  sition="50,25". 
-00000a80: 2020 2020 2020 6f72 6965 6e74 6174 696f        orientatio
-00000a90: 6e3d 2231 2c30 220a 2020 2020 2020 2069  n="1,0".       i
-00000aa0: 643d 2267 7569 6465 3333 3635 220a 2020  d="guide3365".  
-00000ab0: 2020 2020 2069 6e6b 7363 6170 653a 6c6f       inkscape:lo
-00000ac0: 636b 6564 3d22 7472 7565 2220 2f3e 0a20  cked="true" />. 
-00000ad0: 2020 203c 736f 6469 706f 6469 3a67 7569     <sodipodi:gui
-00000ae0: 6465 0a20 2020 2020 2020 706f 7369 7469  de.       positi
-00000af0: 6f6e 3d22 3337 2e35 2c35 3022 0a20 2020  on="37.5,50".   
-00000b00: 2020 2020 6f72 6965 6e74 6174 696f 6e3d      orientation=
-00000b10: 222d 312c 3022 0a20 2020 2020 2020 6964  "-1,0".       id
-00000b20: 3d22 6775 6964 6533 3336 3722 0a20 2020  ="guide3367".   
-00000b30: 2020 2020 696e 6b73 6361 7065 3a6c 6162      inkscape:lab
-00000b40: 656c 3d22 220a 2020 2020 2020 2069 6e6b  el="".       ink
-00000b50: 7363 6170 653a 6c6f 636b 6564 3d22 7472  scape:locked="tr
-00000b60: 7565 220a 2020 2020 2020 2069 6e6b 7363  ue".       inksc
-00000b70: 6170 653a 636f 6c6f 723d 2272 6762 2830  ape:color="rgb(0
-00000b80: 2c30 2c32 3535 2922 202f 3e0a 2020 2020  ,0,255)" />.    
-00000b90: 3c73 6f64 6970 6f64 693a 6775 6964 650a  <sodipodi:guide.
-00000ba0: 2020 2020 2020 2070 6f73 6974 696f 6e3d         position=
-00000bb0: 2232 352c 3330 220a 2020 2020 2020 206f  "25,30".       o
-00000bc0: 7269 656e 7461 7469 6f6e 3d22 302c 3122  rientation="0,1"
-00000bd0: 0a20 2020 2020 2020 6964 3d22 6775 6964  .       id="guid
-00000be0: 6533 3336 3922 0a20 2020 2020 2020 696e  e3369".       in
-00000bf0: 6b73 6361 7065 3a6c 6f63 6b65 643d 2274  kscape:locked="t
-00000c00: 7275 6522 0a20 2020 2020 2020 696e 6b73  rue".       inks
-00000c10: 6361 7065 3a6c 6162 656c 3d22 220a 2020  cape:label="".  
-00000c20: 2020 2020 2069 6e6b 7363 6170 653a 636f       inkscape:co
-00000c30: 6c6f 723d 2272 6762 2830 2c30 2c32 3535  lor="rgb(0,0,255
-00000c40: 2922 202f 3e0a 2020 2020 3c73 6f64 6970  )" />.    <sodip
-00000c50: 6f64 693a 6775 6964 650a 2020 2020 2020  odi:guide.      
-00000c60: 2070 6f73 6974 696f 6e3d 2232 352c 3022   position="25,0"
-00000c70: 0a20 2020 2020 2020 6f72 6965 6e74 6174  .       orientat
-00000c80: 696f 6e3d 2230 2c2d 3122 0a20 2020 2020  ion="0,-1".     
-00000c90: 2020 6964 3d22 6775 6964 6533 3337 3122    id="guide3371"
-00000ca0: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
-00000cb0: 3a6c 6f63 6b65 643d 2274 7275 6522 202f  :locked="true" /
-00000cc0: 3e0a 2020 2020 3c73 6f64 6970 6f64 693a  >.    <sodipodi:
-00000cd0: 6775 6964 650a 2020 2020 2020 2070 6f73  guide.       pos
-00000ce0: 6974 696f 6e3d 2234 352c 3530 220a 2020  ition="45,50".  
-00000cf0: 2020 2020 206f 7269 656e 7461 7469 6f6e       orientation
-00000d00: 3d22 2d31 2c30 220a 2020 2020 2020 2069  ="-1,0".       i
-00000d10: 643d 2267 7569 6465 3639 3933 220a 2020  d="guide6993".  
-00000d20: 2020 2020 2069 6e6b 7363 6170 653a 6c61       inkscape:la
-00000d30: 6265 6c3d 2222 0a20 2020 2020 2020 696e  bel="".       in
-00000d40: 6b73 6361 7065 3a6c 6f63 6b65 643d 2274  kscape:locked="t
-00000d50: 7275 6522 0a20 2020 2020 2020 696e 6b73  rue".       inks
-00000d60: 6361 7065 3a63 6f6c 6f72 3d22 7267 6228  cape:color="rgb(
-00000d70: 302c 302c 3235 3529 2220 2f3e 0a20 2020  0,0,255)" />.   
-00000d80: 203c 736f 6469 706f 6469 3a67 7569 6465   <sodipodi:guide
-00000d90: 0a20 2020 2020 2020 706f 7369 7469 6f6e  .       position
-00000da0: 3d22 3232 2e35 2c35 3022 0a20 2020 2020  ="22.5,50".     
-00000db0: 2020 6f72 6965 6e74 6174 696f 6e3d 222d    orientation="-
-00000dc0: 312c 3022 0a20 2020 2020 2020 6964 3d22  1,0".       id="
-00000dd0: 6775 6964 6531 3236 3739 220a 2020 2020  guide12679".    
-00000de0: 2020 2069 6e6b 7363 6170 653a 6c61 6265     inkscape:labe
-00000df0: 6c3d 2222 0a20 2020 2020 2020 696e 6b73  l="".       inks
-00000e00: 6361 7065 3a6c 6f63 6b65 643d 2274 7275  cape:locked="tru
-00000e10: 6522 0a20 2020 2020 2020 696e 6b73 6361  e".       inksca
-00000e20: 7065 3a63 6f6c 6f72 3d22 7267 6228 302c  pe:color="rgb(0,
-00000e30: 302c 3235 3529 2220 2f3e 0a20 2020 203c  0,255)" />.    <
-00000e40: 736f 6469 706f 6469 3a67 7569 6465 0a20  sodipodi:guide. 
-00000e50: 2020 2020 2020 706f 7369 7469 6f6e 3d22        position="
-00000e60: 3333 2e35 352c 3530 220a 2020 2020 2020  33.55,50".      
-00000e70: 206f 7269 656e 7461 7469 6f6e 3d22 2d31   orientation="-1
-00000e80: 2c30 220a 2020 2020 2020 2069 643d 2267  ,0".       id="g
-00000e90: 7569 6465 3133 3432 3722 0a20 2020 2020  uide13427".     
-00000ea0: 2020 696e 6b73 6361 7065 3a6c 6162 656c    inkscape:label
-00000eb0: 3d22 220a 2020 2020 2020 2069 6e6b 7363  ="".       inksc
-00000ec0: 6170 653a 6c6f 636b 6564 3d22 7472 7565  ape:locked="true
-00000ed0: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
-00000ee0: 653a 636f 6c6f 723d 2272 6762 2830 2c30  e:color="rgb(0,0
-00000ef0: 2c32 3535 2922 202f 3e0a 2020 2020 3c73  ,255)" />.    <s
-00000f00: 6f64 6970 6f64 693a 6775 6964 650a 2020  odipodi:guide.  
-00000f10: 2020 2020 2070 6f73 6974 696f 6e3d 2234       position="4
-00000f20: 372e 352c 3530 220a 2020 2020 2020 206f  7.5,50".       o
-00000f30: 7269 656e 7461 7469 6f6e 3d22 2d31 2c30  rientation="-1,0
-00000f40: 220a 2020 2020 2020 2069 643d 2267 7569  ".       id="gui
-00000f50: 6465 3133 3739 3722 0a20 2020 2020 2020  de13797".       
-00000f60: 696e 6b73 6361 7065 3a6c 6162 656c 3d22  inkscape:label="
-00000f70: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
-00000f80: 653a 6c6f 636b 6564 3d22 7472 7565 220a  e:locked="true".
-00000f90: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
-00000fa0: 636f 6c6f 723d 2272 6762 2830 2c30 2c32  color="rgb(0,0,2
-00000fb0: 3535 2922 202f 3e0a 2020 2020 3c73 6f64  55)" />.    <sod
-00000fc0: 6970 6f64 693a 6775 6964 650a 2020 2020  ipodi:guide.    
-00000fd0: 2020 2070 6f73 6974 696f 6e3d 2232 352c     position="25,
-00000fe0: 3235 220a 2020 2020 2020 206f 7269 656e  25".       orien
-00000ff0: 7461 7469 6f6e 3d22 302c 3122 0a20 2020  tation="0,1".   
-00001000: 2020 2020 6964 3d22 6775 6964 6531 3337      id="guide137
-00001010: 3939 220a 2020 2020 2020 2069 6e6b 7363  99".       inksc
-00001020: 6170 653a 6c61 6265 6c3d 2222 0a20 2020  ape:label="".   
-00001030: 2020 2020 696e 6b73 6361 7065 3a6c 6f63      inkscape:loc
-00001040: 6b65 643d 2274 7275 6522 0a20 2020 2020  ked="true".     
-00001050: 2020 696e 6b73 6361 7065 3a63 6f6c 6f72    inkscape:color
-00001060: 3d22 7267 6228 302c 302c 3235 3529 2220  ="rgb(0,0,255)" 
-00001070: 2f3e 0a20 2020 203c 736f 6469 706f 6469  />.    <sodipodi
-00001080: 3a67 7569 6465 0a20 2020 2020 2020 706f  :guide.       po
-00001090: 7369 7469 6f6e 3d22 3335 2e34 3232 3238  sition="35.42228
-000010a0: 382c 302e 3433 3633 3030 3931 220a 2020  8,0.43630091".  
-000010b0: 2020 2020 206f 7269 656e 7461 7469 6f6e       orientation
-000010c0: 3d22 2d31 2c30 220a 2020 2020 2020 2069  ="-1,0".       i
-000010d0: 643d 2267 7569 6465 3237 3730 3922 0a20  d="guide27709". 
-000010e0: 2020 2020 2020 696e 6b73 6361 7065 3a6c        inkscape:l
-000010f0: 6162 656c 3d22 220a 2020 2020 2020 2069  abel="".       i
-00001100: 6e6b 7363 6170 653a 6c6f 636b 6564 3d22  nkscape:locked="
-00001110: 7472 7565 220a 2020 2020 2020 2069 6e6b  true".       ink
-00001120: 7363 6170 653a 636f 6c6f 723d 2272 6762  scape:color="rgb
-00001130: 2830 2c30 2c32 3535 2922 202f 3e0a 2020  (0,0,255)" />.  
-00001140: 2020 3c73 6f64 6970 6f64 693a 6775 6964    <sodipodi:guid
-00001150: 650a 2020 2020 2020 2070 6f73 6974 696f  e.       positio
-00001160: 6e3d 2231 332e 3339 3734 3631 2c33 312e  n="13.397461,31.
-00001170: 3639 3837 3239 220a 2020 2020 2020 206f  698729".       o
-00001180: 7269 656e 7461 7469 6f6e 3d22 302e 352c  rientation="0.5,
-00001190: 2d30 2e38 3636 3032 3534 220a 2020 2020  -0.8660254".    
-000011a0: 2020 2069 643d 2267 7569 6465 3334 3831     id="guide3481
-000011b0: 3822 0a20 2020 2020 2020 696e 6b73 6361  8".       inksca
-000011c0: 7065 3a6c 6162 656c 3d22 220a 2020 2020  pe:label="".    
-000011d0: 2020 2069 6e6b 7363 6170 653a 6c6f 636b     inkscape:lock
-000011e0: 6564 3d22 7472 7565 220a 2020 2020 2020  ed="true".      
-000011f0: 2069 6e6b 7363 6170 653a 636f 6c6f 723d   inkscape:color=
-00001200: 2272 6762 2830 2c30 2c32 3535 2922 202f  "rgb(0,0,255)" /
-00001210: 3e0a 2020 2020 3c73 6f64 6970 6f64 693a  >.    <sodipodi:
-00001220: 6775 6964 650a 2020 2020 2020 2070 6f73  guide.       pos
-00001230: 6974 696f 6e3d 2232 352c 3236 220a 2020  ition="25,26".  
-00001240: 2020 2020 206f 7269 656e 7461 7469 6f6e       orientation
-00001250: 3d22 2d30 2e35 2c2d 302e 3836 3630 3235  ="-0.5,-0.866025
-00001260: 3422 0a20 2020 2020 2020 6964 3d22 6775  4".       id="gu
-00001270: 6964 6533 3438 3230 220a 2020 2020 2020  ide34820".      
-00001280: 2069 6e6b 7363 6170 653a 6c61 6265 6c3d   inkscape:label=
-00001290: 2222 0a20 2020 2020 2020 696e 6b73 6361  "".       inksca
-000012a0: 7065 3a6c 6f63 6b65 643d 2274 7275 6522  pe:locked="true"
-000012b0: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
-000012c0: 3a63 6f6c 6f72 3d22 7267 6228 302c 302c  :color="rgb(0,0,
-000012d0: 3235 3529 2220 2f3e 0a20 2020 203c 736f  255)" />.    <so
-000012e0: 6469 706f 6469 3a67 7569 6465 0a20 2020  dipodi:guide.   
-000012f0: 2020 2020 706f 7369 7469 6f6e 3d22 3235      position="25
-00001300: 2c32 3422 0a20 2020 2020 2020 6f72 6965  ,24".       orie
-00001310: 6e74 6174 696f 6e3d 222d 302e 352c 2d30  ntation="-0.5,-0
-00001320: 2e38 3636 3032 3534 220a 2020 2020 2020  .8660254".      
-00001330: 2069 643d 2267 7569 6465 3335 3033 3322   id="guide35033"
-00001340: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
-00001350: 3a6c 6162 656c 3d22 220a 2020 2020 2020  :label="".      
-00001360: 2069 6e6b 7363 6170 653a 6c6f 636b 6564   inkscape:locked
-00001370: 3d22 7472 7565 220a 2020 2020 2020 2069  ="true".       i
-00001380: 6e6b 7363 6170 653a 636f 6c6f 723d 2272  nkscape:color="r
-00001390: 6762 2830 2c30 2c32 3535 2922 202f 3e0a  gb(0,0,255)" />.
-000013a0: 2020 2020 3c73 6f64 6970 6f64 693a 6775      <sodipodi:gu
-000013b0: 6964 650a 2020 2020 2020 2070 6f73 6974  ide.       posit
-000013c0: 696f 6e3d 2232 352c 3235 220a 2020 2020  ion="25,25".    
-000013d0: 2020 206f 7269 656e 7461 7469 6f6e 3d22     orientation="
-000013e0: 2d30 2e35 2c2d 302e 3836 3630 3235 3422  -0.5,-0.8660254"
-000013f0: 0a20 2020 2020 2020 6964 3d22 6775 6964  .       id="guid
-00001400: 6533 3530 3335 220a 2020 2020 2020 2069  e35035".       i
-00001410: 6e6b 7363 6170 653a 6c61 6265 6c3d 2222  nkscape:label=""
-00001420: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
-00001430: 3a6c 6f63 6b65 643d 2274 7275 6522 0a20  :locked="true". 
-00001440: 2020 2020 2020 696e 6b73 6361 7065 3a63        inkscape:c
-00001450: 6f6c 6f72 3d22 7267 6228 302c 302c 3235  olor="rgb(0,0,25
-00001460: 3529 2220 2f3e 0a20 2020 203c 736f 6469  5)" />.    <sodi
-00001470: 706f 6469 3a67 7569 6465 0a20 2020 2020  podi:guide.     
-00001480: 2020 706f 7369 7469 6f6e 3d22 3234 2e31    position="24.1
-00001490: 3333 3937 352c 3234 2e34 3939 3939 3922  33975,24.499999"
-000014a0: 0a20 2020 2020 2020 6f72 6965 6e74 6174  .       orientat
-000014b0: 696f 6e3d 2230 2e35 2c2d 302e 3836 3630  ion="0.5,-0.8660
-000014c0: 3235 3422 0a20 2020 2020 2020 696e 6b73  254".       inks
-000014d0: 6361 7065 3a6c 6f63 6b65 643d 2274 7275  cape:locked="tru
-000014e0: 6522 0a20 2020 2020 2020 6964 3d22 6775  e".       id="gu
-000014f0: 6964 6533 3535 3732 220a 2020 2020 2020  ide35572".      
-00001500: 2069 6e6b 7363 6170 653a 6c61 6265 6c3d   inkscape:label=
-00001510: 2222 0a20 2020 2020 2020 696e 6b73 6361  "".       inksca
-00001520: 7065 3a63 6f6c 6f72 3d22 7267 6228 302c  pe:color="rgb(0,
-00001530: 302c 3235 3529 2220 2f3e 0a20 2020 203c  0,255)" />.    <
-00001540: 736f 6469 706f 6469 3a67 7569 6465 0a20  sodipodi:guide. 
-00001550: 2020 2020 2020 706f 7369 7469 6f6e 3d22        position="
-00001560: 3932 2e33 3339 3538 332c 2d32 392e 3131  92.339583,-29.11
-00001570: 3034 3136 220a 2020 2020 2020 206f 7269  0416".       ori
-00001580: 656e 7461 7469 6f6e 3d22 2d30 2e35 2c2d  entation="-0.5,-
-00001590: 302e 3836 3630 3235 3422 0a20 2020 2020  0.8660254".     
-000015a0: 2020 6964 3d22 6775 6964 6533 3536 3438    id="guide35648
-000015b0: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
-000015c0: 653a 6c61 6265 6c3d 2222 0a20 2020 2020  e:label="".     
-000015d0: 2020 696e 6b73 6361 7065 3a6c 6f63 6b65    inkscape:locke
-000015e0: 643d 2274 7275 6522 0a20 2020 2020 2020  d="true".       
-000015f0: 696e 6b73 6361 7065 3a63 6f6c 6f72 3d22  inkscape:color="
-00001600: 7267 6228 302c 302c 3235 3529 2220 2f3e  rgb(0,0,255)" />
-00001610: 0a20 2020 203c 736f 6469 706f 6469 3a67  .    <sodipodi:g
-00001620: 7569 6465 0a20 2020 2020 2020 706f 7369  uide.       posi
-00001630: 7469 6f6e 3d22 3335 2e37 3336 3531 362c  tion="35.736516,
-00001640: 3137 2e38 3031 3236 3922 0a20 2020 2020  17.801269".     
-00001650: 2020 6f72 6965 6e74 6174 696f 6e3d 2230    orientation="0
-00001660: 2e35 2c2d 302e 3836 3630 3235 3422 0a20  .5,-0.8660254". 
-00001670: 2020 2020 2020 6964 3d22 6775 6964 6534        id="guide4
-00001680: 3734 3731 220a 2020 2020 2020 2069 6e6b  7471".       ink
-00001690: 7363 6170 653a 6c61 6265 6c3d 2222 0a20  scape:label="". 
-000016a0: 2020 2020 2020 696e 6b73 6361 7065 3a6c        inkscape:l
-000016b0: 6f63 6b65 643d 2274 7275 6522 0a20 2020  ocked="true".   
-000016c0: 2020 2020 696e 6b73 6361 7065 3a63 6f6c      inkscape:col
-000016d0: 6f72 3d22 7267 6228 302c 302c 3235 3529  or="rgb(0,0,255)
-000016e0: 2220 2f3e 0a20 203c 2f73 6f64 6970 6f64  " />.  </sodipod
-000016f0: 693a 6e61 6d65 6476 6965 773e 0a20 203c  i:namedview>.  <
-00001700: 6465 6673 0a20 2020 2020 6964 3d22 6465  defs.     id="de
-00001710: 6673 3931 3922 3e0a 2020 2020 3c6d 6172  fs919">.    <mar
-00001720: 6b65 720a 2020 2020 2020 2073 7479 6c65  ker.       style
-00001730: 3d22 6f76 6572 666c 6f77 3a76 6973 6962  ="overflow:visib
-00001740: 6c65 3b22 0a20 2020 2020 2020 6964 3d22  le;".       id="
-00001750: 4172 726f 7731 4c65 6e64 220a 2020 2020  Arrow1Lend".    
-00001760: 2020 2072 6566 583d 2230 2e30 220a 2020     refX="0.0".  
-00001770: 2020 2020 2072 6566 593d 2230 2e30 220a       refY="0.0".
-00001780: 2020 2020 2020 206f 7269 656e 743d 2261         orient="a
-00001790: 7574 6f22 0a20 2020 2020 2020 696e 6b73  uto".       inks
-000017a0: 6361 7065 3a73 746f 636b 6964 3d22 4172  cape:stockid="Ar
-000017b0: 726f 7731 4c65 6e64 220a 2020 2020 2020  row1Lend".      
-000017c0: 2069 6e6b 7363 6170 653a 6973 7374 6f63   inkscape:isstoc
-000017d0: 6b3d 2274 7275 6522 3e0a 2020 2020 2020  k="true">.      
-000017e0: 3c70 6174 680a 2020 2020 2020 2020 2074  <path.         t
-000017f0: 7261 6e73 666f 726d 3d22 7363 616c 6528  ransform="scale(
-00001800: 302e 3829 2072 6f74 6174 6528 3138 3029  0.8) rotate(180)
-00001810: 2074 7261 6e73 6c61 7465 2831 322e 352c   translate(12.5,
-00001820: 3029 220a 2020 2020 2020 2020 2073 7479  0)".         sty
-00001830: 6c65 3d22 6669 6c6c 2d72 756c 653a 6576  le="fill-rule:ev
-00001840: 656e 6f64 643b 6669 6c6c 3a63 6f6e 7465  enodd;fill:conte
-00001850: 7874 2d73 7472 6f6b 653b 7374 726f 6b65  xt-stroke;stroke
-00001860: 3a63 6f6e 7465 7874 2d73 7472 6f6b 653b  :context-stroke;
-00001870: 7374 726f 6b65 2d77 6964 7468 3a31 2e30  stroke-width:1.0
-00001880: 7074 3b22 0a20 2020 2020 2020 2020 643d  pt;".         d=
-00001890: 224d 2030 2e30 2c30 2e30 204c 2035 2e30  "M 0.0,0.0 L 5.0
-000018a0: 2c2d 352e 3020 4c20 2d31 322e 352c 302e  ,-5.0 L -12.5,0.
-000018b0: 3020 4c20 352e 302c 352e 3020 4c20 302e  0 L 5.0,5.0 L 0.
-000018c0: 302c 302e 3020 7a20 220a 2020 2020 2020  0,0.0 z ".      
-000018d0: 2020 2069 643d 2270 6174 6838 3636 2220     id="path866" 
-000018e0: 2f3e 0a20 2020 203c 2f6d 6172 6b65 723e  />.    </marker>
-000018f0: 0a20 2020 203c 6d61 726b 6572 0a20 2020  .    <marker.   
-00001900: 2020 2020 7374 796c 653d 226f 7665 7266      style="overf
-00001910: 6c6f 773a 7669 7369 626c 653b 220a 2020  low:visible;".  
-00001920: 2020 2020 2069 643d 2241 7272 6f77 324c       id="Arrow2L
-00001930: 656e 6422 0a20 2020 2020 2020 7265 6658  end".       refX
-00001940: 3d22 302e 3022 0a20 2020 2020 2020 7265  ="0.0".       re
-00001950: 6659 3d22 302e 3022 0a20 2020 2020 2020  fY="0.0".       
-00001960: 6f72 6965 6e74 3d22 6175 746f 220a 2020  orient="auto".  
-00001970: 2020 2020 2069 6e6b 7363 6170 653a 7374       inkscape:st
-00001980: 6f63 6b69 643d 2241 7272 6f77 324c 656e  ockid="Arrow2Len
-00001990: 6422 0a20 2020 2020 2020 696e 6b73 6361  d".       inksca
-000019a0: 7065 3a69 7373 746f 636b 3d22 7472 7565  pe:isstock="true
-000019b0: 223e 0a20 2020 2020 203c 7061 7468 0a20  ">.      <path. 
-000019c0: 2020 2020 2020 2020 7472 616e 7366 6f72          transfor
-000019d0: 6d3d 2273 6361 6c65 2831 2e31 2920 726f  m="scale(1.1) ro
-000019e0: 7461 7465 2831 3830 2920 7472 616e 736c  tate(180) transl
-000019f0: 6174 6528 312c 3029 220a 2020 2020 2020  ate(1,0)".      
-00001a00: 2020 2064 3d22 4d20 382e 3731 3835 3837     d="M 8.718587
-00001a10: 382c 342e 3033 3337 3335 3220 4c20 2d32  8,4.0337352 L -2
-00001a20: 2e32 3037 3238 3935 2c30 2e30 3136 3031  .2072895,0.01601
-00001a30: 3332 3536 204c 2038 2e37 3138 3538 3834  3256 L 8.7185884
-00001a40: 2c2d 342e 3030 3137 3037 3820 4320 362e  ,-4.0017078 C 6.
-00001a50: 3937 3330 3930 302c 2d31 2e36 3239 3634  9730900,-1.62964
-00001a60: 3639 2036 2e39 3833 3134 3736 2c31 2e36  69 6.9831476,1.6
-00001a70: 3135 3734 3431 2038 2e37 3138 3538 3738  157441 8.7185878
-00001a80: 2c34 2e30 3333 3733 3532 207a 2022 0a20  ,4.0337352 z ". 
-00001a90: 2020 2020 2020 2020 7374 796c 653d 2273          style="s
-00001aa0: 7472 6f6b 653a 636f 6e74 6578 742d 7374  troke:context-st
-00001ab0: 726f 6b65 3b66 696c 6c2d 7275 6c65 3a65  roke;fill-rule:e
-00001ac0: 7665 6e6f 6464 3b66 696c 6c3a 636f 6e74  venodd;fill:cont
-00001ad0: 6578 742d 7374 726f 6b65 3b73 7472 6f6b  ext-stroke;strok
-00001ae0: 652d 7769 6474 683a 302e 3632 3530 3030  e-width:0.625000
-00001af0: 3030 3b73 7472 6f6b 652d 6c69 6e65 6a6f  00;stroke-linejo
-00001b00: 696e 3a72 6f75 6e64 3b22 0a20 2020 2020  in:round;".     
-00001b10: 2020 2020 6964 3d22 7061 7468 3838 3422      id="path884"
-00001b20: 202f 3e0a 2020 2020 3c2f 6d61 726b 6572   />.    </marker
-00001b30: 3e0a 2020 2020 3c6d 6172 6b65 720a 2020  >.    <marker.  
-00001b40: 2020 2020 2073 7479 6c65 3d22 6f76 6572       style="over
-00001b50: 666c 6f77 3a76 6973 6962 6c65 220a 2020  flow:visible".  
-00001b60: 2020 2020 2069 643d 2241 7272 6f77 314c       id="Arrow1L
-00001b70: 656e 642d 3622 0a20 2020 2020 2020 7265  end-6".       re
-00001b80: 6658 3d22 3022 0a20 2020 2020 2020 7265  fX="0".       re
-00001b90: 6659 3d22 3022 0a20 2020 2020 2020 6f72  fY="0".       or
-00001ba0: 6965 6e74 3d22 6175 746f 220a 2020 2020  ient="auto".    
-00001bb0: 2020 2069 6e6b 7363 6170 653a 7374 6f63     inkscape:stoc
-00001bc0: 6b69 643d 2241 7272 6f77 314c 656e 6422  kid="Arrow1Lend"
-00001bd0: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
-00001be0: 3a69 7373 746f 636b 3d22 7472 7565 223e  :isstock="true">
-00001bf0: 0a20 2020 2020 203c 7061 7468 0a20 2020  .      <path.   
-00001c00: 2020 2020 2020 7472 616e 7366 6f72 6d3d        transform=
-00001c10: 226d 6174 7269 7828 2d30 2e38 2c30 2c30  "matrix(-0.8,0,0
-00001c20: 2c2d 302e 382c 2d31 302c 3029 220a 2020  ,-0.8,-10,0)".  
-00001c30: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
-00001c40: 6c6c 3a63 6f6e 7465 7874 2d73 7472 6f6b  ll:context-strok
-00001c50: 653b 6669 6c6c 2d72 756c 653a 6576 656e  e;fill-rule:even
-00001c60: 6f64 643b 7374 726f 6b65 3a63 6f6e 7465  odd;stroke:conte
-00001c70: 7874 2d73 7472 6f6b 653b 7374 726f 6b65  xt-stroke;stroke
-00001c80: 2d77 6964 7468 3a31 7074 220a 2020 2020  -width:1pt".    
-00001c90: 2020 2020 2064 3d22 4d20 302c 3020 352c       d="M 0,0 5,
-00001ca0: 2d35 202d 3132 2e35 2c30 2035 2c35 205a  -5 -12.5,0 5,5 Z
-00001cb0: 220a 2020 2020 2020 2020 2069 643d 2270  ".         id="p
-00001cc0: 6174 6838 3039 3422 202f 3e0a 2020 2020  ath8094" />.    
-00001cd0: 3c2f 6d61 726b 6572 3e0a 2020 2020 3c6d  </marker>.    <m
-00001ce0: 6172 6b65 720a 2020 2020 2020 2073 7479  arker.       sty
-00001cf0: 6c65 3d22 6f76 6572 666c 6f77 3a76 6973  le="overflow:vis
-00001d00: 6962 6c65 220a 2020 2020 2020 2069 643d  ible".       id=
-00001d10: 226d 6172 6b65 7231 3133 3322 0a20 2020  "marker1133".   
-00001d20: 2020 2020 7265 6658 3d22 3022 0a20 2020      refX="0".   
-00001d30: 2020 2020 7265 6659 3d22 3022 0a20 2020      refY="0".   
-00001d40: 2020 2020 6f72 6965 6e74 3d22 6175 746f      orient="auto
-00001d50: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
-00001d60: 653a 7374 6f63 6b69 643d 2241 7272 6f77  e:stockid="Arrow
-00001d70: 314c 656e 6422 0a20 2020 2020 2020 696e  1Lend".       in
-00001d80: 6b73 6361 7065 3a69 7373 746f 636b 3d22  kscape:isstock="
-00001d90: 7472 7565 223e 0a20 2020 2020 203c 7061  true">.      <pa
-00001da0: 7468 0a20 2020 2020 2020 2020 7472 616e  th.         tran
-00001db0: 7366 6f72 6d3d 226d 6174 7269 7828 2d30  sform="matrix(-0
-00001dc0: 2e38 2c30 2c30 2c2d 302e 382c 2d31 302c  .8,0,0,-0.8,-10,
-00001dd0: 3029 220a 2020 2020 2020 2020 2073 7479  0)".         sty
-00001de0: 6c65 3d22 6669 6c6c 3a63 6f6e 7465 7874  le="fill:context
-00001df0: 2d73 7472 6f6b 653b 6669 6c6c 2d72 756c  -stroke;fill-rul
-00001e00: 653a 6576 656e 6f64 643b 7374 726f 6b65  e:evenodd;stroke
-00001e10: 3a63 6f6e 7465 7874 2d73 7472 6f6b 653b  :context-stroke;
-00001e20: 7374 726f 6b65 2d77 6964 7468 3a31 7074  stroke-width:1pt
-00001e30: 220a 2020 2020 2020 2020 2064 3d22 4d20  ".         d="M 
-00001e40: 302c 3020 352c 2d35 202d 3132 2e35 2c30  0,0 5,-5 -12.5,0
-00001e50: 2035 2c35 205a 220a 2020 2020 2020 2020   5,5 Z".        
-00001e60: 2069 643d 2270 6174 6831 3133 3122 202f   id="path1131" /
-00001e70: 3e0a 2020 2020 3c2f 6d61 726b 6572 3e0a  >.    </marker>.
-00001e80: 2020 3c2f 6465 6673 3e0a 2020 3c67 0a20    </defs>.  <g. 
-00001e90: 2020 2020 6964 3d22 6c61 7965 7232 2d36      id="layer2-6
-00001ea0: 220a 2020 2020 2069 6e6b 7363 6170 653a  ".     inkscape:
-00001eb0: 6c61 6265 6c3d 224c 6f77 6572 220a 2020  label="Lower".  
-00001ec0: 2020 2073 7479 6c65 3d22 6469 7370 6c61     style="displa
-00001ed0: 793a 696e 6c69 6e65 220a 2020 2020 2074  y:inline".     t
-00001ee0: 7261 6e73 666f 726d 3d22 7472 616e 736c  ransform="transl
-00001ef0: 6174 6528 312e 3839 3330 3234 352c 2d38  ate(1.8930245,-8
-00001f00: 2e35 3735 3835 3929 220a 2020 2020 2069  .575859)".     i
-00001f10: 6e6b 7363 6170 653a 6772 6f75 706d 6f64  nkscape:groupmod
-00001f20: 653d 226c 6179 6572 220a 2020 2020 2073  e="layer".     s
-00001f30: 6f64 6970 6f64 693a 696e 7365 6e73 6974  odipodi:insensit
-00001f40: 6976 653d 2274 7275 6522 3e0a 2020 2020  ive="true">.    
-00001f50: 3c70 6174 680a 2020 2020 2020 2073 7479  <path.       sty
-00001f60: 6c65 3d22 6469 7370 6c61 793a 696e 6c69  le="display:inli
-00001f70: 6e65 3b6f 7061 6369 7479 3a30 2e33 3b66  ne;opacity:0.3;f
-00001f80: 696c 6c3a 2361 6264 6565 353b 7374 726f  ill:#abdee5;stro
-00001f90: 6b65 3a23 3030 3030 3030 3b73 7472 6f6b  ke:#000000;strok
-00001fa0: 652d 7769 6474 683a 303b 7374 726f 6b65  e-width:0;stroke
-00001fb0: 2d6c 696e 6563 6170 3a62 7574 743b 7374  -linecap:butt;st
-00001fc0: 726f 6b65 2d6c 696e 656a 6f69 6e3a 6d69  roke-linejoin:mi
-00001fd0: 7465 723b 7374 726f 6b65 2d6d 6974 6572  ter;stroke-miter
-00001fe0: 6c69 6d69 743a 343b 7374 726f 6b65 2d64  limit:4;stroke-d
-00001ff0: 6173 6861 7272 6179 3a6e 6f6e 653b 7374  asharray:none;st
-00002000: 726f 6b65 2d6f 7061 6369 7479 3a31 220a  roke-opacity:1".
-00002010: 2020 2020 2020 2064 3d22 6d20 3232 2e32         d="m 22.2
-00002020: 3430 3935 312c 3334 2e30 3735 3836 2063  40951,34.07586 c
-00002030: 2030 2c30 202d 302e 3735 3630 3739 2c32   0,0 -0.756079,2
-00002040: 302e 3230 3235 3137 2033 2e35 3730 3538  0.202517 3.57058
-00002050: 2c32 322e 3730 3035 3134 2030 2e35 3834  ,22.700514 0.584
-00002060: 3837 322c 302e 3333 3736 3735 2031 2e31  872,0.337675 1.1
-00002070: 3538 3531 392c 302e 3239 3137 3238 2031  58519,0.291728 1
-00002080: 2e37 3133 3238 392c 2d30 2e30 3430 3320  .713289,-0.0403 
-00002090: 6c20 312e 3733 3230 3531 2c2d 302e 3939  l 1.732051,-0.99
-000020a0: 3939 3939 2063 202d 302e 3535 3437 372c  9999 c -0.55477,
-000020b0: 302e 3333 3230 3235 202d 312e 3132 3834  0.332025 -1.1284
-000020c0: 3137 2c30 2e33 3737 3937 3220 2d31 2e37  17,0.377972 -1.7
-000020d0: 3133 3238 392c 302e 3034 3033 202d 342e  13289,0.0403 -4.
-000020e0: 3332 3636 3539 2c2d 322e 3439 3739 3937  326659,-2.497997
-000020f0: 202d 332e 3537 3035 382c 2d32 322e 3730   -3.57058,-22.70
-00002100: 3035 3135 202d 332e 3537 3035 382c 2d32  0515 -3.57058,-2
-00002110: 322e 3730 3035 3135 220a 2020 2020 2020  2.700515".      
-00002120: 2069 643d 2270 6174 6834 3334 3530 2d31   id="path43450-1
-00002130: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
-00002140: 653a 6c61 6265 6c3d 2242 616e 6420 3322  e:label="Band 3"
-00002150: 0a20 2020 2020 2020 736f 6469 706f 6469  .       sodipodi
-00002160: 3a6e 6f64 6574 7970 6573 3d22 6373 6363  :nodetypes="cscc
-00002170: 7363 220a 2020 2020 2020 2073 6f64 6970  sc".       sodip
-00002180: 6f64 693a 696e 7365 6e73 6974 6976 653d  odi:insensitive=
-00002190: 2274 7275 6522 202f 3e0a 2020 2020 3c70  "true" />.    <p
-000021a0: 6174 680a 2020 2020 2020 2073 7479 6c65  ath.       style
-000021b0: 3d22 6469 7370 6c61 793a 696e 6c69 6e65  ="display:inline
-000021c0: 3b66 696c 6c3a 6e6f 6e65 3b73 7472 6f6b  ;fill:none;strok
-000021d0: 653a 2330 3030 3030 303b 7374 726f 6b65  e:#000000;stroke
-000021e0: 2d77 6964 7468 3a30 2e31 3b73 7472 6f6b  -width:0.1;strok
-000021f0: 652d 6c69 6e65 6361 703a 6275 7474 3b73  e-linecap:butt;s
-00002200: 7472 6f6b 652d 6c69 6e65 6a6f 696e 3a6d  troke-linejoin:m
-00002210: 6974 6572 3b73 7472 6f6b 652d 6d69 7465  iter;stroke-mite
-00002220: 726c 696d 6974 3a34 3b73 7472 6f6b 652d  rlimit:4;stroke-
-00002230: 6461 7368 6172 7261 793a 6e6f 6e65 3b73  dasharray:none;s
-00002240: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
-00002250: 0a20 2020 2020 2020 643d 226d 2032 332e  .       d="m 23.
-00002260: 3937 3330 3032 2c33 332e 3037 3538 3620  973002,33.07586 
-00002270: 6320 302c 3020 2d30 2e37 3536 3037 392c  c 0,0 -0.756079,
-00002280: 3230 2e32 3032 3531 3720 332e 3537 3035  20.202517 3.5705
-00002290: 382c 3232 2e37 3030 3531 3420 302e 3538  8,22.700514 0.58
-000022a0: 3438 3732 2c30 2e33 3337 3637 3520 312e  4872,0.337675 1.
-000022b0: 3135 3835 322c 302e 3239 3137 3238 2031  15852,0.291728 1
-000022c0: 2e37 3133 3238 392c 2d30 2e30 3430 3320  .713289,-0.0403 
-000022d0: 6c20 2d31 2e37 3332 3035 312c 3120 6320  l -1.732051,1 c 
-000022e0: 2d30 2e35 3534 3737 2c30 2e33 3332 3032  -0.55477,0.33202
-000022f0: 3420 2d31 2e31 3238 3431 362c 302e 3337  4 -1.128416,0.37
-00002300: 3739 3731 202d 312e 3731 3332 3839 2c30  7971 -1.713289,0
-00002310: 2e30 3430 3320 4320 3231 2e34 3834 3837  .0403 C 21.48487
-00002320: 332c 3534 2e32 3738 3337 3720 3232 2e32  3,54.278377 22.2
-00002330: 3430 3935 322c 3334 2e30 3735 3836 2032  40952,34.07586 2
-00002340: 322e 3234 3039 3532 2c33 342e 3037 3538  2.240952,34.0758
-00002350: 3622 0a20 2020 2020 2020 6964 3d22 7061  6".       id="pa
-00002360: 7468 3532 3433 372d 3522 0a20 2020 2020  th52437-5".     
-00002370: 2020 696e 6b73 6361 7065 3a6c 6162 656c    inkscape:label
-00002380: 3d22 4c69 6e65 2033 220a 2020 2020 2020  ="Line 3".      
-00002390: 2073 6f64 6970 6f64 693a 6e6f 6465 7479   sodipodi:nodety
-000023a0: 7065 733d 2263 7363 6373 6322 0a20 2020  pes="csccsc".   
-000023b0: 2020 2020 736f 6469 706f 6469 3a69 6e73      sodipodi:ins
-000023c0: 656e 7369 7469 7665 3d22 7472 7565 2220  ensitive="true" 
-000023d0: 2f3e 0a20 2020 203c 7061 7468 0a20 2020  />.    <path.   
-000023e0: 2020 2020 7374 796c 653d 2264 6973 706c      style="displ
-000023f0: 6179 3a69 6e6c 696e 653b 6669 6c6c 3a6e  ay:inline;fill:n
-00002400: 6f6e 653b 7374 726f 6b65 3a23 3030 3030  one;stroke:#0000
-00002410: 3030 3b73 7472 6f6b 652d 7769 6474 683a  00;stroke-width:
-00002420: 302e 313b 7374 726f 6b65 2d6c 696e 6563  0.1;stroke-linec
-00002430: 6170 3a62 7574 743b 7374 726f 6b65 2d6c  ap:butt;stroke-l
-00002440: 696e 656a 6f69 6e3a 6d69 7465 723b 7374  inejoin:miter;st
-00002450: 726f 6b65 2d6d 6974 6572 6c69 6d69 743a  roke-miterlimit:
-00002460: 343b 7374 726f 6b65 2d64 6173 6861 7272  4;stroke-dasharr
-00002470: 6179 3a6e 6f6e 653b 7374 726f 6b65 2d6f  ay:none;stroke-o
-00002480: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
-00002490: 2064 3d22 6d20 3333 2e38 3433 3439 312c   d="m 33.843491,
-000024a0: 3430 2e37 3734 3539 2063 2030 2c30 202d  40.77459 c 0,0 -
-000024b0: 322e 3736 3934 3633 2c31 332e 3833 3733  2.769463,13.8373
-000024c0: 3138 202d 362e 3331 3836 3731 2c31 352e  18 -6.318671,15.
-000024d0: 3936 3134 3838 206c 2031 2e37 3331 3938  961488 l 1.73198
-000024e0: 392c 2d30 2e39 3939 3936 3420 4320 3332  9,-0.999964 C 32
-000024f0: 2e38 3036 3031 372c 3533 2e36 3131 3934  .806017,53.61194
-00002500: 3520 3335 2e35 3735 3438 2c33 392e 3737  5 35.57548,39.77
-00002510: 3436 3237 2033 352e 3537 3534 382c 3339  4627 35.57548,39
-00002520: 2e37 3734 3632 3722 0a20 2020 2020 2020  .774627".       
-00002530: 6964 3d22 7061 7468 3234 3737 2d37 220a  id="path2477-7".
-00002540: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
-00002550: 6c61 6265 6c3d 224c 696e 6520 3422 0a20  label="Line 4". 
-00002560: 2020 2020 2020 736f 6469 706f 6469 3a6e        sodipodi:n
-00002570: 6f64 6574 7970 6573 3d22 6363 6363 220a  odetypes="cccc".
-00002580: 2020 2020 2020 2073 6f64 6970 6f64 693a         sodipodi:
-00002590: 696e 7365 6e73 6974 6976 653d 2274 7275  insensitive="tru
-000025a0: 6522 202f 3e0a 2020 2020 3c70 6174 680a  e" />.    <path.
-000025b0: 2020 2020 2020 2073 7479 6c65 3d22 6469         style="di
-000025c0: 7370 6c61 793a 696e 6c69 6e65 3b6f 7061  splay:inline;opa
-000025d0: 6369 7479 3a30 2e33 3b66 696c 6c3a 2361  city:0.3;fill:#a
-000025e0: 6264 6565 353b 7374 726f 6b65 3a23 3030  bdee5;stroke:#00
-000025f0: 3030 3030 3b73 7472 6f6b 652d 7769 6474  0000;stroke-widt
-00002600: 683a 303b 7374 726f 6b65 2d6c 696e 6563  h:0;stroke-linec
-00002610: 6170 3a62 7574 743b 7374 726f 6b65 2d6c  ap:butt;stroke-l
-00002620: 696e 656a 6f69 6e3a 6d69 7465 723b 7374  inejoin:miter;st
-00002630: 726f 6b65 2d6d 6974 6572 6c69 6d69 743a  roke-miterlimit:
-00002640: 343b 7374 726f 6b65 2d64 6173 6861 7272  4;stroke-dasharr
-00002650: 6179 3a6e 6f6e 653b 7374 726f 6b65 2d6f  ay:none;stroke-o
-00002660: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
-00002670: 2064 3d22 6d20 3333 2e38 3433 3439 312c   d="m 33.843491,
-00002680: 3430 2e37 3734 3539 2063 2030 2c30 202d  40.77459 c 0,0 -
-00002690: 322e 3736 3934 3633 2c31 332e 3833 3733  2.769463,13.8373
-000026a0: 3138 202d 362e 3331 3836 3731 2c31 352e  18 -6.318671,15.
-000026b0: 3936 3134 3838 206c 2031 2e37 3331 3938  961488 l 1.73198
-000026c0: 392c 2d30 2e39 3939 3936 3420 4320 3332  9,-0.999964 C 32
-000026d0: 2e38 3036 3031 372c 3533 2e36 3131 3934  .806017,53.61194
-000026e0: 3520 3335 2e35 3735 3438 2c33 392e 3737  5 35.57548,39.77
-000026f0: 3436 3237 2033 352e 3537 3534 382c 3339  4627 35.57548,39
-00002700: 2e37 3734 3632 3720 5a22 0a20 2020 2020  .774627 Z".     
-00002710: 2020 6964 3d22 7061 7468 3434 3631 2d37    id="path4461-7
-00002720: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
-00002730: 653a 6c61 6265 6c3d 2242 616e 6420 3422  e:label="Band 4"
-00002740: 0a20 2020 2020 2020 736f 6469 706f 6469  .       sodipodi
-00002750: 3a6e 6f64 6574 7970 6573 3d22 6363 6363  :nodetypes="cccc
-00002760: 6322 0a20 2020 2020 2020 736f 6469 706f  c".       sodipo
-00002770: 6469 3a69 6e73 656e 7369 7469 7665 3d22  di:insensitive="
-00002780: 7472 7565 2220 2f3e 0a20 203c 2f67 3e0a  true" />.  </g>.
-00002790: 2020 3c67 0a20 2020 2020 696e 6b73 6361    <g.     inksca
-000027a0: 7065 3a6c 6162 656c 3d22 506c 616e 6522  pe:label="Plane"
-000027b0: 0a20 2020 2020 696e 6b73 6361 7065 3a67  .     inkscape:g
-000027c0: 726f 7570 6d6f 6465 3d22 6c61 7965 7222  roupmode="layer"
-000027d0: 0a20 2020 2020 6964 3d22 6c61 7965 7231  .     id="layer1
-000027e0: 220a 2020 2020 2073 7479 6c65 3d22 6469  ".     style="di
-000027f0: 7370 6c61 793a 696e 6c69 6e65 220a 2020  splay:inline".  
-00002800: 2020 2073 6f64 6970 6f64 693a 696e 7365     sodipodi:inse
-00002810: 6e73 6974 6976 653d 2274 7275 6522 3e0a  nsitive="true">.
-00002820: 2020 2020 3c72 6563 740a 2020 2020 2020      <rect.      
-00002830: 2073 7479 6c65 3d22 6f70 6163 6974 793a   style="opacity:
-00002840: 302e 333b 6669 6c6c 3a23 6163 3536 3065  0.3;fill:#ac560e
-00002850: 3b73 7472 6f6b 653a 2330 3030 3030 303b  ;stroke:#000000;
-00002860: 7374 726f 6b65 2d77 6964 7468 3a30 3b73  stroke-width:0;s
-00002870: 7472 6f6b 652d 6c69 6e65 6361 703a 726f  troke-linecap:ro
-00002880: 756e 643b 7374 726f 6b65 2d6c 696e 656a  und;stroke-linej
-00002890: 6f69 6e3a 6265 7665 6c3b 7374 726f 6b65  oin:bevel;stroke
-000028a0: 2d6d 6974 6572 6c69 6d69 743a 343b 7374  -miterlimit:4;st
-000028b0: 726f 6b65 2d64 6173 6861 7272 6179 3a6e  roke-dasharray:n
-000028c0: 6f6e 6522 0a20 2020 2020 2020 6964 3d22  one".       id="
-000028d0: 7265 6374 3230 3031 220a 2020 2020 2020  rect2001".      
-000028e0: 2077 6964 7468 3d22 3133 2e33 3937 3435   width="13.39745
-000028f0: 3922 0a20 2020 2020 2020 6865 6967 6874  9".       height
-00002900: 3d22 3135 2e34 3730 3035 3422 0a20 2020  ="15.470054".   
-00002910: 2020 2020 783d 2232 362e 3033 3632 3939      x="26.036299
-00002920: 220a 2020 2020 2020 2079 3d22 3130 2e35  ".       y="10.5
-00002930: 3636 3234 3322 0a20 2020 2020 2020 696e  66243".       in
-00002940: 6b73 6361 7065 3a6c 6162 656c 3d22 5175  kscape:label="Qu
-00002950: 6164 7261 6e74 2031 220a 2020 2020 2020  adrant 1".      
-00002960: 2074 7261 6e73 666f 726d 3d22 6d61 7472   transform="matr
-00002970: 6978 2830 2e38 3636 3032 3534 2c30 2e35  ix(0.8660254,0.5
-00002980: 2c2d 302e 3836 3630 3235 342c 302e 352c  ,-0.8660254,0.5,
-00002990: 302c 3029 220a 2020 2020 2020 2073 6f64  0,0)".       sod
-000029a0: 6970 6f64 693a 696e 7365 6e73 6974 6976  ipodi:insensitiv
-000029b0: 653d 2274 7275 6522 202f 3e0a 2020 2020  e="true" />.    
-000029c0: 3c72 6563 740a 2020 2020 2020 2073 7479  <rect.       sty
-000029d0: 6c65 3d22 6f70 6163 6974 793a 302e 333b  le="opacity:0.3;
-000029e0: 6669 6c6c 3a23 6666 6331 3037 3b73 7472  fill:#ffc107;str
-000029f0: 6f6b 653a 2330 3030 3030 303b 7374 726f  oke:#000000;stro
-00002a00: 6b65 2d77 6964 7468 3a30 3b73 7472 6f6b  ke-width:0;strok
-00002a10: 652d 6c69 6e65 6361 703a 726f 756e 643b  e-linecap:round;
-00002a20: 7374 726f 6b65 2d6c 696e 656a 6f69 6e3a  stroke-linejoin:
-00002a30: 6265 7665 6c3b 7374 726f 6b65 2d6d 6974  bevel;stroke-mit
-00002a40: 6572 6c69 6d69 743a 343b 7374 726f 6b65  erlimit:4;stroke
-00002a50: 2d64 6173 6861 7272 6179 3a6e 6f6e 6522  -dasharray:none"
-00002a60: 0a20 2020 2020 2020 6964 3d22 7265 6374  .       id="rect
-00002a70: 3133 3033 220a 2020 2020 2020 2077 6964  1303".       wid
-00002a80: 7468 3d22 3133 2e33 3937 3435 3922 0a20  th="13.397459". 
-00002a90: 2020 2020 2020 6865 6967 6874 3d22 3135        height="15
-00002aa0: 2e34 3730 3035 3422 0a20 2020 2020 2020  .470054".       
-00002ab0: 783d 2232 362e 3033 3632 3939 220a 2020  x="26.036299".  
-00002ac0: 2020 2020 2079 3d22 2d34 2e39 3033 3830       y="-4.90380
-00002ad0: 3836 220a 2020 2020 2020 2069 6e6b 7363  86".       inksc
-00002ae0: 6170 653a 6c61 6265 6c3d 2251 7561 6472  ape:label="Quadr
-00002af0: 616e 7420 3222 0a20 2020 2020 2020 7472  ant 2".       tr
-00002b00: 616e 7366 6f72 6d3d 226d 6174 7269 7828  ansform="matrix(
-00002b10: 302e 3836 3630 3235 342c 302e 352c 2d30  0.8660254,0.5,-0
-00002b20: 2e38 3636 3032 3534 2c30 2e35 2c30 2c30  .8660254,0.5,0,0
-00002b30: 2922 0a20 2020 2020 2020 736f 6469 706f  )".       sodipo
-00002b40: 6469 3a69 6e73 656e 7369 7469 7665 3d22  di:insensitive="
-00002b50: 7472 7565 2220 2f3e 0a20 2020 203c 7265  true" />.    <re
-00002b60: 6374 0a20 2020 2020 2020 7374 796c 653d  ct.       style=
-00002b70: 226f 7061 6369 7479 3a30 2e33 3b66 696c  "opacity:0.3;fil
-00002b80: 6c3a 2331 3338 3839 623b 7374 726f 6b65  l:#13889b;stroke
-00002b90: 3a23 3030 3030 3030 3b73 7472 6f6b 652d  :#000000;stroke-
-00002ba0: 7769 6474 683a 303b 7374 726f 6b65 2d6c  width:0;stroke-l
-00002bb0: 696e 6563 6170 3a72 6f75 6e64 3b73 7472  inecap:round;str
-00002bc0: 6f6b 652d 6c69 6e65 6a6f 696e 3a62 6576  oke-linejoin:bev
-00002bd0: 656c 3b73 7472 6f6b 652d 6d69 7465 726c  el;stroke-miterl
-00002be0: 696d 6974 3a34 3b73 7472 6f6b 652d 6461  imit:4;stroke-da
-00002bf0: 7368 6172 7261 793a 6e6f 6e65 220a 2020  sharray:none".  
-00002c00: 2020 2020 2069 643d 2272 6563 7432 3030       id="rect200
-00002c10: 3322 0a20 2020 2020 2020 7769 6474 683d  3".       width=
-00002c20: 2231 332e 3339 3734 3539 220a 2020 2020  "13.397459".    
-00002c30: 2020 2068 6569 6768 743d 2231 352e 3437     height="15.47
-00002c40: 3030 3534 220a 2020 2020 2020 2078 3d22  0054".       x="
-00002c50: 3339 2e34 3333 3735 3422 0a20 2020 2020  39.433754".     
-00002c60: 2020 793d 222d 342e 3930 3338 3038 3622    y="-4.9038086"
-00002c70: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
-00002c80: 3a6c 6162 656c 3d22 5175 6164 7261 6e74  :label="Quadrant
-00002c90: 2033 220a 2020 2020 2020 2074 7261 6e73   3".       trans
-00002ca0: 666f 726d 3d22 6d61 7472 6978 2830 2e38  form="matrix(0.8
-00002cb0: 3636 3032 3534 2c30 2e35 2c2d 302e 3836  660254,0.5,-0.86
-00002cc0: 3630 3235 342c 302e 352c 302c 3029 220a  60254,0.5,0,0)".
-00002cd0: 2020 2020 2020 2073 6f64 6970 6f64 693a         sodipodi:
-00002ce0: 696e 7365 6e73 6974 6976 653d 2274 7275  insensitive="tru
-00002cf0: 6522 202f 3e0a 2020 2020 3c72 6563 740a  e" />.    <rect.
-00002d00: 2020 2020 2020 2073 7479 6c65 3d22 6f70         style="op
-00002d10: 6163 6974 793a 302e 333b 6669 6c6c 3a23  acity:0.3;fill:#
-00002d20: 3230 6339 3937 3b73 7472 6f6b 653a 2330  20c997;stroke:#0
-00002d30: 3030 3030 303b 7374 726f 6b65 2d77 6964  00000;stroke-wid
-00002d40: 7468 3a30 3b73 7472 6f6b 652d 6c69 6e65  th:0;stroke-line
-00002d50: 6361 703a 726f 756e 643b 7374 726f 6b65  cap:round;stroke
-00002d60: 2d6c 696e 656a 6f69 6e3a 6265 7665 6c3b  -linejoin:bevel;
-00002d70: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
-00002d80: 743a 343b 7374 726f 6b65 2d64 6173 6861  t:4;stroke-dasha
-00002d90: 7272 6179 3a6e 6f6e 6522 0a20 2020 2020  rray:none".     
-00002da0: 2020 6964 3d22 7265 6374 3230 3035 220a    id="rect2005".
-00002db0: 2020 2020 2020 2077 6964 7468 3d22 3133         width="13
-00002dc0: 2e33 3937 3435 3922 0a20 2020 2020 2020  .397459".       
-00002dd0: 6865 6967 6874 3d22 3135 2e34 3730 3035  height="15.47005
-00002de0: 3422 0a20 2020 2020 2020 783d 2233 392e  4".       x="39.
-00002df0: 3433 3337 3534 220a 2020 2020 2020 2079  433754".       y
-00002e00: 3d22 3130 2e35 3636 3234 3322 0a20 2020  ="10.566243".   
-00002e10: 2020 2020 696e 6b73 6361 7065 3a6c 6162      inkscape:lab
-00002e20: 656c 3d22 5175 6164 7261 6e74 2034 220a  el="Quadrant 4".
-00002e30: 2020 2020 2020 2074 7261 6e73 666f 726d         transform
-00002e40: 3d22 6d61 7472 6978 2830 2e38 3636 3032  ="matrix(0.86602
-00002e50: 3534 2c30 2e35 2c2d 302e 3836 3630 3235  54,0.5,-0.866025
-00002e60: 342c 302e 352c 302c 3029 220a 2020 2020  4,0.5,0,0)".    
-00002e70: 2020 2073 6f64 6970 6f64 693a 696e 7365     sodipodi:inse
-00002e80: 6e73 6974 6976 653d 2274 7275 6522 202f  nsitive="true" /
-00002e90: 3e0a 2020 2020 3c72 6563 740a 2020 2020  >.    <rect.    
-00002ea0: 2020 2073 7479 6c65 3d22 6f70 6163 6974     style="opacit
-00002eb0: 793a 313b 6669 6c6c 3a6e 6f6e 653b 6669  y:1;fill:none;fi
-00002ec0: 6c6c 2d6f 7061 6369 7479 3a31 3b73 7472  ll-opacity:1;str
-00002ed0: 6f6b 653a 2330 3030 3030 303b 7374 726f  oke:#000000;stro
-00002ee0: 6b65 2d77 6964 7468 3a30 2e33 3232 3337  ke-width:0.32237
-00002ef0: 313b 7374 726f 6b65 2d6c 696e 6563 6170  1;stroke-linecap
-00002f00: 3a72 6f75 6e64 3b73 7472 6f6b 652d 6c69  :round;stroke-li
-00002f10: 6e65 6a6f 696e 3a6d 6974 6572 3b73 7472  nejoin:miter;str
-00002f20: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
-00002f30: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
-00002f40: 793a 6e6f 6e65 220a 2020 2020 2020 2069  y:none".       i
-00002f50: 643d 2272 6563 7434 3933 3722 0a20 2020  d="rect4937".   
-00002f60: 2020 2020 7769 6474 683d 2232 362e 3739      width="26.79
-00002f70: 3439 3138 220a 2020 2020 2020 2068 6569  4918".       hei
-00002f80: 6768 743d 2233 302e 3934 3031 3037 220a  ght="30.940107".
-00002f90: 2020 2020 2020 2078 3d22 3236 2e30 3336         x="26.036
-00002fa0: 3239 3922 0a20 2020 2020 2020 793d 222d  299".       y="-
-00002fb0: 342e 3930 3338 3038 3622 0a20 2020 2020  4.9038086".     
-00002fc0: 2020 696e 6b73 6361 7065 3a6c 6162 656c    inkscape:label
-00002fd0: 3d22 4672 616d 6522 0a20 2020 2020 2020  ="Frame".       
-00002fe0: 7472 616e 7366 6f72 6d3d 226d 6174 7269  transform="matri
-00002ff0: 7828 302e 3836 3630 3235 342c 302e 352c  x(0.8660254,0.5,
-00003000: 2d30 2e38 3636 3032 3534 2c30 2e35 2c30  -0.8660254,0.5,0
-00003010: 2c30 2922 0a20 2020 2020 2020 736f 6469  ,0)".       sodi
-00003020: 706f 6469 3a69 6e73 656e 7369 7469 7665  podi:insensitive
-00003030: 3d22 7472 7565 2220 2f3e 0a20 2020 203c  ="true" />.    <
-00003040: 7061 7468 0a20 2020 2020 2020 7374 796c  path.       styl
-00003050: 653d 2266 696c 6c3a 6e6f 6e65 3b73 7472  e="fill:none;str
-00003060: 6f6b 653a 2330 3030 3030 303b 7374 726f  oke:#000000;stro
-00003070: 6b65 2d77 6964 7468 3a30 2e30 3533 3538  ke-width:0.05358
-00003080: 3939 3b73 7472 6f6b 652d 6c69 6e65 6361  99;stroke-lineca
-00003090: 703a 6275 7474 3b73 7472 6f6b 652d 6c69  p:butt;stroke-li
-000030a0: 6e65 6a6f 696e 3a6d 6974 6572 3b73 7472  nejoin:miter;str
-000030b0: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
-000030c0: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
-000030d0: 793a 302e 3432 3837 3139 2c20 302e 3432  y:0.428719, 0.42
-000030e0: 3837 3139 3b73 7472 6f6b 652d 6461 7368  8719;stroke-dash
-000030f0: 6f66 6673 6574 3a30 3b73 7472 6f6b 652d  offset:0;stroke-
-00003100: 6f70 6163 6974 793a 3122 0a20 2020 2020  opacity:1".     
-00003110: 2020 643d 224d 2031 332e 3339 3734 3632    d="M 13.397462
-00003120: 2c31 382e 3330 3132 3732 2033 362e 3630  ,18.301272 36.60
-00003130: 3235 3433 2c33 312e 3639 3837 3322 0a20  2543,31.69873". 
-00003140: 2020 2020 2020 6964 3d22 7061 7468 3532        id="path52
-00003150: 3634 220a 2020 2020 2020 2069 6e6b 7363  64".       inksc
-00003160: 6170 653a 6c61 6265 6c3d 2258 2d41 7869  ape:label="X-Axi
-00003170: 7322 0a20 2020 2020 2020 736f 6469 706f  s".       sodipo
-00003180: 6469 3a69 6e73 656e 7369 7469 7665 3d22  di:insensitive="
-00003190: 7472 7565 2220 2f3e 0a20 2020 203c 7061  true" />.    <pa
-000031a0: 7468 0a20 2020 2020 2020 7374 796c 653d  th.       style=
-000031b0: 2266 696c 6c3a 6e6f 6e65 3b73 7472 6f6b  "fill:none;strok
-000031c0: 653a 2330 3030 3030 303b 7374 726f 6b65  e:#000000;stroke
-000031d0: 2d77 6964 7468 3a30 2e30 3533 3538 3939  -width:0.0535899
-000031e0: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
-000031f0: 6275 7474 3b73 7472 6f6b 652d 6c69 6e65  butt;stroke-line
-00003200: 6a6f 696e 3a6d 6974 6572 3b73 7472 6f6b  join:miter;strok
-00003210: 652d 6d69 7465 726c 696d 6974 3a34 3b73  e-miterlimit:4;s
-00003220: 7472 6f6b 652d 6461 7368 6172 7261 793a  troke-dasharray:
-00003230: 302e 3432 3837 3139 2c20 302e 3432 3837  0.428719, 0.4287
-00003240: 3139 3b73 7472 6f6b 652d 6461 7368 6f66  19;stroke-dashof
-00003250: 6673 6574 3a30 3b73 7472 6f6b 652d 6f70  fset:0;stroke-op
-00003260: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
-00003270: 643d 224d 2033 382e 3339 3734 3632 2c31  d="M 38.397462,1
-00003280: 372e 3236 3439 3735 2031 312e 3630 3235  7.264975 11.6025
-00003290: 3431 2c33 322e 3733 3530 3237 220a 2020  41,32.735027".  
-000032a0: 2020 2020 2069 643d 2270 6174 6835 3539       id="path559
-000032b0: 3622 0a20 2020 2020 2020 696e 6b73 6361  6".       inksca
-000032c0: 7065 3a6c 6162 656c 3d22 592d 4178 6973  pe:label="Y-Axis
-000032d0: 220a 2020 2020 2020 2073 6f64 6970 6f64  ".       sodipod
-000032e0: 693a 696e 7365 6e73 6974 6976 653d 2274  i:insensitive="t
-000032f0: 7275 6522 202f 3e0a 2020 3c2f 673e 0a20  rue" />.  </g>. 
-00003300: 203c 670a 2020 2020 2069 6e6b 7363 6170   <g.     inkscap
-00003310: 653a 6772 6f75 706d 6f64 653d 226c 6179  e:groupmode="lay
-00003320: 6572 220a 2020 2020 2069 643d 226c 6179  er".     id="lay
-00003330: 6572 3322 0a20 2020 2020 696e 6b73 6361  er3".     inksca
-00003340: 7065 3a6c 6162 656c 3d22 506f 6c61 7222  pe:label="Polar"
-00003350: 0a20 2020 2020 736f 6469 706f 6469 3a69  .     sodipodi:i
-00003360: 6e73 656e 7369 7469 7665 3d22 7472 7565  nsensitive="true
-00003370: 223e 0a20 2020 203c 7061 7468 0a20 2020  ">.    <path.   
-00003380: 2020 2020 6964 3d22 7061 7468 3937 3033      id="path9703
-00003390: 220a 2020 2020 2020 2073 7479 6c65 3d22  ".       style="
-000033a0: 6469 7370 6c61 793a 696e 6c69 6e65 3b6f  display:inline;o
-000033b0: 7061 6369 7479 3a30 2e37 3b66 696c 6c3a  pacity:0.7;fill:
-000033c0: 2361 6264 6565 353b 7374 726f 6b65 3a23  #abdee5;stroke:#
-000033d0: 3030 3030 3030 3b73 7472 6f6b 652d 7769  000000;stroke-wi
-000033e0: 6474 683a 302e 3130 3036 3b73 7472 6f6b  dth:0.1006;strok
-000033f0: 652d 6c69 6e65 6361 703a 726f 756e 643b  e-linecap:round;
-00003400: 7374 726f 6b65 2d6c 696e 656a 6f69 6e3a  stroke-linejoin:
-00003410: 726f 756e 643b 7374 726f 6b65 2d6d 6974  round;stroke-mit
-00003420: 6572 6c69 6d69 743a 303b 7374 726f 6b65  erlimit:0;stroke
-00003430: 2d64 6173 6861 7272 6179 3a6e 6f6e 6522  -dasharray:none"
-00003440: 0a20 2020 2020 2020 643d 226d 2031 322e  .       d="m 12.
-00003450: 3431 3833 3337 2c33 322e 3235 3634 3032  418337,32.256402
-00003460: 2030 2e30 3230 3236 2c2d 302e 3031 3137   0.02026,-0.0117
-00003470: 3220 302e 3132 3633 3833 2c2d 312e 3030  2 0.126383,-1.00
-00003480: 3435 3633 2030 2e31 3236 3131 312c 2d31  4563 0.126111,-1
-00003490: 2e30 3034 3431 3120 312e 3733 3936 3935  .004411 1.739695
-000034a0: 2c2d 302e 3037 3238 2031 2e37 3339 3639  ,-0.0728 1.73969
-000034b0: 322c 2d30 2e30 3732 3820 302e 3032 3032  2,-0.0728 0.0202
-000034c0: 362c 2d30 2e30 3131 3732 2063 202d 342e  6,-0.01172 c -4.
-000034d0: 3231 3031 2c2d 322e 3433 3037 3939 202d  2101,-2.430799 -
-000034e0: 332e 3638 3139 3933 2c2d 362e 3637 3636  3.681993,-6.6766
-000034f0: 3634 2031 2e31 3739 3535 372c 2d39 2e34  64 1.179557,-9.4
-00003500: 3833 3431 3820 342e 3836 3134 3638 2c2d  83418 4.861468,-
-00003510: 322e 3830 3636 3839 2031 322e 3231 3533  2.806689 12.2153
-00003520: 3233 2c2d 332e 3131 3135 3231 2031 362e  23,-3.111521 16.
-00003530: 3432 3534 3939 2c2d 302e 3638 3038 3639  425499,-0.680869
-00003540: 206c 2033 2e35 3130 3135 352c 2d30 2e31   l 3.510155,-0.1
-00003550: 3633 3338 3220 302e 3236 3235 3238 2c2d  63382 0.262528,-
-00003560: 322e 3031 3437 3734 2043 2033 312e 3535  2.014774 C 31.55
-00003570: 3339 3133 2c31 342e 3236 3334 3333 2032  3913,14.263433 2
-00003580: 312e 3034 3830 3831 2c31 342e 3639 3839  1.048081,14.6989
-00003590: 3220 3134 2e31 3033 3036 312c 3138 2e37  2 14.103061,18.7
-000035a0: 3038 3633 3620 372e 3135 3830 3237 2c32  08636 7.158027,2
-000035b0: 322e 3731 3833 3435 2036 2e34 3033 3734  2.718345 6.40374
-000035c0: 3134 2c32 382e 3738 3338 3932 2031 322e  14,28.783892 12.
-000035d0: 3431 3833 322c 3332 2e32 3536 3420 5a22  41832,32.2564 Z"
-000035e0: 0a20 2020 2020 2020 736f 6469 706f 6469  .       sodipodi
-000035f0: 3a6e 6f64 6574 7970 6573 3d22 6363 6363  :nodetypes="cccc
-00003600: 6363 6363 6363 6363 6322 0a20 2020 2020  ccccccccc".     
-00003610: 2020 696e 6b73 6361 7065 3a6c 6162 656c    inkscape:label
-00003620: 3d22 446f 6e75 7420 312d 3222 0a20 2020  ="Donut 1-2".   
-00003630: 2020 2020 736f 6469 706f 6469 3a69 6e73      sodipodi:ins
-00003640: 656e 7369 7469 7665 3d22 7472 7565 2220  ensitive="true" 
-00003650: 2f3e 0a20 2020 203c 7061 7468 0a20 2020  />.    <path.   
-00003660: 2020 2020 6964 3d22 7061 7468 3233 3633      id="path2363
-00003670: 3837 220a 2020 2020 2020 2073 7479 6c65  87".       style
-00003680: 3d22 6469 7370 6c61 793a 696e 6c69 6e65  ="display:inline
-00003690: 3b66 696c 6c3a 6e6f 6e65 3b73 7472 6f6b  ;fill:none;strok
-000036a0: 653a 2330 3030 3030 303b 7374 726f 6b65  e:#000000;stroke
-000036b0: 2d77 6964 7468 3a30 2e30 3530 3330 3032  -width:0.0503002
-000036c0: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
-000036d0: 726f 756e 643b 7374 726f 6b65 2d6d 6974  round;stroke-mit
-000036e0: 6572 6c69 6d69 743a 343b 7374 726f 6b65  erlimit:4;stroke
-000036f0: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
-00003700: 6d61 726b 6572 2d65 6e64 3a75 726c 2823  marker-end:url(#
-00003710: 4172 726f 7731 4c65 6e64 2d36 2922 0a20  Arrow1Lend-6)". 
-00003720: 2020 2020 2020 643d 224d 2031 312e 3634        d="M 11.64
-00003730: 3536 3536 2c32 392e 3032 3930 3832 2043  5656,29.029082 C
-00003740: 2039 2e35 3030 3735 3435 2c32 352e 3939   9.5007545,25.99
-00003750: 3532 3032 2031 312e 3038 3133 312c 3232  5202 11.08131,22
-00003760: 2e32 3133 3736 3520 3135 2e36 3237 3733  .213765 15.62773
-00003770: 322c 3139 2e35 3838 3838 3620 3230 2e31  2,19.588886 20.1
-00003780: 3734 3135 342c 3136 2e39 3634 3031 3120  74154,16.964011 
-00003790: 3236 2e37 3135 3534 2c31 362e 3035 3632  26.71554,16.0562
-000037a0: 3433 2033 312e 3937 3033 3734 2c31 372e  43 31.970374,17.
-000037b0: 3239 3435 3939 220a 2020 2020 2020 2073  294599".       s
-000037c0: 6f64 6970 6f64 693a 6e6f 6465 7479 7065  odipodi:nodetype
-000037d0: 733d 2263 7363 220a 2020 2020 2020 2069  s="csc".       i
-000037e0: 6e6b 7363 6170 653a 6c61 6265 6c3d 2252  nkscape:label="R
-000037f0: 6f74 6174 696e 6720 4172 726f 7720 312d  otating Arrow 1-
-00003800: 3222 0a20 2020 2020 2020 736f 6469 706f  2".       sodipo
-00003810: 6469 3a69 6e73 656e 7369 7469 7665 3d22  di:insensitive="
-00003820: 7472 7565 2220 2f3e 0a20 2020 203c 7061  true" />.    <pa
-00003830: 7468 0a20 2020 2020 2020 6964 3d22 7061  th.       id="pa
-00003840: 7468 3832 3633 2d36 2d34 220a 2020 2020  th8263-6-4".    
-00003850: 2020 2073 7479 6c65 3d22 6469 7370 6c61     style="displa
-00003860: 793a 696e 6c69 6e65 3b6f 7061 6369 7479  y:inline;opacity
-00003870: 3a30 2e37 3b66 696c 6c3a 2361 6264 6565  :0.7;fill:#abdee
-00003880: 353b 7374 726f 6b65 3a23 3030 3030 3030  5;stroke:#000000
-00003890: 3b73 7472 6f6b 652d 7769 6474 683a 302e  ;stroke-width:0.
-000038a0: 3130 3034 3236 3b73 7472 6f6b 652d 6c69  100426;stroke-li
-000038b0: 6e65 6361 703a 726f 756e 643b 7374 726f  necap:round;stro
-000038c0: 6b65 2d6c 696e 656a 6f69 6e3a 6265 7665  ke-linejoin:beve
-000038d0: 6c3b 7374 726f 6b65 2d6d 6974 6572 6c69  l;stroke-miterli
-000038e0: 6d69 743a 303b 7374 726f 6b65 2d64 6173  mit:0;stroke-das
-000038f0: 6861 7272 6179 3a6e 6f6e 6522 0a20 2020  harray:none".   
-00003900: 2020 2020 643d 226d 2033 372e 3630 3633      d="m 37.6063
-00003910: 3238 2c31 372e 3735 3736 3938 202d 302e  28,17.757698 -0.
-00003920: 3032 3032 362c 302e 3031 3137 3220 2d30  02026,0.01172 -0
-00003930: 2e31 3239 3136 382c 312e 3030 3239 3537  .129168,1.002957
-00003940: 202d 302e 3132 3839 3132 2c31 2e30 3032   -0.128912,1.002
-00003950: 3830 3520 2d31 2e37 3336 3930 392c 302e  805 -1.736909,0.
-00003960: 3037 3434 3320 2d31 2e37 3336 3930 392c  07443 -1.736909,
-00003970: 302e 3037 3434 3220 2d30 2e30 3230 3236  0.07442 -0.02026
-00003980: 2c30 2e30 3131 3732 2063 2034 2e31 3935  ,0.01172 c 4.195
-00003990: 3532 372c 322e 3432 3233 3832 2033 2e36  527,2.422382 3.6
-000039a0: 3535 3538 332c 362e 3636 3134 3433 202d  55583,6.661443 -
-000039b0: 312e 3230 362c 392e 3436 3832 3139 202d  1.206,9.468219 -
-000039c0: 342e 3836 3135 3033 2c32 2e38 3036 3730  4.861503,2.80670
-000039d0: 3720 2d31 322e 3230 3335 3734 2c33 2e31  7 -12.203574,3.1
-000039e0: 3138 3337 3420 2d31 362e 3339 3931 3737  18374 -16.399177
-000039f0: 2c30 2e36 3936 3133 3620 6c20 2d33 2e35  ,0.696136 l -3.5
-00003a00: 3034 3538 2c30 2e31 3636 3632 3120 2d30  0458,0.166621 -0
-00003a10: 2e32 3638 3132 362c 322e 3031 3135 3620  .268126,2.01156 
-00003a20: 6320 352e 3939 3337 3435 2c33 2e34 3630  c 5.993745,3.460
-00003a30: 3439 3220 3136 2e34 3832 3733 372c 332e  492 16.482737,3.
-00003a40: 3031 3532 3435 2032 332e 3432 3738 3132  015245 23.427812
-00003a50: 2c2d 302e 3939 3435 3031 2036 2e39 3435  ,-0.994501 6.945
-00003a60: 3037 382c 2d34 2e30 3039 3733 3820 372e  078,-4.009738 7.
-00003a70: 3731 3632 3737 2c2d 3130 2e30 3635 3536  716277,-10.06556
-00003a80: 3320 312e 3732 3235 3137 2c2d 3133 2e35  3 1.722517,-13.5
-00003a90: 3236 3035 3320 7a22 0a20 2020 2020 2020  26053 z".       
-00003aa0: 736f 6469 706f 6469 3a6e 6f64 6574 7970  sodipodi:nodetyp
-00003ab0: 6573 3d22 6363 6363 6363 6363 6363 6363  es="cccccccccccc
-00003ac0: 6322 0a20 2020 2020 2020 696e 6b73 6361  c".       inksca
-00003ad0: 7065 3a6c 6162 656c 3d22 446f 6e75 7420  pe:label="Donut 
-00003ae0: 332d 3422 0a20 2020 2020 2020 736f 6469  3-4".       sodi
-00003af0: 706f 6469 3a69 6e73 656e 7369 7469 7665  podi:insensitive
-00003b00: 3d22 7472 7565 2220 2f3e 0a20 2020 203c  ="true" />.    <
-00003b10: 7061 7468 0a20 2020 2020 2020 6964 3d22  path.       id="
-00003b20: 7061 7468 3233 3439 3336 220a 2020 2020  path234936".    
-00003b30: 2020 2073 7479 6c65 3d22 6469 7370 6c61     style="displa
-00003b40: 793a 696e 6c69 6e65 3b66 696c 6c3a 6e6f  y:inline;fill:no
-00003b50: 6e65 3b73 7472 6f6b 653a 2330 3030 3030  ne;stroke:#00000
-00003b60: 303b 7374 726f 6b65 2d77 6964 7468 3a30  0;stroke-width:0
-00003b70: 2e30 3530 3330 3032 3b73 7472 6f6b 652d  .0503002;stroke-
-00003b80: 6c69 6e65 6361 703a 726f 756e 643b 7374  linecap:round;st
-00003b90: 726f 6b65 2d6d 6974 6572 6c69 6d69 743a  roke-miterlimit:
-00003ba0: 343b 7374 726f 6b65 2d64 6173 6861 7272  4;stroke-dasharr
-00003bb0: 6179 3a6e 6f6e 653b 6d61 726b 6572 2d65  ay:none;marker-e
-00003bc0: 6e64 3a75 726c 2823 4172 726f 7731 4c65  nd:url(#Arrow1Le
-00003bd0: 6e64 2d36 2922 0a20 2020 2020 2020 643d  nd-6)".       d=
-00003be0: 226d 2033 382e 3235 3031 3231 2c32 302e  "m 38.250121,20.
-00003bf0: 3931 3534 3437 2063 2032 2e31 3434 3839  915447 c 2.14489
-00003c00: 372c 332e 3033 3338 3820 302e 3534 3634  7,3.03388 0.5464
-00003c10: 3937 2c36 2e38 3030 3234 3220 2d33 2e39  97,6.800242 -3.9
-00003c20: 3939 3932 392c 392e 3432 3531 3220 2d34  99929,9.42512 -4
-00003c30: 2e35 3436 3432 342c 322e 3632 3438 3820  .546424,2.62488 
-00003c40: 2d31 312e 3036 3939 3534 2c33 2e35 3437  -11.069954,3.547
-00003c50: 3731 3920 2d31 362e 3332 3437 3932 2c32  719 -16.324792,2
-00003c60: 2e33 3039 3336 3222 0a20 2020 2020 2020  .309362".       
-00003c70: 736f 6469 706f 6469 3a6e 6f64 6574 7970  sodipodi:nodetyp
-00003c80: 6573 3d22 6373 6322 0a20 2020 2020 2020  es="csc".       
-00003c90: 696e 6b73 6361 7065 3a6c 6162 656c 3d22  inkscape:label="
-00003ca0: 526f 7461 7469 6e67 2041 7272 6f77 2033  Rotating Arrow 3
-00003cb0: 2d34 220a 2020 2020 2020 2073 6f64 6970  -4".       sodip
-00003cc0: 6f64 693a 696e 7365 6e73 6974 6976 653d  odi:insensitive=
-00003cd0: 2274 7275 6522 202f 3e0a 2020 3c2f 673e  "true" />.  </g>
-00003ce0: 0a20 203c 670a 2020 2020 2069 643d 226c  .  <g.     id="l
-00003cf0: 6179 6572 3222 0a20 2020 2020 696e 6b73  ayer2".     inks
-00003d00: 6361 7065 3a6c 6162 656c 3d22 5570 7065  cape:label="Uppe
-00003d10: 7222 0a20 2020 2020 7374 796c 653d 2264  r".     style="d
-00003d20: 6973 706c 6179 3a69 6e6c 696e 6522 0a20  isplay:inline". 
-00003d30: 2020 2020 736f 6469 706f 6469 3a69 6e73      sodipodi:ins
-00003d40: 656e 7369 7469 7665 3d22 7472 7565 223e  ensitive="true">
-00003d50: 0a20 2020 203c 7061 7468 0a20 2020 2020  .    <path.     
-00003d60: 2020 7374 796c 653d 2264 6973 706c 6179    style="display
-00003d70: 3a69 6e6c 696e 653b 6f70 6163 6974 793a  :inline;opacity:
-00003d80: 302e 333b 6669 6c6c 3a23 6162 6465 6535  0.3;fill:#abdee5
-00003d90: 3b73 7472 6f6b 653a 2330 3030 3030 303b  ;stroke:#000000;
-00003da0: 7374 726f 6b65 2d77 6964 7468 3a30 3b73  stroke-width:0;s
-00003db0: 7472 6f6b 652d 6c69 6e65 6361 703a 6275  troke-linecap:bu
-00003dc0: 7474 3b73 7472 6f6b 652d 6c69 6e65 6a6f  tt;stroke-linejo
-00003dd0: 696e 3a6d 6974 6572 3b73 7472 6f6b 652d  in:miter;stroke-
-00003de0: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
-00003df0: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
-00003e00: 6e65 3b73 7472 6f6b 652d 6f70 6163 6974  ne;stroke-opacit
-00003e10: 793a 3122 0a20 2020 2020 2020 643d 226d  y:1".       d="m
-00003e20: 2031 342e 3236 3334 3837 2c31 372e 3830   14.263487,17.80
-00003e30: 3132 3731 2063 2030 2c30 2032 2e37 3639  1271 c 0,0 2.769
-00003e40: 3436 332c 2d31 332e 3833 3733 3137 3720  463,-13.8373177 
-00003e50: 362e 3331 3836 3731 2c2d 3135 2e39 3631  6.318671,-15.961
-00003e60: 3438 3637 206c 202d 312e 3733 3139 3839  4867 l -1.731989
-00003e70: 2c30 2e39 3939 3936 3320 6320 2d33 2e35  ,0.999963 c -3.5
-00003e80: 3439 3230 382c 322e 3132 3431 3720 2d36  49208,2.12417 -6
-00003e90: 2e33 3138 3637 312c 3135 2e39 3631 3438  .318671,15.96148
-00003ea0: 3637 202d 362e 3331 3836 3731 2c31 352e  67 -6.318671,15.
-00003eb0: 3936 3134 3836 3720 7a22 0a20 2020 2020  9614867 z".     
-00003ec0: 2020 6964 3d22 7061 7468 3434 3631 220a    id="path4461".
-00003ed0: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
-00003ee0: 6c61 6265 6c3d 2242 616e 6420 3122 0a20  label="Band 1". 
-00003ef0: 2020 2020 2020 736f 6469 706f 6469 3a6e        sodipodi:n
-00003f00: 6f64 6574 7970 6573 3d22 6363 6363 6322  odetypes="ccccc"
-00003f10: 0a20 2020 2020 2020 736f 6469 706f 6469  .       sodipodi
-00003f20: 3a69 6e73 656e 7369 7469 7665 3d22 7472  :insensitive="tr
-00003f30: 7565 2220 2f3e 0a20 2020 203c 7061 7468  ue" />.    <path
-00003f40: 0a20 2020 2020 2020 7374 796c 653d 2264  .       style="d
-00003f50: 6973 706c 6179 3a69 6e6c 696e 653b 6669  isplay:inline;fi
-00003f60: 6c6c 3a6e 6f6e 653b 7374 726f 6b65 3a23  ll:none;stroke:#
-00003f70: 3030 3030 3030 3b73 7472 6f6b 652d 7769  000000;stroke-wi
-00003f80: 6474 683a 302e 313b 7374 726f 6b65 2d6c  dth:0.1;stroke-l
-00003f90: 696e 6563 6170 3a62 7574 743b 7374 726f  inecap:butt;stro
-00003fa0: 6b65 2d6c 696e 656a 6f69 6e3a 6d69 7465  ke-linejoin:mite
-00003fb0: 723b 7374 726f 6b65 2d6d 6974 6572 6c69  r;stroke-miterli
-00003fc0: 6d69 743a 343b 7374 726f 6b65 2d64 6173  mit:4;stroke-das
-00003fd0: 6861 7272 6179 3a6e 6f6e 653b 7374 726f  harray:none;stro
-00003fe0: 6b65 2d6f 7061 6369 7479 3a31 220a 2020  ke-opacity:1".  
-00003ff0: 2020 2020 2064 3d22 6d20 3134 2e32 3633       d="m 14.263
-00004000: 3438 372c 3137 2e38 3031 3237 3120 6320  487,17.801271 c 
-00004010: 302c 3020 322e 3736 3934 3633 2c2d 3133  0,0 2.769463,-13
-00004020: 2e38 3337 3331 3737 2036 2e33 3138 3637  .8373177 6.31867
-00004030: 312c 2d31 352e 3936 3134 3836 3720 6c20  1,-15.9614867 l 
-00004040: 2d31 2e37 3331 3938 392c 302e 3939 3939  -1.731989,0.9999
-00004050: 3633 2063 202d 332e 3534 3932 3038 2c32  63 c -3.549208,2
-00004060: 2e31 3234 3137 202d 362e 3331 3836 3731  .12417 -6.318671
-00004070: 2c31 352e 3936 3134 3836 3720 2d36 2e33  ,15.9614867 -6.3
-00004080: 3138 3637 312c 3135 2e39 3631 3438 3637  18671,15.9614867
-00004090: 220a 2020 2020 2020 2069 643d 2270 6174  ".       id="pat
-000040a0: 6832 3437 3722 0a20 2020 2020 2020 696e  h2477".       in
-000040b0: 6b73 6361 7065 3a6c 6162 656c 3d22 4c69  kscape:label="Li
-000040c0: 6e65 2031 220a 2020 2020 2020 2073 6f64  ne 1".       sod
-000040d0: 6970 6f64 693a 6e6f 6465 7479 7065 733d  ipodi:nodetypes=
-000040e0: 2263 6363 6322 0a20 2020 2020 2020 736f  "cccc".       so
-000040f0: 6469 706f 6469 3a69 6e73 656e 7369 7469  dipodi:insensiti
-00004100: 7665 3d22 7472 7565 2220 2f3e 0a20 2020  ve="true" />.   
-00004110: 203c 7061 7468 0a20 2020 2020 2020 7374   <path.       st
-00004120: 796c 653d 2264 6973 706c 6179 3a69 6e6c  yle="display:inl
-00004130: 696e 653b 6f70 6163 6974 793a 302e 333b  ine;opacity:0.3;
-00004140: 6669 6c6c 3a23 6162 6465 6535 3b73 7472  fill:#abdee5;str
-00004150: 6f6b 653a 2330 3030 3030 303b 7374 726f  oke:#000000;stro
-00004160: 6b65 2d77 6964 7468 3a30 3b73 7472 6f6b  ke-width:0;strok
-00004170: 652d 6c69 6e65 6361 703a 6275 7474 3b73  e-linecap:butt;s
-00004180: 7472 6f6b 652d 6c69 6e65 6a6f 696e 3a6d  troke-linejoin:m
-00004190: 6974 6572 3b73 7472 6f6b 652d 6d69 7465  iter;stroke-mite
-000041a0: 726c 696d 6974 3a34 3b73 7472 6f6b 652d  rlimit:4;stroke-
-000041b0: 6461 7368 6172 7261 793a 6e6f 6e65 3b73  dasharray:none;s
-000041c0: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
-000041d0: 0a20 2020 2020 2020 643d 226d 2032 352e  .       d="m 25.
-000041e0: 3836 3630 3237 2c32 342e 3530 3030 3031  866027,24.500001
-000041f0: 2063 2030 2c30 2030 2e37 3536 3037 392c   c 0,0 0.756079,
-00004200: 2d32 302e 3230 3235 3135 3720 2d33 2e35  -20.2025157 -3.5
-00004210: 3730 3538 2c2d 3232 2e37 3030 3531 3237  7058,-22.7005127
-00004220: 202d 302e 3538 3438 3732 2c2d 302e 3333   -0.584872,-0.33
-00004230: 3736 3736 202d 312e 3135 3835 3139 2c2d  7676 -1.158519,-
-00004240: 302e 3239 3137 3239 202d 312e 3731 3332  0.291729 -1.7132
-00004250: 3839 2c30 2e30 3430 3320 6c20 2d31 2e37  89,0.0403 l -1.7
-00004260: 3332 3035 312c 302e 3939 3939 3939 2063  32051,0.999999 c
-00004270: 2030 2e35 3534 3737 2c2d 302e 3333 3230   0.55477,-0.3320
-00004280: 3235 2031 2e31 3238 3431 372c 2d30 2e33  25 1.128417,-0.3
-00004290: 3737 3937 3220 312e 3731 3332 3839 2c2d  77972 1.713289,-
-000042a0: 302e 3034 3033 2034 2e33 3236 3635 392c  0.0403 4.326659,
-000042b0: 322e 3439 3739 3937 2033 2e35 3730 3538  2.497997 3.57058
-000042c0: 2c32 322e 3730 3035 3133 3720 332e 3537  ,22.7005137 3.57
-000042d0: 3035 382c 3232 2e37 3030 3531 3337 220a  058,22.7005137".
-000042e0: 2020 2020 2020 2069 643d 2270 6174 6834         id="path4
-000042f0: 3334 3530 220a 2020 2020 2020 2069 6e6b  3450".       ink
-00004300: 7363 6170 653a 6c61 6265 6c3d 2242 616e  scape:label="Ban
-00004310: 6420 3222 0a20 2020 2020 2020 736f 6469  d 2".       sodi
-00004320: 706f 6469 3a6e 6f64 6574 7970 6573 3d22  podi:nodetypes="
-00004330: 6373 6363 7363 220a 2020 2020 2020 2073  csccsc".       s
-00004340: 6f64 6970 6f64 693a 696e 7365 6e73 6974  odipodi:insensit
-00004350: 6976 653d 2274 7275 6522 202f 3e0a 2020  ive="true" />.  
-00004360: 2020 3c70 6174 680a 2020 2020 2020 2073    <path.       s
-00004370: 7479 6c65 3d22 6469 7370 6c61 793a 696e  tyle="display:in
-00004380: 6c69 6e65 3b66 696c 6c3a 6e6f 6e65 3b73  line;fill:none;s
-00004390: 7472 6f6b 653a 2330 3030 3030 303b 7374  troke:#000000;st
-000043a0: 726f 6b65 2d77 6964 7468 3a30 2e31 3b73  roke-width:0.1;s
-000043b0: 7472 6f6b 652d 6c69 6e65 6361 703a 7371  troke-linecap:sq
-000043c0: 7561 7265 3b73 7472 6f6b 652d 6c69 6e65  uare;stroke-line
-000043d0: 6a6f 696e 3a6d 6974 6572 3b73 7472 6f6b  join:miter;strok
-000043e0: 652d 6d69 7465 726c 696d 6974 3a34 3b73  e-miterlimit:4;s
-000043f0: 7472 6f6b 652d 6461 7368 6172 7261 793a  troke-dasharray:
-00004400: 6e6f 6e65 3b73 7472 6f6b 652d 6f70 6163  none;stroke-opac
-00004410: 6974 793a 3122 0a20 2020 2020 2020 643d  ity:1".       d=
-00004420: 226d 2032 342e 3133 3339 3736 2c32 352e  "m 24.133976,25.
-00004430: 3530 3030 3031 2063 2030 2c30 2030 2e37  500001 c 0,0 0.7
-00004440: 3536 3037 392c 2d32 302e 3230 3235 3135  56079,-20.202515
-00004450: 3720 2d33 2e35 3730 3538 2c2d 3232 2e37  7 -3.57058,-22.7
-00004460: 3030 3531 3237 202d 302e 3538 3438 3732  005127 -0.584872
-00004470: 2c2d 302e 3333 3736 3736 202d 312e 3135  ,-0.337676 -1.15
-00004480: 3835 3139 2c2d 302e 3239 3137 3239 202d  8519,-0.291729 -
-00004490: 312e 3731 3332 3839 2c30 2e30 3430 3320  1.713289,0.0403 
-000044a0: 6c20 312e 3733 3230 3531 2c2d 3120 6320  l 1.732051,-1 c 
-000044b0: 302e 3535 3437 372c 2d30 2e33 3332 3032  0.55477,-0.33202
-000044c0: 3520 312e 3132 3834 3137 2c2d 302e 3337  5 1.128417,-0.37
-000044d0: 3739 3732 2031 2e37 3133 3238 392c 2d30  7972 1.713289,-0
-000044e0: 2e30 3430 3320 342e 3332 3636 3539 2c32  .0403 4.326659,2
-000044f0: 2e34 3937 3939 3720 332e 3537 3035 382c  .497997 3.57058,
-00004500: 3232 2e37 3030 3531 3237 2033 2e35 3730  22.7005127 3.570
-00004510: 3538 2c32 322e 3730 3035 3132 3722 0a20  58,22.7005127". 
-00004520: 2020 2020 2020 6964 3d22 7061 7468 3532        id="path52
-00004530: 3433 3722 0a20 2020 2020 2020 696e 6b73  437".       inks
-00004540: 6361 7065 3a6c 6162 656c 3d22 4c69 6e65  cape:label="Line
-00004550: 2032 220a 2020 2020 2020 2073 6f64 6970   2".       sodip
-00004560: 6f64 693a 6e6f 6465 7479 7065 733d 2263  odi:nodetypes="c
-00004570: 7363 6373 6322 0a20 2020 2020 2020 736f  sccsc".       so
-00004580: 6469 706f 6469 3a69 6e73 656e 7369 7469  dipodi:insensiti
-00004590: 7665 3d22 7472 7565 2220 2f3e 0a20 2020  ve="true" />.   
-000045a0: 203c 7061 7468 0a20 2020 2020 2020 6964   <path.       id
-000045b0: 3d22 7061 7468 3933 3539 220a 2020 2020  ="path9359".    
-000045c0: 2020 2073 7479 6c65 3d22 6469 7370 6c61     style="displa
-000045d0: 793a 696e 6c69 6e65 3b6f 7061 6369 7479  y:inline;opacity
-000045e0: 3a30 2e33 3b66 696c 6c3a 2361 6264 6565  :0.3;fill:#abdee
-000045f0: 353b 6669 6c6c 2d6f 7061 6369 7479 3a31  5;fill-opacity:1
-00004600: 3b73 7472 6f6b 653a 2330 3030 3030 303b  ;stroke:#000000;
-00004610: 7374 726f 6b65 2d77 6964 7468 3a30 3b73  stroke-width:0;s
-00004620: 7472 6f6b 652d 6c69 6e65 6361 703a 726f  troke-linecap:ro
-00004630: 756e 643b 7374 726f 6b65 2d6c 696e 656a  und;stroke-linej
-00004640: 6f69 6e3a 726f 756e 643b 7374 726f 6b65  oin:round;stroke
-00004650: 2d6d 6974 6572 6c69 6d69 743a 343b 7374  -miterlimit:4;st
-00004660: 726f 6b65 2d64 6173 6861 7272 6179 3a6e  roke-dasharray:n
-00004670: 6f6e 6522 0a20 2020 2020 2020 696e 6b73  one".       inks
-00004680: 6361 7065 3a6c 6162 656c 3d22 4172 726f  cape:label="Arro
-00004690: 7722 0a20 2020 2020 2020 696e 6b73 6361  w".       inksca
-000046a0: 7065 3a74 7261 6e73 666f 726d 2d63 656e  pe:transform-cen
-000046b0: 7465 722d 793d 222d 302e 3030 3938 3533  ter-y="-0.009853
-000046c0: 3232 3133 220a 2020 2020 2020 2064 3d22  2213".       d="
-000046d0: 6d20 3335 2e37 3338 3431 352c 3332 2e31  m 35.738415,32.1
-000046e0: 3932 3238 3420 2d30 2e34 3332 3436 312c  92284 -0.432461,
-000046f0: 302e 3234 3838 3033 2030 2e36 3438 3638  0.248803 0.64868
-00004700: 392c 2d31 2e35 3232 3337 3520 302e 3634  9,-1.522375 0.64
-00004710: 3836 3838 2c2d 312e 3532 3233 3736 2030  8688,-1.522376 0
-00004720: 2e36 3438 3638 342c 302e 3737 3539 3638  .648684,0.775968
-00004730: 2030 2e36 3438 3638 372c 302e 3737 3539   0.648687,0.7759
-00004740: 3637 202d 302e 3433 3231 382c 302e 3234  67 -0.43218,0.24
-00004750: 3836 3435 220a 2020 2020 2020 2073 6f64  8645".       sod
-00004760: 6970 6f64 693a 6e6f 6465 7479 7065 733d  ipodi:nodetypes=
-00004770: 2263 6363 6363 6363 220a 2020 2020 2020  "ccccccc".      
-00004780: 2073 6f64 6970 6f64 693a 696e 7365 6e73   sodipodi:insens
-00004790: 6974 6976 653d 2274 7275 6522 202f 3e0a  itive="true" />.
-000047a0: 2020 2020 3c70 6174 680a 2020 2020 2020      <path.      
-000047b0: 2069 643d 2270 6174 6837 3532 3322 0a20   id="path7523". 
-000047c0: 2020 2020 2020 7374 796c 653d 2264 6973        style="dis
-000047d0: 706c 6179 3a69 6e6c 696e 653b 6f70 6163  play:inline;opac
-000047e0: 6974 793a 313b 6669 6c6c 3a6e 6f6e 653b  ity:1;fill:none;
-000047f0: 7374 726f 6b65 3a23 3030 3030 3030 3b73  stroke:#000000;s
-00004800: 7472 6f6b 652d 7769 6474 683a 302e 313b  troke-width:0.1;
-00004810: 7374 726f 6b65 2d6c 696e 6563 6170 3a72  stroke-linecap:r
-00004820: 6f75 6e64 3b73 7472 6f6b 652d 6c69 6e65  ound;stroke-line
-00004830: 6a6f 696e 3a72 6f75 6e64 3b73 7472 6f6b  join:round;strok
-00004840: 652d 6d69 7465 726c 696d 6974 3a34 3b73  e-miterlimit:4;s
-00004850: 7472 6f6b 652d 6461 7368 6172 7261 793a  troke-dasharray:
-00004860: 6e6f 6e65 220a 2020 2020 2020 2069 6e6b  none".       ink
-00004870: 7363 6170 653a 6c61 6265 6c3d 2241 7272  scape:label="Arr
-00004880: 6f77 220a 2020 2020 2020 2069 6e6b 7363  ow".       inksc
-00004890: 6170 653a 7472 616e 7366 6f72 6d2d 6365  ape:transform-ce
-000048a0: 6e74 6572 2d79 3d22 2d30 2e30 3039 3835  nter-y="-0.00985
-000048b0: 3332 3231 3322 0a20 2020 2020 2020 643d  32213".       d=
-000048c0: 226d 2033 352e 3733 3834 3135 2c33 322e  "m 35.738415,32.
-000048d0: 3139 3232 3834 202d 302e 3433 3234 3631  192284 -0.432461
-000048e0: 2c30 2e32 3438 3830 3320 302e 3634 3836  ,0.248803 0.6486
-000048f0: 3839 2c2d 312e 3532 3233 3735 2030 2e36  89,-1.522375 0.6
-00004900: 3438 3638 382c 2d31 2e35 3232 3337 3620  48688,-1.522376 
-00004910: 302e 3634 3836 3834 2c30 2e37 3735 3936  0.648684,0.77596
-00004920: 3820 302e 3634 3836 3837 2c30 2e37 3735  8 0.648687,0.775
-00004930: 3936 3720 2d30 2e34 3332 3138 2c30 2e32  967 -0.43218,0.2
-00004940: 3438 3634 3522 0a20 2020 2020 2020 736f  48645".       so
-00004950: 6469 706f 6469 3a6e 6f64 6574 7970 6573  dipodi:nodetypes
-00004960: 3d22 6363 6363 6363 6322 0a20 2020 2020  ="ccccccc".     
-00004970: 2020 736f 6469 706f 6469 3a69 6e73 656e    sodipodi:insen
-00004980: 7369 7469 7665 3d22 7472 7565 2220 2f3e  sitive="true" />
-00004990: 0a20 2020 203c 7061 7468 0a20 2020 2020  .    <path.     
-000049a0: 2020 7374 796c 653d 2264 6973 706c 6179    style="display
-000049b0: 3a69 6e6c 696e 653b 6669 6c6c 3a6e 6f6e  :inline;fill:non
-000049c0: 653b 7374 726f 6b65 3a23 3030 3030 3030  e;stroke:#000000
-000049d0: 3b73 7472 6f6b 652d 7769 6474 683a 302e  ;stroke-width:0.
-000049e0: 313b 7374 726f 6b65 2d6c 696e 6563 6170  1;stroke-linecap
-000049f0: 3a62 7574 743b 7374 726f 6b65 2d6c 696e  :butt;stroke-lin
-00004a00: 656a 6f69 6e3a 6d69 7465 723b 7374 726f  ejoin:miter;stro
-00004a10: 6b65 2d6d 6974 6572 6c69 6d69 743a 343b  ke-miterlimit:4;
-00004a20: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
-00004a30: 3a30 2e30 352c 2030 2e30 353b 7374 726f  :0.05, 0.05;stro
-00004a40: 6b65 2d64 6173 686f 6666 7365 743a 303b  ke-dashoffset:0;
-00004a50: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
-00004a60: 3b6d 6172 6b65 722d 656e 643a 7572 6c28  ;marker-end:url(
-00004a70: 2341 7272 6f77 314c 656e 6429 220a 2020  #Arrow1Lend)".  
-00004a80: 2020 2020 2064 3d22 6d20 3133 2e33 3930       d="m 13.390
-00004a90: 3335 362c 3138 2e32 3937 3034 3620 6320  356,18.297046 c 
-00004aa0: 302c 3020 322e 3737 3635 3637 2c2d 3133  0,0 2.776567,-13
-00004ab0: 2e38 3333 3231 3537 2036 2e33 3235 3737  .8332157 6.32577
-00004ac0: 352c 2d31 352e 3935 3733 3834 3720 302e  5,-15.9573847 0.
-00004ad0: 3535 3437 372c 2d30 2e33 3332 3032 3520  55477,-0.332025 
-00004ae0: 312e 3132 3834 3137 2c2d 302e 3337 3739  1.128417,-0.3779
-00004af0: 3732 2031 2e37 3133 3238 392c 2d30 2e30  72 1.713289,-0.0
-00004b00: 3430 3320 4320 3235 2e37 3536 3037 392c  403 C 25.756079,
-00004b10: 342e 3739 3733 3632 3320 3235 2c32 342e  4.7973623 25,24.
-00004b20: 3939 3938 3738 2032 352c 3234 2e39 3939  999878 25,24.999
-00004b30: 3837 3820 6d20 302c 3020 6320 302c 3020  878 m 0,0 c 0,0 
-00004b40: 2d30 2e37 3536 3037 392c 3230 2e32 3032  -0.756079,20.202
-00004b50: 3531 3520 332e 3537 3035 3831 2c32 322e  515 3.570581,22.
-00004b60: 3730 3035 3132 2034 2e33 3236 3635 392c  700512 4.326659,
-00004b70: 322e 3439 3739 3939 2038 2e30 3339 3036  2.497999 8.03906
-00004b80: 342c 2d31 352e 3939 3736 3739 2038 2e30  4,-15.997679 8.0
-00004b90: 3339 3036 342c 2d31 352e 3939 3736 3739  39064,-15.997679
-00004ba0: 220a 2020 2020 2020 2069 643d 2270 6174  ".       id="pat
-00004bb0: 6833 3430 3239 220a 2020 2020 2020 2069  h34029".       i
-00004bc0: 6e6b 7363 6170 653a 6c61 6265 6c3d 2243  nkscape:label="C
-00004bd0: 7572 7665 220a 2020 2020 2020 2073 6f64  urve".       sod
-00004be0: 6970 6f64 693a 6e6f 6465 7479 7065 733d  ipodi:nodetypes=
-00004bf0: 2263 7373 6363 7363 220a 2020 2020 2020  "cssccsc".      
-00004c00: 2073 6f64 6970 6f64 693a 696e 7365 6e73   sodipodi:insens
-00004c10: 6974 6976 653d 2274 7275 6522 202f 3e0a  itive="true" />.
-00004c20: 2020 3c2f 673e 0a20 203c 6d65 7461 6461    </g>.  <metada
-00004c30: 7461 0a20 2020 2020 6964 3d22 6d65 7461  ta.     id="meta
-00004c40: 6461 7461 3839 3922 3e0a 2020 2020 3c72  data899">.    <r
-00004c50: 6466 3a52 4446 3e0a 2020 2020 2020 3c63  df:RDF>.      <c
-00004c60: 633a 576f 726b 0a20 2020 2020 2020 2020  c:Work.         
-00004c70: 7264 663a 6162 6f75 743d 2222 3e0a 2020  rdf:about="">.  
-00004c80: 2020 2020 2020 3c64 633a 7469 746c 653e        <dc:title>
-00004c90: 5369 676e 616c 797a 6572 204c 6f67 6f3c  Signalyzer Logo<
-00004ca0: 2f64 633a 7469 746c 653e 0a20 2020 2020  /dc:title>.     
-00004cb0: 2020 203c 6463 3a64 6174 653e 3230 3232     <dc:date>2022
-00004cc0: 2d30 312d 3037 3c2f 6463 3a64 6174 653e  -01-07</dc:date>
-00004cd0: 0a20 2020 2020 2020 203c 6463 3a63 7265  .        <dc:cre
-00004ce0: 6174 6f72 3e0a 2020 2020 2020 2020 2020  ator>.          
-00004cf0: 3c63 633a 4167 656e 743e 0a20 2020 2020  <cc:Agent>.     
-00004d00: 2020 2020 2020 203c 6463 3a74 6974 6c65         <dc:title
-00004d10: 3e4a 6f63 6865 6e20 4765 7268 6165 7573  >Jochen Gerhaeus
-00004d20: 7365 723c 2f64 633a 7469 746c 653e 0a20  ser</dc:title>. 
-00004d30: 2020 2020 2020 2020 203c 2f63 633a 4167           </cc:Ag
-00004d40: 656e 743e 0a20 2020 2020 2020 203c 2f64  ent>.        </d
-00004d50: 633a 6372 6561 746f 723e 0a20 2020 2020  c:creator>.     
-00004d60: 2020 203c 6363 3a6c 6963 656e 7365 0a20     <cc:license. 
-00004d70: 2020 2020 2020 2020 2020 7264 663a 7265            rdf:re
-00004d80: 736f 7572 6365 3d22 6874 7470 3a2f 2f63  source="http://c
-00004d90: 7265 6174 6976 6563 6f6d 6d6f 6e73 2e6f  reativecommons.o
-00004da0: 7267 2f6c 6963 656e 7365 732f 6279 2d6e  rg/licenses/by-n
-00004db0: 632d 7361 2f34 2e30 2f22 202f 3e0a 2020  c-sa/4.0/" />.  
-00004dc0: 2020 2020 2020 3c64 633a 6465 7363 7269        <dc:descri
-00004dd0: 7074 696f 6e3e 5369 676e 616c 797a 6572  ption>Signalyzer
-00004de0: 204c 6f67 6f3c 2f64 633a 6465 7363 7269   Logo</dc:descri
-00004df0: 7074 696f 6e3e 0a20 2020 2020 2020 203c  ption>.        <
-00004e00: 6463 3a72 6967 6874 733e 0a20 2020 2020  dc:rights>.     
-00004e10: 2020 2020 203c 6363 3a41 6765 6e74 3e0a       <cc:Agent>.
-00004e20: 2020 2020 2020 2020 2020 2020 3c64 633a              <dc:
-00004e30: 7469 746c 653e 416c 6c20 5269 6768 7473  title>All Rights
-00004e40: 2072 6573 6572 7665 642e 3c2f 6463 3a74   reserved.</dc:t
-00004e50: 6974 6c65 3e0a 2020 2020 2020 2020 2020  itle>.          
-00004e60: 3c2f 6363 3a41 6765 6e74 3e0a 2020 2020  </cc:Agent>.    
-00004e70: 2020 2020 3c2f 6463 3a72 6967 6874 733e      </dc:rights>
-00004e80: 0a20 2020 2020 203c 2f63 633a 576f 726b  .      </cc:Work
-00004e90: 3e0a 2020 2020 2020 3c63 633a 4c69 6365  >.      <cc:Lice
-00004ea0: 6e73 650a 2020 2020 2020 2020 2072 6466  nse.         rdf
-00004eb0: 3a61 626f 7574 3d22 6874 7470 3a2f 2f63  :about="http://c
-00004ec0: 7265 6174 6976 6563 6f6d 6d6f 6e73 2e6f  reativecommons.o
-00004ed0: 7267 2f6c 6963 656e 7365 732f 6279 2d6e  rg/licenses/by-n
-00004ee0: 632d 7361 2f34 2e30 2f22 3e0a 2020 2020  c-sa/4.0/">.    
-00004ef0: 2020 2020 3c63 633a 7065 726d 6974 730a      <cc:permits.
-00004f00: 2020 2020 2020 2020 2020 2072 6466 3a72             rdf:r
-00004f10: 6573 6f75 7263 653d 2268 7474 703a 2f2f  esource="http://
-00004f20: 6372 6561 7469 7665 636f 6d6d 6f6e 732e  creativecommons.
-00004f30: 6f72 672f 6e73 2352 6570 726f 6475 6374  org/ns#Reproduct
-00004f40: 696f 6e22 202f 3e0a 2020 2020 2020 2020  ion" />.        
-00004f50: 3c63 633a 7065 726d 6974 730a 2020 2020  <cc:permits.    
-00004f60: 2020 2020 2020 2072 6466 3a72 6573 6f75         rdf:resou
-00004f70: 7263 653d 2268 7474 703a 2f2f 6372 6561  rce="http://crea
-00004f80: 7469 7665 636f 6d6d 6f6e 732e 6f72 672f  tivecommons.org/
-00004f90: 6e73 2344 6973 7472 6962 7574 696f 6e22  ns#Distribution"
-00004fa0: 202f 3e0a 2020 2020 2020 2020 3c63 633a   />.        <cc:
-00004fb0: 7265 7175 6972 6573 0a20 2020 2020 2020  requires.       
-00004fc0: 2020 2020 7264 663a 7265 736f 7572 6365      rdf:resource
-00004fd0: 3d22 6874 7470 3a2f 2f63 7265 6174 6976  ="http://creativ
-00004fe0: 6563 6f6d 6d6f 6e73 2e6f 7267 2f6e 7323  ecommons.org/ns#
-00004ff0: 4e6f 7469 6365 2220 2f3e 0a20 2020 2020  Notice" />.     
-00005000: 2020 203c 6363 3a72 6571 7569 7265 730a     <cc:requires.
-00005010: 2020 2020 2020 2020 2020 2072 6466 3a72             rdf:r
-00005020: 6573 6f75 7263 653d 2268 7474 703a 2f2f  esource="http://
-00005030: 6372 6561 7469 7665 636f 6d6d 6f6e 732e  creativecommons.
-00005040: 6f72 672f 6e73 2341 7474 7269 6275 7469  org/ns#Attributi
-00005050: 6f6e 2220 2f3e 0a20 2020 2020 2020 203c  on" />.        <
-00005060: 6363 3a70 726f 6869 6269 7473 0a20 2020  cc:prohibits.   
-00005070: 2020 2020 2020 2020 7264 663a 7265 736f          rdf:reso
-00005080: 7572 6365 3d22 6874 7470 3a2f 2f63 7265  urce="http://cre
-00005090: 6174 6976 6563 6f6d 6d6f 6e73 2e6f 7267  ativecommons.org
-000050a0: 2f6e 7323 436f 6d6d 6572 6369 616c 5573  /ns#CommercialUs
-000050b0: 6522 202f 3e0a 2020 2020 2020 2020 3c63  e" />.        <c
-000050c0: 633a 7065 726d 6974 730a 2020 2020 2020  c:permits.      
-000050d0: 2020 2020 2072 6466 3a72 6573 6f75 7263       rdf:resourc
-000050e0: 653d 2268 7474 703a 2f2f 6372 6561 7469  e="http://creati
-000050f0: 7665 636f 6d6d 6f6e 732e 6f72 672f 6e73  vecommons.org/ns
-00005100: 2344 6572 6976 6174 6976 6557 6f72 6b73  #DerivativeWorks
-00005110: 2220 2f3e 0a20 2020 2020 2020 203c 6363  " />.        <cc
-00005120: 3a72 6571 7569 7265 730a 2020 2020 2020  :requires.      
-00005130: 2020 2020 2072 6466 3a72 6573 6f75 7263       rdf:resourc
-00005140: 653d 2268 7474 703a 2f2f 6372 6561 7469  e="http://creati
-00005150: 7665 636f 6d6d 6f6e 732e 6f72 672f 6e73  vecommons.org/ns
-00005160: 2353 6861 7265 416c 696b 6522 202f 3e0a  #ShareAlike" />.
-00005170: 2020 2020 2020 3c2f 6363 3a4c 6963 656e        </cc:Licen
-00005180: 7365 3e0a 2020 2020 3c2f 7264 663a 5244  se>.    </rdf:RD
-00005190: 463e 0a20 203c 2f6d 6574 6164 6174 613e  F>.  </metadata>
-000051a0: 0a20 203c 670a 2020 2020 2069 6e6b 7363  .  <g.     inksc
-000051b0: 6170 653a 6772 6f75 706d 6f64 653d 226c  ape:groupmode="l
-000051c0: 6179 6572 220a 2020 2020 2069 643d 226c  ayer".     id="l
-000051d0: 6179 6572 3422 0a20 2020 2020 696e 6b73  ayer4".     inks
-000051e0: 6361 7065 3a6c 6162 656c 3d22 5465 7874  cape:label="Text
-000051f0: 220a 2020 2020 2073 6f64 6970 6f64 693a  ".     sodipodi:
-00005200: 696e 7365 6e73 6974 6976 653d 2274 7275  insensitive="tru
-00005210: 6522 0a20 2020 2020 7374 796c 653d 2264  e".     style="d
-00005220: 6973 706c 6179 3a69 6e6c 696e 6522 3e0a  isplay:inline">.
-00005230: 2020 2020 3c74 6578 740a 2020 2020 2020      <text.      
-00005240: 2078 6d6c 3a73 7061 6365 3d22 7072 6573   xml:space="pres
-00005250: 6572 7665 220a 2020 2020 2020 2073 7479  erve".       sty
-00005260: 6c65 3d22 666f 6e74 2d73 7479 6c65 3a6e  le="font-style:n
-00005270: 6f72 6d61 6c3b 666f 6e74 2d76 6172 6961  ormal;font-varia
-00005280: 6e74 3a6e 6f72 6d61 6c3b 666f 6e74 2d77  nt:normal;font-w
-00005290: 6569 6768 743a 626f 6c64 3b66 6f6e 742d  eight:bold;font-
-000052a0: 7374 7265 7463 683a 6e6f 726d 616c 3b66  stretch:normal;f
-000052b0: 6f6e 742d 7369 7a65 3a34 2e39 3338 3839  ont-size:4.93889
-000052c0: 7078 3b6c 696e 652d 6865 6967 6874 3a31  px;line-height:1
-000052d0: 2e32 353b 666f 6e74 2d66 616d 696c 793a  .25;font-family:
-000052e0: 7361 6e73 2d73 6572 6966 3b2d 696e 6b73  sans-serif;-inks
-000052f0: 6361 7065 2d66 6f6e 742d 7370 6563 6966  cape-font-specif
-00005300: 6963 6174 696f 6e3a 2773 616e 732d 7365  ication:'sans-se
-00005310: 7269 6620 426f 6c64 273b 7465 7874 2d61  rif Bold';text-a
-00005320: 6c69 676e 3a63 656e 7465 723b 7465 7874  lign:center;text
-00005330: 2d61 6e63 686f 723a 6d69 6464 6c65 3b66  -anchor:middle;f
-00005340: 696c 6c3a 2330 3934 6261 633b 7374 726f  ill:#094bac;stro
-00005350: 6b65 2d77 6964 7468 3a30 2e32 3634 3538  ke-width:0.26458
-00005360: 3322 0a20 2020 2020 2020 783d 2231 322e  3".       x="12.
-00005370: 3439 3531 3736 220a 2020 2020 2020 2079  495176".       y
-00005380: 3d22 3436 2e39 3537 3538 3422 0a20 2020  ="46.957584".   
-00005390: 2020 2020 6964 3d22 7465 7874 3839 3736      id="text8976
-000053a0: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
-000053b0: 653a 6c61 6265 6c3d 2241 6e61 6c79 7a65  e:label="Analyze
-000053c0: 7222 0a20 2020 2020 2020 736f 6469 706f  r".       sodipo
-000053d0: 6469 3a69 6e73 656e 7369 7469 7665 3d22  di:insensitive="
-000053e0: 7472 7565 223e 3c74 7370 616e 0a20 2020  true"><tspan.   
-000053f0: 2020 2020 2020 736f 6469 706f 6469 3a72        sodipodi:r
-00005400: 6f6c 653d 226c 696e 6522 0a20 2020 2020  ole="line".     
-00005410: 2020 2020 7374 796c 653d 2266 6f6e 742d      style="font-
-00005420: 7374 796c 653a 6e6f 726d 616c 3b66 6f6e  style:normal;fon
-00005430: 742d 7661 7269 616e 743a 6e6f 726d 616c  t-variant:normal
-00005440: 3b66 6f6e 742d 7765 6967 6874 3a62 6f6c  ;font-weight:bol
-00005450: 643b 666f 6e74 2d73 7472 6574 6368 3a6e  d;font-stretch:n
-00005460: 6f72 6d61 6c3b 666f 6e74 2d73 697a 653a  ormal;font-size:
-00005470: 342e 3933 3838 3970 783b 666f 6e74 2d66  4.93889px;font-f
-00005480: 616d 696c 793a 7361 6e73 2d73 6572 6966  amily:sans-serif
-00005490: 3b2d 696e 6b73 6361 7065 2d66 6f6e 742d  ;-inkscape-font-
-000054a0: 7370 6563 6966 6963 6174 696f 6e3a 2773  specification:'s
-000054b0: 616e 732d 7365 7269 6620 426f 6c64 273b  ans-serif Bold';
-000054c0: 7465 7874 2d61 6c69 676e 3a63 656e 7465  text-align:cente
-000054d0: 723b 7465 7874 2d61 6e63 686f 723a 6d69  r;text-anchor:mi
-000054e0: 6464 6c65 3b66 696c 6c3a 2330 3934 6261  ddle;fill:#094ba
-000054f0: 633b 7374 726f 6b65 2d77 6964 7468 3a30  c;stroke-width:0
-00005500: 2e32 3634 3538 3322 0a20 2020 2020 2020  .264583".       
-00005510: 2020 783d 2231 322e 3439 3531 3736 220a    x="12.495176".
-00005520: 2020 2020 2020 2020 2079 3d22 3436 2e39           y="46.9
-00005530: 3537 3538 3422 0a20 2020 2020 2020 2020  57584".         
-00005540: 6964 3d22 7473 7061 6e31 3132 3536 223e  id="tspan11256">
-00005550: 416e 616c 797a 6572 3c2f 7473 7061 6e3e  Analyzer</tspan>
-00005560: 3c2f 7465 7874 3e0a 2020 2020 3c74 6578  </text>.    <tex
-00005570: 740a 2020 2020 2020 2078 6d6c 3a73 7061  t.       xml:spa
-00005580: 6365 3d22 7072 6573 6572 7665 220a 2020  ce="preserve".  
-00005590: 2020 2020 2073 7479 6c65 3d22 666f 6e74       style="font
-000055a0: 2d73 697a 653a 342e 3933 3838 3970 783b  -size:4.93889px;
-000055b0: 6c69 6e65 2d68 6569 6768 743a 312e 3235  line-height:1.25
-000055c0: 3b66 6f6e 742d 6661 6d69 6c79 3a73 616e  ;font-family:san
-000055d0: 732d 7365 7269 663b 2d69 6e6b 7363 6170  s-serif;-inkscap
-000055e0: 652d 666f 6e74 2d73 7065 6369 6669 6361  e-font-specifica
-000055f0: 7469 6f6e 3a27 7361 6e73 2d73 6572 6966  tion:'sans-serif
-00005600: 2c20 4e6f 726d 616c 273b 6669 6c6c 3a23  , Normal';fill:#
-00005610: 3039 3462 6163 3b73 7472 6f6b 652d 7769  094bac;stroke-wi
-00005620: 6474 683a 302e 3236 3435 3833 220a 2020  dth:0.264583".  
-00005630: 2020 2020 2078 3d22 3337 2e35 3330 3134       x="37.53014
-00005640: 3422 0a20 2020 2020 2020 793d 2235 2e37  4".       y="5.7
-00005650: 3238 3930 3632 220a 2020 2020 2020 2069  289062".       i
-00005660: 643d 2274 6578 7432 3834 3722 0a20 2020  d="text2847".   
-00005670: 2020 2020 696e 6b73 6361 7065 3a6c 6162      inkscape:lab
-00005680: 656c 3d22 5369 676e 616c 220a 2020 2020  el="Signal".    
-00005690: 2020 2073 6f64 6970 6f64 693a 696e 7365     sodipodi:inse
-000056a0: 6e73 6974 6976 653d 2274 7275 6522 3e3c  nsitive="true"><
-000056b0: 7473 7061 6e0a 2020 2020 2020 2020 2073  tspan.         s
-000056c0: 6f64 6970 6f64 693a 726f 6c65 3d22 6c69  odipodi:role="li
-000056d0: 6e65 220a 2020 2020 2020 2020 2069 643d  ne".         id=
-000056e0: 2274 7370 616e 3238 3435 220a 2020 2020  "tspan2845".    
-000056f0: 2020 2020 2073 7479 6c65 3d22 666f 6e74       style="font
-00005700: 2d73 7479 6c65 3a6e 6f72 6d61 6c3b 666f  -style:normal;fo
-00005710: 6e74 2d76 6172 6961 6e74 3a6e 6f72 6d61  nt-variant:norma
-00005720: 6c3b 666f 6e74 2d77 6569 6768 743a 626f  l;font-weight:bo
-00005730: 6c64 3b66 6f6e 742d 7374 7265 7463 683a  ld;font-stretch:
-00005740: 6e6f 726d 616c 3b66 6f6e 742d 7369 7a65  normal;font-size
-00005750: 3a34 2e39 3338 3839 7078 3b66 6f6e 742d  :4.93889px;font-
-00005760: 6661 6d69 6c79 3a73 616e 732d 7365 7269  family:sans-seri
-00005770: 663b 2d69 6e6b 7363 6170 652d 666f 6e74  f;-inkscape-font
-00005780: 2d73 7065 6369 6669 6361 7469 6f6e 3a27  -specification:'
-00005790: 7361 6e73 2d73 6572 6966 2042 6f6c 6427  sans-serif Bold'
-000057a0: 3b74 6578 742d 616c 6967 6e3a 6365 6e74  ;text-align:cent
-000057b0: 6572 3b74 6578 742d 616e 6368 6f72 3a6d  er;text-anchor:m
-000057c0: 6964 646c 653b 6669 6c6c 3a23 3039 3462  iddle;fill:#094b
-000057d0: 6163 3b73 7472 6f6b 652d 7769 6474 683a  ac;stroke-width:
-000057e0: 302e 3236 3435 3833 220a 2020 2020 2020  0.264583".      
-000057f0: 2020 2078 3d22 3337 2e35 3330 3134 3422     x="37.530144"
-00005800: 0a20 2020 2020 2020 2020 793d 2235 2e37  .         y="5.7
-00005810: 3238 3930 3632 223e 5369 676e 616c 3c2f  289062">Signal</
-00005820: 7473 7061 6e3e 3c2f 7465 7874 3e0a 2020  tspan></text>.  
-00005830: 3c2f 673e 0a3c 2f73 7667 3e0a            </g>.</svg>.
+00000080: 2231 3630 6d6d 220a 2020 2068 6569 6768  "160mm".   heigh
+00000090: 743d 2235 306d 6d22 0a20 2020 7669 6577  t="50mm".   view
+000000a0: 426f 783d 2230 2030 2031 3630 2035 3022  Box="0 0 160 50"
+000000b0: 0a20 2020 7665 7273 696f 6e3d 2231 2e31  .   version="1.1
+000000c0: 220a 2020 2069 643d 2273 7667 3932 3222  ".   id="svg922"
+000000d0: 0a20 2020 696e 6b73 6361 7065 3a76 6572  .   inkscape:ver
+000000e0: 7369 6f6e 3d22 312e 312e 3120 2833 6266  sion="1.1.1 (3bf
+000000f0: 3561 6530 6432 352c 2032 3032 312d 3039  5ae0d25, 2021-09
+00000100: 2d32 3029 220a 2020 2073 6f64 6970 6f64  -20)".   sodipod
+00000110: 693a 646f 636e 616d 653d 2273 6967 6e61  i:docname="signa
+00000120: 6c79 7a65 722e 7376 6722 0a20 2020 696e  lyzer.svg".   in
+00000130: 6b73 6361 7065 3a65 7870 6f72 742d 6669  kscape:export-fi
+00000140: 6c65 6e61 6d65 3d22 443a 5c57 6f72 6b73  lename="D:\Works
+00000150: 7061 6365 5c44 7261 7769 6e67 735c 6261  pace\Drawings\ba
+00000160: 6e6e 6572 2e70 6e67 220a 2020 2069 6e6b  nner.png".   ink
+00000170: 7363 6170 653a 6578 706f 7274 2d78 6470  scape:export-xdp
+00000180: 693d 2231 3031 2e36 220a 2020 2069 6e6b  i="101.6".   ink
+00000190: 7363 6170 653a 6578 706f 7274 2d79 6470  scape:export-ydp
+000001a0: 693d 2231 3031 2e36 220a 2020 2078 6d6c  i="101.6".   xml
+000001b0: 6e73 3a69 6e6b 7363 6170 653d 2268 7474  ns:inkscape="htt
+000001c0: 703a 2f2f 7777 772e 696e 6b73 6361 7065  p://www.inkscape
+000001d0: 2e6f 7267 2f6e 616d 6573 7061 6365 732f  .org/namespaces/
+000001e0: 696e 6b73 6361 7065 220a 2020 2078 6d6c  inkscape".   xml
+000001f0: 6e73 3a73 6f64 6970 6f64 693d 2268 7474  ns:sodipodi="htt
+00000200: 703a 2f2f 736f 6469 706f 6469 2e73 6f75  p://sodipodi.sou
+00000210: 7263 6566 6f72 6765 2e6e 6574 2f44 5444  rceforge.net/DTD
+00000220: 2f73 6f64 6970 6f64 692d 302e 6474 6422  /sodipodi-0.dtd"
+00000230: 0a20 2020 786d 6c6e 733d 2268 7474 703a  .   xmlns="http:
+00000240: 2f2f 7777 772e 7733 2e6f 7267 2f32 3030  //www.w3.org/200
+00000250: 302f 7376 6722 0a20 2020 786d 6c6e 733a  0/svg".   xmlns:
+00000260: 7376 673d 2268 7474 703a 2f2f 7777 772e  svg="http://www.
+00000270: 7733 2e6f 7267 2f32 3030 302f 7376 6722  w3.org/2000/svg"
+00000280: 0a20 2020 786d 6c6e 733a 7264 663d 2268  .   xmlns:rdf="h
+00000290: 7474 703a 2f2f 7777 772e 7733 2e6f 7267  ttp://www.w3.org
+000002a0: 2f31 3939 392f 3032 2f32 322d 7264 662d  /1999/02/22-rdf-
+000002b0: 7379 6e74 6178 2d6e 7323 220a 2020 2078  syntax-ns#".   x
+000002c0: 6d6c 6e73 3a63 633d 2268 7474 703a 2f2f  mlns:cc="http://
+000002d0: 6372 6561 7469 7665 636f 6d6d 6f6e 732e  creativecommons.
+000002e0: 6f72 672f 6e73 2322 0a20 2020 786d 6c6e  org/ns#".   xmln
+000002f0: 733a 6463 3d22 6874 7470 3a2f 2f70 7572  s:dc="http://pur
+00000300: 6c2e 6f72 672f 6463 2f65 6c65 6d65 6e74  l.org/dc/element
+00000310: 732f 312e 312f 223e 0a20 203c 7469 746c  s/1.1/">.  <titl
+00000320: 650a 2020 2020 2069 643d 2274 6974 6c65  e.     id="title
+00000330: 3930 3122 3e53 6967 6e61 6c79 7a65 7220  901">Signalyzer 
+00000340: 4261 6e6e 6572 3c2f 7469 746c 653e 0a20  Banner</title>. 
+00000350: 203c 736f 6469 706f 6469 3a6e 616d 6564   <sodipodi:named
+00000360: 7669 6577 0a20 2020 2020 6964 3d22 6e61  view.     id="na
+00000370: 6d65 6476 6965 7739 3234 220a 2020 2020  medview924".    
+00000380: 2070 6167 6563 6f6c 6f72 3d22 2366 6666   pagecolor="#fff
+00000390: 6666 6622 0a20 2020 2020 626f 7264 6572  fff".     border
+000003a0: 636f 6c6f 723d 2223 3939 3939 3939 220a  color="#999999".
+000003b0: 2020 2020 2062 6f72 6465 726f 7061 6369       borderopaci
+000003c0: 7479 3d22 3122 0a20 2020 2020 696e 6b73  ty="1".     inks
+000003d0: 6361 7065 3a70 6167 6573 6861 646f 773d  cape:pageshadow=
+000003e0: 2230 220a 2020 2020 2069 6e6b 7363 6170  "0".     inkscap
+000003f0: 653a 7061 6765 6f70 6163 6974 793d 2230  e:pageopacity="0
+00000400: 220a 2020 2020 2069 6e6b 7363 6170 653a  ".     inkscape:
+00000410: 7061 6765 6368 6563 6b65 7262 6f61 7264  pagecheckerboard
+00000420: 3d22 3022 0a20 2020 2020 696e 6b73 6361  ="0".     inksca
+00000430: 7065 3a64 6f63 756d 656e 742d 756e 6974  pe:document-unit
+00000440: 733d 226d 6d22 0a20 2020 2020 7368 6f77  s="mm".     show
+00000450: 6772 6964 3d22 7472 7565 220a 2020 2020  grid="true".    
+00000460: 2073 686f 7767 7569 6465 733d 2274 7275   showguides="tru
+00000470: 6522 0a20 2020 2020 696e 6b73 6361 7065  e".     inkscape
+00000480: 3a67 7569 6465 2d62 626f 783d 2274 7275  :guide-bbox="tru
+00000490: 6522 0a20 2020 2020 696e 6b73 6361 7065  e".     inkscape
+000004a0: 3a7a 6f6f 6d3d 2232 2e38 3238 3432 3731  :zoom="2.8284271
+000004b0: 220a 2020 2020 2069 6e6b 7363 6170 653a  ".     inkscape:
+000004c0: 6378 3d22 3236 322e 3836 3639 3522 0a20  cx="262.86695". 
+000004d0: 2020 2020 696e 6b73 6361 7065 3a63 793d      inkscape:cy=
+000004e0: 2231 382e 3230 3822 0a20 2020 2020 696e  "18.208".     in
+000004f0: 6b73 6361 7065 3a77 696e 646f 772d 7769  kscape:window-wi
+00000500: 6474 683d 2232 3536 3022 0a20 2020 2020  dth="2560".     
+00000510: 696e 6b73 6361 7065 3a77 696e 646f 772d  inkscape:window-
+00000520: 6865 6967 6874 3d22 3133 3631 220a 2020  height="1361".  
+00000530: 2020 2069 6e6b 7363 6170 653a 7769 6e64     inkscape:wind
+00000540: 6f77 2d78 3d22 2d39 220a 2020 2020 2069  ow-x="-9".     i
+00000550: 6e6b 7363 6170 653a 7769 6e64 6f77 2d79  nkscape:window-y
+00000560: 3d22 2d39 220a 2020 2020 2069 6e6b 7363  ="-9".     inksc
+00000570: 6170 653a 7769 6e64 6f77 2d6d 6178 696d  ape:window-maxim
+00000580: 697a 6564 3d22 3122 0a20 2020 2020 696e  ized="1".     in
+00000590: 6b73 6361 7065 3a63 7572 7265 6e74 2d6c  kscape:current-l
+000005a0: 6179 6572 3d22 6c61 7965 7232 2d36 220a  ayer="layer2-6".
+000005b0: 2020 2020 2069 6e6b 7363 6170 653a 6c6f       inkscape:lo
+000005c0: 636b 6775 6964 6573 3d22 6661 6c73 6522  ckguides="false"
+000005d0: 0a20 2020 2020 696e 6b73 6361 7065 3a6f  .     inkscape:o
+000005e0: 626a 6563 742d 7061 7468 733d 2274 7275  bject-paths="tru
+000005f0: 6522 0a20 2020 2020 696e 6b73 6361 7065  e".     inkscape
+00000600: 3a73 6e61 702d 696e 7465 7273 6563 7469  :snap-intersecti
+00000610: 6f6e 2d70 6174 6873 3d22 7472 7565 220a  on-paths="true".
+00000620: 2020 2020 2069 6e6b 7363 6170 653a 736e       inkscape:sn
+00000630: 6170 2d73 6d6f 6f74 682d 6e6f 6465 733d  ap-smooth-nodes=
+00000640: 2274 7275 6522 0a20 2020 2020 696e 6b73  "true".     inks
+00000650: 6361 7065 3a73 6e61 702d 6d69 6470 6f69  cape:snap-midpoi
+00000660: 6e74 733d 2274 7275 6522 0a20 2020 2020  nts="true".     
+00000670: 696e 6b73 6361 7065 3a73 6e61 702d 6f62  inkscape:snap-ob
+00000680: 6a65 6374 2d6d 6964 706f 696e 7473 3d22  ject-midpoints="
+00000690: 7472 7565 220a 2020 2020 2069 6e6b 7363  true".     inksc
+000006a0: 6170 653a 736e 6170 2d63 656e 7465 723d  ape:snap-center=
+000006b0: 2274 7275 6522 0a20 2020 2020 696e 6b73  "true".     inks
+000006c0: 6361 7065 3a73 6e61 702d 6262 6f78 3d22  cape:snap-bbox="
+000006d0: 7472 7565 220a 2020 2020 2069 6e6b 7363  true".     inksc
+000006e0: 6170 653a 6262 6f78 2d70 6174 6873 3d22  ape:bbox-paths="
+000006f0: 7472 7565 220a 2020 2020 2069 6e6b 7363  true".     inksc
+00000700: 6170 653a 6262 6f78 2d6e 6f64 6573 3d22  ape:bbox-nodes="
+00000710: 7472 7565 220a 2020 2020 2069 6e6b 7363  true".     inksc
+00000720: 6170 653a 736e 6170 2d62 626f 782d 6564  ape:snap-bbox-ed
+00000730: 6765 2d6d 6964 706f 696e 7473 3d22 7472  ge-midpoints="tr
+00000740: 7565 220a 2020 2020 2069 6e6b 7363 6170  ue".     inkscap
+00000750: 653a 736e 6170 2d62 626f 782d 6d69 6470  e:snap-bbox-midp
+00000760: 6f69 6e74 733d 2266 616c 7365 220a 2020  oints="false".  
+00000770: 2020 2069 6e6b 7363 6170 653a 736e 6170     inkscape:snap
+00000780: 2d67 7269 6473 3d22 7472 7565 220a 2020  -grids="true".  
+00000790: 2020 2069 6e6b 7363 6170 653a 736e 6170     inkscape:snap
+000007a0: 2d67 6c6f 6261 6c3d 2274 7275 6522 0a20  -global="true". 
+000007b0: 2020 2020 696e 6b73 6361 7065 3a73 6e61      inkscape:sna
+000007c0: 702d 6e6f 6465 733d 2274 7275 6522 0a20  p-nodes="true". 
+000007d0: 2020 2020 696e 6b73 6361 7065 3a73 6e61      inkscape:sna
+000007e0: 702d 6f74 6865 7273 3d22 7472 7565 220a  p-others="true".
+000007f0: 2020 2020 2069 6e6b 7363 6170 653a 736e       inkscape:sn
+00000800: 6170 2d74 6f2d 6775 6964 6573 3d22 7472  ap-to-guides="tr
+00000810: 7565 220a 2020 2020 2069 6e6b 7363 6170  ue".     inkscap
+00000820: 653a 736e 6170 2d70 6167 653d 2274 7275  e:snap-page="tru
+00000830: 6522 202f 3e0a 2020 3c64 6566 730a 2020  e" />.  <defs.  
+00000840: 2020 2069 643d 2264 6566 7339 3139 223e     id="defs919">
+00000850: 0a20 2020 203c 6d61 726b 6572 0a20 2020  .    <marker.   
+00000860: 2020 2020 7374 796c 653d 226f 7665 7266      style="overf
+00000870: 6c6f 773a 7669 7369 626c 6522 0a20 2020  low:visible".   
+00000880: 2020 2020 6964 3d22 4172 726f 7731 4c65      id="Arrow1Le
+00000890: 6e64 220a 2020 2020 2020 2072 6566 583d  nd".       refX=
+000008a0: 2230 220a 2020 2020 2020 2072 6566 593d  "0".       refY=
+000008b0: 2230 220a 2020 2020 2020 206f 7269 656e  "0".       orien
+000008c0: 743d 2261 7574 6f22 0a20 2020 2020 2020  t="auto".       
+000008d0: 696e 6b73 6361 7065 3a73 746f 636b 6964  inkscape:stockid
+000008e0: 3d22 4172 726f 7731 4c65 6e64 220a 2020  ="Arrow1Lend".  
+000008f0: 2020 2020 2069 6e6b 7363 6170 653a 6973       inkscape:is
+00000900: 7374 6f63 6b3d 2274 7275 6522 3e0a 2020  stock="true">.  
+00000910: 2020 2020 3c70 6174 680a 2020 2020 2020      <path.      
+00000920: 2020 2074 7261 6e73 666f 726d 3d22 6d61     transform="ma
+00000930: 7472 6978 282d 302e 382c 302c 302c 2d30  trix(-0.8,0,0,-0
+00000940: 2e38 2c2d 3130 2c30 2922 0a20 2020 2020  .8,-10,0)".     
+00000950: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
+00000960: 636f 6e74 6578 742d 7374 726f 6b65 3b66  context-stroke;f
+00000970: 696c 6c2d 7275 6c65 3a65 7665 6e6f 6464  ill-rule:evenodd
+00000980: 3b73 7472 6f6b 653a 636f 6e74 6578 742d  ;stroke:context-
+00000990: 7374 726f 6b65 3b73 7472 6f6b 652d 7769  stroke;stroke-wi
+000009a0: 6474 683a 3170 7422 0a20 2020 2020 2020  dth:1pt".       
+000009b0: 2020 643d 224d 2030 2c30 2035 2c2d 3520    d="M 0,0 5,-5 
+000009c0: 2d31 322e 352c 3020 352c 3520 5a22 0a20  -12.5,0 5,5 Z". 
+000009d0: 2020 2020 2020 2020 6964 3d22 7061 7468          id="path
+000009e0: 3836 3622 202f 3e0a 2020 2020 3c2f 6d61  866" />.    </ma
+000009f0: 726b 6572 3e0a 2020 2020 3c6d 6172 6b65  rker>.    <marke
+00000a00: 720a 2020 2020 2020 2073 7479 6c65 3d22  r.       style="
+00000a10: 6f76 6572 666c 6f77 3a76 6973 6962 6c65  overflow:visible
+00000a20: 220a 2020 2020 2020 2069 643d 2241 7272  ".       id="Arr
+00000a30: 6f77 324c 656e 6422 0a20 2020 2020 2020  ow2Lend".       
+00000a40: 7265 6658 3d22 3022 0a20 2020 2020 2020  refX="0".       
+00000a50: 7265 6659 3d22 3022 0a20 2020 2020 2020  refY="0".       
+00000a60: 6f72 6965 6e74 3d22 6175 746f 220a 2020  orient="auto".  
+00000a70: 2020 2020 2069 6e6b 7363 6170 653a 7374       inkscape:st
+00000a80: 6f63 6b69 643d 2241 7272 6f77 324c 656e  ockid="Arrow2Len
+00000a90: 6422 0a20 2020 2020 2020 696e 6b73 6361  d".       inksca
+00000aa0: 7065 3a69 7373 746f 636b 3d22 7472 7565  pe:isstock="true
+00000ab0: 223e 0a20 2020 2020 203c 7061 7468 0a20  ">.      <path. 
+00000ac0: 2020 2020 2020 2020 7472 616e 7366 6f72          transfor
+00000ad0: 6d3d 226d 6174 7269 7828 2d31 2e31 2c30  m="matrix(-1.1,0
+00000ae0: 2c30 2c2d 312e 312c 2d31 2e31 2c30 2922  ,0,-1.1,-1.1,0)"
+00000af0: 0a20 2020 2020 2020 2020 643d 224d 2038  .         d="M 8
+00000b00: 2e37 3138 3538 3738 2c34 2e30 3333 3733  .7185878,4.03373
+00000b10: 3532 202d 322e 3230 3732 3839 352c 302e  52 -2.2072895,0.
+00000b20: 3031 3630 3133 3236 2038 2e37 3138 3538  01601326 8.71858
+00000b30: 3834 2c2d 342e 3030 3137 3037 3820 6320  84,-4.0017078 c 
+00000b40: 2d31 2e37 3435 3439 3834 2c32 2e33 3732  -1.7454984,2.372
+00000b50: 3036 3039 202d 312e 3733 3534 3430 382c  0609 -1.7354408,
+00000b60: 352e 3631 3734 3531 3920 2d36 652d 372c  5.6174519 -6e-7,
+00000b70: 382e 3033 3534 3433 207a 220a 2020 2020  8.035443 z".    
+00000b80: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
+00000b90: 3a63 6f6e 7465 7874 2d73 7472 6f6b 653b  :context-stroke;
+00000ba0: 6669 6c6c 2d72 756c 653a 6576 656e 6f64  fill-rule:evenod
+00000bb0: 643b 7374 726f 6b65 3a63 6f6e 7465 7874  d;stroke:context
+00000bc0: 2d73 7472 6f6b 653b 7374 726f 6b65 2d77  -stroke;stroke-w
+00000bd0: 6964 7468 3a30 2e36 3235 3b73 7472 6f6b  idth:0.625;strok
+00000be0: 652d 6c69 6e65 6a6f 696e 3a72 6f75 6e64  e-linejoin:round
+00000bf0: 220a 2020 2020 2020 2020 2069 643d 2270  ".         id="p
+00000c00: 6174 6838 3834 2220 2f3e 0a20 2020 203c  ath884" />.    <
+00000c10: 2f6d 6172 6b65 723e 0a20 2020 203c 6d61  /marker>.    <ma
+00000c20: 726b 6572 0a20 2020 2020 2020 7374 796c  rker.       styl
+00000c30: 653d 226f 7665 7266 6c6f 773a 7669 7369  e="overflow:visi
+00000c40: 626c 6522 0a20 2020 2020 2020 6964 3d22  ble".       id="
+00000c50: 4172 726f 7731 4c65 6e64 2d36 220a 2020  Arrow1Lend-6".  
+00000c60: 2020 2020 2072 6566 583d 2230 220a 2020       refX="0".  
+00000c70: 2020 2020 2072 6566 593d 2230 220a 2020       refY="0".  
+00000c80: 2020 2020 206f 7269 656e 743d 2261 7574       orient="aut
+00000c90: 6f22 0a20 2020 2020 2020 696e 6b73 6361  o".       inksca
+00000ca0: 7065 3a73 746f 636b 6964 3d22 4172 726f  pe:stockid="Arro
+00000cb0: 7731 4c65 6e64 220a 2020 2020 2020 2069  w1Lend".       i
+00000cc0: 6e6b 7363 6170 653a 6973 7374 6f63 6b3d  nkscape:isstock=
+00000cd0: 2274 7275 6522 3e0a 2020 2020 2020 3c70  "true">.      <p
+00000ce0: 6174 680a 2020 2020 2020 2020 2074 7261  ath.         tra
+00000cf0: 6e73 666f 726d 3d22 6d61 7472 6978 282d  nsform="matrix(-
+00000d00: 302e 382c 302c 302c 2d30 2e38 2c2d 3130  0.8,0,0,-0.8,-10
+00000d10: 2c30 2922 0a20 2020 2020 2020 2020 7374  ,0)".         st
+00000d20: 796c 653d 2266 696c 6c3a 636f 6e74 6578  yle="fill:contex
+00000d30: 742d 7374 726f 6b65 3b66 696c 6c2d 7275  t-stroke;fill-ru
+00000d40: 6c65 3a65 7665 6e6f 6464 3b73 7472 6f6b  le:evenodd;strok
+00000d50: 653a 636f 6e74 6578 742d 7374 726f 6b65  e:context-stroke
+00000d60: 3b73 7472 6f6b 652d 7769 6474 683a 3170  ;stroke-width:1p
+00000d70: 7422 0a20 2020 2020 2020 2020 643d 224d  t".         d="M
+00000d80: 2030 2c30 2035 2c2d 3520 2d31 322e 352c   0,0 5,-5 -12.5,
+00000d90: 3020 352c 3520 5a22 0a20 2020 2020 2020  0 5,5 Z".       
+00000da0: 2020 6964 3d22 7061 7468 3830 3934 2220    id="path8094" 
+00000db0: 2f3e 0a20 2020 203c 2f6d 6172 6b65 723e  />.    </marker>
+00000dc0: 0a20 2020 203c 6d61 726b 6572 0a20 2020  .    <marker.   
+00000dd0: 2020 2020 7374 796c 653d 226f 7665 7266      style="overf
+00000de0: 6c6f 773a 7669 7369 626c 6522 0a20 2020  low:visible".   
+00000df0: 2020 2020 6964 3d22 6d61 726b 6572 3131      id="marker11
+00000e00: 3333 220a 2020 2020 2020 2072 6566 583d  33".       refX=
+00000e10: 2230 220a 2020 2020 2020 2072 6566 593d  "0".       refY=
+00000e20: 2230 220a 2020 2020 2020 206f 7269 656e  "0".       orien
+00000e30: 743d 2261 7574 6f22 0a20 2020 2020 2020  t="auto".       
+00000e40: 696e 6b73 6361 7065 3a73 746f 636b 6964  inkscape:stockid
+00000e50: 3d22 4172 726f 7731 4c65 6e64 220a 2020  ="Arrow1Lend".  
+00000e60: 2020 2020 2069 6e6b 7363 6170 653a 6973       inkscape:is
+00000e70: 7374 6f63 6b3d 2274 7275 6522 3e0a 2020  stock="true">.  
+00000e80: 2020 2020 3c70 6174 680a 2020 2020 2020      <path.      
+00000e90: 2020 2074 7261 6e73 666f 726d 3d22 6d61     transform="ma
+00000ea0: 7472 6978 282d 302e 382c 302c 302c 2d30  trix(-0.8,0,0,-0
+00000eb0: 2e38 2c2d 3130 2c30 2922 0a20 2020 2020  .8,-10,0)".     
+00000ec0: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
+00000ed0: 636f 6e74 6578 742d 7374 726f 6b65 3b66  context-stroke;f
+00000ee0: 696c 6c2d 7275 6c65 3a65 7665 6e6f 6464  ill-rule:evenodd
+00000ef0: 3b73 7472 6f6b 653a 636f 6e74 6578 742d  ;stroke:context-
+00000f00: 7374 726f 6b65 3b73 7472 6f6b 652d 7769  stroke;stroke-wi
+00000f10: 6474 683a 3170 7422 0a20 2020 2020 2020  dth:1pt".       
+00000f20: 2020 643d 224d 2030 2c30 2035 2c2d 3520    d="M 0,0 5,-5 
+00000f30: 2d31 322e 352c 3020 352c 3520 5a22 0a20  -12.5,0 5,5 Z". 
+00000f40: 2020 2020 2020 2020 6964 3d22 7061 7468          id="path
+00000f50: 3131 3331 2220 2f3e 0a20 2020 203c 2f6d  1131" />.    </m
+00000f60: 6172 6b65 723e 0a20 203c 2f64 6566 733e  arker>.  </defs>
+00000f70: 0a20 203c 670a 2020 2020 2069 643d 226c  .  <g.     id="l
+00000f80: 6179 6572 322d 3622 0a20 2020 2020 696e  ayer2-6".     in
+00000f90: 6b73 6361 7065 3a6c 6162 656c 3d22 4c6f  kscape:label="Lo
+00000fa0: 7765 7222 0a20 2020 2020 7374 796c 653d  wer".     style=
+00000fb0: 2264 6973 706c 6179 3a69 6e6c 696e 6522  "display:inline"
+00000fc0: 0a20 2020 2020 7472 616e 7366 6f72 6d3d  .     transform=
+00000fd0: 2274 7261 6e73 6c61 7465 2831 2e38 3933  "translate(1.893
+00000fe0: 3032 3435 2c2d 382e 3537 3538 3539 2922  0245,-8.575859)"
+00000ff0: 0a20 2020 2020 696e 6b73 6361 7065 3a67  .     inkscape:g
+00001000: 726f 7570 6d6f 6465 3d22 6c61 7965 7222  roupmode="layer"
+00001010: 0a20 2020 2020 736f 6469 706f 6469 3a69  .     sodipodi:i
+00001020: 6e73 656e 7369 7469 7665 3d22 7472 7565  nsensitive="true
+00001030: 223e 0a20 2020 203c 7061 7468 0a20 2020  ">.    <path.   
+00001040: 2020 2020 7374 796c 653d 2264 6973 706c      style="displ
+00001050: 6179 3a69 6e6c 696e 653b 6f70 6163 6974  ay:inline;opacit
+00001060: 793a 302e 333b 6669 6c6c 3a23 6162 6465  y:0.3;fill:#abde
+00001070: 6535 3b73 7472 6f6b 653a 2330 3030 3030  e5;stroke:#00000
+00001080: 303b 7374 726f 6b65 2d77 6964 7468 3a30  0;stroke-width:0
+00001090: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
+000010a0: 6275 7474 3b73 7472 6f6b 652d 6c69 6e65  butt;stroke-line
+000010b0: 6a6f 696e 3a6d 6974 6572 3b73 7472 6f6b  join:miter;strok
+000010c0: 652d 6d69 7465 726c 696d 6974 3a34 3b73  e-miterlimit:4;s
+000010d0: 7472 6f6b 652d 6461 7368 6172 7261 793a  troke-dasharray:
+000010e0: 6e6f 6e65 3b73 7472 6f6b 652d 6f70 6163  none;stroke-opac
+000010f0: 6974 793a 3122 0a20 2020 2020 2020 643d  ity:1".       d=
+00001100: 226d 2032 352e 3032 3031 3233 2c33 342e  "m 25.020123,34.
+00001110: 3037 3538 3620 6320 302c 3020 2d30 2e37  07586 c 0,0 -0.7
+00001120: 3536 3037 392c 3230 2e32 3032 3531 3720  56079,20.202517 
+00001130: 332e 3537 3035 382c 3232 2e37 3030 3531  3.57058,22.70051
+00001140: 3420 302e 3538 3438 3732 2c30 2e33 3337  4 0.584872,0.337
+00001150: 3637 3520 312e 3135 3835 3139 2c30 2e32  675 1.158519,0.2
+00001160: 3931 3732 3820 312e 3731 3332 3839 2c2d  91728 1.713289,-
+00001170: 302e 3034 3033 206c 2031 2e37 3332 3035  0.0403 l 1.73205
+00001180: 312c 2d30 2e39 3939 3939 3920 6320 2d30  1,-0.999999 c -0
+00001190: 2e35 3534 3737 2c30 2e33 3332 3032 3520  .55477,0.332025 
+000011a0: 2d31 2e31 3238 3431 372c 302e 3337 3739  -1.128417,0.3779
+000011b0: 3732 202d 312e 3731 3332 3839 2c30 2e30  72 -1.713289,0.0
+000011c0: 3430 3320 2d34 2e33 3236 3635 392c 2d32  403 -4.326659,-2
+000011d0: 2e34 3937 3939 3720 2d33 2e35 3730 3538  .497997 -3.57058
+000011e0: 2c2d 3232 2e37 3030 3531 3520 2d33 2e35  ,-22.700515 -3.5
+000011f0: 3730 3538 2c2d 3232 2e37 3030 3531 3522  7058,-22.700515"
+00001200: 0a20 2020 2020 2020 6964 3d22 7061 7468  .       id="path
+00001210: 3433 3435 302d 3122 0a20 2020 2020 2020  43450-1".       
+00001220: 696e 6b73 6361 7065 3a6c 6162 656c 3d22  inkscape:label="
+00001230: 4261 6e64 2033 220a 2020 2020 2020 2073  Band 3".       s
+00001240: 6f64 6970 6f64 693a 6e6f 6465 7479 7065  odipodi:nodetype
+00001250: 733d 2263 7363 6373 6322 0a20 2020 2020  s="csccsc".     
+00001260: 2020 736f 6469 706f 6469 3a69 6e73 656e    sodipodi:insen
+00001270: 7369 7469 7665 3d22 7472 7565 2220 2f3e  sitive="true" />
+00001280: 0a20 2020 203c 7061 7468 0a20 2020 2020  .    <path.     
+00001290: 2020 7374 796c 653d 2264 6973 706c 6179    style="display
+000012a0: 3a69 6e6c 696e 653b 6669 6c6c 3a6e 6f6e  :inline;fill:non
+000012b0: 653b 7374 726f 6b65 3a23 3030 3030 3030  e;stroke:#000000
+000012c0: 3b73 7472 6f6b 652d 7769 6474 683a 302e  ;stroke-width:0.
+000012d0: 313b 7374 726f 6b65 2d6c 696e 6563 6170  1;stroke-linecap
+000012e0: 3a62 7574 743b 7374 726f 6b65 2d6c 696e  :butt;stroke-lin
+000012f0: 656a 6f69 6e3a 6d69 7465 723b 7374 726f  ejoin:miter;stro
+00001300: 6b65 2d6d 6974 6572 6c69 6d69 743a 343b  ke-miterlimit:4;
+00001310: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
+00001320: 3a6e 6f6e 653b 7374 726f 6b65 2d6f 7061  :none;stroke-opa
+00001330: 6369 7479 3a31 220a 2020 2020 2020 2064  city:1".       d
+00001340: 3d22 6d20 3236 2e37 3532 3137 342c 3333  ="m 26.752174,33
+00001350: 2e30 3735 3836 2063 2030 2c30 202d 302e  .07586 c 0,0 -0.
+00001360: 3735 3630 3739 2c32 302e 3230 3235 3137  756079,20.202517
+00001370: 2033 2e35 3730 3538 2c32 322e 3730 3035   3.57058,22.7005
+00001380: 3134 2030 2e35 3834 3837 322c 302e 3333  14 0.584872,0.33
+00001390: 3736 3735 2031 2e31 3538 3532 2c30 2e32  7675 1.15852,0.2
+000013a0: 3931 3732 3820 312e 3731 3332 3839 2c2d  91728 1.713289,-
+000013b0: 302e 3034 3033 206c 202d 312e 3733 3230  0.0403 l -1.7320
+000013c0: 3531 2c31 2063 202d 302e 3535 3437 372c  51,1 c -0.55477,
+000013d0: 302e 3333 3230 3234 202d 312e 3132 3834  0.332024 -1.1284
+000013e0: 3136 2c30 2e33 3737 3937 3120 2d31 2e37  16,0.377971 -1.7
+000013f0: 3133 3238 392c 302e 3034 3033 2043 2032  13289,0.0403 C 2
+00001400: 342e 3236 3430 3435 2c35 342e 3237 3833  4.264045,54.2783
+00001410: 3737 2032 352e 3032 3031 3234 2c33 342e  77 25.020124,34.
+00001420: 3037 3538 3620 3235 2e30 3230 3132 342c  07586 25.020124,
+00001430: 3334 2e30 3735 3836 220a 2020 2020 2020  34.07586".      
+00001440: 2069 643d 2270 6174 6835 3234 3337 2d35   id="path52437-5
+00001450: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
+00001460: 653a 6c61 6265 6c3d 224c 696e 6520 3322  e:label="Line 3"
+00001470: 0a20 2020 2020 2020 736f 6469 706f 6469  .       sodipodi
+00001480: 3a6e 6f64 6574 7970 6573 3d22 6373 6363  :nodetypes="cscc
+00001490: 7363 220a 2020 2020 2020 2073 6f64 6970  sc".       sodip
+000014a0: 6f64 693a 696e 7365 6e73 6974 6976 653d  odi:insensitive=
+000014b0: 2274 7275 6522 202f 3e0a 2020 2020 3c70  "true" />.    <p
+000014c0: 6174 680a 2020 2020 2020 2073 7479 6c65  ath.       style
+000014d0: 3d22 6469 7370 6c61 793a 696e 6c69 6e65  ="display:inline
+000014e0: 3b66 696c 6c3a 6e6f 6e65 3b73 7472 6f6b  ;fill:none;strok
+000014f0: 653a 2330 3030 3030 303b 7374 726f 6b65  e:#000000;stroke
+00001500: 2d77 6964 7468 3a30 2e31 3b73 7472 6f6b  -width:0.1;strok
+00001510: 652d 6c69 6e65 6361 703a 6275 7474 3b73  e-linecap:butt;s
+00001520: 7472 6f6b 652d 6c69 6e65 6a6f 696e 3a6d  troke-linejoin:m
+00001530: 6974 6572 3b73 7472 6f6b 652d 6d69 7465  iter;stroke-mite
+00001540: 726c 696d 6974 3a34 3b73 7472 6f6b 652d  rlimit:4;stroke-
+00001550: 6461 7368 6172 7261 793a 6e6f 6e65 3b73  dasharray:none;s
+00001560: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
+00001570: 0a20 2020 2020 2020 643d 226d 2033 362e  .       d="m 36.
+00001580: 3632 3236 3633 2c34 302e 3737 3435 3920  622663,40.77459 
+00001590: 6320 302c 3020 2d32 2e37 3639 3436 332c  c 0,0 -2.769463,
+000015a0: 3133 2e38 3337 3331 3820 2d36 2e33 3138  13.837318 -6.318
+000015b0: 3637 312c 3135 2e39 3631 3438 3820 6c20  671,15.961488 l 
+000015c0: 312e 3733 3139 3839 2c2d 302e 3939 3939  1.731989,-0.9999
+000015d0: 3634 2063 2033 2e35 3439 3230 382c 2d32  64 c 3.549208,-2
+000015e0: 2e31 3234 3136 3920 362e 3331 3836 3731  .124169 6.318671
+000015f0: 2c2d 3135 2e39 3631 3438 3720 362e 3331  ,-15.961487 6.31
+00001600: 3836 3731 2c2d 3135 2e39 3631 3438 3722  8671,-15.961487"
+00001610: 0a20 2020 2020 2020 6964 3d22 7061 7468  .       id="path
+00001620: 3234 3737 2d37 220a 2020 2020 2020 2069  2477-7".       i
+00001630: 6e6b 7363 6170 653a 6c61 6265 6c3d 224c  nkscape:label="L
+00001640: 696e 6520 3422 0a20 2020 2020 2020 736f  ine 4".       so
+00001650: 6469 706f 6469 3a6e 6f64 6574 7970 6573  dipodi:nodetypes
+00001660: 3d22 6363 6363 220a 2020 2020 2020 2073  ="cccc".       s
+00001670: 6f64 6970 6f64 693a 696e 7365 6e73 6974  odipodi:insensit
+00001680: 6976 653d 2274 7275 6522 202f 3e0a 2020  ive="true" />.  
+00001690: 2020 3c70 6174 680a 2020 2020 2020 2073    <path.       s
+000016a0: 7479 6c65 3d22 6469 7370 6c61 793a 696e  tyle="display:in
+000016b0: 6c69 6e65 3b6f 7061 6369 7479 3a30 2e33  line;opacity:0.3
+000016c0: 3b66 696c 6c3a 2361 6264 6565 353b 7374  ;fill:#abdee5;st
+000016d0: 726f 6b65 3a23 3030 3030 3030 3b73 7472  roke:#000000;str
+000016e0: 6f6b 652d 7769 6474 683a 303b 7374 726f  oke-width:0;stro
+000016f0: 6b65 2d6c 696e 6563 6170 3a62 7574 743b  ke-linecap:butt;
+00001700: 7374 726f 6b65 2d6c 696e 656a 6f69 6e3a  stroke-linejoin:
+00001710: 6d69 7465 723b 7374 726f 6b65 2d6d 6974  miter;stroke-mit
+00001720: 6572 6c69 6d69 743a 343b 7374 726f 6b65  erlimit:4;stroke
+00001730: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
+00001740: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
+00001750: 220a 2020 2020 2020 2064 3d22 6d20 3336  ".       d="m 36
+00001760: 2e36 3232 3636 332c 3430 2e37 3734 3539  .622663,40.77459
+00001770: 2063 2030 2c30 202d 322e 3736 3934 3633   c 0,0 -2.769463
+00001780: 2c31 332e 3833 3733 3138 202d 362e 3331  ,13.837318 -6.31
+00001790: 3836 3731 2c31 352e 3936 3134 3838 206c  8671,15.961488 l
+000017a0: 2031 2e37 3331 3938 392c 2d30 2e39 3939   1.731989,-0.999
+000017b0: 3936 3420 6320 332e 3534 3932 3038 2c2d  964 c 3.549208,-
+000017c0: 322e 3132 3431 3639 2036 2e33 3138 3637  2.124169 6.31867
+000017d0: 312c 2d31 352e 3936 3134 3837 2036 2e33  1,-15.961487 6.3
+000017e0: 3138 3637 312c 2d31 352e 3936 3134 3837  18671,-15.961487
+000017f0: 207a 220a 2020 2020 2020 2069 643d 2270   z".       id="p
+00001800: 6174 6834 3436 312d 3722 0a20 2020 2020  ath4461-7".     
+00001810: 2020 696e 6b73 6361 7065 3a6c 6162 656c    inkscape:label
+00001820: 3d22 4261 6e64 2034 220a 2020 2020 2020  ="Band 4".      
+00001830: 2073 6f64 6970 6f64 693a 6e6f 6465 7479   sodipodi:nodety
+00001840: 7065 733d 2263 6363 6363 220a 2020 2020  pes="ccccc".    
+00001850: 2020 2073 6f64 6970 6f64 693a 696e 7365     sodipodi:inse
+00001860: 6e73 6974 6976 653d 2274 7275 6522 202f  nsitive="true" /
+00001870: 3e0a 2020 3c2f 673e 0a20 203c 670a 2020  >.  </g>.  <g.  
+00001880: 2020 2069 6e6b 7363 6170 653a 6c61 6265     inkscape:labe
+00001890: 6c3d 2250 6c61 6e65 220a 2020 2020 2069  l="Plane".     i
+000018a0: 6e6b 7363 6170 653a 6772 6f75 706d 6f64  nkscape:groupmod
+000018b0: 653d 226c 6179 6572 220a 2020 2020 2069  e="layer".     i
+000018c0: 643d 226c 6179 6572 3122 0a20 2020 2020  d="layer1".     
+000018d0: 7374 796c 653d 2264 6973 706c 6179 3a69  style="display:i
+000018e0: 6e6c 696e 6522 0a20 2020 2020 736f 6469  nline".     sodi
+000018f0: 706f 6469 3a69 6e73 656e 7369 7469 7665  podi:insensitive
+00001900: 3d22 7472 7565 223e 0a20 2020 203c 7265  ="true">.    <re
+00001910: 6374 0a20 2020 2020 2020 7374 796c 653d  ct.       style=
+00001920: 226f 7061 6369 7479 3a30 2e33 3b66 696c  "opacity:0.3;fil
+00001930: 6c3a 2361 6335 3630 653b 7374 726f 6b65  l:#ac560e;stroke
+00001940: 3a23 3030 3030 3030 3b73 7472 6f6b 652d  :#000000;stroke-
+00001950: 7769 6474 683a 303b 7374 726f 6b65 2d6c  width:0;stroke-l
+00001960: 696e 6563 6170 3a72 6f75 6e64 3b73 7472  inecap:round;str
+00001970: 6f6b 652d 6c69 6e65 6a6f 696e 3a62 6576  oke-linejoin:bev
+00001980: 656c 3b73 7472 6f6b 652d 6d69 7465 726c  el;stroke-miterl
+00001990: 696d 6974 3a34 3b73 7472 6f6b 652d 6461  imit:4;stroke-da
+000019a0: 7368 6172 7261 793a 6e6f 6e65 220a 2020  sharray:none".  
+000019b0: 2020 2020 2069 643d 2272 6563 7432 3030       id="rect200
+000019c0: 3122 0a20 2020 2020 2020 7769 6474 683d  1".       width=
+000019d0: 2231 332e 3339 3734 3539 220a 2020 2020  "13.397459".    
+000019e0: 2020 2068 6569 6768 743d 2231 352e 3437     height="15.47
+000019f0: 3030 3534 220a 2020 2020 2020 2078 3d22  0054".       x="
+00001a00: 3237 2e36 3430 3836 3322 0a20 2020 2020  27.640863".     
+00001a10: 2020 793d 2238 2e39 3631 3638 3822 0a20    y="8.961688". 
+00001a20: 2020 2020 2020 696e 6b73 6361 7065 3a6c        inkscape:l
+00001a30: 6162 656c 3d22 5175 6164 7261 6e74 2031  abel="Quadrant 1
+00001a40: 220a 2020 2020 2020 2074 7261 6e73 666f  ".       transfo
+00001a50: 726d 3d22 6d61 7472 6978 2830 2e38 3636  rm="matrix(0.866
+00001a60: 3032 3534 2c30 2e35 2c2d 302e 3836 3630  0254,0.5,-0.8660
+00001a70: 3235 342c 302e 352c 302c 3029 220a 2020  254,0.5,0,0)".  
+00001a80: 2020 2020 2073 6f64 6970 6f64 693a 696e       sodipodi:in
+00001a90: 7365 6e73 6974 6976 653d 2274 7275 6522  sensitive="true"
+00001aa0: 202f 3e0a 2020 2020 3c72 6563 740a 2020   />.    <rect.  
+00001ab0: 2020 2020 2073 7479 6c65 3d22 6f70 6163       style="opac
+00001ac0: 6974 793a 302e 333b 6669 6c6c 3a23 6666  ity:0.3;fill:#ff
+00001ad0: 6331 3037 3b73 7472 6f6b 653a 2330 3030  c107;stroke:#000
+00001ae0: 3030 303b 7374 726f 6b65 2d77 6964 7468  000;stroke-width
+00001af0: 3a30 3b73 7472 6f6b 652d 6c69 6e65 6361  :0;stroke-lineca
+00001b00: 703a 726f 756e 643b 7374 726f 6b65 2d6c  p:round;stroke-l
+00001b10: 696e 656a 6f69 6e3a 6265 7665 6c3b 7374  inejoin:bevel;st
+00001b20: 726f 6b65 2d6d 6974 6572 6c69 6d69 743a  roke-miterlimit:
+00001b30: 343b 7374 726f 6b65 2d64 6173 6861 7272  4;stroke-dasharr
+00001b40: 6179 3a6e 6f6e 6522 0a20 2020 2020 2020  ay:none".       
+00001b50: 6964 3d22 7265 6374 3133 3033 220a 2020  id="rect1303".  
+00001b60: 2020 2020 2077 6964 7468 3d22 3133 2e33       width="13.3
+00001b70: 3937 3435 3922 0a20 2020 2020 2020 6865  97459".       he
+00001b80: 6967 6874 3d22 3135 2e34 3730 3035 3422  ight="15.470054"
+00001b90: 0a20 2020 2020 2020 783d 2232 372e 3634  .       x="27.64
+00001ba0: 3038 3633 220a 2020 2020 2020 2079 3d22  0863".       y="
+00001bb0: 2d36 2e35 3038 3336 3536 220a 2020 2020  -6.5083656".    
+00001bc0: 2020 2069 6e6b 7363 6170 653a 6c61 6265     inkscape:labe
+00001bd0: 6c3d 2251 7561 6472 616e 7420 3222 0a20  l="Quadrant 2". 
+00001be0: 2020 2020 2020 7472 616e 7366 6f72 6d3d        transform=
+00001bf0: 226d 6174 7269 7828 302e 3836 3630 3235  "matrix(0.866025
+00001c00: 342c 302e 352c 2d30 2e38 3636 3032 3534  4,0.5,-0.8660254
+00001c10: 2c30 2e35 2c30 2c30 2922 0a20 2020 2020  ,0.5,0,0)".     
+00001c20: 2020 736f 6469 706f 6469 3a69 6e73 656e    sodipodi:insen
+00001c30: 7369 7469 7665 3d22 7472 7565 2220 2f3e  sitive="true" />
+00001c40: 0a20 2020 203c 7265 6374 0a20 2020 2020  .    <rect.     
+00001c50: 2020 7374 796c 653d 226f 7061 6369 7479    style="opacity
+00001c60: 3a30 2e33 3b66 696c 6c3a 2331 3338 3839  :0.3;fill:#13889
+00001c70: 623b 7374 726f 6b65 3a23 3030 3030 3030  b;stroke:#000000
+00001c80: 3b73 7472 6f6b 652d 7769 6474 683a 303b  ;stroke-width:0;
+00001c90: 7374 726f 6b65 2d6c 696e 6563 6170 3a72  stroke-linecap:r
+00001ca0: 6f75 6e64 3b73 7472 6f6b 652d 6c69 6e65  ound;stroke-line
+00001cb0: 6a6f 696e 3a62 6576 656c 3b73 7472 6f6b  join:bevel;strok
+00001cc0: 652d 6d69 7465 726c 696d 6974 3a34 3b73  e-miterlimit:4;s
+00001cd0: 7472 6f6b 652d 6461 7368 6172 7261 793a  troke-dasharray:
+00001ce0: 6e6f 6e65 220a 2020 2020 2020 2069 643d  none".       id=
+00001cf0: 2272 6563 7432 3030 3322 0a20 2020 2020  "rect2003".     
+00001d00: 2020 7769 6474 683d 2231 332e 3339 3734    width="13.3974
+00001d10: 3539 220a 2020 2020 2020 2068 6569 6768  59".       heigh
+00001d20: 743d 2231 352e 3437 3030 3534 220a 2020  t="15.470054".  
+00001d30: 2020 2020 2078 3d22 3431 2e30 3338 3331       x="41.03831
+00001d40: 3922 0a20 2020 2020 2020 793d 222d 362e  9".       y="-6.
+00001d50: 3530 3833 3635 3622 0a20 2020 2020 2020  5083656".       
+00001d60: 696e 6b73 6361 7065 3a6c 6162 656c 3d22  inkscape:label="
+00001d70: 5175 6164 7261 6e74 2033 220a 2020 2020  Quadrant 3".    
+00001d80: 2020 2074 7261 6e73 666f 726d 3d22 6d61     transform="ma
+00001d90: 7472 6978 2830 2e38 3636 3032 3534 2c30  trix(0.8660254,0
+00001da0: 2e35 2c2d 302e 3836 3630 3235 342c 302e  .5,-0.8660254,0.
+00001db0: 352c 302c 3029 220a 2020 2020 2020 2073  5,0,0)".       s
+00001dc0: 6f64 6970 6f64 693a 696e 7365 6e73 6974  odipodi:insensit
+00001dd0: 6976 653d 2274 7275 6522 202f 3e0a 2020  ive="true" />.  
+00001de0: 2020 3c72 6563 740a 2020 2020 2020 2073    <rect.       s
+00001df0: 7479 6c65 3d22 6f70 6163 6974 793a 302e  tyle="opacity:0.
+00001e00: 333b 6669 6c6c 3a23 3230 6339 3937 3b73  3;fill:#20c997;s
+00001e10: 7472 6f6b 653a 2330 3030 3030 303b 7374  troke:#000000;st
+00001e20: 726f 6b65 2d77 6964 7468 3a30 3b73 7472  roke-width:0;str
+00001e30: 6f6b 652d 6c69 6e65 6361 703a 726f 756e  oke-linecap:roun
+00001e40: 643b 7374 726f 6b65 2d6c 696e 656a 6f69  d;stroke-linejoi
+00001e50: 6e3a 6265 7665 6c3b 7374 726f 6b65 2d6d  n:bevel;stroke-m
+00001e60: 6974 6572 6c69 6d69 743a 343b 7374 726f  iterlimit:4;stro
+00001e70: 6b65 2d64 6173 6861 7272 6179 3a6e 6f6e  ke-dasharray:non
+00001e80: 6522 0a20 2020 2020 2020 6964 3d22 7265  e".       id="re
+00001e90: 6374 3230 3035 220a 2020 2020 2020 2077  ct2005".       w
+00001ea0: 6964 7468 3d22 3133 2e33 3937 3435 3922  idth="13.397459"
+00001eb0: 0a20 2020 2020 2020 6865 6967 6874 3d22  .       height="
+00001ec0: 3135 2e34 3730 3035 3422 0a20 2020 2020  15.470054".     
+00001ed0: 2020 783d 2234 312e 3033 3833 3139 220a    x="41.038319".
+00001ee0: 2020 2020 2020 2079 3d22 382e 3936 3136         y="8.9616
+00001ef0: 3838 220a 2020 2020 2020 2069 6e6b 7363  88".       inksc
+00001f00: 6170 653a 6c61 6265 6c3d 2251 7561 6472  ape:label="Quadr
+00001f10: 616e 7420 3422 0a20 2020 2020 2020 7472  ant 4".       tr
+00001f20: 616e 7366 6f72 6d3d 226d 6174 7269 7828  ansform="matrix(
+00001f30: 302e 3836 3630 3235 342c 302e 352c 2d30  0.8660254,0.5,-0
+00001f40: 2e38 3636 3032 3534 2c30 2e35 2c30 2c30  .8660254,0.5,0,0
+00001f50: 2922 0a20 2020 2020 2020 736f 6469 706f  )".       sodipo
+00001f60: 6469 3a69 6e73 656e 7369 7469 7665 3d22  di:insensitive="
+00001f70: 7472 7565 2220 2f3e 0a20 2020 203c 7265  true" />.    <re
+00001f80: 6374 0a20 2020 2020 2020 7374 796c 653d  ct.       style=
+00001f90: 226f 7061 6369 7479 3a31 3b66 696c 6c3a  "opacity:1;fill:
+00001fa0: 6e6f 6e65 3b66 696c 6c2d 6f70 6163 6974  none;fill-opacit
+00001fb0: 793a 313b 7374 726f 6b65 3a23 3030 3030  y:1;stroke:#0000
+00001fc0: 3030 3b73 7472 6f6b 652d 7769 6474 683a  00;stroke-width:
+00001fd0: 302e 3332 3233 3731 3b73 7472 6f6b 652d  0.322371;stroke-
+00001fe0: 6c69 6e65 6361 703a 726f 756e 643b 7374  linecap:round;st
+00001ff0: 726f 6b65 2d6c 696e 656a 6f69 6e3a 6d69  roke-linejoin:mi
+00002000: 7465 723b 7374 726f 6b65 2d6d 6974 6572  ter;stroke-miter
+00002010: 6c69 6d69 743a 343b 7374 726f 6b65 2d64  limit:4;stroke-d
+00002020: 6173 6861 7272 6179 3a6e 6f6e 6522 0a20  asharray:none". 
+00002030: 2020 2020 2020 6964 3d22 7265 6374 3439        id="rect49
+00002040: 3337 220a 2020 2020 2020 2077 6964 7468  37".       width
+00002050: 3d22 3236 2e37 3934 3931 3822 0a20 2020  ="26.794918".   
+00002060: 2020 2020 6865 6967 6874 3d22 3330 2e39      height="30.9
+00002070: 3430 3130 3722 0a20 2020 2020 2020 783d  40107".       x=
+00002080: 2232 372e 3634 3038 3633 220a 2020 2020  "27.640863".    
+00002090: 2020 2079 3d22 2d36 2e35 3038 3336 3536     y="-6.5083656
+000020a0: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
+000020b0: 653a 6c61 6265 6c3d 2246 7261 6d65 220a  e:label="Frame".
+000020c0: 2020 2020 2020 2074 7261 6e73 666f 726d         transform
+000020d0: 3d22 6d61 7472 6978 2830 2e38 3636 3032  ="matrix(0.86602
+000020e0: 3534 2c30 2e35 2c2d 302e 3836 3630 3235  54,0.5,-0.866025
+000020f0: 342c 302e 352c 302c 3029 220a 2020 2020  4,0.5,0,0)".    
+00002100: 2020 2073 6f64 6970 6f64 693a 696e 7365     sodipodi:inse
+00002110: 6e73 6974 6976 653d 2274 7275 6522 202f  nsitive="true" /
+00002120: 3e0a 2020 2020 3c70 6174 680a 2020 2020  >.    <path.    
+00002130: 2020 2073 7479 6c65 3d22 6669 6c6c 3a6e     style="fill:n
+00002140: 6f6e 653b 7374 726f 6b65 3a23 3030 3030  one;stroke:#0000
+00002150: 3030 3b73 7472 6f6b 652d 7769 6474 683a  00;stroke-width:
+00002160: 302e 3035 3335 3839 393b 7374 726f 6b65  0.0535899;stroke
+00002170: 2d6c 696e 6563 6170 3a62 7574 743b 7374  -linecap:butt;st
+00002180: 726f 6b65 2d6c 696e 656a 6f69 6e3a 6d69  roke-linejoin:mi
+00002190: 7465 723b 7374 726f 6b65 2d6d 6974 6572  ter;stroke-miter
+000021a0: 6c69 6d69 743a 343b 7374 726f 6b65 2d64  limit:4;stroke-d
+000021b0: 6173 6861 7272 6179 3a30 2e34 3238 3731  asharray:0.42871
+000021c0: 392c 2030 2e34 3238 3731 393b 7374 726f  9, 0.428719;stro
+000021d0: 6b65 2d64 6173 686f 6666 7365 743a 303b  ke-dashoffset:0;
+000021e0: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
+000021f0: 220a 2020 2020 2020 2064 3d22 4d20 3136  ".       d="M 16
+00002200: 2e31 3736 3633 342c 3138 2e33 3031 3237  .176634,18.30127
+00002210: 3220 3339 2e33 3831 3731 352c 3331 2e36  2 39.381715,31.6
+00002220: 3938 3733 220a 2020 2020 2020 2069 643d  9873".       id=
+00002230: 2270 6174 6835 3236 3422 0a20 2020 2020  "path5264".     
+00002240: 2020 696e 6b73 6361 7065 3a6c 6162 656c    inkscape:label
+00002250: 3d22 582d 4178 6973 220a 2020 2020 2020  ="X-Axis".      
+00002260: 2073 6f64 6970 6f64 693a 696e 7365 6e73   sodipodi:insens
+00002270: 6974 6976 653d 2274 7275 6522 202f 3e0a  itive="true" />.
+00002280: 2020 2020 3c70 6174 680a 2020 2020 2020      <path.      
+00002290: 2073 7479 6c65 3d22 6669 6c6c 3a6e 6f6e   style="fill:non
+000022a0: 653b 7374 726f 6b65 3a23 3030 3030 3030  e;stroke:#000000
+000022b0: 3b73 7472 6f6b 652d 7769 6474 683a 302e  ;stroke-width:0.
+000022c0: 3035 3335 3839 393b 7374 726f 6b65 2d6c  0535899;stroke-l
+000022d0: 696e 6563 6170 3a62 7574 743b 7374 726f  inecap:butt;stro
+000022e0: 6b65 2d6c 696e 656a 6f69 6e3a 6d69 7465  ke-linejoin:mite
+000022f0: 723b 7374 726f 6b65 2d6d 6974 6572 6c69  r;stroke-miterli
+00002300: 6d69 743a 343b 7374 726f 6b65 2d64 6173  mit:4;stroke-das
+00002310: 6861 7272 6179 3a30 2e34 3238 3731 392c  harray:0.428719,
+00002320: 2030 2e34 3238 3731 393b 7374 726f 6b65   0.428719;stroke
+00002330: 2d64 6173 686f 6666 7365 743a 303b 7374  -dashoffset:0;st
+00002340: 726f 6b65 2d6f 7061 6369 7479 3a31 220a  roke-opacity:1".
+00002350: 2020 2020 2020 2064 3d22 4d20 3431 2e31         d="M 41.1
+00002360: 3736 3633 342c 3137 2e32 3634 3937 3520  76634,17.264975 
+00002370: 3134 2e33 3831 3731 332c 3332 2e37 3335  14.381713,32.735
+00002380: 3032 3722 0a20 2020 2020 2020 6964 3d22  027".       id="
+00002390: 7061 7468 3535 3936 220a 2020 2020 2020  path5596".      
+000023a0: 2069 6e6b 7363 6170 653a 6c61 6265 6c3d   inkscape:label=
+000023b0: 2259 2d41 7869 7322 0a20 2020 2020 2020  "Y-Axis".       
+000023c0: 736f 6469 706f 6469 3a69 6e73 656e 7369  sodipodi:insensi
+000023d0: 7469 7665 3d22 7472 7565 2220 2f3e 0a20  tive="true" />. 
+000023e0: 203c 2f67 3e0a 2020 3c67 0a20 2020 2020   </g>.  <g.     
+000023f0: 696e 6b73 6361 7065 3a67 726f 7570 6d6f  inkscape:groupmo
+00002400: 6465 3d22 6c61 7965 7222 0a20 2020 2020  de="layer".     
+00002410: 6964 3d22 6c61 7965 7233 220a 2020 2020  id="layer3".    
+00002420: 2069 6e6b 7363 6170 653a 6c61 6265 6c3d   inkscape:label=
+00002430: 2250 6f6c 6172 220a 2020 2020 2073 6f64  "Polar".     sod
+00002440: 6970 6f64 693a 696e 7365 6e73 6974 6976  ipodi:insensitiv
+00002450: 653d 2274 7275 6522 3e0a 2020 2020 3c70  e="true">.    <p
+00002460: 6174 680a 2020 2020 2020 2069 643d 2270  ath.       id="p
+00002470: 6174 6839 3730 3322 0a20 2020 2020 2020  ath9703".       
+00002480: 7374 796c 653d 2264 6973 706c 6179 3a69  style="display:i
+00002490: 6e6c 696e 653b 6f70 6163 6974 793a 302e  nline;opacity:0.
+000024a0: 373b 6669 6c6c 3a23 6162 6465 6535 3b73  7;fill:#abdee5;s
+000024b0: 7472 6f6b 653a 2330 3030 3030 303b 7374  troke:#000000;st
+000024c0: 726f 6b65 2d77 6964 7468 3a30 2e31 3030  roke-width:0.100
+000024d0: 363b 7374 726f 6b65 2d6c 696e 6563 6170  6;stroke-linecap
+000024e0: 3a72 6f75 6e64 3b73 7472 6f6b 652d 6c69  :round;stroke-li
+000024f0: 6e65 6a6f 696e 3a72 6f75 6e64 3b73 7472  nejoin:round;str
+00002500: 6f6b 652d 6d69 7465 726c 696d 6974 3a30  oke-miterlimit:0
+00002510: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
+00002520: 793a 6e6f 6e65 220a 2020 2020 2020 2064  y:none".       d
+00002530: 3d22 6d20 3135 2e31 3937 3530 392c 3332  ="m 15.197509,32
+00002540: 2e32 3536 3430 3220 302e 3032 3032 362c  .256402 0.02026,
+00002550: 2d30 2e30 3131 3732 2030 2e31 3236 3338  -0.01172 0.12638
+00002560: 332c 2d31 2e30 3034 3536 3320 302e 3132  3,-1.004563 0.12
+00002570: 3631 3131 2c2d 312e 3030 3434 3131 2031  6111,-1.004411 1
+00002580: 2e37 3339 3639 352c 2d30 2e30 3732 3820  .739695,-0.0728 
+00002590: 312e 3733 3936 3932 2c2d 302e 3037 3238  1.739692,-0.0728
+000025a0: 2030 2e30 3230 3236 2c2d 302e 3031 3137   0.02026,-0.0117
+000025b0: 3220 6320 2d34 2e32 3130 312c 2d32 2e34  2 c -4.2101,-2.4
+000025c0: 3330 3739 3920 2d33 2e36 3831 3939 332c  30799 -3.681993,
+000025d0: 2d36 2e36 3736 3636 3420 312e 3137 3935  -6.676664 1.1795
+000025e0: 3537 2c2d 392e 3438 3334 3138 2034 2e38  57,-9.483418 4.8
+000025f0: 3631 3436 382c 2d32 2e38 3036 3638 3920  61468,-2.806689 
+00002600: 3132 2e32 3135 3332 332c 2d33 2e31 3131  12.215323,-3.111
+00002610: 3532 3120 3136 2e34 3235 3439 392c 2d30  521 16.425499,-0
+00002620: 2e36 3830 3836 3920 6c20 332e 3531 3031  .680869 l 3.5101
+00002630: 3535 2c2d 302e 3136 3333 3832 2030 2e32  55,-0.163382 0.2
+00002640: 3632 3532 382c 2d32 2e30 3134 3737 3420  62528,-2.014774 
+00002650: 4320 3334 2e33 3333 3038 352c 3134 2e32  C 34.333085,14.2
+00002660: 3633 3433 3320 3233 2e38 3237 3235 332c  63433 23.827253,
+00002670: 3134 2e36 3938 3932 2031 362e 3838 3232  14.69892 16.8822
+00002680: 3333 2c31 382e 3730 3836 3336 2039 2e39  33,18.708636 9.9
+00002690: 3337 3230 3232 2c32 322e 3731 3833 3435  372022,22.718345
+000026a0: 2039 2e31 3832 3931 3632 2c32 382e 3738   9.1829162,28.78
+000026b0: 3338 3932 2031 352e 3139 3734 3932 2c33  3892 15.197492,3
+000026c0: 322e 3235 3634 205a 220a 2020 2020 2020  2.2564 Z".      
+000026d0: 2073 6f64 6970 6f64 693a 6e6f 6465 7479   sodipodi:nodety
+000026e0: 7065 733d 2263 6363 6363 6363 6363 6363  pes="ccccccccccc
+000026f0: 6363 220a 2020 2020 2020 2069 6e6b 7363  cc".       inksc
+00002700: 6170 653a 6c61 6265 6c3d 2244 6f6e 7574  ape:label="Donut
+00002710: 2031 2d32 220a 2020 2020 2020 2073 6f64   1-2".       sod
+00002720: 6970 6f64 693a 696e 7365 6e73 6974 6976  ipodi:insensitiv
+00002730: 653d 2274 7275 6522 202f 3e0a 2020 2020  e="true" />.    
+00002740: 3c70 6174 680a 2020 2020 2020 2069 643d  <path.       id=
+00002750: 2270 6174 6832 3336 3338 3722 0a20 2020  "path236387".   
+00002760: 2020 2020 7374 796c 653d 2264 6973 706c      style="displ
+00002770: 6179 3a69 6e6c 696e 653b 6669 6c6c 3a6e  ay:inline;fill:n
+00002780: 6f6e 653b 7374 726f 6b65 3a23 3030 3030  one;stroke:#0000
+00002790: 3030 3b73 7472 6f6b 652d 7769 6474 683a  00;stroke-width:
+000027a0: 302e 3035 3033 3030 323b 7374 726f 6b65  0.0503002;stroke
+000027b0: 2d6c 696e 6563 6170 3a72 6f75 6e64 3b73  -linecap:round;s
+000027c0: 7472 6f6b 652d 6d69 7465 726c 696d 6974  troke-miterlimit
+000027d0: 3a34 3b73 7472 6f6b 652d 6461 7368 6172  :4;stroke-dashar
+000027e0: 7261 793a 6e6f 6e65 3b6d 6172 6b65 722d  ray:none;marker-
+000027f0: 656e 643a 7572 6c28 2341 7272 6f77 314c  end:url(#Arrow1L
+00002800: 656e 642d 3629 220a 2020 2020 2020 2064  end-6)".       d
+00002810: 3d22 6d20 3134 2e34 3234 3832 382c 3239  ="m 14.424828,29
+00002820: 2e30 3239 3038 3220 6320 2d32 2e31 3434  .029082 c -2.144
+00002830: 392c 2d33 2e30 3333 3838 202d 302e 3536  9,-3.03388 -0.56
+00002840: 3433 3436 2c2d 362e 3831 3533 3137 2033  4346,-6.815317 3
+00002850: 2e39 3832 3037 362c 2d39 2e34 3430 3139  .982076,-9.44019
+00002860: 3620 342e 3534 3634 3232 2c2d 322e 3632  6 4.546422,-2.62
+00002870: 3438 3735 2031 312e 3038 3738 3038 2c2d  4875 11.087808,-
+00002880: 332e 3533 3236 3433 2031 362e 3334 3236  3.532643 16.3426
+00002890: 3432 2c2d 322e 3239 3432 3837 220a 2020  42,-2.294287".  
+000028a0: 2020 2020 2073 6f64 6970 6f64 693a 6e6f       sodipodi:no
+000028b0: 6465 7479 7065 733d 2263 7363 220a 2020  detypes="csc".  
+000028c0: 2020 2020 2069 6e6b 7363 6170 653a 6c61       inkscape:la
+000028d0: 6265 6c3d 2252 6f74 6174 696e 6720 4172  bel="Rotating Ar
+000028e0: 726f 7720 312d 3222 0a20 2020 2020 2020  row 1-2".       
+000028f0: 736f 6469 706f 6469 3a69 6e73 656e 7369  sodipodi:insensi
+00002900: 7469 7665 3d22 7472 7565 2220 2f3e 0a20  tive="true" />. 
+00002910: 2020 203c 7061 7468 0a20 2020 2020 2020     <path.       
+00002920: 6964 3d22 7061 7468 3832 3633 2d36 2d34  id="path8263-6-4
+00002930: 220a 2020 2020 2020 2073 7479 6c65 3d22  ".       style="
+00002940: 6469 7370 6c61 793a 696e 6c69 6e65 3b6f  display:inline;o
+00002950: 7061 6369 7479 3a30 2e37 3b66 696c 6c3a  pacity:0.7;fill:
+00002960: 2361 6264 6565 353b 7374 726f 6b65 3a23  #abdee5;stroke:#
+00002970: 3030 3030 3030 3b73 7472 6f6b 652d 7769  000000;stroke-wi
+00002980: 6474 683a 302e 3130 3034 3236 3b73 7472  dth:0.100426;str
+00002990: 6f6b 652d 6c69 6e65 6361 703a 726f 756e  oke-linecap:roun
+000029a0: 643b 7374 726f 6b65 2d6c 696e 656a 6f69  d;stroke-linejoi
+000029b0: 6e3a 6265 7665 6c3b 7374 726f 6b65 2d6d  n:bevel;stroke-m
+000029c0: 6974 6572 6c69 6d69 743a 303b 7374 726f  iterlimit:0;stro
+000029d0: 6b65 2d64 6173 6861 7272 6179 3a6e 6f6e  ke-dasharray:non
+000029e0: 6522 0a20 2020 2020 2020 643d 226d 2034  e".       d="m 4
+000029f0: 302e 3338 3535 2c31 372e 3735 3736 3938  0.3855,17.757698
+00002a00: 202d 302e 3032 3032 362c 302e 3031 3137   -0.02026,0.0117
+00002a10: 3220 2d30 2e31 3239 3136 382c 312e 3030  2 -0.129168,1.00
+00002a20: 3239 3537 202d 302e 3132 3839 3132 2c31  2957 -0.128912,1
+00002a30: 2e30 3032 3830 3520 2d31 2e37 3336 3930  .002805 -1.73690
+00002a40: 392c 302e 3037 3434 3320 2d31 2e37 3336  9,0.07443 -1.736
+00002a50: 3930 392c 302e 3037 3434 3220 2d30 2e30  909,0.07442 -0.0
+00002a60: 3230 3236 2c30 2e30 3131 3732 2063 2034  2026,0.01172 c 4
+00002a70: 2e31 3935 3532 372c 322e 3432 3233 3832  .195527,2.422382
+00002a80: 2033 2e36 3535 3538 332c 362e 3636 3134   3.655583,6.6614
+00002a90: 3433 202d 312e 3230 362c 392e 3436 3832  43 -1.206,9.4682
+00002aa0: 3139 202d 342e 3836 3135 3033 2c32 2e38  19 -4.861503,2.8
+00002ab0: 3036 3730 3720 2d31 322e 3230 3335 3734  06707 -12.203574
+00002ac0: 2c33 2e31 3138 3337 3420 2d31 362e 3339  ,3.118374 -16.39
+00002ad0: 3931 3737 2c30 2e36 3936 3133 3620 6c20  9177,0.696136 l 
+00002ae0: 2d33 2e35 3034 3538 2c30 2e31 3636 3632  -3.50458,0.16662
+00002af0: 3120 2d30 2e32 3638 3132 362c 322e 3031  1 -0.268126,2.01
+00002b00: 3135 3620 6320 352e 3939 3337 3435 2c33  156 c 5.993745,3
+00002b10: 2e34 3630 3439 3220 3136 2e34 3832 3733  .460492 16.48273
+00002b20: 372c 332e 3031 3532 3435 2032 332e 3432  7,3.015245 23.42
+00002b30: 3738 3132 2c2d 302e 3939 3435 3031 2036  7812,-0.994501 6
+00002b40: 2e39 3435 3037 382c 2d34 2e30 3039 3733  .945078,-4.00973
+00002b50: 3820 372e 3731 3632 3737 2c2d 3130 2e30  8 7.716277,-10.0
+00002b60: 3635 3536 3320 312e 3732 3235 3137 2c2d  65563 1.722517,-
+00002b70: 3133 2e35 3236 3035 3320 7a22 0a20 2020  13.526053 z".   
+00002b80: 2020 2020 736f 6469 706f 6469 3a6e 6f64      sodipodi:nod
+00002b90: 6574 7970 6573 3d22 6363 6363 6363 6363  etypes="cccccccc
+00002ba0: 6363 6363 6322 0a20 2020 2020 2020 696e  ccccc".       in
+00002bb0: 6b73 6361 7065 3a6c 6162 656c 3d22 446f  kscape:label="Do
+00002bc0: 6e75 7420 332d 3422 0a20 2020 2020 2020  nut 3-4".       
+00002bd0: 736f 6469 706f 6469 3a69 6e73 656e 7369  sodipodi:insensi
+00002be0: 7469 7665 3d22 7472 7565 2220 2f3e 0a20  tive="true" />. 
+00002bf0: 2020 203c 7061 7468 0a20 2020 2020 2020     <path.       
+00002c00: 6964 3d22 7061 7468 3233 3439 3336 220a  id="path234936".
+00002c10: 2020 2020 2020 2073 7479 6c65 3d22 6469         style="di
+00002c20: 7370 6c61 793a 696e 6c69 6e65 3b66 696c  splay:inline;fil
+00002c30: 6c3a 6e6f 6e65 3b73 7472 6f6b 653a 2330  l:none;stroke:#0
+00002c40: 3030 3030 303b 7374 726f 6b65 2d77 6964  00000;stroke-wid
+00002c50: 7468 3a30 2e30 3530 3330 3032 3b73 7472  th:0.0503002;str
+00002c60: 6f6b 652d 6c69 6e65 6361 703a 726f 756e  oke-linecap:roun
+00002c70: 643b 7374 726f 6b65 2d6d 6974 6572 6c69  d;stroke-miterli
+00002c80: 6d69 743a 343b 7374 726f 6b65 2d64 6173  mit:4;stroke-das
+00002c90: 6861 7272 6179 3a6e 6f6e 653b 6d61 726b  harray:none;mark
+00002ca0: 6572 2d65 6e64 3a75 726c 2823 4172 726f  er-end:url(#Arro
+00002cb0: 7731 4c65 6e64 2d36 2922 0a20 2020 2020  w1Lend-6)".     
+00002cc0: 2020 643d 226d 2034 312e 3032 3932 3933    d="m 41.029293
+00002cd0: 2c32 302e 3931 3534 3437 2063 2032 2e31  ,20.915447 c 2.1
+00002ce0: 3434 3839 372c 332e 3033 3338 3820 302e  44897,3.03388 0.
+00002cf0: 3534 3634 3937 2c36 2e38 3030 3234 3220  546497,6.800242 
+00002d00: 2d33 2e39 3939 3932 392c 392e 3432 3531  -3.999929,9.4251
+00002d10: 3220 2d34 2e35 3436 3432 342c 322e 3632  2 -4.546424,2.62
+00002d20: 3438 3820 2d31 312e 3036 3939 3534 2c33  488 -11.069954,3
+00002d30: 2e35 3437 3731 3920 2d31 362e 3332 3437  .547719 -16.3247
+00002d40: 3932 2c32 2e33 3039 3336 3222 0a20 2020  92,2.309362".   
+00002d50: 2020 2020 736f 6469 706f 6469 3a6e 6f64      sodipodi:nod
+00002d60: 6574 7970 6573 3d22 6373 6322 0a20 2020  etypes="csc".   
+00002d70: 2020 2020 696e 6b73 6361 7065 3a6c 6162      inkscape:lab
+00002d80: 656c 3d22 526f 7461 7469 6e67 2041 7272  el="Rotating Arr
+00002d90: 6f77 2033 2d34 220a 2020 2020 2020 2073  ow 3-4".       s
+00002da0: 6f64 6970 6f64 693a 696e 7365 6e73 6974  odipodi:insensit
+00002db0: 6976 653d 2274 7275 6522 202f 3e0a 2020  ive="true" />.  
+00002dc0: 3c2f 673e 0a20 203c 670a 2020 2020 2069  </g>.  <g.     i
+00002dd0: 643d 226c 6179 6572 3222 0a20 2020 2020  d="layer2".     
+00002de0: 696e 6b73 6361 7065 3a6c 6162 656c 3d22  inkscape:label="
+00002df0: 5570 7065 7222 0a20 2020 2020 7374 796c  Upper".     styl
+00002e00: 653d 2264 6973 706c 6179 3a69 6e6c 696e  e="display:inlin
+00002e10: 6522 0a20 2020 2020 7472 616e 7366 6f72  e".     transfor
+00002e20: 6d3d 2274 7261 6e73 6c61 7465 2832 2e37  m="translate(2.7
+00002e30: 3739 3137 3531 2922 0a20 2020 2020 736f  791751)".     so
+00002e40: 6469 706f 6469 3a69 6e73 656e 7369 7469  dipodi:insensiti
+00002e50: 7665 3d22 7472 7565 223e 0a20 2020 203c  ve="true">.    <
+00002e60: 7061 7468 0a20 2020 2020 2020 7374 796c  path.       styl
+00002e70: 653d 2264 6973 706c 6179 3a69 6e6c 696e  e="display:inlin
+00002e80: 653b 6f70 6163 6974 793a 302e 333b 6669  e;opacity:0.3;fi
+00002e90: 6c6c 3a23 6162 6465 6535 3b73 7472 6f6b  ll:#abdee5;strok
+00002ea0: 653a 2330 3030 3030 303b 7374 726f 6b65  e:#000000;stroke
+00002eb0: 2d77 6964 7468 3a30 3b73 7472 6f6b 652d  -width:0;stroke-
+00002ec0: 6c69 6e65 6361 703a 6275 7474 3b73 7472  linecap:butt;str
+00002ed0: 6f6b 652d 6c69 6e65 6a6f 696e 3a6d 6974  oke-linejoin:mit
+00002ee0: 6572 3b73 7472 6f6b 652d 6d69 7465 726c  er;stroke-miterl
+00002ef0: 696d 6974 3a34 3b73 7472 6f6b 652d 6461  imit:4;stroke-da
+00002f00: 7368 6172 7261 793a 6e6f 6e65 3b73 7472  sharray:none;str
+00002f10: 6f6b 652d 6f70 6163 6974 793a 3122 0a20  oke-opacity:1". 
+00002f20: 2020 2020 2020 643d 226d 2031 342e 3236        d="m 14.26
+00002f30: 3334 3837 2c31 372e 3830 3132 3731 2063  3487,17.801271 c
+00002f40: 2030 2c30 2032 2e37 3639 3436 332c 2d31   0,0 2.769463,-1
+00002f50: 332e 3833 3733 3137 3720 362e 3331 3836  3.8373177 6.3186
+00002f60: 3731 2c2d 3135 2e39 3631 3438 3637 206c  71,-15.9614867 l
+00002f70: 202d 312e 3733 3139 3839 2c30 2e39 3939   -1.731989,0.999
+00002f80: 3936 3320 6320 2d33 2e35 3439 3230 382c  963 c -3.549208,
+00002f90: 322e 3132 3431 3720 2d36 2e33 3138 3637  2.12417 -6.31867
+00002fa0: 312c 3135 2e39 3631 3438 3637 202d 362e  1,15.9614867 -6.
+00002fb0: 3331 3836 3731 2c31 352e 3936 3134 3836  318671,15.961486
+00002fc0: 3720 7a22 0a20 2020 2020 2020 6964 3d22  7 z".       id="
+00002fd0: 7061 7468 3434 3631 220a 2020 2020 2020  path4461".      
+00002fe0: 2069 6e6b 7363 6170 653a 6c61 6265 6c3d   inkscape:label=
+00002ff0: 2242 616e 6420 3122 0a20 2020 2020 2020  "Band 1".       
+00003000: 736f 6469 706f 6469 3a6e 6f64 6574 7970  sodipodi:nodetyp
+00003010: 6573 3d22 6363 6363 6322 0a20 2020 2020  es="ccccc".     
+00003020: 2020 736f 6469 706f 6469 3a69 6e73 656e    sodipodi:insen
+00003030: 7369 7469 7665 3d22 7472 7565 2220 2f3e  sitive="true" />
+00003040: 0a20 2020 203c 7061 7468 0a20 2020 2020  .    <path.     
+00003050: 2020 7374 796c 653d 2264 6973 706c 6179    style="display
+00003060: 3a69 6e6c 696e 653b 6669 6c6c 3a6e 6f6e  :inline;fill:non
+00003070: 653b 7374 726f 6b65 3a23 3030 3030 3030  e;stroke:#000000
+00003080: 3b73 7472 6f6b 652d 7769 6474 683a 302e  ;stroke-width:0.
+00003090: 313b 7374 726f 6b65 2d6c 696e 6563 6170  1;stroke-linecap
+000030a0: 3a62 7574 743b 7374 726f 6b65 2d6c 696e  :butt;stroke-lin
+000030b0: 656a 6f69 6e3a 6d69 7465 723b 7374 726f  ejoin:miter;stro
+000030c0: 6b65 2d6d 6974 6572 6c69 6d69 743a 343b  ke-miterlimit:4;
+000030d0: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
+000030e0: 3a6e 6f6e 653b 7374 726f 6b65 2d6f 7061  :none;stroke-opa
+000030f0: 6369 7479 3a31 220a 2020 2020 2020 2064  city:1".       d
+00003100: 3d22 6d20 3134 2e32 3633 3438 372c 3137  ="m 14.263487,17
+00003110: 2e38 3031 3237 3120 6320 302c 3020 322e  .801271 c 0,0 2.
+00003120: 3736 3934 3633 2c2d 3133 2e38 3337 3331  769463,-13.83731
+00003130: 3737 2036 2e33 3138 3637 312c 2d31 352e  77 6.318671,-15.
+00003140: 3936 3134 3836 3720 6c20 2d31 2e37 3331  9614867 l -1.731
+00003150: 3938 392c 302e 3939 3939 3633 2063 202d  989,0.999963 c -
+00003160: 332e 3534 3932 3038 2c32 2e31 3234 3137  3.549208,2.12417
+00003170: 202d 362e 3331 3836 3731 2c31 352e 3936   -6.318671,15.96
+00003180: 3134 3836 3720 2d36 2e33 3138 3637 312c  14867 -6.318671,
+00003190: 3135 2e39 3631 3438 3637 220a 2020 2020  15.9614867".    
+000031a0: 2020 2069 643d 2270 6174 6832 3437 3722     id="path2477"
+000031b0: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
+000031c0: 3a6c 6162 656c 3d22 4c69 6e65 2031 220a  :label="Line 1".
+000031d0: 2020 2020 2020 2073 6f64 6970 6f64 693a         sodipodi:
+000031e0: 6e6f 6465 7479 7065 733d 2263 6363 6322  nodetypes="cccc"
+000031f0: 0a20 2020 2020 2020 736f 6469 706f 6469  .       sodipodi
+00003200: 3a69 6e73 656e 7369 7469 7665 3d22 7472  :insensitive="tr
+00003210: 7565 2220 2f3e 0a20 2020 203c 7061 7468  ue" />.    <path
+00003220: 0a20 2020 2020 2020 7374 796c 653d 2264  .       style="d
+00003230: 6973 706c 6179 3a69 6e6c 696e 653b 6f70  isplay:inline;op
+00003240: 6163 6974 793a 302e 333b 6669 6c6c 3a23  acity:0.3;fill:#
+00003250: 6162 6465 6535 3b73 7472 6f6b 653a 2330  abdee5;stroke:#0
+00003260: 3030 3030 303b 7374 726f 6b65 2d77 6964  00000;stroke-wid
+00003270: 7468 3a30 3b73 7472 6f6b 652d 6c69 6e65  th:0;stroke-line
+00003280: 6361 703a 6275 7474 3b73 7472 6f6b 652d  cap:butt;stroke-
+00003290: 6c69 6e65 6a6f 696e 3a6d 6974 6572 3b73  linejoin:miter;s
+000032a0: 7472 6f6b 652d 6d69 7465 726c 696d 6974  troke-miterlimit
+000032b0: 3a34 3b73 7472 6f6b 652d 6461 7368 6172  :4;stroke-dashar
+000032c0: 7261 793a 6e6f 6e65 3b73 7472 6f6b 652d  ray:none;stroke-
+000032d0: 6f70 6163 6974 793a 3122 0a20 2020 2020  opacity:1".     
+000032e0: 2020 643d 226d 2032 352e 3836 3630 3237    d="m 25.866027
+000032f0: 2c32 342e 3530 3030 3031 2063 2030 2c30  ,24.500001 c 0,0
+00003300: 2030 2e37 3536 3037 392c 2d32 302e 3230   0.756079,-20.20
+00003310: 3235 3135 3720 2d33 2e35 3730 3538 2c2d  25157 -3.57058,-
+00003320: 3232 2e37 3030 3531 3237 202d 302e 3538  22.7005127 -0.58
+00003330: 3438 3732 2c2d 302e 3333 3736 3736 202d  4872,-0.337676 -
+00003340: 312e 3135 3835 3139 2c2d 302e 3239 3137  1.158519,-0.2917
+00003350: 3239 202d 312e 3731 3332 3839 2c30 2e30  29 -1.713289,0.0
+00003360: 3430 3320 6c20 2d31 2e37 3332 3035 312c  403 l -1.732051,
+00003370: 302e 3939 3939 3939 2063 2030 2e35 3534  0.999999 c 0.554
+00003380: 3737 2c2d 302e 3333 3230 3235 2031 2e31  77,-0.332025 1.1
+00003390: 3238 3431 372c 2d30 2e33 3737 3937 3220  28417,-0.377972 
+000033a0: 312e 3731 3332 3839 2c2d 302e 3034 3033  1.713289,-0.0403
+000033b0: 2034 2e33 3236 3635 392c 322e 3439 3739   4.326659,2.4979
+000033c0: 3937 2033 2e35 3730 3538 2c32 322e 3730  97 3.57058,22.70
+000033d0: 3035 3133 3720 332e 3537 3035 382c 3232  05137 3.57058,22
+000033e0: 2e37 3030 3531 3337 220a 2020 2020 2020  .7005137".      
+000033f0: 2069 643d 2270 6174 6834 3334 3530 220a   id="path43450".
+00003400: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+00003410: 6c61 6265 6c3d 2242 616e 6420 3222 0a20  label="Band 2". 
+00003420: 2020 2020 2020 736f 6469 706f 6469 3a6e        sodipodi:n
+00003430: 6f64 6574 7970 6573 3d22 6373 6363 7363  odetypes="csccsc
+00003440: 220a 2020 2020 2020 2073 6f64 6970 6f64  ".       sodipod
+00003450: 693a 696e 7365 6e73 6974 6976 653d 2274  i:insensitive="t
+00003460: 7275 6522 202f 3e0a 2020 2020 3c70 6174  rue" />.    <pat
+00003470: 680a 2020 2020 2020 2073 7479 6c65 3d22  h.       style="
+00003480: 6469 7370 6c61 793a 696e 6c69 6e65 3b66  display:inline;f
+00003490: 696c 6c3a 6e6f 6e65 3b73 7472 6f6b 653a  ill:none;stroke:
+000034a0: 2330 3030 3030 303b 7374 726f 6b65 2d77  #000000;stroke-w
+000034b0: 6964 7468 3a30 2e31 3b73 7472 6f6b 652d  idth:0.1;stroke-
+000034c0: 6c69 6e65 6361 703a 7371 7561 7265 3b73  linecap:square;s
+000034d0: 7472 6f6b 652d 6c69 6e65 6a6f 696e 3a6d  troke-linejoin:m
+000034e0: 6974 6572 3b73 7472 6f6b 652d 6d69 7465  iter;stroke-mite
+000034f0: 726c 696d 6974 3a34 3b73 7472 6f6b 652d  rlimit:4;stroke-
+00003500: 6461 7368 6172 7261 793a 6e6f 6e65 3b73  dasharray:none;s
+00003510: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
+00003520: 0a20 2020 2020 2020 643d 226d 2032 342e  .       d="m 24.
+00003530: 3133 3339 3736 2c32 352e 3530 3030 3031  133976,25.500001
+00003540: 2063 2030 2c30 2030 2e37 3536 3037 392c   c 0,0 0.756079,
+00003550: 2d32 302e 3230 3235 3135 3720 2d33 2e35  -20.2025157 -3.5
+00003560: 3730 3538 2c2d 3232 2e37 3030 3531 3237  7058,-22.7005127
+00003570: 202d 302e 3538 3438 3732 2c2d 302e 3333   -0.584872,-0.33
+00003580: 3736 3736 202d 312e 3135 3835 3139 2c2d  7676 -1.158519,-
+00003590: 302e 3239 3137 3239 202d 312e 3731 3332  0.291729 -1.7132
+000035a0: 3839 2c30 2e30 3430 3320 6c20 312e 3733  89,0.0403 l 1.73
+000035b0: 3230 3531 2c2d 3120 6320 302e 3535 3437  2051,-1 c 0.5547
+000035c0: 372c 2d30 2e33 3332 3032 3520 312e 3132  7,-0.332025 1.12
+000035d0: 3834 3137 2c2d 302e 3337 3739 3732 2031  8417,-0.377972 1
+000035e0: 2e37 3133 3238 392c 2d30 2e30 3430 3320  .713289,-0.0403 
+000035f0: 342e 3332 3636 3539 2c32 2e34 3937 3939  4.326659,2.49799
+00003600: 3720 332e 3537 3035 382c 3232 2e37 3030  7 3.57058,22.700
+00003610: 3531 3237 2033 2e35 3730 3538 2c32 322e  5127 3.57058,22.
+00003620: 3730 3035 3132 3722 0a20 2020 2020 2020  7005127".       
+00003630: 6964 3d22 7061 7468 3532 3433 3722 0a20  id="path52437". 
+00003640: 2020 2020 2020 696e 6b73 6361 7065 3a6c        inkscape:l
+00003650: 6162 656c 3d22 4c69 6e65 2032 220a 2020  abel="Line 2".  
+00003660: 2020 2020 2073 6f64 6970 6f64 693a 6e6f       sodipodi:no
+00003670: 6465 7479 7065 733d 2263 7363 6373 6322  detypes="csccsc"
+00003680: 0a20 2020 2020 2020 736f 6469 706f 6469  .       sodipodi
+00003690: 3a69 6e73 656e 7369 7469 7665 3d22 7472  :insensitive="tr
+000036a0: 7565 2220 2f3e 0a20 2020 203c 7061 7468  ue" />.    <path
+000036b0: 0a20 2020 2020 2020 6964 3d22 7061 7468  .       id="path
+000036c0: 3933 3539 220a 2020 2020 2020 2073 7479  9359".       sty
+000036d0: 6c65 3d22 6469 7370 6c61 793a 696e 6c69  le="display:inli
+000036e0: 6e65 3b6f 7061 6369 7479 3a30 2e33 3b66  ne;opacity:0.3;f
+000036f0: 696c 6c3a 2361 6264 6565 353b 6669 6c6c  ill:#abdee5;fill
+00003700: 2d6f 7061 6369 7479 3a31 3b73 7472 6f6b  -opacity:1;strok
+00003710: 653a 2330 3030 3030 303b 7374 726f 6b65  e:#000000;stroke
+00003720: 2d77 6964 7468 3a30 3b73 7472 6f6b 652d  -width:0;stroke-
+00003730: 6c69 6e65 6361 703a 726f 756e 643b 7374  linecap:round;st
+00003740: 726f 6b65 2d6c 696e 656a 6f69 6e3a 726f  roke-linejoin:ro
+00003750: 756e 643b 7374 726f 6b65 2d6d 6974 6572  und;stroke-miter
+00003760: 6c69 6d69 743a 343b 7374 726f 6b65 2d64  limit:4;stroke-d
+00003770: 6173 6861 7272 6179 3a6e 6f6e 6522 0a20  asharray:none". 
+00003780: 2020 2020 2020 696e 6b73 6361 7065 3a6c        inkscape:l
+00003790: 6162 656c 3d22 4172 726f 7722 0a20 2020  abel="Arrow".   
+000037a0: 2020 2020 696e 6b73 6361 7065 3a74 7261      inkscape:tra
+000037b0: 6e73 666f 726d 2d63 656e 7465 722d 793d  nsform-center-y=
+000037c0: 222d 302e 3030 3938 3533 3232 3133 220a  "-0.0098532213".
+000037d0: 2020 2020 2020 2064 3d22 6d20 3335 2e37         d="m 35.7
+000037e0: 3338 3431 352c 3332 2e31 3932 3238 3420  38415,32.192284 
+000037f0: 2d30 2e34 3332 3436 312c 302e 3234 3838  -0.432461,0.2488
+00003800: 3033 2030 2e36 3438 3638 392c 2d31 2e35  03 0.648689,-1.5
+00003810: 3232 3337 3520 302e 3634 3836 3838 2c2d  22375 0.648688,-
+00003820: 312e 3532 3233 3736 2030 2e36 3438 3638  1.522376 0.64868
+00003830: 342c 302e 3737 3539 3638 2030 2e36 3438  4,0.775968 0.648
+00003840: 3638 372c 302e 3737 3539 3637 202d 302e  687,0.775967 -0.
+00003850: 3433 3231 382c 302e 3234 3836 3435 220a  43218,0.248645".
+00003860: 2020 2020 2020 2073 6f64 6970 6f64 693a         sodipodi:
+00003870: 6e6f 6465 7479 7065 733d 2263 6363 6363  nodetypes="ccccc
+00003880: 6363 220a 2020 2020 2020 2073 6f64 6970  cc".       sodip
+00003890: 6f64 693a 696e 7365 6e73 6974 6976 653d  odi:insensitive=
+000038a0: 2274 7275 6522 202f 3e0a 2020 2020 3c70  "true" />.    <p
+000038b0: 6174 680a 2020 2020 2020 2069 643d 2270  ath.       id="p
+000038c0: 6174 6837 3532 3322 0a20 2020 2020 2020  ath7523".       
+000038d0: 7374 796c 653d 2264 6973 706c 6179 3a69  style="display:i
+000038e0: 6e6c 696e 653b 6f70 6163 6974 793a 313b  nline;opacity:1;
+000038f0: 6669 6c6c 3a6e 6f6e 653b 7374 726f 6b65  fill:none;stroke
+00003900: 3a23 3030 3030 3030 3b73 7472 6f6b 652d  :#000000;stroke-
+00003910: 7769 6474 683a 302e 313b 7374 726f 6b65  width:0.1;stroke
+00003920: 2d6c 696e 6563 6170 3a72 6f75 6e64 3b73  -linecap:round;s
+00003930: 7472 6f6b 652d 6c69 6e65 6a6f 696e 3a72  troke-linejoin:r
+00003940: 6f75 6e64 3b73 7472 6f6b 652d 6d69 7465  ound;stroke-mite
+00003950: 726c 696d 6974 3a34 3b73 7472 6f6b 652d  rlimit:4;stroke-
+00003960: 6461 7368 6172 7261 793a 6e6f 6e65 220a  dasharray:none".
+00003970: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+00003980: 6c61 6265 6c3d 2241 7272 6f77 220a 2020  label="Arrow".  
+00003990: 2020 2020 2069 6e6b 7363 6170 653a 7472       inkscape:tr
+000039a0: 616e 7366 6f72 6d2d 6365 6e74 6572 2d79  ansform-center-y
+000039b0: 3d22 2d30 2e30 3039 3835 3332 3231 3322  ="-0.0098532213"
+000039c0: 0a20 2020 2020 2020 643d 226d 2033 352e  .       d="m 35.
+000039d0: 3733 3834 3135 2c33 322e 3139 3232 3834  738415,32.192284
+000039e0: 202d 302e 3433 3234 3631 2c30 2e32 3438   -0.432461,0.248
+000039f0: 3830 3320 302e 3634 3836 3839 2c2d 312e  803 0.648689,-1.
+00003a00: 3532 3233 3735 2030 2e36 3438 3638 382c  522375 0.648688,
+00003a10: 2d31 2e35 3232 3337 3620 302e 3634 3836  -1.522376 0.6486
+00003a20: 3834 2c30 2e37 3735 3936 3820 302e 3634  84,0.775968 0.64
+00003a30: 3836 3837 2c30 2e37 3735 3936 3720 2d30  8687,0.775967 -0
+00003a40: 2e34 3332 3138 2c30 2e32 3438 3634 3522  .43218,0.248645"
+00003a50: 0a20 2020 2020 2020 736f 6469 706f 6469  .       sodipodi
+00003a60: 3a6e 6f64 6574 7970 6573 3d22 6363 6363  :nodetypes="cccc
+00003a70: 6363 6322 0a20 2020 2020 2020 736f 6469  ccc".       sodi
+00003a80: 706f 6469 3a69 6e73 656e 7369 7469 7665  podi:insensitive
+00003a90: 3d22 7472 7565 2220 2f3e 0a20 2020 203c  ="true" />.    <
+00003aa0: 7061 7468 0a20 2020 2020 2020 7374 796c  path.       styl
+00003ab0: 653d 2264 6973 706c 6179 3a69 6e6c 696e  e="display:inlin
+00003ac0: 653b 6669 6c6c 3a6e 6f6e 653b 7374 726f  e;fill:none;stro
+00003ad0: 6b65 3a23 3030 3030 3030 3b73 7472 6f6b  ke:#000000;strok
+00003ae0: 652d 7769 6474 683a 302e 313b 7374 726f  e-width:0.1;stro
+00003af0: 6b65 2d6c 696e 6563 6170 3a62 7574 743b  ke-linecap:butt;
+00003b00: 7374 726f 6b65 2d6c 696e 656a 6f69 6e3a  stroke-linejoin:
+00003b10: 6d69 7465 723b 7374 726f 6b65 2d6d 6974  miter;stroke-mit
+00003b20: 6572 6c69 6d69 743a 343b 7374 726f 6b65  erlimit:4;stroke
+00003b30: 2d64 6173 6861 7272 6179 3a30 2e30 352c  -dasharray:0.05,
+00003b40: 2030 2e30 353b 7374 726f 6b65 2d64 6173   0.05;stroke-das
+00003b50: 686f 6666 7365 743a 303b 7374 726f 6b65  hoffset:0;stroke
+00003b60: 2d6f 7061 6369 7479 3a31 3b6d 6172 6b65  -opacity:1;marke
+00003b70: 722d 656e 643a 7572 6c28 2341 7272 6f77  r-end:url(#Arrow
+00003b80: 314c 656e 6429 220a 2020 2020 2020 2064  1Lend)".       d
+00003b90: 3d22 6d20 3133 2e33 3930 3335 362c 3138  ="m 13.390356,18
+00003ba0: 2e32 3937 3034 3620 6320 302c 3020 322e  .297046 c 0,0 2.
+00003bb0: 3737 3635 3637 2c2d 3133 2e38 3333 3231  776567,-13.83321
+00003bc0: 3537 2036 2e33 3235 3737 352c 2d31 352e  57 6.325775,-15.
+00003bd0: 3935 3733 3834 3720 302e 3535 3437 372c  9573847 0.55477,
+00003be0: 2d30 2e33 3332 3032 3520 312e 3132 3834  -0.332025 1.1284
+00003bf0: 3137 2c2d 302e 3337 3739 3732 2031 2e37  17,-0.377972 1.7
+00003c00: 3133 3238 392c 2d30 2e30 3430 3320 4320  13289,-0.0403 C 
+00003c10: 3235 2e37 3536 3037 392c 342e 3739 3733  25.756079,4.7973
+00003c20: 3632 3320 3235 2c32 342e 3939 3938 3738  623 25,24.999878
+00003c30: 2032 352c 3234 2e39 3939 3837 3820 6d20   25,24.999878 m 
+00003c40: 302c 3020 6320 302c 3020 2d30 2e37 3536  0,0 c 0,0 -0.756
+00003c50: 3037 392c 3230 2e32 3032 3531 3520 332e  079,20.202515 3.
+00003c60: 3537 3035 3831 2c32 322e 3730 3035 3132  570581,22.700512
+00003c70: 2034 2e33 3236 3635 392c 322e 3439 3739   4.326659,2.4979
+00003c80: 3939 2038 2e30 3339 3036 342c 2d31 352e  99 8.039064,-15.
+00003c90: 3939 3736 3739 2038 2e30 3339 3036 342c  997679 8.039064,
+00003ca0: 2d31 352e 3939 3736 3739 220a 2020 2020  -15.997679".    
+00003cb0: 2020 2069 643d 2270 6174 6833 3430 3239     id="path34029
+00003cc0: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
+00003cd0: 653a 6c61 6265 6c3d 2243 7572 7665 220a  e:label="Curve".
+00003ce0: 2020 2020 2020 2073 6f64 6970 6f64 693a         sodipodi:
+00003cf0: 6e6f 6465 7479 7065 733d 2263 7373 6363  nodetypes="csscc
+00003d00: 7363 220a 2020 2020 2020 2073 6f64 6970  sc".       sodip
+00003d10: 6f64 693a 696e 7365 6e73 6974 6976 653d  odi:insensitive=
+00003d20: 2274 7275 6522 202f 3e0a 2020 3c2f 673e  "true" />.  </g>
+00003d30: 0a20 203c 6d65 7461 6461 7461 0a20 2020  .  <metadata.   
+00003d40: 2020 6964 3d22 6d65 7461 6461 7461 3839    id="metadata89
+00003d50: 3922 3e0a 2020 2020 3c72 6466 3a52 4446  9">.    <rdf:RDF
+00003d60: 3e0a 2020 2020 2020 3c63 633a 576f 726b  >.      <cc:Work
+00003d70: 0a20 2020 2020 2020 2020 7264 663a 6162  .         rdf:ab
+00003d80: 6f75 743d 2222 3e0a 2020 2020 2020 2020  out="">.        
+00003d90: 3c64 633a 7469 746c 653e 5369 676e 616c  <dc:title>Signal
+00003da0: 797a 6572 2042 616e 6e65 723c 2f64 633a  yzer Banner</dc:
+00003db0: 7469 746c 653e 0a20 2020 2020 2020 203c  title>.        <
+00003dc0: 6463 3a64 6174 653e 3230 3232 2d30 312d  dc:date>2022-01-
+00003dd0: 3037 3c2f 6463 3a64 6174 653e 0a20 2020  07</dc:date>.   
+00003de0: 2020 2020 203c 6463 3a63 7265 6174 6f72       <dc:creator
+00003df0: 3e0a 2020 2020 2020 2020 2020 3c63 633a  >.          <cc:
+00003e00: 4167 656e 743e 0a20 2020 2020 2020 2020  Agent>.         
+00003e10: 2020 203c 6463 3a74 6974 6c65 3e4a 6f63     <dc:title>Joc
+00003e20: 6865 6e20 4765 7268 6165 7573 7365 723c  hen Gerhaeusser<
+00003e30: 2f64 633a 7469 746c 653e 0a20 2020 2020  /dc:title>.     
+00003e40: 2020 2020 203c 2f63 633a 4167 656e 743e       </cc:Agent>
+00003e50: 0a20 2020 2020 2020 203c 2f64 633a 6372  .        </dc:cr
+00003e60: 6561 746f 723e 0a20 2020 2020 2020 203c  eator>.        <
+00003e70: 6363 3a6c 6963 656e 7365 0a20 2020 2020  cc:license.     
+00003e80: 2020 2020 2020 7264 663a 7265 736f 7572        rdf:resour
+00003e90: 6365 3d22 6874 7470 3a2f 2f63 7265 6174  ce="http://creat
+00003ea0: 6976 6563 6f6d 6d6f 6e73 2e6f 7267 2f6c  ivecommons.org/l
+00003eb0: 6963 656e 7365 732f 6279 2d6e 632d 7361  icenses/by-nc-sa
+00003ec0: 2f34 2e30 2f22 202f 3e0a 2020 2020 2020  /4.0/" />.      
+00003ed0: 2020 3c64 633a 6465 7363 7269 7074 696f    <dc:descriptio
+00003ee0: 6e3e 5369 676e 616c 797a 6572 2042 616e  n>Signalyzer Ban
+00003ef0: 6e65 723c 2f64 633a 6465 7363 7269 7074  ner</dc:descript
+00003f00: 696f 6e3e 0a20 2020 2020 2020 203c 6463  ion>.        <dc
+00003f10: 3a72 6967 6874 733e 0a20 2020 2020 2020  :rights>.       
+00003f20: 2020 203c 6363 3a41 6765 6e74 3e0a 2020     <cc:Agent>.  
+00003f30: 2020 2020 2020 2020 2020 3c64 633a 7469            <dc:ti
+00003f40: 746c 653e 416c 6c20 5269 6768 7473 2072  tle>All Rights r
+00003f50: 6573 6572 7665 642e 3c2f 6463 3a74 6974  eserved.</dc:tit
+00003f60: 6c65 3e0a 2020 2020 2020 2020 2020 3c2f  le>.          </
+00003f70: 6363 3a41 6765 6e74 3e0a 2020 2020 2020  cc:Agent>.      
+00003f80: 2020 3c2f 6463 3a72 6967 6874 733e 0a20    </dc:rights>. 
+00003f90: 2020 2020 203c 2f63 633a 576f 726b 3e0a       </cc:Work>.
+00003fa0: 2020 2020 2020 3c63 633a 4c69 6365 6e73        <cc:Licens
+00003fb0: 650a 2020 2020 2020 2020 2072 6466 3a61  e.         rdf:a
+00003fc0: 626f 7574 3d22 6874 7470 3a2f 2f63 7265  bout="http://cre
+00003fd0: 6174 6976 6563 6f6d 6d6f 6e73 2e6f 7267  ativecommons.org
+00003fe0: 2f6c 6963 656e 7365 732f 6279 2d6e 632d  /licenses/by-nc-
+00003ff0: 7361 2f34 2e30 2f22 3e0a 2020 2020 2020  sa/4.0/">.      
+00004000: 2020 3c63 633a 7065 726d 6974 730a 2020    <cc:permits.  
+00004010: 2020 2020 2020 2020 2072 6466 3a72 6573           rdf:res
+00004020: 6f75 7263 653d 2268 7474 703a 2f2f 6372  ource="http://cr
+00004030: 6561 7469 7665 636f 6d6d 6f6e 732e 6f72  eativecommons.or
+00004040: 672f 6e73 2352 6570 726f 6475 6374 696f  g/ns#Reproductio
+00004050: 6e22 202f 3e0a 2020 2020 2020 2020 3c63  n" />.        <c
+00004060: 633a 7065 726d 6974 730a 2020 2020 2020  c:permits.      
+00004070: 2020 2020 2072 6466 3a72 6573 6f75 7263       rdf:resourc
+00004080: 653d 2268 7474 703a 2f2f 6372 6561 7469  e="http://creati
+00004090: 7665 636f 6d6d 6f6e 732e 6f72 672f 6e73  vecommons.org/ns
+000040a0: 2344 6973 7472 6962 7574 696f 6e22 202f  #Distribution" /
+000040b0: 3e0a 2020 2020 2020 2020 3c63 633a 7265  >.        <cc:re
+000040c0: 7175 6972 6573 0a20 2020 2020 2020 2020  quires.         
+000040d0: 2020 7264 663a 7265 736f 7572 6365 3d22    rdf:resource="
+000040e0: 6874 7470 3a2f 2f63 7265 6174 6976 6563  http://creativec
+000040f0: 6f6d 6d6f 6e73 2e6f 7267 2f6e 7323 4e6f  ommons.org/ns#No
+00004100: 7469 6365 2220 2f3e 0a20 2020 2020 2020  tice" />.       
+00004110: 203c 6363 3a72 6571 7569 7265 730a 2020   <cc:requires.  
+00004120: 2020 2020 2020 2020 2072 6466 3a72 6573           rdf:res
+00004130: 6f75 7263 653d 2268 7474 703a 2f2f 6372  ource="http://cr
+00004140: 6561 7469 7665 636f 6d6d 6f6e 732e 6f72  eativecommons.or
+00004150: 672f 6e73 2341 7474 7269 6275 7469 6f6e  g/ns#Attribution
+00004160: 2220 2f3e 0a20 2020 2020 2020 203c 6363  " />.        <cc
+00004170: 3a70 726f 6869 6269 7473 0a20 2020 2020  :prohibits.     
+00004180: 2020 2020 2020 7264 663a 7265 736f 7572        rdf:resour
+00004190: 6365 3d22 6874 7470 3a2f 2f63 7265 6174  ce="http://creat
+000041a0: 6976 6563 6f6d 6d6f 6e73 2e6f 7267 2f6e  ivecommons.org/n
+000041b0: 7323 436f 6d6d 6572 6369 616c 5573 6522  s#CommercialUse"
+000041c0: 202f 3e0a 2020 2020 2020 2020 3c63 633a   />.        <cc:
+000041d0: 7065 726d 6974 730a 2020 2020 2020 2020  permits.        
+000041e0: 2020 2072 6466 3a72 6573 6f75 7263 653d     rdf:resource=
+000041f0: 2268 7474 703a 2f2f 6372 6561 7469 7665  "http://creative
+00004200: 636f 6d6d 6f6e 732e 6f72 672f 6e73 2344  commons.org/ns#D
+00004210: 6572 6976 6174 6976 6557 6f72 6b73 2220  erivativeWorks" 
+00004220: 2f3e 0a20 2020 2020 2020 203c 6363 3a72  />.        <cc:r
+00004230: 6571 7569 7265 730a 2020 2020 2020 2020  equires.        
+00004240: 2020 2072 6466 3a72 6573 6f75 7263 653d     rdf:resource=
+00004250: 2268 7474 703a 2f2f 6372 6561 7469 7665  "http://creative
+00004260: 636f 6d6d 6f6e 732e 6f72 672f 6e73 2353  commons.org/ns#S
+00004270: 6861 7265 416c 696b 6522 202f 3e0a 2020  hareAlike" />.  
+00004280: 2020 2020 3c2f 6363 3a4c 6963 656e 7365      </cc:License
+00004290: 3e0a 2020 2020 3c2f 7264 663a 5244 463e  >.    </rdf:RDF>
+000042a0: 0a20 203c 2f6d 6574 6164 6174 613e 0a20  .  </metadata>. 
+000042b0: 203c 670a 2020 2020 2069 6e6b 7363 6170   <g.     inkscap
+000042c0: 653a 6772 6f75 706d 6f64 653d 226c 6179  e:groupmode="lay
+000042d0: 6572 220a 2020 2020 2069 643d 226c 6179  er".     id="lay
+000042e0: 6572 3422 0a20 2020 2020 696e 6b73 6361  er4".     inksca
+000042f0: 7065 3a6c 6162 656c 3d22 5465 7874 220a  pe:label="Text".
+00004300: 2020 2020 2073 7479 6c65 3d22 6469 7370       style="disp
+00004310: 6c61 793a 6e6f 6e65 220a 2020 2020 2073  lay:none".     s
+00004320: 6f64 6970 6f64 693a 696e 7365 6e73 6974  odipodi:insensit
+00004330: 6976 653d 2274 7275 6522 3e0a 2020 2020  ive="true">.    
+00004340: 3c74 6578 740a 2020 2020 2020 2078 6d6c  <text.       xml
+00004350: 3a73 7061 6365 3d22 7072 6573 6572 7665  :space="preserve
+00004360: 220a 2020 2020 2020 2073 7479 6c65 3d22  ".       style="
+00004370: 666f 6e74 2d73 7479 6c65 3a6e 6f72 6d61  font-style:norma
+00004380: 6c3b 666f 6e74 2d76 6172 6961 6e74 3a6e  l;font-variant:n
+00004390: 6f72 6d61 6c3b 666f 6e74 2d77 6569 6768  ormal;font-weigh
+000043a0: 743a 626f 6c64 3b66 6f6e 742d 7374 7265  t:bold;font-stre
+000043b0: 7463 683a 6e6f 726d 616c 3b66 6f6e 742d  tch:normal;font-
+000043c0: 7369 7a65 3a34 2e39 3338 3839 7078 3b6c  size:4.93889px;l
+000043d0: 696e 652d 6865 6967 6874 3a31 2e32 353b  ine-height:1.25;
+000043e0: 666f 6e74 2d66 616d 696c 793a 7361 6e73  font-family:sans
+000043f0: 2d73 6572 6966 3b2d 696e 6b73 6361 7065  -serif;-inkscape
+00004400: 2d66 6f6e 742d 7370 6563 6966 6963 6174  -font-specificat
+00004410: 696f 6e3a 2773 616e 732d 7365 7269 6620  ion:'sans-serif 
+00004420: 426f 6c64 273b 7465 7874 2d61 6c69 676e  Bold';text-align
+00004430: 3a63 656e 7465 723b 7465 7874 2d61 6e63  :center;text-anc
+00004440: 686f 723a 6d69 6464 6c65 3b66 696c 6c3a  hor:middle;fill:
+00004450: 2330 3733 3938 343b 7374 726f 6b65 2d77  #073984;stroke-w
+00004460: 6964 7468 3a30 2e32 3634 3538 3322 0a20  idth:0.264583". 
+00004470: 2020 2020 2020 783d 2231 352e 3237 3433        x="15.2743
+00004480: 3532 220a 2020 2020 2020 2079 3d22 3436  52".       y="46
+00004490: 2e39 3537 3538 3422 0a20 2020 2020 2020  .957584".       
+000044a0: 6964 3d22 7465 7874 3839 3736 220a 2020  id="text8976".  
+000044b0: 2020 2020 2069 6e6b 7363 6170 653a 6c61       inkscape:la
+000044c0: 6265 6c3d 2241 6e61 6c79 7a65 7222 0a20  bel="Analyzer". 
+000044d0: 2020 2020 2020 736f 6469 706f 6469 3a69        sodipodi:i
+000044e0: 6e73 656e 7369 7469 7665 3d22 7472 7565  nsensitive="true
+000044f0: 223e 3c74 7370 616e 0a20 2020 2020 2020  "><tspan.       
+00004500: 2020 736f 6469 706f 6469 3a72 6f6c 653d    sodipodi:role=
+00004510: 226c 696e 6522 0a20 2020 2020 2020 2020  "line".         
+00004520: 7374 796c 653d 2266 6f6e 742d 7374 796c  style="font-styl
+00004530: 653a 6e6f 726d 616c 3b66 6f6e 742d 7661  e:normal;font-va
+00004540: 7269 616e 743a 6e6f 726d 616c 3b66 6f6e  riant:normal;fon
+00004550: 742d 7765 6967 6874 3a62 6f6c 643b 666f  t-weight:bold;fo
+00004560: 6e74 2d73 7472 6574 6368 3a6e 6f72 6d61  nt-stretch:norma
+00004570: 6c3b 666f 6e74 2d73 697a 653a 342e 3933  l;font-size:4.93
+00004580: 3838 3970 783b 666f 6e74 2d66 616d 696c  889px;font-famil
+00004590: 793a 7361 6e73 2d73 6572 6966 3b2d 696e  y:sans-serif;-in
+000045a0: 6b73 6361 7065 2d66 6f6e 742d 7370 6563  kscape-font-spec
+000045b0: 6966 6963 6174 696f 6e3a 2773 616e 732d  ification:'sans-
+000045c0: 7365 7269 6620 426f 6c64 273b 7465 7874  serif Bold';text
+000045d0: 2d61 6c69 676e 3a63 656e 7465 723b 7465  -align:center;te
+000045e0: 7874 2d61 6e63 686f 723a 6d69 6464 6c65  xt-anchor:middle
+000045f0: 3b66 696c 6c3a 2330 3733 3938 343b 7374  ;fill:#073984;st
+00004600: 726f 6b65 2d77 6964 7468 3a30 2e32 3634  roke-width:0.264
+00004610: 3538 3322 0a20 2020 2020 2020 2020 783d  583".         x=
+00004620: 2231 352e 3237 3433 3532 220a 2020 2020  "15.274352".    
+00004630: 2020 2020 2079 3d22 3436 2e39 3537 3538       y="46.95758
+00004640: 3422 0a20 2020 2020 2020 2020 6964 3d22  4".         id="
+00004650: 7473 7061 6e31 3132 3536 223e 416e 616c  tspan11256">Anal
+00004660: 797a 6572 3c2f 7473 7061 6e3e 3c2f 7465  yzer</tspan></te
+00004670: 7874 3e0a 2020 2020 3c74 6578 740a 2020  xt>.    <text.  
+00004680: 2020 2020 2078 6d6c 3a73 7061 6365 3d22       xml:space="
+00004690: 7072 6573 6572 7665 220a 2020 2020 2020  preserve".      
+000046a0: 2073 7479 6c65 3d22 666f 6e74 2d73 697a   style="font-siz
+000046b0: 653a 342e 3933 3838 3970 783b 6c69 6e65  e:4.93889px;line
+000046c0: 2d68 6569 6768 743a 312e 3235 3b66 6f6e  -height:1.25;fon
+000046d0: 742d 6661 6d69 6c79 3a73 616e 732d 7365  t-family:sans-se
+000046e0: 7269 663b 2d69 6e6b 7363 6170 652d 666f  rif;-inkscape-fo
+000046f0: 6e74 2d73 7065 6369 6669 6361 7469 6f6e  nt-specification
+00004700: 3a27 7361 6e73 2d73 6572 6966 2c20 4e6f  :'sans-serif, No
+00004710: 726d 616c 273b 6669 6c6c 3a23 3037 3339  rmal';fill:#0739
+00004720: 3834 3b73 7472 6f6b 652d 7769 6474 683a  84;stroke-width:
+00004730: 302e 3236 3435 3833 220a 2020 2020 2020  0.264583".      
+00004740: 2078 3d22 3430 2e33 3039 3331 3122 0a20   x="40.309311". 
+00004750: 2020 2020 2020 793d 2235 2e37 3238 3930        y="5.72890
+00004760: 3632 220a 2020 2020 2020 2069 643d 2274  62".       id="t
+00004770: 6578 7432 3834 3722 0a20 2020 2020 2020  ext2847".       
+00004780: 696e 6b73 6361 7065 3a6c 6162 656c 3d22  inkscape:label="
+00004790: 5369 676e 616c 220a 2020 2020 2020 2073  Signal".       s
+000047a0: 6f64 6970 6f64 693a 696e 7365 6e73 6974  odipodi:insensit
+000047b0: 6976 653d 2274 7275 6522 3e3c 7473 7061  ive="true"><tspa
+000047c0: 6e0a 2020 2020 2020 2020 2073 6f64 6970  n.         sodip
+000047d0: 6f64 693a 726f 6c65 3d22 6c69 6e65 220a  odi:role="line".
+000047e0: 2020 2020 2020 2020 2069 643d 2274 7370           id="tsp
+000047f0: 616e 3238 3435 220a 2020 2020 2020 2020  an2845".        
+00004800: 2073 7479 6c65 3d22 666f 6e74 2d73 7479   style="font-sty
+00004810: 6c65 3a6e 6f72 6d61 6c3b 666f 6e74 2d76  le:normal;font-v
+00004820: 6172 6961 6e74 3a6e 6f72 6d61 6c3b 666f  ariant:normal;fo
+00004830: 6e74 2d77 6569 6768 743a 626f 6c64 3b66  nt-weight:bold;f
+00004840: 6f6e 742d 7374 7265 7463 683a 6e6f 726d  ont-stretch:norm
+00004850: 616c 3b66 6f6e 742d 7369 7a65 3a34 2e39  al;font-size:4.9
+00004860: 3338 3839 7078 3b66 6f6e 742d 6661 6d69  3889px;font-fami
+00004870: 6c79 3a73 616e 732d 7365 7269 663b 2d69  ly:sans-serif;-i
+00004880: 6e6b 7363 6170 652d 666f 6e74 2d73 7065  nkscape-font-spe
+00004890: 6369 6669 6361 7469 6f6e 3a27 7361 6e73  cification:'sans
+000048a0: 2d73 6572 6966 2042 6f6c 6427 3b74 6578  -serif Bold';tex
+000048b0: 742d 616c 6967 6e3a 6365 6e74 6572 3b74  t-align:center;t
+000048c0: 6578 742d 616e 6368 6f72 3a6d 6964 646c  ext-anchor:middl
+000048d0: 653b 6669 6c6c 3a23 3037 3339 3834 3b73  e;fill:#073984;s
+000048e0: 7472 6f6b 652d 7769 6474 683a 302e 3236  troke-width:0.26
+000048f0: 3435 3833 220a 2020 2020 2020 2020 2078  4583".         x
+00004900: 3d22 3430 2e33 3039 3331 3122 0a20 2020  ="40.309311".   
+00004910: 2020 2020 2020 793d 2235 2e37 3238 3930        y="5.72890
+00004920: 3632 223e 5369 676e 616c 3c2f 7473 7061  62">Signal</tspa
+00004930: 6e3e 3c2f 7465 7874 3e0a 2020 3c2f 673e  n></text>.  </g>
+00004940: 0a20 203c 670a 2020 2020 2069 643d 226c  .  <g.     id="l
+00004950: 6179 6572 3522 0a20 2020 2020 696e 6b73  ayer5".     inks
+00004960: 6361 7065 3a6c 6162 656c 3d22 4261 6e6e  cape:label="Bann
+00004970: 6572 220a 2020 2020 2073 7479 6c65 3d22  er".     style="
+00004980: 6469 7370 6c61 793a 696e 6c69 6e65 220a  display:inline".
+00004990: 2020 2020 2069 6e6b 7363 6170 653a 6772       inkscape:gr
+000049a0: 6f75 706d 6f64 653d 226c 6179 6572 220a  oupmode="layer".
+000049b0: 2020 2020 2073 6f64 6970 6f64 693a 696e       sodipodi:in
+000049c0: 7365 6e73 6974 6976 653d 2274 7275 6522  sensitive="true"
+000049d0: 3e0a 2020 2020 3c74 6578 740a 2020 2020  >.    <text.    
+000049e0: 2020 2078 6d6c 3a73 7061 6365 3d22 7072     xml:space="pr
+000049f0: 6573 6572 7665 220a 2020 2020 2020 2073  eserve".       s
+00004a00: 7479 6c65 3d22 666f 6e74 2d73 697a 653a  tyle="font-size:
+00004a10: 3136 2e39 3333 3370 783b 6c69 6e65 2d68  16.9333px;line-h
+00004a20: 6569 6768 743a 312e 3235 3b66 6f6e 742d  eight:1.25;font-
+00004a30: 6661 6d69 6c79 3a73 616e 732d 7365 7269  family:sans-seri
+00004a40: 663b 2d69 6e6b 7363 6170 652d 666f 6e74  f;-inkscape-font
+00004a50: 2d73 7065 6369 6669 6361 7469 6f6e 3a27  -specification:'
+00004a60: 7361 6e73 2d73 6572 6966 2c20 4e6f 726d  sans-serif, Norm
+00004a70: 616c 273b 6669 6c6c 3a23 3037 3339 3834  al';fill:#073984
+00004a80: 3b73 7472 6f6b 652d 7769 6474 683a 302e  ;stroke-width:0.
+00004a90: 3236 3435 3833 220a 2020 2020 2020 2078  264583".       x
+00004aa0: 3d22 3130 362e 3438 3137 3422 0a20 2020  ="106.48174".   
+00004ab0: 2020 2020 793d 2232 392e 3038 3732 3522      y="29.08725"
+00004ac0: 0a20 2020 2020 2020 6964 3d22 7465 7874  .       id="text
+00004ad0: 3238 3437 2d38 220a 2020 2020 2020 2069  2847-8".       i
+00004ae0: 6e6b 7363 6170 653a 6c61 6265 6c3d 2253  nkscape:label="S
+00004af0: 6967 6e61 6c79 7a65 7222 0a20 2020 2020  ignalyzer".     
+00004b00: 2020 736f 6469 706f 6469 3a69 6e73 656e    sodipodi:insen
+00004b10: 7369 7469 7665 3d22 7472 7565 223e 3c74  sitive="true"><t
+00004b20: 7370 616e 0a20 2020 2020 2020 2020 736f  span.         so
+00004b30: 6469 706f 6469 3a72 6f6c 653d 226c 696e  dipodi:role="lin
+00004b40: 6522 0a20 2020 2020 2020 2020 6964 3d22  e".         id="
+00004b50: 7473 7061 6e32 3834 352d 3522 0a20 2020  tspan2845-5".   
+00004b60: 2020 2020 2020 7374 796c 653d 2266 6f6e        style="fon
+00004b70: 742d 7374 796c 653a 6e6f 726d 616c 3b66  t-style:normal;f
+00004b80: 6f6e 742d 7661 7269 616e 743a 6e6f 726d  ont-variant:norm
+00004b90: 616c 3b66 6f6e 742d 7765 6967 6874 3a62  al;font-weight:b
+00004ba0: 6f6c 643b 666f 6e74 2d73 7472 6574 6368  old;font-stretch
+00004bb0: 3a6e 6f72 6d61 6c3b 666f 6e74 2d73 697a  :normal;font-siz
+00004bc0: 653a 3136 2e39 3333 3370 783b 666f 6e74  e:16.9333px;font
+00004bd0: 2d66 616d 696c 793a 7361 6e73 2d73 6572  -family:sans-ser
+00004be0: 6966 3b2d 696e 6b73 6361 7065 2d66 6f6e  if;-inkscape-fon
+00004bf0: 742d 7370 6563 6966 6963 6174 696f 6e3a  t-specification:
+00004c00: 2773 616e 732d 7365 7269 6620 426f 6c64  'sans-serif Bold
+00004c10: 273b 7465 7874 2d61 6c69 676e 3a63 656e  ';text-align:cen
+00004c20: 7465 723b 7465 7874 2d61 6e63 686f 723a  ter;text-anchor:
+00004c30: 6d69 6464 6c65 3b66 696c 6c3a 2330 3733  middle;fill:#073
+00004c40: 3938 343b 7374 726f 6b65 2d77 6964 7468  984;stroke-width
+00004c50: 3a30 2e32 3634 3538 3322 0a20 2020 2020  :0.264583".     
+00004c60: 2020 2020 783d 2231 3036 2e34 3831 3734      x="106.48174
+00004c70: 220a 2020 2020 2020 2020 2079 3d22 3239  ".         y="29
+00004c80: 2e30 3837 3235 223e 5369 676e 616c 797a  .08725">Signalyz
+00004c90: 6572 3c2f 7473 7061 6e3e 3c2f 7465 7874  er</tspan></text
+00004ca0: 3e0a 2020 3c2f 673e 0a3c 2f73 7667 3e0a  >.  </g>.</svg>.
```

### Comparing `signalyzer-0.2.4/docs/Makefile` & `signalyzer-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `signalyzer-0.2.4/docs/annex/contributing.rst` & `signalyzer-0.3.0/docs/annex/contributing.rst`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-.. _project: https://gitlab.com/signalytics/signalyzer
-.. _issue: https://gitlab.com/signalytics/signalyzer/-/issues
-
-Issue Reports
-=============
-
-Filing an Issue Report
-----------------------
-
-If you encounter a bug, misfeature, or missing feature, please file an `issue`_
-report. We also appreciate reports of incomplete or misleading information in the
-documentation; file those against the "documentation" category.
-
-Don't hesitate to file an `issue`_ report, even if you think I may know about it
-already, or aren't sure of the details. Just give us as much information as you
-have, and if it's already fixed or has already been discussed, I'll add a note
-to that effect in the report.
-
-The `issue`_ tracker should definitely be used for feature requests, it's not
-only for bugs. We track the development in it, so it's the way to be sure the
-developers won't forget about an issue.
-
-Submitting Patches
-------------------
-
-If you develop a bug fix or enhancement, please file that in the `issue`_ tracker
-as well. The `issue`_ tracker allows you to attach files. All patches must be
-offered under the same terms of the license used by the `project`_, so be sure
-you are authorized to give us the patch under those terms.
-
-If you want to discuss your patch before or after developing it, mail to
-jochen_privat@gmx.com. But be sure to file the `issue`_ report as well;
-if the patch is only on the list and not in the `issue`_ tracker, it's likely to
-slip through the cracks.
+.. _project: https://gitlab.com/signalytics/signalyzer
+.. _issue: https://gitlab.com/signalytics/signalyzer/-/issues
+
+Issue Reports
+=============
+
+Filing an Issue Report
+----------------------
+
+If you encounter a bug, misfeature, or missing feature, please file an `issue`_
+report. We also appreciate reports of incomplete or misleading information in the
+documentation; file those against the "documentation" category.
+
+Don't hesitate to file an `issue`_ report, even if you think I may know about it
+already, or aren't sure of the details. Just give us as much information as you
+have, and if it's already fixed or has already been discussed, I'll add a note
+to that effect in the report.
+
+The `issue`_ tracker should definitely be used for feature requests, it's not
+only for bugs. We track the development in it, so it's the way to be sure the
+developers won't forget about an issue.
+
+Submitting Patches
+------------------
+
+If you develop a bug fix or enhancement, please file that in the `issue`_ tracker
+as well. The `issue`_ tracker allows you to attach files. All patches must be
+offered under the same terms of the license used by the `project`_, so be sure
+you are authorized to give us the patch under those terms.
+
+If you want to discuss your patch before or after developing it, mail to
+jochen_privat@gmx.com. But be sure to file the `issue`_ report as well;
+if the patch is only on the list and not in the `issue`_ tracker, it's likely to
+slip through the cracks.
```

### Comparing `signalyzer-0.2.4/docs/api/index.rst` & `signalyzer-0.3.0/docs/api/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,27 @@
 ***
 
 This part of the documentation lists the full API reference of all public
 classes and functions.
 
 .. currentmodule:: signalyzer
 
+Type Hints Support
+==================
+
+.. autoclass:: Number
+
+.. autoclass:: Sample
+
+.. autoclass:: Samples
+
+.. autoclass:: Operand
+
+.. autoclass:: DataFrame
+
 Signal Traces
 =============
 
 Trace
 -----
 
 .. autoclass:: Trace
@@ -81,28 +94,32 @@
 
 SlewRateLimiterTraces
 ---------------------
 
 .. autoclass:: SlewRateLimiterTraces
    :members:
 
-
 ExponentialSmoothingTraces
 --------------------------
 
 .. autoclass:: ExponentialSmoothingTraces
    :members:
 
-
 LinearRegressionTraces
 ----------------------
 
 .. autoclass:: LinearRegressionTraces
    :members:
 
+AlphaBetaFilterTraces
+---------------------
+
+.. autoclass:: AlphaBetaFilterTraces
+   :members:
+
 Representations
 ===============
 
 2D-Point
 --------
 
 .. autoclass:: Point2D
@@ -159,28 +176,29 @@
 
 .. autoclass:: LinearRegression
    :members:
 
 Filtering
 ---------
 
-.. autoclass:: IIRFilter
+.. autoclass:: AlphaBetaFilter
    :members:
 
+.. autoclass:: IIRFilter
+   :members:
 
 State Machines
 ==============
 
 Statemachine
 ------------
 
 .. autoclass:: Statemachine
    :members:
 
-
 Converters
 ==========
 
 as_traces
 ---------
 
 .. autofunction:: as_traces
```

### Comparing `signalyzer-0.2.4/docs/collections/exponential-smoothing-traces.rst` & `signalyzer-0.3.0/docs/collections/exponential-smoothing-traces.rst`

 * *Files 4% similar despite different names*

```diff
@@ -265,14 +265,47 @@
   >>> # trend sign trace by attribute
   >>> traces.trend_sign
   Trace(label='Trace', samples=[])
   >>> # trend sign trace by key
   >>> traces['trend_sign']
   Trace(label='Trace', samples=[])
 
+Trend Inflection Trace
+----------------------
+
+You can get the *trend inflection* :class:`Trace` between the predicted
+*forecast* and the estimated *level* with the
+:attr:`~ExponentialSmoothingTraces.trend_inflection` attribute from the
+:class:`ExponentialSmoothingTraces` collection.
+
+The :class:`Trace` with the *trend sign* :attr:`~Trace.samples` is returned.
+
+  >>> # trend sign trace by attribute
+  >>> traces.trend_inflection
+  Trace(label='Trace', samples=[])
+  >>> # trend sign trace by key
+  >>> traces['trend_inflection']
+  Trace(label='Trace', samples=[])
+
+Error Trace
+-----------
+
+You can get the prognosis *error* :class:`Trace`
+with the :attr:`~ExponentialSmoothingTraces.error` attribute from the
+:class:`ExponentialSmoothingTraces` collection.
+
+The :class:`Trace` with the *error* :attr:`~Trace.samples` is returned.
+
+  >>> # error trace by attribute
+  >>> traces.error
+  Trace(label='Trace', samples=[])
+  >>> # error trace by key
+  >>> traces['error']
+  Trace(label='Trace', samples=[])
+
 Absolute Error Trace
 --------------------
 
 You can get the *absolute error* :class:`Trace` with the
 :attr:`~ExponentialSmoothingTraces.absolute_error` attribute from the
 :class:`ExponentialSmoothingTraces` collection.
```

### Comparing `signalyzer-0.2.4/docs/collections/index.rst` & `signalyzer-0.3.0/docs/collections/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
    :caption: Trace Collections
    :hidden:
 
    vector-traces
    statistics-traces
    set-traces
    slew-rate-limiter-traces
+   alpha-beta-filter-traces
    exponential-smoothing-traces
    linear-regression-traces
 
 Create a Collection of Traces
 -----------------------------
 
 You can create an empty collection of :class:`Traces` by calling the
```

### Comparing `signalyzer-0.2.4/docs/collections/linear-regression-traces.rst` & `signalyzer-0.3.0/docs/collections/linear-regression-traces.rst`

 * *Files identical despite different names*

### Comparing `signalyzer-0.2.4/docs/collections/set-traces.rst` & `signalyzer-0.3.0/docs/collections/set-traces.rst`

 * *Files identical despite different names*

### Comparing `signalyzer-0.2.4/docs/collections/slew-rate-limiter-traces.rst` & `signalyzer-0.3.0/docs/collections/slew-rate-limiter-traces.rst`

 * *Files identical despite different names*

### Comparing `signalyzer-0.2.4/docs/collections/statistics-traces.rst` & `signalyzer-0.3.0/docs/collections/statistics-traces.rst`

 * *Files identical despite different names*

### Comparing `signalyzer-0.2.4/docs/collections/vector-traces.rst` & `signalyzer-0.3.0/docs/collections/vector-traces.rst`

 * *Files 4% similar despite different names*

```diff
@@ -49,42 +49,43 @@
   >>> traces = VectorTraces()
   >>> traces
   VectorTraces(x=Trace(label='Trace', samples=[]),
                y=Trace(label='Trace', samples=[]),
                r=Trace(label='Vector:r', samples=[]),
                phi=Trace(label='Vector:phi', samples=[]),
                theta=Trace(label='Vector:theta', samples=[]),
+               delta_phi=Trace(label='Vector:delta_phi', samples=[]),
                distance=Trace(label='Vector:distance', samples=[]),
                dot=Trace(label='Vector:dot', samples=[]))
 
 Number of Traces
 ----------------
 
 You can get the number of the traces in the :class:`VectorTraces` collection
 with the built-in function :func:`len`.
 
   >>> # number of traces in the collection
   >>> len(traces)
-  7
+  8
 
 Names of the Traces
 -------------------
 
 You can get the :class:`list` with the names of the traces in the
 :class:`VectorTraces` collection.
 
 A :class:`list` with the key names of the traces is returned.
 
   >>> # key names of the traces in the collection
   >>> list(traces)
-  ['x', 'y', 'r', 'phi', 'theta', 'distance', 'dot']
+  ['x', 'y', 'r', 'phi', 'theta', 'delta_phi', 'distance', 'dot']
 
   >>> # key names of the traces in the collection
   >>> list(traces.keys())
-  ['x', 'y', 'r', 'phi', 'theta', 'distance', 'dot']
+  ['x', 'y', 'r', 'phi', 'theta', 'delta_phi', 'distance', 'dot']
 
 x-Coordinate Trace
 ------------------
 
 You can get the vector *x-coordinate* :class:`Trace` with the
 :attr:`~VectorTraces.x` attribute from the :class:`VectorTraces` collection.
 
@@ -158,14 +159,35 @@
   >>> # vector angle trace in degree by attribute
   >>> traces.theta
   Trace(label='Vector:theta', samples=[])
   >>> # vector angle trace in degree by key
   >>> traces['theta']
   Trace(label='Vector:theta', samples=[])
 
+Delta Angle Trace in Radians
+----------------------------
+
+You can get the *delta angle* :class:`Trace` from :math:`-\pi` to :math:`+\pi`
+with the :attr:`~VectorTraces.delta_phi` attribute from the :class:`VectorTraces`
+collection.
+
+The :class:`Trace` with the *delta angles* in radians of the consecutive x,y-points
+computed from the *x-coordinate*, *y-coordinate* :attr:`~Trace.samples` is
+returned.
+
+A positive *delta angle* indicates an anti-clockwise rotation, and a negative
+*delta angle* a clockwise rotation.
+
+  >>> # delta angle trace in radians by attribute
+  >>> traces.delta_phi
+  Trace(label='Vector:delta_phi', samples=[])
+  >>> # delta angle trace in radians by key
+  >>> traces['delta_phi']
+  Trace(label='Vector:delta_phi', samples=[])
+
 Euclidean Distance Trace
 ------------------------
 
 You can get the euclidean *distance* :class:`Trace` with the
 :attr:`~VectorTraces.distance` attribute from the :class:`VectorTraces`
 collection.
```

### Comparing `signalyzer-0.2.4/docs/index.rst` & `signalyzer-0.3.0/docs/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 .. _JupyterLab: https://jupyter.org/
 .. _numpy: https://numpy.org/
 .. _scipy: https://www.scipy.org/
 .. _pandas: https://pandas.pydata.org/docs/
 .. _plotly: https://plotly.com/python/
 .. _dash: https://dash.plotly.com/
+.. _streamlit: https://streamlit.io/
 .. _voila: https://voila.readthedocs.io/
 .. _PyPI package registry: https://gitlab.com/signalytics/signalyzer/-/packages
 .. _PyPI: https://pypi.org/project/signalyzer
 
 .. |status| image:: https://img.shields.io/pypi/status/signalyzer.svg
    :target: https://pypi.org/project/signalyzer
 .. |docs| image:: https://readthedocs.org/projects/signalyzer/badge/?version=latest
@@ -58,20 +59,21 @@
 * slicing of the measured signal
 * evaluate statemachine transitions observed by measured state signal
 
 .. important::
 
   The ``signalyzer`` package is best used within the `JupyterLab`_ web-based
   interactive development environment for Jupyter notebooks or with Plotly
-  `Dash`_ or Jupyter `voila`_ to build standalone web applications and dashboards.
+  `Dash`_, `Streamlit`_  or Jupyter `voila`_ to build standalone web applications
+  and dashboards.
 
 Dependencies
 ------------
 
-The **signalyzer** package runs on `Python 3.9 <https://www.python.org>`_ or
+The **signalyzer** package runs on `Python 3.10 <https://www.python.org>`_ or
 higher, and depends on the external packages
 
 * `numpy`_ for mathematical computations
 * `scipy`_ for signal processing and signal statistics computations
 * `pandas`_ for data import and statistic computations
 * `plotly`_ for visualizations
 
@@ -124,28 +126,28 @@
    :caption: State Machines
    :maxdepth: 3
    :hidden:
 
    statemachine/index
 
 .. toctree::
-   :maxdepth: 4
    :caption: References
+   :maxdepth: 4
    :hidden:
 
    api/index
 
 .. toctree::
-   :maxdepth: 2
    :caption: Annex
+   :maxdepth: 2
    :hidden:
 
    annex/changelog
    annex/license
    annex/contributing
 
 .. toctree::
-   :maxdepth: 1
    :caption: Indexes
+   :maxdepth: 1
    :hidden:
 
    genindex
```

### Comparing `signalyzer-0.2.4/docs/make.bat` & `signalyzer-0.3.0/docs/make.bat`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,29 +7,29 @@
 if "%SPHINXBUILD%" == "" (
 	set SPHINXBUILD=sphinx-build
 )
 set SOURCEDIR=.
 set BUILDDIR=_build
 set SPHINXPROJ=Signalyzer
 
-if "%1" == "" goto help
-
 %SPHINXBUILD% >NUL 2>NUL
 if errorlevel 9009 (
 	echo.
 	echo.The 'sphinx-build' command was not found. Make sure you have Sphinx
 	echo.installed, then set the SPHINXBUILD environment variable to point
 	echo.to the full path of the 'sphinx-build' executable. Alternatively you
 	echo.may add the Sphinx directory to PATH.
 	echo.
 	echo.If you don't have Sphinx installed, grab it from
 	echo.https://www.sphinx-doc.org/
 	exit /b 1
 )
 
+if "%1" == "" goto help
+
 %SPHINXBUILD% -M %1 %SOURCEDIR% %BUILDDIR% %SPHINXOPTS% %O%
 goto end
 
 :help
 %SPHINXBUILD% -M help %SOURCEDIR% %BUILDDIR% %SPHINXOPTS% %O%
 
 :end
```

### Comparing `signalyzer-0.2.4/docs/processing/change-rate-limiting.rst` & `signalyzer-0.3.0/docs/processing/change-rate-limiting.rst`

 * *Files identical despite different names*

### Comparing `signalyzer-0.2.4/docs/processing/clipping.rst` & `signalyzer-0.3.0/docs/processing/clipping.rst`

 * *Files identical despite different names*

### Comparing `signalyzer-0.2.4/docs/processing/dt1-element.rst` & `signalyzer-0.3.0/docs/processing/dt1-element.rst`

 * *Files identical despite different names*

### Comparing `signalyzer-0.2.4/docs/processing/exponential-smoothing.rst` & `signalyzer-0.3.0/docs/processing/exponential-smoothing.rst`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     trend_inflection=Trace(label='Signal:exponential:trend_inflection',
                            samples=[0.0, 1.0, 1.0]),
     error=Trace(label='Signal:exponential:error',
                 samples=[0.0, 1.0, 1.4000000000000001]),
     correction=Trace(label='Signal:exponential:correction',
                      samples=[0.0, 0.3, 0.42000000000000004]),
     absolute_error=Trace(label='Signal:exponential:absolute_error',
-                         samples=[0.0, 0.21, 0.294]),
+                         samples=[0.0, 0.21, 0.44099999999999995]),
     variance=Trace(label='Signal:exponential:variance',
                    samples=[0.0, 0.21, 0.5586]),
     deviation=Trace(label='Signal:exponential:deviation',
                     samples=[0.0, 0.458257569495584, 0.7473954776421918]),
     skew=Trace(label='Signal:exponential:skew',
                    samples=[0.0, 2.182178902359923, 2.9077569539828634]),
     kurtosis=Trace(label='Signal:exponential:kurtosis',
@@ -72,15 +72,15 @@
 Figure
 ------
 
 You can visualize the trace collection with a figure containing the subplots of
 the traces in the collection by calling the method
 :meth:`~ExponentialSmoothingTraces.figure`.
 
-  >>> figure = Trace('Signal', [1, 2, 3]).exponential(0.3).figure()
+  >>> figure = Trace('Signal', range(20)).exponential(0.3).figure()
 
 .. plotly::
 
   from signalyzer import Trace
 
   signal = Trace('Signal', range(20))
   traces = signal.exponential(0.3)
```

### Comparing `signalyzer-0.2.4/docs/processing/iir-filters.rst` & `signalyzer-0.3.0/docs/processing/iir-filters.rst`

 * *Files identical despite different names*

### Comparing `signalyzer-0.2.4/docs/processing/index.rst` & `signalyzer-0.3.0/docs/processing/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
    change-rate-limiting
    slew-rate-limiting
    slew-rate-limiter
    iir-filters
    logic-functions
    pt1-element
    dt1-element
+   alpha-beta-filter
    exponential-smoothing
    window-generator
    moving-events
    moving-differentiation
    moving-averages
    moving-linear-regression
 
@@ -94,14 +95,15 @@
 ---------
 
 .. csv-table::
    :header: "Method", "Name", "Label"
    :widths: 20, 80, 20
    :align: left
 
+   :meth:`~Trace.alpha_beta_filter`, :ref:`Alpha-Beta Filter <alpha-beta filter>`, ``'filter'``
    :meth:`~Trace.exponential`, :ref:`Exponential smoothing <exponential smoothing>`, ``'exponential'``
 
 Moving Window Functions
 -----------------------
 
 .. csv-table::
    :header: "Method", "Name", "Label"
```

### Comparing `signalyzer-0.2.4/docs/processing/logic-functions.rst` & `signalyzer-0.3.0/docs/processing/logic-functions.rst`

 * *Files 8% similar despite different names*

```diff
@@ -103,33 +103,35 @@
 ----------------
 
 .. important::
 
   The *operands* are converted to :class:`int` before the operation is performed.
 
 You can prioritize the ``Truth=1`` values of the **binary** signal
-:attr:`~Trace.samples` of multiple :ref:`signal traces <signal trace>` by
+:attr:`~Trace.samples` from multiple :ref:`signal traces <signal trace>` by
 calling the function :func:`priority` with the iterable *operands* in the
-descending order to prioritize. This means the *highest* priority have the
-``Truth=1`` values of the first provided operand.
+descending order to prioritize them.
+
+This means the *highest* priority have the ``Truth=1`` values of the first
+provided operand.
 
 The lowest priority number is determined by the number of the provided
 *operands*.
 
 A new :class:`Trace` instance *labeled* with the preformed logic function
 ``'Priority'`` is returned containing the priority numbers for the prioritized
-the ``Truth=1`` values of the given *operands*.
+``Truth=1`` values of the given *operands*.
 
-    >>> # prioritize binary signals from left to right in descending order
     >>> signal = Trace('Signal', [-1.0, -0.5, 0.0, 0.5, 1.0])
+    >>> # prioritize binary signals from left to right in descending order
     >>> priority(signal == 0, signal <= 0, signal >= 1)
     Trace(label='Priority', samples=[1, 1, 0, 3, 2])
 
-    >>> # prioritize binary signals starting from 1 as highest priority number
     >>> signal = Trace('Signal', [-1.0, -0.5, 0.0, 0.5, 1.0])
+    >>> # prioritize binary signals starting from 1 as highest priority number
     >>> priority(signal == 0, signal <= 0, signal >= 1, highest=1)
     Trace(label='Priority', samples=[2, 2, 1, 4, 3])
 
 .. note::
 
   The *operands* should have the same length, otherwise only a subset of the
   signal :attr:`~Trace.samples` is returned!
```

### Comparing `signalyzer-0.2.4/docs/processing/moving-averages.rst` & `signalyzer-0.3.0/docs/processing/moving-averages.rst`

 * *Files identical despite different names*

### Comparing `signalyzer-0.2.4/docs/processing/moving-differentiation.rst` & `signalyzer-0.3.0/docs/processing/moving-differentiation.rst`

 * *Files identical despite different names*

### Comparing `signalyzer-0.2.4/docs/processing/moving-events.rst` & `signalyzer-0.3.0/docs/processing/moving-events.rst`

 * *Files identical despite different names*

### Comparing `signalyzer-0.2.4/docs/processing/moving-linear-regression.rst` & `signalyzer-0.3.0/docs/processing/moving-linear-regression.rst`

 * *Files identical despite different names*

### Comparing `signalyzer-0.2.4/docs/processing/pt1-element.rst` & `signalyzer-0.3.0/docs/processing/pt1-element.rst`

 * *Files identical despite different names*

### Comparing `signalyzer-0.2.4/docs/processing/slew-rate-limiter.rst` & `signalyzer-0.3.0/docs/processing/slew-rate-limiter.rst`

 * *Files identical despite different names*

### Comparing `signalyzer-0.2.4/docs/processing/slew-rate-limiting.rst` & `signalyzer-0.3.0/docs/processing/slew-rate-limiting.rst`

 * *Files identical despite different names*

### Comparing `signalyzer-0.2.4/docs/statemachine/index.rst` & `signalyzer-0.3.0/docs/statemachine/index.rst`

 * *Files identical despite different names*

### Comparing `signalyzer-0.2.4/docs/trace/operations.rst` & `signalyzer-0.3.0/docs/trace/operations.rst`

 * *Files identical despite different names*

### Comparing `signalyzer-0.2.4/docs/transformations/arithmetic_operators.rst` & `signalyzer-0.3.0/docs/transformations/arithmetic_operators.rst`

 * *Files identical despite different names*

### Comparing `signalyzer-0.2.4/docs/transformations/assignment_operators.rst` & `signalyzer-0.3.0/docs/transformations/assignment_operators.rst`

 * *Files identical despite different names*

### Comparing `signalyzer-0.2.4/docs/transformations/bitwise_operators.rst` & `signalyzer-0.3.0/docs/transformations/bitwise_operators.rst`

 * *Files identical despite different names*

### Comparing `signalyzer-0.2.4/docs/transformations/comparison_operators.rst` & `signalyzer-0.3.0/docs/transformations/comparison_operators.rst`

 * *Files identical despite different names*

### Comparing `signalyzer-0.2.4/docs/transformations/differentiating_functions.rst` & `signalyzer-0.3.0/docs/transformations/differentiating_functions.rst`

 * *Files identical despite different names*

### Comparing `signalyzer-0.2.4/docs/transformations/index.rst` & `signalyzer-0.3.0/docs/transformations/index.rst`

 * *Files identical despite different names*

### Comparing `signalyzer-0.2.4/docs/transformations/integrating_functions.rst` & `signalyzer-0.3.0/docs/transformations/integrating_functions.rst`

 * *Files identical despite different names*

### Comparing `signalyzer-0.2.4/docs/transformations/mathematical_functions.rst` & `signalyzer-0.3.0/docs/transformations/mathematical_functions.rst`

 * *Files identical despite different names*

### Comparing `signalyzer-0.2.4/docs/transformations/statistics.rst` & `signalyzer-0.3.0/docs/transformations/statistics.rst`

 * *Files identical despite different names*

### Comparing `signalyzer-0.2.4/docs/transformations/trigonometric_functions.rst` & `signalyzer-0.3.0/docs/transformations/trigonometric_functions.rst`

 * *Files 0% similar despite different names*

```diff
@@ -244,15 +244,15 @@
 calling the method :func:`~Trace.asinh`.
 
 A new :class:`Trace` instance *labeled* with the performed transformation
 ``'asinh'`` is returned.
 
   >>> Trace('Signal', [-1, 0, 1]).asinh()
   Trace(label='Signal:asinh',
-        samples=[-0.8813735870195429, 0.0, 0.8813735870195429])
+        samples=[-0.881373587019543, 0.0, 0.881373587019543])
 
 .. plotly::
 
   from signalyzer import Trace
 
   signal = Trace('Signal', [-1, 0, 1])
   trace = signal.asinh()
@@ -269,15 +269,15 @@
 
 A new :class:`Trace` instance *labeled* with the performed transformation
 ``'acosh'`` is returned.
 
   >>> from math import pi
   >>> Trace('Signal', [1, pi/2, pi]).acosh()
   Trace(label='Signal:acosh',
-        samples=[0.0, 1.0232274785475506, 1.811526272460853])
+        samples=[0.0, 1.0232274785475506, 1.8115262724608532])
 
 .. plotly::
 
   from math import pi
   from signalyzer import Trace
 
   signal = Trace('Signal', [1, pi/2, pi])
```

### Comparing `signalyzer-0.2.4/docs/transformations/value_conversions.rst` & `signalyzer-0.3.0/docs/transformations/value_conversions.rst`

 * *Files identical despite different names*

### Comparing `signalyzer-0.2.4/docs/transformations/x-axis_transformations.rst` & `signalyzer-0.3.0/docs/transformations/x-axis_transformations.rst`

 * *Files identical despite different names*

### Comparing `signalyzer-0.2.4/make.bat` & `signalyzer-0.3.0/make.bat`

 * *Files identical despite different names*

### Comparing `signalyzer-0.2.4/notebooks/DFT.ipynb` & `signalyzer-0.3.0/notebooks/DFT.ipynb`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9755847953216374%*

 * *Differences: {"'cells'": "{11: {'id': 'd9cfbbc4-aab1-45b8-aff7-0960894cc605', 'source': {insert: [(0, 'def "*

 * *            "_dft(x):\\n'), (2, '    Function to calculate the discrete Fourier Transform of a 1D "*

 * *            "real-valued signal x.\\n'), (7, '    e = np.exp(-2j * np.pi * k * (n / N))\\n')], "*

 * *            "delete: [10, 8, 7, 2, 0]}}, 12: {'id': '4e34e7db-01da-4346-9dc1-acf012468703', "*

 * *            "'source': ['_dft(trace)']}, 13: {'id': '52178519-1366-487f-9206-b6f48ca70914', "*

 * *            '\'source\': [\'def […]*

```diff
@@ -17,14 +17,24 @@
             "source": [
                 "import numpy as np"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "d15fc2e3-5ce4-4f06-981e-3cc79de92b77",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "import scipy"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
             "id": "64bdf6c7-0725-4f33-9ffc-0e2a8025bcf7",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import plotly.graph_objects as go"
             ]
         },
@@ -97,95 +107,73 @@
             "source": [
                 "trace.figure()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "52178519-1366-487f-9206-b6f48ca70914",
+            "id": "d9cfbbc4-aab1-45b8-aff7-0960894cc605",
             "metadata": {},
             "outputs": [],
             "source": [
-                "def dft(x):\n",
+                "def _dft(x):\n",
                 "    \"\"\"\n",
-                "    Function to calculate the discrete Fourier Transform of a 1D real-valued signal x\n",
+                "    Function to calculate the discrete Fourier Transform of a 1D real-valued signal x.\n",
                 "    \"\"\"\n",
                 "    N = len(x)\n",
                 "    n = np.arange(N)\n",
                 "    k = n.reshape((N, 1))\n",
-                "    e = np.exp(-2j * np.pi * k * n / N)\n",
-                "    \n",
+                "    e = np.exp(-2j * np.pi * k * (n / N))\n",
                 "    X = np.dot(e, x)\n",
-                "    \n",
                 "    return X"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "ff057b31-78a8-4d76-a2d6-648a35696b66",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "X = dft(trace)\n",
-                "X"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "c09277ee-014a-4e2e-97e5-90caf554f08d",
+            "id": "4e34e7db-01da-4346-9dc1-acf012468703",
             "metadata": {},
             "outputs": [],
             "source": [
-                "N = len(X)\n",
-                "N"
+                "_dft(trace)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "413b0dc3-c53e-4835-9add-a18646932e1e",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "n = np.arange(N)\n",
-                "n"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "87d3f064-352d-4abb-8f60-c7371a09f5e2",
+            "id": "52178519-1366-487f-9206-b6f48ca70914",
             "metadata": {},
             "outputs": [],
             "source": [
-                "T = N * dt\n",
-                "T"
+                "def dft(trace):\n",
+                "    \"\"\"\n",
+                "    Function to calculate the discrete Fourier Transform of a 1D real-valued signal x\n",
+                "    \"\"\"\n",
+                "    N = len(trace)\n",
+                "    return (scipy.fft.fftfreq(N), scipy.fft.fft(trace, N))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "0c4190c2-a3bc-4203-8b6b-d48efb2f234d",
+            "id": "f386a66a-2ab6-4caf-989d-eb9d05212ece",
             "metadata": {},
             "outputs": [],
             "source": [
-                "freq = n / T \n",
-                "freq"
+                "f, A = dft(trace)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "b85e48b9-b0c4-4e8a-b76c-daf2f5667c4d",
             "metadata": {},
             "outputs": [],
             "source": [
-                "go.Figure(go.Scatter(x=freq, y=abs(X), mode='markers+lines')) "
+                "go.Figure(go.Scatter(x=f / dt, y=abs(A), mode='lines'))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "466a445d-fc51-4784-8c39-5850085e0b25",
             "metadata": {},
```

### Comparing `signalyzer-0.2.4/notebooks/chord/.ipynb_checkpoints/chord-checkpoint.ipynb` & `signalyzer-0.3.0/notebooks/chord/chord.ipynb`

 * *Files identical despite different names*

### Comparing `signalyzer-0.2.4/notebooks/chord/.ipynb_checkpoints/chord-diagram-checkpoint.ipynb` & `signalyzer-0.3.0/notebooks/chord/chord-diagram.ipynb`

 * *Files identical despite different names*

### Comparing `signalyzer-0.2.4/notebooks/statemachine/statemachine.ipynb` & `signalyzer-0.3.0/notebooks/statemachine/statemachine.ipynb`

 * *Files identical despite different names*

### Comparing `signalyzer-0.2.4/notebooks/statistics/statistics.ipynb` & `signalyzer-0.3.0/notebooks/statistics/statistics.ipynb`

 * *Files identical despite different names*

### Comparing `signalyzer-0.2.4/notebooks/trace/trace.ipynb` & `signalyzer-0.3.0/notebooks/trace/trace.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9987003968253968%*

 * *Differences: {"'cells'": "{insert: [(1093, OrderedDict([('cell_type', 'markdown'), ('id', "*

 * *            "'2a97fc56-8c54-445d-9e5c-edb77fe4d759'), ('metadata', OrderedDict()), ('source', "*

 * *            "['### Alpha-Beta Filter (g-h Filter)'])])), (1094, OrderedDict([('cell_type', "*

 * *            "'code'), ('execution_count', None), ('id', 'b827fd71-10de-443e-849f-95050902212a'), "*

 * *            '(\'metadata\', OrderedDict()), (\'outputs\', []), (\'source\', ["trace = '*

 * *            'Trace(\'Signal\', [1, 2, 3, 4, 5, 6, 7, 8, 9 […]*

```diff
@@ -10648,14 +10648,62 @@
             "metadata": {},
             "source": [
                 "## Signal Processing: Smoothing"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "2a97fc56-8c54-445d-9e5c-edb77fe4d759",
+            "metadata": {},
+            "source": [
+                "### Alpha-Beta Filter (g-h Filter)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "b827fd71-10de-443e-849f-95050902212a",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "trace = Trace('Signal', [1, 2, 3, 4, 5, 6, 7, 8, 9])"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "dc2e8474-ca6a-4e5c-bcac-e987162ce657",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "traces = trace.alpha_beta_filter(dt=1, alpha=0.5, beta=1)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "b25c471c-8a2c-4343-a80f-79b2eca03a2b",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "traces"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "8940536e-b611-4ca1-8270-70ec242856f4",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "traces.figure(original=trace)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
             "id": "6aca4085-1e07-49b2-aee5-4260bc4352e1",
             "metadata": {},
             "source": [
                 "### Expontial Smoothing 2nd-Order"
             ]
         },
         {
@@ -10921,15 +10969,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.10"
+            "version": "3.10.7"
         },
         "toc-autonumbering": false,
         "toc-showcode": false,
         "toc-showmarkdowntxt": false,
         "toc-showtags": false
     },
     "nbformat": 4,
```

### Comparing `signalyzer-0.2.4/setup.cfg` & `signalyzer-0.3.0/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -55,52 +55,52 @@
 00000360: 6e67 7561 6765 203a 3a20 456e 676c 6973  nguage :: Englis
 00000370: 680d 0a09 4f70 6572 6174 696e 6720 5379  h...Operating Sy
 00000380: 7374 656d 203a 3a20 4f53 2049 6e64 6570  stem :: OS Indep
 00000390: 656e 6465 6e74 0d0a 0950 726f 6772 616d  endent...Program
 000003a0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
 000003b0: 2050 7974 686f 6e0d 0a09 5072 6f67 7261   Python...Progra
 000003c0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-000003d0: 3a20 5079 7468 6f6e 203a 3a20 332e 390d  : Python :: 3.9.
-000003e0: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-000003f0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000400: 203a 3a20 332e 3130 0d0a 0954 6f70 6963   :: 3.10...Topic
-00000410: 203a 3a20 4564 7563 6174 696f 6e0d 0a09   :: Education...
-00000420: 546f 7069 6320 3a3a 2053 6369 656e 7469  Topic :: Scienti
-00000430: 6669 632f 456e 6769 6e65 6572 696e 670d  fic/Engineering.
-00000440: 0a09 546f 7069 6320 3a3a 2053 6369 656e  ..Topic :: Scien
-00000450: 7469 6669 632f 456e 6769 6e65 6572 696e  tific/Engineerin
-00000460: 6720 3a3a 2049 6e66 6f72 6d61 7469 6f6e  g :: Information
-00000470: 2041 6e61 6c79 7369 730d 0a09 546f 7069   Analysis...Topi
-00000480: 6320 3a3a 2053 6369 656e 7469 6669 632f  c :: Scientific/
-00000490: 456e 6769 6e65 6572 696e 6720 3a3a 2056  Engineering :: V
-000004a0: 6973 7561 6c69 7a61 7469 6f6e 0d0a 7072  isualization..pr
-000004b0: 6f6a 6563 745f 7572 6c73 203d 200d 0a09  oject_urls = ...
-000004c0: 4973 7375 6520 5472 6163 6b65 7220 3d20  Issue Tracker = 
-000004d0: 6874 7470 733a 2f2f 6769 746c 6162 2e63  https://gitlab.c
-000004e0: 6f6d 2f73 6967 6e61 6c79 7469 6373 2f73  om/signalytics/s
-000004f0: 6967 6e61 6c79 7a65 722f 2d2f 6973 7375  ignalyzer/-/issu
-00000500: 6573 2f0d 0a09 446f 6375 6d65 6e74 6174  es/...Documentat
-00000510: 696f 6e20 3d20 6874 7470 733a 2f2f 7369  ion = https://si
-00000520: 676e 616c 797a 6572 2e72 6561 6474 6865  gnalyzer.readthe
-00000530: 646f 6373 2e69 6f0d 0a09 536f 7572 6365  docs.io...Source
-00000540: 2043 6f64 6520 3d20 6874 7470 733a 2f2f   Code = https://
-00000550: 6769 746c 6162 2e63 6f6d 2f73 6967 6e61  gitlab.com/signa
-00000560: 6c79 7469 6373 2f73 6967 6e61 6c79 7a65  lytics/signalyze
-00000570: 722f 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d  r/....[options].
-00000580: 0a70 6163 6b61 6765 7320 3d20 6669 6e64  .packages = find
-00000590: 3a0d 0a70 6163 6b61 6765 5f64 6972 203d  :..package_dir =
-000005a0: 203d 2073 7263 0d0a 696e 7374 616c 6c5f   = src..install_
-000005b0: 7265 7175 6972 6573 203d 200d 0a09 6e75  requires = ...nu
-000005c0: 6d70 793e 3d31 2e32 312e 350d 0a09 7363  mpy>=1.21.5...sc
-000005d0: 6970 793e 3d31 2e37 2e33 0d0a 0970 616e  ipy>=1.7.3...pan
-000005e0: 6461 733e 3d31 2e33 2e35 0d0a 0970 6c6f  das>=1.3.5...plo
-000005f0: 746c 793e 3d35 2e35 0d0a 7079 7468 6f6e  tly>=5.5..python
-00000600: 5f72 6571 7569 7265 7320 3d20 3e3d 2033  _requires = >= 3
-00000610: 2e39 0d0a 696e 636c 7564 655f 7061 636b  .9..include_pack
-00000620: 6167 655f 6461 7461 203d 2054 7275 650d  age_data = True.
-00000630: 0a7a 6970 5f73 6166 6520 3d20 4661 6c73  .zip_safe = Fals
-00000640: 650d 0a0d 0a5b 6f70 7469 6f6e 732e 7061  e....[options.pa
-00000650: 636b 6167 6573 2e66 696e 645d 0d0a 7768  ckages.find]..wh
-00000660: 6572 6520 3d20 7372 630d 0a0d 0a5b 6567  ere = src....[eg
-00000670: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
-00000680: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
-00000690: 3d20 300d 0a0d 0a                        = 0....
+000003d0: 3a20 5079 7468 6f6e 203a 3a20 332e 3130  : Python :: 3.10
+000003e0: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
+000003f0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00000400: 6e20 3a3a 2033 2e31 310d 0a09 546f 7069  n :: 3.11...Topi
+00000410: 6320 3a3a 2045 6475 6361 7469 6f6e 0d0a  c :: Education..
+00000420: 0954 6f70 6963 203a 3a20 5363 6965 6e74  .Topic :: Scient
+00000430: 6966 6963 2f45 6e67 696e 6565 7269 6e67  ific/Engineering
+00000440: 0d0a 0954 6f70 6963 203a 3a20 5363 6965  ...Topic :: Scie
+00000450: 6e74 6966 6963 2f45 6e67 696e 6565 7269  ntific/Engineeri
+00000460: 6e67 203a 3a20 496e 666f 726d 6174 696f  ng :: Informatio
+00000470: 6e20 416e 616c 7973 6973 0d0a 0954 6f70  n Analysis...Top
+00000480: 6963 203a 3a20 5363 6965 6e74 6966 6963  ic :: Scientific
+00000490: 2f45 6e67 696e 6565 7269 6e67 203a 3a20  /Engineering :: 
+000004a0: 5669 7375 616c 697a 6174 696f 6e0d 0a70  Visualization..p
+000004b0: 726f 6a65 6374 5f75 726c 7320 3d20 0d0a  roject_urls = ..
+000004c0: 0949 7373 7565 2054 7261 636b 6572 203d  .Issue Tracker =
+000004d0: 2068 7474 7073 3a2f 2f67 6974 6c61 622e   https://gitlab.
+000004e0: 636f 6d2f 7369 676e 616c 7974 6963 732f  com/signalytics/
+000004f0: 7369 676e 616c 797a 6572 2f2d 2f69 7373  signalyzer/-/iss
+00000500: 7565 732f 0d0a 0944 6f63 756d 656e 7461  ues/...Documenta
+00000510: 7469 6f6e 203d 2068 7474 7073 3a2f 2f73  tion = https://s
+00000520: 6967 6e61 6c79 7a65 722e 7265 6164 7468  ignalyzer.readth
+00000530: 6564 6f63 732e 696f 0d0a 0953 6f75 7263  edocs.io...Sourc
+00000540: 6520 436f 6465 203d 2068 7474 7073 3a2f  e Code = https:/
+00000550: 2f67 6974 6c61 622e 636f 6d2f 7369 676e  /gitlab.com/sign
+00000560: 616c 7974 6963 732f 7369 676e 616c 797a  alytics/signalyz
+00000570: 6572 2f0d 0a0d 0a5b 6f70 7469 6f6e 735d  er/....[options]
+00000580: 0d0a 7061 636b 6167 6573 203d 2066 696e  ..packages = fin
+00000590: 643a 0d0a 7061 636b 6167 655f 6469 7220  d:..package_dir 
+000005a0: 3d20 3d20 7372 630d 0a69 6e73 7461 6c6c  = = src..install
+000005b0: 5f72 6571 7569 7265 7320 3d20 0d0a 096e  _requires = ...n
+000005c0: 756d 7079 3e3d 312e 3234 2e31 0d0a 0973  umpy>=1.24.1...s
+000005d0: 6369 7079 3e3d 312e 3130 2e31 0d0a 0970  cipy>=1.10.1...p
+000005e0: 616e 6461 733e 3d32 2e30 2e30 0d0a 0970  andas>=2.0.0...p
+000005f0: 6c6f 746c 793e 3d35 2e31 342e 310d 0a70  lotly>=5.14.1..p
+00000600: 7974 686f 6e5f 7265 7175 6972 6573 203d  ython_requires =
+00000610: 203e 3d20 332e 3130 0d0a 696e 636c 7564   >= 3.10..includ
+00000620: 655f 7061 636b 6167 655f 6461 7461 203d  e_package_data =
+00000630: 2054 7275 650d 0a7a 6970 5f73 6166 6520   True..zip_safe 
+00000640: 3d20 4661 6c73 650d 0a0d 0a5b 6f70 7469  = False....[opti
+00000650: 6f6e 732e 7061 636b 6167 6573 2e66 696e  ons.packages.fin
+00000660: 645d 0d0a 7768 6572 6520 3d20 7372 630d  d]..where = src.
+00000670: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
+00000680: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
+00000690: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
```

### Comparing `signalyzer-0.2.4/src/signalyzer/__init__.py` & `signalyzer-0.3.0/src/signalyzer/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 # -*- coding: utf-8 -*-
 """
 signalyzer.py
 ~~~~~~~~~~~~~
 Public package API.
 
-:copyright: (c) 2021-2022 by Jochen Gerhaeusser.
+:copyright: (c) 2021-2023 by Jochen Gerhaeusser.
 :license: BSD, see LICENSE for details.
 """
+from __future__ import annotations
 
 from .trace import *
 from .statemachine import *
 
 # package exports
 __all__ = [
+    # Custom Types
+    'Number',
+    'Sample', 'Samples',
+    'Operand',
+    'DataFrame',
+
     # Representations
     'Point2D', 'Vector',
     'Point3D',
     'State2D', 'State3D',
 
     # Signal Processing
     'Statistics',
@@ -33,14 +40,13 @@
     'logical_and', 'logical_or', 'priority',
     'Traces', 'as_traces',
     'VectorTraces', 'polar',
     'StatisticsTraces',
     'MovingAverageTraces',
     'SetTraces', 'combine',
     'SlewRateLimiterTraces',
+    'AlphaBetaFilterTraces',
     'ExponentialSmoothingTraces',
-    'LinearRegressionTraces',
-
+    'LinearRegressionTraces'
 ]
 
-__version__ = '0.2.4'
-
+__version__ = '0.3.0'
```

### Comparing `signalyzer-0.2.4/src/signalyzer/constants.py` & `signalyzer-0.3.0/src/signalyzer/constants.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,25 @@
-# -*- coding: utf-8 -*-
-"""
-constants.py
-~~~~~~~~~~~~
-Constants.
-
-:copyright: (c) 2021 by Jochen Gerhaeusser.
-:license: BSD, see LICENSE for details
-"""
-
-import numpy as np
-
-#: Maximal value for a 32-bit floating point number
-f32_MAX: float = (1 - 2 ** -24) * 2 ** 128
-
-#: Maximal value for a cubic 32-bit floating point number
-f32_MAX_POW3 = np.cbrt(f32_MAX)
-
-#: Minimal de-normalized value for a floating-point number
-f32_MIN: float = 2 ** -149
-
-#: Minimal normalized value for a floating-point number
-f32_MIN_POSITIVE: float = 2 ** -126
-
-#: Epsilon value for a 32-bit floating-point number
-f32_EPSILON: float = 2 ** -24
+# -*- coding: utf-8 -*-
+"""
+constants.py
+~~~~~~~~~~~~
+Constants.
+
+:copyright: (c) 2021 by Jochen Gerhaeusser.
+:license: BSD, see LICENSE for details
+"""
+import numpy as np
+
+#: Maximal value for a 32-bit floating point number
+f32_MAX: float = (1 - 2 ** -24) * 2 ** 128
+
+#: Maximal value for a cubic 32-bit floating point number
+f32_MAX_POW3 = np.cbrt(f32_MAX)
+
+#: Minimal de-normalized value for a floating-point number
+f32_MIN: float = 2 ** -149
+
+#: Minimal normalized value for a floating-point number
+f32_MIN_POSITIVE: float = 2 ** -126
+
+#: Epsilon value for a 32-bit floating-point number
+f32_EPSILON: float = 2 ** -24
```

### Comparing `signalyzer-0.2.4/src/signalyzer/statemachine/__init__.py` & `signalyzer-0.3.0/src/signalyzer/statemachine/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,76 +7,78 @@
 
 :copyright: (c) 2022 by Jochen Gerhaeusser.
 :license: BSD, see LICENSE for details
 """
 from __future__ import annotations
 
 from dataclasses import (
-    dataclass, field, fields)
+    dataclass, field, fields, Field)
 from itertools import (
     chain, permutations, repeat)
+from typing import (
+    Any, Iterator, MutableMapping, Optional, Sequence)
 
 import plotly.express as px
 import plotly.figure_factory as ff
 import plotly.graph_objects as go
 
 from .. import Trace
-from ..types import *
 
 # module exports
 __all__ = [
     'State2D',
     'State3D',
     'Statemachine',
 ]
 
 
 @dataclass(eq=False)
 class Statemachine(MutableMapping):
-    """ statemachine data class to :attr:`evaluate` the state transitions
+    """ Statemachine data class to :attr:`evaluate` the state transitions
     between :attr:`states` of a statemachine.
 
     A *state* of the statemachine is defined by a tuple pair, consisting of
     a unique integer *number* of the state, and the *label* of the state.
 
     The :attr:`states` of a statemachine must define a consecutive, ascending
     interval of integer :attr:`numbers`.
     """
     #: States of the statemachine
-    states: Union[Dict[int, Union[str, State2D, State3D]]]
+    states: dict[int, str | State2D | State3D]
     #: Signal trace with the state numbers
     signal: Trace = field(default_factory=Trace)
     #: List with the state labels of the statemachine
-    labels: List = field(default_factory=list)
+    labels: list[str] = field(default_factory=list)
     #: Matrix with the counted transitions between the states
-    matrix: List[List[int]] = field(default_factory=list)
+    matrix: list[list[int]] = field(default_factory=list)
 
     @classmethod
     def create(cls,
-               states: Union[int, Iterable[str, State2D, State3D]],
-               start: Optional[int] = 0,
-               **kwargs) -> Statemachine:
+               states: int | Sequence[str | State2D | State3D],
+               start: int = 0,
+               **kwargs: Any) -> Statemachine:
         """ Creates either a statemachine with the number of *states* without
-        labeling them, or a statemachine with states from an iterable containing
+        labeling them, or a statemachine with states from a sequence containing
         the labels or representations of the *states* to create.
 
-        :param states: number of states or a list with the labels or
+        :param states: number of states or a sequence with the labels or
             representations for the :attr:`states` to create
+        :type states: int | Sequence[str | State2D | State3D]
         :param int start: start number for the :attr:`states` to create
             Default is ``0``.
         """
         if isinstance(states, int):
             nodes = dict(enumerate(range(states), start))
         elif isinstance(states, (list, tuple)):
             nodes = dict(enumerate(states, start))
         else:
             nodes = dict()
         return cls(states=nodes, **kwargs)
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         if not self.labels:
             for key, value in self.items():
                 if isinstance(value, (State2D, State3D)):
                     self.labels.append(value.name)
                 elif value is None:
                     self.labels.append(str(key))
                 else:
@@ -85,43 +87,43 @@
             # computes the transition matrix
             self.evaluate()
         elif not self.matrix:
             # initialize zeroed transition matrix
             self.matrix = self.zeroed_matrix()
 
     @property
-    def numbers(self):
+    def numbers(self) -> list[int]:
         """ List with the state numbers of the statemachine."""
         return list(self.states.keys())
 
-    def __setitem__(self, key: int, value: Union[str, State2D, State3D]):
+    def __setitem__(self, key: int, value: str | State2D | State3D):
         self.states[key] = value
 
-    def __getitem__(self, key: int) -> Union[str, State2D, State3D]:
+    def __getitem__(self, key: int) -> str | State2D | State3D:
         return self.states[key]
 
-    def __delitem__(self, key):
+    def __delitem__(self, key: int):
         raise NotImplemented()
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator[int]:
         return iter(self.states)
 
     def __len__(self) -> int:
         return len(self.states)
 
-    def fields(self) -> Tuple[Any, ...]:
+    def fields(self) -> tuple[Field, ...]:
         """ Returns a tuple describing the fields of the data class."""
         return fields(self)
 
-    def zeroed_matrix(self) -> List[List[int, ...]]:
+    def zeroed_matrix(self) -> list[list[int]]:
         """ Returns the zeroed transition matrix of the statemachine.
         """
         return [[0] * len(self) for _ in range(len(self))]
 
-    def zeroed_counters(self) -> Dict[tuple[int, ...], int]:
+    def zeroed_counters(self) -> dict[tuple[int, int], int]:
         """ Returns the dictionary with the zeroed state transition counters
         of the statemachine."""
         return dict((transition, 0) for transition in permutations(self.states, 2))
 
     def evaluate(self, signal: Optional[Trace] = None) -> Statemachine:
         """ Counts the state transitions between the :attr:`states` of the
         statemachine in the :attr:`signal`.
@@ -155,63 +157,63 @@
 
         # fill transition matrix with counted transitions
         for key, value in counters.items():
             i, j = key
             self.matrix[i - offset][j - offset] = value
         return self
 
-    def flatten(self) -> Iterator:
+    def flatten(self) -> Iterator[int]:
         """ Returns an iterator to flatten the state transition :attr:`matrix`
         into a list.
         """
         return chain.from_iterable(self.matrix)
 
-    def data(self) -> List[List[str, int, ...]]:
+    def data(self) -> list[list[str | int]]:
         """ Returns the data table with the counted state transitions
         between the :attr:`states` of the statemachine.
         """
         # table data
         data = list()
         # add column labels
         data.append([''] + self.labels)
         # add rows
         for name, values in zip(self.labels, self.matrix):
             data.append([name] + values)
         return data
 
-    def table(self, **kwargs) -> go.Figure:
+    def table(self, **kwargs: Any) -> go.Figure:
         """ Returns a table figure for the state transition :attr:`matrix`
-        of the statemachine. """
+        of the statemachine."""
         return ff.create_table(self.data(), index=True, **kwargs)
 
-    def plot(self, **kwargs) -> go.Heatmap:
+    def plot(self, **kwargs: Any) -> go.Heatmap:
         """ Returns a heatmap plot for the state transition :attr:`matrix`
         of the statemachine."""
         settings = dict(
             z=self.matrix,
             x=self.labels,
             y=self.labels
         )
         plot = go.Heatmap(**settings)
         return plot.update(**kwargs)
 
-    def heatmap(self, **kwargs) -> go.Figure:
+    def heatmap(self, **kwargs: Any) -> go.Figure:
         """ Returns a heatmap figure for the state transition :attr:`matrix`
         of the statemachine."""
         # default settings
         settings = dict(
             x=self.labels,
             y=self.labels,
             text_auto=True,
             color_continuous_scale='Blues'
         )
         settings.update(kwargs)
         return px.imshow(self.matrix, **settings)
 
-    def flowchart(self, **kwargs) -> go.Sankey:
+    def flowchart(self, **kwargs: Any) -> go.Sankey:
         """ Returns a sankey flow-chart plot for the state transition
         :attr:`matrix` of the statemachine."""
         # number of states
         count = len(self)
 
         settings = dict(
             node=dict(label=self.labels),
```

### Comparing `signalyzer-0.2.4/src/signalyzer/trace/__init__.py` & `signalyzer-0.3.0/src/signalyzer/trace/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,44 @@
 # -*- coding: utf-8 -*-
 """
 trace
 ~~~~~
 Module contains a trace to analyze, process, visualize time-discrete measured
 signals.
 
-:copyright: (c) 2021-2022 by Jochen Gerhaeusser.
+:copyright: (c) 2021-2023 by Jochen Gerhaeusser.
 :license: BSD, see LICENSE for details
 """
 from __future__ import annotations
 
 import math
 import operator
 import statistics as stats
 from collections import defaultdict
 from dataclasses import (
-    dataclass, field, replace, fields, asdict, astuple)
+    asdict, astuple, dataclass, field, fields, Field, replace)
 from itertools import (
     accumulate, chain, islice, repeat, tee)
+from typing import (
+    Any, Callable,
+    Iterable, Iterator,
+    Mapping, MutableMapping,
+    Optional,
+    Sequence, MutableSequence,
+    TypeAlias,
+    Union)
 
 import numpy as np
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
 from scipy.stats.mstats import winsorize
 
-from ..types import *
-
 # module exports
 __all__ = [
+    'Number', 'Sample', 'Samples', 'Operand', 'DataFrame',
     'Trace', 'vectorize',
     'logical_and', 'logical_or', 'priority',
     'Traces', 'as_traces',
     'Point2D',
     'Point3D',
     'Vector',
     'VectorTraces', 'polar',
@@ -41,42 +48,61 @@
     'SetTraces', 'combine',
     'SlewRateLimiter',
     'SlewRateLimiterTraces',
     'ExponentialSmoothing',
     'ExponentialSmoothingTraces',
     'LinearRegression',
     'LinearRegressionTraces',
+    'AlphaBetaFilter',
+    'AlphaBetaFilterTraces',
     'IIRFilter',
 ]
 
+#: Numeric type
+Number: TypeAlias = Union[bool, int, float]
+
+#: Sample type
+Sample: TypeAlias = Union[Number, str]
+
+#: Samples type
+Samples: TypeAlias = Union[MutableSequence[Sample], Iterable[Sample], Iterable[None]]
+
+#: Operand type
+Operand: TypeAlias = Union[Iterable[Number], Number]
+
+#: Data frame type
+DataFrame: TypeAlias = Mapping[str, Iterable[Sample]]
+
 # Signum function
 sign = np.sign
 
 
-def _pairwise(trace: Union[Iterator, List, Trace]) -> Iterator[Tuple[Number, Number]]:
+def _pairwise(trace: (Iterator[Number] |
+                      Sequence[Number] |
+                      Trace)) -> Iterator[tuple[Number, Number]]:
     """ Returns a pairwise iterator for the signal :attr:`~Trace.samples` in a
     :class:`Trace`.
 
     :param trace: trace to iterate
     """
     a, b = tee(trace)
     next(b, None)
     return zip(a, b)
 
 
-def _clip(value: Number,
-          lower: Optional[Number],
-          upper: Optional[Number]) -> Number:
+def _clip(value: float | int,
+          lower: float | int | None,
+          upper: float | int | None) -> float | int:
     """ Returns the *value* limited between the *lower* and *upper* bound.
 
     .. note:: The *upper* bound is dominant over the *lower* bound.
 
-    :param value: value to clip
-    :param lower: value of the lower bound or None
-    :param upper: value of the upper bound or None
+    :param float | int value: value to clip
+    :param float | int lower: optional value of the lower bound or ``None``
+    :param float | int upper: optional value of the upper bound or ``None``
     """
     if lower is None and upper is None:
         # no bound
         return value
     elif upper is None:
         # lower bound
         return max(value, lower)
@@ -84,30 +110,31 @@
         # upper bound
         return min(value, upper)
     else:
         # both bounds
         return min(upper, max(lower, value))
 
 
-def _clamp(value: Number, bound: Optional[Number]) -> Number:
+def _clamp(value: float | int,
+           bound: float | int) -> float | int:
     """ Returns the *value* symmetrically clamped at the *bound*.
 
-    :param value: value to clamp
-    :param bound: bound to clamp at
+    :param float | int value: value to clamp
+    :param float | int bound: bound to clamp at
     """
     bound = abs(bound)
     return _clip(value, -bound, bound)
 
 
 def vectorize(operand: Operand) -> Samples:
     """ Returns for an :class:`int`, :class:`float`, :class:`bool` or number
     literal :class:`str` *operand* an endless iterator, otherwise the *operand*
     is returned unchanged.
 
-    :param operand: operand to vectorize
+    :param Operand operand: operand to vectorize
     """
     if operand is None:
         return repeat(None)
     if isinstance(operand, (int, float, bool)):
         # create number iterator
         return repeat(operand)
     if isinstance(operand, str):
@@ -142,23 +169,25 @@
     a2: float
     #: Sum of the 1st-feedback stage of the SOS-IIR filter
     s1: float = 0.0
     #: Sum of the 2nd-feedback stage of the SOS-IIR filter
     s2: float = 0.0
 
     @classmethod
-    def band_pass(cls, dt: float, f0: float,
+    def band_pass(cls,
+                  dt: float,
+                  f0: float,
                   q: float = 1 / math.sqrt(2)) -> IIRFilter:
         """ Creates a digital second-order IIR band-pass filter with normalized
         filter coefficients for the given sampling-time *dt*, center frequency
         *f0* and quality factor *q* of the filter.
 
-        :param dt: sampling-time of the filter in seconds
-        :param f0: center frequency of the filter in Hertz
-        :param q: inverse of bandwidth factor of the filter
+        :param float dt: sampling-time of the filter in seconds
+        :param float f0: center frequency of the filter in Hertz
+        :param float q: inverse of bandwidth factor of the filter
         """
         omega = 2 * math.pi * f0 * dt
         alpha = math.sin(omega) / (2 * q)
 
         # filter coefficients numerator
         b0 = alpha
         b1 = 0
@@ -169,23 +198,25 @@
         a1 = -2 * math.cos(omega)
         a2 = 1 - alpha
 
         # second-order IIR filter with normalized filter coefficients
         return cls(b0 / a0, b1 / a0, b2 / a0, a1 / a0, a2 / a0)
 
     @classmethod
-    def low_pass(cls, dt: float, f0: float,
+    def low_pass(cls,
+                 dt: float,
+                 f0: float,
                  q: float = 1 / math.sqrt(2)) -> IIRFilter:
         """ Creates a digital second-order IIR low-pass filter with normalized
         filter coefficients for the given sampling-time *dt*, cutoff frequency
         *f0* and quality factor *q* of the filter.
 
-        :param dt: sampling-time of the filter in seconds
-        :param f0: cutoff frequency of the filter in Hertz
-        :param q: inverse of bandwidth factor of the filter
+        :param float dt: sampling-time of the filter in seconds
+        :param float f0: cutoff frequency of the filter in Hertz
+        :param float q: inverse of bandwidth factor of the filter
         """
         omega = 2 * math.pi * f0 * dt
         alpha = math.sin(omega) / (2 * q)
 
         # filter coefficients numerator
         b0 = (1 - math.cos(omega)) / 2
         b1 = 1 - math.cos(omega)
@@ -196,23 +227,25 @@
         a1 = -2 * math.cos(omega)
         a2 = 1 - alpha
 
         # second-order IIR filter with normalized filter coefficients
         return cls(b0 / a0, b1 / a0, b2 / a0, a1 / a0, a2 / a0)
 
     @classmethod
-    def high_pass(cls, dt: float, f0: float,
+    def high_pass(cls,
+                  dt: float,
+                  f0: float,
                   q: float = 1 / math.sqrt(2)) -> IIRFilter:
         """ Creates a digital second-order IIR high-pass filter with normalized
         filter coefficients for the given sampling-time *dt*, cutoff frequency
         *f0* and quality factor *q* of the filter.
 
-        :param dt: sampling-time of the filter in seconds
-        :param f0: cutoff frequency of the filter in Hertz
-        :param q: inverse of bandwidth factor of the filter
+        :param float dt: sampling-time of the filter in seconds
+        :param float f0: cutoff frequency of the filter in Hertz
+        :param float q: inverse of bandwidth factor of the filter
         """
         omega = 2 * math.pi * f0 * dt
         alpha = math.sin(omega) / (2 * q)
 
         # filter coefficients numerator
         b0 = (1 + math.cos(omega)) / 2
         b1 = -(1 + math.cos(omega))
@@ -223,22 +256,25 @@
         a1 = -2 * math.cos(omega)
         a2 = 1 - alpha
 
         # second-order IIR filter with normalized filter coefficients
         return cls(b0 / a0, b1 / a0, b2 / a0, a1 / a0, a2 / a0)
 
     @classmethod
-    def notch(cls, dt: float, f0: float, q: float = 1 / math.sqrt(2)) -> IIRFilter:
+    def notch(cls,
+              dt: float,
+              f0: float,
+              q: float = 1 / math.sqrt(2)) -> IIRFilter:
         """ Creates a digital second-order IIR notch filter with normalized
         filter coefficients for the given sampling-time *dt*, center frequency
         *f0* and quality factor *q* of the filter.
 
-        :param dt: sampling-time of the filter in seconds
-        :param f0: center frequency of the filter in Hertz
-        :param q: inverse of bandwidth factor of the filter
+        :param float dt: sampling-time of the filter in seconds
+        :param float f0: center frequency of the filter in Hertz
+        :param float q: inverse of bandwidth factor of the filter
         """
         omega = 2 * math.pi * f0 * dt
         alpha = math.sin(omega) / (2 * q)
 
         # filter coefficients numerator
         b0 = 1
         b1 = -2 * math.cos(omega)
@@ -249,23 +285,25 @@
         a1 = -2 * math.cos(omega)
         a2 = 1 - alpha
 
         # second-order IIR filter with normalized filter coefficients
         return cls(b0 / a0, b1 / a0, b2 / a0, a1 / a0, a2 / a0)
 
     @classmethod
-    def all_pass(cls, dt: float, f0: float,
+    def all_pass(cls,
+                 dt: float,
+                 f0: float,
                  q: float = 1 / math.sqrt(2)) -> IIRFilter:
         """ Creates a digital second-order IIR all-pass filter with normalized
         filter coefficients for the given sampling-time *dt*, center frequency
         *f0* and quality factor *q* of the filter.
 
-        :param dt: sampling-time of the filter in seconds
-        :param f0: center frequency of the filter in Hertz
-        :param q: inverse of bandwidth factor of the filter
+        :param float dt: sampling-time of the filter in seconds
+        :param float f0: center frequency of the filter in Hertz
+        :param float q: inverse of bandwidth factor of the filter
         """
         omega = 2 * math.pi * f0 * dt
         alpha = math.sin(omega) / (2 * q)
 
         # filter coefficients numerator
         b0 = 1 - alpha
         b1 = -2 * math.cos(omega)
@@ -275,25 +313,25 @@
         a0 = 1 + alpha
         a1 = -2 * math.cos(omega)
         a2 = 1 - alpha
 
         # second-order IIR filter with normalized filter coefficients
         return cls(b0 / a0, b1 / a0, b2 / a0, a1 / a0, a2 / a0)
 
-    def clear(self):
+    def clear(self) -> None:
         """ Clears the sum value of the feedback stages of the SOS-IIR filter.
         """
         self.s1 = 0.0
         self.s2 = 0.0
 
-    def compute(self, x: float) -> float:
+    def compute(self, x: float | int) -> float:
         """ Computes for the sample :math:`x` the SOS-IIR filter equation in
         canonical form with the configured normalized filter coefficients.
 
-        :param x: sample value to compute
+        :param float | int x: sample value to compute
         """
         # normalized canonical form
         y = self.b0 * x + self.s1
         self.s1 = (self.b1 * x - self.a1 * y) + self.s2
         self.s2 = (self.b2 * x - self.a2 * y)
         return y
 
@@ -312,21 +350,24 @@
             # samples type conversion -> list
             self.samples = list(self.samples)
         if not isinstance(self.label, str):
             # label type conversion -> str
             self.label = str(self.label)
 
     @classmethod
-    def from_dict(cls, key: str, data: DataFrame, **kwargs) -> Trace:
+    def from_dict(cls,
+                  key: str,
+                  data: DataFrame,
+                  **kwargs: Any) -> Trace:
         """ Returns a new trace labeled with the *key*, and the signal
         :attr:`samples` from the value of the *data* dictionary item selected
         by the *key*.
 
-        :param str key: key name of the signal :attr:`samples` to select from the
-            data dictionary
+        :param str key: key name of the signal :attr:`samples` to select from
+            the data dictionary
         :param DataFrame data: dictionary with signal :attr:`samples`
         :keyword str label: optional :attr:`label` to set instead of the key name
         """
         kwargs['label'] = kwargs.get('label', key)
         kwargs['samples'] = data[key]
         return cls(**kwargs)
 
@@ -343,138 +384,144 @@
         """ Returns the stem of the trace :attr:`label`."""
         return self.label.partition(':')[0]
 
     def __len__(self) -> int:
         """ Returns the number of signal :attr:`samples` in the trace."""
         return len(self.samples)
 
-    def __getitem__(self, index: int) -> Union[List[Sample], Sample]:
+    def __getitem__(self,
+                    index: int | slice) -> Sample | MutableSequence[Sample]:
         """ Returns the sample at the *index* from the trace.
 
-        :param int index: index of the sample to get
+        :param int | slice index: index of the sample or the slice of the
+            samples to get
         """
         if isinstance(index, slice):
             return self.samples[index]
         else:
             return self.samples[index]
 
-    def __setitem__(self, index: int, value: Sample) -> None:
+    def __setitem__(self,
+                    index: int,
+                    value: Sample) -> None:
         """ Sets the sample at the *index* to the *value* in the trace.
 
         :param int index: index of the sample to set
-        :param value: numerical value to set
-        :type value: int, float
+        :param Sample value: numerical value to set
         """
         self.samples[index] = value
 
-    def __contains__(self, item) -> bool:
+    def __contains__(self, item: Sample) -> bool:
         """ Checks if the *item* is in the signal :attr:`samples` of the trace.
         """
         return item in self.samples
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator[Sample]:
         """ Returns an iterator over the signal :attr:`samples` in the trace."""
         return iter(self.samples)
 
-    def __reversed__(self) -> Iterator[Union[int, bool, float, str]]:
+    def __reversed__(self) -> Iterator[Sample]:
         """ Returns a reverse iterator over the signal :attr:`samples` in the
         trace."""
         return reversed(self.samples)
 
-    def repeat(self, times: Optional[int] = 1) -> Iterator[Sample]:
+    def repeat(self, times: int = 1) -> Iterator[Sample]:
         """ Returns an iterator repeating each signal sample of the trace
         n-*times*.
 
-        :param times: number of times to repeat a sample.
+        :param int times: number of times to repeat a sample.
             Default is ``1``.
         """
         return chain.from_iterable((map(lambda x: repeat(x, times), self)))
 
-    def fields(self) -> Tuple[Any, ...]:
+    def fields(self) -> tuple[Field, ...]:
         """ Returns a tuple describing the fields of the data class."""
         return fields(self)
 
-    def as_dict(self) -> Dict[str, Any]:
+    def as_dict(self) -> dict[str, Any]:
         """ Returns the trace data class as a dictionary."""
         return asdict(self)
 
     def as_tuple(self) -> tuple[Any, ...]:
         """ Returns the trace data class as a tuple.
         """
         return astuple(self)
 
-    def bool(self, **kwargs) -> Trace:
+    def bool(self, **kwargs: Any) -> Trace:
         """ Returns a new trace with the signal :attr:`samples` converted to
         booleans.
 
         :keyword str label: optional trace label to set
         """
         return replace(self,
                        label=kwargs.get('label', f'{self.label}:bool'),
                        samples=map(bool, self))
 
-    def int(self, base: Optional[int] = None, **kwargs) -> Trace:
+    def int(self,
+            base: int | None = None,
+            **kwargs: Any) -> Trace:
         """ Returns a new trace with the signal :attr:`samples` converted to
         integers.
 
+        :param int | None base: radix base of the integer literal to convert
         :keyword str label: optional trace label to set
         """
         if base is None:
             return replace(self,
                            label=kwargs.get('label', f'{self.label}:int'),
                            samples=map(int, self))
         return replace(self,
                        label=kwargs.get('label', f'{self.label}:int'),
                        samples=map(lambda item: int(item, base), self))
 
-    def float(self, **kwargs) -> Trace:
+    def float(self, **kwargs: Any) -> Trace:
         """ Returns a new trace with the signal :attr:`samples` converted to
         floating-points.
 
         :keyword str label: optional trace label to set
         """
         return replace(self,
                        label=kwargs.get('label', f'{self.label}:float'),
                        samples=map(float, self))
 
-    def bin(self, **kwargs) -> Trace:
+    def bin(self, **kwargs: Any) -> Trace:
         """ Returns a new trace with the signal :attr:`samples` converted to
         binary literals.
 
         :keyword str label: optional trace label to set
         """
         return replace(self,
                        label=kwargs.get('label', f'{self.label}:bin'),
                        samples=map(bin, self))
 
-    def oct(self, **kwargs) -> Trace:
+    def oct(self, **kwargs: Any) -> Trace:
         """ Returns a new trace with the signal :attr:`samples` converted to
         octal literals.
 
         :keyword str label: optional trace label to set
         """
         return replace(self,
                        label=kwargs.get('label', f'{self.label}:oct'),
                        samples=map(oct, self))
 
-    def hex(self, **kwargs) -> Trace:
+    def hex(self, **kwargs: Any) -> Trace:
         """ Returns a new trace with the signal :attr:`samples` converted to
         hexadecimal literals.
 
         :keyword str label: optional trace label to set
         """
         return replace(self,
                        label=kwargs.get('label', f'{self.label}:hex'),
                        samples=map(hex, self))
 
     def less(self, operand: Operand) -> Trace:
         """ Returns a new trace with the results as integers of the lesser
         comparison between the signal :attr:`samples` and the operand.
 
-        :parameter operand: iterable or number to compare with
+        :param Operand operand: iterable or number to compare with
 
         .. note:: An iterable *operand* should have at least the same length as
             the trace :attr:`samples`, otherwise only a subset of the signal
             :attr:`samples` is returned!
         """
         return replace(self,
                        label=f'{self.label}:lt',
@@ -484,15 +531,15 @@
     def __lt__(self, operand: Operand) -> Trace:
         return self.less(operand)
 
     def less_equal(self, operand: Operand) -> Trace:
         """ Returns a new trace with the results as integers of the lesser or
         equal comparison between the signal :attr:`samples` and the operand.
 
-        :parameter operand: iterable or number to compare with
+        :param Operand operand: iterable or number to compare with
 
         .. note:: An iterable *operand* should have at least the same length
             as the signal :attr:`samples`, otherwise only a subset of the signal
             :attr:`samples` is returned!
         """
         return replace(self,
                        label=f'{self.label}:le',
@@ -502,15 +549,15 @@
     def __le__(self, operand: Operand) -> Trace:
         return self.less_equal(operand)
 
     def equal(self, operand: Operand) -> Trace:
         """ Returns a new trace with the results as integers of the equal
         comparison between the signal :attr:`samples` and the operand.
 
-        :parameter operand: iterable or number to compare with
+        :param Operand operand: iterable or number to compare with
 
         .. note:: An iterable *operand* should have at least the same length
             as the signal :attr:`samples`, otherwise only a subset of the signal
             :attr:`samples` is returned!
         """
         return replace(self,
                        label=f'{self.label}:eq',
@@ -520,15 +567,15 @@
     def __eq__(self, operand: Operand) -> Trace:
         return self.equal(operand)
 
     def not_equal(self, operand: Operand) -> Trace:
         """ Returns a new trace with the results as integers of the not equal
         comparison between the signal :attr:`samples` and the operand.
 
-        :parameter operand: iterable or number to compare with
+        :param Operand operand: iterable or number to compare with
 
         .. note:: An iterable *operand* should have at least the same length
             as the signal :attr:`samples`, otherwise only a subset of the signal
             :attr:`samples` is returned!
         """
         return replace(self, label=f'{self.label}:ne',
                        samples=map(lambda lhs, rhs: int(lhs != rhs),
@@ -537,15 +584,15 @@
     def __ne__(self, operand: Operand) -> Trace:
         return self.not_equal(operand)
 
     def greater_equal(self, operand: Operand) -> Trace:
         """ Returns a new trace with the results as integers of the greater or
         equal comparison between the signal :attr:`samples` and the operand.
 
-        :parameter operand: iterable or number to compare with
+        :param Operand operand: iterable or number to compare with
 
         .. note:: An iterable *operand* should have at least the same length
             as the signal :attr:`samples`, otherwise only a subset of the signal
             :attr:`samples` is returned!
         """
         return replace(self,
                        label=f'{self.label}:ge',
@@ -555,15 +602,15 @@
     def __ge__(self, operand: Operand) -> Trace:
         return self.greater_equal(operand)
 
     def greater(self, operand: Operand) -> Trace:
         """ Returns a new trace with the results as integers of the greater
         comparison between the signal :attr:`samples` and the operand.
 
-        :parameter operand: iterable or number to compare with
+        :param Operand operand: iterable or number to compare with
 
         .. note:: An iterable *operand* should have at least the same length
             as the signal :attr:`samples`, otherwise only a subset of the signal
             :attr:`samples` is returned!
         """
         return replace(self,
                        label=f'{self.label}:gt',
@@ -573,15 +620,15 @@
     def __gt__(self, operand: Operand) -> Trace:
         return self.greater(operand)
 
     def add(self, summand: Operand) -> Trace:
         """ Returns a new trace with the sums of the signal :attr:`samples`
         and the *summand*.
 
-        :parameter summand: iterable or number
+        :param Operand summand: iterable or number
 
         .. note:: An iterable *summand* should have at least the same length
             as the signal :attr:`samples`, otherwise only a subset of the signal
             :attr:`samples` is returned!
         """
         return replace(self,
                        label=f'{self.label}:add',
@@ -591,30 +638,30 @@
     def __add__(self, summand: Operand) -> Trace:
         return self.add(summand)
 
     def __radd__(self, summand: Operand) -> Trace:
         """ Returns a new trace with the sums of the *summand* and the signal
         :attr:`samples`.
 
-        :parameter summand: iterable or number
+        :param Operand summand: iterable or number
 
         .. note:: An iterable *summand* should have at least the same length
             as the signal :attr:`samples`, otherwise only a subset of the signal
             :attr:`samples` is returned!
         """
         return replace(self,
                        label=f'{self.label}:radd',
                        samples=map(lambda a, b: a + b,
                                    vectorize(summand), self))
 
     def sub(self, subtrahend: Operand) -> Trace:
         """ Returns a new trace with the differences between the signal
         :attr:`samples` and the *subtrahend*.
 
-        :parameter subtrahend: iterable or number
+        :param Operand subtrahend: iterable or number
 
         .. note:: An iterable *subtrahend* should have at least the same length
             as the signal :attr:`samples`, otherwise only a subset of the signal
             :attr:`samples` is returned!
         """
         return replace(self,
                        label=f'{self.label}:sub',
@@ -624,30 +671,30 @@
     def __sub__(self, subtrahend: Operand) -> Trace:
         return self.sub(subtrahend)
 
     def __rsub__(self, minuend: Operand) -> Trace:
         """ Returns a new trace with the differences between the *minuend* and
         the signal :attr:`samples`.
 
-        :parameter minuend: iterable or number
+        :param Operand minuend: iterable or number
 
         .. note:: An iterable *minuend* should have at least the same length
             as the signal :attr:`samples`, otherwise only a subset of the signal
             :attr:`samples` is returned!
         """
         return replace(self,
                        label=f'{self.label}:rsub',
                        samples=map(lambda a, b: a - b,
                                    vectorize(minuend), self))
 
     def mul(self, factor: Operand) -> Trace:
         """ Returns a new trace with the products between the signal
         :attr:`samples` and the *factor*.
 
-        :parameter factor: iterable or number
+        :param Operand factor: iterable or number
 
         .. note:: An iterable *factor* should have at least the same length
             as the signal :attr:`samples`, otherwise only a subset of the signal
             :attr:`samples` is returned!
         """
         return replace(self,
                        label=f'{self.label}:mul',
@@ -657,30 +704,30 @@
     def __mul__(self, factor: Operand) -> Trace:
         return self.mul(factor)
 
     def __rmul__(self, factor: Operand) -> Trace:
         """ Returns a new trace with the products between the *factor* and the
         signal :attr:`samples`.
 
-        :parameter factor: iterable or number
+        :param Operand factor: iterable or number
 
         .. note:: An iterable *factor* should have at least the same length
             as the signal :attr:`samples`, otherwise only a subset of the signal
             :attr:`samples` is returned!
         """
         return replace(self,
                        label=f'{self.label}:rmul',
                        samples=map(lambda a, b: a * b,
                                    vectorize(factor), self))
 
     def div(self, divisor: Operand) -> Trace:
         """ Returns a new trace with the quotients between the signal
         :attr:`samples` and the *divisor*.
 
-        :parameter divisor: iterable or number
+        :param Operand divisor: iterable or number
 
         .. note:: An iterable *divisor* should have at least the same length
             as the signal :attr:`samples`, otherwise only a subset of the signal
             :attr:`samples` is returned!
 
         .. note:: Zero-divisions between samples are resolved by returning
             zero for the samples in the new trace where the divisor is zero!
@@ -693,15 +740,15 @@
     def __truediv__(self, divisor: Operand) -> Trace:
         return self.div(divisor)
 
     def __rtruediv__(self, dividend: Operand) -> Trace:
         """ Returns a new trace with the quotients between the *dividend* and
         the signal :attr:`samples`.
 
-        :parameter dividend: iterable or number
+        :param Operand dividend: iterable or number
 
         .. note:: An iterable *dividend* should have at least the same length
             as the signal :attr:`samples`, otherwise only a subset of the signal
             :attr:`samples` is returned!
 
         .. note:: Zero-divisions between samples are resolved by returning
             zero for the samples in the new trace where the divisor is zero!
@@ -711,15 +758,15 @@
                        samples=map(lambda a, b: a / b if b != 0 else 0,
                                    vectorize(dividend), self))
 
     def floordiv(self, divisor: Operand) -> Trace:
         """ Returns a new trace with the integer quotients between the signal
         :attr:`samples` and the *divisor*.
 
-        :parameter divisor: iterable or number
+        :param Operand divisor: iterable or number
 
         .. note:: An iterable *divisor* should have at least the same length
             as the signal :attr:`samples`, otherwise only a subset of the signal
             :attr:`samples` is returned!
 
         .. note:: Zero-divisions between samples are resolved by returning
             zero for the samples in the new trace where the divisor is zero!
@@ -732,15 +779,15 @@
     def __floordiv__(self, divisor: Operand) -> Trace:
         return self.floordiv(divisor)
 
     def __rfloordiv__(self, dividend: Operand) -> Trace:
         """ Returns a new trace with the integer quotients between the
         *dividend* and the signal :attr:`samples`.
 
-        :parameter dividend: iterable or number
+        :param Operand dividend: iterable or number
 
         .. note:: An iterable *dividend* should have at least the same length
             as the signal :attr:`samples`, otherwise only a subset of the signal
             :attr:`samples` is returned!
 
         .. note:: Zero-divisions between samples are resolved by returning
             zero for the samples in the new trace where the divisor is zero!
@@ -752,15 +799,15 @@
 
     def mod(self, divisor: Operand) -> Trace:
         """ Returns a new trace with the remainders between the signal
         :attr:`samples` and the *divisor*.
 
         The sign of the remainders is determined by the *divisor*.
 
-        :parameter divisor: iterable or number
+        :param Operand divisor: iterable or number
 
         .. note:: An iterable *divisor* should have at least the same length
             as the signal :attr:`samples`, otherwise only a subset of the signal
             :attr:`samples` is returned!
 
         .. note:: Zero-divisions between samples are resolved by returning
             zero for the samples in the new trace where the divisor is zero!
@@ -773,15 +820,15 @@
     def __mod__(self, divisor: Operand) -> Trace:
         return self.mod(divisor)
 
     def __rmod__(self, dividend: Operand) -> Trace:
         """ Returns a new trace with the remainders between the *dividend* and
         the signal :attr:`samples`.
 
-        :parameter dividend: iterable or number
+        :param Operand dividend: iterable or number
 
         .. note:: An iterable *dividend* should have at least the same length
             as the signal :attr:`samples`, otherwise only a subset of the signal
             :attr:`samples` is returned!
 
         .. note:: Zero-divisions between samples are resolved by returning
             zero for the samples in the new trace where the divisor is zero!
@@ -793,15 +840,15 @@
 
     def fmod(self, divisor: Operand) -> Trace:
         """ Returns a new trace with the remainders between the signal
         :attr:`samples` and the *divisor*.
 
         The sign of a remainder is determined by the signal sample.
 
-        :parameter divisor: iterable or number
+        :param Operand divisor: iterable or number
 
         .. note:: An iterable *divisor* should have at least the same length
             as the signal :attr:`samples`, otherwise only a subset of the signal
             :attr:`samples` is returned!
 
         .. note:: Zero-divisions between samples are resolved by returning
             zero for the samples in the new trace where the divisor is zero!
@@ -811,15 +858,15 @@
                        samples=map(lambda a, b: math.fmod(a, b) if b != 0 else 0,
                                    self, vectorize(divisor)))
 
     def pow(self, exponent: Operand) -> Trace:
         """ Returns a new trace with the exponentiated values for the signal
         :attr:`samples` raised to the power of the *exponent*.
 
-        :parameter exponent: iterable or number
+        :param Operand exponent: iterable or number
 
         .. note:: An iterable *exponent* should have at least the same length
             as the signal :attr:`samples`, otherwise only a subset of the signal
             :attr:`samples` is returned!
         """
         return replace(self,
                        label=f'{self.label}:pow',
@@ -829,30 +876,30 @@
     def __pow__(self, exponent: Operand) -> Trace:
         return self.pow(exponent)
 
     def __rpow__(self, base: Operand) -> Trace:
         """ Returns a new trace with the exponentiated values for the *base*
         raised to the power of the signal :attr:`samples`.
 
-        :parameter base: iterable or number
+        :param Operand base: iterable or number
 
         .. note:: An iterable *base* should have at least the same length
             as the signal :attr:`samples`, otherwise only a subset of the signal
             :attr:`samples` is returned!
         """
         return replace(self,
                        label=f'{self.label}:rpow',
                        samples=map(lambda a, b: a ** b,
                                    vectorize(base), self))
 
     def bitwise_and(self, operand: Operand) -> Trace:
         """ Returns a new trace with the bitwise ANDed values of the signal
         :attr:`samples` and the *operand*.
 
-        :parameter operand: iterable or number
+        :param Operand operand: iterable or number
 
         .. note:: An iterable *operand* should have at least the same length
             as the signal :attr:`samples`, otherwise only a subset of the signal
             :attr:`samples` is returned!
         """
         return replace(self,
                        label=f'{self.label}:and',
@@ -862,30 +909,30 @@
     def __and__(self, operand: Operand) -> Trace:
         return self.bitwise_and(operand)
 
     def __rand__(self, operand: Operand) -> Trace:
         """ Returns a new trace with the bitwise ANDed values of the *operand*
         and the signal :attr:`samples`.
 
-        :parameter operand: iterable or number
+        :param Operand operand: iterable or number
 
         .. note:: An iterable *operand* should have at least the same length
             as the signal :attr:`samples`, otherwise only a subset of the signal
             :attr:`samples` is returned!
         """
         return replace(self,
                        label=f'{self.label}:rand',
                        samples=map(lambda a, b: int(a) & int(b),
                                    vectorize(operand), self))
 
     def bitwise_or(self, operand: Operand) -> Trace:
         """ Returns a new trace with the bitwise ORed values of the signal
         :attr:`samples` and the *operand*.
 
-        :parameter operand: iterable or number
+        :param Operand operand: iterable or number
 
         .. note:: An iterable *operand* should have at least the same length
             as the signal :attr:`samples`, otherwise only a subset of the signal
             :attr:`samples` is returned!
         """
         return replace(self,
                        label=f'{self.label}:or',
@@ -895,30 +942,30 @@
     def __or__(self, operand: Operand) -> Trace:
         return self.bitwise_or(operand)
 
     def __ror__(self, operand: Operand) -> Trace:
         """ Returns a new trace with the bitwise ORed values of the *operand*
         and the signal :attr:`samples`.
 
-        :parameter operand: iterable or number
+        :param Operand operand: iterable or number
 
         .. note:: An iterable *operand* should have at least the same length
             as the signal :attr:`samples`, otherwise only a subset of the signal
             :attr:`samples` is returned!
         """
         return replace(self,
                        label=f'{self.label}:ror',
                        samples=map(lambda a, b: int(a) | int(b),
                                    vectorize(operand), self))
 
     def bitwise_xor(self, operand: Operand) -> Trace:
         """ Returns a new trace with the bitwise XORed values of the signal
         :attr:`samples` and the *operand*.
 
-        :parameter operand: iterable or number
+        :param Operand operand: iterable or number
 
         .. note:: An iterable *operand* should have at least the same length
             as the signal :attr:`samples`, otherwise only a subset of the signal
             :attr:`samples` is returned!
         """
         return replace(self,
                        label=f'{self.label}:xor',
@@ -928,30 +975,30 @@
     def __xor__(self, operand: Operand) -> Trace:
         return self.bitwise_xor(operand)
 
     def __rxor__(self, operand: Operand) -> Trace:
         """ Returns a new trace with the bitwise XORed values of the *operand*
         and the signal :attr:`samples`.
 
-        :parameter operand: iterable or number
+        :param Operand operand: iterable or number
 
         .. note:: An iterable *operand* should have at least the same length
             as the signal :attr:`samples`, otherwise only a subset of the signal
             :attr:`samples` is returned!
         """
         return replace(self,
                        label=f'{self.label}:rxor',
                        samples=map(lambda a, b: int(a) ^ int(b),
                                    vectorize(operand), self))
 
     def left_shift(self, operand: Operand) -> Trace:
         """ Returns a new trace with the bitwise left-shifted signal
         :attr:`samples` by the *operand*.
 
-        :parameter operand: iterable or number
+        :param Operand operand: iterable or number
 
         .. note:: An iterable *operand* should have at least the same length
             as the signal :attr:`samples`, otherwise only a subset of the signal
             :attr:`samples` is returned!
         """
         return replace(self,
                        label=f'{self.label}:shl',
@@ -961,30 +1008,30 @@
     def __lshift__(self, operand: Operand) -> Trace:
         return self.left_shift(operand)
 
     def __rlshift__(self, operand: Operand) -> Trace:
         """ Returns a new trace with the bitwise left-shifted *operand* by the
         signal :attr:`samples`.
 
-        :parameter operand: iterable or number
+        :param Operand operand: iterable or number
 
         .. note:: An iterable *operand* should have at least the same length
             as the signal :attr:`samples`, otherwise only a subset of the signal
             :attr:`samples` is returned!
         """
         return replace(self,
                        label=f'{self.label}:rshl',
                        samples=map(lambda a, b: int(a) << int(b),
                                    vectorize(operand), self))
 
     def right_shift(self, operand: Operand) -> Trace:
         """ Returns a new trace with the right shifted signal :attr:`samples`
         by the *operand*.
 
-        :parameter operand: iterable or number
+        :param Operand operand: iterable or number
 
         .. note:: An iterable *operand* should have at least the same length
             as the signal :attr:`samples`, otherwise only a subset of the signal
             :attr:`samples` is returned!
         """
         return replace(self,
                        label=f'{self.label}:shr',
@@ -994,26 +1041,29 @@
     def __rshift__(self, operand: Operand) -> Trace:
         return self.right_shift(operand)
 
     def __rrshift__(self, operand: Operand) -> Trace:
         """ Returns a new trace with the right-shifted *operand* by the signal
         :attr:`samples`.
 
-        :parameter operand: iterable or number
+        :param Operand operand: iterable or number
 
         .. note:: An iterable *operand* should have at least the same length
             as the signal :attr:`samples`, otherwise only a subset of the signal
             :attr:`samples` is returned!
         """
         return replace(self,
                        label=f'{self.label}:rshr',
                        samples=map(lambda a, b: int(a) >> int(b),
                                    vectorize(operand), self))
 
-    def bits(self, index: int, number: int = 1, **kwargs) -> Trace:
+    def bits(self,
+             index: int,
+             number: int = 1,
+             **kwargs: Any) -> Trace:
         """ Returns a new trace with the unpacked *number* of bits starting
         at the bit *index* from the signal :attr:`samples` of the trace.
 
         :param int index: start index of the bits to unpack [0..31]
         :param int number: number of bits to unpack [1..32-index].
             Default is ``1``.
         :keyword str label: optional trace label to set
@@ -1096,15 +1146,15 @@
 
     def __irshift__(self, operand: Operand) -> Trace:
         for i, item in enumerate(zip(self, vectorize(operand))):
             self[i] >>= item[1]
         self.label += ':ishr'
         return self
 
-    def neg(self, **kwargs) -> Trace:
+    def neg(self, **kwargs: Any) -> Trace:
         """ Returns a new trace with the negated values of the signal
         :attr:`samples`.
 
         :keyword str label: optional trace label to set
         """
         return replace(self,
                        label=kwargs.get('label', f'{self.label}:neg'),
@@ -1126,42 +1176,51 @@
 
     def __abs__(self) -> Trace:
         """ Returns a new trace with the absolute values of the signal
         :attr:`samples`.
         """
         return self.abs()
 
-    def invert(self, **kwargs) -> Trace:
+    def invert(self, **kwargs: Any) -> Trace:
         """ Returns a new trace with the bitwise inverted values of the signal
         :attr:`samples`.
 
         :keyword str label: optional trace label to set
         """
         return replace(self,
                        label=kwargs.get('label', f'{self.label}:not'),
                        samples=map(lambda item: ~item, self))
 
     def __invert__(self) -> Trace:
         return self.invert()
 
-    def round(self, *args, **kwargs) -> Trace:
+    def round(self,
+              ndigits: Optional[int] = None,
+              **kwargs: Any) -> Trace:
         """ Returns a new trace with the rounded values of the signal
         :attr:`samples`.
+
+        :param int | None ndigits: optional number of digits rounded after the
+            decimal point
+        :keyword str label: optional trace label to set
         """
         return replace(self,
-                       label=f'{self.label}:round',
-                       samples=map(lambda item: round(item, *args, **kwargs), self))
+                       label=kwargs.get('label', f'{self.label}:round'),
+                       samples=map(lambda item: round(item, ndigits), self))
 
-    def __round__(self, *args, **kwargs) -> Trace:
+    def __round__(self, ndigits: Optional[int] = None) -> Trace:
         """ Returns a new trace with the rounded values of the signal
         :attr:`samples`.
+
+        :param int | None ndigits: optional number of digits rounded after the
+            decimal point
         """
-        return self.round(*args, **kwargs)
+        return self.round(ndigits)
 
-    def trunc(self, **kwargs) -> Trace:
+    def trunc(self, **kwargs: Any) -> Trace:
         """ Returns a new trace with the truncated values of the signal
         :attr:`samples`.
 
         :keyword str label: optional trace label to set
         """
         return replace(self,
                        label=kwargs.get('label', f'{self.label}:trunc'),
@@ -1169,95 +1228,95 @@
 
     def __trunc__(self) -> Trace:
         """ Returns a new trace with the truncated values of the signal
         :attr:`samples`.
         """
         return self.trunc()
 
-    def floor(self, **kwargs) -> Trace:
+    def floor(self, **kwargs: Any) -> Trace:
         """ Returns a new trace with the floor, rounded integers of the signal
         :attr:`samples`.
 
         :keyword str label: optional trace label to set
         """
         return replace(self,
                        label=kwargs.get('label', f'{self.label}:floor'),
                        samples=map(math.floor, self))
 
     def __floor__(self) -> Trace:
         return self.floor()
 
-    def ceil(self, **kwargs) -> Trace:
+    def ceil(self, **kwargs: Any) -> Trace:
         """ Returns a new trace with the ceil, rounded integers of the signal
         :attr:`samples`.
 
         :keyword str label: optional trace label to set
         """
         return replace(self,
                        label=kwargs.get('label', f'{self.label}:ceil'),
                        samples=map(math.ceil, self))
 
     def __ceil__(self) -> Trace:
         return self.ceil()
 
-    def sign(self, **kwargs) -> Trace:
+    def sign(self, **kwargs: Any) -> Trace:
         """ Returns a new trace with the signum values of the signal
         :attr:`samples` of the trace.
 
         :keyword str label: optional trace label to set
         """
         return replace(self,
                        label=kwargs.get('label', f'{self.label}:sign'),
                        samples=map(sign, self))
 
-    def zero(self, **kwargs) -> Trace:
+    def zero(self, **kwargs: Any) -> Trace:
         """ Returns a new trace with the test results as integers for testing
         the signal :attr:`samples` to be zero or not.
 
         :keyword str label: optional trace label to set
         """
         return replace(self,
                        label=kwargs.get('label', f'{self.label}:zero'),
                        samples=map(lambda x: int(sign(x) == 0), self))
 
-    def positive(self, **kwargs) -> Trace:
+    def positive(self, **kwargs: Any) -> Trace:
         """ Returns a new trace with the test results as integers for testing
         the signal :attr:`samples` to be positive or not.
 
         :keyword str label: optional trace label to set
         """
         return replace(self,
                        label=kwargs.get('label', f'{self.label}:positive'),
                        samples=map(lambda x: int(sign(x) == 1), self))
 
-    def negative(self, **kwargs) -> Trace:
+    def negative(self, **kwargs: Any) -> Trace:
         """ Returns a new trace with the test results as integers for testing
         the signal :attr:`samples` to be negative or not.
 
         :keyword str label: optional trace label to set
         """
         return replace(self,
                        label=kwargs.get('label', f'{self.label}:negative'),
                        samples=map(lambda x: int(sign(x) == -1), self))
 
-    def delta(self, **kwargs) -> Trace:
+    def delta(self, **kwargs: Any) -> Trace:
         """ Returns a new trace with the deltas between the consecutive signal
         :attr:`samples`.
 
         :keyword str label: optional trace label to set
         :keyword float preset: optional preset value to compute the delta.
             Default is the first value in the signal samples.
         """
         return replace(self,
                        label=kwargs.get('label', f'{self.label}:delta'),
                        samples=map(lambda x: x[1] - x[0], _pairwise(chain(
                            [kwargs.get('preset', self[0] if self else None)],
                            self))))
 
-    def enter_positive(self, **kwargs) -> Trace:
+    def enter_positive(self, **kwargs: Any) -> Trace:
         """ Returns a new trace with the test results as integers for checking
         the signal :attr:`samples` starts to be positive.
 
 
         :keyword str label: optional trace label to set
         :keyword float preset: optional preset value to compute the delta.
             Default is the first value in the signal samples.
@@ -1266,15 +1325,15 @@
         deltas = signs.delta(kwargs=kwargs)
         return replace(self,
                        label=kwargs.get('label', f'{self.label}:enter_positive'),
                        samples=map(
                            lambda signum, delta: int(signum == 1 and delta > 0),
                            signs, deltas))
 
-    def left_positive(self, **kwargs) -> Trace:
+    def left_positive(self, **kwargs: Any) -> Trace:
         """ Returns a new trace with the test results as integers for checking
         the signal :attr:`samples` stops to be positive.
 
         :keyword str label: optional trace label to set
         :keyword float preset: optional preset value to compute the delta.
             Default is the first value in the signal samples.
         """
@@ -1283,15 +1342,15 @@
         return replace(self,
                        label=kwargs.get('label', f'{self.label}:left_positive'),
                        samples=map(lambda signum, delta: int(
                            (signum == 0 and delta == -1) or (
                                signum == -1 and delta == -2)),
                                    signs, deltas))
 
-    def enter_negative(self, **kwargs) -> Trace:
+    def enter_negative(self, **kwargs: Any) -> Trace:
         """ Returns a new trace with the test results as integers for checking
         the signal :attr:`samples` starts to be negative.
 
         :keyword str label: optional trace label to set
         :keyword float preset: optional preset value to compute the delta.
             Default is the first value in the signal samples.
         """
@@ -1299,15 +1358,15 @@
         deltas = signs.delta(kwargs=kwargs)
         return replace(self,
                        label=kwargs.get('label', f'{self.label}:enter_negative'),
                        samples=map(
                            lambda signum, delta: int(signum == -1 and delta < 0),
                            signs, deltas))
 
-    def left_negative(self, **kwargs) -> Trace:
+    def left_negative(self, **kwargs: Any) -> Trace:
         """ Returns a new trace with the test results as integers for checking
         the signal :attr:`samples` stops to be negative.
 
         :keyword str label: optional trace label to set
         :keyword float preset: optional preset value to compute the delta.
             Default is the first value in the signal samples.
         """
@@ -1316,27 +1375,30 @@
         return replace(self,
                        label=kwargs.get('label', f'{self.label}:left_negative'),
                        samples=map(lambda signum, delta: int(
                            (signum == 0 and delta == 1) or (
                                signum == 1 and delta == 2)),
                                    signs, deltas))
 
-    def accumulate(self, func=operator.add, **kwargs) -> Trace:
+    def accumulate(self,
+                   func: Callable[[Number, Number], Number] = operator.add,
+                   **kwargs: Any) -> Trace:
         """ Returns a new trace with the accumulated signal :attr:`samples`.
 
-        :param func: function to use for the accumulation of the samples.
-            Default is the ``+`` operator.
+        :param Callable[[Number, Number], Number] func: function to use for the
+            accumulation of the samples.
+            Default is the function :func:`operator.add`.
         :keyword str label: optional trace label to set
         """
         return replace(self,
                        label=kwargs.get('label', f'{self.label}:accumulate'),
                        samples=accumulate(self,
                                           func=func))
 
-    def sums_positive(self, **kwargs) -> Trace:
+    def sums_positive(self, **kwargs: Any) -> Trace:
         """ Returns a new trace with the integrated signal :attr:`samples`
         limited to positive sums.
 
         :keyword str label: optional trace label to set
         """
         samples = accumulate(self, lambda s, x: s + x if s + x > 0 else 0)
 
@@ -1344,15 +1406,15 @@
             samples = list(samples)
             samples[0] = 0
 
         return replace(self,
                        label=kwargs.get('label', f'{self.label}:sums_positive'),
                        samples=samples)
 
-    def sums_negative(self, **kwargs) -> Trace:
+    def sums_negative(self, **kwargs: Any) -> Trace:
         """ Returns a new trace with the integrated signal :attr:`samples`
         limited to negative sums.
 
         :keyword str label: optional trace label to set
         """
         samples = accumulate(self, lambda s, x: s + x if s + x < 0 else 0)
 
@@ -1360,167 +1422,173 @@
             samples = list(samples)
             samples[0] = 0
 
         return replace(self,
                        label=kwargs.get('label', f'{self.label}:sums_negative'),
                        samples=samples)
 
-    def sin(self, **kwargs) -> Trace:
+    def sin(self, **kwargs: Any) -> Trace:
         """ Returns a new trace with the sines of the signal :attr:`samples`
         in radians.
 
         :keyword str label: optional trace label to set
         """
         return replace(self,
                        label=kwargs.get('label', f'{self.label}:sin'),
                        samples=map(math.sin, self))
 
-    def cos(self, **kwargs) -> Trace:
+    def cos(self, **kwargs: Any) -> Trace:
         """ Returns a new trace with the cosines of the signal :attr:`samples`
         in radians.
 
         :keyword str label: optional trace label to set
         """
         return replace(self,
                        label=kwargs.get('label', f'{self.label}:cos'),
                        samples=map(math.cos, self))
 
-    def tan(self, **kwargs) -> Trace:
+    def tan(self, **kwargs: Any) -> Trace:
         """ Returns a new trace with the tangents of the signal :attr:`samples`
         in radians.
 
         :keyword str label: optional trace label to set
         """
         return replace(self,
                        label=kwargs.get('label', f'{self.label}:tan'),
                        samples=map(math.tan, self))
 
-    def asin(self, **kwargs) -> Trace:
+    def asin(self, **kwargs: Any) -> Trace:
         """ Returns a new trace with the arc sines of the signal
         :attr:`samples`.
 
         :keyword str label: optional trace label to set
         """
         return replace(self,
                        label=kwargs.get('label', f'{self.label}:asin'),
                        samples=map(math.asin, self))
 
-    def acos(self, **kwargs) -> Trace:
+    def acos(self, **kwargs: Any) -> Trace:
         """ Returns a new trace with the arc cosines of the signal
         :attr:`samples`.
 
         :keyword str label: optional trace label to set
         """
         return replace(self,
                        label=kwargs.get('label', f'{self.label}:acos'),
                        samples=map(math.acos, self))
 
-    def atan(self, **kwargs) -> Trace:
+    def atan(self, **kwargs: Any) -> Trace:
         """ Returns a new trace with the arc tangents of the signal
         :attr:`samples`.
 
         :keyword str label: optional trace label to set
         """
         return replace(self,
                        label=kwargs.get('label', f'{self.label}:atan'),
                        samples=map(math.atan, self))
 
-    def sinh(self, **kwargs) -> Trace:
+    def sinh(self, **kwargs: Any) -> Trace:
         """ Returns a new trace with the hyperbolic sines of the signal
         :attr:`samples`.
 
         :keyword str label: optional trace label to set
         """
         return replace(self,
                        label=kwargs.get('label', f'{self.label}:sinh'),
                        samples=map(math.sinh, self))
 
-    def cosh(self, **kwargs) -> Trace:
+    def cosh(self, **kwargs: Any) -> Trace:
         """ Returns a new trace with the hyperbolic cosines of the signal
         :attr:`samples`.
 
         :keyword str label: optional trace label to set
         """
         return replace(self,
                        label=kwargs.get('label', f'{self.label}:cosh'),
                        samples=map(math.cosh, self))
 
-    def tanh(self, **kwargs) -> Trace:
+    def tanh(self, **kwargs: Any) -> Trace:
         """ Returns a new trace with the hyperbolic tangents of the signal
         :attr:`samples`.
 
         :keyword str label: optional trace label to set
         """
         return replace(self,
                        label=kwargs.get('label', f'{self.label}:tanh'),
                        samples=map(math.tanh, self))
 
-    def asinh(self, **kwargs) -> Trace:
+    def asinh(self, **kwargs: Any) -> Trace:
         """ Returns a new trace with the area hyperbolic sines of the
         signal :attr:`samples`.
 
         :keyword str label: optional trace label to set
         """
         return replace(self,
                        label=kwargs.get('label', f'{self.label}:asinh'),
                        samples=map(math.asinh, self))
 
-    def acosh(self, **kwargs) -> Trace:
+    def acosh(self, **kwargs: Any) -> Trace:
         """ Returns a new trace with the area hyperbolic cosines of the
         signal :attr:`samples`.
 
         :keyword str label: optional trace label to set
         """
         return replace(self,
                        label=kwargs.get('label', f'{self.label}:acosh'),
                        samples=map(math.acosh, self))
 
-    def atanh(self, **kwargs) -> Trace:
+    def atanh(self, **kwargs: Any) -> Trace:
         """ Returns a new trace with the area hyperbolic tangents of the
         signal :attr:`samples`.
 
         :keyword str label: optional trace label to set
         """
         return replace(self,
                        label=kwargs.get('label', f'{self.label}:atanh'),
                        samples=map(math.atanh, self))
 
-    def sort(self, *args, **kwargs) -> Trace:
+    def sort(self, **kwargs: Any) -> Trace:
         """ Returns a new trace with the sorted signal :attr:`samples` :math:`N`
         in ascending order.
+
+        :keyword key: function of one argument that is used to extract a
+            comparison key from each sample. Default is ``None``.
+        :keyword bool reverse: if ``True`` the sorted signal :attr:`samples` are
+            returned in descending order.
         """
         return replace(self,
                        label=f'{self.label}:sort',
-                       samples=sorted(self, *args, **kwargs))
+                       samples=sorted(self, **kwargs))
 
     def winsorize(self,
-                  limits: Optional[
-                      Union[float,
-                            tuple[Optional[float], Optional[float]]]] = None,
-                  **kwargs):
+                  limits: (float |
+                           tuple[Optional[float], Optional[float]] |
+                           None) = None,
+                  **kwargs: Any):
         """ Returns a new trace with the winsorized signal :attr:`samples`
         :math:`N`.
 
         The nth-lowest sample values are set to the ``limits[0]``-th percentile
         sample value, and the nth-highest sample values are set to the
         ``(1.0 - limits[1])``-th percentile sample value.
 
         :param limits: either a pair of the percentages as floats between
             ``0.0`` and ``1.0`` to cut on each side of the sorted signal
             samples in ascending order, or the percentage for both sides.
 
             The value of one limit can be set to ``None`` to indicate an open
             interval for this side.
+        :type limits: float | tuple[Optional[float], Optional[float]] | None
         :keyword str label: optional trace label to set
         """
         if not self or limits is None:
             return self
         return replace(self,
                        label=kwargs.get('label', f'{self.label}:winsorize'),
-                       samples=winsorize(self, limits).data)
+                       samples=winsorize(np.array(self), limits).data)
 
     def index_of(self, sample: Sample) -> int:
         """ Returns the *index* of the first occurrence of the *sample* :math:`x`
         in the signal :attr:`samples` :math:`N` or ``-1`` if no sample could be
         found.
 
         :param sample: sample value to look for
@@ -1534,67 +1602,76 @@
         """ Returns the *number* of occurrences of the *sample* :math:`x` in the
         signal :attr:`samples` :math:`N`.
 
         :param sample: sample value to count
         """
         return operator.countOf(self, sample)
 
-    def sum(self, *operands, **kwargs) -> Union[Trace, float]:
+    def sum(self,
+            *operands: Operand,
+            **kwargs: Any) -> Trace | float:
         """ Returns either a new trace with the sums of the signal :attr:`samples`
         and the provided *operands*, or the sum :math:`\\sum\\limits_{i=0}^{N}{x_i}`
         of the signal :attr:`samples` :math:`N` of the trace in case no *operands*
         are provided.
 
         An *operand* can be either a fix number or an array-like iterable.
 
-        :parameter operands: operands to sum up with each signal sample
+        :param operands: operands to sum up with each signal sample
+        :type operands: tuple[Operand, ...]
         :keyword str label: optional trace label to set
 
         .. note:: An iterable *operand* should have at least the same length
             as the signal :attr:`samples`, otherwise only a subset of the signal
             :attr:`samples` is returned!
         """
         if not operands:
             return sum(self)
         return replace(self,
                        label=kwargs.get('label', f'{self.label}:sum'),
                        samples=map(lambda t: sum(t),
                                    zip(self, *map(vectorize, operands))))
 
-    def min(self, *operands: Tuple[Operand], **kwargs) -> Union[Trace, Sample]:
+    def min(self,
+            *operands: Operand,
+            **kwargs: Any) -> Trace | Sample:
         """ Returns either a new trace with the minimums of the signal
         :attr:`samples` and the provided *operands*, or the minimum :math:`x_{min}`
         in the signal :attr:`samples` :math:`N` of the trace in case no *operands*
         are provided.
 
         An *operand* can be either a fix number or an array-like iterable.
 
-        :parameter operands: operands to compare with each signal sample
+        :param Operand operands: operands to compare with each signal sample
+        :type operands: tuple[Operand, ...]
         :keyword str label: optional trace label to set
 
         .. note:: An iterable *operand* should have at least the same length
             as the signal :attr:`samples`, otherwise only a subset of the signal
             :attr:`samples` is returned!
         """
         if not operands:
             return min(self)
         return replace(self,
                        label=kwargs.get('label', f'{self.label}:min'),
                        samples=map(lambda t: min(t),
                                    zip(self, *map(vectorize, operands))))
 
-    def max(self, *operands: Tuple[Operand], **kwargs) -> Union[Trace, Sample]:
+    def max(self,
+            *operands: Operand,
+            **kwargs: Any) -> Trace | Sample:
         """ Returns either a new trace with the maximus of the signal
         :attr:`samples` and the provided *operands*, or the maximum :math:`x_{max}`
         in the signal :attr:`samples` :math:`N` of the trace in case no *operands*
         are provided.
 
         An *operand* can be either a fix number or an array-like iterable.
 
-        :parameter operands: operands to compare with each signal sample
+        :param Operand operands: operands to compare with each signal sample
+        :type operands: tuple[Operand, ...]
         :keyword str label: optional trace label to set
 
         .. note:: An iterable *operand* should have at least the same length
             as the signal :attr:`samples`, otherwise only a subset of the signal
             :attr:`samples` is returned!
         """
         if not operands:
@@ -1610,23 +1687,26 @@
         return max(self) - min(self)
 
     def midrange(self) -> Union[float, int]:
         """ Returns the *midrange* :math:`\\frac{x_{max} + x_{min}}{2}` of the
         signal :attr:`samples` :math:`N`."""
         return (max(self) + min(self)) / 2
 
-    def average(self, *operands, **kwargs) -> Union[Trace, float]:
+    def average(self,
+                *operands: Operand,
+                **kwargs: Any) -> Trace | float:
         """ Returns either a new trace with the averages of the signal
         :attr:`samples` and the provided *operands*, or the average
         :math:`\\overline{x}` of the signal :attr:`samples` :math:`N` of the
         trace in case no *operands* are provided.
 
         An *operand* can be either a fix number or an array-like iterable.
 
-        :parameter operands: operands to compute with each signal sample
+        :param Operand operands: operands to compute with each signal sample
+        :type operands: tuple[Operand, ...]
         :keyword str label: optional trace label to set
 
         .. note:: An iterable *operand* should have at least the same length
             as the signal :attr:`samples`, otherwise only a subset of the signal
             :attr:`samples` is returned!
         """
         if not operands:
@@ -1648,27 +1728,27 @@
         if not n:
             return 0.0
         if n < 2:
             return self[0]
         return (2 / (n * (n + 1))) * sum([w * x for w, x in enumerate(self, 1)])
 
     def winsor_mean(self,
-                    limits: Optional[
-                        Union[float,
-                              tuple[Optional[float], Optional[float]]]] = None
-                    ) -> Union[float, int]:
-        """ Returns the winsorized arithmetic *mean* :math:`\\overline{x}_{w\\alpha}`
-        of the signal :attr:`samples` :math:`N`.
+                    limits: (float |
+                             tuple[Optional[float], Optional[float]] |
+                             None) = None) -> Union[float, int]:
+        """ Returns the winsorized arithmetic *mean*
+        :math:`\\overline{x}_{w\\alpha}` of the signal :attr:`samples` :math:`N`.
 
         :param limits: either a pair of the percentages as floats between
             ``0.0`` and ``1.0`` to cut on each side of the sorted signal
             samples in ascending order, or the percentage for both sides.
 
             The value of one limit can be set to ``None`` to indicate an open
             interval for this side.
+        :type limits: float | tuple[Optional[float], Optional[float]] | None
         """
         samples = self.winsorize(limits)
         return stats.mean(samples) if samples else 0.0
 
     def median(self) -> Union[float, int]:
         """ Returns the median :math:`\\overline{x}_{med}` of the signal
         :attr:`samples` :math:`N`."""
@@ -1698,127 +1778,128 @@
         signal :attr:`samples` :math:`N`."""
         if self:
             center = self.median()
             return sum(map(lambda x: abs(x - center), self)) / len(self)
         else:
             return 0.0
 
-    def variance(self, **kwargs) -> float:
+    def variance(self, **kwargs: Any) -> float:
         """ Returns the biased sample *variance* :math:`\sigma^2` of the signal
         :attr:`samples` :math:`N`.
 
-        :keyword center: optional center value.
+        :keyword float | int center: optional center value.
             Default is the arithmetic :attr:`mean` of the signal :attr:`samples`.
         :keyword bool unbiased: optional if ``True`` computes the unbiased
             *variance* :math:`\sigma^2`. Default is ``False``.
         """
         center = kwargs.get('center', self.mean())
         count = len(self)
 
         if count < 2:
             return 0.0
         if kwargs.get('unbiased', False):
             count -= 1
         return sum(map(lambda x: (x - center) ** 2, self)) / count
 
-    def std(self, **kwargs) -> float:
+    def std(self, **kwargs: Any) -> float:
         """ Returns the biased sample *standard deviation* :math:`\sigma` of the
         signal :attr:`samples` :math:`N`.
 
-        :keyword center: optional center value.
+        :keyword float | int center: optional center value.
             Default is the arithmetic :attr:`mean` of the signal :attr:`samples`.
         :keyword bool unbiased: optional if ``True`` computes the unbiased
             *standard deviation* :math:`\sigma`. Default is ``False``.
         """
         return math.sqrt(self.variance(**kwargs))
 
-    def coefficient(self, **kwargs) -> float:
+    def coefficient(self, **kwargs: Any) -> float:
         """ Returns the *coefficient of variation* :math:`c_v` of the signal
         :attr:`samples` :math:`N`.
 
-        :keyword center: optional center value.
+        :keyword float | int center: optional center value.
             Default is the arithmetic :attr:`mean` of the signal :attr:`samples`.
-        :keyword std: optional standard deviation.
+        :keyword float | int std: optional standard deviation.
             Default is the biased standard deviation :attr:`std` of the signal
             :attr:`samples`.
         :keyword bool unbiased: optional if ``True`` uses the unbiased
             *standard deviation* :math:`\sigma`. Default is ``False``.
         """
         center = kwargs.get('center', self.mean())
         std = kwargs.get('std', self.std(**kwargs))
         return std / center if center else 0.0
 
-    def skew(self, **kwargs) -> float:
+    def skew(self, **kwargs: Any) -> float:
         """ Returns the biased sample *skew* of the signal :attr:`samples`
         :math:`N`.
 
-        :keyword center: optional center value.
+        :keyword float | int center: optional center value.
             Default is the arithmetic :attr:`mean` of the signal :attr:`samples`.
-        :keyword std: optional standard deviation.
+        :keyword float | int std: optional standard deviation.
             Default is the biased standard deviation :attr:`std` of the signal
             :attr:`samples`.
         :keyword bool unbiased: optional if ``True`` uses the unbiased
             *standard deviation* :math:`\sigma`. Default is ``False``.
         """
         center = kwargs.get('center', self.mean())
         std = kwargs.get('std', self.std(**kwargs))
         count = len(self)
         if count < 2 or not std:
             return 0.0
         return sum(map(lambda x: ((x - center) / std) ** 3, self)) / count
 
-    def kurtosis(self, **kwargs) -> float:
+    def kurtosis(self, **kwargs: Any) -> float:
         """ Returns the biased sample *kurtosis* of the signal :attr:`samples`
         :math:`N`.
 
-        :keyword center: optional center value.
+        :keyword float | int center: optional center value.
             Default is the arithmetic :attr:`mean` of the signal :attr:`samples`.
-        :keyword std: optional standard deviation.
+        :keyword float | int std: optional standard deviation.
             Default is the biased standard deviation :attr:`std` of the signal
             :attr:`samples`.
         :keyword bool unbiased: optional if ``True`` uses the unbiased
             *standard deviation* :math:`\sigma`. Default is ``False``.
         """
         center = kwargs.get('center', self.mean())
         std = kwargs.get('std', self.std(**kwargs))
         count = len(self)
         if count < 2 or not std:
             return 0.0
         return sum(map(lambda x: ((x - center) / std) ** 4, self)) / count
 
-    def zscore(self, **kwargs) -> Trace:
+    def zscore(self, **kwargs: Any) -> Trace:
         """ Returns a new trace with the biased z-scored signal :attr:`samples`
         :math:`N`.
 
-        :keyword center: optional center value.
+        :keyword float | int center: optional center value.
             Default is the arithmetic :attr:`mean` of the signal :attr:`samples`.
-        :keyword std: optional biased standard deviation.
+        :keyword float | int std: optional biased standard deviation.
             Default is the biased standard deviation :attr:`std` of the signal
             :attr:`samples`.
         :keyword str label: optional trace label to set
         """
         center = kwargs.get('center', self.mean())
         std = kwargs.get('std', self.std(**kwargs))
         return replace(self,
                        label=kwargs.get('label', f'{self.label}:zscore'),
                        samples=map(lambda x: ((x - center) / std) if std else 0.0,
                                    self))
 
     def clip(self,
              lower: Optional[Operand] = None,
-             upper: Optional[Operand] = None, **kwargs) -> Trace:
+             upper: Optional[Operand] = None,
+             **kwargs: Any) -> Trace:
         """ Returns either a new trace with the signal :attr:`samples` limited
         between the provided *lower* and *upper* bound, or the same trace in case
         no bounds are provided.
 
         A *bound* can be either a fix number or an array-like iterable.
 
-        :param Operand lower: optional lower bound to clip at.
+        :param Operand | None lower: optional lower bound to clip at.
             Default is ``None``, this means the bound is not considered.
-        :param Operand upper: optional upper bound to clip at.
+        :param Operand | None upper: optional upper bound to clip at.
             Default is ``None``, this means the bound is not considered.
         :keyword str label: optional trace label to set
 
         .. note:: The *upper* bound is dominant over the *lower* bound.
 
         .. note:: An iterable *bound* should have at least the same length
             as the signal :attr:`samples`, otherwise only a subset of the signal
@@ -1827,47 +1908,49 @@
         if lower is None and upper is None:
             return self
         return replace(self,
                        label=kwargs.get('label', f'{self.label}:clip'),
                        samples=map(_clip,
                                    self, *map(vectorize, (lower, upper))))
 
-    def clamp(self, bound: Optional[Operand] = None, **kwargs) -> Trace:
+    def clamp(self,
+              bound: Operand | None = None,
+              **kwargs: Any) -> Trace:
         """ Returns either a new trace with the signal :attr:`samples` symmetrically
         clamped at the provided *bound*, or the same trace in case no bound is
         provided.
 
         A *bound* can be either a fix number or an array-like iterable.
 
-        :param Operand bound: optional bound to clamp at.
+        :param Operand | None bound: optional bound to clamp at.
             Default is ``None``, this means the bound is not considered.
         :keyword str label: optional trace label to set
 
         .. note:: An iterable *bound* should have at least the same length
             as the signal :attr:`samples`, otherwise only a subset of the signal
             :attr:`samples` is returned!
         """
         if bound is None:
             return self
         return replace(self,
                        label=kwargs.get('label', f'{self.label}:clamp'),
                        samples=map(_clamp, self, vectorize(bound)))
 
     def interpolate(self,
-                    x: List[Union[int, float]],
-                    y: List[Union[int, float]],
-                    **kwargs) -> Trace:
+                    x: Sequence[Union[int, float]],
+                    y: Sequence[Union[int, float]],
+                    **kwargs: Any) -> Trace:
         """ Returns a new trace with the signal :attr:`samples` of the
         trace piecewise linear interpolated between the data points.
 
         The data points are internally sorted by their x-coordinates to be in
         ascending order.
 
-        :param list x: x-coordinates of the data points.
-        :param list y: y-coordinates of the data points.
+        :param Sequence[int | float] x: x-coordinates of the data points.
+        :param Sequence[int | float] y: y-coordinates of the data points.
         :keyword str label: optional trace label to set
         """
         # sort data points
         x, y = zip(*sorted(zip(x, y)))
 
         if len(x) < 2:
             return self
@@ -1875,15 +1958,15 @@
         return replace(self,
                        label=kwargs.get('label', f'{self.label}:interpolate'),
                        samples=np.interp(self, x, y) if self else list())
 
     def delay(self,
               on: int = 0,
               off: int = 0,
-              **kwargs) -> Trace:
+              **kwargs: Any) -> Trace:
         """ Returns a new trace with the change-rate limited signal
         :attr:`samples` of the binary signal trace.
 
         The change-rate of the binary signal :attr:`samples` is limited by the
         numbers of samples to delay the *on*-state (``1``), and by the numbers
         of samples to delay the *off*-state (``0``) of the binary signal trace.
 
@@ -1924,15 +2007,15 @@
 
         return replace(self,
                        label=kwargs.get('label', f'{self.label}:delay'),
                        samples=samples)
 
     def ramp(self,
              limits: Optional[tuple[Optional[Operand], Optional[Operand]]] = None,
-             **kwargs) -> Trace:
+             **kwargs: Any) -> Trace:
         """ Returns either a new trace with the signal :attr:`samples` limited
         by the maximal allowed positive and/or negative delta *limits* between
         consecutive :attr:`samples`, or the same trace in case no *limits* are
         provided.
 
         The maximal allowed *positive* delta limit can be either a fix number
         or an array-like iterable.
@@ -1941,17 +2024,18 @@
         or an array-like iterable.
 
         :param limits: optional a pair with the maximal allowed positive and
             negative deltas between consecutive samples.
 
             The value of one limit can be set to ``None`` to indicate an
             unlimited ramp for this side.
-        :keyword str label: optional trace label to set
+        :type limits: Optional[tuple[Optional[Operand], Optional[Operand]]]
         :keyword float preset: optional preset value of the ramp.
             Default is the first value in the signal samples.
+        :keyword str label: optional trace label to set
 
         .. note:: An iterable maximal allowed *positive* or *negative* step
             should have at least the same length as the signal :attr:`samples`,
             otherwise only a subset of the signal :attr:`samples` is returned!
         """
         if not limits:
             return replace(self,
@@ -1980,17 +2064,17 @@
             samples.append(level)
 
         return replace(self,
                        label=kwargs.get('label', f'{self.label}:ramp'),
                        samples=samples)
 
     def slew(self,
-             limits: Optional[tuple[Optional[Operand], Optional[Operand]]],
+             limits: tuple[Optional[Operand], Optional[Operand]],
              hold: Optional[Operand] = None,
-             **kwargs) -> SlewRateLimiterTraces:
+             **kwargs: Any) -> SlewRateLimiterTraces:
         """ Slew-rate limiter over the signal :attr:`samples` of the trace.
 
         The maximal allowed *positive* delta limit can be either a fix number
         or an array-like iterable.
 
         The maximal allowed *negative* delta limit can be either a fix number
         or an array-like iterable.
@@ -2000,16 +2084,19 @@
         or an array-like iterable.
 
         :param limits: a pair with the maximal allowed positive and negative
             deltas between consecutive samples.
 
             The value of one limit can be set to ``None`` to indicate an
             unlimited ramp for this side.
-        :param Operand hold: optional number of samples to hold the previous
-            sample value when one of the configured slew-rates becomes violated.
+        :type limits: tuple[Optional[Operand], Optional[Operand]]
+        :param hold: optional number of samples to hold the
+            previous sample value when one of the configured slew-rates becomes
+            violated.
+        :type hold: Operand | None
         :keyword float preset: optional preset value of the limiter.
             Default is the first value in the signal samples.
         :keyword str label: optional trace label to set
         """
         level = kwargs.get('preset', self[0] if self else 0)
         counter = 0
 
@@ -2059,81 +2146,86 @@
         for key, value in as_traces(samples).items():
             traces[key] = replace(self,
                                   label=f'{label}:{key}',
                                   samples=value)
         return SlewRateLimiterTraces(**traces)
 
     def band_pass(self, dt: float, f0: float, q: float = 1 / math.sqrt(2),
-                  **kwargs) -> Trace:
+                  **kwargs: Any) -> Trace:
         """ Returns a new trace with the signal :attr:`samples` filtered with a
         second-order IIR band-pass filter.
 
-        :param dt: sampling-time of the :attr:`~Trace.samples` (filter) in seconds
-        :param f0: center frequency of the filter in Hertz
-        :param q: inverse of bandwidth factor of the filter
+        :param float dt: sampling-time of the :attr:`~Trace.samples` (filter)
+            in seconds
+        :param float f0: center frequency of the filter in Hertz
+        :param float q: inverse of bandwidth factor of the filter
         :keyword str label: optional trace label to set
         """
         _filter = IIRFilter.band_pass(dt, f0, q)
         return replace(self,
                        label=kwargs.get('label', f'{self.label}:band-pass'),
                        samples=map(_filter.compute, self))
 
     def low_pass(self, dt: float, f0: float, q: float = 1 / math.sqrt(2),
-                 **kwargs) -> Trace:
+                 **kwargs: Any) -> Trace:
         """ Returns a new trace with the signal :attr:`samples` filtered with a
         second-order IIR low-pass filter.
 
-        :param dt: sampling-time of the :attr:`~Trace.samples` (filter) in seconds
-        :param f0: cutoff frequency of the filter in Hertz
-        :param q: inverse of bandwidth factor of the filter
+        :param float dt: sampling-time of the :attr:`~Trace.samples` (filter)
+            in seconds
+        :param float f0: cutoff frequency of the filter in Hertz
+        :param float q: inverse of bandwidth factor of the filter
         :keyword str label: optional trace label to set
         """
         _filter = IIRFilter.low_pass(dt, f0, q)
         return replace(self,
                        label=kwargs.get('label', f'{self.label}:low-pass'),
                        samples=map(_filter.compute, self))
 
     def high_pass(self, dt: float, f0: float, q: float = 1 / math.sqrt(2),
-                  **kwargs) -> Trace:
+                  **kwargs: Any) -> Trace:
         """ Returns a new trace with the signal :attr:`samples` filtered with a
         second-order IIR high-pass filter.
 
-        :param dt: sampling-time of the :attr:`~Trace.samples` (filter) in seconds
-        :param f0: cutoff frequency of the filter in Hertz
-        :param q: inverse of bandwidth factor of the filter
+        :param float dt: sampling-time of the :attr:`~Trace.samples` (filter)
+            in seconds
+        :param float f0: cutoff frequency of the filter in Hertz
+        :param float q: inverse of bandwidth factor of the filter
         :keyword str label: optional trace label to set
         """
         _filter = IIRFilter.high_pass(dt, f0, q)
         return replace(self,
                        label=kwargs.get('label', f'{self.label}:high-pass'),
                        samples=map(_filter.compute, self))
 
     def notch(self, dt: float, f0: float, q: float = 1 / math.sqrt(2),
-              **kwargs) -> Trace:
+              **kwargs: Any) -> Trace:
         """ Returns a new trace with the signal :attr:`samples` filtered with a
         second-order IIR notch filter.
 
-        :param dt: sampling-time of the :attr:`~Trace.samples` (filter) in seconds
-        :param f0: center frequency of the filter in Hertz
-        :param q: inverse of bandwidth factor of the filter
+        :param float dt: sampling-time of the :attr:`~Trace.samples` (filter)
+            in seconds
+        :param float f0: center frequency of the filter in Hertz
+        :param float q: inverse of bandwidth factor of the filter
         :keyword str label: optional trace label to set
         """
         _filter = IIRFilter.notch(dt, f0, q)
         return replace(self,
                        label=kwargs.get('label', f'{self.label}:notch'),
                        samples=map(_filter.compute, self))
 
     def all_pass(self, dt: float, f0: float, q: float = 1 / math.sqrt(2),
-                 **kwargs) -> Trace:
+                 **kwargs: Any) -> Trace:
         """ Returns a new trace with the signal :attr:`samples` filtered with a
         second-order IIR all-pass filter.
 
-        :param dt: sampling-time of the :attr:`~Trace.samples` (filter) in seconds
-        :param f0: center frequency of the filter in Hertz
-        :param q: inverse of bandwidth factor of the filter
+        :param float dt: sampling-time of the :attr:`~Trace.samples` (filter)
+            in seconds
+        :param float f0: center frequency of the filter in Hertz
+        :param float q: inverse of bandwidth factor of the filter
         :keyword str label: optional trace label to set
         """
         _filter = IIRFilter.all_pass(dt, f0, q)
         return replace(self,
                        label=kwargs.get('label', f'{self.label}:all-pass'),
                        samples=map(_filter.compute, self))
 
@@ -2144,21 +2236,21 @@
         else:
             factor = _clip(1.0 - ratio, 0.0, 1.0)
         return factor
 
     def dt1(self,
             ratio: Operand,
             gain: Operand = 1,
-            **kwargs) -> Trace:
+            **kwargs: Any) -> Trace:
         """ Returns a new trace with the signal :attr:`samples` of the trace
         processed by the transfer function of a DT1-element.
 
-        :param ratio: integer ratios between damping time and sampling time,
-            or floating-point ratios between sampling time and damping time.
-        :type ratio: int, float
+        :param Operand ratio: integer ratios between damping time and sampling
+            time, or floating-point ratios between sampling time and damping
+            time.
         :param Operand gain: proportional gain of the DT1-element.
         :keyword float preset: optional preset value of the DT1-element.
             Default is the first value in the signal samples.
         :keyword str label: optional trace label to set
         """
         y = kwargs.get('preset', self[0] if self else 0.0)
         previous = self[0] if self else 0.0
@@ -2182,21 +2274,21 @@
         else:
             factor = _clip(ratio, 0.0, 1.0)
         return factor
 
     def pt1(self,
             ratio: Operand,
             gain: Operand = 1,
-            **kwargs) -> Trace:
+            **kwargs: Any) -> Trace:
         """ Returns a new trace with the signal :attr:`samples` of the
         trace processed by the transfer function of a PT1-element.
 
-        :param ratio: integer ratio between smoothing time and sampling time,
-            or floating-point ratio between sampling time and smoothing time.
-        :type ratio: Operand
+        :param Operand ratio: integer ratio between smoothing time and sampling
+            time, or floating-point ratio between sampling time and smoothing
+            time.
         :param Operand gain: proportional gain of the PT1-element.
         :keyword float preset: optional preset value of the PT1-element.
             Default is the first value in the signal samples.
         :keyword str label: optional trace label to set
         """
         y = kwargs.get('preset', self[0] if self else 0.0)
         samples = list()
@@ -2207,15 +2299,87 @@
             y += (value - y) * factor
             samples.append(p * y)
 
         return replace(self,
                        label=kwargs.get('label', f'{self.label}:pt1'),
                        samples=samples)
 
-    def exponential(self, alpha: float, **kwargs) -> ExponentialSmoothingTraces:
+    def alpha_beta_filter(self,
+                          dt: float,
+                          alpha: Operand,
+                          beta: Operand,
+                          **kwargs: Any) -> AlphaBetaFilterTraces:
+        """ Alpha-beta filter over the signal :attr:`samples` of the trace.
+
+        :param float dt: sampling-time of the :attr:`~Trace.samples` (filter)
+            in seconds
+        :param Operand alpha: adaption factor for the level prediction
+            ``[0.0: Ignore signal sample, ..., 1.0[``.
+        :param Operand beta: adaption factor for the trend prediction
+            ``[0.0: Ignore signal sample, ..., 2.0]``.
+        :keyword float level: optional initial level of the alpha-beta filter.
+            Default is the first value in the signal samples.
+        :keyword float trend: optional initial trend of the alpha-beta filter.
+            Default is ``0.0``.
+        :keyword str label: optional trace label to set
+        """
+        # initialize alpha-beta filter
+        level = kwargs.get('level', self.samples[0])
+        trend = kwargs.get('trend', 0.0)
+
+        samples = list()
+        for value, alpha, beta in zip(self.samples,
+                                      vectorize(alpha),
+                                      vectorize(beta)):
+            # Forecast value (prediction)
+            forecast = level + trend * dt
+            # Prediction residual
+            residual = value - forecast
+            # Level value (estimation)
+            level = forecast + (alpha * residual)
+            # Trend value (estimation)
+            trend += (beta * residual) / dt
+
+            denominator = alpha * (4 - 2 * alpha - beta)
+            # Forecast variance reduction factor (prediction)
+            variance_forecast = (2 * alpha ** 2 + 2 * beta + alpha * beta)
+            variance_forecast /= denominator
+            # Level variance reduction factor (estimation)
+            variance_level = (2 * alpha ** 2 + 2 * beta - 3 * alpha * beta)
+            variance_level /= denominator
+            # Trend variance reduction factor (estimation)
+            variance_trend = (2 * beta ** 2) / (dt ** 2)
+            variance_trend /= denominator
+
+            # results of the alpha-beta filter
+            results = AlphaBetaFilter(
+                forecast=forecast,
+                forecast_sign=sign(forecast),
+                level=level,
+                level_sign=sign(level),
+                trend=trend,
+                trend_sign=sign(trend),
+                trend_inflection=sign(level - forecast),
+                error=residual,
+                variance_forecast=variance_forecast,
+                variance_level=variance_level,
+                variance_trend=variance_trend)
+            samples.append(asdict(results))
+
+        traces = dict()
+        label = kwargs.get('label', f'{self.label}:filter')
+        for key, value in as_traces(samples).items():
+            traces[key] = replace(self,
+                                  label=f'{label}:{key}',
+                                  samples=value)
+        return AlphaBetaFilterTraces(**traces)
+
+    def exponential(self,
+                    alpha: float,
+                    **kwargs: Any) -> ExponentialSmoothingTraces:
         """ Second-order exponential smoothing over the signal
         :attr:`samples` of the trace.
 
         :param float alpha: smoothing factor ``[0.0:freeze..1.0:transparent]``
         :keyword float level: optional initial level of the exponential smoothing.
             Default is the first value in the signal samples.
         :keyword float trend: optional initial trend of the exponential smoothing.
@@ -2228,34 +2392,34 @@
         alpha = _clip(alpha, 0.0, 1.0)
         prognosis = [
             (level - ((1 - alpha) / alpha) * trend if alpha > 0 else 0),
             (level - 2 * ((1 - alpha) / alpha) * trend if alpha > 0 else 0)
         ]
 
         # initialize signal statistic
-        absolute = 0.0
+        absolute_error = 0.0
         variance = 0.0
         skew = 0.0
         kurtosis = 0.0
         samples = list()
         for value in self.samples:
-            # prognosis error
-            error = value - ((2 * prognosis[0] - prognosis[1]) + trend)
+            # prognosis residual
+            residual = value - ((2 * prognosis[0] - prognosis[1]) + trend)
             # empirical absolute error of the distribution (1st central moment)
-            absolute_error = (1 - alpha) * (absolute + alpha * abs(error))
+            absolute_error = (1 - alpha) * (absolute_error + alpha * abs(residual))
             # empirical variance of the distribution (2nd central moment)
-            variance = (1 - alpha) * (variance + alpha * (error ** 2))
+            variance = (1 - alpha) * (variance + alpha * (residual ** 2))
             # empirical standard deviation of the distribution
             deviation = math.sqrt(variance)
             # empirical skew of the distribution (3rd central moment)
             skew = (1.0 - alpha) * (skew + alpha * (
-                (error / deviation) ** 3 if deviation != 0.0 else 0.0))
+                (residual / deviation) ** 3 if deviation != 0.0 else 0.0))
             # empirical kurtosis of the distribution (4th central moment)
             kurtosis = (1.0 - alpha) * (kurtosis + alpha * (
-                (error / deviation) ** 4 if deviation != 0.0 else 0.0))
+                (residual / deviation) ** 4 if deviation != 0.0 else 0.0))
             # first-order exponentially smoothed value
             smoothed1 = (1.0 - alpha) * prognosis[0] + alpha * value
             # second-order exponentially smoothed value
             smoothed2 = (1.0 - alpha) * prognosis[1] + alpha * smoothed1
             # prognosis level (exponentially smoothed signal value)
             level = 2 * smoothed1 - smoothed2
             # prognosis trend
@@ -2273,16 +2437,16 @@
                 prognosis2=prognosis[1],
                 prognosis=2 * prognosis[0] - prognosis[1],
                 smoothed1=smoothed1,
                 smoothed2=smoothed2,
                 trend=trend,
                 trend_sign=sign(trend),
                 trend_inflection=sign(forecast - level),
-                error=error,
-                correction=alpha * error,
+                error=residual,
+                correction=alpha * residual,
                 absolute_error=absolute_error,
                 variance=variance,
                 deviation=deviation,
                 skew=skew,
                 kurtosis=kurtosis)
             # new prognosis values
             prognosis = [smoothed1, smoothed2]
@@ -2292,15 +2456,17 @@
         label = kwargs.get('label', f'{self.label}:exponential')
         for key, value in as_traces(samples).items():
             traces[key] = replace(self,
                                   label=f'{label}:{key}',
                                   samples=value)
         return ExponentialSmoothingTraces(**traces)
 
-    def window(self, size: int, **kwargs) -> Iterator[Tuple[Sample, ...]]:
+    def window(self,
+               size: int,
+               **kwargs: Any) -> Iterator[tuple[Sample, ...]]:
         """ Moving window generator over the signal :attr:`samples` of the trace.
 
         :param int size: moving window size (number of samples)
         :keyword float preset: optional preset value to fill the moving window.
             Default is the first value in the signal samples.
         """
         if not self or size <= 0:
@@ -2309,17 +2475,18 @@
             # moving windows iterator
             windows = tee(
                 chain(repeat(kwargs.get('preset', self[0]), size - 1),
                       iter(self)), size)
             yield from zip(
                 *(islice(window, i, None) for i, window in enumerate(windows)))
 
-    def moving_events(self, size: int,
+    def moving_events(self,
+                      size: int,
                       value: Sample = 1,
-                      **kwargs) -> Trace:
+                      **kwargs: Any) -> Trace:
         """ Returns a new trace with the number of *value* occurrences (events)
         in the moving window over the signal :attr:`samples` of the trace.
 
         :param int size: moving window size
         :param value: value to check. Default is ``1``.
         :keyword int preset: optional preset value to fill the moving window.
             Default is ``None``.
@@ -2328,15 +2495,17 @@
         samples = list()
         for values in self.window(size, preset=kwargs.get('preset', None)):
             samples.append(list(values).count(value))
         return replace(self,
                        label=kwargs.get('label', f'{self.label}:events'),
                        samples=samples)
 
-    def moving_average(self, size: int, **kwargs) -> MovingAverageTraces:
+    def moving_average(self,
+                       size: int,
+                       **kwargs: Any) -> MovingAverageTraces:
         """ Moving average over the signal :attr:`samples` of the trace.
 
         :param int size: moving window size (number of samples)
         :keyword float preset: optional preset value to fill the moving window.
             Default is the first value in the signal samples.
         """
         samples = list()
@@ -2367,37 +2536,47 @@
         traces = dict()
         label = kwargs.get('label', f'{self.label}:average')
         for key, value in as_traces(samples).items():
             traces[key] = Trace(label=f'{label}:{key}',
                                 samples=value)
         return MovingAverageTraces(**traces)
 
-    def moving_differential(self, size: int, **kwargs) -> Trace:
+    def moving_differential(self,
+                            size: int,
+                            **kwargs: Any) -> Trace:
         """ Moving differential over the signal :attr:`samples` of the trace.
 
         :param int size: moving window size (number of samples)
         :keyword float preset: optional preset value to fill the moving window.
             Default is the first value in the signal samples.
         :keyword str label: optional trace label to set
         """
         return replace(self,
                        label=kwargs.get('label', f'{self.label}:differential'),
                        samples=[((y[-1] - y[0]) / (size - 1)) if
                                 size > 1 else 0 for y in
                                 self.window(size, **kwargs)])
 
-    def moving_regression(self, size: int, **kwargs) -> LinearRegressionTraces:
+    def moving_regression(self,
+                          size: int,
+                          **kwargs: Any) -> LinearRegressionTraces:
         """ Moving linear regression over the signal :attr:`samples` of the
         trace.
 
-        :param int size: moving window size
+        :param int size: moving window size (> 1)
         :keyword float preset: optional preset value to fill the moving window.
             Default is the first value in the signal samples.
         :keyword str label: optional trace label to set
         """
+        if not self.samples:
+            return LinearRegressionTraces()
+
+        if size < 2:
+            return LinearRegressionTraces(level=self)
+
         samples = list()
         # x-coordinate values
         x_values = list(range(size))
         for y_values in self.window(size, **kwargs):
             # arithmetic mean of the x-coordinate values
             mean_x = stats.mean(x_values)
             # arithmetic mean of the y-coordinate values (1st central moment)
@@ -2472,15 +2651,17 @@
         label = kwargs.get('label', f'{self.label}:regression')
         for key, value in as_traces(samples).items():
             traces[key] = replace(self,
                                   label=f'{label}:{key}',
                                   samples=value)
         return LinearRegressionTraces(**traces)
 
-    def move(self, number: int, **kwargs) -> Trace:
+    def move(self,
+             number: int,
+             **kwargs: Any) -> Trace:
         """ Returns a new trace with the moved signal :attr:`samples` by the
         number of samples either to the right or to the left.
 
         A positive *number* moves the signal :attr:`samples` to the right. This
         means a *number* of the first value in signal :attr:`samples` is inserted
         at the beginning of the signal :attr:`samples` to move as the *fill*
         value, and the *number* of the last signal :attr:`samples` are removed
@@ -2490,45 +2671,48 @@
         means a *number* of the last value in the signal :attr:`samples` is
         appended at end of the signal :attr:`samples` to move as the *fill*
         value, and the *number* of the first signal :attr:`samples` are removed
         from the signal :attr:`samples` to move.
 
         :param int number: number of samples to move to the right (``> 0``) or
             to the left (``< 0``).
-        :keyword str label: optional trace label to set
         :keyword float fill: optional fill value.
             Default is the first or last value in the signal samples.
+        :keyword str label: optional trace label to set
         """
         # copy samples
         samples = self[:]
         if not samples or not number:
             # nothing to move
             pass
         elif number > 0:
             # move to right
             number = min(number, len(samples))
-            fill = kwargs.get('fill', self[0])
+            fill = kwargs.get('fill', samples[0])
             samples = [fill] * number + samples[:-number]
         elif number < 0:
             # move to left
             number = min(-number, len(samples))
-            fill = kwargs.get('fill', self[-1])
-            samples = samples[number:] + [fill] * number
+            fill = kwargs.get('fill', samples[-1])
+            samples = samples[number:]
+            samples += [fill] * number
 
         return replace(self,
                        label=kwargs.get('label', f'{self.label}:move'),
                        samples=samples)
 
-    def slice(self, *args, **kwargs) -> Trace:
+    def slice(self,
+              *args: tuple[int, ...],
+              **kwargs: Any) -> Trace:
         """ Returns a new trace with the signal :attr:`samples` sliced with the
         built-in function :func:`slice` in the range given by the arguments
         *args*.
 
-        :param args: optional *start*, *stop* index and *step* for slicing the
-            signal :attr:`samples`.
+        :param tuple[int, ...] args: optional *start*, *stop* index and *step*
+            for slicing the signal :attr:`samples`.
         :keyword str label: optional trace label to set
         """
         if not args:
             samples = self.samples[:]
         else:
             samples = self.samples[slice(*args)]
         return replace(self,
@@ -2543,39 +2727,39 @@
     def iter_point(self) -> Iterator[Point2D]:
         """ Returns an iterator for the x,y-points of the trace.
         """
         for x, y in zip(self.iter_x(), self):
             yield Point2D(x, y)
 
     @property
-    def x_values(self) -> List[int]:
+    def x_values(self) -> list[int]:
         """ Returns a list with the x-coordinates of the trace.
         """
         return list(self.iter_x())
 
     @property
-    def y_values(self) -> List(Sample):
+    def y_values(self) -> list[Sample]:
         """ Returns a list with the y-coordinates of the trace.
         """
         return list(self)
 
     @property
     def digital(self) -> Digital:
         """ Returns a new digital trace with *shared* signal :attr:`samples`.
         """
         return Digital(**asdict(self))
 
     def plot(self,
              index: Optional[int] = None,
              n: Optional[int] = None,
-             **kwargs) -> go.Scatter:
+             **kwargs: Any) -> go.Scatter:
         """ Returns the scatter plot of the trace.
 
-        :param int index: start index of the samples to plot
-        :param n: number of samples to plot
+        :param int index: optional start index of the samples to plot
+        :param int n: optional number of samples to plot
         """
         # pack x,y-pairs
         pairs = list(zip(self.iter_x(), self))
         if pairs:
             # slice pairs
             index = 0 if index is None else max(0, index)
             if n is None:
@@ -2602,36 +2786,36 @@
         _plot = go.Scatter(**settings)
         # update plot
         return _plot.update(kwargs)
 
     def figure(self,
                index: Optional[int] = None,
                n: Optional[int] = None,
-               **kwargs) -> go.Figure:
+               **kwargs: Any) -> go.Figure:
         """ Returns a figure with the scatter plot of the trace.
 
-        :param int index: start index of the samples to plot
-        :param n: number of samples to plot
+        :param int index: optional start index of the samples to plot
+        :param int n: optional number of samples to plot
         """
         return go.Figure(self.plot(index, n, **kwargs))
 
 
 @dataclass
 class Digital(Trace):
     """ Trace data class for time-discrete digital signal samples.
     """
 
     def plot(self,
              index: Optional[int] = None,
              n: Optional[int] = None,
-             **kwargs) -> go.Scatter:
+             **kwargs: Any) -> go.Scatter:
         """ Returns the plot of the digital signal trace.
 
-        :param int index: start index of the samples to plot
-        :param n: number of samples to plot
+        :param int index: optional start index of the samples to plot
+        :param int n: optional number of samples to plot
         """
         # pack x,y-pairs
         pairs = list(zip(self.iter_x(), self))
 
         if pairs:
             # slice pairs
             index = 0 if index is None else max(0, index)
@@ -2659,19 +2843,20 @@
 
         # create plot with default settings
         _plot = go.Scatter(**settings)
         # update plot
         return _plot.update(kwargs)
 
 
-def logical_and(*operands: Tuple[Iterable], **kwargs) -> Trace:
+def logical_and(*operands: Trace | Iterable,
+                **kwargs: Any) -> Trace:
     """ Returns a new trace with the logical ANDed values of the given iterable
     *operands*.
 
-    :parameter operands: trace or iterable
+    :param Trace | Iterable] operands: trace or iterable
     :keyword str label: optional trace label to set.
         Default is ``'And'``.
 
     .. note:: The *operands* should have the same length, otherwise only a
         subset of the signal :attr:`samples` is returned!
     """
     label = kwargs.get('label', 'And')
@@ -2679,19 +2864,20 @@
         return Trace(label)
     samples = list()
     for t in zip(*operands):
         samples.append(int(all(t)))
     return Trace(label, samples)
 
 
-def logical_or(*operands: Tuple[Iterable], **kwargs) -> Trace:
+def logical_or(*operands: Trace | Iterable,
+               **kwargs: Any) -> Trace:
     """ Returns a new trace with the logical ORed values of the given iterable
     *operands*.
 
-    :parameter operands: trace or iterable
+    :param Trace | Iterable operands: trace or iterable
     :keyword str label: optional trace label to set.
         Default is ``'Or'``.
 
     .. note:: The *operands* should have the same length, otherwise only a
         subset of the signal :attr:`samples` is returned!
     """
     label = kwargs.get('label', 'Or')
@@ -2699,27 +2885,28 @@
         return Trace(label)
     samples = list()
     for t in zip(*operands):
         samples.append(int(any(t)))
     return Trace(label, samples)
 
 
-def priority(*operands: Tuple[Iterable], **kwargs) -> Trace:
+def priority(*operands: Trace | Iterable,
+             **kwargs: Any) -> Trace:
     """ Returns a new trace with the priority numbers defined by the order of
     the given *operands*, and determined from the ``Truth=1`` values of the
     given *operands*.
 
     The priority starts with ``0`` as the *highest* priority number for the
     ``Truth=1`` values of the first given iterable operand to the lowest
     priority number determined by the number of the given *operands*.
 
     The iterable *operands* must contain either boolean values or integer
     values ``1`` or ``0``.
 
-    :parameter operands: trace or iterable to prioritize
+    :param Trace | Iterable operands: trace or iterable to prioritize
     :keyword int highest: optional number for the highest priority.
         Default is ``0``.
     :keyword str label: optional trace label to set.
         Default is ``'Priority'``.
 
     .. note:: The *operands* should have the same length, otherwise only a
         subset of the signal :attr:`samples` is returned!
@@ -2736,69 +2923,68 @@
         try:
             samples.append(tuple(map(int, t)).index(1) + highest)
         except ValueError:
             samples.append(lowest)
     return Trace(label, samples)
 
 
-def as_traces(samples: List[Dict[str, Any]]) -> Dict[str, List[Any]]:
+def as_traces(samples: Sequence[dict[str, Any]]) -> dict[str, list[Sample]]:
     """ Converts the list of samples into the trace format."""
     if not samples:
         return dict()
-    samples = samples
     names = list(samples[0].keys())
     trace = defaultdict(list)
     for sample in samples:
         for name in names:
             trace[name].append(sample[name])
     return dict(trace)
 
 
 @dataclass(eq=False)
 class Traces(MutableMapping):
     """ Base data class for a collection of traces with mutable mapping support.
     """
 
-    def labels(self) -> Tuple[str, ...]:
+    def labels(self) -> tuple[str, ...]:
         """ Returns a tuple of the trace labels in the collection."""
         return tuple([trace.label for trace in self.values()])
 
     def relabel(self, label: str) -> Traces:
         """ Relabels the all traces with in the collection by keeping the last
         part of the trace :attr:`~Trace.label` unchanged and the rest replaced
         by the base *label*.
 
-        :param str label: base label to set for the traces in the collection.
+        :param str label: base label to set for the traces in the collection
         """
         for field_ in fields(self):
             trace = getattr(self, field_.name)
             if isinstance(trace, Trace):
                 trace.label = f"{label}:{trace.label.split(':')[-1]}"
         return self
 
     def __setitem__(self, key: str, value: Trace):
         self.__dict__[key] = value
 
-    def __getitem__(self, key) -> Trace:
+    def __getitem__(self, key: str) -> Trace:
         return self.__dict__[key]
 
-    def __delitem__(self, key):
+    def __delitem__(self, key: str):
         raise NotImplemented()
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator[str]:
         return iter(self.__dict__)
 
     def __len__(self) -> int:
         return len(self.__dict__)
 
-    def fields(self) -> Tuple[Any, ...]:
+    def fields(self) -> tuple[Field, ...]:
         """ Returns a tuple describing the fields of the data class."""
         return fields(self)
 
-    def as_dict(self) -> Dict[str, Any]:
+    def as_dict(self) -> dict[str, Any]:
         """ Returns the collection of traces as a dictionary.
         """
         return asdict(self)
 
     def as_tuple(self) -> tuple[Any, ...]:
         """ Returns the collection of traces as a tuple.
         """
@@ -2841,21 +3027,22 @@
     #: Empirical biased sample kurtosis of the set (4th central moment).
     kurtosis: Trace = field(default_factory=Trace)
 
     def figure(self,
                index: Optional[int] = None,
                n: Optional[int] = None,
                original: Optional[Trace] = None,
-               subplots: Optional[Dict[str, Any]] = None) -> go.Figure:
+               subplots: Optional[dict[str, Any]] = None) -> go.Figure:
         """ Returns a figure of subplots for the traces in the collection.
 
-        :param int index: start index of the samples to plot
-        :param n: number of samples to plot
+        :param int index: optional start index of the samples to plot
+        :param int n: optional number of samples to plot
         :param Trace original: optional original trace to add to the plot
-        :param dict subplots: dictionary with the settings for the subplots
+        :param dict subplots: optional dictionary with the settings for the
+            subplots
         """
         # base subplots configuration
         subplots_ = dict(
             rows=6,
             cols=1,
             shared_xaxes=True,
             row_heights=(3, 1, 1, 1, 1, 1),
@@ -2924,41 +3111,46 @@
 
 @dataclass(eq=False)
 class SetTraces(StatisticsTraces):
     """ Collection of :class:`Statistics` traces for the combined set of
     multiple signal samples."""
 
     @classmethod
-    def from_traces(cls, *operands: Tuple[Operand], **kwargs) -> SetTraces:
+    def from_traces(cls,
+                    *operands: Operand,
+                    **kwargs: Any) -> SetTraces:
         """ Returns the collection of :class:`Statistics` traces computed over
         the combined sets of the *operands*.
 
         An operand can be either a number or an array-like iterable.
 
         :param operands: operands to compute the statistics with
+        :type operands: tuple[Operand, ...]
         :keyword str label: optional traces base label to set
 
         .. note:: All iterable *operands* must have the same length, otherwise
             only a subset of the operand values is returned!
         """
         instance = cls(**combine(*operands, **kwargs))
         label = kwargs.get('label')
         if label is not None:
             return instance.relabel(label)
         else:
             return instance
 
 
-def combine(*operands: Tuple[Operand], **kwargs) -> Dict[str, Trace]:
+def combine(*operands: Operand,
+            **kwargs: Any) -> dict[str, Trace]:
     """ Returns a dictionary with the traces for the statistics results computed
     over the combined sets of *operands*.
 
     An operand can be either a number or an array-like iterable.
 
-    :param operands: operands to compute the statistics with
+    :param Operand operands: operands to compute the statistics with
+    :type operands: tuple[Operand, ...]
     :keyword str label: optional trace label stem to set
 
     .. note:: All iterable *operands* must have the same length, otherwise
         only a subset of the operand values is returned!
     """
     if not operands:
         return dict()
@@ -3037,48 +3229,61 @@
     represented in polar coordinates.
     """
     #: Trace with cartesian x-coordinates of the vector
     x: Trace = field(default_factory=Trace)
     #: Trace with cartesian y-coordinates of the vector
     y: Trace = field(default_factory=Trace)
     #: Trace with radii of the vector
-    r: Optional[Trace] = field(default=None)
+    r: Trace | None = field(default=None)
     #: Trace with angles of the vector in radians [-pi..pi]
-    phi: Optional[Trace] = field(default=None)
+    phi: Trace | None = field(default=None)
     #: Trace with angles of the vector in degree [0..360].
-    theta: Optional[Trace] = field(default=None)
+    theta: Trace | None = field(default=None)
+    #: Trace with delta angles of the consecutive x,y-points in radians [-pi..pi]
+    delta_phi: Trace | None = field(default=None)
     #: Trace with euclidean distances of the consecutive x,y-points.
-    distance: Optional[Trace] = field(default=None)
+    distance: Trace | None = field(default=None)
     #: Trace with dot products of the consecutive x,y-points.
-    dot: Optional[Trace] = field(default=None)
+    dot: Trace | None = field(default=None)
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         # dictionary with the vector results
         vector = polar(self.x, self.y)
         if self.r is None:
             self['r'] = vector.get('r', Trace(label='Vector:r'))
         if self.phi is None:
             self['phi'] = vector.get('phi', Trace(label='Vector:phi'))
         if self.theta is None:
             self['theta'] = vector.get('theta', Trace(label='Vector:theta'))
+        self.delta_phi = Trace('Vector:delta_phi')
         self.distance = Trace('Vector:distance')
         self.dot = Trace('Vector:dot')
+
+        for angles in self.phi.window(2):
+            # angular velocity
+            omega = angles[1] - angles[0]
+            if omega > math.pi:
+                omega -= 2 * math.pi
+            elif omega < -math.pi:
+                omega += 2 * math.pi
+            self.delta_phi.samples.append(omega)
+
         for coordinates in zip(self.x.window(2), self.y.window(2)):
             points = [(x, y) for x, y in zip(coordinates[0], coordinates[1])]
             self.distance.samples.append(math.dist(*points))
             self.dot.samples.append(np.dot(*points))
 
     def plot(self,
              index: Optional[int] = None,
              n: Optional[int] = None,
-             **kwargs) -> go.Scatterpolar:
+             **kwargs: Any) -> go.Scatterpolar:
         """ Returns the scatter polar plot of the vector traces.
 
-        :param int index: start index of the samples to plot
-        :param n: number of samples to plot
+        :param int index: optional start index of the samples to plot
+        :param int n: optional number of samples to plot
         """
         # pack r,theta-pairs
         pairs = list(zip(self.r, self.theta))
 
         if pairs:
             # slice pairs
             index = 0 if index is None else max(0, index)
@@ -3104,15 +3309,15 @@
         )
         # create plot with default settings
         _plot = go.Scatterpolar(**settings)
         # update plot
         return _plot.update(kwargs)
 
 
-def polar(x: Trace, y: Trace, **kwargs) -> Dict[str, Trace]:
+def polar(x: Trace, y: Trace, **kwargs: Any) -> dict[str, Trace]:
     """ Returns a dictionary with the traces for the two *x*, *y* signal samples
     converted into a vector represented in polar coordinates.
 
     :param Trace x: cartesian x-coordinate signal trace of the vector
     :param Trace y: cartesian y-coordinate signal trace of the vector
     :keyword str label: optional traces base label to set.
         Default is ``Vector``.
@@ -3140,15 +3345,15 @@
     #: Radius of the vector.
     r: float = 0.0
     #: Angle of the vector in radians [-pi..+pi].
     phi: float = 0.0
     #: Angle of the vector in degrees [0..360].
     theta: Optional[float] = None
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         if self.theta is None:
             angel = float(np.degrees(self.phi))
             self.theta = angel + 360.0 if angel < 0.0 else angel
 
 
 @dataclass(eq=True, order=True)
 class Point2D:
@@ -3174,28 +3379,28 @@
         angel = float(np.degrees(self.phi))
         return angel + 360.0 if angel < 0 else angel
 
     def as_vector(self):
         """ Returns a :class:`Vector` for the 2-dimensional point."""
         return Vector(self.r, self.phi)
 
-    def as_dict(self) -> Dict[str, Any]:
+    def as_dict(self) -> dict[str, Any]:
         """ Returns the 2-dimensional point as a dictionary."""
         return asdict(self)
 
     def as_tuple(self) -> tuple[Any, ...]:
         """ Returns the 2-dimensional point as a tuple."""
         return astuple(self)
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator[tuple[int, float]]:
         """ Returns an iterator over the coordinates of the 2-dimensional point.
         """
         return iter(astuple(self))
 
-    def __reversed__(self):
+    def __reversed__(self) -> Iterator[tuple[int, float]]:
         """ Returns a reverse iterator over the coordinates of the 2-dimensional
         point.
         """
         return reversed(astuple(self))
 
 
 @dataclass(eq=True, order=True)
@@ -3205,32 +3410,32 @@
     x: int = 0.0
     #: Y-coordinate of the 3-dimensional point.
     y: float = 0.0
     #: Z-coordinate of the 3-dimensional point.
     z: float = 0.0
 
     @property
-    def r(self):
+    def r(self) -> float:
         """ Radius of the 3-dimensional point."""
         return math.hypot(self.x, self.y, self.z)
 
-    def as_dict(self) -> Dict[str, Any]:
+    def as_dict(self) -> dict[str, Any]:
         """ Returns the 3-dimensional point as a dictionary."""
         return asdict(self)
 
     def as_tuple(self) -> tuple[Any, ...]:
         """ Returns the 3-dimensional point as a tuple."""
         return astuple(self)
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator[tuple[int, float, float]]:
         """ Returns an iterator over the coordinates of the 3-dimensional point.
         """
         return iter(astuple(self))
 
-    def __reversed__(self):
+    def __reversed__(self) -> Iterator[tuple[int, float, float]]:
         """ Returns a reverse iterator over the coordinates of the 3-dimensional
         point.
         """
         return reversed(astuple(self))
 
 
 @dataclass(eq=False)
@@ -3244,21 +3449,22 @@
     #: Slew-rate limiter active ``(0: signal unlimited, 1: signal limited)``.
     active: Trace = field(default_factory=Trace)
 
     def figure(self,
                index: Optional[int] = None,
                n: Optional[int] = None,
                original: Optional[Trace] = None,
-               subplots: Optional[Dict[str, Any]] = None) -> go.Figure:
+               subplots: Optional[dict[str, Any]] = None) -> go.Figure:
         """ Returns a figure of subplots for the traces.
 
-        :param int index: start index of the samples to plot
-        :param n: number of samples to plot
+        :param int index: optional start index of the samples to plot
+        :param int n: optional number of samples to plot
         :param Trace original: optional original trace to add to the plot
-        :param dict subplots: dictionary with the settings for the subplots
+        :param dict subplots: optional dictionary with the settings for the
+            subplots
         """
         # base subplots configuration
         subplots_ = dict(
             rows=3,
             cols=1,
             shared_xaxes=True,
             row_heights=(2, 0.5, 0.25),
@@ -3300,14 +3506,137 @@
     #: Signal deviation.
     deviation: float = 0.0
     #: Slew-rate limiter active ``(0: signal unlimited, 1: signal limited)``.
     active: int = 0
 
 
 @dataclass(eq=False)
+class AlphaBetaFilterTraces(Traces):
+    """ Collection of :class:`AlphaBetaFilter` traces for signal samples
+    filtered with an alpha-beta filter. """
+    #: Signal forecast value.
+    forecast: Trace = field(default_factory=Trace)
+    #: Sign of the signal forecast ``(-1: negative, 0: zero, 1: positive)``.
+    forecast_sign: Trace = field(default_factory=Trace)
+    #: Signal level value.
+    level: Trace = field(default_factory=Trace)
+    #: Sign of the signal level ``(-1: negative, 0: zero, 1: positive)``.
+    level_sign: Trace = field(default_factory=Trace)
+    #: Signal trend value.
+    trend: Trace = field(default_factory=Trace)
+    #: Sign of the signal trend ``(-1: negative, 0: zero, 1: positive)``.
+    trend_sign: Trace = field(default_factory=Trace)
+    #: Inflection of the signal prognosis trend ``(1: increase, -1: decrease)``.
+    trend_inflection: Trace = field(default_factory=Trace)
+    #: Signal prognosis error.
+    error: Trace = field(default_factory=Trace)
+    #: Signal forecast variance reduction factor.
+    variance_forecast: Trace = field(default_factory=Trace)
+    #: Signal level variance reduction factor.
+    variance_level: Trace = field(default_factory=Trace)
+    #: Signal trend variance reduction factor.
+    variance_trend: Trace = field(default_factory=Trace)
+
+    def figure(self,
+               index: Optional[int] = None,
+               n: Optional[int] = None,
+               original: Optional[Trace] = None,
+               subplots: Optional[dict[str, Any]] = None) -> go.Figure:
+        """ Returns a figure of subplots for the traces.
+
+        :param int index: optional start index of the samples to plot
+        :param int n: optional number of samples to plot
+        :param Trace original: optional original trace to add to the plot
+        :param dict subplots: optional dictionary with the settings for the
+            subplots
+        """
+        # base subplots configuration
+        subplots_ = dict(
+            rows=8,
+            cols=1,
+            shared_xaxes=True,
+            row_heights=(3, 0.25, 0.25, 1.25, 0.25, 0.25, 1, 0.25),
+            vertical_spacing=0.01,
+            x_title='samples')
+
+        if subplots is not None:
+            subplots_.update(subplots)
+        fig = make_subplots(**subplots_)
+
+        # row 1
+        if isinstance(original, Trace):
+            fig.add_trace(original.plot(index, n),
+                          row=1, col=1)
+        fig.add_trace(self.forecast.plot(index, n),
+                      row=1, col=1)
+        fig.add_trace(self.level.plot(index, n),
+                      row=1, col=1)
+        # row 2
+        fig.add_trace(self.forecast_sign.digital.plot(index, n, fill='tozeroy'),
+                      row=2, col=1)
+        # row 3
+        fig.add_trace(self.level_sign.digital.plot(index, n, fill='tozeroy'),
+                      row=3, col=1)
+        # row 4
+        fig.add_trace(self.trend.plot(index, n, fill='tozeroy'),
+                      row=4, col=1)
+        # row 5
+        fig.add_trace(self.trend_sign.digital.plot(index, n, fill='tozeroy'),
+                      row=5, col=1)
+        # row 6
+        fig.add_trace(self.trend_inflection.digital.plot(index, n, fill='tozeroy'),
+                      row=6, col=1)
+        # row 7
+        fig.add_trace(self.error.plot(index, n),
+                      row=7, col=1)
+        # row 8
+        fig.add_trace(self.variance_forecast.plot(index, n),
+                      row=8, col=1)
+        fig.add_trace(self.variance_level.plot(index, n),
+                      row=8, col=1)
+        fig.add_trace(self.variance_trend.plot(index, n),
+                      row=8, col=1)
+
+        # base layout configuration
+        fig.update_layout(
+            height=900,
+            margin=dict(t=50, b=60, l=50, r=50)
+        )
+
+        return fig
+
+
+@dataclass(eq=True, frozen=True)
+class AlphaBetaFilter:
+    """ Alpha-beta filter results."""
+    #: Signal forecast value.
+    forecast: float = 0.0
+    #: Sign of the signal forecast ``(-1: negative, 0: zero, 1: positive)``.
+    forecast_sign: float = 0
+    #: Signal level value.
+    level: float = 0.0
+    #: Sign of the signal level ``(-1: negative, 0: zero, 1: positive)``.
+    level_sign: float = 0.0
+    #: Signal trend value.
+    trend: float = 0.0
+    #: Sign of the signal trend ``(-1: negative, 0: zero, 1: positive)``.
+    trend_sign: float = 0.0
+    #: Inflection of the signal prognosis trend ``(1: increase, -1: decrease)``.
+    trend_inflection: float = 0.0
+    #: Signal prediction error value.
+    error: float = 0.0
+    #: Signal forecast variance reduction factor.
+    variance_forecast: float = 0.0
+    #: Signal level variance reduction factor.
+    variance_level: float = 0.0
+    #: Signal trend variance reduction factor.
+    variance_trend: float = 0.0
+
+
+@dataclass(eq=False)
 class ExponentialSmoothingTraces(Traces):
     """ Collection of :class:`ExponentialSmoothing` traces for signal samples
     processed with a 2nd-order exponential smoothing. """
     #: Signal forecast value.
     forecast: Trace = field(default_factory=Trace)
     #: Sign of the signal forecast ``(-1: negative, 0: zero, 1: positive)``.
     forecast_sign: Trace = field(default_factory=Trace)
@@ -3346,21 +3675,22 @@
     #: Empirical kurtosis of the distribution (4th central moment).
     kurtosis: Trace = field(default_factory=Trace)
 
     def figure(self,
                index: Optional[int] = None,
                n: Optional[int] = None,
                original: Optional[Trace] = None,
-               subplots: Optional[Dict[str, Any]] = None) -> go.Figure:
+               subplots: Optional[dict[str, Any]] = None) -> go.Figure:
         """ Returns a figure of subplots for the traces.
 
-        :param int index: start index of the samples to plot
-        :param n: number of samples to plot
+        :param int index: optional start index of the samples to plot
+        :param int n: optional number of samples to plot
         :param Trace original: optional original trace to add to the plot
-        :param dict subplots: dictionary with the settings for the subplots
+        :param dict subplots: optional dictionary with the settings for the
+            subplots
         """
         # base subplots configuration
         subplots_ = dict(
             rows=10,
             cols=1,
             shared_xaxes=True,
             row_heights=(3, 0.25, 0.25, 1.25, 0.25, 0.25, 1, 1, 1, 0.75),
@@ -3510,21 +3840,22 @@
     #: Empirical kurtosis of the distribution (4th central moment).
     kurtosis: Trace = field(default_factory=Trace)
 
     def figure(self,
                index: Optional[int] = None,
                n: Optional[int] = None,
                original: Optional[Trace] = None,
-               subplots: Optional[Dict[str, Any]] = None) -> go.Figure:
+               subplots: Optional[dict[str, Any]] = None) -> go.Figure:
         """ Returns a figure of subplots for the traces in the collection.
 
-        :param int index: start index of the samples to plot
-        :param n: number of samples to plot
+        :param int index: optional start index of the samples to plot
+        :param int n: optional number of samples to plot
         :param Trace original: optional original trace to add to the plot
-        :param dict subplots: dictionary with the settings for the subplots
+        :param dict subplots: optional dictionary with the settings for the
+            subplots
         """
         # base subplots configuration
         subplots_ = dict(
             rows=7,
             cols=1,
             shared_xaxes=True,
             row_heights=(5, 1, 1, 1, 1, 1, 1),
```

### Comparing `signalyzer-0.2.4/src/signalyzer.egg-info/PKG-INFO` & `signalyzer-0.3.0/src/signalyzer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signalyzer
-Version: 0.2.4
+Version: 0.3.0
 Summary: Signal analyzer for time-discrete, equidistant measured signals
 Home-page: https://gitlab.com/signalytics/signalyzer/
 Download-URL: https://gitlab.com/signalytics/signalyzer/-/packages
 Author: Jochen Gerhaeusser
 Author-email: jochen_privat@gmx.de
 License: BSD-3-Clause
 Project-URL: Issue Tracker, https://gitlab.com/signalytics/signalyzer/-/issues/
@@ -17,21 +17,21 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Education
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Visualization
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
   <img src="https://signalytics.gitlab.io/signalyzer/_static/images/signalyzer.svg"><br>
 </div>
 
@@ -71,16 +71,16 @@
 * moving OLS linear regression with window statistics
 * shifting (moving) of the measured signal
 * slicing of the measured signal
 * evaluate statemachine transitions observed by measured state signal
 
 > **Important**: The **signalyzer** package is best used within [JupyterLab] a
 > web-based interactive development environment for [Jupyter] notebooks or with
-> Plotly [Dash] or Jupyter [voila] to build standalone web applications and
-> dashboards.
+> Plotly [Dash], [Streamlit] or Jupyter [voila] to build standalone web
+> applications and dashboards.
 
 ## Table of Contents
 [Back to top]: #table-of-contents
 
 1. [Project Status](#project-status)
 2. [Project Structure](#project-structure)
 3. [Getting Started](#getting-started)
@@ -96,36 +96,36 @@
 6. [Documentation](#documentation)
 7. [Contributing](#contributing)
 8. [License](#license)
 9. [Authors](#authors)
 
 ## Project Status
 
-This [project] is a work in progress and far away from stable.
-Feedback is always welcomed!
+This [project] is stable and active. Feedback is always welcomed!
 
 **[Back to top](#table-of-contents)**
 
 ## Project Structure
 
 The [project] is organized in sub-folders.
 
+- `assets`: [Project] assets files
 - `docs/`: [Sphinx] documentation
 - `notebooks/`: [Jupyter] notebooks
 - `src/signalyzer/`: Package sources
   - `signalyzer/trace`: Trace module sources
   - `signalyzer/statemachine`: Statemachine module sources
 
 **[Back to top](#table-of-contents)**
 
 ## Getting Started
 
 ### Dependencies
 
-The `signalyzer` package requires at least [Python] 3.9 and depends on the
+The `signalyzer` package requires at least [Python] 3.10 and depends on the
 external packages:
 
 - [numpy]
 - [scipy]
 - [pandas]
 - [plotly]
 
@@ -244,19 +244,18 @@
 [sphinx-plotly-directive]: https://pypi.org/project/sphinx-plotly-directive
 [numpy]: https://pypi.org/project/numpy
 [scipy]: https://pypi.org/project/scipy
 [pandas]: https://pypi.org/project/pandas
 [plotly]: https://pypi.org/project/plotly
 [voila]: https://voila.readthedocs.io
 [dash]: https://dash.plotly.com/
+[streamlit]: https://streamlit.io/
 [JupyterLab]: https://jupyter.org
 [Jupyter]: https://jupyter.org
 [gitlab]: https://gitlab.com
 [project]: https://gitlab.com/signalytics/signalyzer
 [PyPI package registry]: https://gitlab.com/signalytics/signalyzer/-/packages
 [repository tag list]: https://gitlab.com/signalytics/signalyzer/-/tags
 [contributors]: https://gitlab.com/signalytics/signalyzer/-/graphs/main
 [GitLab Pages]: https://signalytics.gitlab.io/signalyzer
 [installation guide]: https://signalytics.gitlab.io/signalyzer/intro.html#installation
 [Read The Docs]: https://signalyzer.readthedocs.io
-
-
```

### Comparing `signalyzer-0.2.4/src/signalyzer.egg-info/SOURCES.txt` & `signalyzer-0.3.0/src/signalyzer.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,55 +1,41 @@
-.editorconfig
-.gitattributes
-.gitignore
-.gitlab-ci.yml
-.pypirc
-.readthedocs.yaml
 CHANGELOG.rst
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
 make.bat
 pyproject.toml
 requirements.txt
 runtime.txt
 setup.cfg
 setup.py
-assets/signalyzer.svg
-assets/banner/banner.png
-assets/icons/favicon_16x16.ico
-assets/icons/favicon_16x16.png
-assets/icons/favicon_32x32.ico
-assets/icons/favicon_32x32.png
-assets/icons/favicon_64x64.ico
-assets/icons/favicon_64x64.png
-assets/logo/logo.png
-assets/logo/logo.svg
 docs/Makefile
 docs/conf.py
 docs/genindex.rst
 docs/index.rst
 docs/make.bat
 docs/requirements.txt
 docs/_static/images/banner.png
 docs/_static/images/favicon.ico
 docs/_static/images/logo.png
 docs/_static/images/signalyzer.svg
 docs/annex/changelog.rst
 docs/annex/contributing.rst
 docs/annex/license.rst
 docs/api/index.rst
+docs/collections/alpha-beta-filter-traces.rst
 docs/collections/exponential-smoothing-traces.rst
 docs/collections/index.rst
 docs/collections/linear-regression-traces.rst
 docs/collections/set-traces.rst
 docs/collections/slew-rate-limiter-traces.rst
 docs/collections/statistics-traces.rst
 docs/collections/vector-traces.rst
+docs/processing/alpha-beta-filter.rst
 docs/processing/change-rate-limiting.rst
 docs/processing/clipping.rst
 docs/processing/dt1-element.rst
 docs/processing/exponential-smoothing.rst
 docs/processing/iir-filters.rst
 docs/processing/index.rst
 docs/processing/logic-functions.rst
@@ -75,24 +61,25 @@
 docs/transformations/integrating_functions.rst
 docs/transformations/mathematical_functions.rst
 docs/transformations/statistics.rst
 docs/transformations/trigonometric_functions.rst
 docs/transformations/value_conversions.rst
 docs/transformations/x-axis_transformations.rst
 notebooks/DFT.ipynb
+notebooks/analyzer.ipynb
+notebooks/analyzer/Slope-Velocity-Estimator.pdf
+notebooks/analyzer/analyzer.ipynb
+notebooks/analyzer/recording.csv
 notebooks/chord/chord-diagram.ipynb
 notebooks/chord/chord.ipynb
-notebooks/chord/.ipynb_checkpoints/chord-checkpoint.ipynb
-notebooks/chord/.ipynb_checkpoints/chord-diagram-checkpoint.ipynb
 notebooks/statemachine/statemachine.ipynb
 notebooks/statistics/statistics.ipynb
 notebooks/trace/trace.ipynb
 src/signalyzer/__init__.py
 src/signalyzer/constants.py
-src/signalyzer/types.py
 src/signalyzer.egg-info/PKG-INFO
 src/signalyzer.egg-info/SOURCES.txt
 src/signalyzer.egg-info/dependency_links.txt
 src/signalyzer.egg-info/not-zip-safe
 src/signalyzer.egg-info/requires.txt
 src/signalyzer.egg-info/top_level.txt
 src/signalyzer/statemachine/__init__.py
```

