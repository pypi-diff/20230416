# Comparing `tmp/raman_fitting-0.6.18.tar.gz` & `tmp/raman_fitting-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raman_fitting-0.6.18.tar", last modified: Sun Mar  5 21:42:52 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `raman_fitting-0.6.18.tar` & `raman_fitting-0.7.0.tar`

### file list

```diff
@@ -1,133 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 21:42:52.605857 raman_fitting-0.6.18/
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/.envrc
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 21:42:52.573856 raman_fitting-0.6.18/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 21:42:52.581857 raman_fitting-0.6.18/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/.github/workflows/build-test-codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/.github/workflows/github-actions-demo.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/.github/workflows/test-release-candidate.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/.github/workflows/tox_actions.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/.github/workflows/upload-to-testpypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/.secrets.baseline
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-03-05 21:42:52.605857 raman_fitting-0.6.18/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/build.info
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 21:42:52.581857 raman_fitting-0.6.18/examples/
--rw-r--r--   0 runner    (1001) docker     (123)  1106668 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/examples/fitting_Model_1st_6peaks+Si.png
--rw-r--r--   0 runner    (1001) docker     (123)  1462158 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/examples/raw_data.png
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-03-05 21:42:52.605857 raman_fitting-0.6.18/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 21:42:52.573856 raman_fitting-0.6.18/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 21:42:52.585857 raman_fitting-0.6.18/src/raman_fitting/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/src/raman_fitting/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/src/raman_fitting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-03-05 21:42:52.000000 raman_fitting-0.6.18/src/raman_fitting/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/src/raman_fitting/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 21:42:52.589857 raman_fitting-0.6.18/src/raman_fitting/config/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/src/raman_fitting/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/src/raman_fitting/config/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/src/raman_fitting/config/filepath_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/src/raman_fitting/config/filepath_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/src/raman_fitting/config/logging_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 21:42:52.589857 raman_fitting-0.6.18/src/raman_fitting/datafiles/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/src/raman_fitting/datafiles/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 21:42:52.589857 raman_fitting-0.6.18/src/raman_fitting/datafiles/example_files/
--rw-r--r--   0 runner    (1001) docker     (123)    51806 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/src/raman_fitting/datafiles/example_files/Si_spectrum01.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/src/raman_fitting/datafiles/example_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/src/raman_fitting/datafiles/example_files/empty-lines_1.txt
--rw-r--r--   0 runner    (1001) docker     (123)    52388 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/src/raman_fitting/datafiles/example_files/testDW38C_pos1.txt
--rw-r--r--   0 runner    (1001) docker     (123)    51871 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/src/raman_fitting/datafiles/example_files/testDW38C_pos2.txt
--rw-r--r--   0 runner    (1001) docker     (123)    52034 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/src/raman_fitting/datafiles/example_files/testDW38C_pos3.txt
--rw-r--r--   0 runner    (1001) docker     (123)    51781 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/src/raman_fitting/datafiles/example_files/testDW38C_pos4.txt
--rw-r--r--   0 runner    (1001) docker     (123)    52339 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/src/raman_fitting/datafiles/example_files/wrong-values-in-lines_pos1.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 21:42:52.593857 raman_fitting-0.6.18/src/raman_fitting/deconvolution_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/src/raman_fitting/deconvolution_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12897 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/src/raman_fitting/deconvolution_models/base_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 21:42:52.593857 raman_fitting-0.6.18/src/raman_fitting/deconvolution_models/default_peaks/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/src/raman_fitting/deconvolution_models/default_peaks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24260 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/src/raman_fitting/deconvolution_models/default_peaks/base_peak.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/src/raman_fitting/deconvolution_models/default_peaks/first_order_peaks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/src/raman_fitting/deconvolution_models/default_peaks/normalization_peaks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/src/raman_fitting/deconvolution_models/default_peaks/second_order_peaks.py
--rw-r--r--   0 runner    (1001) docker     (123)    13020 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/src/raman_fitting/deconvolution_models/fit_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/src/raman_fitting/deconvolution_models/model_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13406 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/src/raman_fitting/deconvolution_models/peak_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 21:42:52.593857 raman_fitting-0.6.18/src/raman_fitting/delegating/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/src/raman_fitting/delegating/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13877 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/src/raman_fitting/delegating/main_delegator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 21:42:52.593857 raman_fitting-0.6.18/src/raman_fitting/docker/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/src/raman_fitting/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/src/raman_fitting/docker/run_make_examples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 21:42:52.593857 raman_fitting-0.6.18/src/raman_fitting/exporting/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/src/raman_fitting/exporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/src/raman_fitting/exporting/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/src/raman_fitting/exporting/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11844 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/src/raman_fitting/exporting/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 21:42:52.597857 raman_fitting-0.6.18/src/raman_fitting/indexing/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/src/raman_fitting/indexing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8844 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/src/raman_fitting/indexing/filedata_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/src/raman_fitting/indexing/filename_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/src/raman_fitting/indexing/filename_parser_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/src/raman_fitting/indexing/filename_parser_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12663 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/src/raman_fitting/indexing/indexer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 21:42:52.597857 raman_fitting-0.6.18/src/raman_fitting/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/src/raman_fitting/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/src/raman_fitting/interfaces/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/src/raman_fitting/make_examples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 21:42:52.597857 raman_fitting-0.6.18/src/raman_fitting/processing/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/src/raman_fitting/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10718 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/src/raman_fitting/processing/cleaner.py
--rw-r--r--   0 runner    (1001) docker     (123)    11805 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/src/raman_fitting/processing/spectrum_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/src/raman_fitting/processing/spectrum_template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 21:42:52.597857 raman_fitting-0.6.18/src/raman_fitting/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/src/raman_fitting/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/src/raman_fitting/utils/coordinators.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/src/raman_fitting/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/src/raman_fitting/utils/file_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 21:42:52.585857 raman_fitting-0.6.18/src/raman_fitting.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-03-05 21:42:52.000000 raman_fitting-0.6.18/src/raman_fitting.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-03-05 21:42:52.000000 raman_fitting-0.6.18/src/raman_fitting.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-05 21:42:52.000000 raman_fitting-0.6.18/src/raman_fitting.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-05 21:42:52.000000 raman_fitting-0.6.18/src/raman_fitting.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-03-05 21:42:52.000000 raman_fitting-0.6.18/src/raman_fitting.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-05 21:42:52.000000 raman_fitting-0.6.18/src/raman_fitting.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 21:42:52.601857 raman_fitting-0.6.18/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 21:42:52.601857 raman_fitting-0.6.18/tests/deconvolution_models/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/tests/deconvolution_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/tests/deconvolution_models/test_base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12612 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/tests/deconvolution_models/test_base_peaks.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/tests/deconvolution_models/test_fit_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/tests/deconvolution_models/test_peak_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 21:42:52.601857 raman_fitting-0.6.18/tests/delegating/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/tests/delegating/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/tests/delegating/test_main_delegator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 21:42:52.601857 raman_fitting-0.6.18/tests/exporting/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/tests/exporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/tests/exporting/test_plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 21:42:52.601857 raman_fitting-0.6.18/tests/indexing/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/tests/indexing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/tests/indexing/test_filename_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/tests/indexing/test_filename_parser_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/tests/indexing/test_filename_parser_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/tests/indexing/test_indexer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 21:42:52.605857 raman_fitting-0.6.18/tests/processing/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/tests/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/tests/processing/test_cleaner.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/tests/processing/test_prepare_mean_spectrum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/tests/processing/test_spectrum_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/tests/test_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 21:42:52.605857 raman_fitting-0.6.18/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/tests/utils/test_coordinators.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/todos.md
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-03-05 21:41:52.000000 raman_fitting-0.6.18/tox.ini
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/.build.info
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/.flake8
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/.gitattributes
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/.secrets.baseline
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/Dockerfile
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/requirements.txt
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/setup.cfg
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/todos.md
+-rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/.github/workflows/build-test-codecov.yml
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/.github/workflows/github-actions-demo.yml
+-rw-r--r--   0        0        0     4547 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/.github/workflows/test-release-candidate.yaml
+-rw-r--r--   0        0        0     3442 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/.github/workflows/upload-to-testpypi.yml
+-rw-r--r--   0        0        0  1106668 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/examples/fitting_Model_1st_6peaks+Si.png
+-rw-r--r--   0        0        0  1462158 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/examples/raw_data.png
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/src/raman_fitting/MANIFEST.in
+-rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/src/raman_fitting/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/src/raman_fitting/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/src/raman_fitting/config/__init__.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/src/raman_fitting/config/constants.py
+-rw-r--r--   0        0        0     4227 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/src/raman_fitting/config/filepath_helper.py
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/src/raman_fitting/config/filepath_settings.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/src/raman_fitting/config/logging_config.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/src/raman_fitting/datafiles/__init__.py
+-rw-r--r--   0        0        0    51806 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/src/raman_fitting/datafiles/example_files/Si_spectrum01.txt
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/src/raman_fitting/datafiles/example_files/__init__.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/src/raman_fitting/datafiles/example_files/empty-lines_1.txt
+-rw-r--r--   0        0        0    52388 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/src/raman_fitting/datafiles/example_files/testDW38C_pos1.txt
+-rw-r--r--   0        0        0    51871 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/src/raman_fitting/datafiles/example_files/testDW38C_pos2.txt
+-rw-r--r--   0        0        0    52034 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/src/raman_fitting/datafiles/example_files/testDW38C_pos3.txt
+-rw-r--r--   0        0        0    51781 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/src/raman_fitting/datafiles/example_files/testDW38C_pos4.txt
+-rw-r--r--   0        0        0    52339 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/src/raman_fitting/datafiles/example_files/wrong-values-in-lines_pos1.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/src/raman_fitting/deconvolution_models/__init__.py
+-rw-r--r--   0        0        0     9653 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/src/raman_fitting/deconvolution_models/base_model.py
+-rw-r--r--   0        0        0    12964 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/src/raman_fitting/deconvolution_models/fit_models.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/src/raman_fitting/deconvolution_models/model_config.py
+-rw-r--r--   0        0        0    11400 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/src/raman_fitting/deconvolution_models/peak_validation.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/src/raman_fitting/deconvolution_models/default_peaks/__init__.py
+-rw-r--r--   0        0        0    22380 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/src/raman_fitting/deconvolution_models/default_peaks/base_peak.py
+-rw-r--r--   0        0        0     5125 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/src/raman_fitting/deconvolution_models/default_peaks/first_order_peaks.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/src/raman_fitting/deconvolution_models/default_peaks/normalization_peaks.py
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/src/raman_fitting/deconvolution_models/default_peaks/second_order_peaks.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/src/raman_fitting/delegating/__init__.py
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/src/raman_fitting/delegating/main_delegator.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/src/raman_fitting/docker/__init__.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/src/raman_fitting/docker/run_make_examples.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/src/raman_fitting/exporting/__init__.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/src/raman_fitting/exporting/database.py
+-rw-r--r--   0        0        0     5275 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/src/raman_fitting/exporting/exporter.py
+-rw-r--r--   0        0        0     9191 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/src/raman_fitting/exporting/plotting.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/src/raman_fitting/indexing/__init__.py
+-rw-r--r--   0        0        0     8835 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/src/raman_fitting/indexing/filedata_parser.py
+-rw-r--r--   0        0        0     6027 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/src/raman_fitting/indexing/filename_parser.py
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/src/raman_fitting/indexing/filename_parser_collector.py
+-rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/src/raman_fitting/indexing/filename_parser_helpers.py
+-rw-r--r--   0        0        0    11693 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/src/raman_fitting/indexing/indexer.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/src/raman_fitting/interfaces/__init__.py
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/src/raman_fitting/interfaces/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/src/raman_fitting/processing/__init__.py
+-rw-r--r--   0        0        0    10714 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/src/raman_fitting/processing/cleaner.py
+-rw-r--r--   0        0        0    11803 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/src/raman_fitting/processing/spectrum_constructor.py
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/src/raman_fitting/processing/spectrum_template.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/src/raman_fitting/utils/__init__.py
+-rw-r--r--   0        0        0     5147 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/src/raman_fitting/utils/coordinators.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/src/raman_fitting/utils/exceptions.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/src/raman_fitting/utils/file_reader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/tests/__init__.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/tests/conftest.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/tests/empty.toml
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/tests/test_sample.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/tests/deconvolution_models/__init__.py
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/tests/deconvolution_models/test_base_model.py
+-rw-r--r--   0        0        0    12630 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/tests/deconvolution_models/test_base_peaks.py
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/tests/deconvolution_models/test_fit_models.py
+-rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/tests/deconvolution_models/test_peak_validation.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/tests/delegating/__init__.py
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/tests/delegating/test_main_delegator.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/tests/exporting/__init__.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/tests/exporting/test_plotting.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/tests/indexing/__init__.py
+-rw-r--r--   0        0        0     3511 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/tests/indexing/test_filename_parser.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/tests/indexing/test_filename_parser_collector.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/tests/indexing/test_filename_parser_helpers.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/tests/indexing/test_indexer.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/tests/processing/__init__.py
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/tests/processing/test_cleaner.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/tests/processing/test_prepare_mean_spectrum.py
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/tests/processing/test_spectrum_constructor.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/tests/utils/__init__.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/tests/utils/test_coordinators.py
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/LICENSE
+-rw-r--r--   0        0        0     4736 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/README.md
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     7203 2020-02-02 00:00:00.000000 raman_fitting-0.7.0/PKG-INFO
```

### Comparing `raman_fitting-0.6.18/.flake8` & `raman_fitting-0.7.0/.flake8`

 * *Files identical despite different names*

### Comparing `raman_fitting-0.6.18/.github/workflows/github-actions-demo.yml` & `raman_fitting-0.7.0/.github/workflows/github-actions-demo.yml`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,14 @@
   Explore-GitHub-Actions:
     runs-on: ubuntu-latest
     steps:
       - run: echo "🎉 The job was automatically triggered by a ${{ github.event_name }} event."
       - run: echo "🐧 This job is now running on a ${{ runner.os }} server hosted by GitHub!"
       - run: echo "🔎 The name of your branch is ${{ github.ref }} and your repository is ${{ github.repository }}."
       - name: Check out repository code
-        uses: actions/checkout@v2
+        uses: actions/checkout@v3
       - run: echo "💡 The ${{ github.repository }} repository has been cloned to the runner by $GITHUB_ACTOR or ${{ github.actor }}."
       - run: echo "🖥️ The workflow is now ready to test your code on the runner."
       - name: List files in the repository
         run: |
           ls ${{ github.workspace }}
       - run: echo "🍏 This job's status is ${{ job.status }}."
```

### Comparing `raman_fitting-0.6.18/.github/workflows/test-release-candidate.yaml` & `raman_fitting-0.7.0/.github/workflows/test-release-candidate.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # Reference:
 # https://github.com/scottclowe/python-template-repo
 
 name: release candidate tests
 
 on:
   workflow_dispatch:
-  
+
   push:
     branches:
       # Release branches.
       # Examples: "v1", "v3.0", "v1.2.x", "1.5.0", "1.2rc0"
       # Expected usage is (for example) a branch named "v1.2.x" which contains
       # the latest release in the 1.2 series.
       - 'v[0-9]+'
@@ -48,40 +48,36 @@
     types: [created, edited, published]
 
 jobs:
   test-build:
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        os: [ubuntu-latest]
+        os: [ubuntu-latest, windows-latest, macos-latest]
         # windows-latest !=> gives error in 'if' statetement
-        python-version: ["3.8", "3.9"]
-        include:
-          - os: macos-latest
-            python-version: "3.9"
+        python-version: ["3.9", "3.10", "3.11"]
     env:
       OS: ${{ matrix.os }}
       PYTHON: ${{ matrix.python-version }}
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
 
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        python -m pip install flake8 
+        python -m pip install flake8
         python -m pip install pytest pytest-cov coverage
-        python -m pip install setuptools-scm
-        python3 -m pip install setuptools wheel build
-        if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
+        python -m pip install -U build
+        python -m pip install -r requirements.txt
         python -m pip install --editable .[test]
 
     - name: Sanity check with flake8
       run: |
         # stop the build if there are Python syntax errors or undefined names
         python -m flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
         # exit-zero treats all errors as warnings
@@ -101,41 +97,32 @@
       with:
         flags: unittests
         env_vars: OS,PYTHON
         name: Python ${{ matrix.python-version }} on ${{ runner.os }}
 
     - name: Build wheels
       run: |
-        python -m pip install --upgrade setuptools wheel twine
-        python setup.py sdist bdist_wheel
+        python3 -m pip install -U build
+        python3 -m build
 
     - name: Store wheel artifacts
       uses: actions/upload-artifact@v2
       with:
         name: wheel-${{ runner.os }}
         path: dist/*
 
-    #- name: Build HTML docs
-    #  run: |
-    #    python -m pip install --editable .[docs]
-    #    cd docs
-    #    make html
-    #    cd ..
 
   publish:
-    
     # Disabled by default
     if: startsWith(github.ref, 'refs/tags/')
-    #false &&
-      
     needs: test-build
 
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
 
     - name: Download wheel artifacts
       uses: actions/download-artifact@v2
       with:
         name: wheel-${{ runner.os }}
         path: dist/
```

### Comparing `raman_fitting-0.6.18/.github/workflows/upload-to-testpypi.yml` & `raman_fitting-0.7.0/.github/workflows/upload-to-testpypi.yml`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # This is a basic workflow to help you get started with Actions
 
 name: Publish to TestPyPI and PyPI
 
-# Controls when the action will run. 
+# Controls when the action will run.
 on:
   # Triggers the workflow on push to the master branch
   #push:
   #  branches: [ master ]
 
   # Allows you to run this workflow manually from the Actions tab
   workflow_dispatch:
@@ -19,75 +19,72 @@
     name: Build Python 🐍 distributions to 📦
     #if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
     runs-on: ubuntu-latest
 
     # Steps represent a sequence of tasks that will be executed as part of the job
     steps:
       # Checks-out your repository under $GITHUB_WORKSPACE, so your job can access it
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
         # with:
         # fetch-depth: 0
       - name: Fetch all history for all tags and branches
         run: git fetch --prune --unshallow
 
-      - name: Set up python 3.8
-        uses: actions/setup-python@v2
+      - name: Set up python 3.11
+        uses: actions/setup-python@v4
         with:
-          python-version: 3.8 
+          python-version: 3.11
 
-      # Installs and upgrades pip, installs other dependencies and installs the package from setup.py
+      # Installs and upgrades pip, installs other dependencies and installs the package from pyproject.toml
       - name: Installs and upgrades pip and installs other dependencies
         run: |
           # Upgrade pip
           python3 -m pip install --upgrade pip
           # Install build deps
-          python3 -m pip install setuptools wheel build
-          python3 -m pip install setuptools-scm
+          python3 -m pip install -U build
           # If requirements.txt exists, install from it
-          if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
-          
+          python3 -m pip install -r requirements.txt
+
       - name: Builds the package
         run: |
-          # Install the package from setup.py
-          # python3 setup.py sdist bdist_wheel
           # Install package with build
           python3 -m build
-      
+
       - name: Store wheel artifacts
         uses: actions/upload-artifact@v2
         with:
           name: wheel-${{ runner.os }}-${{ runner.python-version }}
           path: dist/*
-          
+
   publish:
-  
+
     name: Publish 📦 to PyPI and TestPyPI
     #if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
     needs: build
     runs-on: ubuntu-latest
     # Steps represent a sequence of tasks that will be executed as part of the job
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
 
       - name: Download wheel artifacts
         uses: actions/download-artifact@v2
         with:
           name: wheel-${{ runner.os }}-${{ runner.python-version }}
           path: dist/
 
       - name: Store aggregated wheel artifacts
         uses: actions/upload-artifact@v2
         with:
           name: wheels
           path: dist/*
 
       # Checks-out your repository under $GITHUB_WORKSPACE, so your job can access it
-      - name: Check to TestPyPI 
+      - name: Check to TestPyPI
         run: |
-          python3 -m pip install twine
+          python3 -m pip install -U twine
           # Check twine in advance even though gh-action-pypi also does that
           twine check dist/*
         # Upload to TestPyPI
       - name: Publish package to TestPyPI 📦
         if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags/v')
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
```

### Comparing `raman_fitting-0.6.18/.gitignore` & `raman_fitting-0.7.0/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 # SageMath parsed files
 *.sage.py
 
 # Environments
 .env
 .venv
 env/
-env311/
+env*/
 venv/
 ENV/
 env.bak/
 venv.bak/
 
 # Spyder project settings
 .spyderproject
@@ -131,8 +131,8 @@
 /*.pkl
 
 # extra tox files
 tox.ini.bak
 tox-generated.ini
 
 # Generated by setuptools-scm
-src/*/_version.py
+*/*/_version.py
```

### Comparing `raman_fitting-0.6.18/.secrets.baseline` & `raman_fitting-0.7.0/.secrets.baseline`

 * *Files identical despite different names*

### Comparing `raman_fitting-0.6.18/LICENSE` & `raman_fitting-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `raman_fitting-0.6.18/PKG-INFO` & `raman_fitting-0.7.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,67 +1,39 @@
-Metadata-Version: 2.1
-Name: raman_fitting
-Version: 0.6.18
-Summary: Python framework for the batch processing and deconvolution of raman spectra.
-Home-page: https://github.com/MyPyDavid/raman-fitting.git
-Author: David Wallace
-Author-email: wdz.wallace@protonmail.com
-Project-URL: Source Code, https://github.com/MyPyDavid/raman-fitting.git
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Physics
-Classifier: Topic :: Scientific/Engineering :: Chemistry
-Requires-Python: >=3.7.0
-Description-Content-Type: text/markdown
-Provides-Extra: testing
-Provides-Extra: dev
-License-File: LICENSE
-
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![CI GH actions](https://github.com/MyPyDavid/raman-fitting/actions/workflows/build-test-codecov.yml/badge.svg)](https://github.com/MyPyDavid/raman-fitting/actions/workflows/build-test-codecov.yml)
 [![codecov](https://codecov.io/gh/MyPyDavid/raman-fitting/branch/main/graph/badge.svg?token=II9JZAODJY)](https://codecov.io/gh/MyPyDavid/raman-fitting)
 [![Test & Upload to TestPyPI](https://github.com/MyPyDavid/raman-fitting/actions/workflows/upload-to-testpypi.yml/badge.svg)](https://github.com/MyPyDavid/raman-fitting/actions/workflows/upload-to-testpypi.yml)
 
 <p align="center" width="100%">
   <img src="https://user-images.githubusercontent.com/13996213/140090631-ed7c9f51-7630-49b6-9081-fb0675a5a4c9.png" alt="raman_cover_img"  width="200px" height="100px"/>
-</p> 
+</p>
 
 
 # raman-fitting
  A Python framework that performs a deconvolution on typical parts of interest on the spectrum of carbonaceous materials.
  The deconvolutions are done with models which are composed of collections of lineshapes or peaks that are typically assigned to these spectra in scientific literature.
 
-
-
-
-In batch processing mode this framework will index raman data files in a chosen folder.
+In batch processing mode this package will index the raman data files in a chosen folder.
 First, it will try to extract a sample ID and position number from the filenames and create an index of the files in a dataframe. Over this index a preprocessing, fitting and exporting loop will start.
 There are several models, each with a different combination of typical peaks, used for fitting. Each individual typical peak is defined as a class in the deconvolution/default_peaks folder with some added literature reference in the docstring. Here, the individual peak parameter settings can also be easily adjusted for initial values, limits, shape (eg. Lorentzian, Gaussian and Voigt) or be fixed at certain initial values.
 Export is done with plots and excel files for the spectral data and fitting parameters for further analysis.
 
 
 ### Example plots
 
 https://github.com/MyPyDavid/raman-fitting/wiki
 
 
-### Installation
+### Set up virtual environment and install the package
 
 A release is now available on PyPI, installation can be done with these commands in a terminal.
 ``` bash
 # Setting up and activating a virtual environment
-python -m venv testenv
-source /testenv/bin/activate
+python -m venv env # python 3.11 is recommended
+source env/bin/activate
 
 # Installation from PyPI
 python -m pip install raman_fitting
 ```
 
 #### From source installation
 
@@ -90,15 +62,20 @@
 or these commands in the Python interpreter or in a Jupyter Notebook.
 ``` python
 import raman_fitting
 raman_fitting.make_examples()
 ```
 This test run should yield the resulting plots and files in the following folder. Where home means the local user home directory depending on the OS.
 ``` bash
+# Linux
 home/.raman_fitting/example_results
+
+# For Other OSs, log messages will show:
+# Results saved in ...
+
 ```
 
 #### Fitting your own datafiles
 Place your data files in the default location or change this default setting in the config.
 ``` bash
 home/.raman_fitting/datafiles
 ```
@@ -125,17 +102,17 @@
 An example of filename formatting and parsing result:
 ``` python
 samplename1_pos1.txt => sampleID = 'samplename1', position = 1
 sample2-100_3.txt => sampleID = 'sample2-100', position = 3
 ```
 ### Version
 
-The current version is v0.6.18
+The current version is v0.7.0
 
 ### Dependencies
 
-- python >= 3.7
-- lmfit >= 1.0.0
-- pandas >= 1.0.5
-- scipy >= 1.4.1
-- matplotlib >= 3.1.2
-- numpy >= 1.19.2
+- python >= 3.11
+- lmfit >= 1.2.0
+- pandas >= 2.0.0
+- scipy >= 1.10.1
+- matplotlib >= 3.7.2
+- numpy >= 1.24.2
```

### Comparing `raman_fitting-0.6.18/build.info` & `raman_fitting-0.7.0/.build.info`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,27 @@
 # Build release overview
 # Reference:
-# https://github.com/pauliacomi/pyGAPS/blob/6bab0653dca40a44d9247c873b180937365ea0d8/.build.info
-
+# https://github.com/pauliacomi/pyGAPS/blob/c19bf45a896ff787acf8a29f77652a90236dd6c5/.build.info
 # This file contains details about how to
 # perform a release of this package
 
 # Create new branch for release (we use git flow)
 # Respect semantic versioning for the releases
 git flow release start x.y.z
 
 # Ensure all tests are passing
 # or use CI provider to run them automatically
 pytest --cov --cov-report xml:coverage.xml
 
 # Run bumpversion to change any version strings
 # scattered throughout the source code
-<<<<<<< HEAD
-# !!! Check if pre-commit hooks are there or not..
-# bump2version fails after pre-commit hook fails
-#
-# bump2version patch --no-commit
-# --allow-dirty
-#
-# bump2version major/minor/patch
-=======
+bumpversion major/minor/patch
 # !!! Check if pre-commit hooks are enabled
 # bump2version may fail the commit if pre-commit hooks fail...
 # bump2version patch --no-commit
-# bumpversion major/minor/patch
->>>>>>> release/0.6.15
 
 # Finish branch
 git flow release finish x.y.z
 
 # Push, including tags
 git push --tags
```

### Comparing `raman_fitting-0.6.18/examples/fitting_Model_1st_6peaks+Si.png` & `raman_fitting-0.7.0/examples/fitting_Model_1st_6peaks+Si.png`

 * *Files identical despite different names*

### Comparing `raman_fitting-0.6.18/examples/raw_data.png` & `raman_fitting-0.7.0/examples/raw_data.png`

 * *Files identical despite different names*

### Comparing `raman_fitting-0.6.18/src/raman_fitting/__init__.py` & `raman_fitting-0.7.0/src/raman_fitting/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,67 +7,70 @@
 __status__ = "Development"
 __future_package_name__ = "pyramdeconv"
 __current_package_name__ = "raman_fitting"
 __package_name__ = __current_package_name__
 
 
 try:
-    from ._version import version
+    from ._version import __version__
+except ImportError:
+    # -- Source mode --
+    try:
+        # use setuptools_scm to get the current version from src using git
+        from setuptools_scm import get_version as _gv
+        from os import path as _path
+
+        __version__ = _gv(_path.join(_path.dirname(__file__), _path.pardir))
+    except ModuleNotFoundError:
+        __version__ = "importerr_modulenotfound_version"
+    except Exception as e:
+        __version__ = "importerr_exception_version"
+except Exception as e:
+    __version__ = "catch_exception_version"
 
-    __version__ = version
-except:
-    __version__ = "__version__ = '0.6.18'"
-
-
-from raman_fitting.config import filepath_settings
-from raman_fitting.config import logging_config
-
-# VERSION_PATH = config.PACKAGE_ROOT / 'VERSION.txt'
-# with open(VERSION_PATH, 'r') as version_file:
-# IDEA change version definitino
-# __version__ = version_file.read().strip()
 
 import logging
 import sys
 import warnings
 
 # Configure logger for use in package
 logger = logging.getLogger(__package_name__)
 
 log_format = (
-    "[%(asctime)s] — %(name)s — %(levelname)s —" "%(funcName)s:%(lineno)d—12s %(message)s")
-    # '[%(asctime)s] %(levelname)-8s %(name)-12s %(message)s')
+    "[%(asctime)s] — %(name)s — %(levelname)s —"
+    "%(funcName)s:%(lineno)d—12s %(message)s"
+)
+# '[%(asctime)s] %(levelname)-8s %(name)-12s %(message)s')
 
 # Define basic configuration
 logging.basicConfig(
     # Define logging level
     level=logging.DEBUG,
     # Define the format of log messages
     format=log_format,
     # Provide the filename to store the log messages
-    filename=('debug.log'),
+    filename=("debug.log"),
 )
 
 formatter = logging.Formatter(log_format)
-# logger.setLevel(logging.DEBUG)
-# from raman_fitting.config import logging_config
-# logger.addHandler(logging_config.get_console_handler())
-# logger.propagate = False
+from raman_fitting.config import logging_config
+
+logger.addHandler(logging_config.get_console_handler())
 
 # create console handler
 ch = logging.StreamHandler(stream=sys.stdout)
 ch.setLevel(logging.INFO)
 ch.setFormatter(formatter)
 
 # add the handlers to the logger
 logger.addHandler(ch)
 
 # This code is written for Python 3.
-if sys.version_info[0] != 3:
-    logger.error("raman_fitting requires Python 3.")
+if sys.version_info.major < 3 and sys.version_info.minor < 7:
+    logger.error(f"{__package_name__} requires Python 3.7 or higher.")
     sys.exit(1)
 
 # Let users know if they're missing any hard dependencies
 hard_dependencies = ("numpy", "pandas", "scipy", "matplotlib", "lmfit")
 soft_dependencies = {}
 missing_dependencies = []
 
@@ -84,12 +87,26 @@
     if not importlib.util.find_spec(dependency):
         warnings.warn(
             f"Missing important package {dependency}. {soft_dependencies[dependency]}"
         )
 
 del hard_dependencies, soft_dependencies, dependency, missing_dependencies
 
-# from raman_fitting import main_run_fit, indexer
+# Main Loop Delegator
+from raman_fitting.delegating.main_delegator import MainDelegator, make_examples
+
+# Indexer
+from raman_fitting.indexing.indexer import MakeRamanFilesIndex as make_index
 
-# Other user-facing functions
-from .api import *
+# Processing
+from raman_fitting.processing.spectrum_template import SpectrumTemplate
+from raman_fitting.processing.spectrum_constructor import (
+    SpectrumDataLoader,
+    SpectrumDataCollection,
+)
+
+# Modelling / fitting
+from raman_fitting.deconvolution_models.fit_models import InitializeModels, Fitter
 
+# Exporting / Plotting
+from raman_fitting.exporting.exporter import Exporter
+from raman_fitting.config import filepath_settings
```

### Comparing `raman_fitting-0.6.18/src/raman_fitting/config/filepath_helper.py` & `raman_fitting-0.7.0/src/raman_fitting/config/filepath_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # from .. import __package_name__
 
 logger = logging.getLogger(__name__)
 
 from raman_fitting.config import filepath_settings as config
 
-#%%
+# %%
 
 
 def get_directory_paths_for_run_mode(run_mode: str = "", **kwargs) -> Dict:
     """
     Parameters
     ----------
     run_mode : str, optional
@@ -47,21 +47,19 @@
         RESULTS_DIR = config.RESULTS_DIR
         DATASET_DIR = config.DATASET_DIR
         # INDEX_FILE = config.INDEX_FILE
     else:
         logger.warning(f"Run mode {run_mode} not recognized. Exiting...")
 
     INDEX_FILE = RESULTS_DIR / config.INDEX_FILE_NAME
-    DB_FILE = RESULTS_DIR / config.DB_FILE_NAME
 
     dest_dirs = {
         "RESULTS_DIR": Path(RESULTS_DIR),
         "DATASET_DIR": Path(DATASET_DIR),
         "INDEX_FILE": Path(INDEX_FILE),
-        "DB_FILE": Path(DB_FILE),
     }
 
     if kwargs:
         dest_dirs = override_from_kwargs(dest_dirs, **kwargs)
 
     check_and_make_dirs(dest_dirs)
```

### Comparing `raman_fitting-0.6.18/src/raman_fitting/config/logging_config.py` & `raman_fitting-0.7.0/src/raman_fitting/config/logging_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,27 +7,28 @@
 # it is in the same Python interpreter process.
 
 FORMATTER = logging.Formatter(
     "%(asctime)s — %(name)s — %(levelname)s —" "%(funcName)s:%(lineno)d — %(message)s"
 )
 
 
-
 log_format = (
-    "[%(asctime)s] — %(name)s — %(levelname)s —" "%(funcName)s:%(lineno)d—12s %(message)s")
-    # '[%(asctime)s] %(levelname)-8s %(name)-12s %(message)s')
+    "[%(asctime)s] — %(name)s — %(levelname)s —"
+    "%(funcName)s:%(lineno)d—12s %(message)s"
+)
+# '[%(asctime)s] %(levelname)-8s %(name)-12s %(message)s')
 
 # Define basic configuration
 logging.basicConfig(
     # Define logging level
     level=logging.DEBUG,
     # Define the format of log messages
     format=log_format,
     # Provide the filename to store the log messages
-    filename=('debug.log'),
+    filename=("debug.log"),
 )
 
 
 def get_console_handler():
     console_handler = logging.StreamHandler(sys.stdout)
     console_handler.setFormatter(FORMATTER)
     return console_handler
```

### Comparing `raman_fitting-0.6.18/src/raman_fitting/datafiles/example_files/Si_spectrum01.txt` & `raman_fitting-0.7.0/src/raman_fitting/datafiles/example_files/Si_spectrum01.txt`

 * *Files identical despite different names*

### Comparing `raman_fitting-0.6.18/src/raman_fitting/datafiles/example_files/testDW38C_pos1.txt` & `raman_fitting-0.7.0/src/raman_fitting/datafiles/example_files/testDW38C_pos1.txt`

 * *Files identical despite different names*

### Comparing `raman_fitting-0.6.18/src/raman_fitting/datafiles/example_files/testDW38C_pos2.txt` & `raman_fitting-0.7.0/src/raman_fitting/datafiles/example_files/testDW38C_pos2.txt`

 * *Files identical despite different names*

### Comparing `raman_fitting-0.6.18/src/raman_fitting/datafiles/example_files/testDW38C_pos3.txt` & `raman_fitting-0.7.0/src/raman_fitting/datafiles/example_files/testDW38C_pos3.txt`

 * *Files identical despite different names*

### Comparing `raman_fitting-0.6.18/src/raman_fitting/datafiles/example_files/testDW38C_pos4.txt` & `raman_fitting-0.7.0/src/raman_fitting/datafiles/example_files/testDW38C_pos4.txt`

 * *Files identical despite different names*

### Comparing `raman_fitting-0.6.18/src/raman_fitting/datafiles/example_files/wrong-values-in-lines_pos1.txt` & `raman_fitting-0.7.0/src/raman_fitting/datafiles/example_files/wrong-values-in-lines_pos1.txt`

 * *Files identical despite different names*

### Comparing `raman_fitting-0.6.18/src/raman_fitting/deconvolution_models/base_model.py` & `raman_fitting-0.7.0/src/raman_fitting/deconvolution_models/base_model.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,19 @@
-""" The member of the validated collection of BasePeaks are here assembled into fitting Models"""
-
+""" The members of the validated collection of BasePeaks are assembled here into fitting Models"""
 import logging
 from warnings import warn
 
 from lmfit import Model
 
-# from .. import __package_name__
+from raman_fitting.deconvolution_models.peak_validation import PeakModelValidator
 
 logger = logging.getLogger(__name__)
 
-
 _SUBSTRATE_PEAK = "Si1_peak"
 
-from raman_fitting.deconvolution_models.peak_validation import PeakModelValidator
-
-# if __name__ == "__main__":
-#     pass
-# else:
-#     from .peak_validation import PeakModelValidator
-
-#%%
 
 # ====== InitializeMode======= #
 class InitializeModels:
     """
     This class will initialize and validate the different fitting models.
     The models are of type lmfit.model.CompositeModel and stored in a dict with names
     for the models as keys.
@@ -41,30 +31,28 @@
     def __init__(self, standard_models=True):
         self._cqnm = self.__class__.__name__
 
         self.peak_collection = self.get_peak_collection(PeakModelValidator)
 
         self.all_models = {}
         self.construct_standard_models()
-        # self.normalization_model = self.peak_collection.normalization
 
     def get_peak_collection(self, func):
         try:
             peak_collection = func()
             logger.debug(
                 f"{self._cqnm} collection of peaks validated with {func}:\n{peak_collection}"
             )
 
         except Exception as e:
             logger.error(f"{self._cqnm} failure in call {func}.\n\t{e}")
             peak_collection = []
         return peak_collection
 
     def construct_standard_models(self):
-
         _models = {}
         _models_1st = {
             f"1st_{key}": BaseModel(
                 peak_collection=self.peak_collection, model_name=value
             )
             for key, value in self._standard_1st_order_models.items()
         }
@@ -114,26 +102,20 @@
     # IDEA change include substrate to  has substrate and remove from init
     def __init__(
         self,
         model_name: str = "",
         peak_collection=PeakModelValidator(),
         substrate_peak_name: str = _SUBSTRATE_PEAK,
     ):
-
         self.peak_collection = peak_collection
         self.peak_options = self.set_peak_options()
         self.substrate_peak_name = substrate_peak_name
-        # self.include_substrate = include_substrate
-        # has_substrate: bool = False,
         self._substrate_name = self.substrate_peak_name.split(self._SUFFIX)[0]
         self.model_name = model_name
-
         self.lmfit_model = self.model_constructor_from_model_name(self.model_name)
-        # self.model_constructor()
-        # self.peak_dict = self.peak_collection.get_dict()
 
     def set_peak_options(self):
         _opts = {}
         for _pk in self.peak_collection.options:
             try:
                 _prefix = _pk.split(self._SUFFIX)[0]
                 if _prefix:
@@ -155,39 +137,29 @@
         _ch = True
         name = self.validate_model_name_input(name)
         if hasattr(self, "_model_name"):
             if name == self._model_name:
                 _ch = False
         if _ch:
             self.lmfit_model = self.model_constructor_from_model_name(name)
-            # self._equalize_name_choice(name)
             self._model_name = name
 
     @property
     def has_substrate(self):
         _has = False
         if hasattr(self, "model_name"):
             _has = self.name_contains_substrate(self.model_name)
 
         return _has
 
     @has_substrate.setter
     def has_substrate(self, value):
-        # _hasattr_model = hasattr(self, 'model')
         raise AttributeError(
             f'{self.__class__.__name__} this property can not be set "{value}", use add_ or remove_ substrate function.'
         )
-        # _ch = True
-        # if hasattr(self,'_include_substrate'):
-        #     if _choice == self._include_substrate:
-        #         _ch = False
-        # if _ch:
-        #     self._equalize_name_choice(None, _choice)
-        #     self._include_substrate = _choice
-        # self._include_substrate = _choice
 
     def name_contains_substrate(self, _name):
         """Checks if name contains the substrate name, returns bool"""
         _name_contains_any = False
         if type(_name) == str:
             _name_contains_any = any(
                 i == self._substrate_name for i in _name.split("+")
@@ -203,24 +175,22 @@
                     BaseModelWarning,
                 )
                 _new_name = "+".join(
                     i for i in _name.split("+") if i not in self._substrate_name
                 )  # remove substr name
                 if _new_name != _name:
                     self.model_name = _new_name
-        # return _name
 
     def add_substrate(self):
         if hasattr(self, "model_name"):
             _name = self.model_name
             if not self.name_contains_substrate(_name):
                 _new_name = _name + f"+{self._substrate_name}"  # add substr name
                 if _new_name != _name:
                     self.model_name = _new_name
-        # return _name
 
     def validate_model_name_input(self, value):
         """checks if given input name is valid"""
         if type(value) != str:
             raise TypeError(
                 f'Given name "{value}" for model_name should be a string insteady of type({type(value).__name__})'
             )
@@ -264,15 +234,14 @@
             )
 
         if not _peak_models:
             _lmfit_model = None
         elif len(_peak_models) == 1:
             _lmfit_model = _peak_models[0].peak_model
         elif len(_peak_models) >= 2:
-            # _eval_model_name = ' + '.join([i[0] for i in _peak_models])
             _composite_model = None
             for _pkmod in _peak_models:
                 _mod = _pkmod.peak_model
                 if not _composite_model:
                     _composite_model = _mod
                 else:
                     try:
@@ -288,54 +257,14 @@
             warn(
                 f"Model constructor does not yield type ({type(Model)} {type(_lmfit_model)}.",
                 BaseModelWarning,
             )
         return _lmfit_model
 
     def __repr__(self):
-
         _choice = "no" if not self.has_substrate else "yes"
         _txt = f"{self.model_name}, substrate ({_choice}): "
         if hasattr(self, "lmfit_model"):
             _txt += "\n\t" + repr(self.lmfit_model)
         else:
             _txt += "empty model"
         return _txt
-
-    # def _0equalize_from_model_name(self,_name):
-    #     pass
-    # def _0equalize_from_incl_substrate(self,_choice):
-    #     pass
-    # def _0equalize_name_choice(self, _name, _choice):
-    #     _change = False
-    #     if _choice != None and _name == None and hasattr(self, '_model_name'):
-    #         # change model name when choice is set
-    #         _name = self._add_or_rem_substrate_to_model_name(_choice, self._model_name)
-    #         if _name != self._model_name:
-    #             _change = True
-    #             self._model_name = _name
-    #     if _name != None and _choice == None and hasattr(self, '_include_substrate'):
-    #         # change include subtrate choice when model name is set
-    #         _name_contains = self._name_contains_substrate(_name)
-    #         if _name_contains != self._include_substrate:
-    #             _change = True
-    #             self._include_substrate = _name_contains
-    #         if hasattr(self,'_model_name'):
-    #             _change = bool(_name != self._model_name)
-    #     # if _name != None and hasattr(self, '_model_name')
-    #     print(f'Change {_change}, name {_name}, choice {_choice}')
-    #     if _change  and _name:
-    #         self.lmfit_model = self.model_constructor_from_model_name(_name)
-    #     elif not _choice and _contains:
-    #         _substr_name = self.substrate_peak_name.split(self._SUFFIX)[0]
-    #         warn(f'\n{self.__class__.__name__} include substrate is set to {_choice} so "{_substr_name}" is removed from {_name}.\n',BaseModelWarning)
-    #         _name = '+'.join(i for i in _name.split('+') if i not in _substr_name)  # remove substr name
-
-    # def _0add_or_rem_substrate_to_model_name(self, _choice, _name):
-    #     _substr_name = self.substrate_peak_name.split(self._SUFFIX)[0]
-    #     _contains = self._name_contains_substrate(_name)
-    #     if _choice and not _contains:
-    #         _name = _name+f'+{_substr_name}'  # add substr name
-    #     elif not _choice and _contains:
-    #         warn(f'\n{self.__class__.__name__} include substrate is set to {_choice} so "{_substr_name}" is removed from {_name}.\n',BaseModelWarning)
-    #         _name = '+'.join(i for i in _name.split('+') if i not in _substr_name)  # remove substr name
-    #     return _name
```

### Comparing `raman_fitting-0.6.18/src/raman_fitting/deconvolution_models/default_peaks/base_peak.py` & `raman_fitting-0.7.0/src/raman_fitting/deconvolution_models/default_peaks/base_peak.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,22 @@
-# from collections import OrderedDict
-
 import inspect
 from functools import partialmethod
 from keyword import iskeyword as _iskeyword
 from warnings import warn
 
 from lmfit import Parameter, Parameters
 
-# import operator
-# from abc import ABC, abstractmethod
 from lmfit.models import GaussianModel, LorentzianModel, Model, VoigtModel
 
-# from lmfit import CompositeModel
-
-# print('name: ',__name__,'file: ', __file__, __package__)
-
-if __name__ in ("__main__"):
-    from raman_fitting.utils.coordinators import FieldsTracker as FieldsTracker
+if __name__ in ("__main__",):
+    from raman_fitting.utils.coordinators import FieldsTracker
 else:
     from ...utils.coordinators import FieldsTracker
 
-# __all__ = [Base]
 
-
-#%%
 class BasePeakWarning(UserWarning):  # pragma: no cover
     pass
 
 
 class BasePeak(type):
     """
     Base class for easier definition of typical intensity peaks found in the
@@ -92,52 +81,39 @@
         "param_hints": ["input_param_settings"],
     }
 
     PEAK_TYPE_OPTIONS = ["Lorentzian", "Gaussian", "Voigt"]
 
     # ('value', 'vary', 'min', 'max', 'expr') # optional
     default_settings = {"gamma": {"value": 1, "min": 1e-05, "max": 70, "vary": False}}
-    # _intern = list(super.__dict__.keys())+['__module__','_kwargs']
     subclasses = []
 
     _debug = False
 
-    # def __call__(cls, *args, **kwargs):
-    #     print(f'Request received to create an instance of class: {cls}...')
     def __prepare__(name, bases, **kwargs):
         """prepare method only for debugging"""
         if "debug" in kwargs.keys():
             if kwargs.get("debug", False):
                 print(f"__prepare ,name {name}, bases{bases}, kwargs {kwargs}")
-        # kwargs.update({'debug': False})
         return kwargs
 
     def __new__(mcls, name, *args, **kwargs):
-
-        # print(
-        #             f"Called __new ,_args {_}"
-        #         )
         if len(args) == 2:
-            # default arg __new__ input
             bases, cls_dict = args
         else:
             bases, cls_dict = (), {}
 
         if kwargs.get("debug", False):
             mcls._debug = True
         if cls_dict.get("debug", False):
             mcls._debug = True
         if mcls._debug:
             print(
                 f"Called __new ({mcls} ),name {name}, bases{bases}, cls_dict {cls_dict.keys()} kwargs {kwargs}"
             )
-        # print(f'vars: {vars(cls)}')
-
-        # From namdedtuple source:
-        # test input arguments names
         for name_ in [name] + list(kwargs.keys()):
             if type(name_) is not str:
                 raise TypeError("Class name and keywords names must be strings")
             if not name_.isidentifier():
                 raise ValueError(
                     "Class name and keywords names must be valid "
                     f"identifiers: {name_!r}"
@@ -191,15 +167,14 @@
             setattr(self, "peak_model", self.create_peak_model())
 
         # Fourth thing, check class __init__ for setting of field values and delete from cls dict
         if "__init__" in cls_dict.keys():
             cls_init_part_obj = partialmethod(cls_dict["__init__"])
 
             sig = inspect.signature(cls_dict["__init__"])
-            # breakpoint()
             _cls_init_part_obj_funcs = {
                 k: val
                 for k, val in cls_dict.items()
                 if inspect.isfunction(val) and k != "__init__"
             }
 
             for fname, func in _cls_init_part_obj_funcs.items():
@@ -231,15 +206,14 @@
         else:
             pass
 
         cls_dict["__init__"] = _init_subclass_replacement
 
         if fco.status:
             pass
-            # print(f'Good class definition all values for fields are present: {fco.results}', BasePeakWarning)
         else:
             warn(
                 f"Definition for {name} is not complete, please redefine {fco.missing} in class",
                 BasePeakWarning,
             )
 
         if mcls._debug:
@@ -256,21 +230,17 @@
         setattr(cls_object, "_debug", mcls._debug)
         setattr(cls_object, "fco", fco)
         setattr(cls_object, "PEAK_TYPE_OPTIONS", mcls.PEAK_TYPE_OPTIONS)
         cls_object = mcls._set_other_methods(cls_object)
         return cls_object
 
     def __init__(self, name, *args, **kwargs):
-        # bases, cls_dict removed and kept only *args
-        # print(f"__init_ base called ({self} with name '{name}' args {args} and kwargs {kwargs})")
         # subclassess are appended here
         if self not in self.subclasses:
             self.subclasses.append(self)
-        # super().__init__(name)
-        # print(f"__init_ super called ({self.__init__})")
 
     @classmethod
     def _cleanup_init_dict(cls, _dict):
         """cleans up the __init__ dictionary from defined class"""
         _dkeys = list(_dict.keys())
         _result = {}
         while _dkeys:
@@ -280,36 +250,32 @@
             ]  # clean field match
             _synmatch = [
                 (k, syn)
                 for k, val in cls._synonyms.items()
                 for syn in val
                 if syn in _dk
             ]  # synonym field match
-            # print(_dk, _kmatch,_synmatch)
             if _kmatch:
                 _result.update({i[0]: _dict[i[1]] for i in _kmatch})
             elif not _kmatch and _synmatch:
                 _result.update({i[0]: _dict[i[1]] for i in _synmatch})
         return _result
 
     @classmethod
     def _set_other_methods(cls, cls_object):
         """sets other methods found in this baseclass on the defined cls object"""
         _other_methods = [
             i for i in dir(cls) if not i.startswith("_") and not i == "mro"
         ]
-        # and not hasattr(cls_object, i)]
         for method in _other_methods:
-            # print(f'__new setting method {method}')
             _mcls_obj = getattr(cls, method)
             if method.endswith("__") and not method.startswith("__"):
                 method = f"__{method}"
 
             if not isinstance(_mcls_obj, property):
-                # print(f'__new setting {method} on {_mcls_obj} is callable')
                 setattr(cls_object, method, _mcls_obj)
         return cls_object
 
     @property
     def peak_type(self):
         """This property (str) should be assigned and in self.PEAK_TYPE_OPTIONS"""
         return self._peak_type
@@ -317,15 +283,14 @@
     @peak_type.setter
     def peak_type(self, value: str):
         """The peak type property should be in PEAK_TYPE_OPTIONS"""
         if not isinstance(value, str):
             raise TypeError(f'The value "{value}" is not a string.')
         value_ = None
         if any([value.upper() == i.upper() for i in self.PEAK_TYPE_OPTIONS]):
-            # self.type_to_model_chooser(value)
             value_ = value
         elif any([i.upper() in value.upper() for i in self.PEAK_TYPE_OPTIONS]):
             _opts = [i for i in self.PEAK_TYPE_OPTIONS if i.upper() in value.upper()]
             if len(_opts) == 1:
                 value_ = _opts[0]
 
                 warn(
@@ -343,15 +308,14 @@
         else:
             raise ValueError(
                 f'The value "{value}" for "peak_type" is not in {self.PEAK_TYPE_OPTIONS}.'
             )
         if value_:
             self._peak_type = value_
             self.fco.store("user_input", "peak_type", value)
-            # self.set_peak_model_from_fields()
             self.peak_model = self.create_peak_model()
 
     @property
     def peak_model(self):
         if not hasattr(self, "_peak_model"):
             self.create_peak_model()
         else:
@@ -368,63 +332,58 @@
         else:
             self._peak_model = value
 
     def create_peak_model(self):
         _peak_model = None
         if self.fco.status:
             if all(hasattr(self, field) for field in self._fields):
-
                 try:
                     create_model_kwargs = dict(
                         peak_name=self.peak_name,
                         peak_type=self.peak_type,
                         param_hints=self.param_hints,
                     )
 
                     if hasattr(self, "create_model_kwargs"):
                         _orig_kwargs = self.create_model_kwargs
 
                     _peak_model = LMfitModelConstructorMethods.create_peak_model_from_name_type_param_hints(
                         **create_model_kwargs
                     )
                     self.create_model_kwargs = create_model_kwargs
-                    # model = self.make_model_and_set_param_hints(prefix_, peak_type_, param_hints_)
                 except Exception as e:
                     print(f"try make models:\n{self}, \n\t {e}")
             else:
                 pass
         else:
             pass
             print(f"missing field {self.fco.missing} {self},\n")
         return _peak_model
 
     @property
     def param_hints(self):
         """This property is dict of dicts and sets the initial values for the parameters"""
-        # if hasattr(self, '_peak_model'):
         if hasattr(self, "_param_hints"):
             if isinstance(self._param_hints, Parameters):
                 return self._param_hints
             else:
                 raise TypeError(
                     f"{self.__class__.__name__} self._param_hints is not instance of Parameters"
                 )
 
     @param_hints.setter
     def param_hints(self, value, **kwargs):
-        # print(f'paramhints: val:{value},\nkw:{kwargs}')
         if isinstance(value, Parameters):
             param_hints_ = value
         else:
             dict_ = {}
             if isinstance(value, dict):
                 dict_ = {**dict_, **value}
             if kwargs:
                 dict_ = {**dict_, **kwargs}
-            # print(f'paramhints: {self},\n {dict_}')
             param_hints_ = LMfitModelConstructorMethods.param_hints_constructor(
                 param_hints=dict_, default_settings=self.default_settings
             )
         self._param_hints = param_hints_
         self.fco.store("user_input", "param_hints", param_hints_)
         if not isinstance(self, BasePeak):
             self.peak_model = self.create_peak_model()
@@ -438,18 +397,16 @@
         return self._peak_name
 
     @peak_name.setter
     def peak_name(self, value: str, maxlen=20):
         if len(value) < maxlen:
             prefix_set = value + "_"
             self._peak_name = value
-            # print(f"peak_name set:{value}")
             self.fco.store("user_input", "peak_name", value)
             self.peak_model = self.create_peak_model()
-            # self.set_peak_model_from_fields()
         else:
             raise ValueError(
                 f'The value "{value}" for peak_name is too long({len(value)}) (max. {maxlen}).'
             )
 
     def repr__(self):
         _repr = f"{self.__class__.__name__}"
@@ -476,22 +433,22 @@
     def print_params(self):
         if self.peak_model:
             self.peak_model.print_param_hints()
         else:
             print(f"No model set for: {self}")
 
 
-#%%
+# %%
+
 
-#%%
+# %%
 # LMfitModelConstructorMethods.create_peak_model_from_name_type_param_hints(peak_model= new.peak_model)
 # new.peak_name
-#%%
+# %%
 class LMfitModelConstructorMethods:
-
     PARAMETER_ARGS = inspect.signature(Parameter).parameters.keys()
 
     @classmethod
     def create_peak_model_from_name_type_param_hints(
         cls,
         peak_model: Model = None,
         peak_name: str = None,
@@ -601,22 +558,17 @@
                 for pname, par in param_hints_.items():
                     try:
                         _par_hint_dict = {
                             pn: getattr(par, pn, None)
                             for pn in cls.PARAMETER_ARGS
                             if getattr(par, pn, None)
                         }
-                        # _par_hint_dict = {k: val for k, val in _par_hint_dict.items() if val}
                         model.set_param_hint(**_par_hint_dict)
                     except Exception as e:
                         _error += f"Error in make_model_hints, check param_hints for {pname} with {par}, {e}"
-                # return model
             except Exception as e:
                 _error += f"Error in make_model_hints, check param_hints \n{e}"
         else:
             _error += f"TypeError in make_model_hints, check types of model {type(model)} param_hints_{type(param_hints_)}"
         if _error:
             warn("Errors found in setting of param hints: {_error}", BasePeakWarning)
         return model
-
-
-#%%
```

### Comparing `raman_fitting-0.6.18/src/raman_fitting/deconvolution_models/default_peaks/first_order_peaks.py` & `raman_fitting-0.7.0/src/raman_fitting/deconvolution_models/default_peaks/first_order_peaks.py`

 * *Files identical despite different names*

### Comparing `raman_fitting-0.6.18/src/raman_fitting/deconvolution_models/default_peaks/normalization_peaks.py` & `raman_fitting-0.7.0/src/raman_fitting/deconvolution_models/default_peaks/normalization_peaks.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 if __name__ == "__main__":
     from raman_fitting.deconvolution_models.base_peak import BasePeak
 else:
     from .base_peak import BasePeak
 
 __all__ = ["norm_G_peak", "norm_D_peak"]
+
 # ====== PEAKS USED FOR NORMALIZATION ======= #
 
 
 class norm_G_peak(metaclass=BasePeak):
     """G_peak used for normalization"""
 
     def __init__(self, *args, **kwargs):
@@ -17,16 +18,14 @@
         self.peak_type = "Lorentzian"
         self.input_param_settings = {
             "center": {"value": 1581, "min": 1500, "max": 1600},
             "sigma": {"value": 40, "min": 1e-05, "max": 1e3},
             "amplitude": {"value": 8e4, "min": 1e2},
         }
 
-    # norm_G_peak = BasePeak(peak_name=peak_name,peak_type=peak_type,input_param_settings=settings)
-
 
 class norm_D_peak(metaclass=BasePeak):
     """D_peak for normalization"""
 
     def __init__(self, *args, **kwargs):
         self.peak_name = "norm_D"
         self.peak_type = "Lorentzian"
```

### Comparing `raman_fitting-0.6.18/src/raman_fitting/deconvolution_models/default_peaks/second_order_peaks.py` & `raman_fitting-0.7.0/src/raman_fitting/deconvolution_models/default_peaks/second_order_peaks.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 if __name__ == "__main__":
     from raman_fitting.deconvolution_models.base_peak import BasePeak
 else:
     from .base_peak import BasePeak
 
 __all__ = ["D4D4_peak", "D1D1_peak", "GD1_peak", "D2D2_peak"]
 
+
 # ====== SECOND ORDER PEAKS ======= #
+
+
 class D4D4_peak(metaclass=BasePeak):
     """
     2nd order D4 peak
     """
 
     def __init__(self):
         self.peak_type = "Lorentzian"
@@ -41,15 +44,14 @@
 
 
 class GD1_peak(metaclass=BasePeak):
     """
     2nd order G+D(1) peak
     """
 
-    #        D2D2_mod = VoigtModel(prefix='D2D2_')
     def __init__(self):
         self.peak_type = "Lorentzian"
         self.peak_name = "GD1"
         self.input_param_settings = {
             "center": {"value": 2900, "min": 2800, "max": 2950},
             "sigma": {"value": 50, "min": 1, "max": 200},
             "amplitude": {"value": 10, "min": 1e-03, "max": 100},
@@ -57,20 +59,15 @@
 
 
 class D2D2_peak(metaclass=BasePeak):
     """
     2nd order D2 peak, aka 2D2
     """
 
-    #        D2D2_mod = VoigtModel(prefix='D2D2_')
-
     def __init__(self):
         self.peak_type = "Lorentzian"
         self.peak_name = "D2D2"
         self.input_param_settings = {
             "center": {"value": 3250, "min": 3000, "max": 3400},
             "sigma": {"value": 60, "min": 20, "max": 200},
             "amplitude": {"value": 1, "min": 1e-03, "max": 100},
         }
-
-
-# ====== SECOND ORDER PEAKS ======= #
```

### Comparing `raman_fitting-0.6.18/src/raman_fitting/deconvolution_models/fit_models.py` & `raman_fitting-0.7.0/src/raman_fitting/deconvolution_models/fit_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,14 @@
         self.FitResults = {}
         info = {}
         if hasattr(value, "info"):
             info = {**info, **value.info}
         self.info = info
 
     def fit_delegator(self):
-
         if self.start_fit:
             logger.info(
                 f"\n{self._qcnm} is starting to fit the models on spectrum:\n\t{self.info.get('SampleID','no name')}"
             )
 
             self.fit_models(self.models.second_order)  # second order should go first
             logger.info(
@@ -82,15 +81,14 @@
             # rum:\t{self.info.get('SampleID','no name')}\n")
             self.fit_models(self.models.first_order)
             logger.info(
                 f"\t - first order finished, {len(self.models.first_order)} models"
             )
 
     def fit_models(self, model_selection):
-
         _fittings = {}
         logger.debug(f"{self._qcnm} fit_models starting.")
         for modname, model in model_selection.items():
             modname, model
             _windowname = [i for i in self.fit_windows if modname[0:3] in i][0]
             _data = self.spectra.get(_windowname)
             _int_lbl = self.get_int_label(_data)
@@ -104,15 +102,15 @@
                 )
                 prep = PrepareParams(out, extra_fit_results=self.FitResults)
                 _fittings.update({modname: prep.FitResult})
             except Exception as e:
                 logger.warning(
                     f"{self._qcnm} fit_model failed for {modname}: {model}, because:\n {e}"
                 )
-            
+
         self.FitResults.update(**_fittings)
 
     def run_fit(self, model, _data, method="leastsq", **kws):
         # ideas: improve fitting loop so that starting parameters from modelX and modelX+Si are shared, faster...
         _fit_res, _param_res = {}, {}
         init_params = model.make_params()
         x, y = _data.ramanshift, _data[kws.get("_int_lbl")]
@@ -142,15 +140,14 @@
                 elif any("int" in i for i in cols):
                     _lbl = [i for i in cols if "int" in i][0]
 
         return _lbl
 
 
 class PrepareParams:
-
     fit_attr_export_lst = (
         "chisqr",
         "redchi",
         "bic",
         "aic",
         "method",
         "message",
@@ -201,19 +198,19 @@
             [i.prefix for i in self.comps]
         )  # peaks is prefix from components
 
         _mod_lbl = "Model"
         if hasattr(value, "_modelname"):
             _mod_lbl = f'Model_{getattr(value,"_modelname")}'
         self.model_name_lbl = _mod_lbl
-        
+
         self.raw_data_lbl = value._int_lbl
 
         self._model_result = value
-        
+
         self.make_result()
 
     def make_result(self):
         self.prep_params()
         self.prep_components()
         self.FitReport = self.model_result.fit_report(show_correl=False)
 
@@ -325,20 +322,19 @@
         else:
             return {}
 
     def prep_components(self):
         # FittingParams = pd.DataFrame(fit_params_od,index=[peak_model])
         _fit_comps_data = OrderedDict({"RamanShift": self.model_result.userkws["x"]})
         _fit_comps_data.update(self.model_result.eval_components())
-        
+
         # IDEA take out
         # print('===/n',self.model_result, '/n')
         # print('===/n',self.model_result.__dict__.keys(), '/n')
-        
-        
+
         _fit_comps_data.update(
             {
                 self.model_name_lbl: self.model_result.best_fit,
                 "residuals": self.model_result.residual,
                 self.model_result._int_lbl: self.model_result.data,
             }
         )
```

### Comparing `raman_fitting-0.6.18/src/raman_fitting/deconvolution_models/model_config.py` & `raman_fitting-0.7.0/src/raman_fitting/deconvolution_models/model_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,22 +11,20 @@
 else:
     from model_validation import PeakModelValidator
 
     from ..config.config import PACKAGE_HOME
 
 
 class ModelConfigurator:
-
     standard_config_file = "model_config_standard.cfg"
 
     def __init__(self, **kwargs):
         self._kwargs = kwargs
 
     def find_user_config_files(self):
         pass
 
     def file_handler(self):
         pass
 
     def standard_valid_models(self):
-
         peak_collection = PeakModelValidator()
```

### Comparing `raman_fitting-0.6.18/src/raman_fitting/deconvolution_models/peak_validation.py` & `raman_fitting-0.7.0/src/raman_fitting/deconvolution_models/peak_validation.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,30 +14,29 @@
 from typing import Tuple
 from warnings import warn
 
 import matplotlib.pyplot as plt
 import pandas as pd
 from lmfit import Parameters
 
-# _file_parent_name = Path(__file__).parent.name
-# print(__name__,__file__,f'name: {_file_parent_name}')
-
 if __name__ == "__main__":  # or _file_parent_name == 'deconvolution_models':
     # import first_order_peaks
     # import second_order_peaks
     # import normalization_peaks
     from default_peaks import BasePeak
+
+    __package_name__ = __name__
 else:
     from .. import __package_name__
     from .default_peaks.base_peak import BasePeak
 
-    logger = logging.getLogger(__package_name__)
+logger = logging.getLogger(__package_name__)
 
 
-#%%
+# %%
 class PeakValidationWarning(UserWarning):
     pass
 
 
 class NotFoundAnyModelsWarning(PeakValidationWarning):
     pass
 
@@ -67,22 +66,15 @@
     )
 
     CMAP_OPTIONS_DEFAULT = ("Dark2", "tab20")
     fallback_color = (0.4, 0.4, 0.4, 1.0)
 
     debug = False
 
-    # standard_model_selection = []
-    # _bad_models = []
-    # _skip_models = []
-    # endwsith = '_peak'
-
     def __init__(self, *args, cmap_options=CMAP_OPTIONS_DEFAULT, **kwargs):
-        # self.model_prefixes = model_prefixes
-        # self._endswith = endwsith
         self.debug = self._set_debug(**kwargs)
         self._cmap_options = cmap_options
 
         self._inspect_models = self.get_subclasses_from_base(self.BASE_PEAK)
 
         self.valid_models = []
         self._invalid_models = []
@@ -94,17 +86,14 @@
 
         self.lmfit_models = self.assign_colors_to_lmfit_mod_inst(self.selected_models)
         self.add_model_names_var_names(self.lmfit_models)
 
         self.model_dict = self.get_model_dict(self.lmfit_models)
         self.options = self.model_dict.keys()
 
-        # self.options = ()
-        # self.extra_assignments()
-
     def _set_debug(self, **value):
         _debug = self.debug
         if isinstance(value, dict):
             if "debug" in value.keys():
                 _debug = bool(value.get("debug", False))
         return _debug
 
@@ -132,26 +121,17 @@
             warn(
                 f"\nNo baseclasses were found in inspected modules for {str(_BaseClass)}:\n",
                 NotFoundAnyModelsWarning,
             )
 
         return _all_subclasses
 
-        # {", ".join(self._standard_modules)}
-        # elif not self._inspect_models:
-        # warn(f'\nNo base models were found in:\n {", ".join([str(i) for i in self._inspect_modules_all])}.\n', NotFoundAnyModelsWarning)
-        # assert self._inspect_models, 'inspect.getmembers found 0 models, change the search parameters for _standard_modules or BASE_PEAK'
-
     def _inspect_modules_for_classes(self):
         """Optional method Inspect other modules for subclasses"""
         pass
-        # self._inspect_modules_all = _all_subclasses
-        # [cl for i in (inspect.getmembers(mod, inspect.isclass)
-        # for mod in self._standard_modules)
-        # for cl in i]
 
     def validation_inspect_models(self, inspect_models: list = []):
         """Validates each member of a list for making a valid model instance"""
         _model_validations = []
         valid_models = []
 
         for model in inspect_models:
@@ -178,20 +158,14 @@
             )
 
         return valid_models, _invalid_models
 
     def filter_valid_models(self, value):
         """Optional method for extra filters on valid model selection"""
         return value
-        # self._skipped_models = set(self._bad_models + self._skip_models)
-        # if self.standard_model_selection:
-        # self.selected_models = [i for i in self.valid_models if not i.model_inst.name in self._skipped_models]
-        # if self._endswith:
-        # self.selected_models = [(m, ngr) for m, ngr in self.valid_models
-        # if (i.model_inst.name.endswith(self._endswith) and not i.model_inst.name  in self._skipped_models)]
 
     def sort_selected_models(self, value):
         """Sorting the selected valid models for color assigment etc.."""
         _sorted = value
         _setting_key = None
         try:
             _setting_key = [i for i in self.BASE_PEAK._fields if "param_hints" in i]
@@ -242,25 +216,23 @@
                     )
         return (True, _inst, f"{_inst} is a valid model")
 
     @staticmethod
     def get_cmap_list(
         lst, cmap_options: Tuple = (), fallback_color: Tuple = ()
     ) -> Tuple:
-
         cmap = [(0, 0, 0, 1) for i in lst]  # black as fallback default color
 
         # set fallback color from class
         if isinstance(fallback_color, tuple):
             if len(fallback_color) == 4:
                 cmap = [fallback_color for i in lst]
 
         # set cmap colors from cmap options
         if cmap_options:
-
             try:
                 pltcmaps = [plt.get_cmap(cmap) for cmap in cmap_options]
                 # Take shortest colormap but not
                 cmap = min(
                     [i for i in pltcmaps if len(lst) <= len(i.colors)],
                     key=lambda x: len(x.colors),
                     default=cmap,
@@ -281,20 +253,17 @@
             fallback_color=self.fallback_color,
         )
         lmfit_models = []
         for n, _arg in enumerate(selected_models):
             _m_inst = _arg.model_inst
             _m_inst._modelvalidation = _arg
             _m_inst.color = ", ".join([str(i) for i in cmap_get[n]])
-            # _m_inst._funcname = str(m).split('__main__.')[-1][:-2]
             _m_inst._lenpars = len(_m_inst.peak_model.param_names)
             lmfit_models.append(_m_inst)
         return lmfit_models
-        # self.lmfit_models= sorted(self.lmfit_models, key= lambda x: x._lenpars)
-        # self.lmfit_models = _mod_inst
 
     def add_standard_init_params(self):
         self.standard_init_params = Parameters()
         self.standard_init_params.add_many(*BasePeak._params_guesses_base)
 
     def add_model_names_var_names(self, lmfit_models):
         _mod_param_names = {
@@ -322,38 +291,31 @@
 
     def get_dict(self):
         return {
             i.__module__ + ", " + i.__class__.__name__: i for i in self.lmfit_models
         }
 
     def __getattr__(self, name):
-        # raise AttributeError(f'Chosen name "{name}" not in in options: "{", ".join(self.options)}".')
         try:
             _options = self.__getattribute__("options")
             if name in _options:
                 return self.model_dict.get(name, None)
             raise AttributeError(
                 f'Chosen name "{name}" not in options: "{", ".join(_options)}".'
             )
         except AttributeError:
-            # if 'normalization' in name:
-            # return self.normalization_model()
             raise AttributeError(f'Chosen name "{name}" not in attributes')
-        # else:
-        # raise AttributeError(f'Chosen name "{name}" not in in options: "{", ".join(self.options)}".')
 
     def normalization_model(self):
         pass  # IDEA separate peaks in groups
 
     def __iter__(self):
         for mod_inst in self.lmfit_models:
             yield mod_inst
-        # self.params_set = set([a for m in self.lmfit_models for a in m[1].param_names])
 
-    #    lmfit_models = [Model(i.func,name=i.name) for i in model_selection]
     def __repr__(self):
         _repr = "Validated Peak model collection"
         if self.selected_models:
             _selmods = f", {len(self.selected_models)} models from: " + "\n\t- "
             _repr += _selmods
             _joinmods = "\n\t- ".join(
                 [f"{i.peak_group}: {i.model_inst} \t" for i in self.selected_models]
```

### Comparing `raman_fitting-0.6.18/src/raman_fitting/delegating/main_delegator.py` & `raman_fitting-0.7.0/src/raman_fitting/delegating/main_delegator.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,42 +14,21 @@
 from raman_fitting.exporting.exporter import Exporter
 from raman_fitting.indexing.indexer import MakeRamanFilesIndex
 from raman_fitting.processing.spectrum_constructor import (
     SpectrumDataCollection,
     SpectrumDataLoader,
 )
 
-# from processing.cleaner import SpectrumCleaner
 from raman_fitting.processing.spectrum_template import SpectrumTemplate
 from raman_fitting.interfaces.cli import RUN_MODES
 
 if __name__ == "__main__":
     pass
 
-
-# else:
-#     # from .. import __package_name__
-#     from ..cli.cli import RUN_MODES
-#     from ..config import config
-#     from ..config.filepaths import get_directory_paths_for_run_mode
-#     from ..deconvolution_models.fit_models import Fitter
-#     from ..deconvolution_models.base_model import InitializeModels
-#     from ..export.exporter import Exporter
-#     from ..indexer.indexer import MakeRamanFilesIndex
-#     from ..processing.spectrum_constructor import (
-#         SpectrumDataCollection,
-#         SpectrumDataLoader,
-#     )
-
-#     # from processing.cleaner import SpectrumCleaner
-#     from ..processing.spectrum_template import SpectrumTemplate
-
 logger = logging.getLogger(__name__)
-# from raman_fitting.indexer.indexer import OrganizeRamanFiles
-# from raman_fitting.processing.spectrum_constructor import SpectrumDataLoader, SpectrumDataCollection
 
 
 class prdError(Exception):
     """Base error raised by pyramdeconv (future package name of raman_fitting)."""
 
 
 class MainDelegatorError(prdError):
@@ -62,20 +41,15 @@
     """
     Main delegator for the processing of files containing Raman spectra.
 
     Input parameters is DataFrame of index
     Creates plots and files in the config RESULTS directory.
     """
 
-    # DEFAULT_RUN_MODE = {'run_mode' : 'normal'}
-    # _kwargs = {}
-
     def __init__(self, run_mode="normal", **kwargs):
-
-        # print(f'{self} kwargs:', kwargs)
         self.kwargs = kwargs
         self._cqnm = __class__.__qualname__
 
         self.run_mode = run_mode
         if run_mode not in RUN_MODES:
             logger.warning(
                 f"{self}\n\twarning run_mode choice {run_mode} not in\n\t{RUN_MODES}"
@@ -83,27 +57,21 @@
 
         self.dest_dirs = get_directory_paths_for_run_mode(run_mode=run_mode)
         self.RESULTS_DIR = self.dest_dirs["RESULTS_DIR"]
         self.DATASET_DIR = self.dest_dirs["DATASET_DIR"]
         self.INDEX_FILE = self.dest_dirs["INDEX_FILE"]
 
         self.spectrum = SpectrumTemplate()
-        # self.index = RamanIndex
 
         self.run_delegator(**self.kwargs)
 
     def index_delegator(self, **kwargs):
-
         RF_index = MakeRamanFilesIndex(
             **kwargs,
         )
-        # run_mode=self.run_mode,
-        # RESULTS_DIR=self.RESULTS_DIR,
-        # DATASET_DIR=self.DATASET_DIR,
-        # INDEX_FILE=self.INDEX_FILE,
         logger.info(f"index_delegator index prepared with len {len(RF_index)}")
         return RF_index
 
     def run_delegator(self, **kwargs):
         # IDEA remove self.set_models() removed InitModels
         self._failed_samples = []
         self.export_collect = []
@@ -130,15 +98,14 @@
             logger.info(
                 f"\n{self._cqnm} models initialized for run mode ({self.run_mode}):\n\n{repr(models)}"
             )
 
             if self.run_mode in ("normal", "make_examples"):
                 if not self.index.empty:
                     logger.debug(f"{self._cqnm}. starting run generator.")
-                    # self.index
 
                     self._run_gen(**self.kwargs)
                 else:
                     pass
                 # info raman loop finished because index is empty
             elif self.run_mode == "DEBUG":
                 logger.debug(f"Debug run mode {self}. Models initialized {models}")
@@ -182,68 +149,56 @@
             yield (grpnm, nm, sID_grp)
 
     def _run_gen(self, **kwargs):
         # #IDEA sort of coordinator coroutine, can implement still deque
         sgrp_grpby = self.index.groupby(self.spectrum.grp_names.sGrp_cols[0])
         logger.info(f"{self._cqnm} _run_gen starting: {kwargs}")
         _mygen = self._generator(sgrp_grpby, **kwargs)
-        Exporter(self.export_collect)  # clean up and 
+        Exporter(self.export_collect)  # clean up and
         logger.info(
-                    f"\n{self._cqnm} run finished.\n Results saved in {self.RESULTS_DIR}"
-                )
+            f"\n{self._cqnm} run finished.\n Results saved in {self.RESULTS_DIR}"
+        )
 
     def _generator(self, sgrp_grpby, **kwargs):
-        # _sgrpgen = self.sample_group_gen()
         export_collect = []
         for sgrpnm, sgrp_grp in sgrp_grpby:
             sID_grpby = sgrp_grp.groupby(list(self.spectrum.grp_names.sGrp_cols[1:]))
-            # _sID_gen = self._sID_gen(grpnm, sgrp_grp)
             logger.info(f"{self._cqnm} _generator starting group: {sgrpnm}")
             exporter_sample = None
             for sIDnm, sIDgrp in sID_grpby:
                 try:
                     exporter_sample = self.simple_process_sample_wrapper(
                         sgrpnm, sIDnm, sIDgrp, **kwargs
                     )
-                    # yield from self.simple_process_sample_wrapper(_sID_gen, **kwargs)
-                    # starmap(process_sample_wrapper, args_for_starmap )
-                    # args_for_starmap = zip(repeat(self.process_sample), _sID_gen, repeat(kwargs))
                 except GeneratorExit:
                     logger.warning(f"{self._cqnm} _generator closed.")
                     return ()
                 except Exception as e:
                     logger.warning(f"{self._cqnm} _generator exception: {e}")
-                    # return ()
                 export_collect.append(exporter_sample)
         return export_collect
 
     def coordinator(self):
         pass
 
     def simple_process_sample_wrapper(self, *sID_args, **kwargs):
-        # if _gen:
-        # for sID_args in _gen:
         logger.info(
             f"{self._cqnm} starting simple process_sample_wrapper args:\n\t - {sID_args[0]}\n\t - {kwargs.keys()}"
         )
         exporter_sample = None
         try:
             logger.debug(
                 f"{self._cqnm} simple process_sample_wrapper starting:\n\t - {sID_args[1]}"
             )
             exporter_sample = self.process_sample(*sID_args, **kwargs)
             if exporter_sample:
                 logger.debug(
                     f"{self._cqnm} simple process_sample_wrapper appending export:\n\t - {exporter_sample}"
                 )
                 self.export_collect.append(exporter_sample)
-        # except StopIteration:
-        # logger.info(
-        #     f"{self._cqnm} _gen StopIteration for simple process wrapper "
-        # )
         except Exception as e:
             logger.warning(
                 f"{self._cqnm} simple process_sample_wrapper exception on call process sample: {e}"
             )
             self._failed_samples.append((e, sID_args, kwargs))
         return exporter_sample
 
@@ -260,37 +215,31 @@
         """
         Loops over individual Sample positions (files) from a SampleID and performs the
         fitting, plotting and exporting.
         """
         logger.info(
             f"{self._cqnm} process_sample called:\n\t - {sgrpnm}, {sIDnm}\n\t - {kwargs.keys()}"
         )
-        # self = args[0]
-        # args = args[]
-        # grpnm, nm, sID_grp = args
 
         models = kwargs.get("models", None)
 
-        # sGr, (sID, sDate) = sgrpnm, nm # just for developer
-
         sGr_out = dict(zip(self.spectrum.grp_names.sGrp_cols, (sgrpnm,) + sIDnm))
         export_info_out = add_make_sample_group_destdirs(sID_grp)
         sample_pos_grp, sPos_cols = self.test_positions(
             sID_grp, sIDnm, list(self.spectrum.grp_names.sPos_cols)
         )
 
         sample_spectra = []
         for meannm, meangrp in sample_pos_grp:
             logger.info(f"{self._cqnm} process sample mean loop file: {meannm}.")
             sPos_out = dict(zip(self.spectrum.grp_names.sPos_cols, meannm))
             _spectrum_position_info_kwargs = {**sGr_out, **export_info_out, **sPos_out}
             spectrum_data = SpectrumDataLoader(
                 file=meannm[-1], run_kwargs=_spectrum_position_info_kwargs, ovv=meangrp
             )
-            # spectrum_data.plot_raw()
             sample_spectra.append(spectrum_data)
         if sample_spectra:
             spectra_collection = SpectrumDataCollection(sample_spectra)
             ft = Fitter(spectra_collection, RamanModels=models)
             rex = Exporter(ft)
             return rex
         else:
@@ -298,30 +247,16 @@
                 f"{self._cqnm} process sample spectra empty {','.join(map(str,[sgrpnm, sIDnm]))}."
             )
             return None
 
     def __repr__(self):
         return f'Maindelegator: run_mode = {self.run_mode}, {", ".join([f"{k} = {str(val)}" for k,val in self.kwargs.items()])}'
 
-        # _count = 0
-        # while True:
-        #     try:
-        #         next(_mygen)
-        #         _count += 1
-        #     except StopIteration:
-        #         logger.debug(
-        #             f"{self._cqnm} _run_gen StopIteration after {_count } steps"
-        #         )
-        #         # print('StopIteration for mygen')
-        #         break
-        #     finally:
-
 
 def add_make_sample_group_destdirs(sample_grp: pd.DataFrame):
-
     dest_grp_dir = Path(
         sample_grp.DestDir.unique()[0]
     )  # takes one destination directory from Sample Groups
     dest_fit_plots = dest_grp_dir.joinpath("Fitting_Plots")
     dest_fit_comps = dest_grp_dir.joinpath("Fitting_Components")
     dest_fit_comps.mkdir(parents=True, exist_ok=True)
 
@@ -341,20 +276,18 @@
     def wrapper(*args, **kwargs):
         logger.debug(
             f"process_sample_wrapper args:\n\t - {fn}\n\t - {args}\n\t - {kwargs.keys()}"
         )
         exp_sample = None
         try:
             exp_sample = fn(*args, **kwargs)
-            # self.export_collect.append(exp_sample)
         except Exception as e:
             logger.error(
                 f"process_sample_wrapper process_sample_wrapper exception on call {fn}: {e}"
             )
-            # self._failed_samples.append((e, args, kwargs))
             exp_sample = (e, args, kwargs)
 
         return exp_sample
 
 
 def make_examples():
     _main_run = MainDelegator(run_mode="make_examples")
```

### Comparing `raman_fitting-0.6.18/src/raman_fitting/exporting/exporter.py` & `raman_fitting-0.7.0/src/raman_fitting/exporting/exporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,14 @@
             k: val for k, val in self.fitter.FitResults.items() if k.startswith("1st")
         }
         _2nd = {
             k: val for k, val in self.fitter.FitResults.items() if k.startswith("2nd")
         }
 
         for modname_2, fitres_2 in _2nd.items():
-
             self.export_xls_from_spec(fitres_2)
             pars2.append(fitres_2.FitParameters)
             for modname_1, fitres_1 in _1st.items():
                 self.export_xls_from_spec(fitres_1)
                 try:
                     fit_spectrum_plot(
                         modname_1,
```

### Comparing `raman_fitting-0.6.18/src/raman_fitting/exporting/plotting.py` & `raman_fitting-0.7.0/src/raman_fitting/exporting/plotting.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 import matplotlib.lines as mlines
 import matplotlib.pyplot as plt
 from matplotlib import gridspec
 from matplotlib.ticker import AutoMinorLocator, FormatStrFormatter, MultipleLocator
 
 matplotlib.rcParams.update({"font.size": 14})
 
-#%%
+# %%
+
 
 # IDEA PLOTTING PER PEAK MODEL
 def plotting_info(windowname):  # pragma: no cover
     axes = {
         "full": (0, 0),
         "low": (0, 1),
         "1st_order": (0, 2),
@@ -45,15 +46,14 @@
     try:
         fig, ax = plt.subplots(2, 3, figsize=(18, 12))
         ax_wn = []
 
         for spec in fitting_specs:
             try:
                 ax_wn = ax[plotting_info(spec.windowname)]
-                #                spec.windowname
                 _legend = True if "full" == spec.windowname else False
                 spec.mean_spec.plot(
                     x="ramanshift",
                     y=spec.sID_rawcols,
                     ax=ax_wn,
                     alpha=0.5,
                     legend=_legend,
@@ -65,15 +65,14 @@
                     c="k",
                     alpha=0.7,
                     lw=3,
                     legend=_legend,
                 )
 
                 ax_wn.set_title(spec.windowname)
-                #                _legend = True if 'full' in spec.windowname else False
                 if _legend:
                     ax_wn.legend(fontsize=10)
 
             except:
                 pass
 
         plt.suptitle(spec.sIDmean_col, fontsize=16)
@@ -84,71 +83,61 @@
         )
         plt.close()
     except Exception as e:
         print("no extra Raw Data plots: {0}".format(e))
 
 
 def raw_data_spectra_export(fitting_specs):
-    #    fitting_specs
     try:
         for spec in fitting_specs:
-            #            spec.windowname, spec.sIDmean_col
             wnxl_outpath_spectra = spec.mean_info.DestRaw.unique()[0].joinpath(
                 f"spectra_{spec.sIDmean_col}_{spec.windowname}.xlsx"
             )
             spec.mean_spec.to_excel(wnxl_outpath_spectra)
 
         _0_spec = fitting_specs[0]
         wnxl_outpath_info = _0_spec.mean_info.DestRaw.unique()[0].joinpath(
             f"info_{_0_spec.sIDmean_col}.xlsx"
         )
         _0_spec.mean_info.to_excel(wnxl_outpath_info)
-
-    #            ax_wn = ax[plotting_info(spec.windowname)]
     except Exception as e:
         print("no extra Raw Data plots: {0}".format(e))
 
 
 def fit_spectrum_plot(
     peak1,
     peak2,
     res1_peak_spec,
     res2_peak_spec,
     plot_Annotation=True,
     plot_Residuals=True,
 ):  # pragma: no cover
-
     modname_2 = peak2
-    #%%
+    # %%
     sID = res1_peak_spec.extrainfo["SampleID"]
     SampleBgmean_col = res1_peak_spec.raw_data_col
 
-    #    sID, DestPlotDir, SampleBgmean_col, FitData, FitModPeaks, FitData_2nd,comps, comps_2nd,out, out_2nd,
     FitData_1st = res1_peak_spec.FitComponents
     Model_peak_col_1st = res1_peak_spec.model_name
     Model_data_col_1st = res1_peak_spec.model_name
-    # f'Model_{Model_peak_col_1st}'
     compscols_1st = [
         i for i in FitData_1st.columns if i.endswith("_") and not i.startswith("Si")
     ]
-    #    FitReport_1st = res1_peak_spec.FitReport
 
     FitData_2nd = res2_peak_spec.FitComponents
     Model_peak_col_2nd = res2_peak_spec.model_name
     Model_data_col_2nd = res2_peak_spec.model_name
-    # f'Model_{Model_peak_col_2nd}'
     compscols_2nd = [i for i in FitData_2nd.columns if i.endswith("_")]
 
     FitPars, FitPars_2nd = res1_peak_spec.FitParameters, res2_peak_spec.FitParameters
 
     fig = plt.figure(figsize=(28, 24))
     gs = gridspec.GridSpec(4, 1, height_ratios=[4, 1, 4, 1])
     ax = plt.subplot(gs[0])
     axRes = plt.subplot(gs[1])
-    #                axAnn = plt.subplot(gs[1])
     ax2nd = plt.subplot(gs[2])
     ax2ndRes = plt.subplot(gs[3])
     ax2ndRes.grid(True), axRes.grid(True, "both")
     ax2nd.grid(True), ax.grid(True, "both")
     ax.get_yaxis().set_tick_params(direction="in")
     ax.get_xaxis().set_tick_params(direction="in")
     ax.set_title(SampleBgmean_col)
@@ -157,17 +146,14 @@
     ax.yaxis.set_minor_locator(AutoMinorLocator(2))
     ax.tick_params(which="both", direction="in")
     ax2nd.xaxis.set_minor_locator(AutoMinorLocator(2))
     ax2nd.yaxis.set_minor_locator(AutoMinorLocator(2))
     ax2nd.tick_params(which="both", direction="in")
     ax.set_facecolor("oldlace"), ax2nd.set_facecolor("oldlace")
     axRes.set_facecolor("oldlace"), ax2ndRes.set_facecolor("oldlace")
-    #                for FitN in [PosInts_Bg,PosInts_Bg_2nd]:
-    #                    fig,ax = plt.subplots(1,1,figsize=(12,12))
-    #                if FitN.RamanShift.max() > 2300:
     ax2nd.plot(
         FitData_2nd["RamanShift"],
         FitData_2nd[Model_data_col_2nd],
         label=Model_data_col_2nd,
         lw=3,
         c="r",
     )
@@ -205,19 +191,15 @@
             f"{fit_comp_col_2nd}\n {FitPars_2nd[center_col].round(0).iloc[0]:.0f}",
             xy=(
                 FitPars_2nd[center_col].iloc[0] * 0.97,
                 0.8 * FitPars_2nd[height_col].iloc[0],
             ),
             xycoords="data",
         )
-    #    ax2nd.plot(FitData_2nd['RamanShift'], comps_2nd['D1D1_'], color='lime',ls='--',lw=4,label='2*D')
-    #    ax2nd.plot(FitData_2nd['RamanShift'], comps_2nd['D4D4_'], color='purple',ls='--',lw=4,label='2*D4')
-    #    ax2nd.plot(FitData_2nd['RamanShift'], comps_2nd['GD1_'], color='pink',ls='--',lw=4,label='G+D1')
     ax2nd.set_ylim(-0.02, FitData_2nd[Model_data_col_2nd].max() * 1.5)
-    #                else:
     ax.plot(
         FitData_1st["RamanShift"],
         FitData_1st[Model_data_col_1st],
         label=Model_data_col_1st,
         lw=3,
         c="r",
     )
@@ -225,15 +207,15 @@
         FitData_1st["RamanShift"],
         FitData_1st[res1_peak_spec.raw_data_col],
         label="Data",
         lw=3,
         c="grey",
         alpha=0.8,
     )
-    
+
     if plot_Residuals:
         axRes.plot(
             FitData_1st["RamanShift"],
             FitData_1st[res1_peak_spec.raw_data_col] - FitData_1st[Model_data_col_1st],
             label="Residual",
             lw=3,
             c="k",
@@ -254,46 +236,28 @@
         )
         ax.annotate(
             f"{fit_comp_col_1st}:\n {FitPars[center_col].round(0).iloc[0]:.0f}",
             xy=(FitPars[center_col].iloc[0] * 0.97, 0.7 * FitPars[height_col].iloc[0]),
             xycoords="data",
         )
 
-    #    ax.plot(FitData_1st['RamanShift'], FitData_1st['D_'], color='lime',ls='--',lw=4,label='D')
-    #                ax.plot(FitData['RamanShift'], comps['D2_'], color='grey',ls='--',lw=4,label='D2')
-    #    ax.plot(FitData_1st['RamanShift'], FitData_1st['D3_'], 'b--',lw=4,label='D3')
-    #    ax.plot(FitData_1st['RamanShift'], FitData_1st['D4_'], color='purple',ls='--',lw=4,label='D4')
-    if "peaks" in peak1:
-        #        ax.plot(FitData_1st['RamanShift'], FitData_1st['D2_'], color='magenta',ls='--',lw=4,label='D2')
-        #        ax.annotate('D2:\n %.0f'%FitPars['D2_center'],xy=(FitPars['D2_center']*0.97,0.8*FitPars['I_D2']),xycoords='data')
-        if peak1.endswith("+Si"):
-            ax.plot(
-                FitData_1st["RamanShift"],
-                FitData_1st["Si1_"],
-                "b--",
-                lw=4,
-                label="Si_substrate",
+    if "peaks" in peak1 and peak1.endswith("+Si"):
+        ax.plot(
+            FitData_1st["RamanShift"],
+            FitData_1st["Si1_"],
+            "b--",
+            lw=4,
+            label="Si_substrate",
+        )
+        if FitPars["Si1_fwhm"].iloc[0] > 1:
+            ax.annotate(
+                "Si_substrate:\n %.0f" % FitPars["Si1_center"],
+                xy=(FitPars["Si1_center"] * 0.97, 0.8 * FitPars["Si1_height"]),
+                xycoords="data",
             )
-            if FitPars["Si1_fwhm"].iloc[0] > 1:
-                ax.annotate(
-                    "Si_substrate:\n %.0f" % FitPars["Si1_center"],
-                    xy=(FitPars["Si1_center"] * 0.97, 0.8 * FitPars["Si1_height"]),
-                    xycoords="data",
-                )
-    #        if '6peaks' in FitModPeaks:
-    #            ax.plot(FitData_1st['RamanShift'], FitData_1st['D5_'],  color='darkorange',ls='--',lw=4,label='D5')
-    #            ax.annotate('D5:\n %.0f'%FitPars['D5_center'],xy=(FitPars['D5_center']*0.97,0.8*FitPars['I_D5']),xycoords='data')
-    ##                    for colN,col in FitN.iteritems():
-    #                        if 'RamanShift' in colN or colN.split('_')[-1] == 'count' or colN.split('_')[-1] == 'std' :
-    #                            continue
-    #                        w,i = FitN['RamanShift'].values,col.values
-    #                        if 'mean' in colN:
-    #                            ax.plot(w[::],i[::],label=colN)
-    #                        else:
-    #                            ax.scatter(w[::],i[::],label=colN)
     if plot_Annotation:
         frsplit = res1_peak_spec.FitReport.split()
         if len(frsplit) > 200:
             fr = res1_peak_spec.FitReport.replace("prefix='D3_'", "prefix='D3_' \n")
         else:
             fr = res1_peak_spec.FitReport
         props = dict(boxstyle="round", facecolor="wheat", alpha=0.5)
@@ -318,18 +282,15 @@
 
     ax.legend(loc=1), ax.set_xlabel("Raman shift (cm$^{-1}$)"), ax.set_ylabel(
         "normalized I / a.u."
     )
     ax2nd.legend(loc=1), ax2nd.set_xlabel("Raman shift (cm$^{-1}$)"), ax2nd.set_ylabel(
         "normalized I / a.u."
     )
-    #                plt.show()
 
-    #    plt.show()
     plt.savefig(
         res1_peak_spec.extrainfo["DestFittingModel"].with_suffix(".png"),
         dpi=100,
         bbox_extra_artists=(Report1, Report2),
         bbox_inches="tight",
     )
     plt.close()
-    #%%
```

### Comparing `raman_fitting-0.6.18/src/raman_fitting/indexing/filedata_parser.py` & `raman_fitting-0.7.0/src/raman_fitting/indexing/filedata_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import numpy as np
 import pandas as pd
 
 
 logger = logging.getLogger(__name__)
 
 
-#%%
+# %%
 class SpectrumReader:
     """
     Reads a clean spectrum from a file Path or str
 
     with columns "ramanshift" and "intensity".
     Double checks the values
     Sets a hash attribute afterwards
@@ -37,30 +37,28 @@
     # using slots since there will be many instances of this class
 
     __slots__ = (
         *("filepath", "max_bytesize", "spectrum", "spectrum_hash", "spectrum_length"),
         *spectrum_keys_expected_values.keys(),
     )
 
-    def __init__(self, filepath: Path, max_bytesize=10 ** 6):
-
+    def __init__(self, filepath: Path, max_bytesize=10**6):
         if not isinstance(filepath, Path):
             if isinstance(filepath, str):
                 filepath = Path(filepath)
             else:
                 raise TypeError("Argument given is not Path nor str")
 
         self.filepath = filepath
         self.max_bytesize = max_bytesize
 
         self.spectrum = pd.DataFrame(data=[], columns=self.spectrum_data_keys)
         if filepath.exists():
             filesize = filepath.stat().st_size
             if filesize < max_bytesize:
-
                 self.spectrum = self.spectrum_parser(self.filepath)
                 self.double_check_spectrum_values(
                     self.spectrum, expected_values=self.spectrum_keys_expected_values
                 )
         else:
             logger.warning("File does not exist")
 
@@ -87,15 +85,14 @@
 
         spectrum_data = pd.DataFrame()
 
         suffix = ""
         suffix = filepath.suffix
         if suffix in self.supported_filetypes:
             if suffix == ".txt":
-
                 try:
                     spectrum_data = self.use_np_loadtxt(filepath)
 
                 except Exception as exc:
                     logger.warning(
                         f"Can not complete use_np_loadtxt for:\n{filepath}\n{exc}"
                     )
@@ -112,15 +109,14 @@
 
         else:
             logger.warning(f"Filetype {suffix} not supported")
 
         return spectrum_data
 
     def use_np_loadtxt(self, filepath, usecols=(0, 1), **kwargs):
-
         try:
             loaded_array = np.loadtxt(filepath, usecols=usecols, **kwargs)
         except IndexError:
             logger.debug(f"IndexError called np genfromtxt for {filepath}")
             loaded_array = np.genfromtxt(filepath, invalid_raise=False)
         except ValueError:
             logger.debug(f"ValueError called np genfromtxt for {filepath}")
@@ -143,15 +139,14 @@
 
     def double_check_spectrum_values(
         self, spectrum_data: pd.DataFrame, expected_values: dict = {}
     ):
         if all([i in spectrum_data.columns for i in expected_values.keys()]):
             _len = len(spectrum_data)
             for _key, expectations in expected_values.items():
-
                 if expectations:
                     for exp_method, exp_value in expectations.items():
                         _check = False
                         if "len" in exp_method:
                             _spectrum_value = _len
                             _check = np.isclose(_spectrum_value, exp_value, rtol=0.1)
 
@@ -172,15 +167,15 @@
                             )
         else:
             logger.error(
                 f"The dataframe does not have all the keys from {self.spectrum_data_keys}"
             )
 
     @staticmethod
-    def read_text(filepath, max_bytes=10 ** 6, encoding="utf-8", errors=None):
+    def read_text(filepath, max_bytes=10**6, encoding="utf-8", errors=None):
         """additional read text method for raw text data inspection"""
         _text = "read_text_method"
         filesize = filepath.stat().st_size
         if filesize < max_bytes:
             try:
                 _text = filepath.read_text(encoding=encoding, errors=errors)
                 # _text.splitlines()
@@ -230,8 +225,8 @@
         return _txt
 
     def quickplot(self):
         """Plot for quickly checking the spectrum"""
         try:
             self.spectrum.plot(x="ramanshift", y="intensity")
         except TypeError:
-            logger.warning(f"No numeric data to plot")
+            logger.warning("No numeric data to plot")
```

### Comparing `raman_fitting-0.6.18/src/raman_fitting/indexing/filename_parser.py` & `raman_fitting-0.7.0/src/raman_fitting/indexing/filename_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # from .. import __package_name__
 
 from .filedata_parser import SpectrumReader
 from .filename_parser_helpers import filestem_to_sid_and_pos, sID_to_sgrpID, get_fstats
 
 logger = logging.getLogger(__name__)
 
-#%%
+# %%
 # _extra_sID_name = 'Si-ref'
 index_primary_key = "rfID"
 index_file_primary_keys = {f"{index_primary_key}": "string"}
 index_file_path_keys = {"FileStem": "string", "FilePath": "Path"}
 index_file_sample_keys = {
     "SampleID": "string",
     "SamplePos": "int64",
```

### Comparing `raman_fitting-0.6.18/src/raman_fitting/indexing/filename_parser_collector.py` & `raman_fitting-0.7.0/src/raman_fitting/indexing/filename_parser_collector.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 logger = logging.getLogger(__name__)
 
 from .filename_parser import PathParser
 
 
 def make_collection(raman_files: Collection, **kwargs) -> List[PathParser]:
-
     pp_collection = []
     # _error_parse_filenames
     for file in raman_files:
         try:
             pp_res = PathParser(file, **kwargs)
             pp_collection.append(pp_res)
         except Exception as e:
```

### Comparing `raman_fitting-0.6.18/src/raman_fitting/indexing/filename_parser_helpers.py` & `raman_fitting-0.7.0/src/raman_fitting/indexing/filename_parser_helpers.py`

 * *Files identical despite different names*

### Comparing `raman_fitting-0.6.18/src/raman_fitting/indexing/indexer.py` & `raman_fitting-0.7.0/src/raman_fitting/indexing/indexer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,78 +1,53 @@
 """ Indexer for raman data files """
-import hashlib
-from typing import List
-
-# get_directory_paths_for_run_mode
-# from .index_selection import index_selection
 import logging
-import sys
 from pathlib import Path
+import sys
+from typing import List
 
 import pandas as pd
 
 from raman_fitting.config.filepath_helper import get_directory_paths_for_run_mode
-
-# parse_filepath_to_sid_and_pos
 from raman_fitting.indexing.filename_parser import index_dtypes_collection
 from raman_fitting.indexing.filename_parser_collector import make_collection
 
-# from raman_fitting.utils._dev_sqlite_db import df_to_db_sqlalchemy
-
-# from .. import __package_name__
-
-
 logger = logging.getLogger(__name__)
 logger.propagate = False
 
 __all__ = ["MakeRamanFilesIndex"]
 
-#%%
-
 
 class MakeRamanFilesIndex:
     """
 
     Finds the RAMAN files in the data folder from config and creates an overview, on the attribute .index
     finds a list of files,
 
     """
 
-    # index_file_sample_cols = {'FileStem': 'string',
-    #                           'SampleID': 'string',
-    #                           'SamplePos': 'int64',
-    #                           'SampleGroup': 'string',
-    #                           'FilePath': 'string')
-    # index_file_stat_cols = ('FileCreationDate' , 'FileCreation','FileModDate', 'FileMod', 'FileHash')
-    # INDEX_FILE_NAME = 'index.csv'
     debug = False
 
     table_name = "ramanfiles"
 
-    # RESULTS_DIR = config.RESULTS_DIR,
-    #              DATASET_DIR = config.DATASET_DIR,
-    #              INDEX_FILE = config.INDEX_FILE,
     def __init__(
         self, force_reload=True, run_mode="normal", dataset_dirs=None, **kwargs
     ):
-
         self._cqnm = self.__class__.__qualname__
 
         self._kwargs = kwargs
         self.force_reload = force_reload
         self.run_mode = run_mode
 
         if not dataset_dirs:
             dataset_dirs = get_directory_paths_for_run_mode(run_mode=self.run_mode)
 
         self.dataset_dirs = dataset_dirs
         for k, val in self.dataset_dirs.items():
             if isinstance(val, Path):
                 setattr(self, k, val)
-                # if val.is_dir() or val.is_file():
 
         self.raman_files = self.find_files(data_dir=self.DATASET_DIR)
         self.index = pd.DataFrame()
         self._error_parse_filenames = []
         if "normal" in run_mode and not self.debug and not self.force_reload:
             self.index = self.load_index()
 
@@ -84,15 +59,15 @@
     @staticmethod
     def find_files(data_dir: Path = Path()) -> List:
         """
         Creates a list of all raman type files found in the DATASET_DIR which are used in the creation of the index.
         """
 
         if not isinstance(data_dir, Path):
-            logger.warning(f"find_files warning: arg is not Path.")
+            logger.warning("find_files warning: arg is not Path.")
             return []
 
         raman_files_raw = []
         if data_dir.exists():
             RFs = data_dir.rglob("*txt")
             if RFs:
                 raman_files_raw = [
@@ -161,27 +136,24 @@
                 self.INDEX_FILE.parent.mkdir(exist_ok=True, parents=True)
 
             index.to_csv(self.INDEX_FILE)
 
             _dtypes = index.dtypes.to_frame("dtypes")
             _dtypes.to_csv(self._dtypes_filepath())
 
-            # self.save_merge_to_db(DB_filepath, index, self.table_name)
-
             logger.info(
                 f"{self._cqnm} Succesfully Exported Raman Index file to:\n\t{self.INDEX_FILE}\nwith len({len(index)})."
             )
         else:
             logger.info(f"{self._cqnm} Empty index not exported")
 
     def load_index(self):
         """loads the index from from defined Index file"""
         if self.INDEX_FILE.exists():
             try:
-
                 _dtypes = pd.read_csv(self._dtypes_filepath(), index_col=[0]).to_dict()[
                     "dtypes"
                 ]
 
                 _dtypes_datetime = {
                     k: val
                     for k, val in _dtypes.items()
@@ -284,15 +256,14 @@
             default_selection = "all"
         index_selection = pd.DataFrame()
         logger.info(
             f"{self._cqnm} starting index selection from index({len(index)}) with:\n default selection: {default_selection}\n and {kwargs}"
         )
 
         if not index.empty:
-
             if default_selection:
                 if default_selection == "all":
                     index_selection = index.copy()
 
             if "samplegroups" in _keys:
                 if _kws["samplegroups"]:
                     index_selection = index.loc[
@@ -356,9 +327,8 @@
 
     except Exception as e:
         logger.error(f"Raman Index error: {e}")
     return RamanIndex
 
 
 if __name__ == "__main__":
-    # print(getattr(__file__, 'testdt'))
     RamanIndex = main()
```

### Comparing `raman_fitting-0.6.18/src/raman_fitting/interfaces/cli.py` & `raman_fitting-0.7.0/src/raman_fitting/interfaces/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import argparse
-import pathlib
-import importlib.metadata
 
 
-# def _testing():
-#     args = parser.parse_args(['-M', 'debug'])
 RUN_MODES = ["normal", "testing", "debug", "make_index", "make_examples"]
 
 try:
+    import importlib.metadata
+
     _version = importlib.metadata.version("raman_fitting")
-except Exception as e:
+except ImportError:
     _version = "version.not.found"
 
 _version_text = f"\n=== CLI raman_fitting version: {_version} ===\n"
-# print(_version_text)
 
 
 def main():
-
     """
     The command line interface for raman_fitting
     """
 
     parser = argparse.ArgumentParser(
         description="Command-line interface for raman_fitting package main."
     )
```

### Comparing `raman_fitting-0.6.18/src/raman_fitting/processing/cleaner.py` & `raman_fitting-0.7.0/src/raman_fitting/processing/cleaner.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 from raman_fitting.processing.spectrum_template import (
     SpecTemplate,
     SpectrumWindowLimits,
     SpectrumWindows,
 )
 
+
 class SpectrumMethodException(ValueError):
     pass
 
 
 class SpectrumMethods:
     """
     Parent class to hold several Spetrum Methods as children
@@ -46,15 +47,14 @@
         self.ramanshift = ramanshift
         self.intensity = intensity
         self.label = label
         self.kwargs = kwargs
 
     @staticmethod
     def filtered_int(intensity=None):
-
         try:
             int_savgol_fltr = signal.savgol_filter(intensity, 13, 3, mode="nearest")
         except Exception as e:
             raise SpectrumMethodException(f"no intensity given to filter, {e}")
             int_savgol_fltr = []
         return int_savgol_fltr
 
@@ -152,15 +152,14 @@
             "norm_int": normalization_intensity,
         }
         self.norm_dict = norm_dict
 
     def set_normalized_data(self):
         _normd = {}
         for windowname, spec in self.blcorr_data.items():
-
             label = f"norm_blcorr_{windowname}"
             if self.label:
                 label = f"{self.label}_{label}"
 
             _data = self.data(spec.ramanshift, spec.intensity * self.norm_factor, label)
             _normd.update(**{windowname: _data})
         self.norm_data = _normd
@@ -246,24 +245,22 @@
 
     @property
     def despiked_intensity(self):
         return self._despiked_intensity
 
     @despiked_intensity.setter
     def despiked_intensity(self, value):
-
         result = self.run_despike_steps(value, self.Z_threshold)
 
         self._despiked_intensity = result["despiked_intensity"]
 
         self.result = result
         self.df = pd.DataFrame(result)
 
     def run_despike_steps(self, intensity, Z_threshold):
-
         Z_t = self.calc_Z(intensity)
         Z_t_filtered = self.calc_Z_filtered(Z_t, Z_threshold)
         i_despiked = self.despike_filter(
             intensity, Z_t_filtered, self.moving_window_size
         )
 
         result_values = [intensity, Z_t, Z_t_filtered, i_despiked]
@@ -299,15 +296,14 @@
     def despike_filter(
         intensity, Z_t_filtered, moving_window_size, ignore_lims=(20, 46)
     ):
         n = len(intensity)
         i_despiked = copy.deepcopy(intensity)
         spikes = np.where(np.isnan(Z_t_filtered))
         for i in list(spikes[0]):
-
             if i < ignore_lims[0] or i > ignore_lims[1]:
                 w = np.arange(
                     max(0, i - moving_window_size), min(n, i + moving_window_size)
                 )
                 w = w[~np.isnan(Z_t_filtered[w])]
                 if intensity[w].any():
                     i_despiked[i] = np.mean(intensity[w])
```

### Comparing `raman_fitting-0.6.18/src/raman_fitting/processing/spectrum_constructor.py` & `raman_fitting-0.7.0/src/raman_fitting/processing/spectrum_constructor.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,23 +32,23 @@
 @dataclass(order=True, frozen=False)
 class SpectrumDataLoader:
     """
     Raman Spectrum Loader Dataclass, reads in the file and constructs a clean spectrum from the data.
     A sequence of steps is performed on the raw data from SpectrumReader.
     The steps/methods are: smoothening filter, despiking and baseline correction.
     """
+
     _fields = ("ramanshift", "intensity")
     file: Path = field(default=Path(Path.cwd().joinpath("empty.txt")))
     spectrum_length: int = field(default=0, init=False)
     info: Dict = field(default_factory=dict, repr=False)
     ovv: pd.DataFrame = field(default_factory=pd.DataFrame, repr=False)
     run_kwargs: Dict = field(default_factory=dict, repr=False)
 
     def __post_init__(self):
-
         self._qcnm = self.__class__.__qualname__
 
         self.register = {}  # this stores the data of each method as they are performed
         self.filtered_intensity = None
         self._despike = None
         self._baseline_corrected = None
         self.clean_data = None
@@ -123,15 +123,14 @@
         self._baseline_corrected = _baseline_corrected
 
         _fullspec = _baseline_corrected.norm_data["full"]
         self.register_spectrum(_fullspec.ramanshift, _fullspec.intensity, out_lbl)
         self.clean_data = _baseline_corrected.norm_data
 
     def set_clean_data_df(self):
-
         self.clean_df = {
             k: pd.DataFrame(
                 {"ramanshift": val.ramanshift, f"int_{self.SamplePos}": val.intensity}
             )
             for k, val in self.clean_data.items()
         }
 
@@ -249,15 +248,14 @@
 
     def calc_mean(self):
         """Core function of the merging of spectra of different sample positions"""
         _merged_window_specs = {}
         _speclst = []
         _posmean_lbl_base = f'int_{self.info.get("SampleID")}_mean'
         for wndwnm, data in self.prep_clean_data.items():
-
             _merge_df = pd.DataFrame()
             _pos_lbl_lst = []
 
             for _pos, _sp in data:
                 _pos_lbl = f"int_{_pos}"
 
                 _dfspec = pd.DataFrame(
```

### Comparing `raman_fitting-0.6.18/src/raman_fitting/processing/spectrum_template.py` & `raman_fitting-0.7.0/src/raman_fitting/processing/spectrum_template.py`

 * *Files identical despite different names*

### Comparing `raman_fitting-0.6.18/src/raman_fitting/utils/coordinators.py` & `raman_fitting-0.7.0/src/raman_fitting/utils/coordinators.py`

 * *Files identical despite different names*

### Comparing `raman_fitting-0.6.18/src/raman_fitting/utils/file_reader.py` & `raman_fitting-0.7.0/src/raman_fitting/utils/file_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 
     def read_in(self):
         ramanshift, intensity_raw = np.array([]), np.array([])
         i = 0
         while not ramanshift.any():
             try:
                 ramanshift, intensity_raw = np.loadtxt(
-                    self._filepath, usecols=(0, 1), unpack=True, skiprows=i
+                    self._file_path, usecols=(0, 1), unpack=True, skiprows=i
                 )
-                print(self._filepath, len(ramanshift), len(intensity_raw))
+                print(self._file_path, len(ramanshift), len(intensity_raw))
                 self._skiprows = i
                 self._read_succes = True
             except ValueError:
                 i += 1
 
         self.ramanshift = ramanshift
         self.intensity_raw = intensity_raw
```

### Comparing `raman_fitting-0.6.18/tests/deconvolution_models/test_base_model.py` & `raman_fitting-0.7.0/tests/deconvolution_models/test_base_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 import unittest
 from functools import partial
 
 import pytest
 from lmfit import Model
 
-import raman_fitting
 from raman_fitting.deconvolution_models.base_model import _SUBSTRATE_PEAK, BaseModel
 
 _SUBSTRATE_PREFIX = _SUBSTRATE_PEAK.split("peak")[0]
 
 
 def _get_list_components(bm):
     _listcompsprefix = partial(map, lambda x,: getattr(x, "prefix"))
```

### Comparing `raman_fitting-0.6.18/tests/deconvolution_models/test_base_peaks.py` & `raman_fitting-0.7.0/tests/deconvolution_models/test_base_peaks.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 import logging
 import unittest
 
 import pytest
 from lmfit import Model
 
 # from raman_fitting.deconvolution_models import first_order_peaks
-import raman_fitting
+# import raman_fitting
 from raman_fitting.deconvolution_models.default_peaks.base_peak import (
     BasePeak,
     BasePeakWarning,
     LMfitModelConstructorMethods,
 )
 
 logger = logging.getLogger(__name__)
 logging.captureWarnings(True)  # sends these warning to the logger
 
 
-#%%
+# %%
 
 
 def _error_message_contains(excinfo, testmsg: str, verbose: bool = False):
     _fltr_str = [
         i if not i in ["(", ")"] else " "
         for i in str(excinfo.value)
         if i.isalnum() or i in (",", ".", " ", "_", "(", ")")
@@ -35,29 +35,28 @@
 
     if not _test or verbose:
         print(list(((i, i in _cl_str_split) for i in testmsg.split(" "))))
         print(_cl_str_split)
     return _test
 
 
-#%%
+# %%
 
 
 class TestBasePeak(unittest.TestCase):
-
-    #%% TESTING
+    # %% TESTING
 
     def test_BasePeak_attributes(self):
         self.assertTrue(BasePeak.__doc__)
         self.assertTrue(BasePeak._fields)
         self.assertTrue(BasePeak._sources)
         self.assertTrue(BasePeak.PEAK_TYPE_OPTIONS)
 
     def test_empty_base_class_raises(self):
-        #%%
+        # %%
 
         class EmptyTestChild(metaclass=BasePeak):
             pass
 
         eb = EmptyTestChild()
 
         with pytest.raises(ValueError) as excinfo:
@@ -66,30 +65,30 @@
 
         with pytest.raises(ValueError) as excinfo:
             eb.peak_name = 10 * "emptytest"
         assert _error_message_contains(excinfo, "value for peak_name is too long 90")
 
         self.assertFalse(eb.peak_model)
 
-        #%%
+        # %%
 
     def test_empty_base_class_with_kwargs_raises(self):
-        #%%
+        # %%
 
         class EmptyTestChild(
             metaclass=BasePeak,
             testkwarg2=2,
             testkwarg3=3,
             peak_type="Voigt",
             verbose=True,
         ):
             pass
 
         eb = EmptyTestChild()
-        #%%
+        # %%
 
         self.assertEqual(eb.peak_type, "Voigt")
         self.assertEqual(eb.testkwarg2, 2)
 
         with pytest.raises(ValueError) as excinfo:
             eb.peak_type = "emptytest"
         self.assertTrue(
@@ -117,28 +116,28 @@
             _error_message_contains(
                 excinfo,
                 ''''Multiple options ['Lorentzian', 'Voigt'] for misspelled value "VoigtLorentzian"''',
             )
         )
 
     def test_empty_base_class_with_false_input(self):
-        #%%
+        # %%
 
         class EmptyTestChild(metaclass=BasePeak, peak_type="FalsePeak"):
             pass
 
         with pytest.raises(ValueError) as excinfo:
             eb = EmptyTestChild()
         self.assertTrue(
             _error_message_contains(excinfo, "value emptytest for peak_type not in")
         )
 
-    #%%
+    # %%
     def test_base_class_good_with_init_extra_tests(self):
-        #%%
+        # %%
         class TestD1peak(metaclass=BasePeak, debug=True):
             """
             here is docstring of TestD1peak,
             small spelling error on peak_type
             """
 
             def __init__(self, *args, **kwargs):
@@ -184,15 +183,15 @@
         #     _def_param = td1.param_hints_constructor(_err_hints)
         # self.assertTrue(
         #     _error_message_contains(
         #         excinfo, " Unable to create a Parameter from center and (1, 2, 3, 4):"
         #     )
         # )
 
-    #%%
+    # %%
     def test_base_class_good_with_init(self):
         class TestD1peak(metaclass=BasePeak, debug=True):
             """
             test_base_class_good_with_init
             but with spelling error in peak_type
             """
 
@@ -207,18 +206,18 @@
                 }
 
         td1 = TestD1peak()
         _class_str = "TestD1peak, <lmfit.Model: Model(voigt, prefix='D1D1_')>, center : 2600 < 2650 > 2750"
         self.assertIn(_class_str, str(td1))
         # print(td1)
 
-    #%%
+    # %%
 
     def test_base_class_good_with_init_added_method(self):
-        #%%
+        # %%
         class TestD1peakmeta(metaclass=BasePeak, a=2):
             """
             here is docstring of TestD1peak
             """
 
             def __init__(self, *args, **kwargs):
                 # super().__init__(self)
@@ -240,18 +239,18 @@
                 # return arg
 
         td1m = TestD1peakmeta(add=33)
         _teststr = "TestD1peakmeta, <lmfit.Model: Model(lorentzian, prefix='D1D1_')>, center : 2600 < 2650 > 2750"
         self.assertIn(_teststr, str(td1m))
         # assert str(td1m) == _teststr
 
-        #%%
+        # %%
 
     def test_base_class_good_with_attributes_and_init(self):
-        #%%
+        # %%
         class NewChildClassAttr(metaclass=BasePeak):
             """New child class for easier definition"""
 
             _test = "testkwarg"
 
             param_hints = {
                 "center": {"value": 2435, "min": 2400, "max": 2550},
@@ -266,15 +265,15 @@
                 pass
                 # super().__init__()
 
         nca = NewChildClassAttr()
         _center_value = nca.peak_model.param_hints["center"]["value"]
         assert _center_value == 2435
         # print('Instance child:', nca)
-        #%%
+        # %%
 
     def test_base_class_good_with_attributes_no_init(self):
         class NewChildClassAttrNoInit(metaclass=BasePeak):
             """New child class for easier definition"""
 
             _test = "testkwarg"
 
@@ -290,18 +289,18 @@
             # pass
             # super().__init__()
 
         ncni = NewChildClassAttrNoInit()
         _center_value = ncni.peak_model.param_hints["center"]["value"]
         assert _center_value == 2435
 
-        #%%
+        # %%
 
     def test_base_class_good_with_attributes_init_collision_values(self):
-        #%%
+        # %%
         class NewChildClassInit(metaclass=BasePeak, peak_type="Gaussian"):
             """New child class for easier definition"""
 
             _test = "testkwarg"
             peak_type = "Lorentzian"
             param_hints = {
                 "center": {"value": 2435, "min": 2400, "max": 2550},
@@ -335,19 +334,17 @@
         new.param_hints = {"center": {"value": 200}}
         newinst = new()
         _newinst_str = "newPeak, <lmfit.Model: Model(voigt, prefix='newPeak_')>, center : -inf < 200 > inf"
         self.assertEqual(str(newinst), _newinst_str)
 
 
 class TestLMfitModelConstructorMethods(unittest.TestCase):
-
     LMfit = LMfitModelConstructorMethods
 
     def test_make_model_from_peak_type_and_name(self):
-
         model = self.LMfit.make_model_from_peak_type_and_name(
             peak_type="Voigt", peak_name="lmfitpeak"
         )
         self.assertTrue(isinstance(model, Model))
         self.assertEqual(model.prefix, "lmfitpeak")
 
         with pytest.raises(NotImplementedError) as excinfo:
@@ -359,11 +356,11 @@
             )
         )
 
 
 # self = TestLMfitModelConstructorMethods()
 
 
-#%%
+# %%
 if __name__ == "__main__":
     unittest.main()
     self = TestBasePeak()
```

### Comparing `raman_fitting-0.6.18/tests/deconvolution_models/test_fit_models.py` & `raman_fitting-0.7.0/tests/deconvolution_models/test_fit_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,14 +36,13 @@
     def test_empty_PrepareParams(self):
         # pp =
         with self.assertRaises(AttributeError):
             PrepareParams({})
 
 
 def _testing():
-
     self = ft
     self = prep
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `raman_fitting-0.6.18/tests/deconvolution_models/test_peak_validation.py` & `raman_fitting-0.7.0/tests/deconvolution_models/test_peak_validation.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,57 +27,52 @@
         with self.assertWarns(NotFoundAnyModelsWarning):
             self.pmv.get_subclasses_from_base("")
 
         with self.assertWarns(NotFoundAnyModelsWarning):
             self.pmv.get_subclasses_from_base(str)
 
     def test_validation_inspect_models(self):
-
         _valid = self.pmv.validation_inspect_models([str])
         self.assertTrue(_valid)
         self.assertFalse(_valid[1][0].valid)
         self.assertIn("has no attr", _valid[1][0].message)
 
         _valid = self.pmv.validation_inspect_models([Model])
         self.assertTrue(_valid)
         self.assertFalse(_valid[1][0].valid)
         self.assertIn("Unable to initialize model", _valid[1][0].message)
 
     def test_get_cmap_list(self):
-
         _cmap = self.pmv.get_cmap_list([], cmap_options=())
         self.assertEqual(_cmap, [])
         _cmap = self.pmv.get_cmap_list(
             [1] * 50, cmap_options=(), fallback_color=self.pmv.fallback_color
         )
         self.assertEqual(_cmap, [self.pmv.fallback_color] * 50)
         _cmap = self.pmv.get_cmap_list([1] * 5)
         self.assertEqual(len(_cmap), 5)
 
     def test___getattr__(self):
-
         with self.assertRaises(AttributeError):
             self.pmv.fake_attr
 
     def test___iter__(self):
         _iter = [i for i in self.pmv]
         self.assertIsInstance(_iter, list)
 
     def test_if_lmfit_models(self):
-
         if self.pmv.lmfit_models:
             _getdict = self.pmv.get_dict()
             self.assertIsInstance(_getdict, dict)
 
             _getdict = self.pmv.get_model_dict(self.pmv.lmfit_models)
             self.assertIsInstance(_getdict, dict)
 
 
 def _debugging():
-
     self = TestPeakModelValidator()
     peaks = PeakModelValidator()
     self.pmv = peaks
     # all([isinstance(i.peak_model, Model) for i in peaks.lmfit_models])
     # all([isinstance(i.peak_model, Model) for i in peaks.get_dict().values()])
```

### Comparing `raman_fitting-0.6.18/tests/delegating/test_main_delegator.py` & `raman_fitting-0.7.0/tests/delegating/test_main_delegator.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,14 @@
         _sample_group = self.maindebug.sample_group_gen()
         _arg = next(_sample_group)
         _destdirs = add_make_sample_group_destdirs(_arg[-1])
         _alltest = all([_arg[0] in a for a in [i.parts for i in _destdirs.values()]])
         self.assertTrue(_alltest)
 
     def test_generator(self):
-
         _sample_group = self.maindebug.sample_group_gen()
         _sample_group_arg = next(_sample_group)
         self.assertTrue(_sample_group_arg)
 
         _sID_gen = self.maindebug._sID_gen(*_sample_group_arg)
         _sID_arg = next(_sID_gen)
         self.assertTrue(_sID_arg)
```

### Comparing `raman_fitting-0.6.18/tests/indexing/test_filename_parser.py` & `raman_fitting-0.7.0/tests/indexing/test_filename_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 
 from raman_fitting.indexing.filename_parser_helpers import filestem_to_sid_and_pos
 
 # import pytest
 
 
 class TestFilenameParser(unittest.TestCase):
-
     example_parse_expected = {
         "errEMP2_1.txt": ("errEMP2", 1),
         "errTS2_pos1.txt": ("errTS2", 1),
         "Si_spectrum01.txt": ("Si", 1),
         "testDW38C_pos1.txt": ("testDW38C", 1),
         "testDW38C_pos2.txt": ("testDW38C", 2),
         "testDW38C_pos3.txt": ("testDW38C", 3),
@@ -60,15 +59,14 @@
         self.assertTrue(all(hasattr(i, self.result_attr) for i in self.data_PPs))
 
     def test_PathParser_empty(self):
         self.assertTrue(hasattr(self.empty_PP, "_flavour"))
         self.assertTrue(hasattr(self.empty_PP, self.result_attr))
 
     def test_PP_extra_from_map(self):
-
         for k, val in _extra_sID_name_mapper.items():
             _mapval = _extra_overwrite_sID_from_mapper(k)
 
             self.assertEqual(_mapval, val)
 
     def test_PP_extra_from_parts(self):
         self.assertEqual("TEST", _extra_overwrite_sgrpID_from_parts([], "TEST"))
@@ -77,15 +75,14 @@
             emptymap_PP = PathParser(f"{k}/TEST.txt")
             self.assertEqual(
                 val,
                 _extra_overwrite_sgrpID_from_parts(emptymap_PP.parts, "TEST"),
             )
 
     def test_PP_parse_filepath_to_sid_and_pos(self):
-
         for file, _expected in self.example_parse_expected.items():
             self.assertEqual(filestem_to_sid_and_pos(file), _expected)
 
     # def test_PathParser(self):
     #     _dfpath = Path(__file__).parent.parent.parent / 'src' / 'raman_fitting' / 'datafiles'
     #     _fls = list(_dfpath.rglob('*.txt'))
     #     _res = []
```

### Comparing `raman_fitting-0.6.18/tests/indexing/test_indexer.py` & `raman_fitting-0.7.0/tests/indexing/test_indexer.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,24 +10,22 @@
 import raman_fitting
 from raman_fitting.datafiles import example_files
 from raman_fitting.indexing.indexer import MakeRamanFilesIndex
 
 
 class TestIndexer(unittest.TestCase):
     def setUp(self):
-
         _example_path = Path(example_files.__path__[0])
         _example_files_contents = list(Path(_example_path).rglob("*txt"))
 
         self._example_files = [i for i in _example_files_contents]
 
         self.RamanIndex = MakeRamanFilesIndex(run_mode="make_examples")
 
     def test_MakeRamanFilesIndex_make_examples(self):
-
         self.assertEqual(len(self.RamanIndex), len(self._example_files))
 
     def test_load_index(self):
         _loaded_index = self.RamanIndex.load_index()
         self.assertTrue(isinstance(_loaded_index, pd.DataFrame))
 
         for col in _loaded_index.columns:
```

### Comparing `raman_fitting-0.6.18/tests/processing/test_cleaner.py` & `raman_fitting-0.7.0/tests/processing/test_cleaner.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,26 +6,24 @@
 
 from raman_fitting.datafiles import example_files
 from raman_fitting.processing.cleaner import Despiker
 
 
 class TestDespiker(unittest.TestCase):
     def test_Despiker(self):
-
         desp = Despiker(np.array([1, 2, 3, 4, 5]))
         self.assertEqual(len(desp.df), 5)
 
         desp = Despiker(np.array([1, 2, 3, 4, 5, 6, 7, 8, 9, 10]))
         self.assertEqual(len(desp.df), 10)
 
         desp = Despiker(np.array([2, 2, 2, 2, 2, 2, 30, 20, 2, 2, 2, 2, 2, 2]))
 
 
 def _debugging():
-
     self = TestDespiker()
     desp = Despiker(np.array([2, 2, 2, 2, 2, 2, 30, 20, 2, 2, 2, 2, 2, 2]))
     desp.plot_Z()
     intensity = desp.result["input_intensity"]
     Z_t_filtered = desp.result["Z_t_filtered"]
     moving_window_size = desp.moving_window_size
     Z_threshold = desp.Z_threshold
```

### Comparing `raman_fitting-0.6.18/tests/processing/test_spectrum_constructor.py` & `raman_fitting-0.7.0/tests/processing/test_spectrum_constructor.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,14 @@
             filter(lambda x: "testDW38C_pos4" in x.name, _example_files_contents)
         )
         self.errorfile = next(
             filter(lambda x: "wrong" in x.name, _example_files_contents)
         )
 
     def test_SpectrumDataLoader_empty(self):
-
         spd = SpectrumDataLoader()
         self.assertEqual(spd.file.name, "empty.txt")
 
     def test_SpectrumDataLoader_file(self):
         pass
         spd = SpectrumDataLoader(
             self.testfile, run_kwargs=dict(SampleID="testfile", SamplePos=1)
```

### Comparing `raman_fitting-0.6.18/tests/utils/test_coordinators.py` & `raman_fitting-0.7.0/tests/utils/test_coordinators.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 import unittest
 import warnings
 
+import raman_fitting
 from raman_fitting.utils.coordinators import FieldsTracker, FieldsTrackerWarning
 
 logger = logging.getLogger(__name__)
 logging.captureWarnings(True)  # sends these warning to the logger
 
 
 def ignore_warnings(test_func):
@@ -16,16 +17,15 @@
 
     return do_test
 
 
 class TestFieldsTracker(unittest.TestCase):
     @ignore_warnings
     def testFCO(self):
-
-        #%%
+        # %%
         fco = FieldsTracker(
             fields=["peak_name", "peak_type", "param_hints"],
             sources=("kwargs", "cls_dict", "init"),
         )
         assert not fco.results
         assert fco.status == False
```

### Comparing `raman_fitting-0.6.18/todos.md` & `raman_fitting-0.7.0/todos.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 # IDEA add docs with Sphinx, readthedocs
 # IDEA improve AsyncIO into main delegator processes
 # IDEA fix plotting because of DeprecationWarning in savefig
 # IDEA add database for spectrum data storage
 # IDEA future GUI webinterface
 
 # IDEA improve fitting loop so that starting parameters from modelX and modelX+Si are shared, faster...
-```
+```
```

