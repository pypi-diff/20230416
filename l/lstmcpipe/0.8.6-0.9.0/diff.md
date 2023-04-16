# Comparing `tmp/lstmcpipe-0.8.6.tar.gz` & `tmp/lstmcpipe-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lstmcpipe-0.8.6.tar", last modified: Wed Jul 13 11:21:02 2022, max compression
+gzip compressed data, was "lstmcpipe-0.9.0.tar", last modified: Mon Oct 10 08:57:13 2022, max compression
```

## Comparing `lstmcpipe-0.8.6.tar` & `lstmcpipe-0.9.0.tar`

### file list

```diff
@@ -1,219 +1,223 @@
-drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-07-13 11:21:02.047926 lstmcpipe-0.8.6/
-drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-07-13 11:21:01.959775 lstmcpipe-0.8.6/.github/
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)      630 2022-04-01 16:15:10.000000 lstmcpipe-0.8.6/.github/pull_request_template.md
-drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-07-13 11:21:01.961983 lstmcpipe-0.8.6/.github/workflows/
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     2293 2022-06-23 07:20:36.000000 lstmcpipe-0.8.6/.github/workflows/CI.yml
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)      786 2022-06-01 16:34:15.000000 lstmcpipe-0.8.6/.github/workflows/codemeta2citation.yml
-drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-07-13 11:21:01.962468 lstmcpipe-0.8.6/.github/workflows/dev/
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     1047 2022-05-19 20:14:47.000000 lstmcpipe-0.8.6/.github/workflows/dev/codemeta2citation.py
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)      868 2022-05-06 08:55:35.000000 lstmcpipe-0.8.6/.github/workflows/docs.yml
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)      403 2022-05-19 20:14:47.000000 lstmcpipe-0.8.6/.github/workflows/pypi.yml
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)      232 2022-05-06 08:55:46.000000 lstmcpipe-0.8.6/.gitignore
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)      676 2022-05-12 06:59:42.000000 lstmcpipe-0.8.6/.pre-commit-config.yaml
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)    18219 2022-04-01 16:15:10.000000 lstmcpipe-0.8.6/.pylintrc
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)      555 2022-05-19 20:14:47.000000 lstmcpipe-0.8.6/CITATION.cff
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)      595 2022-07-13 11:21:02.047398 lstmcpipe-0.8.6/PKG-INFO
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)    13312 2022-06-01 16:34:15.000000 lstmcpipe-0.8.6/README.rst
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     2803 2022-06-01 16:34:15.000000 lstmcpipe-0.8.6/codemeta.json
-drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-07-13 11:21:01.967461 lstmcpipe-0.8.6/docs/
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)      752 2022-04-13 17:39:20.000000 lstmcpipe-0.8.6/docs/Makefile
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     2455 2022-07-04 15:24:42.000000 lstmcpipe-0.8.6/docs/conf.py
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)      475 2022-04-19 12:26:15.000000 lstmcpipe-0.8.6/docs/index.rst
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)      800 2021-12-16 12:11:58.000000 lstmcpipe-0.8.6/docs/make.bat
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     5448 2022-05-20 09:49:47.000000 lstmcpipe-0.8.6/docs/pipeline.rst
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     2121 2022-06-01 16:34:15.000000 lstmcpipe-0.8.6/docs/produce_config_page.py
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)      335 2022-05-24 15:01:00.000000 lstmcpipe-0.8.6/docs/productions.rst
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)      131 2022-04-19 12:26:15.000000 lstmcpipe-0.8.6/docs/requirements.txt
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)      309 2022-06-01 16:34:15.000000 lstmcpipe-0.8.6/environment.yml
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     1079 2022-01-18 22:35:07.000000 lstmcpipe-0.8.6/license.rst
-drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-07-13 11:21:01.970665 lstmcpipe-0.8.6/lstmcpipe/
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)      323 2022-05-12 06:59:42.000000 lstmcpipe-0.8.6/lstmcpipe/__init__.py
-drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-07-13 11:21:01.973828 lstmcpipe-0.8.6/lstmcpipe/_dev_version/
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)      397 2022-05-12 06:59:42.000000 lstmcpipe-0.8.6/lstmcpipe/_dev_version/_dev_version.py
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)       21 2022-07-13 11:21:00.000000 lstmcpipe-0.8.6/lstmcpipe/_version.py
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)      843 2022-05-17 21:37:00.000000 lstmcpipe-0.8.6/lstmcpipe/base_config_lstmcpipe.yaml
-drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-07-13 11:21:01.974852 lstmcpipe-0.8.6/lstmcpipe/benchmarks/
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)        0 2022-03-10 14:15:21.000000 lstmcpipe-0.8.6/lstmcpipe/benchmarks/__init__.py
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     2542 2022-05-12 06:59:42.000000 lstmcpipe-0.8.6/lstmcpipe/benchmarks/irfs.py
-drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-07-13 11:21:01.977720 lstmcpipe-0.8.6/lstmcpipe/config/
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)      680 2022-04-20 13:44:05.000000 lstmcpipe-0.8.6/lstmcpipe/config/__init__.py
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     2120 2022-05-12 06:59:42.000000 lstmcpipe-0.8.6/lstmcpipe/config/dl1ab_tuning.py
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)    37472 2022-06-30 13:35:25.000000 lstmcpipe-0.8.6/lstmcpipe/config/paths_config.py
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     5730 2022-05-24 15:44:30.000000 lstmcpipe-0.8.6/lstmcpipe/config/pipeline_config.py
-drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-07-13 11:21:01.979324 lstmcpipe-0.8.6/lstmcpipe/config/tests/
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)        0 2021-12-14 22:30:35.000000 lstmcpipe-0.8.6/lstmcpipe/config/tests/__init__.py
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     5469 2022-05-17 21:37:00.000000 lstmcpipe-0.8.6/lstmcpipe/config/tests/test_paths_config.py
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     2925 2022-05-17 21:37:00.000000 lstmcpipe-0.8.6/lstmcpipe/config/tests/test_pipeline_config.py
-drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-07-13 11:21:01.980946 lstmcpipe-0.8.6/lstmcpipe/hiperta/
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)        0 2021-12-14 22:30:35.000000 lstmcpipe-0.8.6/lstmcpipe/hiperta/__init__.py
--rwxr-xr-x   0 thomasvuillaume   (502) staff       (20)     2376 2022-05-12 06:59:42.000000 lstmcpipe-0.8.6/lstmcpipe/hiperta/hiperta_r0_to_dl1lstchain.py
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)    10993 2022-05-31 12:09:03.000000 lstmcpipe-0.8.6/lstmcpipe/hiperta/reorganize_dl1hiperta300_to_dl1lstchain060.py
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)    15690 2022-05-31 12:09:03.000000 lstmcpipe-0.8.6/lstmcpipe/hiperta/reorganize_dl1hiperta_to_dl1lstchain.py
-drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-07-13 11:21:01.981990 lstmcpipe-0.8.6/lstmcpipe/io/
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)        0 2021-12-14 22:30:35.000000 lstmcpipe-0.8.6/lstmcpipe/io/__init__.py
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     4420 2022-05-17 21:37:00.000000 lstmcpipe-0.8.6/lstmcpipe/io/data_management.py
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     3219 2022-05-31 12:09:03.000000 lstmcpipe-0.8.6/lstmcpipe/io/lstmcpipe_tree_path.py
-drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-07-13 11:21:01.983209 lstmcpipe-0.8.6/lstmcpipe/io/tests/
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)        0 2022-04-13 17:39:20.000000 lstmcpipe-0.8.6/lstmcpipe/io/tests/__init__.py
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     1232 2022-05-12 06:59:42.000000 lstmcpipe-0.8.6/lstmcpipe/io/tests/test_data_management.py
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     1735 2022-05-12 06:59:42.000000 lstmcpipe-0.8.6/lstmcpipe/io/tests/test_lstmcpipe_tree_path.py
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     1892 2022-05-19 20:14:47.000000 lstmcpipe-0.8.6/lstmcpipe/logging.py
--rwxr-xr-x   0 thomasvuillaume   (502) staff       (20)     9949 2022-07-13 11:20:55.000000 lstmcpipe-0.8.6/lstmcpipe/lstmcpipe_start.py
-drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-07-13 11:21:01.984853 lstmcpipe-0.8.6/lstmcpipe/metrics/
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)    14058 2022-07-12 15:23:11.000000 lstmcpipe-0.8.6/lstmcpipe/metrics/__init__.py
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)        0 2022-07-08 12:52:12.000000 lstmcpipe-0.8.6/lstmcpipe/metrics/angular_resolution.py
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)        0 2022-07-08 12:52:44.000000 lstmcpipe-0.8.6/lstmcpipe/metrics/class.py
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)        0 2022-07-08 12:52:39.000000 lstmcpipe-0.8.6/lstmcpipe/metrics/direction.py
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)        0 2022-07-08 12:52:30.000000 lstmcpipe-0.8.6/lstmcpipe/metrics/energy.py
-drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-07-13 11:21:01.986469 lstmcpipe-0.8.6/lstmcpipe/plots/
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)        0 2021-12-14 22:30:35.000000 lstmcpipe-0.8.6/lstmcpipe/plots/__init__.py
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     3221 2022-05-31 12:09:03.000000 lstmcpipe-0.8.6/lstmcpipe/plots/images_debug.py
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)    13340 2022-07-13 11:20:55.000000 lstmcpipe-0.8.6/lstmcpipe/plots/plot_irfs.py
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)      728 2022-05-12 06:59:42.000000 lstmcpipe-0.8.6/lstmcpipe/plots/plot_models_importance.py
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     2574 2022-06-24 13:17:16.000000 lstmcpipe-0.8.6/lstmcpipe/plots/pointings.py
-drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-07-13 11:21:01.987096 lstmcpipe-0.8.6/lstmcpipe/plots/tests/
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)      365 2022-05-19 20:14:40.000000 lstmcpipe-0.8.6/lstmcpipe/plots/tests/test_pointings.py
-drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-07-13 11:21:01.993299 lstmcpipe-0.8.6/lstmcpipe/scripts/
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)        0 2021-12-14 22:30:35.000000 lstmcpipe-0.8.6/lstmcpipe/scripts/__init__.py
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     6700 2022-05-17 21:37:00.000000 lstmcpipe-0.8.6/lstmcpipe/scripts/generate_test_lapalma.py
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     3595 2022-06-01 16:34:15.000000 lstmcpipe-0.8.6/lstmcpipe/scripts/lstmcpipe_generate_config.py
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     1766 2022-05-31 12:09:03.000000 lstmcpipe-0.8.6/lstmcpipe/scripts/script_batch_filelist_cta.py
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     1913 2022-05-20 10:03:09.000000 lstmcpipe-0.8.6/lstmcpipe/scripts/script_batch_filelist_lst.py
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     2105 2022-05-20 10:03:09.000000 lstmcpipe-0.8.6/lstmcpipe/scripts/script_batch_filelist_lst_dl1ab.py
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     2179 2022-05-20 10:03:09.000000 lstmcpipe-0.8.6/lstmcpipe/scripts/script_batch_filelist_rta.py
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     2346 2022-07-13 11:20:55.000000 lstmcpipe-0.8.6/lstmcpipe/scripts/script_compare_irfs.py
--rwxr-xr-x   0 thomasvuillaume   (502) staff       (20)    12483 2022-05-12 06:59:42.000000 lstmcpipe-0.8.6/lstmcpipe/scripts/script_dl2_to_sensitivity.py
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     2068 2022-06-01 16:34:15.000000 lstmcpipe-0.8.6/lstmcpipe/scripts/script_lstmcpipe_validate_config.py
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     2281 2022-05-12 06:59:42.000000 lstmcpipe-0.8.6/lstmcpipe/scripts/script_train_test_splitting.py
-drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-07-13 11:21:01.994981 lstmcpipe-0.8.6/lstmcpipe/scripts/tests/
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)        0 2021-12-14 22:30:22.000000 lstmcpipe-0.8.6/lstmcpipe/scripts/tests/__init__.py
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)        0 2022-04-20 13:44:05.000000 lstmcpipe-0.8.6/lstmcpipe/scripts/tests/test_lstmcpipe_validate_config.py
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)      982 2022-05-12 06:59:42.000000 lstmcpipe-0.8.6/lstmcpipe/scripts/tests/test_scripts.py
-drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-07-13 11:21:01.997109 lstmcpipe-0.8.6/lstmcpipe/scripts/useful_tmp_scripts/
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     1758 2022-05-19 20:14:40.000000 lstmcpipe-0.8.6/lstmcpipe/scripts/useful_tmp_scripts/clean_corrupted_dl1_dirs_allSky.py
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     1276 2022-05-17 21:37:00.000000 lstmcpipe-0.8.6/lstmcpipe/scripts/useful_tmp_scripts/cleandir.py
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)      986 2022-06-01 16:34:15.000000 lstmcpipe-0.8.6/lstmcpipe/scripts/useful_tmp_scripts/rerun_irfs_mem_issue.py
-drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-07-13 11:21:02.000001 lstmcpipe-0.8.6/lstmcpipe/stages/
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)      869 2022-04-20 13:44:05.000000 lstmcpipe-0.8.6/lstmcpipe/stages/__init__.py
--rwxr-xr-x   0 thomasvuillaume   (502) staff       (20)     4810 2022-07-13 11:20:55.000000 lstmcpipe-0.8.6/lstmcpipe/stages/mc_dl1_to_dl2.py
--rwxr-xr-x   0 thomasvuillaume   (502) staff       (20)     5379 2022-07-13 11:20:55.000000 lstmcpipe-0.8.6/lstmcpipe/stages/mc_dl2_to_irfs.py
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     5241 2022-07-13 11:20:55.000000 lstmcpipe-0.8.6/lstmcpipe/stages/mc_dl2_to_sensitivity.py
--rwxr-xr-x   0 thomasvuillaume   (502) staff       (20)     4300 2022-07-13 11:20:55.000000 lstmcpipe-0.8.6/lstmcpipe/stages/mc_merge_dl1.py
--rwxr-xr-x   0 thomasvuillaume   (502) staff       (20)    13576 2022-07-13 11:20:55.000000 lstmcpipe-0.8.6/lstmcpipe/stages/mc_process_dl1.py
--rwxr-xr-x   0 thomasvuillaume   (502) staff       (20)     7566 2022-07-13 11:20:55.000000 lstmcpipe-0.8.6/lstmcpipe/stages/mc_train.py
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     3876 2022-07-13 11:20:55.000000 lstmcpipe-0.8.6/lstmcpipe/stages/mc_train_test_splitting.py
-drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-07-13 11:21:02.005050 lstmcpipe-0.8.6/lstmcpipe/standard_configs/
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     1249 2021-12-14 22:30:35.000000 lstmcpipe-0.8.6/lstmcpipe/standard_configs/ctapipe_standard_config_v011.json
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     1145 2021-12-14 22:30:35.000000 lstmcpipe-0.8.6/lstmcpipe/standard_configs/hiperta_standard_config.txt
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     6580 2022-04-01 16:15:10.000000 lstmcpipe-0.8.6/lstmcpipe/standard_configs/lstchain_dl1ab_tune_MC_to_Crab_config_v091_MC_Tel1.json
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     2209 2021-12-14 22:30:35.000000 lstmcpipe-0.8.6/lstmcpipe/standard_configs/lstchain_standard_config_v045.json
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     3497 2022-04-01 16:15:10.000000 lstmcpipe-0.8.6/lstmcpipe/standard_configs/lstchain_standard_config_v050.json
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     3633 2021-12-14 22:30:35.000000 lstmcpipe-0.8.6/lstmcpipe/standard_configs/lstchain_standard_config_v052.json
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     3617 2021-12-14 22:30:35.000000 lstmcpipe-0.8.6/lstmcpipe/standard_configs/lstchain_standard_config_v060.json
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     3666 2021-12-14 22:30:35.000000 lstmcpipe-0.8.6/lstmcpipe/standard_configs/lstchain_standard_config_v061.json
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     4635 2021-12-14 22:30:35.000000 lstmcpipe-0.8.6/lstmcpipe/standard_configs/lstchain_standard_config_v070.json
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     6338 2022-03-10 14:15:21.000000 lstmcpipe-0.8.6/lstmcpipe/standard_configs/lstchain_standard_config_v091.json
-drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-07-13 11:21:02.006991 lstmcpipe-0.8.6/lstmcpipe/tests/
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)        0 2021-12-14 22:30:35.000000 lstmcpipe-0.8.6/lstmcpipe/tests/__init__.py
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)      380 2022-05-17 21:37:00.000000 lstmcpipe-0.8.6/lstmcpipe/tests/test_cmd_lines.py
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)       83 2022-05-12 06:59:42.000000 lstmcpipe-0.8.6/lstmcpipe/tests/test_install.py
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)        0 2022-05-24 17:35:32.000000 lstmcpipe-0.8.6/lstmcpipe/tests/test_lstchain.py
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     4520 2022-07-13 11:20:55.000000 lstmcpipe-0.8.6/lstmcpipe/tests/test_utils.py
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)    13455 2022-07-13 11:20:55.000000 lstmcpipe-0.8.6/lstmcpipe/utils.py
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)      857 2022-05-12 06:59:42.000000 lstmcpipe-0.8.6/lstmcpipe/version.py
-drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-07-13 11:21:01.973201 lstmcpipe-0.8.6/lstmcpipe.egg-info/
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)      595 2022-07-13 11:21:01.000000 lstmcpipe-0.8.6/lstmcpipe.egg-info/PKG-INFO
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     9374 2022-07-13 11:21:01.000000 lstmcpipe-0.8.6/lstmcpipe.egg-info/SOURCES.txt
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)        1 2022-07-13 11:21:01.000000 lstmcpipe-0.8.6/lstmcpipe.egg-info/dependency_links.txt
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)      982 2022-07-13 11:21:01.000000 lstmcpipe-0.8.6/lstmcpipe.egg-info/entry_points.txt
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)      107 2022-07-13 11:21:01.000000 lstmcpipe-0.8.6/lstmcpipe.egg-info/requires.txt
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)       10 2022-07-13 11:21:01.000000 lstmcpipe-0.8.6/lstmcpipe.egg-info/top_level.txt
-drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-07-13 11:21:01.953098 lstmcpipe-0.8.6/production_configs/
-drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-07-13 11:21:02.008602 lstmcpipe-0.8.6/production_configs/20210416_v0.7.3_prod5_trans_80_local_taicut_8_4/
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     1840 2022-04-13 17:39:20.000000 lstmcpipe-0.8.6/production_configs/20210416_v0.7.3_prod5_trans_80_local_taicut_8_4/config_MC_prod_20210416_v0.7.3_prod5_trans_80_local_taicut_8_4.yml
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     4692 2022-04-13 17:39:20.000000 lstmcpipe-0.8.6/production_configs/20210416_v0.7.3_prod5_trans_80_local_taicut_8_4/lstchain_standard_config_v073_Tel1_tail_8_4_MC_config.json
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)       65 2022-04-13 17:39:20.000000 lstmcpipe-0.8.6/production_configs/20210416_v0.7.3_prod5_trans_80_local_taicut_8_4/readme.md
-drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-07-13 11:21:02.010112 lstmcpipe-0.8.6/production_configs/20210506_v0.7.3_prod5_trans_80_zen40deg_local_tailcut_8_4/
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     1642 2022-04-13 17:39:20.000000 lstmcpipe-0.8.6/production_configs/20210506_v0.7.3_prod5_trans_80_zen40deg_local_tailcut_8_4/config_MC_prod_20210506_v0.7.3_prod5_trans_80_zen40deg_local_tailcut_8_4.yml
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     4692 2022-04-13 17:39:20.000000 lstmcpipe-0.8.6/production_configs/20210506_v0.7.3_prod5_trans_80_zen40deg_local_tailcut_8_4/lstchain_standard_config_v073_Tel1_tail_8_4_MC_config.json
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)       75 2022-04-13 17:39:20.000000 lstmcpipe-0.8.6/production_configs/20210506_v0.7.3_prod5_trans_80_zen40deg_local_tailcut_8_4/readme.md
-drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-07-13 11:21:02.011521 lstmcpipe-0.8.6/production_configs/20210923_v0.7.5_prod5_trans_80_dynamic_cleaning/
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     1727 2022-04-13 17:39:20.000000 lstmcpipe-0.8.6/production_configs/20210923_v0.7.5_prod5_trans_80_dynamic_cleaning/config_MC_prod_20210923_v0.7.5_prod5_trans_80_dynamic_cleaning.yml
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     4802 2022-04-13 17:39:20.000000 lstmcpipe-0.8.6/production_configs/20210923_v0.7.5_prod5_trans_80_dynamic_cleaning/lstchain_standard_config_v075_Tel1_tail84_dynamic_clean.json
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)       65 2022-04-13 17:39:20.000000 lstmcpipe-0.8.6/production_configs/20210923_v0.7.5_prod5_trans_80_dynamic_cleaning/readme.md
-drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-07-13 11:21:02.013013 lstmcpipe-0.8.6/production_configs/20220215_v0.9.1_prod5_trans_80_local_tailcut_8_4/
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     1880 2022-04-13 17:39:20.000000 lstmcpipe-0.8.6/production_configs/20220215_v0.9.1_prod5_trans_80_local_tailcut_8_4/config_MC_prod_20220215_v0.9.1_prod5_trans_80_local_tailcut_8_4.yml
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     6319 2022-04-13 17:39:20.000000 lstmcpipe-0.8.6/production_configs/20220215_v0.9.1_prod5_trans_80_local_tailcut_8_4/lstchain_standard_config_v091_MC_Tel1.json
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)       69 2022-04-13 17:39:20.000000 lstmcpipe-0.8.6/production_configs/20220215_v0.9.1_prod5_trans_80_local_tailcut_8_4/readme.md
-drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-07-13 11:21:02.014439 lstmcpipe-0.8.6/production_configs/20220218_v0.9.2_prod5_trans_80_dl1ab_tune_MC_to_Crab/
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     1922 2022-04-13 17:39:20.000000 lstmcpipe-0.8.6/production_configs/20220218_v0.9.2_prod5_trans_80_dl1ab_tune_MC_to_Crab/config_MC_prod_20220218_v0.9.2_prod5_trans_80_dl1ab_tune_MC_to_Crab.yml
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     6580 2022-04-13 17:39:20.000000 lstmcpipe-0.8.6/production_configs/20220218_v0.9.2_prod5_trans_80_dl1ab_tune_MC_to_Crab/lstchain_dl1ab_tune_MC_to_Crab_config_v091_MC_Tel1.json
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)       70 2022-04-13 17:39:20.000000 lstmcpipe-0.8.6/production_configs/20220218_v0.9.2_prod5_trans_80_dl1ab_tune_MC_to_Crab/readme.md
-drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-07-13 11:21:02.015680 lstmcpipe-0.8.6/production_configs/20220304_v0.9.3_prod5_trans_80_zen40az180_local_tailcut_8_4/
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     1376 2022-04-13 17:39:20.000000 lstmcpipe-0.8.6/production_configs/20220304_v0.9.3_prod5_trans_80_zen40az180_local_tailcut_8_4/config_MC_prod_20220304_v0.9.3_prod5_trans_80_zen40az180_local_tailcut_8_4.yml
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     6319 2022-04-13 17:39:20.000000 lstmcpipe-0.8.6/production_configs/20220304_v0.9.3_prod5_trans_80_zen40az180_local_tailcut_8_4/lstchain_standard_config_v091_MC_Tel1.json
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)       77 2022-04-13 17:39:20.000000 lstmcpipe-0.8.6/production_configs/20220304_v0.9.3_prod5_trans_80_zen40az180_local_tailcut_8_4/readme.md
-drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-07-13 11:21:02.017391 lstmcpipe-0.8.6/production_configs/20220511_v0.9.6_allsky_std/
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)      183 2022-05-20 09:49:47.000000 lstmcpipe-0.8.6/production_configs/20220511_v0.9.6_allsky_std/README.md
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)      992 2022-05-20 09:49:47.000000 lstmcpipe-0.8.6/production_configs/20220511_v0.9.6_allsky_std/generate.py
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     6453 2022-05-20 09:49:47.000000 lstmcpipe-0.8.6/production_configs/20220511_v0.9.6_allsky_std/lstchain_84.json
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)   234487 2022-05-20 09:49:47.000000 lstmcpipe-0.8.6/production_configs/20220511_v0.9.6_allsky_std/lstmcpipe_config_20220511_allsky_std.yml
-drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-07-13 11:21:02.020649 lstmcpipe-0.8.6/production_configs/20220518_v0.9.6_allsky_dec2276_tuned/
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)      347 2022-05-20 10:24:24.000000 lstmcpipe-0.8.6/production_configs/20220518_v0.9.6_allsky_dec2276_tuned/README.md
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)      255 2022-05-20 10:24:24.000000 lstmcpipe-0.8.6/production_configs/20220518_v0.9.6_allsky_dec2276_tuned/generate.py
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     8492 2022-05-20 10:24:24.000000 lstmcpipe-0.8.6/production_configs/20220518_v0.9.6_allsky_dec2276_tuned/lstchain_config_dec_2276_tuned.json
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)    68680 2022-05-20 10:24:24.000000 lstmcpipe-0.8.6/production_configs/20220518_v0.9.6_allsky_dec2276_tuned/lstmcpipe_config_20220518_allsky_dec2276_tuned.yml
-drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-07-13 11:21:02.022283 lstmcpipe-0.8.6/production_configs/20220523_allsky_std/
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)      248 2022-06-01 16:34:15.000000 lstmcpipe-0.8.6/production_configs/20220523_allsky_std/README.md
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     8179 2022-06-01 16:34:15.000000 lstmcpipe-0.8.6/production_configs/20220523_allsky_std/lstchain_config_2022-05-23.json
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)   110282 2022-06-01 16:34:15.000000 lstmcpipe-0.8.6/production_configs/20220523_allsky_std/lstmcpipe_config_2022-05-23_PathConfigAllSkyFull.yaml
-drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-07-13 11:21:02.025539 lstmcpipe-0.8.6/production_configs/20220523_dec_413_tuned_nsb/
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     8523 2022-06-01 16:34:15.000000 lstmcpipe-0.8.6/production_configs/20220523_dec_413_tuned_nsb/lstchain_config_2022-05-23.json
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)    69249 2022-06-01 16:34:15.000000 lstmcpipe-0.8.6/production_configs/20220523_dec_413_tuned_nsb/lstmcpipe_config_2022-05-23_PathConfigAllSkyFullDL1ab.yaml
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)      499 2022-06-01 16:34:15.000000 lstmcpipe-0.8.6/production_configs/20220523_dec_413_tuned_nsb/readme.md
-drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-07-13 11:21:02.027895 lstmcpipe-0.8.6/production_configs/20220523_src3_dec3476_4822_tuned_nsb/
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     8464 2022-06-01 16:34:15.000000 lstmcpipe-0.8.6/production_configs/20220523_src3_dec3476_4822_tuned_nsb/lstchain_config_2022-05-23.json
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)   114152 2022-06-01 16:34:15.000000 lstmcpipe-0.8.6/production_configs/20220523_src3_dec3476_4822_tuned_nsb/lstmcpipe_config_2022-05-23_PathConfigAllSkyFullDL1ab.yml
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)      520 2022-06-01 16:34:15.000000 lstmcpipe-0.8.6/production_configs/20220523_src3_dec3476_4822_tuned_nsb/readme.md
-drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-07-13 11:21:02.029254 lstmcpipe-0.8.6/production_configs/20220524_dec_4822_tuned/
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)      565 2022-06-01 16:34:15.000000 lstmcpipe-0.8.6/production_configs/20220524_dec_4822_tuned/README_tuned_22_05_24.md
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     7488 2022-06-01 16:34:15.000000 lstmcpipe-0.8.6/production_configs/20220524_dec_4822_tuned/lstchain_config_2022-05-24.json
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)    66936 2022-06-01 16:34:15.000000 lstmcpipe-0.8.6/production_configs/20220524_dec_4822_tuned/lstmcpipe_config_2022-05-24_PathConfigAllSkyFullDL1ab.yaml
-drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-07-13 11:21:02.031694 lstmcpipe-0.8.6/production_configs/20220527_allsky_std_src2_diffgamma/
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)      147 2022-06-01 16:34:15.000000 lstmcpipe-0.8.6/production_configs/20220527_allsky_std_src2_diffgamma/README.md
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     7002 2022-06-01 16:34:15.000000 lstmcpipe-0.8.6/production_configs/20220527_allsky_std_src2_diffgamma/lstchain_config_2022-05-27.json
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     3311 2022-06-01 16:34:15.000000 lstmcpipe-0.8.6/production_configs/20220527_allsky_std_src2_diffgamma/lstmcpipe_config_2022-05-27_PathConfigAllSkyFull.yaml
-drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-07-13 11:21:02.033227 lstmcpipe-0.8.6/production_configs/20220531_dec3476_std/
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)      252 2022-06-01 16:34:15.000000 lstmcpipe-0.8.6/production_configs/20220531_dec3476_std/README.md
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     8225 2022-06-01 16:34:15.000000 lstmcpipe-0.8.6/production_configs/20220531_dec3476_std/lstchain_config_2022-05-31.json
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)    66650 2022-06-01 16:34:15.000000 lstmcpipe-0.8.6/production_configs/20220531_dec3476_std/lstmcpipe_config_2022-05-31_PathConfigAllSkyFull.yaml
-drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-07-13 11:21:02.035218 lstmcpipe-0.8.6/production_configs/20220601_dec3476_tuned/
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)      292 2022-06-01 16:34:15.000000 lstmcpipe-0.8.6/production_configs/20220601_dec3476_tuned/README.md
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     8464 2022-06-01 16:34:15.000000 lstmcpipe-0.8.6/production_configs/20220601_dec3476_tuned/lstchain_config_2022-06-01.json
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)    67036 2022-06-01 16:34:15.000000 lstmcpipe-0.8.6/production_configs/20220601_dec3476_tuned/lstmcpipe_config_2022-06-01_PathConfigAllSkyFullDL1ab.yaml
-drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-07-13 11:21:02.037770 lstmcpipe-0.8.6/production_configs/20220624_dec_4822_tuned_TestDIffuseGammas/
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)      683 2022-06-24 14:00:53.000000 lstmcpipe-0.8.6/production_configs/20220624_dec_4822_tuned_TestDIffuseGammas/README_tuned_22_06_24_TestDiffuseGammas.md
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     7488 2022-06-24 14:00:53.000000 lstmcpipe-0.8.6/production_configs/20220624_dec_4822_tuned_TestDIffuseGammas/lstchain_config_2022-06-24.json
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     6930 2022-06-27 15:21:35.000000 lstmcpipe-0.8.6/production_configs/20220624_dec_4822_tuned_TestDIffuseGammas/lstmcpipe_config_2022-06-24_TestDiffuseGammas.yaml
-drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-07-13 11:21:02.039295 lstmcpipe-0.8.6/production_configs/nsb_psf_tuned_zen40_src2/
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     6583 2022-04-13 17:39:20.000000 lstmcpipe-0.8.6/production_configs/nsb_psf_tuned_zen40_src2/lstchain_config_ze40_south_NSBtuning.json
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     1319 2022-04-13 17:39:20.000000 lstmcpipe-0.8.6/production_configs/nsb_psf_tuned_zen40_src2/lstmcpipe_config.yml
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)      252 2022-04-13 17:39:20.000000 lstmcpipe-0.8.6/production_configs/nsb_psf_tuned_zen40_src2/readme.md
-drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-07-13 11:21:02.040879 lstmcpipe-0.8.6/production_configs/nsb_tuned_zen40_scr1/
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     7106 2022-04-13 17:39:20.000000 lstmcpipe-0.8.6/production_configs/nsb_tuned_zen40_scr1/lstchain_config_NSBtuning.json
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     1421 2022-04-13 17:39:20.000000 lstmcpipe-0.8.6/production_configs/nsb_tuned_zen40_scr1/lstmcpipe_config.yml
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)      232 2022-04-13 17:39:20.000000 lstmcpipe-0.8.6/production_configs/nsb_tuned_zen40_scr1/readme.md
-drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-07-13 11:21:02.042763 lstmcpipe-0.8.6/production_configs/psf_tuned_zen20/
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     7120 2022-04-13 17:39:20.000000 lstmcpipe-0.8.6/production_configs/psf_tuned_zen20/lstchain_config.json
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     1298 2022-04-13 17:39:20.000000 lstmcpipe-0.8.6/production_configs/psf_tuned_zen20/lstmcpipe_config.yml
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)      353 2022-04-13 17:39:20.000000 lstmcpipe-0.8.6/production_configs/psf_tuned_zen20/readme.md
-drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-07-13 11:21:02.044720 lstmcpipe-0.8.6/production_configs/psf_tuned_zen40/
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     7120 2022-04-13 17:39:20.000000 lstmcpipe-0.8.6/production_configs/psf_tuned_zen40/lstchain_config.json
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     1309 2022-04-13 17:39:20.000000 lstmcpipe-0.8.6/production_configs/psf_tuned_zen40/lstmcpipe_config.yml
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)      353 2022-04-13 17:39:20.000000 lstmcpipe-0.8.6/production_configs/psf_tuned_zen40/readme.md
-drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-07-13 11:21:02.046627 lstmcpipe-0.8.6/production_configs/template_prod/
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     6846 2022-04-01 16:15:10.000000 lstmcpipe-0.8.6/production_configs/template_prod/lstchain_config.json
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)      466 2022-06-23 07:20:36.000000 lstmcpipe-0.8.6/production_configs/template_prod/lstmcpipe_config.yml
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)      192 2022-04-01 16:15:10.000000 lstmcpipe-0.8.6/production_configs/template_prod/readme.md
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)       38 2022-07-13 11:21:02.048045 lstmcpipe-0.8.6/setup.cfg
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     3069 2022-06-01 16:34:15.000000 lstmcpipe-0.8.6/setup.py
+drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-10-10 08:57:13.038209 lstmcpipe-0.9.0/
+drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-10-10 08:57:12.854421 lstmcpipe-0.9.0/.github/
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)      630 2022-04-01 16:15:10.000000 lstmcpipe-0.9.0/.github/pull_request_template.md
+drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-10-10 08:57:12.860149 lstmcpipe-0.9.0/.github/workflows/
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     2580 2022-09-11 16:24:04.000000 lstmcpipe-0.9.0/.github/workflows/CI.yml
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)      786 2022-06-01 16:34:15.000000 lstmcpipe-0.9.0/.github/workflows/codemeta2citation.yml
+drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-10-10 08:57:12.861132 lstmcpipe-0.9.0/.github/workflows/dev/
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     1047 2022-05-19 20:14:47.000000 lstmcpipe-0.9.0/.github/workflows/dev/codemeta2citation.py
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)      868 2022-05-06 08:55:35.000000 lstmcpipe-0.9.0/.github/workflows/docs.yml
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)      403 2022-05-19 20:14:47.000000 lstmcpipe-0.9.0/.github/workflows/pypi.yml
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)      232 2022-05-06 08:55:46.000000 lstmcpipe-0.9.0/.gitignore
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)      646 2022-09-09 16:56:05.000000 lstmcpipe-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)    18219 2022-04-01 16:15:10.000000 lstmcpipe-0.9.0/.pylintrc
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)      555 2022-05-19 20:14:47.000000 lstmcpipe-0.9.0/CITATION.cff
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)      595 2022-10-10 08:57:13.037553 lstmcpipe-0.9.0/PKG-INFO
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)    13312 2022-06-01 16:34:15.000000 lstmcpipe-0.9.0/README.rst
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     2803 2022-10-10 08:56:16.000000 lstmcpipe-0.9.0/codemeta.json
+drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-10-10 08:57:12.870147 lstmcpipe-0.9.0/docs/
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)      752 2022-04-13 17:39:20.000000 lstmcpipe-0.9.0/docs/Makefile
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     2455 2022-07-04 15:24:42.000000 lstmcpipe-0.9.0/docs/conf.py
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)      475 2022-04-19 12:26:15.000000 lstmcpipe-0.9.0/docs/index.rst
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)      800 2021-12-16 12:11:58.000000 lstmcpipe-0.9.0/docs/make.bat
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     5448 2022-05-20 09:49:47.000000 lstmcpipe-0.9.0/docs/pipeline.rst
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     2121 2022-06-01 16:34:15.000000 lstmcpipe-0.9.0/docs/produce_config_page.py
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)      335 2022-05-24 15:01:00.000000 lstmcpipe-0.9.0/docs/productions.rst
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)      131 2022-04-19 12:26:15.000000 lstmcpipe-0.9.0/docs/requirements.txt
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)      309 2022-06-01 16:34:15.000000 lstmcpipe-0.9.0/environment.yml
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     1079 2022-01-18 22:35:07.000000 lstmcpipe-0.9.0/license.rst
+drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-10-10 08:57:12.877831 lstmcpipe-0.9.0/lstmcpipe/
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)      323 2022-05-12 06:59:42.000000 lstmcpipe-0.9.0/lstmcpipe/__init__.py
+drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-10-10 08:57:12.883532 lstmcpipe-0.9.0/lstmcpipe/_dev_version/
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)      397 2022-05-12 06:59:42.000000 lstmcpipe-0.9.0/lstmcpipe/_dev_version/_dev_version.py
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)       35 2022-09-09 17:02:28.000000 lstmcpipe-0.9.0/lstmcpipe/_version.py
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)      843 2022-05-17 21:37:00.000000 lstmcpipe-0.9.0/lstmcpipe/base_config_lstmcpipe.yaml
+drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-10-10 08:57:12.885665 lstmcpipe-0.9.0/lstmcpipe/benchmarks/
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)        0 2022-03-10 14:15:21.000000 lstmcpipe-0.9.0/lstmcpipe/benchmarks/__init__.py
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     2542 2022-05-12 06:59:42.000000 lstmcpipe-0.9.0/lstmcpipe/benchmarks/irfs.py
+drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-10-10 08:57:12.892170 lstmcpipe-0.9.0/lstmcpipe/config/
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)      680 2022-04-20 13:44:05.000000 lstmcpipe-0.9.0/lstmcpipe/config/__init__.py
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     2120 2022-05-12 06:59:42.000000 lstmcpipe-0.9.0/lstmcpipe/config/dl1ab_tuning.py
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)    38180 2022-10-10 08:56:16.000000 lstmcpipe-0.9.0/lstmcpipe/config/paths_config.py
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     5730 2022-05-24 15:44:30.000000 lstmcpipe-0.9.0/lstmcpipe/config/pipeline_config.py
+drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-10-10 08:57:12.895328 lstmcpipe-0.9.0/lstmcpipe/config/tests/
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)        0 2021-12-14 22:30:35.000000 lstmcpipe-0.9.0/lstmcpipe/config/tests/__init__.py
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     5469 2022-05-17 21:37:00.000000 lstmcpipe-0.9.0/lstmcpipe/config/tests/test_paths_config.py
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     2925 2022-05-17 21:37:00.000000 lstmcpipe-0.9.0/lstmcpipe/config/tests/test_pipeline_config.py
+drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-10-10 08:57:12.899248 lstmcpipe-0.9.0/lstmcpipe/hiperta/
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)        0 2021-12-14 22:30:35.000000 lstmcpipe-0.9.0/lstmcpipe/hiperta/__init__.py
+-rwxr-xr-x   0 thomasvuillaume   (502) staff       (20)     2376 2022-05-12 06:59:42.000000 lstmcpipe-0.9.0/lstmcpipe/hiperta/hiperta_r0_to_dl1lstchain.py
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)    10993 2022-05-31 12:09:03.000000 lstmcpipe-0.9.0/lstmcpipe/hiperta/reorganize_dl1hiperta300_to_dl1lstchain060.py
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)    15690 2022-05-31 12:09:03.000000 lstmcpipe-0.9.0/lstmcpipe/hiperta/reorganize_dl1hiperta_to_dl1lstchain.py
+drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-10-10 08:57:12.902086 lstmcpipe-0.9.0/lstmcpipe/io/
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)        0 2021-12-14 22:30:35.000000 lstmcpipe-0.9.0/lstmcpipe/io/__init__.py
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     4420 2022-05-17 21:37:00.000000 lstmcpipe-0.9.0/lstmcpipe/io/data_management.py
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     3219 2022-05-31 12:09:03.000000 lstmcpipe-0.9.0/lstmcpipe/io/lstmcpipe_tree_path.py
+drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-10-10 08:57:12.906401 lstmcpipe-0.9.0/lstmcpipe/io/tests/
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)        0 2022-04-13 17:39:20.000000 lstmcpipe-0.9.0/lstmcpipe/io/tests/__init__.py
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     1232 2022-05-12 06:59:42.000000 lstmcpipe-0.9.0/lstmcpipe/io/tests/test_data_management.py
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     1735 2022-05-12 06:59:42.000000 lstmcpipe-0.9.0/lstmcpipe/io/tests/test_lstmcpipe_tree_path.py
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     1892 2022-05-19 20:14:47.000000 lstmcpipe-0.9.0/lstmcpipe/logging.py
+-rwxr-xr-x   0 thomasvuillaume   (502) staff       (20)    10279 2022-10-10 08:56:16.000000 lstmcpipe-0.9.0/lstmcpipe/lstmcpipe_start.py
+drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-10-10 08:57:12.910287 lstmcpipe-0.9.0/lstmcpipe/metrics/
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)    14058 2022-07-12 15:23:11.000000 lstmcpipe-0.9.0/lstmcpipe/metrics/__init__.py
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)        0 2022-07-08 12:52:12.000000 lstmcpipe-0.9.0/lstmcpipe/metrics/angular_resolution.py
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)        0 2022-07-08 12:52:44.000000 lstmcpipe-0.9.0/lstmcpipe/metrics/class.py
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)        0 2022-07-08 12:52:39.000000 lstmcpipe-0.9.0/lstmcpipe/metrics/direction.py
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)        0 2022-07-08 12:52:30.000000 lstmcpipe-0.9.0/lstmcpipe/metrics/energy.py
+drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-10-10 08:57:12.914512 lstmcpipe-0.9.0/lstmcpipe/plots/
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)        0 2021-12-14 22:30:35.000000 lstmcpipe-0.9.0/lstmcpipe/plots/__init__.py
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     3221 2022-05-31 12:09:03.000000 lstmcpipe-0.9.0/lstmcpipe/plots/images_debug.py
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)    13340 2022-07-13 11:20:55.000000 lstmcpipe-0.9.0/lstmcpipe/plots/plot_irfs.py
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)      728 2022-05-12 06:59:42.000000 lstmcpipe-0.9.0/lstmcpipe/plots/plot_models_importance.py
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     2574 2022-06-24 13:17:16.000000 lstmcpipe-0.9.0/lstmcpipe/plots/pointings.py
+drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-10-10 08:57:12.916543 lstmcpipe-0.9.0/lstmcpipe/plots/tests/
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)      365 2022-05-19 20:14:40.000000 lstmcpipe-0.9.0/lstmcpipe/plots/tests/test_pointings.py
+drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-10-10 08:57:12.930997 lstmcpipe-0.9.0/lstmcpipe/scripts/
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)        0 2021-12-14 22:30:35.000000 lstmcpipe-0.9.0/lstmcpipe/scripts/__init__.py
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     6736 2022-09-13 14:00:21.000000 lstmcpipe-0.9.0/lstmcpipe/scripts/generate_test_lapalma.py
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     3595 2022-06-01 16:34:15.000000 lstmcpipe-0.9.0/lstmcpipe/scripts/lstmcpipe_generate_config.py
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     1766 2022-05-31 12:09:03.000000 lstmcpipe-0.9.0/lstmcpipe/scripts/script_batch_filelist_cta.py
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     1913 2022-05-20 10:03:09.000000 lstmcpipe-0.9.0/lstmcpipe/scripts/script_batch_filelist_lst.py
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     2105 2022-05-20 10:03:09.000000 lstmcpipe-0.9.0/lstmcpipe/scripts/script_batch_filelist_lst_dl1ab.py
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     2179 2022-05-20 10:03:09.000000 lstmcpipe-0.9.0/lstmcpipe/scripts/script_batch_filelist_rta.py
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     2346 2022-07-13 11:20:55.000000 lstmcpipe-0.9.0/lstmcpipe/scripts/script_compare_irfs.py
+-rwxr-xr-x   0 thomasvuillaume   (502) staff       (20)    12483 2022-05-12 06:59:42.000000 lstmcpipe-0.9.0/lstmcpipe/scripts/script_dl2_to_sensitivity.py
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     2068 2022-06-01 16:34:15.000000 lstmcpipe-0.9.0/lstmcpipe/scripts/script_lstmcpipe_validate_config.py
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     2281 2022-05-12 06:59:42.000000 lstmcpipe-0.9.0/lstmcpipe/scripts/script_train_test_splitting.py
+drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-10-10 08:57:12.933303 lstmcpipe-0.9.0/lstmcpipe/scripts/tests/
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)        0 2021-12-14 22:30:22.000000 lstmcpipe-0.9.0/lstmcpipe/scripts/tests/__init__.py
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)        0 2022-04-20 13:44:05.000000 lstmcpipe-0.9.0/lstmcpipe/scripts/tests/test_lstmcpipe_validate_config.py
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)      982 2022-05-12 06:59:42.000000 lstmcpipe-0.9.0/lstmcpipe/scripts/tests/test_scripts.py
+drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-10-10 08:57:12.937662 lstmcpipe-0.9.0/lstmcpipe/scripts/useful_tmp_scripts/
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     1758 2022-05-19 20:14:40.000000 lstmcpipe-0.9.0/lstmcpipe/scripts/useful_tmp_scripts/clean_corrupted_dl1_dirs_allSky.py
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     1276 2022-05-17 21:37:00.000000 lstmcpipe-0.9.0/lstmcpipe/scripts/useful_tmp_scripts/cleandir.py
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)      995 2022-09-13 14:00:21.000000 lstmcpipe-0.9.0/lstmcpipe/scripts/useful_tmp_scripts/rerun_irfs_mem_issue.py
+drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-10-10 08:57:12.946992 lstmcpipe-0.9.0/lstmcpipe/stages/
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)      869 2022-04-20 13:44:05.000000 lstmcpipe-0.9.0/lstmcpipe/stages/__init__.py
+-rwxr-xr-x   0 thomasvuillaume   (502) staff       (20)     4654 2022-09-13 14:00:21.000000 lstmcpipe-0.9.0/lstmcpipe/stages/mc_dl1_to_dl2.py
+-rwxr-xr-x   0 thomasvuillaume   (502) staff       (20)     5374 2022-09-13 14:00:21.000000 lstmcpipe-0.9.0/lstmcpipe/stages/mc_dl2_to_irfs.py
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     5051 2022-09-13 14:00:21.000000 lstmcpipe-0.9.0/lstmcpipe/stages/mc_dl2_to_sensitivity.py
+-rwxr-xr-x   0 thomasvuillaume   (502) staff       (20)     3655 2022-09-13 14:00:21.000000 lstmcpipe-0.9.0/lstmcpipe/stages/mc_merge_dl1.py
+-rwxr-xr-x   0 thomasvuillaume   (502) staff       (20)    12769 2022-09-13 14:00:21.000000 lstmcpipe-0.9.0/lstmcpipe/stages/mc_process_dl1.py
+-rwxr-xr-x   0 thomasvuillaume   (502) staff       (20)     7606 2022-09-13 14:00:21.000000 lstmcpipe-0.9.0/lstmcpipe/stages/mc_train.py
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     3921 2022-09-13 14:00:21.000000 lstmcpipe-0.9.0/lstmcpipe/stages/mc_train_test_splitting.py
+drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-10-10 08:57:12.962322 lstmcpipe-0.9.0/lstmcpipe/standard_configs/
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     1249 2021-12-14 22:30:35.000000 lstmcpipe-0.9.0/lstmcpipe/standard_configs/ctapipe_standard_config_v011.json
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     1145 2021-12-14 22:30:35.000000 lstmcpipe-0.9.0/lstmcpipe/standard_configs/hiperta_standard_config.txt
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     6580 2022-04-01 16:15:10.000000 lstmcpipe-0.9.0/lstmcpipe/standard_configs/lstchain_dl1ab_tune_MC_to_Crab_config_v091_MC_Tel1.json
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     2209 2021-12-14 22:30:35.000000 lstmcpipe-0.9.0/lstmcpipe/standard_configs/lstchain_standard_config_v045.json
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     3497 2022-04-01 16:15:10.000000 lstmcpipe-0.9.0/lstmcpipe/standard_configs/lstchain_standard_config_v050.json
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     3633 2021-12-14 22:30:35.000000 lstmcpipe-0.9.0/lstmcpipe/standard_configs/lstchain_standard_config_v052.json
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     3617 2021-12-14 22:30:35.000000 lstmcpipe-0.9.0/lstmcpipe/standard_configs/lstchain_standard_config_v060.json
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     3666 2021-12-14 22:30:35.000000 lstmcpipe-0.9.0/lstmcpipe/standard_configs/lstchain_standard_config_v061.json
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     4635 2021-12-14 22:30:35.000000 lstmcpipe-0.9.0/lstmcpipe/standard_configs/lstchain_standard_config_v070.json
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     6338 2022-03-10 14:15:21.000000 lstmcpipe-0.9.0/lstmcpipe/standard_configs/lstchain_standard_config_v091.json
+drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-10-10 08:57:12.966893 lstmcpipe-0.9.0/lstmcpipe/tests/
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)        0 2021-12-14 22:30:35.000000 lstmcpipe-0.9.0/lstmcpipe/tests/__init__.py
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)      380 2022-05-17 21:37:00.000000 lstmcpipe-0.9.0/lstmcpipe/tests/test_cmd_lines.py
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)       83 2022-05-12 06:59:42.000000 lstmcpipe-0.9.0/lstmcpipe/tests/test_install.py
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)        0 2022-05-24 17:35:32.000000 lstmcpipe-0.9.0/lstmcpipe/tests/test_lstchain.py
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     4637 2022-09-13 14:00:21.000000 lstmcpipe-0.9.0/lstmcpipe/tests/test_utils.py
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)    13904 2022-09-13 14:00:21.000000 lstmcpipe-0.9.0/lstmcpipe/utils.py
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)      857 2022-05-12 06:59:42.000000 lstmcpipe-0.9.0/lstmcpipe/version.py
+drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-10-10 08:57:12.882193 lstmcpipe-0.9.0/lstmcpipe.egg-info/
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)      595 2022-10-10 08:57:12.000000 lstmcpipe-0.9.0/lstmcpipe.egg-info/PKG-INFO
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     9596 2022-10-10 08:57:12.000000 lstmcpipe-0.9.0/lstmcpipe.egg-info/SOURCES.txt
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)        1 2022-10-10 08:57:12.000000 lstmcpipe-0.9.0/lstmcpipe.egg-info/dependency_links.txt
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)      982 2022-10-10 08:57:12.000000 lstmcpipe-0.9.0/lstmcpipe.egg-info/entry_points.txt
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)      107 2022-10-10 08:57:12.000000 lstmcpipe-0.9.0/lstmcpipe.egg-info/requires.txt
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)       10 2022-10-10 08:57:12.000000 lstmcpipe-0.9.0/lstmcpipe.egg-info/top_level.txt
+drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-10-10 08:57:12.843339 lstmcpipe-0.9.0/production_configs/
+drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-10-10 08:57:12.969885 lstmcpipe-0.9.0/production_configs/20210416_v0.7.3_prod5_trans_80_local_taicut_8_4/
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     1840 2022-04-13 17:39:20.000000 lstmcpipe-0.9.0/production_configs/20210416_v0.7.3_prod5_trans_80_local_taicut_8_4/config_MC_prod_20210416_v0.7.3_prod5_trans_80_local_taicut_8_4.yml
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     4692 2022-04-13 17:39:20.000000 lstmcpipe-0.9.0/production_configs/20210416_v0.7.3_prod5_trans_80_local_taicut_8_4/lstchain_standard_config_v073_Tel1_tail_8_4_MC_config.json
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)       65 2022-04-13 17:39:20.000000 lstmcpipe-0.9.0/production_configs/20210416_v0.7.3_prod5_trans_80_local_taicut_8_4/readme.md
+drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-10-10 08:57:12.972791 lstmcpipe-0.9.0/production_configs/20210506_v0.7.3_prod5_trans_80_zen40deg_local_tailcut_8_4/
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     1642 2022-04-13 17:39:20.000000 lstmcpipe-0.9.0/production_configs/20210506_v0.7.3_prod5_trans_80_zen40deg_local_tailcut_8_4/config_MC_prod_20210506_v0.7.3_prod5_trans_80_zen40deg_local_tailcut_8_4.yml
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     4692 2022-04-13 17:39:20.000000 lstmcpipe-0.9.0/production_configs/20210506_v0.7.3_prod5_trans_80_zen40deg_local_tailcut_8_4/lstchain_standard_config_v073_Tel1_tail_8_4_MC_config.json
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)       75 2022-04-13 17:39:20.000000 lstmcpipe-0.9.0/production_configs/20210506_v0.7.3_prod5_trans_80_zen40deg_local_tailcut_8_4/readme.md
+drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-10-10 08:57:12.975556 lstmcpipe-0.9.0/production_configs/20210923_v0.7.5_prod5_trans_80_dynamic_cleaning/
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     1727 2022-04-13 17:39:20.000000 lstmcpipe-0.9.0/production_configs/20210923_v0.7.5_prod5_trans_80_dynamic_cleaning/config_MC_prod_20210923_v0.7.5_prod5_trans_80_dynamic_cleaning.yml
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     4802 2022-04-13 17:39:20.000000 lstmcpipe-0.9.0/production_configs/20210923_v0.7.5_prod5_trans_80_dynamic_cleaning/lstchain_standard_config_v075_Tel1_tail84_dynamic_clean.json
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)       65 2022-04-13 17:39:20.000000 lstmcpipe-0.9.0/production_configs/20210923_v0.7.5_prod5_trans_80_dynamic_cleaning/readme.md
+drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-10-10 08:57:12.978350 lstmcpipe-0.9.0/production_configs/20220215_v0.9.1_prod5_trans_80_local_tailcut_8_4/
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     1880 2022-04-13 17:39:20.000000 lstmcpipe-0.9.0/production_configs/20220215_v0.9.1_prod5_trans_80_local_tailcut_8_4/config_MC_prod_20220215_v0.9.1_prod5_trans_80_local_tailcut_8_4.yml
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     6319 2022-04-13 17:39:20.000000 lstmcpipe-0.9.0/production_configs/20220215_v0.9.1_prod5_trans_80_local_tailcut_8_4/lstchain_standard_config_v091_MC_Tel1.json
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)       69 2022-04-13 17:39:20.000000 lstmcpipe-0.9.0/production_configs/20220215_v0.9.1_prod5_trans_80_local_tailcut_8_4/readme.md
+drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-10-10 08:57:12.981632 lstmcpipe-0.9.0/production_configs/20220218_v0.9.2_prod5_trans_80_dl1ab_tune_MC_to_Crab/
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     1922 2022-04-13 17:39:20.000000 lstmcpipe-0.9.0/production_configs/20220218_v0.9.2_prod5_trans_80_dl1ab_tune_MC_to_Crab/config_MC_prod_20220218_v0.9.2_prod5_trans_80_dl1ab_tune_MC_to_Crab.yml
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     6580 2022-04-13 17:39:20.000000 lstmcpipe-0.9.0/production_configs/20220218_v0.9.2_prod5_trans_80_dl1ab_tune_MC_to_Crab/lstchain_dl1ab_tune_MC_to_Crab_config_v091_MC_Tel1.json
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)       70 2022-04-13 17:39:20.000000 lstmcpipe-0.9.0/production_configs/20220218_v0.9.2_prod5_trans_80_dl1ab_tune_MC_to_Crab/readme.md
+drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-10-10 08:57:12.985128 lstmcpipe-0.9.0/production_configs/20220304_v0.9.3_prod5_trans_80_zen40az180_local_tailcut_8_4/
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     1376 2022-04-13 17:39:20.000000 lstmcpipe-0.9.0/production_configs/20220304_v0.9.3_prod5_trans_80_zen40az180_local_tailcut_8_4/config_MC_prod_20220304_v0.9.3_prod5_trans_80_zen40az180_local_tailcut_8_4.yml
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     6319 2022-04-13 17:39:20.000000 lstmcpipe-0.9.0/production_configs/20220304_v0.9.3_prod5_trans_80_zen40az180_local_tailcut_8_4/lstchain_standard_config_v091_MC_Tel1.json
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)       77 2022-04-13 17:39:20.000000 lstmcpipe-0.9.0/production_configs/20220304_v0.9.3_prod5_trans_80_zen40az180_local_tailcut_8_4/readme.md
+drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-10-10 08:57:12.990345 lstmcpipe-0.9.0/production_configs/20220511_v0.9.6_allsky_std/
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)      183 2022-05-20 09:49:47.000000 lstmcpipe-0.9.0/production_configs/20220511_v0.9.6_allsky_std/README.md
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)      992 2022-05-20 09:49:47.000000 lstmcpipe-0.9.0/production_configs/20220511_v0.9.6_allsky_std/generate.py
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     6453 2022-05-20 09:49:47.000000 lstmcpipe-0.9.0/production_configs/20220511_v0.9.6_allsky_std/lstchain_84.json
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)   234487 2022-09-11 16:23:39.000000 lstmcpipe-0.9.0/production_configs/20220511_v0.9.6_allsky_std/lstmcpipe_config_20220511_allsky_std.yml
+drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-10-10 08:57:12.995314 lstmcpipe-0.9.0/production_configs/20220518_v0.9.6_allsky_dec2276_tuned/
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)      347 2022-05-20 10:24:24.000000 lstmcpipe-0.9.0/production_configs/20220518_v0.9.6_allsky_dec2276_tuned/README.md
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)      255 2022-05-20 10:24:24.000000 lstmcpipe-0.9.0/production_configs/20220518_v0.9.6_allsky_dec2276_tuned/generate.py
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     8492 2022-05-20 10:24:24.000000 lstmcpipe-0.9.0/production_configs/20220518_v0.9.6_allsky_dec2276_tuned/lstchain_config_dec_2276_tuned.json
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)    68680 2022-05-20 10:24:24.000000 lstmcpipe-0.9.0/production_configs/20220518_v0.9.6_allsky_dec2276_tuned/lstmcpipe_config_20220518_allsky_dec2276_tuned.yml
+drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-10-10 08:57:12.999094 lstmcpipe-0.9.0/production_configs/20220523_allsky_std/
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)      248 2022-06-01 16:34:15.000000 lstmcpipe-0.9.0/production_configs/20220523_allsky_std/README.md
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     8179 2022-06-01 16:34:15.000000 lstmcpipe-0.9.0/production_configs/20220523_allsky_std/lstchain_config_2022-05-23.json
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)   110282 2022-06-01 16:34:15.000000 lstmcpipe-0.9.0/production_configs/20220523_allsky_std/lstmcpipe_config_2022-05-23_PathConfigAllSkyFull.yaml
+drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-10-10 08:57:13.003612 lstmcpipe-0.9.0/production_configs/20220523_dec_413_tuned_nsb/
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     8523 2022-06-01 16:34:15.000000 lstmcpipe-0.9.0/production_configs/20220523_dec_413_tuned_nsb/lstchain_config_2022-05-23.json
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)    69249 2022-06-01 16:34:15.000000 lstmcpipe-0.9.0/production_configs/20220523_dec_413_tuned_nsb/lstmcpipe_config_2022-05-23_PathConfigAllSkyFullDL1ab.yaml
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)      499 2022-06-01 16:34:15.000000 lstmcpipe-0.9.0/production_configs/20220523_dec_413_tuned_nsb/readme.md
+drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-10-10 08:57:13.006269 lstmcpipe-0.9.0/production_configs/20220523_src3_dec3476_4822_tuned_nsb/
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     8464 2022-06-01 16:34:15.000000 lstmcpipe-0.9.0/production_configs/20220523_src3_dec3476_4822_tuned_nsb/lstchain_config_2022-05-23.json
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)   114152 2022-06-01 16:34:15.000000 lstmcpipe-0.9.0/production_configs/20220523_src3_dec3476_4822_tuned_nsb/lstmcpipe_config_2022-05-23_PathConfigAllSkyFullDL1ab.yml
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)      520 2022-06-01 16:34:15.000000 lstmcpipe-0.9.0/production_configs/20220523_src3_dec3476_4822_tuned_nsb/readme.md
+drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-10-10 08:57:13.007799 lstmcpipe-0.9.0/production_configs/20220524_dec_4822_tuned/
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)      565 2022-06-01 16:34:15.000000 lstmcpipe-0.9.0/production_configs/20220524_dec_4822_tuned/README_tuned_22_05_24.md
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     7488 2022-06-01 16:34:15.000000 lstmcpipe-0.9.0/production_configs/20220524_dec_4822_tuned/lstchain_config_2022-05-24.json
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)    66936 2022-06-01 16:34:15.000000 lstmcpipe-0.9.0/production_configs/20220524_dec_4822_tuned/lstmcpipe_config_2022-05-24_PathConfigAllSkyFullDL1ab.yaml
+drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-10-10 08:57:13.009965 lstmcpipe-0.9.0/production_configs/20220527_allsky_std_src2_diffgamma/
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)      147 2022-06-01 16:34:15.000000 lstmcpipe-0.9.0/production_configs/20220527_allsky_std_src2_diffgamma/README.md
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     7002 2022-06-01 16:34:15.000000 lstmcpipe-0.9.0/production_configs/20220527_allsky_std_src2_diffgamma/lstchain_config_2022-05-27.json
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     3311 2022-06-01 16:34:15.000000 lstmcpipe-0.9.0/production_configs/20220527_allsky_std_src2_diffgamma/lstmcpipe_config_2022-05-27_PathConfigAllSkyFull.yaml
+drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-10-10 08:57:13.011356 lstmcpipe-0.9.0/production_configs/20220531_dec3476_std/
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)      252 2022-06-01 16:34:15.000000 lstmcpipe-0.9.0/production_configs/20220531_dec3476_std/README.md
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     8225 2022-06-01 16:34:15.000000 lstmcpipe-0.9.0/production_configs/20220531_dec3476_std/lstchain_config_2022-05-31.json
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)    66650 2022-06-01 16:34:15.000000 lstmcpipe-0.9.0/production_configs/20220531_dec3476_std/lstmcpipe_config_2022-05-31_PathConfigAllSkyFull.yaml
+drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-10-10 08:57:13.013851 lstmcpipe-0.9.0/production_configs/20220601_dec3476_tuned/
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)      292 2022-06-01 16:34:15.000000 lstmcpipe-0.9.0/production_configs/20220601_dec3476_tuned/README.md
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     8464 2022-06-01 16:34:15.000000 lstmcpipe-0.9.0/production_configs/20220601_dec3476_tuned/lstchain_config_2022-06-01.json
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)    67036 2022-06-01 16:34:15.000000 lstmcpipe-0.9.0/production_configs/20220601_dec3476_tuned/lstmcpipe_config_2022-06-01_PathConfigAllSkyFullDL1ab.yaml
+drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-10-10 08:57:13.019039 lstmcpipe-0.9.0/production_configs/20220624_dec_4822_tuned_TestDIffuseGammas/
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)      683 2022-06-24 14:00:53.000000 lstmcpipe-0.9.0/production_configs/20220624_dec_4822_tuned_TestDIffuseGammas/README_tuned_22_06_24_TestDiffuseGammas.md
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     7488 2022-06-24 14:00:53.000000 lstmcpipe-0.9.0/production_configs/20220624_dec_4822_tuned_TestDIffuseGammas/lstchain_config_2022-06-24.json
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     6930 2022-06-27 15:21:35.000000 lstmcpipe-0.9.0/production_configs/20220624_dec_4822_tuned_TestDIffuseGammas/lstmcpipe_config_2022-06-24_TestDiffuseGammas.yaml
+drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-10-10 08:57:13.024437 lstmcpipe-0.9.0/production_configs/20220905_src4_high_NSB/
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     8269 2022-09-09 16:56:05.000000 lstmcpipe-0.9.0/production_configs/20220905_src4_high_NSB/lstchain_config_2022-09-05.json
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)    71199 2022-09-09 16:56:05.000000 lstmcpipe-0.9.0/production_configs/20220905_src4_high_NSB/lstmcpipe_config_2022-09-05_PathConfigAllSkyFull.yaml
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)      329 2022-09-09 16:56:05.000000 lstmcpipe-0.9.0/production_configs/20220905_src4_high_NSB/readme.md
+drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-10-10 08:57:13.026911 lstmcpipe-0.9.0/production_configs/nsb_psf_tuned_zen40_src2/
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     6583 2022-04-13 17:39:20.000000 lstmcpipe-0.9.0/production_configs/nsb_psf_tuned_zen40_src2/lstchain_config_ze40_south_NSBtuning.json
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     1319 2022-04-13 17:39:20.000000 lstmcpipe-0.9.0/production_configs/nsb_psf_tuned_zen40_src2/lstmcpipe_config.yml
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)      252 2022-04-13 17:39:20.000000 lstmcpipe-0.9.0/production_configs/nsb_psf_tuned_zen40_src2/readme.md
+drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-10-10 08:57:13.029332 lstmcpipe-0.9.0/production_configs/nsb_tuned_zen40_scr1/
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     7106 2022-04-13 17:39:20.000000 lstmcpipe-0.9.0/production_configs/nsb_tuned_zen40_scr1/lstchain_config_NSBtuning.json
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     1421 2022-04-13 17:39:20.000000 lstmcpipe-0.9.0/production_configs/nsb_tuned_zen40_scr1/lstmcpipe_config.yml
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)      232 2022-04-13 17:39:20.000000 lstmcpipe-0.9.0/production_configs/nsb_tuned_zen40_scr1/readme.md
+drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-10-10 08:57:13.031715 lstmcpipe-0.9.0/production_configs/psf_tuned_zen20/
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     7120 2022-04-13 17:39:20.000000 lstmcpipe-0.9.0/production_configs/psf_tuned_zen20/lstchain_config.json
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     1298 2022-04-13 17:39:20.000000 lstmcpipe-0.9.0/production_configs/psf_tuned_zen20/lstmcpipe_config.yml
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)      353 2022-04-13 17:39:20.000000 lstmcpipe-0.9.0/production_configs/psf_tuned_zen20/readme.md
+drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-10-10 08:57:13.034628 lstmcpipe-0.9.0/production_configs/psf_tuned_zen40/
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     7120 2022-04-13 17:39:20.000000 lstmcpipe-0.9.0/production_configs/psf_tuned_zen40/lstchain_config.json
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     1309 2022-04-13 17:39:20.000000 lstmcpipe-0.9.0/production_configs/psf_tuned_zen40/lstmcpipe_config.yml
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)      353 2022-04-13 17:39:20.000000 lstmcpipe-0.9.0/production_configs/psf_tuned_zen40/readme.md
+drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-10-10 08:57:13.036838 lstmcpipe-0.9.0/production_configs/template_prod/
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     6847 2022-09-09 16:56:38.000000 lstmcpipe-0.9.0/production_configs/template_prod/lstchain_config.json
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)      463 2022-09-09 16:56:38.000000 lstmcpipe-0.9.0/production_configs/template_prod/lstmcpipe_config.yml
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)      193 2022-09-09 16:56:38.000000 lstmcpipe-0.9.0/production_configs/template_prod/readme.md
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)       38 2022-10-10 08:57:13.038424 lstmcpipe-0.9.0/setup.cfg
+-rw-r--r--   0 thomasvuillaume   (502) staff       (20)     3069 2022-06-01 16:34:15.000000 lstmcpipe-0.9.0/setup.py
```

### Comparing `lstmcpipe-0.8.6/.github/pull_request_template.md` & `lstmcpipe-0.9.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/.github/workflows/CI.yml` & `lstmcpipe-0.9.0/.github/workflows/CI.yml`

 * *Files 9% similar despite different names*

```diff
@@ -61,21 +61,25 @@
       - name: Detect added configs
         uses: tj-actions/changed-files@v18.2
         id: verify-changed-files
         with:
           files: |
             production_configs/*/*.yml
             production_configs/*/*.yaml
-            production_configs/*/*.json
+            # production_configs/*/*.json
+            # TODO: solve issue in github actions extracting sublist of yaml files, see below
+
       - name: Validate added configs.
         if: steps.verify-changed-files.outputs.any_changed == 'true'
         run: |
           source $CONDA/etc/profile.d/conda.sh
           conda activate ci
           export filelist="${{ steps.verify-changed-files.outputs.all_changed_files }}"
-          export filelist=`grep -E '\.yaml$|\.yml$' <<< ${filelist[*]}`
+          # export filelist=`grep -P '\.yaml$|\.yml$' <<< ${filelist[*]}`
+          # the above line works on ubuntu but fails on github action, not following the given pattern
           echo "Added yaml files: $filelist"
           for file in $filelist; do
-            echo "Checking $file...";
+            echo "Checking $file";
+            echo "lstmcpipe_validate_config $file -lc `dirname $file`/*lstchain*.json"
             lstmcpipe_validate_config $file -lc `dirname $file`/*lstchain*.json ;
             echo "Valid!";
-          done
+          done
```

### Comparing `lstmcpipe-0.8.6/.github/workflows/codemeta2citation.yml` & `lstmcpipe-0.9.0/.github/workflows/codemeta2citation.yml`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/.github/workflows/dev/codemeta2citation.py` & `lstmcpipe-0.9.0/.github/workflows/dev/codemeta2citation.py`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/.github/workflows/docs.yml` & `lstmcpipe-0.9.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/.pre-commit-config.yaml` & `lstmcpipe-0.9.0/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 repos:
 - repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v3.2.0
+  rev: v4.3.0
   hooks:
     - id: trailing-whitespace
     - id: end-of-file-fixer
     - id: check-yaml
     - id: check-added-large-files
     - id: check-merge-conflict
     - id: check-json
 
 - repo: https://github.com/psf/black
-  rev: stable
+  rev: 22.8.0
   hooks:
   - id: black
     language_version: python3
     args:
       - --line-length=120
       - --skip-string-normalization
       - --exclude="""\.git |
         \.__pycache__|
         build"""
 
--   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v1.2.3
-    hooks:
-    - id: flake8
-      language_version: python3
-      args:
-        - "--max-line-length=120"
+- repo: https://gitlab.com/pycqa/flake8
+  rev: 3.9.2
+  hooks:
+  - id: flake8
+    language_version: python3
+    args:
+      - "--max-line-length=120"
```

### Comparing `lstmcpipe-0.8.6/.pylintrc` & `lstmcpipe-0.9.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/CITATION.cff` & `lstmcpipe-0.9.0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/PKG-INFO` & `lstmcpipe-0.9.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lstmcpipe
-Version: 0.8.6
+Version: 0.9.0
 Summary: Scripts to ease the reduction of MC data on the LST cluster at La Palma. With this package, the analysis/creation of R1/DL0/DL1/DL2/IRFs can be orchestrated.
 Home-page: https://github.com/cta-observatory/lstmcpipe
 Author: Thomas Vuillaume,Enrique Garcia,Lukas Nickel,
 Author-email: thomas.vuillaume@lapp.in2p3.fr
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lstmcpipe-0.8.6/README.rst` & `lstmcpipe-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/codemeta.json` & `lstmcpipe-0.9.0/codemeta.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9047619047619048%*

 * *Differences: {"'datePublished'": "'2022-10-10'",*

 * * "'downloadUrl'": "'https://github.com/cta-observatory/lstmcpipe/archive/refs/tags/v0.9.0.tar.gz'",*

 * * "'releaseNotes'": "'**Full Changelog**: "*

 * *                   "https://github.com/cta-observatory/lstmcpipe/compare/v0.8.6...v0.9.0'",*

 * * "'version'": "'0.9.0'"}*

```diff
@@ -35,18 +35,18 @@
             "email": "lukas.nickel@tu-dortmund.de",
             "familyName": "Nickel",
             "givenName": "Lukas"
         }
     ],
     "codeRepository": "git+https://github.com/cta-observatory/lstmcpipe.git",
     "dateCreated": "2019-09-09",
-    "datePublished": "2022-05-31",
+    "datePublished": "2022-10-10",
     "description": "Scripts to ease the reduction of MC data on the LST cluster at La Palma. With this package, the analysis/creation of R1/DL0/DL1/DL2/IRFs can be orchestrated.",
     "developmentStatus": "active",
-    "downloadUrl": "https://github.com/cta-observatory/lstmcpipe/archive/refs/tags/v0.8.5.tar.gz",
+    "downloadUrl": "https://github.com/cta-observatory/lstmcpipe/archive/refs/tags/v0.9.0.tar.gz",
     "funder": {
         "@type": "Organization",
         "name": "European Union\u2019s Horizon 2020 research and innovation programme"
     },
     "funding": "824064",
     "isPartOf": "https://www.cta-observatory.org/",
     "issueTracker": "https://github.com/cta-observatory/lstmcpipe/issues",
@@ -68,10 +68,10 @@
         "familyName": "Garcia",
         "givenName": "Enrique"
     },
     "name": "lstmcpipe",
     "programmingLanguage": [
         "Python 3"
     ],
-    "releaseNotes": "**Full Changelog**: https://github.com/cta-observatory/lstmcpipe/compare/v0.8.4...v0.8.5",
-    "version": "0.8.5"
+    "releaseNotes": "**Full Changelog**: https://github.com/cta-observatory/lstmcpipe/compare/v0.8.6...v0.9.0",
+    "version": "0.9.0"
 }
```

### Comparing `lstmcpipe-0.8.6/docs/Makefile` & `lstmcpipe-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/docs/conf.py` & `lstmcpipe-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/docs/make.bat` & `lstmcpipe-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/docs/pipeline.rst` & `lstmcpipe-0.9.0/docs/pipeline.rst`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/docs/produce_config_page.py` & `lstmcpipe-0.9.0/docs/produce_config_page.py`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/license.rst` & `lstmcpipe-0.9.0/license.rst`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/lstmcpipe/base_config_lstmcpipe.yaml` & `lstmcpipe-0.9.0/lstmcpipe/base_config_lstmcpipe.yaml`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/lstmcpipe/benchmarks/irfs.py` & `lstmcpipe-0.9.0/lstmcpipe/benchmarks/irfs.py`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/lstmcpipe/config/__init__.py` & `lstmcpipe-0.9.0/lstmcpipe/config/__init__.py`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/lstmcpipe/config/dl1ab_tuning.py` & `lstmcpipe-0.9.0/lstmcpipe/config/dl1ab_tuning.py`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/lstmcpipe/config/paths_config.py` & `lstmcpipe-0.9.0/lstmcpipe/config/paths_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/env python
 
 import os
+import warnings
 from pathlib import Path
 from ruamel.yaml import YAML
 from datetime import date
 import re
 import numpy as np
 import astropy.units as u
 from astropy.table import QTable, join
@@ -626,30 +627,34 @@
             dl1 = self.dl1_dir(particle, '')
             merged_dl1 = self.training_merged_dl1(particle)
             paths.append(
                 {
                     'input': dl1,
                     'output': merged_dl1,
                     'options': '--pattern */*.h5 --no-image',
-                    'slurm_options': '-p long',
+                    'extra_slurm_options': {'partition': 'long'},
                 }
             )
         return paths
 
     @property
     def train_pipe(self):
         paths = [
             {
                 'input': {
                     'gamma': self.training_merged_dl1('GammaDiffuse'),
                     'proton': self.training_merged_dl1('Protons'),
                 },
                 'output': self.models_dir(),
-                'slurm_options': '-p xxl --mem=160G --cpus-per-task=16' if self.dec == _crab_dec
-                else '-p xxl --mem=100G --cpus-per-task=16',
+                'extra_slurm_options': {'partition': 'xxl',
+                                        'mem': '160G',
+                                        'cpus-per-task': 16} if self.dec == _crab_dec
+                else {'partition': 'xxl',
+                      'mem': '100G',
+                      'cpus-per-task': 16}
             }
         ]
         return paths
 
 
 class PathConfigAllSkyTesting(PathConfigAllSkyBase):
     def __init__(self, prod_id, dec):
@@ -789,15 +794,15 @@
         paths = []
         for pointing in self.pointing_dirs():
             paths.append(
                 {
                     'input': self.testing_merged_dl1(pointing),
                     'path_model': self.models_dir(),
                     'output': self.dl2_dir(pointing),
-                    'slurm_options': '--mem=80GB' if self.dec == _crab_dec else '--mem=60GB'
+                    'extra_slurm_options': {'mem': '80GB' if self.dec == _crab_dec else '60GB'}
                 }
             )
         return paths
 
     def dl2_output_file(self, pointing):
         filename = os.path.basename(self.testing_merged_dl1(pointing).replace('dl1_', 'dl2_'))
         return os.path.join(self.dl2_dir(pointing), filename)
@@ -812,15 +817,15 @@
                     'input': {
                         'gamma_file': self.dl2_output_file(pointing),
                         'proton_file': None,
                         'electron_file': None,
                     },
                     'output': os.path.join(self.irf_dir(pointing), f'irf_{self.prod_id}_{pointing}.fits.gz'),
                     'options': '--point-like',
-                    'slurm_options': '--mem=6GB'
+                    'extra_slurm_options': {'mem':'6GB'}
                 }
             )
 
         return paths
 
 
 class PathConfigAllSkyFull(PathConfig):
@@ -931,19 +936,23 @@
         self.stages = ['dl1ab', 'merge_dl1', 'train_pipe']
         self.source_prod_id = source_prod_id
         self.source_config = PathConfigAllSkyTraining(source_prod_id, dec)
         if run_checker:
             self.check_source_prod()
         
     def check_source_prod(self):
+        marked_for_removal = []
         for particle in self.training_particles:
-            for pointing in self.pointing_dirs(particle):
+            for pidx, pointing in enumerate(self.pointing_dirs(particle)):
                 source_dl1 = Path(self.source_config.dl1_dir(particle, pointing))
                 if not source_dl1.exists():
-                    raise FileNotFoundError(f"{source_dl1} should exist to run this DL1ab")
+                    warnings.warn(f"{source_dl1} does not exist but MC file for {particle} - {pointing} does. "
+                                  f"This node will be removed from production.")
+                    marked_for_removal.append(pidx)
+        self._training_pointings.remove_rows(pidx)
 
     @property
     def dl1ab(self):
         paths = []
         for particle in self.training_particles:
             for pointing in self.pointing_dirs(particle):
                 source_dl1 = self.source_config.dl1_dir(particle, pointing)
@@ -972,18 +981,22 @@
         self.stages = ['dl1ab', 'merge_dl1', 'dl1_to_dl2', 'dl2_to_irfs']
         self.source_prod_id = source_prod_id
         self.source_config = PathConfigAllSkyTesting(source_prod_id, dec)
         if run_checker:
             self.check_source_prod()
         
     def check_source_prod(self):
-        for pointing in self.pointing_dirs():
+        marked_for_removal = []
+        for pidx, pointing in enumerate(self.pointing_dirs()):
             source_dl1 = Path(self.source_config.dl1_dir(pointing))
             if not source_dl1.exists():
-                raise FileNotFoundError(f"{source_dl1} should exist to run this DL1ab")
+                warnings.warn(f"{source_dl1} does not exist but MC file for {pointing} does. "
+                              f"This node will be removed from production.")
+                marked_for_removal.append(pidx)
+        self._testing_pointings.remove_rows(marked_for_removal)
 
     @property
     def dl1ab(self):
         paths = []
         for pointing in self.pointing_dirs():
             source_dl1 = self.source_config.dl1_dir(pointing)
             target_dl1 = self.dl1_dir(pointing)
```

### Comparing `lstmcpipe-0.8.6/lstmcpipe/config/pipeline_config.py` & `lstmcpipe-0.9.0/lstmcpipe/config/pipeline_config.py`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/lstmcpipe/config/tests/test_paths_config.py` & `lstmcpipe-0.9.0/lstmcpipe/config/tests/test_paths_config.py`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/lstmcpipe/config/tests/test_pipeline_config.py` & `lstmcpipe-0.9.0/lstmcpipe/config/tests/test_pipeline_config.py`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/lstmcpipe/hiperta/hiperta_r0_to_dl1lstchain.py` & `lstmcpipe-0.9.0/lstmcpipe/hiperta/hiperta_r0_to_dl1lstchain.py`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/lstmcpipe/hiperta/reorganize_dl1hiperta300_to_dl1lstchain060.py` & `lstmcpipe-0.9.0/lstmcpipe/hiperta/reorganize_dl1hiperta300_to_dl1lstchain060.py`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/lstmcpipe/hiperta/reorganize_dl1hiperta_to_dl1lstchain.py` & `lstmcpipe-0.9.0/lstmcpipe/hiperta/reorganize_dl1hiperta_to_dl1lstchain.py`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/lstmcpipe/io/data_management.py` & `lstmcpipe-0.9.0/lstmcpipe/io/data_management.py`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/lstmcpipe/io/lstmcpipe_tree_path.py` & `lstmcpipe-0.9.0/lstmcpipe/io/lstmcpipe_tree_path.py`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/lstmcpipe/io/tests/test_data_management.py` & `lstmcpipe-0.9.0/lstmcpipe/io/tests/test_data_management.py`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/lstmcpipe/io/tests/test_lstmcpipe_tree_path.py` & `lstmcpipe-0.9.0/lstmcpipe/io/tests/test_lstmcpipe_tree_path.py`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/lstmcpipe/logging.py` & `lstmcpipe-0.9.0/lstmcpipe/logging.py`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/lstmcpipe/lstmcpipe_start.py` & `lstmcpipe-0.9.0/lstmcpipe/lstmcpipe_start.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     batch_train_pipe,
     batch_dl1_to_dl2,
     batch_dl2_to_irfs,
     batch_dl2_to_sensitivity,
     batch_plot_rf_features,
 )
 
-
 parser = argparse.ArgumentParser(description="MC R0 to DL3 full pipeline")
 
 parser.add_argument(
     "--config_mc_prod",
     "-c",
     action="store",
     type=str,
@@ -67,26 +66,26 @@
 parser.add_argument(
     "--config_file_ctapipe",
     "-conf_cta",
     action="store",
     type=str,
     dest="config_file_ctapipe",
     help="Path to a ctapipe-like configuration file."
-    'Only to be declared if WORKFLOW_KIND = "ctapipe" and only used up to dl1.',
+         'Only to be declared if WORKFLOW_KIND = "ctapipe" and only used up to dl1.',
     default=None,
 )
 
 parser.add_argument(
     "--config_file_rta",
     "-conf_rta",
     action="store",
     type=str,
     dest="config_file_rta",
     help="Path to a HiPeRTA-like configuration file."
-    'Only to be declared if WORKFLOW_KIND = "hiperta" and only used up to dl1.',
+         'Only to be declared if WORKFLOW_KIND = "hiperta" and only used up to dl1.',
     default=None,
 )
 
 parser.add_argument("--debug", action="store_true", help="print debug messages to stderr")
 parser.add_argument(
     "--log-file",
     action="store",
@@ -94,14 +93,15 @@
     dest="log_file",
     help="Optional log file. This is independent of the slurm job logs and only handles lstmcpipe logging",
     default=None,
 )
 
 args = parser.parse_args()
 
+
 #######################################################################################################################
 
 
 def main():
     """
     Main lstmcpipe script. This will launch the selected stages and start the processing.
     The jobs are submitted, but not awaited meaning that the analysis will be going on after
@@ -237,19 +237,24 @@
         all_job_ids.update({"plot_rf_feat": job_from_plot_rf_feat})
 
     else:
         job_from_train_pipe = None
 
     # 4 STAGE --> DL1 to DL2 stage
     if "dl1_to_dl2" in stages_to_run:
+        jobs_dependency_for_dl1_dl2 = jobs_from_merge
+        if job_from_train_pipe is not None:
+            jobs_dependency_for_dl1_dl2 = ','.join([jobs_dependency_for_dl1_dl2,
+                                                    job_from_train_pipe]) if jobs_dependency_for_dl1_dl2 is not None \
+                else job_from_train_pipe
 
         jobs_from_dl1_dl2 = batch_dl1_to_dl2(
             lstmcpipe_config['stages']['dl1_to_dl2'],
             Path(args.config_file_lst).resolve().as_posix(),
-            job_from_train_pipe,  # Single jobid from train
+            jobs_dependency_for_dl1_dl2,
             batch_config=batch_config,
             logs=logs_files,
         )
 
         update_scancel_file(scancel_file, jobs_from_dl1_dl2)
         all_job_ids.update({"dl1_to_dl2": jobs_from_dl1_dl2})
     else:
```

### Comparing `lstmcpipe-0.8.6/lstmcpipe/metrics/__init__.py` & `lstmcpipe-0.9.0/lstmcpipe/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/lstmcpipe/plots/images_debug.py` & `lstmcpipe-0.9.0/lstmcpipe/plots/images_debug.py`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/lstmcpipe/plots/plot_irfs.py` & `lstmcpipe-0.9.0/lstmcpipe/plots/plot_irfs.py`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/lstmcpipe/plots/plot_models_importance.py` & `lstmcpipe-0.9.0/lstmcpipe/plots/plot_models_importance.py`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/lstmcpipe/plots/pointings.py` & `lstmcpipe-0.9.0/lstmcpipe/plots/pointings.py`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/lstmcpipe/scripts/generate_test_lapalma.py` & `lstmcpipe-0.9.0/lstmcpipe/scripts/generate_test_lapalma.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,21 +101,21 @@
         pcdl1ab.test_configs[dec].source_config.testing_dir = os.path.join(
             working_dir, pc.test_configs[dec].testing_dir.replace(allsky_test_base_dir, 'DL0/AllSky/')
         )
         
     pc.generate()
     for stage_name, stage_steps in pc.paths.items():
         for step in stage_steps:
-            step['slurm_options'] = '-p short'
+            step['extra_slurm_options'] = {'partition': 'short'}
     pc.save_yml(os.path.join(path_to_config_file, f'test_AllSky_{date.today()}.yaml'), overwrite=overwrite)
     
     pcdl1ab.generate()
     for stage_name, stage_steps in pcdl1ab.paths.items():
         for step in stage_steps:
-            step['slurm_options'] = '-p short'
+            step['extra_slurm_options'] = {'partition': 'short'}
     pcdl1ab.save_yml(os.path.join(path_to_config_file, f'test_AllSky_{date.today()}_dl1ab.yaml'), overwrite=overwrite)
 
 
 
 if __name__ == '__main__':
 
     parser = argparse.ArgumentParser(description='Generate test tree')
```

### Comparing `lstmcpipe-0.8.6/lstmcpipe/scripts/lstmcpipe_generate_config.py` & `lstmcpipe-0.9.0/lstmcpipe/scripts/lstmcpipe_generate_config.py`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/lstmcpipe/scripts/script_batch_filelist_cta.py` & `lstmcpipe-0.9.0/lstmcpipe/scripts/script_batch_filelist_cta.py`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/lstmcpipe/scripts/script_batch_filelist_lst.py` & `lstmcpipe-0.9.0/lstmcpipe/scripts/script_batch_filelist_lst.py`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/lstmcpipe/scripts/script_batch_filelist_lst_dl1ab.py` & `lstmcpipe-0.9.0/lstmcpipe/scripts/script_batch_filelist_lst_dl1ab.py`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/lstmcpipe/scripts/script_batch_filelist_rta.py` & `lstmcpipe-0.9.0/lstmcpipe/scripts/script_batch_filelist_rta.py`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/lstmcpipe/scripts/script_compare_irfs.py` & `lstmcpipe-0.9.0/lstmcpipe/scripts/script_compare_irfs.py`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/lstmcpipe/scripts/script_dl2_to_sensitivity.py` & `lstmcpipe-0.9.0/lstmcpipe/scripts/script_dl2_to_sensitivity.py`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/lstmcpipe/scripts/script_lstmcpipe_validate_config.py` & `lstmcpipe-0.9.0/lstmcpipe/scripts/script_lstmcpipe_validate_config.py`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/lstmcpipe/scripts/script_train_test_splitting.py` & `lstmcpipe-0.9.0/lstmcpipe/scripts/script_train_test_splitting.py`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/lstmcpipe/scripts/tests/test_scripts.py` & `lstmcpipe-0.9.0/lstmcpipe/scripts/tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/lstmcpipe/scripts/useful_tmp_scripts/clean_corrupted_dl1_dirs_allSky.py` & `lstmcpipe-0.9.0/lstmcpipe/scripts/useful_tmp_scripts/clean_corrupted_dl1_dirs_allSky.py`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/lstmcpipe/scripts/useful_tmp_scripts/cleandir.py` & `lstmcpipe-0.9.0/lstmcpipe/scripts/useful_tmp_scripts/cleandir.py`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/lstmcpipe/scripts/useful_tmp_scripts/rerun_irfs_mem_issue.py` & `lstmcpipe-0.9.0/lstmcpipe/scripts/useful_tmp_scripts/rerun_irfs_mem_issue.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Run python rerun_irfs_mem_issue.py lstmcpipe_config.yaml
 """
+
 from ruamel.yaml import YAML
 import sys
 from pathlib import Path
 
 
 yaml = YAML()
 
@@ -18,21 +19,21 @@
 cfg['stages'].pop('train_pipe', None)
 cfg['stages'].pop('dl1_to_dl2', None)
 
 to_rerun = []
 for p in cfg['stages']['dl2_to_irfs']:
     if not Path(p['output']).is_file():
         print(p['output'])
-        p['slurm_options'] = '--mem=6GB'
+        p['extra_slurm_options'] = {'mem':'6GB'}
         to_rerun.append(p)
 
 cfg['stages']['dl2_to_irfs'] = to_rerun
 print(f"{len(to_rerun)} irfs to re-produce")
 
 
-output_filename = filename.parent.joinpath(filename.stem + '_rerun.yaml')
+output_filename = filename.parent.joinpath(f'{filename.stem}_rerun.yaml')
 
 if to_rerun and not Path(output_filename).exists():
     print(f"Run lstmcpipe -c {output_filename}")
     yaml.dump(cfg, open(output_filename, 'w'))
 elif Path(output_filename).exists():
     raise FileExistsError(output_filename)
```

### Comparing `lstmcpipe-0.8.6/lstmcpipe/stages/__init__.py` & `lstmcpipe-0.9.0/lstmcpipe/stages/__init__.py`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/lstmcpipe/stages/mc_dl1_to_dl2.py` & `lstmcpipe-0.9.0/lstmcpipe/stages/mc_dl1_to_dl2.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,25 +2,18 @@
 
 import shutil
 import logging
 from pathlib import Path
 from ..utils import save_log_to_file, SbatchLstMCStage
 from ..io.data_management import check_and_make_dir_without_verification
 
-
 log = logging.getLogger(__name__)
 
 
-def batch_dl1_to_dl2(
-    dict_paths,
-    config_file,
-    jobid_from_training,
-    batch_config,
-    logs,
-):
+def batch_dl1_to_dl2(dict_paths, config_file, jobid_from_training, batch_config, logs):
     """
     Function to batch the dl1_to_dl2 stage once the lstchain train_pipe batched jobs have finished.
 
     Parameters
     ----------
     dict_paths : dict
         Core dictionary with {stage: PATHS} information
@@ -37,57 +30,48 @@
 
     Returns
     -------
     jobid_for_dl2_to_dl3 : str
         string containing the jobids to be passed to the next stage of the workflow (as a slurm dependency)
 
     """
-
     log_dl1_to_dl2 = {}
     jobid_for_dl2_to_dl3 = []
     debug_log = {}
-
-    log.info("==== START {} ==== \n".format("batch dl1_to_dl2_workflow"))
-
+    log.info("==== START batch dl1_to_dl2_workflow ==== \n")
     for paths in dict_paths:
-
         job_logs, jobid = dl1_to_dl2(
             paths["input"],
             paths["output"],
             path_models=paths["path_model"],
             config_file=config_file,
             wait_jobid_train_pipe=jobid_from_training,
             batch_configuration=batch_config,
-            slurm_options=paths.get("slurm_options", None),
+            extra_slurm_options=paths.get("extra_slurm_options", None),
         )
 
         log_dl1_to_dl2.update(job_logs)
-
-        # Single particle dl1_dl2 jobid to be appended
         jobid_for_dl2_to_dl3.append(jobid)
         debug_log[jobid] = f"dl1_to_dl2 jobid that depends on : {jobid_from_training} training job"
 
     jobid_for_dl2_to_dl3 = ",".join(jobid_for_dl2_to_dl3)
-
     save_log_to_file(log_dl1_to_dl2, logs["log_file"], workflow_step="dl1_to_dl2")
     save_log_to_file(debug_log, logs["debug_file"], workflow_step="dl1_to_dl2")
-
-    log.info("==== END {} ====".format("batch dl1_to_dl2_workflow"))
-
+    log.info("==== END batch dl1_to_dl2_workflow ====")
     return jobid_for_dl2_to_dl3
 
 
 def dl1_to_dl2(
     input_file,
     output_dir,
     path_models,
     config_file,
     wait_jobid_train_pipe=None,
     batch_configuration='',
-    slurm_options=None,
+    extra_slurm_options=None,
 ):
     """
     Convert onsite files from dl1 to dl2
 
     Parameters
     ----------
     input_file : str
@@ -101,50 +85,42 @@
     wait_jobid_train_pipe : str
         Comma-separated string with the batched jobid from the train stage to indicate the
         dependencies of the current job to be batched
     batch_configuration : dict
         Dictionary containing the (full) source_environment and the slurm_account strings
         to be passed to the sbatch commands
         ! NOTE : train_pipe AND dl1_to_dl2 MUST BE RUN WITH THE SAME ENVIRONMENT
-    slurm_options: str
+    extra_slurm_options: dict
         Extra slurm options to be passed to the sbatch command
 
     Returns
     -------
     log_dl1_to_dl2 : dict
         log dictionary containing {jobid: batch_cmd} information
 
     jobid_dl1_to_dl2 : str
         batched job_id to be passed to later stages
 
     """
-    log.info("Working on DL1 files in {}".format(Path(input_file).parent.as_posix()))
-
+    log.info(f"Working on DL1 files in {Path(input_file).parent.as_posix()}")
     check_and_make_dir_without_verification(output_dir)
-    log.info("Output dir: {}".format(output_dir))
-
-    log_dl1_to_dl2 = {}
-
-    cmd = f"lstchain_dl1_to_dl2 -f {input_file} -p {path_models}" f" -o {output_dir}"
+    log.info(f"Output dir: {output_dir}")
+    cmd = f"lstchain_dl1_to_dl2 -f {input_file} -p {path_models} -o {output_dir}"
     if config_file is not None:
         cmd += f" -c {Path(config_file).resolve().as_posix()}"
-
     sbatch_dl1_dl2 = SbatchLstMCStage(
-        "dl1_to_dl2",  # default: -p short --mem=32G
+        "dl1_to_dl2",
         wrap_command=cmd,
         slurm_error=Path(output_dir).joinpath("dl1_dl2-%j.e").resolve().as_posix(),
         slurm_output=Path(output_dir).joinpath("dl1_dl2-%j.o").resolve().as_posix(),
-        slurm_deps=wait_jobid_train_pipe,
-        slurm_options=slurm_options,
+        slurm_dependencies=wait_jobid_train_pipe,
+        extra_slurm_options=extra_slurm_options,
         slurm_account=batch_configuration["slurm_account"],
         source_environment=batch_configuration["source_environment"],
     )
 
     jobid_dl1_to_dl2 = sbatch_dl1_dl2.submit()
-    log_dl1_to_dl2.update({jobid_dl1_to_dl2: sbatch_dl1_dl2.slurm_command})
-
+    log_dl1_to_dl2 = {jobid_dl1_to_dl2: sbatch_dl1_dl2.slurm_command}
     log.info(f"Submitted batch job {jobid_dl1_to_dl2}")
-
     if config_file is not None:
         shutil.copyfile(config_file, Path(output_dir).joinpath(Path(config_file).name))
-
     return log_dl1_to_dl2, jobid_dl1_to_dl2
```

### Comparing `lstmcpipe-0.8.6/lstmcpipe/stages/mc_dl2_to_irfs.py` & `lstmcpipe-0.9.0/lstmcpipe/stages/mc_dl2_to_irfs.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,21 +9,15 @@
 from ..utils import save_log_to_file, SbatchLstMCStage
 from ..io.data_management import check_and_make_dir_without_verification
 
 
 log = logging.getLogger(__name__)
 
 
-def batch_dl2_to_irfs(
-    dict_paths,
-    config_file,
-    job_ids_from_dl1_dl2,
-    batch_config,
-    logs,
-):
+def batch_dl2_to_irfs(dict_paths, config_file, job_ids_from_dl1_dl2, batch_config, logs):
     """
     Batches the dl2_to_irfs stage (lstchain lstchain_create_irf_files script) once the dl1_to_dl2 stage had finished.
 
     Parameters
     ----------
     dict_paths : dict
         Core dictionary with {stage: PATHS} information
@@ -39,59 +33,59 @@
         Dictionary with logs files
 
     Returns
     -------
     jobs_from_dl2_irf: str
         Comma-separated jobids batched in the current stage
     """
-    log.info("==== START {} ====".format("batch mc_dl2_to_irfs"))
+    log.info("==== START batch mc_dl2_to_irfs ====")
 
     log_dl2_to_irfs = {}
     jobid_for_check = []
     debug_log = {}
 
     for paths in dict_paths:
         job_logs, jobid = dl2_to_irfs(
             paths["input"]["gamma_file"],  # gamma_file must always be provided
             paths["input"].get("electron_file", None),  # electron_file might be missing in case of point-like IRFs
-            paths["input"].get("proton_file", None),   # proton_file might be missing in case of point-like IRFs
+            paths["input"].get("proton_file", None),  # proton_file might be missing in case of point-like IRFs
             paths["output"],
             config_file=config_file,
             options=paths.get("options", None),
             batch_configuration=batch_config,
             wait_jobs_dl1dl2=job_ids_from_dl1_dl2,
-            slurm_options=paths.get("slurm_options", None),
+            extra_slurm_options=paths.get("extra_slurm_options", None),
         )
 
         log_dl2_to_irfs.update(log_dl2_to_irfs)
         jobid_for_check.append(jobid)
         debug_log[jobid] = (
             f"jobid from dl2_to_irfs stage that depends of the dl1_to_dl2 stage " f"job_ids; {job_ids_from_dl1_dl2}"
         )
 
     jobid_for_check = ",".join(jobid_for_check)
 
     save_log_to_file(log_dl2_to_irfs, logs["log_file"], workflow_step="dl2_to_irfs")
     save_log_to_file(debug_log, logs["debug_file"], workflow_step="dl2_to_irfs")
 
-    log.info("==== END {} ====".format("batch mc_dl2_to_irfs"))
+    log.info("==== END batch mc_dl2_to_irfs ====")
 
     return jobid_for_check
 
 
 def dl2_to_irfs(
     gamma_file,
     electron_file,
     proton_file,
     outfile,
     config_file,
     options,
     batch_configuration,
     wait_jobs_dl1dl2,
-    slurm_options=None,
+    extra_slurm_options=None,
 ):
     """
     Batches interactively the lstchain `lstchain_create_irf_files` entry point.
 
     Parameters
     ----------
     gamma_file: str
@@ -105,15 +99,15 @@
         Most common: --irf-point-like
     batch_configuration : dict
         Dictionary containing the (full) source_environment and the slurm_account strings to be passed to the
         sbatch commands
     wait_jobs_dl1dl2: str
         Comma separated string with the job ids of previous stages (dl1_to_dl2 stage) to be passed as dependencies to
         the create_irfs_files job to be batched.
-    slurm_options: str
+    extra_slurm_options: dict
         Extra slurm options to be passed to the sbatch command
 
     Returns
     -------
     log_dl2_to_irfs: dict
         Dictionary-wise log containing {'job_id': 'batched_cmd'} items
     job_id_dl2_irfs: str
@@ -136,16 +130,16 @@
     log.info(f"Output dir IRF of {gamma_file}: {output_dir}")
 
     sbatch_dl2_irfs = SbatchLstMCStage(
         "dl2_to_irfs",
         wrap_command=cmd,
         slurm_error=Path(output_dir).joinpath("job_dl2_to_irfs-%j.e").resolve().as_posix(),
         slurm_output=Path(output_dir).joinpath("job_dl2_to_irfs-%j.o").resolve().as_posix(),
-        slurm_deps=wait_jobs_dl1dl2,
-        slurm_options=slurm_options,
+        slurm_dependencies=wait_jobs_dl1dl2,
+        extra_slurm_options=extra_slurm_options,
         slurm_account=batch_configuration["slurm_account"],
         source_environment=batch_configuration["source_environment"],
     )
 
     job_id_dl2_irfs = sbatch_dl2_irfs.submit()
     log_dl2_to_irfs.update({job_id_dl2_irfs: sbatch_dl2_irfs.slurm_command})
```

### Comparing `lstmcpipe-0.8.6/lstmcpipe/stages/mc_dl2_to_sensitivity.py` & `lstmcpipe-0.9.0/lstmcpipe/stages/mc_dl2_to_sensitivity.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,17 @@
 #!/usr/bin/env python
 
 import logging
 from pathlib import Path
 from ..utils import save_log_to_file, SbatchLstMCStage
 
-
 log = logging.getLogger(__name__)
 
 
-def batch_dl2_to_sensitivity(
-    dict_paths,
-    job_ids_from_dl1_dl2,
-    batch_config,
-    logs,
-):
+def batch_dl2_to_sensitivity(dict_paths, job_ids_from_dl1_dl2, batch_config, logs):
     """
     Batches the dl2_to_sensitivity stage (`stages.script_dl2_to_sensitivity` based in the pyIRF iib) once the
     dl1_to_dl2 stage had finished.
 
     Parameters
     ----------
     dict_paths : dict
@@ -32,120 +26,102 @@
         Dictionary with logs files
 
     Returns
     -------
     jobid_for_check: str
         Comma-separated jobids batched in the current stage
     """
-    log.info("==== START {} ====".format("batch mc_dl2_to_sensitivity"))
-
+    log.info('==== START batch mc_dl2_to_sensitivity ====')
     log_dl2_to_sensitivity = {}
     jobid_for_check = []
     debug_log = {}
-
     for paths in dict_paths:
         job_logs, jobid = dl2_to_sensitivity(
             paths["input"],
             paths["output"],
             batch_configuration=batch_config,
             wait_jobs_dl1_dl2=job_ids_from_dl1_dl2,
-            slurm_options=paths.get("slurm_options", None),
+            extra_slurm_options=paths.get("extra_slurm_options", None),
         )
+
         jobid_for_check.append(jobid)
         log_dl2_to_sensitivity.update(job_logs)
         debug_log[jobid] = (
-            f"Job_ids from the dl2_to_sensitivity stage and the plot_irfs script that "
-            f"depends on the dl1_to_dl2 stage job_ids; {job_ids_from_dl1_dl2}"
+            f"Job_ids from the dl2_to_sensitivity stage and the plot_irfs script that depends on the "
+            f"dl1_to_dl2 stage job_ids; {job_ids_from_dl1_dl2} "
         )
 
     jobid_for_check = ",".join(jobid_for_check)
-
     save_log_to_file(log_dl2_to_sensitivity, logs["log_file"], "dl2_to_sensitivity")
-    save_log_to_file(debug_log, logs["debug_file"], "dl2_to_sensitivity")
-
-    log.info("==== END {} ====".format("batch mc_dl2_to_sensitivity"))
 
+    save_log_to_file(debug_log, logs["debug_file"], "dl2_to_sensitivity")
+    log.info('==== END batch mc_dl2_to_sensitivity ====')
     return jobid_for_check
 
 
-def dl2_to_sensitivity(
-    input_paths,
-    output,
-    batch_configuration,
-    wait_jobs_dl1_dl2,
-    slurm_options=None,
-):
+def dl2_to_sensitivity(input_paths, output, batch_configuration, wait_jobs_dl1_dl2, extra_slurm_options=None):
     """
     Function to run the `script_dl2_to_sensitivity` for the gamma (and the different gamma offsets) and gamma-diffuse
     particles.
     Creates the sensitivity *.fits.gz files and the corresponding sensitivity curve plot.
 
     Parameters
     ----------
     input_paths: dict
     output: str
     batch_configuration : dict
         Dictionary containing the (full) source_environment and the slurm_account strings to be passed to the
         sbatch commands
     wait_jobs_dl1_dl2: str
         Comma-separated string with the jobs (dependency) to wait for before launching the cmd
-    slurm_options: str
+    extra_slurm_options: dict
         Extra slurm options to be passed to the sbatch command
 
     Returns
     -------
     log_dl2_to_sensitivity: dict
         Dictionary with job_id-slurm command key-value pair used for logging
     job_id: str
         String with job_ids batched by the dl2_to_sensitivity script
 
     """
-    log_dl2_to_sensitivity = {}
-    jobids_dl2_to_sensitivity = []
-
     g_file = input_paths["gamma_file"]
     p_file = input_paths["proton_file"]
     e_file = input_paths["electron_file"]
-
     cmd_sens = f"lstmcpipe_dl2_to_sensitivity -g {g_file} -p {p_file} -e {e_file} -o {output}"
 
     sbatch_dl2_sens = SbatchLstMCStage(
-        "dl2_sens",  # --partition=short --mem=32G
+        "dl2_sens",
         wrap_command=cmd_sens,
         slurm_error=Path(output).parent.joinpath("job_dl2_to_sensitivity.e"),
         slurm_output=Path(output).parent.joinpath("job_dl2_to_sensitivity.o"),
-        slurm_deps=wait_jobs_dl1_dl2,
-        slurm_options=slurm_options,
+        slurm_dependencies=wait_jobs_dl1_dl2,
+        extra_slurm_options=extra_slurm_options,
         slurm_account=batch_configuration["slurm_account"],
         source_environment=batch_configuration["source_environment"],
     )
 
     job_id_dl2_sens = sbatch_dl2_sens.submit()
-    log_dl2_to_sensitivity.update({job_id_dl2_sens: job_id_dl2_sens.slurm_command})
-    jobids_dl2_to_sensitivity.append(job_id_dl2_sens)
-
+    log_dl2_to_sensitivity = {job_id_dl2_sens: job_id_dl2_sens.slurm_command}
+    jobids_dl2_to_sensitivity = [job_id_dl2_sens]
     log.info(f"Output dir of sensitivity file: {output}")
     log.info(f"Submitted batch job {job_id_dl2_sens}")
-
-    # Create plot from sensitivity files
     cmd_plot_sens = f'lstmcpipe_plot_irfs -f {output} -o {output.replace(".fits.gz", ".png")}'
 
     sbatch_plot_sens = SbatchLstMCStage(
-        "dl2_sens_plot",  # --partition=short
+        "dl2_sens_plot",
         wrap_command=cmd_plot_sens,
         slurm_error=Path(output).parent.joinpath("job_plot_sensitivity-%j.e"),
         slurm_output=Path(output).parent.joinpath("job_plot_sensitivity-%j.o"),
-        slurm_deps=job_id_dl2_sens,
-        slurm_options=slurm_options,
+        slurm_dependencies=job_id_dl2_sens,
+        extra_slurm_options=extra_slurm_options,
         slurm_account=batch_configuration["slurm_account"],
         source_environment=batch_configuration["source_environment"],
         backend="export MPLBACKEND=Agg; ",
     )
 
     job_id_plot_sens = sbatch_plot_sens.submit()
-    log_dl2_to_sensitivity.update({job_id_plot_sens: sbatch_plot_sens.slurm_command})
+    log_dl2_to_sensitivity[job_id_plot_sens] = sbatch_plot_sens.slurm_command
     jobids_dl2_to_sensitivity.append(job_id_plot_sens)
-
     log.info(f"Output dir of sensitivity plots: {output}")
     log.info(f"Submitted batch job {job_id_plot_sens}")
-
     return log_dl2_to_sensitivity, ",".join(jobids_dl2_to_sensitivity)
```

### Comparing `lstmcpipe-0.8.6/lstmcpipe/stages/mc_merge_dl1.py` & `lstmcpipe-0.9.0/lstmcpipe/stages/mc_merge_dl1.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,21 +3,15 @@
 import logging
 from pathlib import Path
 from ..utils import save_log_to_file, SbatchLstMCStage
 
 log = logging.getLogger(__name__)
 
 
-def batch_merge_dl1(
-    dict_paths,
-    batch_config,
-    logs,
-    jobid_from_splitting,
-    workflow_kind="lstchain",
-):
+def batch_merge_dl1(dict_paths, batch_config, logs, jobid_from_splitting, workflow_kind="lstchain"):
     """
     Function to batch the onsite_mc_merge_and_copy function once the all the r0_to_dl1 jobs (batched by particle type)
     have finished.
 
     Batch 8 merge_and_copy_dl1 jobs ([train, test] x particle) + the move_dl1 and move_dir jobs (2 per particle).
 
     Parameters
@@ -39,99 +33,78 @@
          Comma-separated str with all the job-ids to be passed to the next
          stage of the workflow (as a slurm dependency)
 
     """
     log_merge = {}
     all_jobs_merge_stage = []
     debug_log = {}
-
-    log.info("==== START {} ====".format("batch merge_and_copy_dl1_workflow"))
-    # TODO Lukas: merging option will come inside the
-    #  dict_paths["merge_dl1"]["merging_options"]
-    #    if isinstance(smart_merge, str):
-    #        merge_flag = "lst" in smart_merge
-    #    else:
-    #        merge_flag = smart_merge
-    #    log.debug("Merge flag set: {}".format(merge_flag))
-
+    log.info('==== START batch merge_and_copy_dl1_workflow ====')
     for paths in dict_paths:
         job_logs, jobid_debug = merge_dl1(
             paths["input"],
             paths["output"],
             merging_options=paths.get('options', None),
             batch_configuration=batch_config,
             wait_jobs_split=jobid_from_splitting,
             workflow_kind=workflow_kind,
-            slurm_options=paths.get("slurm_options", None),
+            extra_slurm_options=paths.get("extra_slurm_options", None),
         )
 
         log_merge.update(job_logs)
         all_jobs_merge_stage.append(jobid_debug)
-
-    jobids_for_train = ','.join(all_jobs_merge_stage)
-
     save_log_to_file(log_merge, logs["log_file"], "merge_dl1")
     save_log_to_file(debug_log, logs["debug_file"], workflow_step="merge_dl1")
-
-    log.info("==== END {} ====".format("batch merge_and_copy_dl1_workflow"))
-
-    return jobids_for_train
+    log.info('==== END batch merge_and_copy_dl1_workflow ====')
+    return ','.join(all_jobs_merge_stage)
 
 
 def merge_dl1(
     input_dir,
     output_file,
     batch_configuration,
     wait_jobs_split="",
     merging_options=None,
     workflow_kind="lstchain",
-    slurm_options=None,
+    extra_slurm_options=None,
 ):
     """
 
     Parameters
     ----------
     input_dir: str
     output_file: str
     batch_configuration: dict
     wait_jobs_split: str
     merging_options: dict
     workflow_kind: str
-    slurm_options: str
+    extra_slurm_options: dict
         Extra slurm options to be passed to the sbatch command
 
     Returns
     -------
     log_merge: dict
     jobid_merge: str
 
     """
     merging_options = "" if merging_options is None else merging_options
-    log_merge = {}
-
-    # command passed changes depending on the workflow_kind
-    if workflow_kind == "lstchain":
-        cmd = f'lstchain_merge_hdf5_files -d {input_dir} -o {output_file} {merging_options}'
-    elif workflow_kind == "hiperta":
-        # HiPeRTA workflow still uses --smart flag (lstchain v0.6.3)
+    if workflow_kind in ["lstchain", "hiperta"]:
         cmd = f'lstchain_merge_hdf5_files -d {input_dir} -o {output_file} {merging_options}'
-    else:  # ctapipe case
+
+    else:
         cmd = f'ctapipe-merge --input-dir {input_dir} --output {output_file} {merging_options}'
 
     sbatch_merge_dl1 = SbatchLstMCStage(
         "merge_dl1",
         wrap_command=cmd,
         slurm_error=Path(output_file).parent.joinpath("merging-output.e"),
         slurm_output=Path(output_file).parent.joinpath("merging-output.o"),
-        slurm_deps=wait_jobs_split,
-        slurm_options=slurm_options,
+        slurm_dependencies=wait_jobs_split,
+        extra_slurm_options=extra_slurm_options,
         slurm_account=batch_configuration["slurm_account"],
         source_environment=batch_configuration["source_environment"],
     )
 
     jobid_merge = sbatch_merge_dl1.submit()
-    log_merge.update({jobid_merge: sbatch_merge_dl1.slurm_command})
-
+    log_merge = {jobid_merge: sbatch_merge_dl1.slurm_command}
     log.info(f"\nMerging DL1 file from {input_dir} dir into {output_file} file.")
     log.info(f"Submitted batch job {jobid_merge}")
-
     return log_merge, jobid_merge
```

### Comparing `lstmcpipe-0.8.6/lstmcpipe/stages/mc_process_dl1.py` & `lstmcpipe-0.9.0/lstmcpipe/stages/mc_process_dl1.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,22 +7,15 @@
 from pathlib import Path
 from ..utils import save_log_to_file, SbatchLstMCStage
 from ..io.data_management import check_data_path, get_input_filelist
 
 log = logging.getLogger(__name__)
 
 
-def batch_process_dl1(
-    dict_paths,
-    conf_file,
-    batch_config,
-    logs,
-    workflow_kind="lstchain",
-    new_production=True,
-):
+def batch_process_dl1(dict_paths, conf_file, batch_config, logs, workflow_kind="lstchain", new_production=True):
     """
     Batch the dl1 processing jobs by particle type.
 
     Parameters
     ----------
     dict_paths : dict
         Core dictionary with {stage: PATHS} information
@@ -42,75 +35,65 @@
     -------
     jobids_dl1_processing_stage : str
         string, separated by commas, containing all the jobids of this stage
     """
     log_process_dl1 = {}
     debug_log = {}
     jobids_dl1_processing_stage = []
-
-    log.info("==== START {} dl1 processing ====".format(workflow_kind))
-
+    log.info(f"==== START {workflow_kind} dl1 processing ====")
     if new_production:
-
         for paths in dict_paths["r0_to_dl1"]:
-
             try:
                 check_data_path(paths["input"], glob="*.simtel.gz")
             except ValueError:
                 debug_log["**EMPTY_R0_DIR**"] = f'{paths["input"]} directory does not contain any simtel.gz file'
-                continue
 
+                continue
             job_logs, jobid = r0_to_dl1(
                 paths["input"],
                 paths["output"],
                 config_file=conf_file,
                 batch_config=batch_config,
                 workflow_kind=workflow_kind,
-                slurm_options=paths.get("slurm_options", None),
+                extra_slurm_options=paths.get("extra_slurm_options", None),
             )
+
             log_process_dl1.update(job_logs)
             jobids_dl1_processing_stage.append(jobid)
             debug_log[jobid] = f'r0_dl1 job from input dir: {paths["input"]}'
-
     else:
-
         for paths in dict_paths["dl1ab"]:
             job_logs, jobid = reprocess_dl1(
                 paths["input"],
                 paths["output"],
                 config_file=conf_file,
                 batch_config=batch_config,
                 workflow_kind=workflow_kind,
-                slurm_options=paths.get("slurm_options", None),
+                extra_slurm_options=paths.get("extra_slurm_options", None),
             )
 
             log_process_dl1.update(job_logs)
             jobids_dl1_processing_stage.append(jobid)
             debug_log[jobid] = f'dl1ab job from input dir: {paths["input"]}'
-
-    # Create a string to be directly passed
     jobids_dl1_processing_stage = ",".join(jobids_dl1_processing_stage)
-
     save_log_to_file(log_process_dl1, logs["log_file"], "r0_to_dl1")
     save_log_to_file(debug_log, logs["debug_file"], workflow_step="r0_to_dl1")
-
-    log.info("==== END {} dl1 processing ====".format(workflow_kind))
-
+    log.info(f"==== END {workflow_kind} dl1 processing ====")
     return jobids_dl1_processing_stage
 
 
 def r0_to_dl1(
     input_dir,
     output_dir,
     workflow_kind="lstchain",
     config_file=None,
     batch_config=None,
     debug_mode=False,
     keep_rta_file=False,
-    slurm_options=None,
+    extra_slurm_options=None,
 ):
     """
     R0 to DL1 MC onsite conversion.
     Organizes files and launches slurm jobs in two slurm arrays.
 
 
     Parameters
@@ -122,15 +105,15 @@
     config_file : str or Path
         Path to the {lstchain, ctapipe, HiPeRTA} configuration file
     batch_config : dict
         Dictionary containing the full (source + env) source_environment and the slurm_account strings.
         ! NOTE : train_pipe AND dl1_to_dl2 **MUST** be run with the same environment.
     workflow_kind: str
         One of the supported pipelines. Defines the command to be run on r0 files
-    slurm_options: str
+    extra_slurm_options: dict
         Extra slurm options to be passed
 
     # HIPERTA ARGUMENTS
     keep_rta_file : bool
         Flag to indicate whether to keep (keep_rta_file = True) or remove (keep_rta_file = Flase ) the
         `dl1v06_reorganized_*.h5` output file (hiperta_r0_dl1 and re-organiser stages).
         Argument to be passed to the hiperta_r0_to_dl1lstchain script.
@@ -141,93 +124,73 @@
     Returns
     -------
     jobid2log : dict
         dictionary log containing {jobid: batch_cmd} information
     jobids_r0_dl1
         A list of all the jobs sent for input dir
     """
-
-    log.info("\nStarting R0 to DL1 processing for files in dir : {}".format(input_dir))
-
+    log.info(f'\nStarting R0 to DL1 processing for files in dir : {input_dir}')
     if workflow_kind == "lstchain":
         base_cmd = f"lstmcpipe_lst_core_r0_dl1 -c {config_file} "
         jobtype_id = "LST"
     elif workflow_kind == "ctapipe":
         base_cmd = f"lstmcpipe_cta_core_r0_dl1 -c {config_file} "
         jobtype_id = "CTA"
     elif workflow_kind == "hiperta":
         base_cmd = f"lstmcpipe_rta_core_r0_dl1 -c {config_file} "
         if keep_rta_file:
             base_cmd += " --keep_rta_file"
         if debug_mode:
             base_cmd += " --debug_mode"
-
         jobtype_id = "RTA"
     else:
         base_cmd = ''
         jobtype_id = ''
         log.critical("Please, select an allowed workflow kind.")
         exit(-1)
-
     raw_files_list = get_input_filelist(input_dir, glob_pattern="*.simtel.gz")
-
-    if len(raw_files_list) < 50:
-        dl1_files_per_job = 20
-    else:
-        dl1_files_per_job = 50
-
+    dl1_files_per_job = 20 if len(raw_files_list) < 50 else 50
     with open("r0_to_dl1.list", "w+") as newfile:
         for f in raw_files_list:
             newfile.write(f)
             newfile.write("\n")
-
-    log.info("{} raw R0 files".format(len(raw_files_list)))
-
-    # If file exists, means that prod is being re-run
+    log.info(f"{len(raw_files_list)} raw R0 files")
     output_dir = Path(output_dir)
     if output_dir.exists() and any(output_dir.iterdir()):
         shutil.rmtree(output_dir)
-
     job_logs_dir = output_dir.joinpath("job_logs_r0dl1")
     Path(job_logs_dir).mkdir(exist_ok=True, parents=True)
-
-    log.info("DL1 DATA DIR: {}".format(output_dir))
-
+    log.info(f"DL1 DATA DIR: {output_dir}")
     jobid2log, jobids_r0_dl1 = submit_dl1_jobs(
         input_dir,
         output_dir,
         base_cmd=base_cmd,
         file_list=raw_files_list,
         job_type_id=jobtype_id,
         dl1_files_per_batched_job=dl1_files_per_job,
         job_logs_dir=job_logs_dir,
         batch_config=batch_config,
         dl1_processing_type="r0_to_dl1",
-        slurm_options=slurm_options,
+        extra_slurm_options=extra_slurm_options,
     )
 
-    # copy config into working dir
     if config_file is not None:
         shutil.copyfile(config_file, job_logs_dir.joinpath(Path(config_file).name))
-
-    # save file lists into logs
     shutil.move("r0_to_dl1.list", job_logs_dir)
-
-    # return it log dictionary
     return jobid2log, jobids_r0_dl1
 
 
 def reprocess_dl1(
     input_dir,
     output_dir,
     workflow_kind="lstchain",
     config_file=None,
     batch_config=None,
     dl1_files_per_job=50,
-    slurm_options=None,
+    extra_slurm_options=None,
 ):
     """
     Reprocessing of existing dl1 files.
     Organizes files and launches slurm jobs in two slurm arrays.
     The same train/test split performed with the earlier r0 to dl1
     processing is used.
 
@@ -242,90 +205,79 @@
     batch_config : dict
         Dictionary containing the (full) source_environment and the slurm_account strings.
         ! NOTE : train_pipe AND dl1_to_dl2 **MUST** be run with the same environment.
     workflow_kind: str
         One of the supported pipelines. Defines the command to be run on r0 files
     dl1_files_per_job: int
         Number of dl1 files to be processed per job array that was batched.
-    slurm_options: str
+    extra_slurm_options: dict
         Extra slurm options to be passed to the sbatch command
 
     Returns
     -------
     jobid2log : dict
         dictionary log containing {jobid: batch_cmd} information
     jobids_dl1_dl1
         A list of all the jobs sent for input dir
     """
-    log.info("Applying DL1ab on DL1 files in {}".format(input_dir))
-
+    log.info(f"Applying DL1ab on DL1 files in {input_dir}")
     if workflow_kind == "lstchain":
         base_cmd = f"lstmcpipe_lst_core_dl1ab -c {config_file} "
         jobtype_id = "LST"
     elif workflow_kind == "ctapipe":
         base_cmd = f"lstmcpipe_cta_core_r0_dl1 -c {config_file} "
         jobtype_id = "CTA"
     else:
         base_cmd = ""
         jobtype_id = ""
         log.critical(f"Unknown workflow {workflow_kind}")
         exit(-1)
-
     check_data_path(input_dir)
     dl1ab_filelist = [file.resolve().as_posix() for file in Path(input_dir).glob("*.h5")]
 
-    log.info("{} DL1 files".format(len(dl1ab_filelist)))
-
+    log.info(f"{len(dl1ab_filelist)} DL1 files")
     with open("dl1ab.list", "w+") as newfile:
         for f in dl1ab_filelist:
             newfile.write(f)
             newfile.write("\n")
-
     Path(output_dir).mkdir(exist_ok=True, parents=True)
     job_logs_dir = Path(output_dir).joinpath("job_logs_dl1ab")
     Path(job_logs_dir).mkdir(exist_ok=True)
-
-    log.info("DL1ab destination DATA DIR: {}".format(output_dir))
-
+    log.info(f"DL1ab destination DATA DIR: {output_dir}")
     jobid2log, jobids_dl1_dl1 = submit_dl1_jobs(
         input_dir,
         output_dir,
         base_cmd=base_cmd,
         file_list=dl1ab_filelist,
         job_type_id=jobtype_id,
         dl1_files_per_batched_job=dl1_files_per_job,
         job_logs_dir=job_logs_dir,
         batch_config=batch_config,
         dl1_processing_type="dl1ab",
-        slurm_options=slurm_options,
+        extra_slurm_options=extra_slurm_options,
     )
 
-    # copy config into working dir
     if config_file is not None:
         shutil.copyfile(config_file, job_logs_dir.joinpath(Path(config_file).name))
-
-    # save file lists into logs
     shutil.move("dl1ab.list", job_logs_dir)
-
-    # return it log dictionary
     return jobid2log, jobids_dl1_dl1
 
 
 def submit_dl1_jobs(
     input_dir,
     output_dir,
     base_cmd,
     file_list,
     job_type_id,
     dl1_files_per_batched_job,
     job_logs_dir,
     batch_config,
     n_jobs_parallel=100,
     dl1_processing_type="r0_to_dl1",
-    slurm_options="",
+    extra_slurm_options=None,
 ):
     """
     Compose sbatch command and batches it
 
     Parameters
     ----------
     input_dir: str
@@ -347,65 +299,50 @@
         Dictionary containing the full (source + env) source_environment and the slurm_account strings.
         ! NOTE : train_pipe AND dl1_to_dl2 **MUST** be run with the same environment.
     n_jobs_parallel: int
         Number of array jobs to be processed in parallel.
         Default = 100
     dl1_processing_type: str
         String for job and filelist naming
-    slurm_options: str
+    extra_slurm_options: dict
         Extra slurm options to be passed
 
     Returns
     -------
     jobid2log: dict
     jobid: str
 
     """
-    jobid2log = {}
-
     number_of_sublists = len(file_list) // dl1_files_per_batched_job + int(
         len(file_list) % dl1_files_per_batched_job > 0
     )
 
     for i in range(number_of_sublists):
-        output_file = job_logs_dir.joinpath("{}_{}.sublist".format(dl1_processing_type, i)).resolve().as_posix()
+        output_file = job_logs_dir.joinpath(f"{dl1_processing_type}_{i}.sublist").resolve().as_posix()
+
         with open(output_file, "w+") as out:
-            for line in file_list[i * dl1_files_per_batched_job : dl1_files_per_batched_job * (i + 1)]:  # noqa
+            for line in file_list[i * dl1_files_per_batched_job:dl1_files_per_batched_job * (i + 1)]:
                 out.write(line)
                 out.write("\n")
-
     log.info(f"{number_of_sublists} files generated for list of files at {input_dir}")
 
-    sublist_names = [f.as_posix() for f in Path(job_logs_dir).glob("*.sublist")]  # Number of sublists ??
-
-    # start 1 jobarray with all files included. The job selects its file based on its task id
+    sublist_names = [f.as_posix() for f in Path(job_logs_dir).glob("*.sublist")]
     cmd = f'{base_cmd} -f {" ".join(sublist_names)} --output_dir {output_dir}'
+    extra_slurm_default_options = {'partition': 'long', 'array': f"0-{len(sublist_names) - 1}%{n_jobs_parallel}"}
 
+    if extra_slurm_options is not None:
+        extra_slurm_default_options.update(extra_slurm_options)
     sbatch_process_dl1 = SbatchLstMCStage(
         dl1_processing_type,
         wrap_command=cmd,
+        job_name=f"{job_type_id}-{dl1_processing_type}",
         slurm_error=job_logs_dir.joinpath("job_%A_%a.e").as_posix(),
         slurm_output=job_logs_dir.joinpath("job_%A_%a.o").as_posix(),
         slurm_account=batch_config["slurm_account"],
         source_environment=batch_config["source_environment"],
+        extra_slurm_options=extra_slurm_default_options,
     )
-    if dl1_processing_type == "r0_to_dl1":
-        sbatch_process_dl1.r0_dl1_options(
-            process_dl1_job_name=f"{job_type_id}-{dl1_processing_type}",
-            array=f"0-{len(sublist_names) - 1}%{n_jobs_parallel}",
-            partition="long",
-            extra_slurm_options="",
-        )
-    elif dl1_processing_type == "dl1ab":
-        sbatch_process_dl1.dl1ab_options(
-            process_dl1ab_job_name=f"{job_type_id}-{dl1_processing_type}",
-            array=f"0-{len(sublist_names) - 1}%{n_jobs_parallel}",
-            partition="long",
-            extra_slurm_options="",
-        )
 
     jobid = sbatch_process_dl1.submit()
     log.debug(f"Submitted batch job {jobid}")
-
-    jobid2log.update({jobid: sbatch_process_dl1.slurm_command})
-
+    jobid2log = {jobid: sbatch_process_dl1.slurm_command}
     return jobid2log, jobid
```

### Comparing `lstmcpipe-0.8.6/lstmcpipe/stages/mc_train.py` & `lstmcpipe-0.9.0/lstmcpipe/stages/mc_train.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,30 +51,30 @@
         job_logs, jobid = train_pipe(
             gamma_dl1_train_file,
             proton_dl1_train_file,
             models_dir,
             config_file=config_file,
             batch_configuration=batch_config,
             wait_jobs_dl1=jobids_from_merge,
-            slurm_options=paths.get("slurm_options", None),
+            extra_slurm_options=paths.get("extra_slurm_options", None),
         )
 
         log_train.update(job_logs)
         jobid_for_dl1_to_dl2.append(jobid)
 
         debug_train[jobid] = (
             f"The single jobid from train_pipe that depends of {jobids_from_merge} - merge" f"_and_copy jobids"
         )
 
     jobid_for_dl1_to_dl2 = ",".join(jobid_for_dl1_to_dl2)
 
     save_log_to_file(log_train, logs["log_file"], workflow_step="train_pipe")
     save_log_to_file(debug_train, logs["debug_file"], workflow_step="train_pipe")
 
-    log.info("==== END {} ====".format("batch mc_train_workflow"))
+    log.info("==== END batch mc_train_workflow ====")
 
     return jobid_for_dl1_to_dl2
 
 
 def batch_plot_rf_features(
     dict_paths,
     config_file,
@@ -117,15 +117,15 @@
         cmd = f"lstmcpipe_plot_models_importance {models_dir} -cf {config_file}"
 
         sbatch_rf_feat = SbatchLstMCStage(
             "RF_importance",
             wrap_command=cmd,
             slurm_error=Path(models_dir).joinpath("job_plot_rf_feat_importance.e").resolve().as_posix(),
             slurm_output=Path(models_dir).joinpath(models_dir, "job_plot_rf_feat_importance.o").resolve().as_posix(),
-            slurm_deps=train_jobid,
+            slurm_dependencies=train_jobid,
             slurm_account=batch_configuration["slurm_account"],
             source_environment=batch_configuration["source_environment"],
             backend="export MPLBACKEND=Agg;",
         )
 
         jobid = sbatch_rf_feat.submit()
 
@@ -147,15 +147,15 @@
 def train_pipe(
     gamma_dl1_train_file,
     proton_dl1_train_file,
     models_dir,
     config_file=None,
     batch_configuration='',
     wait_jobs_dl1=None,
-    slurm_options=None,
+    extra_slurm_options=None,
 ):
     """
     Train RF from MC DL1 data (onsite LaPalma cluster)
 
     Parameters
     ----------
     gamma_dl1_train_file: str
@@ -169,15 +169,15 @@
     batch_configuration : dict
         Dictionary containing the (full) source_environment and the slurm_account strings to be passed to the
         sbatch commands
         ! NOTE : train_pipe AND dl1_to_dl2 MUST BE RUN WITH THE SAME ENVIRONMENT
     wait_jobs_dl1 : str
         A string (of chained job_ids separated by ',' and without spaces between each element), containing
         all the job_ids of the merging stage
-    slurm_options: str
+    extra_slurm_options: dict
         Extra slurm options to be passed to the sbatch command
 
     Returns
     -------
     log_train : dict
         dictionary containing the jobid of the batched job as key and the run command (the lstchain_mc_train
         command with all its corresponding arguments) as value.
@@ -196,16 +196,16 @@
         cmd = cmd + " -c {}".format(config_file)
 
     sbatch_train_pipe = SbatchLstMCStage(
         "train_pipe",
         wrap_command=cmd,
         slurm_error=Path(models_dir).joinpath("train_job.e").resolve().as_posix(),
         slurm_output=Path(models_dir).joinpath("train_job.o").resolve().as_posix(),
-        slurm_deps=wait_jobs_dl1,
-        slurm_options=slurm_options,
+        slurm_dependencies=wait_jobs_dl1,
+        extra_slurm_options=extra_slurm_options,
         slurm_account=batch_configuration["slurm_account"],
         source_environment=batch_configuration["source_environment"],
     )
 
     jobid_train = sbatch_train_pipe.submit()
     log_train.update({jobid_train: sbatch_train_pipe.slurm_command})
```

### Comparing `lstmcpipe-0.8.6/lstmcpipe/stages/mc_train_test_splitting.py` & `lstmcpipe-0.9.0/lstmcpipe/stages/mc_train_test_splitting.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
     for paths in dict_paths:
         job_logs, jobid = train_test_split(
             paths["input"],
             paths["output"],
             wait_jobid_r0_dl1=jobids_from_r0dl1,
             batch_configuration=batch_config,
-            slurm_options=paths.get("slurm_options", None),
+            extra_slurm_options=paths.get("extra_slurm_options", None),
         )
 
         log_splitting.update(job_logs)
         jobids_for_merging.append(jobid)
         debug_log[jobid] = f"Train test splitting jobid that depends on : {jobids_from_r0dl1}"
 
     jobids_for_merging = ",".join(jobids_for_merging)
@@ -60,25 +60,25 @@
 
 
 def train_test_split(
     input_dir,
     output_dirs,
     batch_configuration,
     wait_jobid_r0_dl1=None,
-    slurm_options=None,
+    extra_slurm_options=None,
 ):
     """
 
     Parameters
     ----------
     input_dir: str
     output_dirs: dict
     batch_configuration: dict
     wait_jobid_r0_dl1: str
-    slurm_options: str
+    extra_slurm_options: dict
         Extra slurm options to be passed to the sbatch command
 
     Returns
     -------
 
     """
     log_splitting = {}
@@ -108,16 +108,16 @@
     )
 
     sbatch_tt_splitting = SbatchLstMCStage(
         "train_test_splitting",
         wrap_command=cmd,
         slurm_error=Path(input_dir).joinpath(input_dir, "split_tt_%j.e"),
         slurm_output=Path(input_dir).joinpath(input_dir, "split_tt_%j.o"),
-        slurm_deps=wait_jobid_r0_dl1,
-        slurm_options=slurm_options,
+        slurm_dependencies=wait_jobid_r0_dl1,
+        extra_slurm_options=extra_slurm_options,
         slurm_account=batch_configuration["slurm_account"],
         source_environment=batch_configuration["source_environment"],
     )
 
     jobid_split = sbatch_tt_splitting.submit()
     log_splitting.update({jobid_split: sbatch_tt_splitting.slurm_command})
```

### Comparing `lstmcpipe-0.8.6/lstmcpipe/standard_configs/ctapipe_standard_config_v011.json` & `lstmcpipe-0.9.0/lstmcpipe/standard_configs/ctapipe_standard_config_v011.json`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/lstmcpipe/standard_configs/hiperta_standard_config.txt` & `lstmcpipe-0.9.0/lstmcpipe/standard_configs/hiperta_standard_config.txt`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/lstmcpipe/standard_configs/lstchain_dl1ab_tune_MC_to_Crab_config_v091_MC_Tel1.json` & `lstmcpipe-0.9.0/lstmcpipe/standard_configs/lstchain_dl1ab_tune_MC_to_Crab_config_v091_MC_Tel1.json`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/lstmcpipe/standard_configs/lstchain_standard_config_v045.json` & `lstmcpipe-0.9.0/lstmcpipe/standard_configs/lstchain_standard_config_v045.json`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/lstmcpipe/standard_configs/lstchain_standard_config_v050.json` & `lstmcpipe-0.9.0/lstmcpipe/standard_configs/lstchain_standard_config_v050.json`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/lstmcpipe/standard_configs/lstchain_standard_config_v052.json` & `lstmcpipe-0.9.0/lstmcpipe/standard_configs/lstchain_standard_config_v052.json`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/lstmcpipe/standard_configs/lstchain_standard_config_v060.json` & `lstmcpipe-0.9.0/lstmcpipe/standard_configs/lstchain_standard_config_v060.json`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/lstmcpipe/standard_configs/lstchain_standard_config_v061.json` & `lstmcpipe-0.9.0/lstmcpipe/standard_configs/lstchain_standard_config_v061.json`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/lstmcpipe/standard_configs/lstchain_standard_config_v070.json` & `lstmcpipe-0.9.0/lstmcpipe/standard_configs/lstchain_standard_config_v070.json`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/lstmcpipe/standard_configs/lstchain_standard_config_v091.json` & `lstmcpipe-0.9.0/lstmcpipe/standard_configs/lstchain_standard_config_v091.json`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/lstmcpipe/tests/test_utils.py` & `lstmcpipe-0.9.0/lstmcpipe/tests/test_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -69,44 +69,44 @@
 def test_sbatch_lst_mc_stage():
     with pytest.raises(TypeError):
         SbatchLstMCStage()
         SbatchLstMCStage("merge")
 
     sbatch = SbatchLstMCStage(stage="r0_to_dl1", wrap_command="command to be batched")
     assert (
-        sbatch.slurm_command == 'sbatch --parsable --job-name=r0_dl1 --partition=long --array=0-0%100  '
-        '--error=./slurm-%j.e --output=./slurm-%j.o   --wrap="command to be batched"'
+        sbatch.slurm_command == 'sbatch --parsable --partition=long --job-name=r0_dl1 --array=0-0%100 '
+                                '--error=./slurm-%j.e --output=./slurm-%j.o  --wrap="command to be batched"'
     )
 
-    sbatch.slurm_options = "-A lstrta -p xxl --mem 160G --cpus-per-task=32"
+    sbatch.extra_slurm_options = {'account': 'lstrta', 'partition': 'xxl', 'mem': '160G', 'cpus-per-task': 32}
     assert (
-        sbatch.slurm_command == 'sbatch --parsable --job-name=r0_dl1 -A lstrta -p xxl --mem 160G --cpus-per-task=32 '
-        '--error=./slurm-%j.e --output=./slurm-%j.o   --wrap="command to be batched"'
+        sbatch.slurm_command == 'sbatch --parsable --partition=xxl --job-name=r0_dl1 --array=0-0%100 '
+                                '--error=./slurm-%j.e --output=./slurm-%j.o --account=lstrta --mem=160G '
+                                '--cpus-per-task=32  --wrap="command to be batched"'
     )
 
-    sbatch.slurm_options = None
-    sbatch.check_slurm_dependencies("123,243,345,456")
-    assert sbatch.slurm_dependencies == "--dependency=afterok:123,243,345,456"
+    sbatch.extra_slurm_options = None
+    sbatch.slurm_dependencies = "123,243,345,456"
+    assert sbatch._construct_slurm_dependencies() == "--dependency=afterok:123,243,345,456"
 
     sbatch.compose_wrap_command(
         wrap_command="python args",
         source_env="source .bashrc_file; conda activate   ",
         backend="  export MPLBACKEND=Agg    ",
     )
     assert sbatch.wrap_cmd == '--wrap="export MPLBACKEND=Agg; source .bashrc_file; conda activate; python args"'
 
     with pytest.raises(ValueError):
         sbatch.submit()  # slurm not installed
-        sbatch.stage_default_options("invented_stage")
-        sbatch.check_slurm_dependencies(slurm_deps="123,,234")
+        sbatch.stage_default_options("dummy_stage")
+        sbatch.set_slurm_dependencies(slurm_deps="123,,234")
 
     stages = sbatch._valid_stages
     for stage in stages:
-        sbatch.stage_default_options(stage)
-        assert "--job-name=" in sbatch.job_name
+        assert "--job-name=" in sbatch.slurm_command
         assert "--partition=" in sbatch.slurm_command
 
 
 def test_dump_lstchain_std_config():
     with tempfile.TemporaryDirectory() as tmpdir:
         outfile = Path(tmpdir).joinpath('cfg.json')
         dump_lstchain_std_config(filename=outfile, allsky=False)
```

### Comparing `lstmcpipe-0.8.6/lstmcpipe/version.py` & `lstmcpipe-0.9.0/lstmcpipe/version.py`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/lstmcpipe.egg-info/PKG-INFO` & `lstmcpipe-0.9.0/lstmcpipe.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lstmcpipe
-Version: 0.8.6
+Version: 0.9.0
 Summary: Scripts to ease the reduction of MC data on the LST cluster at La Palma. With this package, the analysis/creation of R1/DL0/DL1/DL2/IRFs can be orchestrated.
 Home-page: https://github.com/cta-observatory/lstmcpipe
 Author: Thomas Vuillaume,Enrique Garcia,Lukas Nickel,
 Author-email: thomas.vuillaume@lapp.in2p3.fr
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lstmcpipe-0.8.6/lstmcpipe.egg-info/SOURCES.txt` & `lstmcpipe-0.9.0/lstmcpipe.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -151,14 +151,17 @@
 production_configs/20220531_dec3476_std/lstmcpipe_config_2022-05-31_PathConfigAllSkyFull.yaml
 production_configs/20220601_dec3476_tuned/README.md
 production_configs/20220601_dec3476_tuned/lstchain_config_2022-06-01.json
 production_configs/20220601_dec3476_tuned/lstmcpipe_config_2022-06-01_PathConfigAllSkyFullDL1ab.yaml
 production_configs/20220624_dec_4822_tuned_TestDIffuseGammas/README_tuned_22_06_24_TestDiffuseGammas.md
 production_configs/20220624_dec_4822_tuned_TestDIffuseGammas/lstchain_config_2022-06-24.json
 production_configs/20220624_dec_4822_tuned_TestDIffuseGammas/lstmcpipe_config_2022-06-24_TestDiffuseGammas.yaml
+production_configs/20220905_src4_high_NSB/lstchain_config_2022-09-05.json
+production_configs/20220905_src4_high_NSB/lstmcpipe_config_2022-09-05_PathConfigAllSkyFull.yaml
+production_configs/20220905_src4_high_NSB/readme.md
 production_configs/nsb_psf_tuned_zen40_src2/lstchain_config_ze40_south_NSBtuning.json
 production_configs/nsb_psf_tuned_zen40_src2/lstmcpipe_config.yml
 production_configs/nsb_psf_tuned_zen40_src2/readme.md
 production_configs/nsb_tuned_zen40_scr1/lstchain_config_NSBtuning.json
 production_configs/nsb_tuned_zen40_scr1/lstmcpipe_config.yml
 production_configs/nsb_tuned_zen40_scr1/readme.md
 production_configs/psf_tuned_zen20/lstchain_config.json
```

### Comparing `lstmcpipe-0.8.6/lstmcpipe.egg-info/entry_points.txt` & `lstmcpipe-0.9.0/lstmcpipe.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/production_configs/20210416_v0.7.3_prod5_trans_80_local_taicut_8_4/config_MC_prod_20210416_v0.7.3_prod5_trans_80_local_taicut_8_4.yml` & `lstmcpipe-0.9.0/production_configs/20210416_v0.7.3_prod5_trans_80_local_taicut_8_4/config_MC_prod_20210416_v0.7.3_prod5_trans_80_local_taicut_8_4.yml`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/production_configs/20210416_v0.7.3_prod5_trans_80_local_taicut_8_4/lstchain_standard_config_v073_Tel1_tail_8_4_MC_config.json` & `lstmcpipe-0.9.0/production_configs/20210416_v0.7.3_prod5_trans_80_local_taicut_8_4/lstchain_standard_config_v073_Tel1_tail_8_4_MC_config.json`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/production_configs/20210506_v0.7.3_prod5_trans_80_zen40deg_local_tailcut_8_4/config_MC_prod_20210506_v0.7.3_prod5_trans_80_zen40deg_local_tailcut_8_4.yml` & `lstmcpipe-0.9.0/production_configs/20210506_v0.7.3_prod5_trans_80_zen40deg_local_tailcut_8_4/config_MC_prod_20210506_v0.7.3_prod5_trans_80_zen40deg_local_tailcut_8_4.yml`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/production_configs/20210506_v0.7.3_prod5_trans_80_zen40deg_local_tailcut_8_4/lstchain_standard_config_v073_Tel1_tail_8_4_MC_config.json` & `lstmcpipe-0.9.0/production_configs/20210506_v0.7.3_prod5_trans_80_zen40deg_local_tailcut_8_4/lstchain_standard_config_v073_Tel1_tail_8_4_MC_config.json`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/production_configs/20210923_v0.7.5_prod5_trans_80_dynamic_cleaning/config_MC_prod_20210923_v0.7.5_prod5_trans_80_dynamic_cleaning.yml` & `lstmcpipe-0.9.0/production_configs/20210923_v0.7.5_prod5_trans_80_dynamic_cleaning/config_MC_prod_20210923_v0.7.5_prod5_trans_80_dynamic_cleaning.yml`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/production_configs/20210923_v0.7.5_prod5_trans_80_dynamic_cleaning/lstchain_standard_config_v075_Tel1_tail84_dynamic_clean.json` & `lstmcpipe-0.9.0/production_configs/20210923_v0.7.5_prod5_trans_80_dynamic_cleaning/lstchain_standard_config_v075_Tel1_tail84_dynamic_clean.json`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/production_configs/20220215_v0.9.1_prod5_trans_80_local_tailcut_8_4/config_MC_prod_20220215_v0.9.1_prod5_trans_80_local_tailcut_8_4.yml` & `lstmcpipe-0.9.0/production_configs/20220215_v0.9.1_prod5_trans_80_local_tailcut_8_4/config_MC_prod_20220215_v0.9.1_prod5_trans_80_local_tailcut_8_4.yml`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/production_configs/20220215_v0.9.1_prod5_trans_80_local_tailcut_8_4/lstchain_standard_config_v091_MC_Tel1.json` & `lstmcpipe-0.9.0/production_configs/20220215_v0.9.1_prod5_trans_80_local_tailcut_8_4/lstchain_standard_config_v091_MC_Tel1.json`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/production_configs/20220218_v0.9.2_prod5_trans_80_dl1ab_tune_MC_to_Crab/config_MC_prod_20220218_v0.9.2_prod5_trans_80_dl1ab_tune_MC_to_Crab.yml` & `lstmcpipe-0.9.0/production_configs/20220218_v0.9.2_prod5_trans_80_dl1ab_tune_MC_to_Crab/config_MC_prod_20220218_v0.9.2_prod5_trans_80_dl1ab_tune_MC_to_Crab.yml`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/production_configs/20220218_v0.9.2_prod5_trans_80_dl1ab_tune_MC_to_Crab/lstchain_dl1ab_tune_MC_to_Crab_config_v091_MC_Tel1.json` & `lstmcpipe-0.9.0/production_configs/20220218_v0.9.2_prod5_trans_80_dl1ab_tune_MC_to_Crab/lstchain_dl1ab_tune_MC_to_Crab_config_v091_MC_Tel1.json`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/production_configs/20220304_v0.9.3_prod5_trans_80_zen40az180_local_tailcut_8_4/config_MC_prod_20220304_v0.9.3_prod5_trans_80_zen40az180_local_tailcut_8_4.yml` & `lstmcpipe-0.9.0/production_configs/20220304_v0.9.3_prod5_trans_80_zen40az180_local_tailcut_8_4/config_MC_prod_20220304_v0.9.3_prod5_trans_80_zen40az180_local_tailcut_8_4.yml`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/production_configs/20220304_v0.9.3_prod5_trans_80_zen40az180_local_tailcut_8_4/lstchain_standard_config_v091_MC_Tel1.json` & `lstmcpipe-0.9.0/production_configs/20220304_v0.9.3_prod5_trans_80_zen40az180_local_tailcut_8_4/lstchain_standard_config_v091_MC_Tel1.json`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/production_configs/20220511_v0.9.6_allsky_std/generate.py` & `lstmcpipe-0.9.0/production_configs/20220511_v0.9.6_allsky_std/generate.py`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/production_configs/20220511_v0.9.6_allsky_std/lstchain_84.json` & `lstmcpipe-0.9.0/production_configs/20220511_v0.9.6_allsky_std/lstchain_84.json`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/production_configs/20220511_v0.9.6_allsky_std/lstmcpipe_config_20220511_allsky_std.yml` & `lstmcpipe-0.9.0/production_configs/20220511_v0.9.6_allsky_std/lstmcpipe_config_20220511_allsky_std.yml`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/production_configs/20220518_v0.9.6_allsky_dec2276_tuned/lstchain_config_dec_2276_tuned.json` & `lstmcpipe-0.9.0/production_configs/20220518_v0.9.6_allsky_dec2276_tuned/lstchain_config_dec_2276_tuned.json`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/production_configs/20220518_v0.9.6_allsky_dec2276_tuned/lstmcpipe_config_20220518_allsky_dec2276_tuned.yml` & `lstmcpipe-0.9.0/production_configs/20220518_v0.9.6_allsky_dec2276_tuned/lstmcpipe_config_20220518_allsky_dec2276_tuned.yml`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/production_configs/20220523_allsky_std/lstchain_config_2022-05-23.json` & `lstmcpipe-0.9.0/production_configs/20220523_allsky_std/lstchain_config_2022-05-23.json`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/production_configs/20220523_allsky_std/lstmcpipe_config_2022-05-23_PathConfigAllSkyFull.yaml` & `lstmcpipe-0.9.0/production_configs/20220523_allsky_std/lstmcpipe_config_2022-05-23_PathConfigAllSkyFull.yaml`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/production_configs/20220523_dec_413_tuned_nsb/lstchain_config_2022-05-23.json` & `lstmcpipe-0.9.0/production_configs/20220523_dec_413_tuned_nsb/lstchain_config_2022-05-23.json`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/production_configs/20220523_dec_413_tuned_nsb/lstmcpipe_config_2022-05-23_PathConfigAllSkyFullDL1ab.yaml` & `lstmcpipe-0.9.0/production_configs/20220523_dec_413_tuned_nsb/lstmcpipe_config_2022-05-23_PathConfigAllSkyFullDL1ab.yaml`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/production_configs/20220523_src3_dec3476_4822_tuned_nsb/lstchain_config_2022-05-23.json` & `lstmcpipe-0.9.0/production_configs/20220523_src3_dec3476_4822_tuned_nsb/lstchain_config_2022-05-23.json`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/production_configs/20220523_src3_dec3476_4822_tuned_nsb/lstmcpipe_config_2022-05-23_PathConfigAllSkyFullDL1ab.yml` & `lstmcpipe-0.9.0/production_configs/20220523_src3_dec3476_4822_tuned_nsb/lstmcpipe_config_2022-05-23_PathConfigAllSkyFullDL1ab.yml`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/production_configs/20220523_src3_dec3476_4822_tuned_nsb/readme.md` & `lstmcpipe-0.9.0/production_configs/20220523_src3_dec3476_4822_tuned_nsb/readme.md`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/production_configs/20220524_dec_4822_tuned/README_tuned_22_05_24.md` & `lstmcpipe-0.9.0/production_configs/20220524_dec_4822_tuned/README_tuned_22_05_24.md`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/production_configs/20220524_dec_4822_tuned/lstchain_config_2022-05-24.json` & `lstmcpipe-0.9.0/production_configs/20220524_dec_4822_tuned/lstchain_config_2022-05-24.json`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/production_configs/20220524_dec_4822_tuned/lstmcpipe_config_2022-05-24_PathConfigAllSkyFullDL1ab.yaml` & `lstmcpipe-0.9.0/production_configs/20220524_dec_4822_tuned/lstmcpipe_config_2022-05-24_PathConfigAllSkyFullDL1ab.yaml`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/production_configs/20220527_allsky_std_src2_diffgamma/lstchain_config_2022-05-27.json` & `lstmcpipe-0.9.0/production_configs/20220527_allsky_std_src2_diffgamma/lstchain_config_2022-05-27.json`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/production_configs/20220527_allsky_std_src2_diffgamma/lstmcpipe_config_2022-05-27_PathConfigAllSkyFull.yaml` & `lstmcpipe-0.9.0/production_configs/20220527_allsky_std_src2_diffgamma/lstmcpipe_config_2022-05-27_PathConfigAllSkyFull.yaml`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/production_configs/20220531_dec3476_std/lstchain_config_2022-05-31.json` & `lstmcpipe-0.9.0/production_configs/20220531_dec3476_std/lstchain_config_2022-05-31.json`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/production_configs/20220531_dec3476_std/lstmcpipe_config_2022-05-31_PathConfigAllSkyFull.yaml` & `lstmcpipe-0.9.0/production_configs/20220531_dec3476_std/lstmcpipe_config_2022-05-31_PathConfigAllSkyFull.yaml`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/production_configs/20220601_dec3476_tuned/lstchain_config_2022-06-01.json` & `lstmcpipe-0.9.0/production_configs/20220601_dec3476_tuned/lstchain_config_2022-06-01.json`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/production_configs/20220601_dec3476_tuned/lstmcpipe_config_2022-06-01_PathConfigAllSkyFullDL1ab.yaml` & `lstmcpipe-0.9.0/production_configs/20220601_dec3476_tuned/lstmcpipe_config_2022-06-01_PathConfigAllSkyFullDL1ab.yaml`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/production_configs/20220624_dec_4822_tuned_TestDIffuseGammas/README_tuned_22_06_24_TestDiffuseGammas.md` & `lstmcpipe-0.9.0/production_configs/20220624_dec_4822_tuned_TestDIffuseGammas/README_tuned_22_06_24_TestDiffuseGammas.md`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/production_configs/20220624_dec_4822_tuned_TestDIffuseGammas/lstchain_config_2022-06-24.json` & `lstmcpipe-0.9.0/production_configs/20220624_dec_4822_tuned_TestDIffuseGammas/lstchain_config_2022-06-24.json`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/production_configs/20220624_dec_4822_tuned_TestDIffuseGammas/lstmcpipe_config_2022-06-24_TestDiffuseGammas.yaml` & `lstmcpipe-0.9.0/production_configs/20220624_dec_4822_tuned_TestDIffuseGammas/lstmcpipe_config_2022-06-24_TestDiffuseGammas.yaml`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/production_configs/nsb_psf_tuned_zen40_src2/lstchain_config_ze40_south_NSBtuning.json` & `lstmcpipe-0.9.0/production_configs/nsb_psf_tuned_zen40_src2/lstchain_config_ze40_south_NSBtuning.json`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/production_configs/nsb_psf_tuned_zen40_src2/lstmcpipe_config.yml` & `lstmcpipe-0.9.0/production_configs/nsb_psf_tuned_zen40_src2/lstmcpipe_config.yml`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/production_configs/nsb_tuned_zen40_scr1/lstchain_config_NSBtuning.json` & `lstmcpipe-0.9.0/production_configs/nsb_tuned_zen40_scr1/lstchain_config_NSBtuning.json`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/production_configs/nsb_tuned_zen40_scr1/lstmcpipe_config.yml` & `lstmcpipe-0.9.0/production_configs/nsb_tuned_zen40_scr1/lstmcpipe_config.yml`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/production_configs/psf_tuned_zen20/lstchain_config.json` & `lstmcpipe-0.9.0/production_configs/psf_tuned_zen20/lstchain_config.json`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/production_configs/psf_tuned_zen20/lstmcpipe_config.yml` & `lstmcpipe-0.9.0/production_configs/psf_tuned_zen20/lstmcpipe_config.yml`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/production_configs/psf_tuned_zen40/lstchain_config.json` & `lstmcpipe-0.9.0/production_configs/psf_tuned_zen40/lstchain_config.json`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/production_configs/psf_tuned_zen40/lstmcpipe_config.yml` & `lstmcpipe-0.9.0/production_configs/psf_tuned_zen40/lstmcpipe_config.yml`

 * *Files identical despite different names*

### Comparing `lstmcpipe-0.8.6/production_configs/template_prod/lstchain_config.json` & `lstmcpipe-0.9.0/production_configs/template_prod/lstchain_config.json`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -258,8 +258,8 @@
       }
     },
     "waveform_nsb_tuning":{
       "nsb_tuning": false,
       "nsb_tuning_ratio": 0.52,
       "spe_location": "lstchain/data/SinglePhE_ResponseInPhE_expo2Gaus.dat"
     }
-  }
+  }
```

### Comparing `lstmcpipe-0.8.6/setup.py` & `lstmcpipe-0.9.0/setup.py`

 * *Files identical despite different names*

