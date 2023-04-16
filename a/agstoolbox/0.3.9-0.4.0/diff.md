# Comparing `tmp/agstoolbox-0.3.9.tar.gz` & `tmp/agstoolbox-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agstoolbox-0.3.9.tar", last modified: Sun Apr  9 22:39:34 2023, max compression
+gzip compressed data, was "agstoolbox-0.4.0.tar", last modified: Sun Apr 16 13:07:04 2023, max compression
```

## Comparing `agstoolbox-0.3.9.tar` & `agstoolbox-0.4.0.tar`

### file list

```diff
@@ -1,101 +1,105 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 22:39:34.274381 agstoolbox-0.3.9/
--rw-rw-rw-   0        0        0       33 2022-01-27 21:21:40.000000 agstoolbox-0.3.9/AUTHORS
--rw-rw-rw-   0        0        0     1090 2022-01-27 21:21:40.000000 agstoolbox-0.3.9/COPYING
--rw-rw-rw-   0        0        0     1069 2023-04-07 14:40:56.000000 agstoolbox-0.3.9/LICENSE
--rw-rw-rw-   0        0        0      101 2023-04-08 20:06:59.000000 agstoolbox-0.3.9/MANIFEST.in
--rw-rw-rw-   0        0        0     1476 2023-04-09 22:39:34.273380 agstoolbox-0.3.9/PKG-INFO
--rw-rw-rw-   0        0        0      595 2023-04-07 14:56:20.000000 agstoolbox-0.3.9/README.rst
--rw-rw-rw-   0        0        0      386 2022-01-27 21:21:40.000000 agstoolbox-0.3.9/agstoolbox
--rw-rw-rw-   0        0        0      416 2023-04-08 22:53:12.000000 agstoolbox-0.3.9/atbx
--rw-rw-rw-   0        0        0     1561 2023-04-08 03:22:39.000000 agstoolbox-0.3.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-09 22:39:34.274381 agstoolbox-0.3.9/setup.cfg
--rw-rw-rw-   0        0        0     1960 2023-04-09 18:04:09.000000 agstoolbox-0.3.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-09 22:39:33.904020 agstoolbox-0.3.9/src/
-drwxrwxrwx   0        0        0        0 2023-04-09 22:39:33.955019 agstoolbox-0.3.9/src/agstoolbox/
--rw-rw-rw-   0        0        0      198 2023-04-09 22:34:19.000000 agstoolbox-0.3.9/src/agstoolbox/__init__.py
--rw-rw-rw-   0        0        0     1023 2023-04-09 03:43:47.000000 agstoolbox-0.3.9/src/agstoolbox/__main__.py
--rw-rw-rw-   0        0        0     1270 2022-02-06 18:41:53.000000 agstoolbox-0.3.9/src/agstoolbox/at_icons.py
--rw-rw-rw-   0        0        0     4322 2023-04-07 02:56:06.000000 agstoolbox-0.3.9/src/agstoolbox/at_tasks.py
--rw-rw-rw-   0        0        0     3874 2023-04-07 02:56:23.000000 agstoolbox-0.3.9/src/agstoolbox/at_trayindicator.py
-drwxrwxrwx   0        0        0        0 2023-04-09 22:39:33.971380 agstoolbox-0.3.9/src/agstoolbox/core/
--rw-rw-rw-   0        0        0        0 2022-01-27 21:22:20.000000 agstoolbox-0.3.9/src/agstoolbox/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 22:39:34.012380 agstoolbox-0.3.9/src/agstoolbox/core/ags/
--rw-rw-rw-   0        0        0        0 2022-01-27 21:21:40.000000 agstoolbox-0.3.9/src/agstoolbox/core/ags/__init__.py
--rw-rw-rw-   0        0        0      340 2023-04-09 03:06:08.000000 agstoolbox-0.3.9/src/agstoolbox/core/ags/ags_editor.py
--rw-rw-rw-   0        0        0   201168 2022-01-30 01:21:58.000000 agstoolbox-0.3.9/src/agstoolbox/core/ags/ags_editor_validation_data.py
--rw-rw-rw-   0        0        0      765 2023-04-09 17:26:51.000000 agstoolbox-0.3.9/src/agstoolbox/core/ags/ags_local_run.py
--rw-rw-rw-   0        0        0      361 2022-03-20 16:56:08.000000 agstoolbox-0.3.9/src/agstoolbox/core/ags/game_project.py
--rw-rw-rw-   0        0        0     3561 2023-04-09 03:08:16.000000 agstoolbox-0.3.9/src/agstoolbox/core/ags/get_game_projects.py
--rw-rw-rw-   0        0        0     2545 2023-04-07 21:27:44.000000 agstoolbox-0.3.9/src/agstoolbox/core/ags/get_local_ags_editors.py
--rw-rw-rw-   0        0        0     1328 2022-02-05 18:27:18.000000 agstoolbox-0.3.9/src/agstoolbox/core/ags/validate_ags_editor.py
-drwxrwxrwx   0        0        0        0 2023-04-09 22:39:34.026381 agstoolbox-0.3.9/src/agstoolbox/core/cmdline/
--rw-rw-rw-   0        0        0        0 2023-04-08 03:10:57.000000 agstoolbox-0.3.9/src/agstoolbox/core/cmdline/__init__.py
--rw-rw-rw-   0        0        0    13174 2023-04-09 22:32:59.000000 agstoolbox-0.3.9/src/agstoolbox/core/cmdline/cmdline.py
--rw-rw-rw-   0        0        0      742 2023-04-08 17:11:05.000000 agstoolbox-0.3.9/src/agstoolbox/core/cmdline/cmdline_download.py
--rw-rw-rw-   0        0        0     1506 2023-04-08 17:09:05.000000 agstoolbox-0.3.9/src/agstoolbox/core/cmdline/progress.py
-drwxrwxrwx   0        0        0        0 2023-04-09 22:39:34.048380 agstoolbox-0.3.9/src/agstoolbox/core/gh/
--rw-rw-rw-   0        0        0        0 2022-01-27 21:21:40.000000 agstoolbox-0.3.9/src/agstoolbox/core/gh/__init__.py
--rw-rw-rw-   0        0        0     1093 2023-04-08 02:50:16.000000 agstoolbox-0.3.9/src/agstoolbox/core/gh/download_release.py
--rw-rw-rw-   0        0        0     1115 2023-04-09 03:46:16.000000 agstoolbox-0.3.9/src/agstoolbox/core/gh/install_release.py
--rw-rw-rw-   0        0        0     3474 2023-04-08 02:44:10.000000 agstoolbox-0.3.9/src/agstoolbox/core/gh/list_releases.py
--rw-rw-rw-   0        0        0      497 2023-04-09 03:35:53.000000 agstoolbox-0.3.9/src/agstoolbox/core/gh/release.py
-drwxrwxrwx   0        0        0        0 2023-04-09 22:39:34.066380 agstoolbox-0.3.9/src/agstoolbox/core/settings/
--rw-rw-rw-   0        0        0        0 2023-04-07 00:44:47.000000 agstoolbox-0.3.9/src/agstoolbox/core/settings/__init__.py
--rw-rw-rw-   0        0        0     5600 2023-04-08 22:11:07.000000 agstoolbox-0.3.9/src/agstoolbox/core/settings/settings.py
--rw-rw-rw-   0        0        0      287 2023-04-09 03:39:13.000000 agstoolbox-0.3.9/src/agstoolbox/core/settings/settings_data.py
--rw-rw-rw-   0        0        0     2286 2023-04-07 02:36:47.000000 agstoolbox-0.3.9/src/agstoolbox/core/settings/settings_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-09 22:39:34.143379 agstoolbox-0.3.9/src/agstoolbox/core/utils/
--rw-rw-rw-   0        0        0        0 2022-01-27 21:23:07.000000 agstoolbox-0.3.9/src/agstoolbox/core/utils/__init__.py
--rw-rw-rw-   0        0        0      796 2023-04-07 01:04:11.000000 agstoolbox-0.3.9/src/agstoolbox/core/utils/basics.py
--rw-rw-rw-   0        0        0      797 2023-04-08 02:50:26.000000 agstoolbox-0.3.9/src/agstoolbox/core/utils/downloader.py
--rw-rw-rw-   0        0        0     4626 2023-04-09 17:11:59.000000 agstoolbox-0.3.9/src/agstoolbox/core/utils/file.py
--rw-rw-rw-   0        0        0      139 2022-01-27 21:57:07.000000 agstoolbox-0.3.9/src/agstoolbox/core/utils/math.py
--rw-rw-rw-   0        0        0       99 2023-04-05 02:07:05.000000 agstoolbox-0.3.9/src/agstoolbox/core/utils/open_in_browser.py
--rw-rw-rw-   0        0        0     1581 2022-01-29 21:55:33.000000 agstoolbox-0.3.9/src/agstoolbox/core/utils/pe.py
--rw-rw-rw-   0        0        0      508 2023-04-09 17:25:55.000000 agstoolbox-0.3.9/src/agstoolbox/core/utils/run.py
--rw-rw-rw-   0        0        0      246 2022-01-27 21:21:40.000000 agstoolbox-0.3.9/src/agstoolbox/core/utils/singleton.py
--rw-rw-rw-   0        0        0     1836 2023-04-07 02:47:18.000000 agstoolbox-0.3.9/src/agstoolbox/core/utils/startup.py
--rw-rw-rw-   0        0        0      641 2023-04-08 16:41:22.000000 agstoolbox-0.3.9/src/agstoolbox/core/utils/systemdirs.py
--rw-rw-rw-   0        0        0     1008 2023-04-09 03:44:30.000000 agstoolbox-0.3.9/src/agstoolbox/core/utils/time.py
--rw-rw-rw-   0        0        0     1256 2023-04-09 03:44:51.000000 agstoolbox-0.3.9/src/agstoolbox/core/utils/win_registry.py
-drwxrwxrwx   0        0        0        0 2023-04-09 22:39:34.155379 agstoolbox-0.3.9/src/agstoolbox/core/version/
--rw-rw-rw-   0        0        0        0 2022-03-20 16:16:18.000000 agstoolbox-0.3.9/src/agstoolbox/core/version/__init__.py
--rw-rw-rw-   0        0        0      258 2023-04-08 01:38:27.000000 agstoolbox-0.3.9/src/agstoolbox/core/version/version.py
--rw-rw-rw-   0        0        0     3313 2023-04-08 01:43:53.000000 agstoolbox-0.3.9/src/agstoolbox/core/version/version_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-09 22:39:34.190379 agstoolbox-0.3.9/src/agstoolbox/data/
--rw-rw-rw-   0        0        0     6036 2022-02-06 18:38:23.000000 agstoolbox-0.3.9/src/agstoolbox/data/at_ags_editor_icon.png
--rw-rw-rw-   0        0        0    53039 2022-01-27 21:21:40.000000 agstoolbox-0.3.9/src/agstoolbox/data/at_ags_engine_icon.png
--rw-rw-rw-   0        0        0     4571 2022-02-06 18:46:17.000000 agstoolbox-0.3.9/src/agstoolbox/data/at_icon.png
--rw-rw-rw-   0        0        0    74585 2022-02-06 18:32:22.000000 agstoolbox-0.3.9/src/agstoolbox/data/at_icon_big.png
--rw-rw-rw-   0        0        0     4036 2022-01-25 11:12:32.000000 agstoolbox-0.3.9/src/agstoolbox/data/exit_icon.png
--rw-rw-rw-   0        0        0     2449 2022-01-25 11:11:19.000000 agstoolbox-0.3.9/src/agstoolbox/data/refresh_icon.png
--rw-rw-rw-   0        0        0     6912 2022-01-25 11:17:17.000000 agstoolbox-0.3.9/src/agstoolbox/data/settings_icon.png
--rw-rw-rw-   0        0        0      538 2022-01-27 21:21:40.000000 agstoolbox-0.3.9/src/agstoolbox/getdata.py
-drwxrwxrwx   0        0        0        0 2023-04-09 22:39:34.203379 agstoolbox-0.3.9/src/agstoolbox/panels/
--rw-rw-rw-   0        0        0        0 2022-01-27 21:21:40.000000 agstoolbox-0.3.9/src/agstoolbox/panels/__init__.py
--rw-rw-rw-   0        0        0     5446 2023-04-07 02:51:49.000000 agstoolbox-0.3.9/src/agstoolbox/panels/at_mainpanel.py
--rw-rw-rw-   0        0        0     7533 2023-04-09 03:39:22.000000 agstoolbox-0.3.9/src/agstoolbox/panels/at_settings_dialog.py
-drwxrwxrwx   0        0        0        0 2023-04-09 22:39:34.214383 agstoolbox-0.3.9/src/agstoolbox/system/
--rw-rw-rw-   0        0        0        0 2023-04-02 19:34:00.000000 agstoolbox-0.3.9/src/agstoolbox/system/__init__.py
--rw-rw-rw-   0        0        0      394 2023-04-02 20:12:53.000000 agstoolbox-0.3.9/src/agstoolbox/system/at_runguard.py
--rw-rw-rw-   0        0        0     1210 2023-04-03 00:55:58.000000 agstoolbox-0.3.9/src/agstoolbox/system/at_unique_application.py
-drwxrwxrwx   0        0        0        0 2023-04-09 22:39:34.252382 agstoolbox-0.3.9/src/agstoolbox/wdgts/
--rw-rw-rw-   0        0        0        0 2022-01-27 21:21:40.000000 agstoolbox-0.3.9/src/agstoolbox/wdgts/__init__.py
--rw-rw-rw-   0        0        0     7381 2023-04-09 03:39:13.000000 agstoolbox-0.3.9/src/agstoolbox/wdgts/at_dirlist_wdgt.py
--rw-rw-rw-   0        0        0     2510 2023-04-09 03:40:47.000000 agstoolbox-0.3.9/src/agstoolbox/wdgts/at_single_dir_wdgt.py
--rw-rw-rw-   0        0        0     6290 2023-04-09 16:00:52.000000 agstoolbox-0.3.9/src/agstoolbox/wdgts/at_tree_item_project.py
--rw-rw-rw-   0        0        0     8291 2023-04-05 02:14:45.000000 agstoolbox-0.3.9/src/agstoolbox/wdgts/at_tree_item_tool.py
--rw-rw-rw-   0        0        0     1428 2023-04-04 01:42:57.000000 agstoolbox-0.3.9/src/agstoolbox/wdgts/at_tree_projects_wdgt.py
--rw-rw-rw-   0        0        0     7062 2023-04-09 15:59:58.000000 agstoolbox-0.3.9/src/agstoolbox/wdgts/at_tree_tools_wdgt.py
-drwxrwxrwx   0        0        0        0 2023-04-09 22:39:34.272379 agstoolbox-0.3.9/src/agstoolbox/wdgts_utils/
--rw-rw-rw-   0        0        0        0 2022-04-27 23:21:51.000000 agstoolbox-0.3.9/src/agstoolbox/wdgts_utils/__init__.py
--rw-rw-rw-   0        0        0      358 2022-04-27 23:30:17.000000 agstoolbox-0.3.9/src/agstoolbox/wdgts_utils/action_utils.py
--rw-rw-rw-   0        0        0      467 2022-04-27 23:52:03.000000 agstoolbox-0.3.9/src/agstoolbox/wdgts_utils/ags_local_extra.py
--rw-rw-rw-   0        0        0      899 2022-04-27 23:49:42.000000 agstoolbox-0.3.9/src/agstoolbox/wdgts_utils/file_explorer.py
--rw-rw-rw-   0        0        0      149 2023-04-02 23:02:36.000000 agstoolbox-0.3.9/src/agstoolbox/wdgts_utils/get_self_path.py
-drwxrwxrwx   0        0        0        0 2023-04-09 22:39:33.970379 agstoolbox-0.3.9/src/agstoolbox.egg-info/
--rw-rw-rw-   0        0        0     1476 2023-04-09 22:39:33.000000 agstoolbox-0.3.9/src/agstoolbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2975 2023-04-09 22:39:33.000000 agstoolbox-0.3.9/src/agstoolbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 22:39:33.000000 agstoolbox-0.3.9/src/agstoolbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-04-09 22:39:33.000000 agstoolbox-0.3.9/src/agstoolbox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-09 22:39:33.000000 agstoolbox-0.3.9/src/agstoolbox.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 13:07:04.398613 agstoolbox-0.4.0/
+-rw-rw-rw-   0        0        0       33 2022-01-27 21:21:40.000000 agstoolbox-0.4.0/AUTHORS
+-rw-rw-rw-   0        0        0     1090 2022-01-27 21:21:40.000000 agstoolbox-0.4.0/COPYING
+-rw-rw-rw-   0        0        0     1069 2023-04-07 14:40:56.000000 agstoolbox-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0      135 2023-04-16 03:30:53.000000 agstoolbox-0.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1476 2023-04-16 13:07:04.397613 agstoolbox-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0      595 2023-04-07 14:56:20.000000 agstoolbox-0.4.0/README.rst
+-rw-rw-rw-   0        0        0      386 2022-01-27 21:21:40.000000 agstoolbox-0.4.0/agstoolbox
+-rw-rw-rw-   0        0        0      416 2023-04-08 22:53:12.000000 agstoolbox-0.4.0/atbx
+-rw-rw-rw-   0        0        0     1561 2023-04-08 03:22:39.000000 agstoolbox-0.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-16 13:07:04.398613 agstoolbox-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     2044 2023-04-16 03:30:53.000000 agstoolbox-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:07:04.024420 agstoolbox-0.4.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-16 13:07:04.084417 agstoolbox-0.4.0/src/agstoolbox/
+-rw-rw-rw-   0        0        0      198 2023-04-16 03:32:00.000000 agstoolbox-0.4.0/src/agstoolbox/__init__.py
+-rw-rw-rw-   0        0        0     1023 2023-04-09 03:43:47.000000 agstoolbox-0.4.0/src/agstoolbox/__main__.py
+-rw-rw-rw-   0        0        0      880 2023-04-16 03:30:53.000000 agstoolbox-0.4.0/src/agstoolbox/at_fonts.py
+-rw-rw-rw-   0        0        0     1321 2023-04-15 17:09:11.000000 agstoolbox-0.4.0/src/agstoolbox/at_icons.py
+-rw-rw-rw-   0        0        0     4322 2023-04-07 02:56:06.000000 agstoolbox-0.4.0/src/agstoolbox/at_tasks.py
+-rw-rw-rw-   0        0        0     4065 2023-04-16 03:30:53.000000 agstoolbox-0.4.0/src/agstoolbox/at_trayindicator.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:07:04.100419 agstoolbox-0.4.0/src/agstoolbox/core/
+-rw-rw-rw-   0        0        0        0 2022-01-27 21:22:20.000000 agstoolbox-0.4.0/src/agstoolbox/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:07:04.139417 agstoolbox-0.4.0/src/agstoolbox/core/ags/
+-rw-rw-rw-   0        0        0        0 2022-01-27 21:21:40.000000 agstoolbox-0.4.0/src/agstoolbox/core/ags/__init__.py
+-rw-rw-rw-   0        0        0      340 2023-04-09 03:06:08.000000 agstoolbox-0.4.0/src/agstoolbox/core/ags/ags_editor.py
+-rw-rw-rw-   0        0        0   201168 2022-01-30 01:21:58.000000 agstoolbox-0.4.0/src/agstoolbox/core/ags/ags_editor_validation_data.py
+-rw-rw-rw-   0        0        0      851 2023-04-09 22:51:01.000000 agstoolbox-0.4.0/src/agstoolbox/core/ags/ags_local_run.py
+-rw-rw-rw-   0        0        0      446 2023-04-16 03:30:53.000000 agstoolbox-0.4.0/src/agstoolbox/core/ags/game_project.py
+-rw-rw-rw-   0        0        0     3875 2023-04-16 03:30:53.000000 agstoolbox-0.4.0/src/agstoolbox/core/ags/get_game_projects.py
+-rw-rw-rw-   0        0        0     2545 2023-04-07 21:27:44.000000 agstoolbox-0.4.0/src/agstoolbox/core/ags/get_local_ags_editors.py
+-rw-rw-rw-   0        0        0     1328 2022-02-05 18:27:18.000000 agstoolbox-0.4.0/src/agstoolbox/core/ags/validate_ags_editor.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:07:04.157417 agstoolbox-0.4.0/src/agstoolbox/core/cmdline/
+-rw-rw-rw-   0        0        0        0 2023-04-08 03:10:57.000000 agstoolbox-0.4.0/src/agstoolbox/core/cmdline/__init__.py
+-rw-rw-rw-   0        0        0    13763 2023-04-09 22:54:35.000000 agstoolbox-0.4.0/src/agstoolbox/core/cmdline/cmdline.py
+-rw-rw-rw-   0        0        0      853 2023-04-09 22:47:08.000000 agstoolbox-0.4.0/src/agstoolbox/core/cmdline/cmdline_download.py
+-rw-rw-rw-   0        0        0     1506 2023-04-08 17:09:05.000000 agstoolbox-0.4.0/src/agstoolbox/core/cmdline/progress.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:07:04.180613 agstoolbox-0.4.0/src/agstoolbox/core/gh/
+-rw-rw-rw-   0        0        0        0 2022-01-27 21:21:40.000000 agstoolbox-0.4.0/src/agstoolbox/core/gh/__init__.py
+-rw-rw-rw-   0        0        0     1093 2023-04-08 02:50:16.000000 agstoolbox-0.4.0/src/agstoolbox/core/gh/download_release.py
+-rw-rw-rw-   0        0        0     1115 2023-04-09 03:46:16.000000 agstoolbox-0.4.0/src/agstoolbox/core/gh/install_release.py
+-rw-rw-rw-   0        0        0     3559 2023-04-10 02:51:20.000000 agstoolbox-0.4.0/src/agstoolbox/core/gh/list_releases.py
+-rw-rw-rw-   0        0        0      497 2023-04-09 03:35:53.000000 agstoolbox-0.4.0/src/agstoolbox/core/gh/release.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:07:04.196612 agstoolbox-0.4.0/src/agstoolbox/core/settings/
+-rw-rw-rw-   0        0        0        0 2023-04-07 00:44:47.000000 agstoolbox-0.4.0/src/agstoolbox/core/settings/__init__.py
+-rw-rw-rw-   0        0        0     5600 2023-04-08 22:11:07.000000 agstoolbox-0.4.0/src/agstoolbox/core/settings/settings.py
+-rw-rw-rw-   0        0        0      287 2023-04-09 03:39:13.000000 agstoolbox-0.4.0/src/agstoolbox/core/settings/settings_data.py
+-rw-rw-rw-   0        0        0     2286 2023-04-07 02:36:47.000000 agstoolbox-0.4.0/src/agstoolbox/core/settings/settings_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:07:04.270613 agstoolbox-0.4.0/src/agstoolbox/core/utils/
+-rw-rw-rw-   0        0        0        0 2022-01-27 21:23:07.000000 agstoolbox-0.4.0/src/agstoolbox/core/utils/__init__.py
+-rw-rw-rw-   0        0        0      796 2023-04-07 01:04:11.000000 agstoolbox-0.4.0/src/agstoolbox/core/utils/basics.py
+-rw-rw-rw-   0        0        0      797 2023-04-08 02:50:26.000000 agstoolbox-0.4.0/src/agstoolbox/core/utils/downloader.py
+-rw-rw-rw-   0        0        0     4626 2023-04-09 17:11:59.000000 agstoolbox-0.4.0/src/agstoolbox/core/utils/file.py
+-rw-rw-rw-   0        0        0      139 2022-01-27 21:57:07.000000 agstoolbox-0.4.0/src/agstoolbox/core/utils/math.py
+-rw-rw-rw-   0        0        0       99 2023-04-05 02:07:05.000000 agstoolbox-0.4.0/src/agstoolbox/core/utils/open_in_browser.py
+-rw-rw-rw-   0        0        0     1581 2022-01-29 21:55:33.000000 agstoolbox-0.4.0/src/agstoolbox/core/utils/pe.py
+-rw-rw-rw-   0        0        0      791 2023-04-09 23:06:08.000000 agstoolbox-0.4.0/src/agstoolbox/core/utils/run.py
+-rw-rw-rw-   0        0        0      246 2022-01-27 21:21:40.000000 agstoolbox-0.4.0/src/agstoolbox/core/utils/singleton.py
+-rw-rw-rw-   0        0        0     1836 2023-04-07 02:47:18.000000 agstoolbox-0.4.0/src/agstoolbox/core/utils/startup.py
+-rw-rw-rw-   0        0        0      641 2023-04-08 16:41:22.000000 agstoolbox-0.4.0/src/agstoolbox/core/utils/systemdirs.py
+-rw-rw-rw-   0        0        0     1008 2023-04-09 03:44:30.000000 agstoolbox-0.4.0/src/agstoolbox/core/utils/time.py
+-rw-rw-rw-   0        0        0     1256 2023-04-09 03:44:51.000000 agstoolbox-0.4.0/src/agstoolbox/core/utils/win_registry.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:07:04.281614 agstoolbox-0.4.0/src/agstoolbox/core/version/
+-rw-rw-rw-   0        0        0        0 2022-03-20 16:16:18.000000 agstoolbox-0.4.0/src/agstoolbox/core/version/__init__.py
+-rw-rw-rw-   0        0        0      258 2023-04-08 01:38:27.000000 agstoolbox-0.4.0/src/agstoolbox/core/version/version.py
+-rw-rw-rw-   0        0        0     3313 2023-04-08 01:43:53.000000 agstoolbox-0.4.0/src/agstoolbox/core/version/version_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:07:04.313614 agstoolbox-0.4.0/src/agstoolbox/data/
+-rw-rw-rw-   0        0        0     6036 2022-02-06 18:38:23.000000 agstoolbox-0.4.0/src/agstoolbox/data/at_ags_editor_icon.png
+-rw-rw-rw-   0        0        0    53039 2022-01-27 21:21:40.000000 agstoolbox-0.4.0/src/agstoolbox/data/at_ags_engine_icon.png
+-rw-rw-rw-   0        0        0     4571 2022-02-06 18:46:17.000000 agstoolbox-0.4.0/src/agstoolbox/data/at_icon.png
+-rw-rw-rw-   0        0        0    74585 2022-02-06 18:32:22.000000 agstoolbox-0.4.0/src/agstoolbox/data/at_icon_big.png
+-rw-rw-rw-   0        0        0     4036 2022-01-25 11:12:32.000000 agstoolbox-0.4.0/src/agstoolbox/data/exit_icon.png
+drwxrwxrwx   0        0        0        0 2023-04-16 13:07:04.314615 agstoolbox-0.4.0/src/agstoolbox/data/fonts/
+-rw-rw-rw-   0        0        0   211576 2023-04-16 03:30:53.000000 agstoolbox-0.4.0/src/agstoolbox/data/fonts/Beedii.ttf
+-rw-rw-rw-   0        0        0     2449 2022-01-25 11:11:19.000000 agstoolbox-0.4.0/src/agstoolbox/data/refresh_icon.png
+-rw-rw-rw-   0        0        0     6912 2022-01-25 11:17:17.000000 agstoolbox-0.4.0/src/agstoolbox/data/settings_icon.png
+-rw-rw-rw-   0        0        0      538 2022-01-27 21:21:40.000000 agstoolbox-0.4.0/src/agstoolbox/getdata.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:07:04.326613 agstoolbox-0.4.0/src/agstoolbox/panels/
+-rw-rw-rw-   0        0        0        0 2022-01-27 21:21:40.000000 agstoolbox-0.4.0/src/agstoolbox/panels/__init__.py
+-rw-rw-rw-   0        0        0     6853 2023-04-16 03:30:53.000000 agstoolbox-0.4.0/src/agstoolbox/panels/at_mainpanel.py
+-rw-rw-rw-   0        0        0     7533 2023-04-09 03:39:22.000000 agstoolbox-0.4.0/src/agstoolbox/panels/at_settings_dialog.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:07:04.337613 agstoolbox-0.4.0/src/agstoolbox/system/
+-rw-rw-rw-   0        0        0        0 2023-04-02 19:34:00.000000 agstoolbox-0.4.0/src/agstoolbox/system/__init__.py
+-rw-rw-rw-   0        0        0      394 2023-04-02 20:12:53.000000 agstoolbox-0.4.0/src/agstoolbox/system/at_runguard.py
+-rw-rw-rw-   0        0        0     1210 2023-04-03 00:55:58.000000 agstoolbox-0.4.0/src/agstoolbox/system/at_unique_application.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:07:04.377613 agstoolbox-0.4.0/src/agstoolbox/wdgts/
+-rw-rw-rw-   0        0        0        0 2022-01-27 21:21:40.000000 agstoolbox-0.4.0/src/agstoolbox/wdgts/__init__.py
+-rw-rw-rw-   0        0        0     7381 2023-04-09 03:39:13.000000 agstoolbox-0.4.0/src/agstoolbox/wdgts/at_dirlist_wdgt.py
+-rw-rw-rw-   0        0        0     3894 2023-04-16 03:30:53.000000 agstoolbox-0.4.0/src/agstoolbox/wdgts/at_searchedit.py
+-rw-rw-rw-   0        0        0     2510 2023-04-09 03:40:47.000000 agstoolbox-0.4.0/src/agstoolbox/wdgts/at_single_dir_wdgt.py
+-rw-rw-rw-   0        0        0     6290 2023-04-09 16:00:52.000000 agstoolbox-0.4.0/src/agstoolbox/wdgts/at_tree_item_project.py
+-rw-rw-rw-   0        0        0     8825 2023-04-16 03:30:53.000000 agstoolbox-0.4.0/src/agstoolbox/wdgts/at_tree_item_tool.py
+-rw-rw-rw-   0        0        0     2318 2023-04-16 03:30:53.000000 agstoolbox-0.4.0/src/agstoolbox/wdgts/at_tree_projects_wdgt.py
+-rw-rw-rw-   0        0        0     9183 2023-04-16 03:30:53.000000 agstoolbox-0.4.0/src/agstoolbox/wdgts/at_tree_tools_wdgt.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:07:04.396613 agstoolbox-0.4.0/src/agstoolbox/wdgts_utils/
+-rw-rw-rw-   0        0        0        0 2022-04-27 23:21:51.000000 agstoolbox-0.4.0/src/agstoolbox/wdgts_utils/__init__.py
+-rw-rw-rw-   0        0        0      358 2022-04-27 23:30:17.000000 agstoolbox-0.4.0/src/agstoolbox/wdgts_utils/action_utils.py
+-rw-rw-rw-   0        0        0      467 2022-04-27 23:52:03.000000 agstoolbox-0.4.0/src/agstoolbox/wdgts_utils/ags_local_extra.py
+-rw-rw-rw-   0        0        0      899 2022-04-27 23:49:42.000000 agstoolbox-0.4.0/src/agstoolbox/wdgts_utils/file_explorer.py
+-rw-rw-rw-   0        0        0      149 2023-04-02 23:02:36.000000 agstoolbox-0.4.0/src/agstoolbox/wdgts_utils/get_self_path.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:07:04.099421 agstoolbox-0.4.0/src/agstoolbox.egg-info/
+-rw-rw-rw-   0        0        0     1476 2023-04-16 13:07:03.000000 agstoolbox-0.4.0/src/agstoolbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3077 2023-04-16 13:07:04.000000 agstoolbox-0.4.0/src/agstoolbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 13:07:03.000000 agstoolbox-0.4.0/src/agstoolbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-04-16 13:07:03.000000 agstoolbox-0.4.0/src/agstoolbox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-16 13:07:03.000000 agstoolbox-0.4.0/src/agstoolbox.egg-info/top_level.txt
```

### Comparing `agstoolbox-0.3.9/COPYING` & `agstoolbox-0.4.0/COPYING`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.9/LICENSE` & `agstoolbox-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.9/PKG-INFO` & `agstoolbox-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: agstoolbox
-Version: 0.3.9
+Version: 0.4.0
 Summary: Utility to help manage Adventure Game Studio Projects and Editors.
 Home-page: https://github.com/ericoporto/agstoolbox
-Download-URL: https://github.com/ericoporto/agstoolbox/tarball/0.3.9
+Download-URL: https://github.com/ericoporto/agstoolbox/tarball/0.4.0
 Author: erico
 Author-email: eri0onpm@gmail.com
 License: MIT
 Keywords: AGS Toolbox,Adventure Game Studio,development,ags,Game Development,gamedev
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `agstoolbox-0.3.9/README.rst` & `agstoolbox-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.9/pyproject.toml` & `agstoolbox-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.9/setup.py` & `agstoolbox-0.4.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-from codecs import open
-from pathlib import Path
-
-from setuptools import setup, find_packages
-import re
-
-with open('src/agstoolbox/__init__.py', 'r') as fd:
-    version = re.search(r'^__version__\s*=\s*[\'"]([^\'"]*)[\'"]',
-                        fd.read(), re.MULTILINE).group(1)
-
-this_directory = Path(__file__).parent
-long_description = (this_directory / "README.rst").read_text()
-
-setup(
-    name='agstoolbox',
-    version=version,
-    description='Utility to help manage Adventure Game Studio Projects and Editors.',
-    long_description=long_description,
-    url='https://github.com/ericoporto/agstoolbox',
-    download_url='https://github.com/ericoporto/agstoolbox/tarball/' + version,
-    author='erico',
-    author_email='eri0onpm@gmail.com',
-    license='MIT',
-    classifiers=[
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-        'Programming Language :: Python :: 3 :: Only'
-    ],
-    keywords=[
-        'AGS Toolbox', 'Adventure Game Studio', 'development', 'ags', 'Game Development', 'gamedev'
-    ],
-    python_requires='>=3.8',
-    install_requires=[
-        'pyqt6',
-        'requests',
-        'defusedxml',
-        'platformdirs',
-        'pefile',
-        'shtab'
-    ],
-    packages=[
-        'agstoolbox',
-        'agstoolbox.core',
-        'agstoolbox.core.ags',
-        'agstoolbox.core.cmdline',
-        'agstoolbox.core.gh',
-        'agstoolbox.core.settings',
-        'agstoolbox.core.utils',
-        'agstoolbox.core.version',
-        'agstoolbox.panels',
-        'agstoolbox.system',
-        'agstoolbox.wdgts',
-        'agstoolbox.wdgts_utils'
-    ],
-    package_dir={"": "src"},
-    scripts=["agstoolbox", "atbx"],
-    package_data={
-        'agstoolbox': ['data/*.png']
-    },
-)
+from codecs import open
+from pathlib import Path
+
+from setuptools import setup, find_packages
+import re
+
+with open('src/agstoolbox/__init__.py', 'r') as fd:
+    version = re.search(r'^__version__\s*=\s*[\'"]([^\'"]*)[\'"]',
+                        fd.read(), re.MULTILINE).group(1)
+
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.rst").read_text()
+
+setup(
+    name='agstoolbox',
+    version=version,
+    description='Utility to help manage Adventure Game Studio Projects and Editors.',
+    long_description=long_description,
+    url='https://github.com/ericoporto/agstoolbox',
+    download_url='https://github.com/ericoporto/agstoolbox/tarball/' + version,
+    author='erico',
+    author_email='eri0onpm@gmail.com',
+    license='MIT',
+    classifiers=[
+        'Intended Audience :: Developers',
+        'License :: OSI Approved :: MIT License',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3 :: Only'
+    ],
+    keywords=[
+        'AGS Toolbox', 'Adventure Game Studio', 'development', 'ags', 'Game Development', 'gamedev'
+    ],
+    python_requires='>=3.8',
+    install_requires=[
+        'pyqt6',
+        'requests',
+        'defusedxml',
+        'platformdirs',
+        'pefile',
+        'shtab'
+    ],
+    packages=[
+        'agstoolbox',
+        'agstoolbox.core',
+        'agstoolbox.core.ags',
+        'agstoolbox.core.cmdline',
+        'agstoolbox.core.gh',
+        'agstoolbox.core.settings',
+        'agstoolbox.core.utils',
+        'agstoolbox.core.version',
+        'agstoolbox.panels',
+        'agstoolbox.system',
+        'agstoolbox.wdgts',
+        'agstoolbox.wdgts_utils'
+    ],
+    package_dir={"": "src"},
+    scripts=["agstoolbox", "atbx"],
+    package_data={
+        'agstoolbox': ['data/*.png', 'data/fonts/*.ttf']
+    },
+)
```

### Comparing `agstoolbox-0.3.9/src/agstoolbox/__main__.py` & `agstoolbox-0.4.0/src/agstoolbox/__main__.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.9/src/agstoolbox/at_icons.py` & `agstoolbox-0.4.0/src/agstoolbox/at_icons.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-from PyQt6 import QtGui
-
-from agstoolbox import getdata
-
-
-def main_icon() -> QtGui.QIcon:
-    return QtGui.QIcon(getdata.path('at_icon.png'))
-
-
-def main_icon_as_pixmap() -> QtGui.QPixmap:
-    return QtGui.QPixmap(getdata.path('at_icon.png'))
-
-
-def ags_editor_icon() -> QtGui.QIcon:
-    return QtGui.QIcon(getdata.path('at_ags_editor_icon.png'))
-
-
-def ags_editor_as_pixmap() -> QtGui.QPixmap:
-    return QtGui.QPixmap(getdata.path('at_ags_editor_icon.png'))
-
-
-def ags_engine_icon() -> QtGui.QIcon:
-    return QtGui.QIcon(getdata.path('at_ags_engine_icon.png'))
-
-
-def ags_engine_as_pixmap() -> QtGui.QPixmap:
-    return QtGui.QPixmap(getdata.path('at_ags_engine_icon.png'))
-
-
-def icon_refresh() -> QtGui.QIcon:
-    return QtGui.QIcon(getdata.path('refresh_icon.png'))
-
-
-def icon_exit() -> QtGui.QIcon:
-    return QtGui.QIcon(getdata.path('exit_icon.png'))
-
-
-def icon_settings() -> QtGui.QIcon:
-    return QtGui.QIcon(getdata.path('settings_icon.png'))
-
-
-def icon_refresh_as_pixmap() -> QtGui.QPixmap:
-    return QtGui.QPixmap(getdata.path('refresh_icon.png'))
-
-
-def icon_exit_as_pixmap() -> QtGui.QPixmap:
-    return QtGui.QPixmap(getdata.path('exit_icon.png'))
-
-
-def icon_settings_as_pixmap() -> QtGui.QPixmap:
-    return QtGui.QPixmap(getdata.path('settings_icon.png'))
+from PyQt6 import QtGui
+
+from agstoolbox import getdata
+
+
+def main_icon() -> QtGui.QIcon:
+    return QtGui.QIcon(getdata.path('at_icon.png'))
+
+
+def main_icon_as_pixmap() -> QtGui.QPixmap:
+    return QtGui.QPixmap(getdata.path('at_icon.png'))
+
+
+def ags_editor_icon() -> QtGui.QIcon:
+    return QtGui.QIcon(getdata.path('at_ags_editor_icon.png'))
+
+
+def ags_editor_as_pixmap() -> QtGui.QPixmap:
+    return QtGui.QPixmap(getdata.path('at_ags_editor_icon.png'))
+
+
+def ags_engine_icon() -> QtGui.QIcon:
+    return QtGui.QIcon(getdata.path('at_ags_engine_icon.png'))
+
+
+def ags_engine_as_pixmap() -> QtGui.QPixmap:
+    return QtGui.QPixmap(getdata.path('at_ags_engine_icon.png'))
+
+
+def icon_refresh() -> QtGui.QIcon:
+    return QtGui.QIcon(getdata.path('refresh_icon.png'))
+
+
+def icon_exit() -> QtGui.QIcon:
+    return QtGui.QIcon(getdata.path('exit_icon.png'))
+
+
+def icon_settings() -> QtGui.QIcon:
+    return QtGui.QIcon(getdata.path('settings_icon.png'))
+
+
+def icon_refresh_as_pixmap() -> QtGui.QPixmap:
+    return QtGui.QPixmap(getdata.path('refresh_icon.png'))
+
+
+def icon_exit_as_pixmap() -> QtGui.QPixmap:
+    return QtGui.QPixmap(getdata.path('exit_icon.png'))
+
+
+def icon_settings_as_pixmap() -> QtGui.QPixmap:
+    return QtGui.QPixmap(getdata.path('settings_icon.png'))
```

### Comparing `agstoolbox-0.3.9/src/agstoolbox/at_tasks.py` & `agstoolbox-0.4.0/src/agstoolbox/at_tasks.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.9/src/agstoolbox/at_trayindicator.py` & `agstoolbox-0.4.0/src/agstoolbox/at_trayindicator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,111 +1,113 @@
-from sys import exit
-from PyQt6 import QtWidgets, QtCore, QtGui
-from PyQt6.QtCore import QTimer
-from PyQt6.QtWidgets import QSystemTrayIcon
-
-from agstoolbox.panels.at_mainpanel import MainWindow
-from agstoolbox.at_icons import main_icon
-from agstoolbox.core.settings.settings import ConstSettings
-from agstoolbox import __title__
-from agstoolbox.core.utils.math import clamp
-from agstoolbox.system.at_unique_application import unique_application
-
-
-class AtTrayIcon(QtWidgets.QSystemTrayIcon):
-
-    def __init__(self, icon, parent=None):
-        QtWidgets.QSystemTrayIcon.__init__(self, icon, parent)
-        self.window = MainWindow()
-        self.window.refresh_all()
-        menu = QtWidgets.QMenu(parent)
-
-        self.activated.connect(self.onTrayIconActivated)
-
-        action_open_toolbox = QtGui.QAction('Open Toolbox', self)
-        action_open_toolbox.triggered.connect(self.open_toolbox)  # load main panel
-
-        action_quit_toolbox = QtGui.QAction('Quit Toolbox', self)
-        action_quit_toolbox.triggered.connect(self.exit)
-
-        menu.addAction(action_open_toolbox)
-        menu.addAction(action_quit_toolbox)
-        self.setContextMenu(menu)
-
-        self.disambiguateTimer = QTimer(self)
-        self.disambiguateTimer.setSingleShot(True)
-        self.disambiguateTimer.timeout.connect(self.disambiguateTimerTimeout)
-
-    def exit(self):
-        QtCore.QCoreApplication.exit()
-
-    def open_toolbox(self):
-        tray_icon_rect = self.geometry()
-        window_pos = QtCore.QRect()
-        window_pos.setSize(QtCore.QSize(
-            ConstSettings().DEFAULT_MAIN_PANEL_WIDTH,
-            ConstSettings().DEFAULT_MAIN_PANEL_HEIGHT
-        ))
-
-        available_geometry = QtGui.QGuiApplication.primaryScreen().availableGeometry()
-
-        pos_x = clamp(tray_icon_rect.x(),
-                      available_geometry.x() + 48,
-                      available_geometry.width() - available_geometry.x() -
-                      window_pos.width() - 48)
-        pos_y = clamp(tray_icon_rect.y(),
-                      available_geometry.y() + 48,
-                      available_geometry.height() - available_geometry.y() -
-                      window_pos.height() - 48)
-
-        window_pos.setX(pos_x)
-        window_pos.setY(pos_y)
-        self.window.setGeometry(window_pos)
-        self.window.setWindowState(
-            self.window.windowState() &
-            ~QtCore.Qt.WindowState.WindowMinimized | QtCore.Qt.WindowState.WindowActive)
-        self.window.raise_()
-        self.window.show()
-        self.window.activateWindow()
-
-    def single_clicked(self):
-        self.open_toolbox()
-
-    def double_clicked(self):
-        self.open_toolbox()
-
-    def onTrayIconActivated(self, reason):
-        if reason == QSystemTrayIcon.ActivationReason.Trigger:
-            self.disambiguateTimer.start(ConstSettings().double_click_interval)
-        elif reason == QSystemTrayIcon.ActivationReason.DoubleClick:
-            self.disambiguateTimer.stop()
-            self.double_clicked()
-
-    def disambiguateTimerTimeout(self):
-        self.single_clicked()
-
-
-class UniqueWidget(QtWidgets.QWidget):
-    def __init__(self):
-        super().__init__()
-        QtWidgets.QApplication.instance().another_instance.connect(self.another_instance)
-
-    def another_instance(self):
-        self.findChild(AtTrayIcon, __title__).open_toolbox()
-
-
-def run_tray_indicator(ap_args):
-    app = unique_application(__title__, ap_args)
-    if not app.is_unique:
-        app.exit()
-        exit(1)
-
-    # this prevents the tray to close if the main panel is closed,
-    # we only exit when quit is explicitly clicked
-    app.setQuitOnLastWindowClosed(False)
-    ConstSettings().double_click_interval = app.doubleClickInterval()
-
-    w = UniqueWidget()
-    tray_icon = AtTrayIcon(main_icon(), w)
-    tray_icon.setObjectName(__title__)
-    tray_icon.show()
-    exit(app.exec())
+from sys import exit
+from PyQt6 import QtWidgets, QtCore, QtGui
+from PyQt6.QtCore import QTimer
+from PyQt6.QtWidgets import QSystemTrayIcon
+
+from agstoolbox.at_fonts import set_custom_fonts
+from agstoolbox.panels.at_mainpanel import MainWindow
+from agstoolbox.at_icons import main_icon
+from agstoolbox.core.settings.settings import ConstSettings
+from agstoolbox import __title__
+from agstoolbox.core.utils.math import clamp
+from agstoolbox.system.at_unique_application import unique_application
+
+
+class AtTrayIcon(QtWidgets.QSystemTrayIcon):
+
+    def __init__(self, icon, parent=None):
+        QtWidgets.QSystemTrayIcon.__init__(self, icon, parent)
+        self.window = MainWindow()
+        self.window.refresh_all()
+        menu = QtWidgets.QMenu(parent)
+
+        self.activated.connect(self.onTrayIconActivated)
+
+        action_open_toolbox = QtGui.QAction('Open Toolbox', self)
+        action_open_toolbox.triggered.connect(self.open_toolbox)  # load main panel
+
+        action_quit_toolbox = QtGui.QAction('Quit Toolbox', self)
+        action_quit_toolbox.triggered.connect(self.exit)
+
+        menu.addAction(action_open_toolbox)
+        menu.addAction(action_quit_toolbox)
+        self.setContextMenu(menu)
+
+        self.disambiguateTimer = QTimer(self)
+        self.disambiguateTimer.setSingleShot(True)
+        self.disambiguateTimer.timeout.connect(self.disambiguateTimerTimeout)
+
+    def exit(self):
+        QtCore.QCoreApplication.exit()
+
+    def open_toolbox(self):
+        tray_icon_rect = self.geometry()
+        window_pos = QtCore.QRect()
+        window_pos.setSize(QtCore.QSize(
+            ConstSettings().DEFAULT_MAIN_PANEL_WIDTH,
+            ConstSettings().DEFAULT_MAIN_PANEL_HEIGHT
+        ))
+
+        available_geometry = QtGui.QGuiApplication.primaryScreen().availableGeometry()
+
+        pos_x = clamp(tray_icon_rect.x(),
+                      available_geometry.x() + 48,
+                      available_geometry.width() - available_geometry.x() -
+                      window_pos.width() - 48)
+        pos_y = clamp(tray_icon_rect.y(),
+                      available_geometry.y() + 48,
+                      available_geometry.height() - available_geometry.y() -
+                      window_pos.height() - 48)
+
+        window_pos.setX(pos_x)
+        window_pos.setY(pos_y)
+        self.window.setGeometry(window_pos)
+        self.window.setWindowState(
+            self.window.windowState() &
+            ~QtCore.Qt.WindowState.WindowMinimized | QtCore.Qt.WindowState.WindowActive)
+        self.window.raise_()
+        self.window.show()
+        self.window.activateWindow()
+
+    def single_clicked(self):
+        self.open_toolbox()
+
+    def double_clicked(self):
+        self.open_toolbox()
+
+    def onTrayIconActivated(self, reason):
+        if reason == QSystemTrayIcon.ActivationReason.Trigger:
+            self.disambiguateTimer.start(ConstSettings().double_click_interval)
+        elif reason == QSystemTrayIcon.ActivationReason.DoubleClick:
+            self.disambiguateTimer.stop()
+            self.double_clicked()
+
+    def disambiguateTimerTimeout(self):
+        self.single_clicked()
+
+
+class UniqueWidget(QtWidgets.QWidget):
+    def __init__(self):
+        super().__init__()
+        QtWidgets.QApplication.instance().another_instance.connect(self.another_instance)
+
+    def another_instance(self):
+        self.findChild(AtTrayIcon, __title__).open_toolbox()
+
+
+def run_tray_indicator(ap_args):
+    app = unique_application(__title__, ap_args)
+    if not app.is_unique:
+        app.exit()
+        exit(1)
+
+    # this prevents the tray to close if the main panel is closed,
+    # we only exit when quit is explicitly clicked
+    app.setQuitOnLastWindowClosed(False)
+    ConstSettings().double_click_interval = app.doubleClickInterval()
+
+    w = UniqueWidget()
+    set_custom_fonts(app, w)
+    tray_icon = AtTrayIcon(main_icon(), w)
+    tray_icon.setObjectName(__title__)
+    tray_icon.show()
+    exit(app.exec())
```

### Comparing `agstoolbox-0.3.9/src/agstoolbox/core/ags/ags_editor_validation_data.py` & `agstoolbox-0.4.0/src/agstoolbox/core/ags/ags_editor_validation_data.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.9/src/agstoolbox/core/ags/ags_local_run.py` & `agstoolbox-0.4.0/src/agstoolbox/core/ags/ags_local_run.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 
 from agstoolbox.core.ags.ags_editor import LocalAgsEditor
 from agstoolbox.core.ags.game_project import GameProject
 from agstoolbox.core.utils.file import get_absolute_path
 from agstoolbox.core.utils.run import run_exe_params
 
 
-def start_ags_editor(editor: LocalAgsEditor):
-    run_exe_params(editor.path)
+def start_ags_editor(editor: LocalAgsEditor, block: bool = False):
+    run_exe_params(editor.path, block)
 
 
-def ags_editor_load_project(editor: LocalAgsEditor, project: GameProject):
+def ags_editor_load_project(editor: LocalAgsEditor, project: GameProject, block: bool = False):
     project_path = get_absolute_path(project.path)
-    run_exe_params(editor.path, [project_path])
+    run_exe_params(editor.path, block, [project_path], )
 
 
-def ags_editor_build_project(editor: LocalAgsEditor, project: GameProject):
+def ags_editor_build_project(editor: LocalAgsEditor, project: GameProject, block: bool = False):
     project_path = get_absolute_path(project.path)
-    run_exe_params(editor.path, ['/compile', project_path])
+    run_exe_params(editor.path, block, ['/compile', project_path])
```

### Comparing `agstoolbox-0.3.9/src/agstoolbox/core/ags/get_game_projects.py` & `agstoolbox-0.4.0/src/agstoolbox/core/ags/get_game_projects.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,119 +1,124 @@
-from __future__ import annotations  # for python 3.8
-import os.path
-from operator import attrgetter
-
-import defusedxml.ElementTree as ETree
-
-from agstoolbox.core.ags.game_project import GameProject, PROJECT_FILE_NAME
-from agstoolbox.core.utils.file import get_dir, get_file_if_exists, get_gp_candidates_in_dir
-from agstoolbox.core.version.version_utils import version_str_to_version
-
-AGS_EDITOR_ROOT_TAG = 'AGSEditorDocument'
-
-
-def text_file_starts_with_xml_Windows1252(filepath: str) -> bool:
-    platform = ''
-    try:
-        with open(filepath, mode='r', encoding='cp1252') as file:
-            platform = file.read(5)
-    except FileNotFoundError:
-        return False
-    except OSError:
-        return False
-    finally:
-        return platform == '<?xml'
-
-
-def is_game_file(filepath: str) -> bool:
-    if not os.path.exists(filepath):
-        return False
-
-    if not filepath.endswith(PROJECT_FILE_NAME):
-        return False
-
-    # it's too big, may crash parser later, better ignore for now
-    if os.path.getsize(filepath) > 268435456:
-        return False
-
-    if not text_file_starts_with_xml_Windows1252(filepath):
-        return False
-
-    tree = ETree.parse(filepath)
-    root = tree.getroot()
-    if not root.tag == AGS_EDITOR_ROOT_TAG:
-        return False
-
-    if 'EditorVersion' not in root.attrib:
-        return False
-
-    return True
-
-
-def gameagf_file_to_game_project(filepath: str) -> GameProject:
-    gp = GameProject()
-    tree = ETree.parse(filepath)
-    root = tree.getroot()
-    gp.path = filepath
-    gp.directory = get_dir(filepath)
-    ico_path = get_file_if_exists(gp.directory, "USER.ICO")
-    if not ico_path:
-        ico_path = get_file_if_exists(gp.directory, "template.ico")
-
-    gp.ico_path = ico_path
-    gp.last_modified = os.path.getmtime(filepath)
-
-    gp.name = root.find('Game/Settings/GameName').text
-    gp.ags_editor_version = version_str_to_version(root.attrib['EditorVersion'])
-    gp.ags_editor_version_index = root.attrib['VersionIndex']
-    return gp
-
-
-def valid_gameagf_file_to_game_project(filepath: str) -> GameProject | None:
-    if is_game_file(filepath):
-        return gameagf_file_to_game_project(filepath)
-    else:
-        return None
-
-
-def list_game_projects_in_dir(filepath: str) -> list[GameProject]:
-    candidates = get_gp_candidates_in_dir(filepath, PROJECT_FILE_NAME)
-    ags_projects = []
-
-    for candidate in candidates:
-        if not is_game_file(candidate):
-            continue
-
-        ags_projects.append(gameagf_file_to_game_project(candidate))
-
-    unique = list(dict.fromkeys(ags_projects))
-    ags_projects = unique
-    ags_projects.sort(key=attrgetter("last_modified"), reverse=True)
-
-    return ags_projects
-
-
-def list_game_projects_in_dir_list(filepaths: list[str]) -> list[GameProject]:
-    ags_projects = []
-    for path in filepaths:
-        candidates = list_game_projects_in_dir(path)
-        ags_projects.extend(candidates)
-
-    unique = list(dict.fromkeys(ags_projects))
-    ags_projects = unique
-    ags_projects.sort(key=attrgetter("last_modified"), reverse=True)
-
-    return ags_projects
-
-
-def get_unique_game_project_in_path(project_path: str) -> GameProject | None:
-    game_project: GameProject | None = valid_gameagf_file_to_game_project(project_path)
-
-    if game_project is None:
-        projects: list[GameProject] = list_game_projects_in_dir(project_path)
-        if len(projects) != 1:
-            print('WARN: Invalid project path, not exactly 1 game project found!')
-            return None
-
-        game_project = projects[0]
-
-    return game_project
+from __future__ import annotations  # for python 3.8
+import os.path
+from operator import attrgetter
+
+import defusedxml.ElementTree as ETree
+
+from agstoolbox.core.ags.game_project import GameProject, PROJECT_FILE_NAME
+from agstoolbox.core.utils.file import get_dir, get_file_if_exists, get_gp_candidates_in_dir
+from agstoolbox.core.version.version_utils import version_str_to_version
+
+AGS_EDITOR_ROOT_TAG = 'AGSEditorDocument'
+
+
+def text_file_starts_with_xml_Windows1252(filepath: str) -> bool:
+    platform = ''
+    try:
+        with open(filepath, mode='r', encoding='cp1252') as file:
+            platform = file.read(5)
+    except FileNotFoundError:
+        return False
+    except OSError:
+        return False
+    finally:
+        return platform == '<?xml'
+
+
+def is_game_file(filepath: str) -> bool:
+    if not os.path.exists(filepath):
+        return False
+
+    if not filepath.endswith(PROJECT_FILE_NAME):
+        return False
+
+    # it's too big, may crash parser later, better ignore for now
+    if os.path.getsize(filepath) > 268435456:
+        return False
+
+    if not text_file_starts_with_xml_Windows1252(filepath):
+        return False
+
+    tree = ETree.parse(filepath)
+    root = tree.getroot()
+    if not root.tag == AGS_EDITOR_ROOT_TAG:
+        return False
+
+    if 'EditorVersion' not in root.attrib:
+        return False
+
+    return True
+
+
+def gameagf_file_to_game_project(filepath: str) -> GameProject:
+    gp = GameProject()
+    tree = ETree.parse(filepath)
+    root = tree.getroot()
+    gp.path = filepath
+    gp.directory = get_dir(filepath)
+    ico_path = get_file_if_exists(gp.directory, "USER.ICO")
+    if not ico_path:
+        ico_path = get_file_if_exists(gp.directory, "template.ico")
+
+    gp.ico_path = ico_path
+    gp.last_modified = os.path.getmtime(filepath)
+
+    gp.name = root.find('Game/Settings/GameName').text
+    game_file_name_htag = root.find('Game/Settings/GameFileName')
+    if game_file_name_htag is not None:
+        gp.game_file = game_file_name_htag.text
+    else:
+        gp.game_file = ""
+    gp.ags_editor_version = version_str_to_version(root.attrib['EditorVersion'])
+    gp.ags_editor_version_index = root.attrib['VersionIndex']
+    return gp
+
+
+def valid_gameagf_file_to_game_project(filepath: str) -> GameProject | None:
+    if is_game_file(filepath):
+        return gameagf_file_to_game_project(filepath)
+    else:
+        return None
+
+
+def list_game_projects_in_dir(filepath: str) -> list[GameProject]:
+    candidates = get_gp_candidates_in_dir(filepath, PROJECT_FILE_NAME)
+    ags_projects = []
+
+    for candidate in candidates:
+        if not is_game_file(candidate):
+            continue
+
+        ags_projects.append(gameagf_file_to_game_project(candidate))
+
+    unique = list(dict.fromkeys(ags_projects))
+    ags_projects = unique
+    ags_projects.sort(key=attrgetter("last_modified"), reverse=True)
+
+    return ags_projects
+
+
+def list_game_projects_in_dir_list(filepaths: list[str]) -> list[GameProject]:
+    ags_projects = []
+    for path in filepaths:
+        candidates = list_game_projects_in_dir(path)
+        ags_projects.extend(candidates)
+
+    unique = list(dict.fromkeys(ags_projects))
+    ags_projects = unique
+    ags_projects.sort(key=attrgetter("last_modified"), reverse=True)
+
+    return ags_projects
+
+
+def get_unique_game_project_in_path(project_path: str) -> GameProject | None:
+    game_project: GameProject | None = valid_gameagf_file_to_game_project(project_path)
+
+    if game_project is None:
+        projects: list[GameProject] = list_game_projects_in_dir(project_path)
+        if len(projects) != 1:
+            print('WARN: Invalid project path, not exactly 1 game project found!')
+            return None
+
+        game_project = projects[0]
+
+    return game_project
```

### Comparing `agstoolbox-0.3.9/src/agstoolbox/core/ags/get_local_ags_editors.py` & `agstoolbox-0.4.0/src/agstoolbox/core/ags/get_local_ags_editors.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.9/src/agstoolbox/core/ags/validate_ags_editor.py` & `agstoolbox-0.4.0/src/agstoolbox/core/ags/validate_ags_editor.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.9/src/agstoolbox/core/cmdline/cmdline.py` & `agstoolbox-0.4.0/src/agstoolbox/core/cmdline/cmdline.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,17 @@
 from agstoolbox.core.gh.release import Release
 from agstoolbox.core.settings.settings import Settings
 from agstoolbox.core.version.version import Version
 from agstoolbox.core.version.version_utils import version_str_to_version
 
 
 def meta_cmd_project(args,
-                     ags_editor_proj_command: Callable[[LocalAgsEditor, GameProject], None] = None):
+                     ags_editor_proj_command: Callable[
+                         [LocalAgsEditor, GameProject, bool], None] = None):
+    block: bool = not args.non_blocking
     prj_path: str = args.PROJECT_PATH
 
     if not Path(prj_path).exists():
         print('ERROR: Invalid project path')
         return
 
     game_project: GameProject | None = get_unique_game_project_in_path(prj_path)
@@ -43,23 +45,23 @@
     project_version: Version = game_project.ags_editor_version
 
     managed_dir: str = Settings().get_tools_install_dir()
     editors = list_probable_ags_editors_in_dir(managed_dir)
 
     for editor in editors:
         if editor.version.as_int == project_version.as_int:
-            ags_editor_proj_command(editor, game_project)
+            ags_editor_proj_command(editor, game_project, block)
             return
 
     unmanaged_dirs: list[str] = Settings().get_manually_installed_editors_search_dirs()
     editors = list_ags_editors_in_dir_list(unmanaged_dirs)
 
     for editor in editors:
         if editor.version.as_int == project_version.as_int:
-            ags_editor_proj_command(editor, game_project)
+            ags_editor_proj_command(editor, game_project, block)
             return
 
     print("ERROR: Failed to find exact match of AGS Editor, wanted " + project_version.as_str)
 
 
 def at_cmd_list_projects(args):
     a_path: str | None = args.path
@@ -116,14 +118,15 @@
     elif is_editor_list:
         at_cmd_list_editors(args)
     else:
         print('ERROR: Invalid list command!')
 
 
 def at_cmd_install(args):
+    quiet: bool = True and args.quiet
     force: bool = True and args.force
     install_arg: str = args.VERSION_OR_PROJECT_PATH
 
     if install_arg is None or install_arg == "":
         print('ERROR: Editor Version specified is invalid!')
         return
 
@@ -152,15 +155,15 @@
 
     if is_install_dir_busy(release_to_install) and not force:
         print('ERROR: Editor Version already installed!')
         return
 
     print("Will install managed AGS Editor release " + release_to_install.version.as_str)
 
-    cmdline_download_release_to_cache(release_to_install)
+    cmdline_download_release_to_cache(release_to_install, quiet)
 
     print("Extracting...")
     install_release_from_cache(release_to_install)
     print("Installed release " + release_to_install.version.as_str)
     pass
 
 
@@ -302,31 +305,37 @@
     p_i.set_defaults(func=at_cmd_install)
     p_ii = p_i.add_subparsers(title='sub_install', dest='sub_install')
     p_iie = p_ii.add_parser('editor', help='install managed AGS Editor')
     p_iie.add_argument('VERSION_OR_PROJECT_PATH',
                        help='version to install or project to grab editor version')
     p_iie.add_argument('-f', '--force', action='store_true', default=None,
                        help='forces installation, overwrite if already exists')
+    p_iie.add_argument('-q', '--quiet', action='store_true', default=False,
+                       help='do not print download progress')
 
     # open command
     p_o = subparsers.add_parser('open', help='open an editor or project')
     p_o.set_defaults(func=at_cmd_open)
     p_oo = p_o.add_subparsers(title='sub_open', dest='sub_open')
     p_ooe = p_oo.add_parser('editor', help='open AGS Editor, by default only managed editors')
     p_ooe.add_argument('EDITOR_VERSION',
                        help='Editor version to open')
     p_oop = p_oo.add_parser('project', help='open AGS Project')
     p_oop.add_argument('PROJECT_PATH',
                        help='path to the project to be opened').complete = shtab.FILE
+    p_oop.add_argument('-n', '--non-blocking', action='store_true', default=False,
+                       help='do not wait for Editor to be closed to continue')
 
     # build command
     p_b = subparsers.add_parser('build', help='build an ags project')
     p_b.set_defaults(func=at_cmd_build)
     p_b.add_argument('PROJECT_PATH',
                      help='path to the project to be built').complete = shtab.FILE
+    p_b.add_argument('-n', '--non-blocking', action='store_true', default=False,
+                     help='do not wait for Editor to be closed to continue')
 
     # settings command
     p_s = subparsers.add_parser('settings', help='modify or show settings')
     p_s.set_defaults(func=at_cmd_settings)
     p_ss = p_s.add_subparsers(title='sub_settings', dest='sub_settings')
 
     p_ssh = p_ss.add_parser('show', help='show settings values')
```

### Comparing `agstoolbox-0.3.9/src/agstoolbox/core/cmdline/cmdline_download.py` & `agstoolbox-0.4.0/src/agstoolbox/core/cmdline/cmdline_download.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 from __future__ import annotations  # for python 3.8
 
 from agstoolbox.core.cmdline.progress import ProgressBar
 from agstoolbox.core.gh.download_release import download_release_to_cache
 from agstoolbox.core.gh.release import Release
 
 
-def cmdline_download_release_to_cache(release: Release):
+def cmdline_download_release_to_cache(release: Release, quiet: bool):
     max_size: int = release.archive_size
-    bar = ProgressBar(' Downloading... ', ' ' + release.archive_name + ' ', max_size, 'B')
+
+    bar = None
+    if not quiet:
+        bar = ProgressBar(' Downloading... ', ' ' + release.archive_name + ' ', max_size, 'B')
 
     def progress_updates(completed_percent: float,
                          c_size: int,
                          acc_c_size: int,
                          total_size_in_bytes: int):
-        bar.update(int(acc_c_size/8), total_size_in_bytes)
+        if bar is not None:
+            bar.update(int(acc_c_size/8), total_size_in_bytes)
 
     download_release_to_cache(release, progress_updates)
 
-    bar.finish()
+    if bar is not None:
+        bar.finish()
```

### Comparing `agstoolbox-0.3.9/src/agstoolbox/core/cmdline/progress.py` & `agstoolbox-0.4.0/src/agstoolbox/core/cmdline/progress.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.9/src/agstoolbox/core/gh/download_release.py` & `agstoolbox-0.4.0/src/agstoolbox/core/gh/download_release.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.9/src/agstoolbox/core/gh/install_release.py` & `agstoolbox-0.4.0/src/agstoolbox/core/gh/install_release.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.9/src/agstoolbox/core/gh/list_releases.py` & `agstoolbox-0.4.0/src/agstoolbox/core/gh/list_releases.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     releases = [None] * len(response_json)
     count = 0
 
     for rel in response_json:
         rls = None
         found_asset = False
 
+        # This can raise a TypeError in some weird condition I don't know what it is
         for asset in rel['assets']:
             # check for either predictable or patch release archives
             if is_asset_archive(rel['name'], asset['name']):
                 rls = Release()
                 rls.archive_id = str(asset['id'])
                 rls.archive_name = asset['name']
                 rls.archive_url = asset['browser_download_url']
```

### Comparing `agstoolbox-0.3.9/src/agstoolbox/core/settings/settings.py` & `agstoolbox-0.4.0/src/agstoolbox/core/settings/settings.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.9/src/agstoolbox/core/settings/settings_utils.py` & `agstoolbox-0.4.0/src/agstoolbox/core/settings/settings_utils.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.9/src/agstoolbox/core/utils/basics.py` & `agstoolbox-0.4.0/src/agstoolbox/core/utils/basics.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.9/src/agstoolbox/core/utils/downloader.py` & `agstoolbox-0.4.0/src/agstoolbox/core/utils/downloader.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.9/src/agstoolbox/core/utils/file.py` & `agstoolbox-0.4.0/src/agstoolbox/core/utils/file.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.9/src/agstoolbox/core/utils/pe.py` & `agstoolbox-0.4.0/src/agstoolbox/core/utils/pe.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.9/src/agstoolbox/core/utils/startup.py` & `agstoolbox-0.4.0/src/agstoolbox/core/utils/startup.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.9/src/agstoolbox/core/utils/systemdirs.py` & `agstoolbox-0.4.0/src/agstoolbox/core/utils/systemdirs.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.9/src/agstoolbox/core/utils/time.py` & `agstoolbox-0.4.0/src/agstoolbox/core/utils/time.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.9/src/agstoolbox/core/utils/win_registry.py` & `agstoolbox-0.4.0/src/agstoolbox/core/utils/win_registry.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.9/src/agstoolbox/core/version/version_utils.py` & `agstoolbox-0.4.0/src/agstoolbox/core/version/version_utils.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.9/src/agstoolbox/data/at_ags_editor_icon.png` & `agstoolbox-0.4.0/src/agstoolbox/data/at_ags_editor_icon.png`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.9/src/agstoolbox/data/at_ags_engine_icon.png` & `agstoolbox-0.4.0/src/agstoolbox/data/at_ags_engine_icon.png`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.9/src/agstoolbox/data/at_icon.png` & `agstoolbox-0.4.0/src/agstoolbox/data/at_icon.png`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.9/src/agstoolbox/data/at_icon_big.png` & `agstoolbox-0.4.0/src/agstoolbox/data/at_icon_big.png`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.9/src/agstoolbox/data/exit_icon.png` & `agstoolbox-0.4.0/src/agstoolbox/data/exit_icon.png`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.9/src/agstoolbox/data/refresh_icon.png` & `agstoolbox-0.4.0/src/agstoolbox/data/refresh_icon.png`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.9/src/agstoolbox/data/settings_icon.png` & `agstoolbox-0.4.0/src/agstoolbox/data/settings_icon.png`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.9/src/agstoolbox/getdata.py` & `agstoolbox-0.4.0/src/agstoolbox/getdata.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.9/src/agstoolbox/panels/at_settings_dialog.py` & `agstoolbox-0.4.0/src/agstoolbox/panels/at_settings_dialog.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.9/src/agstoolbox/system/at_unique_application.py` & `agstoolbox-0.4.0/src/agstoolbox/system/at_unique_application.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.9/src/agstoolbox/wdgts/at_dirlist_wdgt.py` & `agstoolbox-0.4.0/src/agstoolbox/wdgts/at_dirlist_wdgt.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.9/src/agstoolbox/wdgts/at_single_dir_wdgt.py` & `agstoolbox-0.4.0/src/agstoolbox/wdgts/at_single_dir_wdgt.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.9/src/agstoolbox/wdgts/at_tree_item_project.py` & `agstoolbox-0.4.0/src/agstoolbox/wdgts/at_tree_item_project.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.9/src/agstoolbox/wdgts/at_tree_item_tool.py` & `agstoolbox-0.4.0/src/agstoolbox/wdgts/at_tree_item_tool.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,248 +1,254 @@
-from __future__ import annotations  # for python 3.8
-from enum import Enum
-from PyQt6 import QtCore, QtGui, QtWidgets
-from PyQt6.QtWidgets import QTreeWidgetItem, QLabel, QHBoxLayout, QVBoxLayout, QGridLayout, QWidget
-
-from agstoolbox.at_icons import ags_editor_as_pixmap
-from agstoolbox.at_tasks import do_download_managed
-from agstoolbox.core.ags.ags_editor import LocalAgsEditor
-from agstoolbox.core.ags.ags_local_run import start_ags_editor
-from agstoolbox.core.utils.open_in_browser import open_in_browser
-from agstoolbox.wdgts_utils.ags_local_extra import ags_editor_folder_in_explorer
-from agstoolbox.core.gh.release import Release
-from agstoolbox.core.utils.time import s_ago
-from agstoolbox.wdgts_utils.action_utils import DefaultMenuQAction
-
-
-class ToolType(Enum):
-    MANAGED_TOOL = 1
-    AVAILABLE_TO_DOWNLOAD = 2
-    EXTERNALLY_INSTALLED_TOOL = 3
-
-
-class EditorImage(QLabel):
-    def __init__(self, parent: QWidget = None):
-        QLabel.__init__(self, parent)
-
-        pxmap = ags_editor_as_pixmap()
-
-        self.setPixmap(pxmap.scaled(
-            32, 32,
-            QtCore.Qt.AspectRatioMode.KeepAspectRatio,
-            QtCore.Qt.TransformationMode.SmoothTransformation))
-        self.setMaximumSize(32, 32)
-        self.setMinimumSize(32, 32)
-
-
-class TreeItemTool_Header(QTreeWidgetItem):
-    name = None
-    tool_type = None
-
-    def __init__(self, name: str, tool_type: ToolType):
-        QTreeWidgetItem.__init__(self)
-        self.name = name
-        self.setWhatsThis(0, name)
-        self.tool_type = tool_type
-        self.setText(0, name)
-
-    def __lt__(self, other):
-        return False  # keeps unaltered when sorting
-
-    def clear(self):
-        for i in range(self.childCount()):
-            self.removeChild(self.child(0))
-
-
-# Tool Download Item
-class TreeItemTool_Download_Widget(QWidget):
-    release = None
-    # we need to store the thread or the garbage collector will remove it!
-    thread_download = None
-
-    def __init__(self, release: Release, parent: QWidget = None):
-        QWidget.__init__(self, parent)
-        self.release = release
-
-        self.icon_img = EditorImage()
-        self.labelName = QLabel(self.release.name)
-        self.labelName.setWordWrap(True)
-
-        smaller_font = QtGui.QFont(
-            self.labelName.font().family(),
-            self.labelName.font().pointSize() * 0.90,
-        )
-
-        smallest_font = QtGui.QFont(
-            self.labelName.font().family(),
-            self.labelName.font().pointSize() * 0.75,
-        )
-
-        self.labelTime = QLabel(s_ago(self.release.published_at_timestamp))
-        self.labelTime.setFont(smaller_font)
-        self.labelTime.setAlignment(QtCore.Qt.AlignmentFlag.AlignRight)
-
-        self.labelDir = QLabel(self.release.url)
-        self.labelDir.setFont(smallest_font)
-        self.labelDir.setDisabled(True)
-
-        top_hbox = QHBoxLayout()
-        bottom_hbox = QHBoxLayout()
-
-        right_vbox = QVBoxLayout()
-
-        vbox = QVBoxLayout()
-
-        vbox.addLayout(top_hbox)
-        vbox.addLayout(bottom_hbox)
-        top_hbox.addWidget(self.labelName)
-        right_vbox.addWidget(self.labelTime)
-        top_hbox.addLayout(right_vbox)
-        bottom_hbox.addWidget(self.labelDir)
-
-        main_qgrid = QGridLayout()
-        main_qgrid.addWidget(self.icon_img)
-        main_qgrid.addLayout(vbox, 0, 1)
-
-        self.setLayout(main_qgrid)
-
-    def install(self):
-        if self.thread_download is not None:
-            return
-        self.thread_download = do_download_managed(self.release, self.download_ended)
-        self.setEnabled(False)
-
-    def show_gh_rel_page(self):
-        open_in_browser(self.release.html_url)
-
-    def mouseDoubleClickEvent(self, event):
-        self.install()
-
-    def download_ended(self):
-        self.thread_download = None
-        self.parent().parent().tools_schd_update_managed()
-        self.setEnabled(True)
-
-    def contextMenuEvent(self, event):
-        menu = QtWidgets.QMenu(self)
-        install_action = DefaultMenuQAction(menu, "Install as managed Editor")
-        show_gh_rel_page_action = menu.addAction("Show GitHub Release Page")
-        action = menu.exec(self.mapToGlobal(event.pos()))
-        if action == install_action:
-            self.install()
-        elif action == show_gh_rel_page_action:
-            self.show_gh_rel_page()
-
-
-# tool available locally for use
-# either managed or unmanaged (externally installed)
-class TreeItemTool_Local_Widget(QWidget):
-    ags_editor = None
-
-    def __init__(self, ags_editor: LocalAgsEditor, tool_type: ToolType, parent: QWidget = None):
-        QWidget.__init__(self, parent)
-        self.ags_editor = ags_editor
-
-        self.icon_img = EditorImage()
-        self.labelName = QLabel(self.ags_editor.name)
-        self.labelName.setWordWrap(True)
-
-        smaller_font = QtGui.QFont(
-            self.labelName.font().family(),
-            self.labelName.font().pointSize() * 0.90,
-        )
-
-        smallest_font = QtGui.QFont(
-            self.labelName.font().family(),
-            self.labelName.font().pointSize() * 0.75,
-        )
-
-        self.labelVersion = QLabel(self.ags_editor.version.as_str)
-        self.labelVersion.setFont(smaller_font)
-        self.labelVersion.setAlignment(QtCore.Qt.AlignmentFlag.AlignRight)
-
-        self.labelTime = QLabel(s_ago(self.ags_editor.last_modified))
-        self.labelTime.setFont(smaller_font)
-        self.labelTime.setAlignment(QtCore.Qt.AlignmentFlag.AlignRight)
-
-        self.labelDir = QLabel(self.ags_editor.path)
-        self.labelDir.setFont(smallest_font)
-        self.labelDir.setDisabled(True)
-
-        top_hbox = QHBoxLayout()
-        bottom_hbox = QHBoxLayout()
-
-        right_vbox = QVBoxLayout()
-
-        vbox = QVBoxLayout()
-
-        vbox.addLayout(top_hbox)
-        vbox.addLayout(bottom_hbox)
-        top_hbox.addWidget(self.labelName)
-        right_vbox.addWidget(self.labelTime)
-        right_vbox.addWidget(self.labelVersion)
-        top_hbox.addLayout(right_vbox)
-        bottom_hbox.addWidget(self.labelDir)
-
-        main_qgrid = QGridLayout()
-        main_qgrid.addWidget(self.icon_img)
-        main_qgrid.addLayout(vbox, 0, 1)
-
-        self.setLayout(main_qgrid)
-
-    def open_editor(self):
-        start_ags_editor(self.ags_editor)
-
-    def mouseDoubleClickEvent(self, event):
-        self.open_editor()
-
-    def contextMenuEvent(self, event):
-        menu = QtWidgets.QMenu(self)
-        open_editor_action = DefaultMenuQAction(menu, "Open Editor")
-        open_folder_action = menu.addAction("Open Folder in File Explorer")
-        action = menu.exec(self.mapToGlobal(event.pos()))
-        if action == open_editor_action:
-            self.open_editor()
-        elif action == open_folder_action:
-            ags_editor_folder_in_explorer(self.ags_editor)
-
-
-##################################################################################################
-# item widgets
-
-class TreeItemTool_Managed(QTreeWidgetItem):
-    tool_type = ToolType.MANAGED_TOOL
-
-    def __init__(self, parent: QTreeWidgetItem, ags_editor: LocalAgsEditor):
-        QTreeWidgetItem.__init__(self, parent)
-        self.itm_wdgt = TreeItemTool_Local_Widget(ags_editor, self.tool_type)
-
-    def __lt__(self, other):
-        return self.itm_wdgt.ags_editor.version.as_int < other.itm_wdgt.ags_editor.version.as_int
-
-    def updateInTree(self):
-        self.treeWidget().setItemWidget(self, 0, self.itm_wdgt)
-
-
-class TreeItemTool_ExternallyInstalled(QTreeWidgetItem):
-    tool_type = ToolType.EXTERNALLY_INSTALLED_TOOL
-
-    def __init__(self, parent: QTreeWidgetItem, ags_editor: LocalAgsEditor):
-        QTreeWidgetItem.__init__(self, parent)
-        self.itm_wdgt = TreeItemTool_Local_Widget(ags_editor, self.tool_type)
-
-    def __lt__(self, other):
-        return self.itm_wdgt.ags_editor.version.as_int < other.itm_wdgt.ags_editor.version.as_int
-
-    def updateInTree(self):
-        self.treeWidget().setItemWidget(self, 0, self.itm_wdgt)
-
-
-class TreeItemTool_Download(QTreeWidgetItem):
-    tool_type = ToolType.AVAILABLE_TO_DOWNLOAD
-
-    def __init__(self, parent: QTreeWidgetItem, release: Release):
-        QTreeWidgetItem.__init__(self, parent)
-        self.itm_wdgt = TreeItemTool_Download_Widget(release)
-
-    def updateInTree(self):
-        self.treeWidget().setItemWidget(self, 0, self.itm_wdgt)
+from __future__ import annotations  # for python 3.8
+from enum import Enum
+from PyQt6 import QtCore, QtGui, QtWidgets
+from PyQt6.QtWidgets import QTreeWidgetItem, QLabel, QHBoxLayout, QVBoxLayout, QGridLayout, QWidget
+
+from agstoolbox.at_icons import ags_editor_as_pixmap
+from agstoolbox.at_tasks import do_download_managed
+from agstoolbox.core.ags.ags_editor import LocalAgsEditor
+from agstoolbox.core.ags.ags_local_run import start_ags_editor
+from agstoolbox.core.utils.open_in_browser import open_in_browser
+from agstoolbox.wdgts_utils.ags_local_extra import ags_editor_folder_in_explorer
+from agstoolbox.core.gh.release import Release
+from agstoolbox.core.utils.time import s_ago
+from agstoolbox.wdgts_utils.action_utils import DefaultMenuQAction
+
+
+class ToolType(Enum):
+    HEADER = 16
+    MANAGED_TOOL = 1
+    AVAILABLE_TO_DOWNLOAD = 2
+    EXTERNALLY_INSTALLED_TOOL = 4
+
+    MANAGED_TOOL_HEADER = 17
+    AVAILABLE_TO_DOWNLOAD_HEADER = 18
+    EXTERNALLY_INSTALLED_TOOL_HEADER = 20
+
+
+class TreeItemTool(QTreeWidgetItem):
+    tool_type: ToolType = None
+
+    def __init__(self, parent: QTreeWidgetItem | None, tool_type: ToolType):
+        QTreeWidgetItem.__init__(self, parent)
+        self.tool_type = tool_type
+
+
+class EditorImage(QLabel):
+    def __init__(self, parent: QWidget = None):
+        QLabel.__init__(self, parent)
+
+        pxmap = ags_editor_as_pixmap()
+
+        self.setPixmap(pxmap.scaled(
+            32, 32,
+            QtCore.Qt.AspectRatioMode.KeepAspectRatio,
+            QtCore.Qt.TransformationMode.SmoothTransformation))
+        self.setMaximumSize(32, 32)
+        self.setMinimumSize(32, 32)
+
+
+class TreeItemTool_Header(TreeItemTool):
+    name = None
+
+    def __init__(self, name: str, tool_type: ToolType):
+        TreeItemTool.__init__(self, None, tool_type)
+        self.name = name
+        self.setWhatsThis(0, name)
+        self.tool_type = tool_type
+        self.setText(0, name)
+
+    def __lt__(self, other):
+        return False  # keeps unaltered when sorting
+
+    def clear(self):
+        for i in range(self.childCount()):
+            self.removeChild(self.child(0))
+
+
+# Tool Download Item
+class TreeItemTool_Download_Widget(QWidget):
+    release = None
+    # we need to store the thread or the garbage collector will remove it!
+    thread_download = None
+
+    def __init__(self, release: Release, parent: QWidget = None):
+        QWidget.__init__(self, parent)
+        self.release = release
+
+        self.icon_img = EditorImage()
+        self.labelName = QLabel(self.release.name)
+        self.labelName.setWordWrap(True)
+
+        smaller_font = QtGui.QFont(
+            self.labelName.font().family(),
+            self.labelName.font().pointSize() * 0.90,
+        )
+
+        smallest_font = QtGui.QFont(
+            self.labelName.font().family(),
+            self.labelName.font().pointSize() * 0.75,
+        )
+
+        self.labelTime = QLabel(s_ago(self.release.published_at_timestamp))
+        self.labelTime.setFont(smaller_font)
+        self.labelTime.setAlignment(QtCore.Qt.AlignmentFlag.AlignRight)
+
+        self.labelDir = QLabel(self.release.url)
+        self.labelDir.setFont(smallest_font)
+        self.labelDir.setDisabled(True)
+
+        top_hbox = QHBoxLayout()
+        bottom_hbox = QHBoxLayout()
+
+        right_vbox = QVBoxLayout()
+
+        vbox = QVBoxLayout()
+
+        vbox.addLayout(top_hbox)
+        vbox.addLayout(bottom_hbox)
+        top_hbox.addWidget(self.labelName)
+        right_vbox.addWidget(self.labelTime)
+        top_hbox.addLayout(right_vbox)
+        bottom_hbox.addWidget(self.labelDir)
+
+        main_qgrid = QGridLayout()
+        main_qgrid.addWidget(self.icon_img)
+        main_qgrid.addLayout(vbox, 0, 1)
+
+        self.setLayout(main_qgrid)
+
+    def install(self):
+        if self.thread_download is not None:
+            return
+        self.thread_download = do_download_managed(self.release, self.download_ended)
+        self.setEnabled(False)
+
+    def show_gh_rel_page(self):
+        open_in_browser(self.release.html_url)
+
+    def mouseDoubleClickEvent(self, event):
+        self.install()
+
+    def download_ended(self):
+        self.thread_download = None
+        self.parent().parent().tools_schd_update_managed()
+        self.setEnabled(True)
+
+    def contextMenuEvent(self, event):
+        menu = QtWidgets.QMenu(self)
+        install_action = DefaultMenuQAction(menu, "Install as managed Editor")
+        show_gh_rel_page_action = menu.addAction("Show GitHub Release Page")
+        action = menu.exec(self.mapToGlobal(event.pos()))
+        if action == install_action:
+            self.install()
+        elif action == show_gh_rel_page_action:
+            self.show_gh_rel_page()
+
+
+# tool available locally for use
+# either managed or unmanaged (externally installed)
+class TreeItemTool_Local_Widget(QWidget):
+    ags_editor = None
+
+    def __init__(self, ags_editor: LocalAgsEditor, tool_type: ToolType, parent: QWidget = None):
+        QWidget.__init__(self, parent)
+        self.ags_editor = ags_editor
+
+        self.icon_img = EditorImage()
+        self.labelName = QLabel(self.ags_editor.name)
+        self.labelName.setWordWrap(True)
+
+        smaller_font = QtGui.QFont(
+            self.labelName.font().family(),
+            self.labelName.font().pointSize() * 0.90,
+        )
+
+        smallest_font = QtGui.QFont(
+            self.labelName.font().family(),
+            self.labelName.font().pointSize() * 0.75,
+        )
+
+        self.labelVersion = QLabel(self.ags_editor.version.as_str)
+        self.labelVersion.setFont(smaller_font)
+        self.labelVersion.setAlignment(QtCore.Qt.AlignmentFlag.AlignRight)
+
+        self.labelTime = QLabel(s_ago(self.ags_editor.last_modified))
+        self.labelTime.setFont(smaller_font)
+        self.labelTime.setAlignment(QtCore.Qt.AlignmentFlag.AlignRight)
+
+        self.labelDir = QLabel(self.ags_editor.path)
+        self.labelDir.setFont(smallest_font)
+        self.labelDir.setDisabled(True)
+
+        top_hbox = QHBoxLayout()
+        bottom_hbox = QHBoxLayout()
+
+        right_vbox = QVBoxLayout()
+
+        vbox = QVBoxLayout()
+
+        vbox.addLayout(top_hbox)
+        vbox.addLayout(bottom_hbox)
+        top_hbox.addWidget(self.labelName)
+        right_vbox.addWidget(self.labelTime)
+        right_vbox.addWidget(self.labelVersion)
+        top_hbox.addLayout(right_vbox)
+        bottom_hbox.addWidget(self.labelDir)
+
+        main_qgrid = QGridLayout()
+        main_qgrid.addWidget(self.icon_img)
+        main_qgrid.addLayout(vbox, 0, 1)
+
+        self.setLayout(main_qgrid)
+
+    def open_editor(self):
+        start_ags_editor(self.ags_editor)
+
+    def mouseDoubleClickEvent(self, event):
+        self.open_editor()
+
+    def contextMenuEvent(self, event):
+        menu = QtWidgets.QMenu(self)
+        open_editor_action = DefaultMenuQAction(menu, "Open Editor")
+        open_folder_action = menu.addAction("Open Folder in File Explorer")
+        action = menu.exec(self.mapToGlobal(event.pos()))
+        if action == open_editor_action:
+            self.open_editor()
+        elif action == open_folder_action:
+            ags_editor_folder_in_explorer(self.ags_editor)
+
+
+##################################################################################################
+# item widgets
+
+class TreeItemTool_Managed(TreeItemTool):
+    def __init__(self, parent: QTreeWidgetItem, ags_editor: LocalAgsEditor):
+        TreeItemTool.__init__(self, parent, ToolType.MANAGED_TOOL)
+        self.itm_wdgt = TreeItemTool_Local_Widget(ags_editor, self.tool_type)
+
+    def __lt__(self, other):
+        return self.itm_wdgt.ags_editor.version.as_int < other.itm_wdgt.ags_editor.version.as_int
+
+    def updateInTree(self):
+        self.treeWidget().setItemWidget(self, 0, self.itm_wdgt)
+
+
+class TreeItemTool_ExternallyInstalled(TreeItemTool):
+    def __init__(self, parent: QTreeWidgetItem, ags_editor: LocalAgsEditor):
+        TreeItemTool.__init__(self, parent, ToolType.EXTERNALLY_INSTALLED_TOOL)
+        self.itm_wdgt = TreeItemTool_Local_Widget(ags_editor, self.tool_type)
+
+    def __lt__(self, other):
+        return self.itm_wdgt.ags_editor.version.as_int < other.itm_wdgt.ags_editor.version.as_int
+
+    def updateInTree(self):
+        self.treeWidget().setItemWidget(self, 0, self.itm_wdgt)
+
+
+class TreeItemTool_Download(TreeItemTool):
+    def __init__(self, parent: QTreeWidgetItem, release: Release):
+        TreeItemTool.__init__(self, parent, ToolType.AVAILABLE_TO_DOWNLOAD)
+        self.itm_wdgt = TreeItemTool_Download_Widget(release)
+
+    def updateInTree(self):
+        self.treeWidget().setItemWidget(self, 0, self.itm_wdgt)
```

### Comparing `agstoolbox-0.3.9/src/agstoolbox/wdgts_utils/file_explorer.py` & `agstoolbox-0.4.0/src/agstoolbox/wdgts_utils/file_explorer.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.9/src/agstoolbox.egg-info/PKG-INFO` & `agstoolbox-0.4.0/src/agstoolbox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: agstoolbox
-Version: 0.3.9
+Version: 0.4.0
 Summary: Utility to help manage Adventure Game Studio Projects and Editors.
 Home-page: https://github.com/ericoporto/agstoolbox
-Download-URL: https://github.com/ericoporto/agstoolbox/tarball/0.3.9
+Download-URL: https://github.com/ericoporto/agstoolbox/tarball/0.4.0
 Author: erico
 Author-email: eri0onpm@gmail.com
 License: MIT
 Keywords: AGS Toolbox,Adventure Game Studio,development,ags,Game Development,gamedev
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `agstoolbox-0.3.9/src/agstoolbox.egg-info/SOURCES.txt` & `agstoolbox-0.4.0/src/agstoolbox.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 README.rst
 agstoolbox
 atbx
 pyproject.toml
 setup.py
 src/agstoolbox/__init__.py
 src/agstoolbox/__main__.py
+src/agstoolbox/at_fonts.py
 src/agstoolbox/at_icons.py
 src/agstoolbox/at_tasks.py
 src/agstoolbox/at_trayindicator.py
 src/agstoolbox/getdata.py
 src/agstoolbox.egg-info/PKG-INFO
 src/agstoolbox.egg-info/SOURCES.txt
 src/agstoolbox.egg-info/dependency_links.txt
@@ -59,22 +60,24 @@
 src/agstoolbox/data/at_ags_editor_icon.png
 src/agstoolbox/data/at_ags_engine_icon.png
 src/agstoolbox/data/at_icon.png
 src/agstoolbox/data/at_icon_big.png
 src/agstoolbox/data/exit_icon.png
 src/agstoolbox/data/refresh_icon.png
 src/agstoolbox/data/settings_icon.png
+src/agstoolbox/data/fonts/Beedii.ttf
 src/agstoolbox/panels/__init__.py
 src/agstoolbox/panels/at_mainpanel.py
 src/agstoolbox/panels/at_settings_dialog.py
 src/agstoolbox/system/__init__.py
 src/agstoolbox/system/at_runguard.py
 src/agstoolbox/system/at_unique_application.py
 src/agstoolbox/wdgts/__init__.py
 src/agstoolbox/wdgts/at_dirlist_wdgt.py
+src/agstoolbox/wdgts/at_searchedit.py
 src/agstoolbox/wdgts/at_single_dir_wdgt.py
 src/agstoolbox/wdgts/at_tree_item_project.py
 src/agstoolbox/wdgts/at_tree_item_tool.py
 src/agstoolbox/wdgts/at_tree_projects_wdgt.py
 src/agstoolbox/wdgts/at_tree_tools_wdgt.py
 src/agstoolbox/wdgts_utils/__init__.py
 src/agstoolbox/wdgts_utils/action_utils.py
```

