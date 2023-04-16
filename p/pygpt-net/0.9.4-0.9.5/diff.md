# Comparing `tmp/pygpt-net-0.9.4.tar.gz` & `tmp/pygpt-net-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygpt-net-0.9.4.tar", last modified: Sat Apr 15 04:40:42 2023, max compression
+gzip compressed data, was "pygpt-net-0.9.5.tar", last modified: Sun Apr 16 07:59:22 2023, max compression
```

## Comparing `pygpt-net-0.9.4.tar` & `pygpt-net-0.9.5.tar`

### file list

```diff
@@ -1,110 +1,118 @@
-drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-15 04:40:42.444739 pygpt-net-0.9.4/
--rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1077 2023-04-10 01:01:37.000000 pygpt-net-0.9.4/LICENSE
--rw-rw-r--   0 marcin    (1000) marcin    (1000)    18300 2023-04-15 04:40:42.444739 pygpt-net-0.9.4/PKG-INFO
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)    16213 2023-04-15 03:36:32.000000 pygpt-net-0.9.4/README.md
--rw-rw-r--   0 marcin    (1000) marcin    (1000)     1146 2023-04-15 03:25:23.000000 pygpt-net-0.9.4/pyproject.toml
--rw-rw-r--   0 marcin    (1000) marcin    (1000)       38 2023-04-15 04:40:42.444739 pygpt-net-0.9.4/setup.cfg
--rw-rw-r--   0 marcin    (1000) marcin    (1000)     1470 2023-04-15 03:25:23.000000 pygpt-net-0.9.4/setup.py
-drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-15 04:40:42.436739 pygpt-net-0.9.4/src/
-drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-15 04:40:42.436739 pygpt-net-0.9.4/src/pygpt_net/
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)      290 2023-04-15 00:06:51.000000 pygpt-net-0.9.4/src/pygpt_net/CHANGELOG.txt
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)      844 2023-04-14 20:15:03.000000 pygpt-net-0.9.4/src/pygpt_net/__init__.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)      553 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/app.py
-drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-15 04:40:42.440739 pygpt-net-0.9.4/src/pygpt_net/core/
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)      488 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/__init__.py
--rw-rw-r--   0 marcin    (1000) marcin    (1000)     5068 2023-04-15 04:06:33.000000 pygpt-net-0.9.4/src/pygpt_net/core/app.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)    15069 2023-04-15 04:04:45.000000 pygpt-net-0.9.4/src/pygpt_net/core/config.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)    13637 2023-04-15 04:18:58.000000 pygpt-net-0.9.4/src/pygpt_net/core/context.py
-drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-15 04:40:42.440739 pygpt-net-0.9.4/src/pygpt_net/core/controller/
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)      488 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/controller/__init__.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     1662 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/controller/confirm.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     5161 2023-04-15 04:10:26.000000 pygpt-net-0.9.4/src/pygpt_net/core/controller/context.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     1516 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/controller/debug.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     4969 2023-04-15 01:05:50.000000 pygpt-net-0.9.4/src/pygpt_net/core/controller/image.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     1806 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/controller/info.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     5700 2023-04-15 03:25:23.000000 pygpt-net-0.9.4/src/pygpt_net/core/controller/input.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)    10570 2023-04-14 23:30:39.000000 pygpt-net-0.9.4/src/pygpt_net/core/controller/lang.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     1340 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/controller/launcher.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     2040 2023-04-15 04:09:34.000000 pygpt-net-0.9.4/src/pygpt_net/core/controller/main.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)    12782 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/controller/model.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     3558 2023-04-15 02:57:48.000000 pygpt-net-0.9.4/src/pygpt_net/core/controller/output.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)    13609 2023-04-15 03:25:23.000000 pygpt-net-0.9.4/src/pygpt_net/core/controller/plugins.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)    14522 2023-04-15 03:25:23.000000 pygpt-net-0.9.4/src/pygpt_net/core/controller/presets.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)    13247 2023-04-15 00:11:33.000000 pygpt-net-0.9.4/src/pygpt_net/core/controller/settings.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     9135 2023-04-14 22:32:15.000000 pygpt-net-0.9.4/src/pygpt_net/core/controller/theme.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     2601 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/controller/ui.py
-drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-15 04:40:42.440739 pygpt-net-0.9.4/src/pygpt_net/core/debug/
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)      488 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/debug/__init__.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)      988 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/debug/config.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     2110 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/debug/context.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     1554 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/debug/models.py
--rw-rw-r--   0 marcin    (1000) marcin    (1000)     1638 2023-04-15 04:02:02.000000 pygpt-net-0.9.4/src/pygpt_net/core/debug/plugins.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     1954 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/debug/presets.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     3800 2023-04-15 03:42:41.000000 pygpt-net-0.9.4/src/pygpt_net/core/debugger.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     8506 2023-04-15 03:04:36.000000 pygpt-net-0.9.4/src/pygpt_net/core/gpt.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     1737 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/history.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     2467 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/image.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)      832 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/info.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     1926 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/locale.py
-drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-15 04:40:42.440739 pygpt-net-0.9.4/src/pygpt_net/core/plugin/
--rw-rw-r--   0 marcin    (1000) marcin    (1000)      488 2023-04-15 00:11:33.000000 pygpt-net-0.9.4/src/pygpt_net/core/plugin/__init__.py
--rw-rw-r--   0 marcin    (1000) marcin    (1000)     2062 2023-04-15 03:25:23.000000 pygpt-net-0.9.4/src/pygpt_net/core/plugin/base_plugin.py
-drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-15 04:40:42.440739 pygpt-net-0.9.4/src/pygpt_net/core/plugin/real_time/
--rw-rw-r--   0 marcin    (1000) marcin    (1000)      488 2023-04-15 00:11:33.000000 pygpt-net-0.9.4/src/pygpt_net/core/plugin/real_time/__init__.py
--rw-rw-r--   0 marcin    (1000) marcin    (1000)     4205 2023-04-15 03:28:35.000000 pygpt-net-0.9.4/src/pygpt_net/core/plugin/real_time/plugin.py
-drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-15 04:40:42.440739 pygpt-net-0.9.4/src/pygpt_net/core/plugin/self_loop/
--rw-rw-r--   0 marcin    (1000) marcin    (1000)      488 2023-04-15 00:11:33.000000 pygpt-net-0.9.4/src/pygpt_net/core/plugin/self_loop/__init__.py
--rw-rw-r--   0 marcin    (1000) marcin    (1000)     4421 2023-04-15 03:28:35.000000 pygpt-net-0.9.4/src/pygpt_net/core/plugin/self_loop/plugin.py
--rw-rw-r--   0 marcin    (1000) marcin    (1000)     2775 2023-04-15 03:25:23.000000 pygpt-net-0.9.4/src/pygpt_net/core/plugins.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     2467 2023-04-15 00:16:54.000000 pygpt-net-0.9.4/src/pygpt_net/core/settings.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     4501 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/tokens.py
-drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-15 04:40:42.440739 pygpt-net-0.9.4/src/pygpt_net/core/ui/
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)      488 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/ui/__init__.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     3238 2023-04-14 23:23:11.000000 pygpt-net-0.9.4/src/pygpt_net/core/ui/chatbox.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     3324 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/ui/contexts.py
-drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-15 04:40:42.444739 pygpt-net-0.9.4/src/pygpt_net/core/ui/dialog/
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)      488 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/ui/dialog/__init__.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     3170 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/ui/dialog/about.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     1724 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/ui/dialog/changelog.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)      966 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/ui/dialog/ctx_rename.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     1518 2023-04-15 03:49:50.000000 pygpt-net-0.9.4/src/pygpt_net/core/ui/dialog/debug.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     2334 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/ui/dialog/editor.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     1817 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/ui/dialog/image.py
--rw-rw-r--   0 marcin    (1000) marcin    (1000)     6929 2023-04-14 23:06:24.000000 pygpt-net-0.9.4/src/pygpt_net/core/ui/dialog/plugins.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     6330 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/ui/dialog/preset.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     9119 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/ui/dialog/settings.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     2300 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/ui/dialog/start.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)      822 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/ui/dialog/update.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     4238 2023-04-14 22:11:32.000000 pygpt-net-0.9.4/src/pygpt_net/core/ui/dialogs.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     3904 2023-04-15 01:39:43.000000 pygpt-net-0.9.4/src/pygpt_net/core/ui/input.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     2186 2023-04-14 17:23:37.000000 pygpt-net-0.9.4/src/pygpt_net/core/ui/main.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     9065 2023-04-15 03:42:41.000000 pygpt-net-0.9.4/src/pygpt_net/core/ui/menu.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     1008 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/ui/status.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     8550 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/core/ui/toolbox.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)    24651 2023-04-15 01:39:43.000000 pygpt-net-0.9.4/src/pygpt_net/core/ui/widgets.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     6588 2023-04-15 04:07:29.000000 pygpt-net-0.9.4/src/pygpt_net/core/updater.py
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     1464 2023-04-15 04:03:17.000000 pygpt-net-0.9.4/src/pygpt_net/core/utils.py
-drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-15 04:40:42.444739 pygpt-net-0.9.4/src/pygpt_net/data/
-drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-15 04:40:42.444739 pygpt-net-0.9.4/src/pygpt_net/data/config/
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     1357 2023-04-15 04:24:04.000000 pygpt-net-0.9.4/src/pygpt_net/data/config/config.json
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)      669 2023-04-15 04:24:04.000000 pygpt-net-0.9.4/src/pygpt_net/data/config/models.json
-drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-15 04:40:42.444739 pygpt-net-0.9.4/src/pygpt_net/data/config/presets/
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)      255 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/data/config/presets/batman_and_joker.json
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)      287 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/data/config/presets/current.chat.json
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)      276 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/data/config/presets/current.completion.json
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)      259 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/data/config/presets/current.img.json
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)      273 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/data/config/presets/dalle_covboy_tokio.json
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)      525 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/data/config/presets/dalle_woman_photorealistic.json
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     3461 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/data/icon.ico
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)    13970 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/data/icon.png
-drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-15 04:40:42.444739 pygpt-net-0.9.4/src/pygpt_net/data/locale/
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     5548 2023-04-15 03:42:41.000000 pygpt-net-0.9.4/src/pygpt_net/data/locale/locale.en.ini
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     6082 2023-04-15 03:42:41.000000 pygpt-net-0.9.4/src/pygpt_net/data/locale/locale.pl.ini
--rwxrwxr-x   0 marcin    (1000) marcin    (1000)     9703 2023-04-14 00:10:28.000000 pygpt-net-0.9.4/src/pygpt_net/data/logo.png
-drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-15 04:40:42.436739 pygpt-net-0.9.4/src/pygpt_net.egg-info/
--rw-rw-r--   0 marcin    (1000) marcin    (1000)    18300 2023-04-15 04:40:42.000000 pygpt-net-0.9.4/src/pygpt_net.egg-info/PKG-INFO
--rw-rw-r--   0 marcin    (1000) marcin    (1000)     3312 2023-04-15 04:40:42.000000 pygpt-net-0.9.4/src/pygpt_net.egg-info/SOURCES.txt
--rw-rw-r--   0 marcin    (1000) marcin    (1000)        1 2023-04-15 04:40:42.000000 pygpt-net-0.9.4/src/pygpt_net.egg-info/dependency_links.txt
--rw-rw-r--   0 marcin    (1000) marcin    (1000)       49 2023-04-15 04:40:42.000000 pygpt-net-0.9.4/src/pygpt_net.egg-info/entry_points.txt
--rw-rw-r--   0 marcin    (1000) marcin    (1000)      138 2023-04-15 04:40:42.000000 pygpt-net-0.9.4/src/pygpt_net.egg-info/requires.txt
--rw-rw-r--   0 marcin    (1000) marcin    (1000)       10 2023-04-15 04:40:42.000000 pygpt-net-0.9.4/src/pygpt_net.egg-info/top_level.txt
+drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-16 07:59:22.873214 pygpt-net-0.9.5/
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1077 2023-04-10 01:01:37.000000 pygpt-net-0.9.5/LICENSE
+-rw-rw-r--   0 marcin    (1000) marcin    (1000)    19679 2023-04-16 07:59:22.873214 pygpt-net-0.9.5/PKG-INFO
+-rwxrwxr-x   0 marcin    (1000) marcin    (1000)    17594 2023-04-16 07:21:41.000000 pygpt-net-0.9.5/README.md
+-rw-rw-r--   0 marcin    (1000) marcin    (1000)     1220 2023-04-16 07:07:38.000000 pygpt-net-0.9.5/pyproject.toml
+-rw-rw-r--   0 marcin    (1000) marcin    (1000)       38 2023-04-16 07:59:22.873214 pygpt-net-0.9.5/setup.cfg
+-rw-rw-r--   0 marcin    (1000) marcin    (1000)     1555 2023-04-16 07:07:38.000000 pygpt-net-0.9.5/setup.py
+drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-16 07:59:22.865214 pygpt-net-0.9.5/src/
+drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-16 07:59:22.865214 pygpt-net-0.9.5/src/pygpt_net/
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)      485 2023-04-16 06:46:09.000000 pygpt-net-0.9.5/src/pygpt_net/CHANGELOG.txt
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)      844 2023-04-16 04:37:00.000000 pygpt-net-0.9.5/src/pygpt_net/__init__.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)      553 2023-04-14 00:10:28.000000 pygpt-net-0.9.5/src/pygpt_net/app.py
+drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-16 07:59:22.869214 pygpt-net-0.9.5/src/pygpt_net/core/
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)      488 2023-04-14 00:10:28.000000 pygpt-net-0.9.5/src/pygpt_net/core/__init__.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     5532 2023-04-16 07:38:43.000000 pygpt-net-0.9.5/src/pygpt_net/core/app.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)    15069 2023-04-15 04:41:36.000000 pygpt-net-0.9.5/src/pygpt_net/core/config.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)    13902 2023-04-16 03:53:33.000000 pygpt-net-0.9.5/src/pygpt_net/core/context.py
+drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-16 07:59:22.869214 pygpt-net-0.9.5/src/pygpt_net/core/controller/
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)      488 2023-04-14 00:10:28.000000 pygpt-net-0.9.5/src/pygpt_net/core/controller/__init__.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     2175 2023-04-16 06:32:03.000000 pygpt-net-0.9.5/src/pygpt_net/core/controller/audio.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1662 2023-04-14 00:10:28.000000 pygpt-net-0.9.5/src/pygpt_net/core/controller/confirm.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     5161 2023-04-15 04:10:26.000000 pygpt-net-0.9.5/src/pygpt_net/core/controller/context.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1516 2023-04-14 00:10:28.000000 pygpt-net-0.9.5/src/pygpt_net/core/controller/debug.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     4969 2023-04-15 04:41:36.000000 pygpt-net-0.9.5/src/pygpt_net/core/controller/image.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1806 2023-04-14 00:10:28.000000 pygpt-net-0.9.5/src/pygpt_net/core/controller/info.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     6083 2023-04-16 07:07:38.000000 pygpt-net-0.9.5/src/pygpt_net/core/controller/input.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)    10577 2023-04-16 06:32:03.000000 pygpt-net-0.9.5/src/pygpt_net/core/controller/lang.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1340 2023-04-14 00:10:28.000000 pygpt-net-0.9.5/src/pygpt_net/core/controller/launcher.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     2127 2023-04-16 04:34:56.000000 pygpt-net-0.9.5/src/pygpt_net/core/controller/main.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)    12782 2023-04-14 00:10:28.000000 pygpt-net-0.9.5/src/pygpt_net/core/controller/model.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     3558 2023-04-15 04:41:36.000000 pygpt-net-0.9.5/src/pygpt_net/core/controller/output.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)    14504 2023-04-16 06:32:03.000000 pygpt-net-0.9.5/src/pygpt_net/core/controller/plugins.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)    14522 2023-04-15 04:41:36.000000 pygpt-net-0.9.5/src/pygpt_net/core/controller/presets.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)    13247 2023-04-16 05:16:50.000000 pygpt-net-0.9.5/src/pygpt_net/core/controller/settings.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     9129 2023-04-16 00:10:05.000000 pygpt-net-0.9.5/src/pygpt_net/core/controller/theme.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     2601 2023-04-14 00:10:28.000000 pygpt-net-0.9.5/src/pygpt_net/core/controller/ui.py
+drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-16 07:59:22.869214 pygpt-net-0.9.5/src/pygpt_net/core/debug/
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)      488 2023-04-14 00:10:28.000000 pygpt-net-0.9.5/src/pygpt_net/core/debug/__init__.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)      988 2023-04-14 00:10:28.000000 pygpt-net-0.9.5/src/pygpt_net/core/debug/config.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     2110 2023-04-14 00:10:28.000000 pygpt-net-0.9.5/src/pygpt_net/core/debug/context.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1554 2023-04-14 00:10:28.000000 pygpt-net-0.9.5/src/pygpt_net/core/debug/models.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1638 2023-04-15 04:41:36.000000 pygpt-net-0.9.5/src/pygpt_net/core/debug/plugins.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1954 2023-04-14 00:10:28.000000 pygpt-net-0.9.5/src/pygpt_net/core/debug/presets.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     3800 2023-04-15 04:41:36.000000 pygpt-net-0.9.5/src/pygpt_net/core/debugger.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     9837 2023-04-16 07:31:27.000000 pygpt-net-0.9.5/src/pygpt_net/core/gpt.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1737 2023-04-14 00:10:28.000000 pygpt-net-0.9.5/src/pygpt_net/core/history.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     2467 2023-04-14 00:10:28.000000 pygpt-net-0.9.5/src/pygpt_net/core/image.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)      832 2023-04-14 00:10:28.000000 pygpt-net-0.9.5/src/pygpt_net/core/info.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1926 2023-04-14 00:10:28.000000 pygpt-net-0.9.5/src/pygpt_net/core/locale.py
+drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-16 07:59:22.869214 pygpt-net-0.9.5/src/pygpt_net/core/plugin/
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)      488 2023-04-15 04:41:36.000000 pygpt-net-0.9.5/src/pygpt_net/core/plugin/__init__.py
+drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-16 07:59:22.869214 pygpt-net-0.9.5/src/pygpt_net/core/plugin/audio_azure/
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)      488 2023-04-15 04:41:36.000000 pygpt-net-0.9.5/src/pygpt_net/core/plugin/audio_azure/__init__.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     6987 2023-04-16 07:12:53.000000 pygpt-net-0.9.5/src/pygpt_net/core/plugin/audio_azure/plugin.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     2062 2023-04-15 04:41:36.000000 pygpt-net-0.9.5/src/pygpt_net/core/plugin/base_plugin.py
+drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-16 07:59:22.869214 pygpt-net-0.9.5/src/pygpt_net/core/plugin/real_time/
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)      488 2023-04-15 04:41:36.000000 pygpt-net-0.9.5/src/pygpt_net/core/plugin/real_time/__init__.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     4205 2023-04-15 04:41:36.000000 pygpt-net-0.9.5/src/pygpt_net/core/plugin/real_time/plugin.py
+drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-16 07:59:22.869214 pygpt-net-0.9.5/src/pygpt_net/core/plugin/self_loop/
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)      488 2023-04-15 04:41:36.000000 pygpt-net-0.9.5/src/pygpt_net/core/plugin/self_loop/__init__.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     4421 2023-04-15 04:41:36.000000 pygpt-net-0.9.5/src/pygpt_net/core/plugin/self_loop/plugin.py
+drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-16 07:59:22.869214 pygpt-net-0.9.5/src/pygpt_net/core/plugin/web_search/
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)      488 2023-04-15 04:41:36.000000 pygpt-net-0.9.5/src/pygpt_net/core/plugin/web_search/__init__.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     9957 2023-04-16 07:11:07.000000 pygpt-net-0.9.5/src/pygpt_net/core/plugin/web_search/plugin.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     6495 2023-04-16 07:35:14.000000 pygpt-net-0.9.5/src/pygpt_net/core/plugin/web_search/websearch.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     2775 2023-04-15 04:41:36.000000 pygpt-net-0.9.5/src/pygpt_net/core/plugins.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     2467 2023-04-15 04:41:36.000000 pygpt-net-0.9.5/src/pygpt_net/core/settings.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     4501 2023-04-14 00:10:28.000000 pygpt-net-0.9.5/src/pygpt_net/core/tokens.py
+drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-16 07:59:22.873214 pygpt-net-0.9.5/src/pygpt_net/core/ui/
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)      488 2023-04-14 00:10:28.000000 pygpt-net-0.9.5/src/pygpt_net/core/ui/__init__.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     3238 2023-04-15 04:41:36.000000 pygpt-net-0.9.5/src/pygpt_net/core/ui/chatbox.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     3324 2023-04-14 00:10:28.000000 pygpt-net-0.9.5/src/pygpt_net/core/ui/contexts.py
+drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-16 07:59:22.873214 pygpt-net-0.9.5/src/pygpt_net/core/ui/dialog/
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)      488 2023-04-14 00:10:28.000000 pygpt-net-0.9.5/src/pygpt_net/core/ui/dialog/__init__.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     3170 2023-04-14 00:10:28.000000 pygpt-net-0.9.5/src/pygpt_net/core/ui/dialog/about.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1724 2023-04-14 00:10:28.000000 pygpt-net-0.9.5/src/pygpt_net/core/ui/dialog/changelog.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)      966 2023-04-14 00:10:28.000000 pygpt-net-0.9.5/src/pygpt_net/core/ui/dialog/ctx_rename.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1518 2023-04-15 04:41:36.000000 pygpt-net-0.9.5/src/pygpt_net/core/ui/dialog/debug.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     2334 2023-04-14 00:10:28.000000 pygpt-net-0.9.5/src/pygpt_net/core/ui/dialog/editor.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1817 2023-04-14 00:10:28.000000 pygpt-net-0.9.5/src/pygpt_net/core/ui/dialog/image.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     7289 2023-04-16 02:39:18.000000 pygpt-net-0.9.5/src/pygpt_net/core/ui/dialog/plugins.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     6330 2023-04-14 00:10:28.000000 pygpt-net-0.9.5/src/pygpt_net/core/ui/dialog/preset.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     9119 2023-04-16 05:16:33.000000 pygpt-net-0.9.5/src/pygpt_net/core/ui/dialog/settings.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     2300 2023-04-14 00:10:28.000000 pygpt-net-0.9.5/src/pygpt_net/core/ui/dialog/start.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)      822 2023-04-14 00:10:28.000000 pygpt-net-0.9.5/src/pygpt_net/core/ui/dialog/update.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     4238 2023-04-15 04:41:36.000000 pygpt-net-0.9.5/src/pygpt_net/core/ui/dialogs.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     3904 2023-04-15 04:41:36.000000 pygpt-net-0.9.5/src/pygpt_net/core/ui/input.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     2186 2023-04-15 04:41:36.000000 pygpt-net-0.9.5/src/pygpt_net/core/ui/main.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     9194 2023-04-16 05:22:28.000000 pygpt-net-0.9.5/src/pygpt_net/core/ui/menu.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1008 2023-04-14 00:10:28.000000 pygpt-net-0.9.5/src/pygpt_net/core/ui/status.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     8550 2023-04-14 00:10:28.000000 pygpt-net-0.9.5/src/pygpt_net/core/ui/toolbox.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)    24651 2023-04-15 04:41:36.000000 pygpt-net-0.9.5/src/pygpt_net/core/ui/widgets.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     6588 2023-04-16 05:17:33.000000 pygpt-net-0.9.5/src/pygpt_net/core/updater.py
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1464 2023-04-15 04:41:36.000000 pygpt-net-0.9.5/src/pygpt_net/core/utils.py
+drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-16 07:59:22.873214 pygpt-net-0.9.5/src/pygpt_net/data/
+drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-16 07:59:22.873214 pygpt-net-0.9.5/src/pygpt_net/data/config/
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     1357 2023-04-16 06:58:52.000000 pygpt-net-0.9.5/src/pygpt_net/data/config/config.json
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)      669 2023-04-16 07:07:38.000000 pygpt-net-0.9.5/src/pygpt_net/data/config/models.json
+drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-16 07:59:22.873214 pygpt-net-0.9.5/src/pygpt_net/data/config/presets/
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)      255 2023-04-14 00:10:28.000000 pygpt-net-0.9.5/src/pygpt_net/data/config/presets/batman_and_joker.json
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)      287 2023-04-14 00:10:28.000000 pygpt-net-0.9.5/src/pygpt_net/data/config/presets/current.chat.json
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)      276 2023-04-14 00:10:28.000000 pygpt-net-0.9.5/src/pygpt_net/data/config/presets/current.completion.json
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)      259 2023-04-14 00:10:28.000000 pygpt-net-0.9.5/src/pygpt_net/data/config/presets/current.img.json
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)      273 2023-04-14 00:10:28.000000 pygpt-net-0.9.5/src/pygpt_net/data/config/presets/dalle_covboy_tokio.json
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)      525 2023-04-14 00:10:28.000000 pygpt-net-0.9.5/src/pygpt_net/data/config/presets/dalle_woman_photorealistic.json
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     3461 2023-04-14 00:10:28.000000 pygpt-net-0.9.5/src/pygpt_net/data/icon.ico
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)    13970 2023-04-14 00:10:28.000000 pygpt-net-0.9.5/src/pygpt_net/data/icon.png
+drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-16 07:59:22.873214 pygpt-net-0.9.5/src/pygpt_net/data/locale/
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     5604 2023-04-16 07:07:38.000000 pygpt-net-0.9.5/src/pygpt_net/data/locale/locale.en.ini
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     6129 2023-04-16 07:07:38.000000 pygpt-net-0.9.5/src/pygpt_net/data/locale/locale.pl.ini
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     9703 2023-04-14 00:10:28.000000 pygpt-net-0.9.5/src/pygpt_net/data/logo.png
+drwxrwxr-x   0 marcin    (1000) marcin    (1000)        0 2023-04-16 07:59:22.865214 pygpt-net-0.9.5/src/pygpt_net.egg-info/
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)    19679 2023-04-16 07:59:22.000000 pygpt-net-0.9.5/src/pygpt_net.egg-info/PKG-INFO
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)     3595 2023-04-16 07:59:22.000000 pygpt-net-0.9.5/src/pygpt_net.egg-info/SOURCES.txt
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)        1 2023-04-16 07:59:22.000000 pygpt-net-0.9.5/src/pygpt_net.egg-info/dependency_links.txt
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)       49 2023-04-16 07:59:22.000000 pygpt-net-0.9.5/src/pygpt_net.egg-info/entry_points.txt
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)      192 2023-04-16 07:59:22.000000 pygpt-net-0.9.5/src/pygpt_net.egg-info/requires.txt
+-rwxrwxrwx   0 marcin    (1000) marcin    (1000)       10 2023-04-16 07:59:22.000000 pygpt-net-0.9.5/src/pygpt_net.egg-info/top_level.txt
```

### Comparing `pygpt-net-0.9.4/LICENSE` & `pygpt-net-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.4/PKG-INFO` & `pygpt-net-0.9.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pygpt-net
-Version: 0.9.4
-Summary: A GPT4, GPT3, ChatGPT and DALL-E 2 Desktop App with chatbot, text completion and image generation
+Version: 0.9.5
+Summary: GPT4, GPT3, ChatGPT and DALL-E 2 Desktop App with chatbot, text completion and image generation
 Home-page: https://github.com/szczyglis-dev/py-gpt
 Author: Marcin Szczygliński
 Author-email: Marcin Szczygliński <info@pygpt.net>
 Maintainer: Marcin Szczygliński
 Maintainer-email: info@pygpt.net
 License: MIT License
         
@@ -36,55 +36,58 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PYGPT
 
-Current release: **0.9.4** (build: **2023.04.15**) | Official website: https://pygpt.net | Docs: https://pygpt.readthedocs.io
+Current release: **0.9.5** (build: **2023.04.16**) | Official website: https://pygpt.net | Docs: https://pygpt.readthedocs.io
 
 PyPi: https://pypi.org/project/pygpt-net
 
-### **Compiled binary versions for Windows 10, 11 and Linux are available to download on project's page**: https://pygpt.net (in "Download" section)
+### **Compiled versions for Windows 10, 11 and Linux**: https://pygpt.net/#download
 
 ## What is PYGPT?
 
 **PYGPT** is a desktop application that allows you to talk to OpenAI\'s
-artificial intelligence models such as **GPT4** and **GPT3** using your
-own computer and `OpenAI API`. It allows you to talk in chat mode and in
-completion mode, as well as generate images using **DALL-E 2**.
-Moreover, the application has implemented context memory support,
+LLM models such as **GPT4** and **GPT3** using your own computer and `OpenAI API`. 
+It allows you to talk in chat mode and in completion mode, as well as generate images 
+using **DALL-E 2**. PYGPT also adds access to the Internet for GPT via Google Custom 
+Search API and Wikipedia API and includes voice synthesis using Microsoft Azure 
+Text-to-Speech API. Moreover, the application has implemented context memory support,
 context storage, history of contexts, which can be restored at any time
 and e.g. continue the conversation from point in history, and also has a
 convenient and intuitive system of presets that allows you to quickly
-and pleasantly create and manage your prompts.
+and pleasantly create and manage your prompts. Plugins support is also available.
 
 ![app1](https://user-images.githubusercontent.com/61396542/230803425-5035ccd8-50d9-4fef-9774-8843cf3ce5b0.jpg)
 
-You can download compiled application for Windows and Linux on: https://pygpt.net/#download
+You can download compiled version for Windows and Linux at: https://pygpt.net/#download
 
 ## Features
 
 - desktop application for `Windows` and `Linux`, written in Python
 - works similar to `ChatGPT`, but locally (on desktop)
 - 3 modes of operation: chatbot, text completion and image generation
 - supports multiple models: `GPT4` and `GPT3`
 - handles and stores full context of the conversation (short-term
   memory)
+- adds access to the Internet for GPT via Google Custom Search API and Wikipedia API
+- includes voice synthesis using Microsoft Azure Text-to-Speech API
 - stores the history of contexts with the ability to return to
   previous context (long-term memory)
 - allows you to easily manage prompts with handly editable presets
 - intuitive operation and interface
 - allows you to use all the powerful features of `GPT4` and `GPT3`
 - no knowledge of using AI models required
 - enables easy and convenient generation of images using `DALL-E 2`
 - has the ability to support future OpenAI models
 - fully configurable
 - plugins support
-- built-in tokens usage calculation
+- built-in token usage calculation
 - it\'s open source, source code is available on `GitHub`
 - **uses the user\'s API key**
 
 The application is free, open source and runs on PC with `Windows 10`,
 `Windows 11` and `Linux`. The full **Python** source code is available
 on `GitHub`.
 
@@ -338,15 +341,15 @@
 one go. To set the required number of variants that you want to be
 generated, use the slider located in the corner on the right at the
 bottom of the screen (appears in place of the slider with the
 conversation temperature when switching to the image generation mode).
 
 ![dalle](https://user-images.githubusercontent.com/61396542/230803477-8ca3b13b-080d-4acc-9f19-fc2f1762e8e4.jpg)
 
-## Images storage
+## Image storage
 
 The image generated in this way can then be easily saved anywhere on the
 disk (just right-click on it), deleted or displayed in full size in the
 browser.
 
 **Tip:** with presets, you can save prepared prompts and use them later
 when generating subsequent images.
@@ -356,20 +359,29 @@
 generate new content.
 
 ## Plugins
 
 The application allows you to use plugins to extend its functionality.
 Currently, the following plugins are available:
 
-- **SelfLoop** - allows to run GPT in a self-loop, which allows you to
+- **Self Loop** - allows to run GPT in a self-loop, which allows you to
   generate a continuous conversation between AI <> AI. In this mode model talks to itself.
 
-- **RealTime** - auto-append current date and time to the prompt. It tells
+- **Real Time** - auto-append current date and time to the prompt. It tells
   the model what time it is in real time.
 
+- **Web Search** - adds access to the Internet using Google Custom Search Engine and Wikipedia API
+
+- **Audio (Azure)** - adds voice synthesis using Microsoft Azure Text-to-Speech API
+
+## Audio / voice synthesis
+
+The application offers voice synthesis using the **Microsoft Azure Text-To-Speech** API.
+It required your own Microsoft Azure API Key. 
+You can get Api Key for free from [here](https://azure.microsoft.com/en-us/services/cognitive-services/text-to-speech/).
 
 # Tokens calculation
 
 ## Input tokens
 
 Calculation of tokens is implemented in the application. The application
 tries to predict the number of tokens that will be used for a given
@@ -506,24 +518,35 @@
 window.
 
 Simply download the new version and use it instead of the current one,
 all configuration such as context and history will survive between
 versions and will be available in the newly installed version.
 
 
-# Plugins and audio (coming soon)
-
 ## Next releases
 
-Support for plug-ins and voice recognition and synthesis will be added
-in future versions of the application.
+Support for voice recognition will be added in future versions of the application.
 
+## DISCLAIMER
+
+This application is not affiliated with OpenAI in any way.
+Author is not responsible for any damage caused by the use of this application.
+Application is provided as is, without any warranty.
+Please also remember about tokens usage - always check the number of tokens used by 
+the model on OpenAI website and use the application responsibly.
+Enabled plugins (like e.g. Web Search) may use additional tokens,
+not listed in main window. Always control your real token usage on OpenAI website.
 
 # CHANGELOG
 
+## v0.9.5 (2023.04.16)
+
+- added web plugin (adds access to the Internet using Google Custom Search Engine and Wikipedia API)
+- added voice output plugin (adds voice synthesis using Microsoft Azure)
+
 ## v0.9.4 (2023.04.15)
 
 - added plugins support
 
 ## v0.9.3 (2023.04.14)
 
 - packed into PyPI package
```

### Comparing `pygpt-net-0.9.4/README.md` & `pygpt-net-0.9.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,50 +1,53 @@
 # PYGPT
 
-Current release: **0.9.4** (build: **2023.04.15**) | Official website: https://pygpt.net | Docs: https://pygpt.readthedocs.io
+Current release: **0.9.5** (build: **2023.04.16**) | Official website: https://pygpt.net | Docs: https://pygpt.readthedocs.io
 
 PyPi: https://pypi.org/project/pygpt-net
 
-### **Compiled binary versions for Windows 10, 11 and Linux are available to download on project's page**: https://pygpt.net (in "Download" section)
+### **Compiled versions for Windows 10, 11 and Linux**: https://pygpt.net/#download
 
 ## What is PYGPT?
 
 **PYGPT** is a desktop application that allows you to talk to OpenAI\'s
-artificial intelligence models such as **GPT4** and **GPT3** using your
-own computer and `OpenAI API`. It allows you to talk in chat mode and in
-completion mode, as well as generate images using **DALL-E 2**.
-Moreover, the application has implemented context memory support,
+LLM models such as **GPT4** and **GPT3** using your own computer and `OpenAI API`. 
+It allows you to talk in chat mode and in completion mode, as well as generate images 
+using **DALL-E 2**. PYGPT also adds access to the Internet for GPT via Google Custom 
+Search API and Wikipedia API and includes voice synthesis using Microsoft Azure 
+Text-to-Speech API. Moreover, the application has implemented context memory support,
 context storage, history of contexts, which can be restored at any time
 and e.g. continue the conversation from point in history, and also has a
 convenient and intuitive system of presets that allows you to quickly
-and pleasantly create and manage your prompts.
+and pleasantly create and manage your prompts. Plugins support is also available.
 
 ![app1](https://user-images.githubusercontent.com/61396542/230803425-5035ccd8-50d9-4fef-9774-8843cf3ce5b0.jpg)
 
-You can download compiled application for Windows and Linux on: https://pygpt.net/#download
+You can download compiled version for Windows and Linux at: https://pygpt.net/#download
 
 ## Features
 
 - desktop application for `Windows` and `Linux`, written in Python
 - works similar to `ChatGPT`, but locally (on desktop)
 - 3 modes of operation: chatbot, text completion and image generation
 - supports multiple models: `GPT4` and `GPT3`
 - handles and stores full context of the conversation (short-term
   memory)
+- adds access to the Internet for GPT via Google Custom Search API and Wikipedia API
+- includes voice synthesis using Microsoft Azure Text-to-Speech API
 - stores the history of contexts with the ability to return to
   previous context (long-term memory)
 - allows you to easily manage prompts with handly editable presets
 - intuitive operation and interface
 - allows you to use all the powerful features of `GPT4` and `GPT3`
 - no knowledge of using AI models required
 - enables easy and convenient generation of images using `DALL-E 2`
 - has the ability to support future OpenAI models
 - fully configurable
 - plugins support
-- built-in tokens usage calculation
+- built-in token usage calculation
 - it\'s open source, source code is available on `GitHub`
 - **uses the user\'s API key**
 
 The application is free, open source and runs on PC with `Windows 10`,
 `Windows 11` and `Linux`. The full **Python** source code is available
 on `GitHub`.
 
@@ -298,15 +301,15 @@
 one go. To set the required number of variants that you want to be
 generated, use the slider located in the corner on the right at the
 bottom of the screen (appears in place of the slider with the
 conversation temperature when switching to the image generation mode).
 
 ![dalle](https://user-images.githubusercontent.com/61396542/230803477-8ca3b13b-080d-4acc-9f19-fc2f1762e8e4.jpg)
 
-## Images storage
+## Image storage
 
 The image generated in this way can then be easily saved anywhere on the
 disk (just right-click on it), deleted or displayed in full size in the
 browser.
 
 **Tip:** with presets, you can save prepared prompts and use them later
 when generating subsequent images.
@@ -316,20 +319,29 @@
 generate new content.
 
 ## Plugins
 
 The application allows you to use plugins to extend its functionality.
 Currently, the following plugins are available:
 
-- **SelfLoop** - allows to run GPT in a self-loop, which allows you to
+- **Self Loop** - allows to run GPT in a self-loop, which allows you to
   generate a continuous conversation between AI <> AI. In this mode model talks to itself.
 
-- **RealTime** - auto-append current date and time to the prompt. It tells
+- **Real Time** - auto-append current date and time to the prompt. It tells
   the model what time it is in real time.
 
+- **Web Search** - adds access to the Internet using Google Custom Search Engine and Wikipedia API
+
+- **Audio (Azure)** - adds voice synthesis using Microsoft Azure Text-to-Speech API
+
+## Audio / voice synthesis
+
+The application offers voice synthesis using the **Microsoft Azure Text-To-Speech** API.
+It required your own Microsoft Azure API Key. 
+You can get Api Key for free from [here](https://azure.microsoft.com/en-us/services/cognitive-services/text-to-speech/).
 
 # Tokens calculation
 
 ## Input tokens
 
 Calculation of tokens is implemented in the application. The application
 tries to predict the number of tokens that will be used for a given
@@ -466,24 +478,35 @@
 window.
 
 Simply download the new version and use it instead of the current one,
 all configuration such as context and history will survive between
 versions and will be available in the newly installed version.
 
 
-# Plugins and audio (coming soon)
-
 ## Next releases
 
-Support for plug-ins and voice recognition and synthesis will be added
-in future versions of the application.
+Support for voice recognition will be added in future versions of the application.
 
+## DISCLAIMER
+
+This application is not affiliated with OpenAI in any way.
+Author is not responsible for any damage caused by the use of this application.
+Application is provided as is, without any warranty.
+Please also remember about tokens usage - always check the number of tokens used by 
+the model on OpenAI website and use the application responsibly.
+Enabled plugins (like e.g. Web Search) may use additional tokens,
+not listed in main window. Always control your real token usage on OpenAI website.
 
 # CHANGELOG
 
+## v0.9.5 (2023.04.16)
+
+- added web plugin (adds access to the Internet using Google Custom Search Engine and Wikipedia API)
+- added voice output plugin (adds voice synthesis using Microsoft Azure)
+
 ## v0.9.4 (2023.04.15)
 
 - added plugins support
 
 ## v0.9.3 (2023.04.14)
 
 - packed into PyPI package
```

### Comparing `pygpt-net-0.9.4/pyproject.toml` & `pygpt-net-0.9.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pygpt-net"
-version = "0.9.4"
-description = "A GPT4, GPT3, ChatGPT and DALL-E 2 Desktop App with chatbot, text completion and image generation"
+version = "0.9.5"
+description = "GPT4, GPT3, ChatGPT and DALL-E 2 Desktop App with chatbot, text completion and image generation"
 readme = "README.md"
 authors = [{ name = "Marcin Szczygliński", email = "info@pygpt.net" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["py_gpt", "py-gpt", "pygpt", "desktop", "app", "gpt", "gpt4", "gpt3", "chatgpt", "dall-e", "chat",
     "chatbot", "text completion", "image generation", "ai", "api", "openai", "api key", "context memory", "history",
     "presets", "ui", "qt", "pyside"]
 dependencies = [
+    'beautifulsoup4>=4.12.2',
     'openai>=0.27.4',
     'packaging>=23.0',
+    'pydub>=0.25.1',
     'pyinstaller>=5.9.0',
     'PySide6-Essentials>=6.4.2',
     'qt-material>=2.14',
     'show-in-file-manager>=1.1.4',
     'tiktoken>=0.3.3',
+    'wikipedia>=1.4.0',
 ]
 requires-python = ">=3.9"
 
 [project.urls]
 Homepage = "https://github.com/szczyglis-dev/py-gpt"
 
 [project.scripts]
-pygpt = "pygpt_net.core.app:run"
+pygpt = "pygpt_net.core.app:run"
```

### Comparing `pygpt-net-0.9.4/setup.py` & `pygpt-net-0.9.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.9.4'
-DESCRIPTION = 'A GPT4, GPT3, ChatGPT and DALL-E 2 Desktop App with chatbot, text completion and image generation'
+VERSION = '0.9.5'
+DESCRIPTION = 'GPT4, GPT3, ChatGPT and DALL-E 2 Desktop App with chatbot, text completion and image generation'
 LONG_DESCRIPTION = 'A package containing a GPT4, GPT3, ChatGPT and DALL-E 2 desktop chatbot, ' \
                    'text completion and image generation app, using OpenAI API and your own API Key. ' \
                    'It includes context memory and history, editable presets, customizable UI and more.'
 
 setup(
     name='pygpt-net',
     version=VERSION,
@@ -19,16 +19,19 @@
     packages=find_packages('src'),
     package_dir={'': 'src'},
     package_data={'': ['CHANGELOG.txt', 'data/*', 'data/locale/*', 'data/config/*', 'data/config/presets/*']},
     url='https://github.com/szczyglis-dev/py-gpt',
     keywords='py_gpt, py-gpt, pygpt, desktop, app, gpt, gpt4, gpt3, chatgpt, dall-e, chat, chatbot, text completion,'
              'image generation, ai, api, openai, api key, context memory, history, presets, ui, qt, pyside',
     install_requires=[
+        'beautifulsoup4>=4.12.2',
         'openai>=0.27.4',
         'packaging>=23.0',
+        'pydub>=0.25.1',
         'pyinstaller>=5.9.0',
         'PySide6-Essentials>=6.4.2',
         'qt-material>=2.14',
         'show-in-file-manager>=1.1.4',
         'tiktoken>=0.3.3',
+        'wikipedia>=1.4.0',
     ],
 )
```

### Comparing `pygpt-net-0.9.4/src/pygpt_net/__init__.py` & `pygpt-net-0.9.5/src/pygpt_net/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2023.04.15 09:00:00                  #
+# Updated Date: 2023.04.16 09:00:00                  #
 # ================================================== #
 
 __author__ = "Marcin Szczygliński"
 __copyright__ = "Copyright 2023, Marcin Szczygliński"
 __credits__ = ["Marcin Szczygliński"]
 __license__ = "MIT"
-__version__ = "0.9.4"
-__build__ = "2023.04.15"
+__version__ = "0.9.5"
+__build__ = "2023.04.16"
 __maintainer__ = "Marcin Szczygliński"
 __github__ = "https://github.com/szczyglis-dev/py-gpt"
 __website__ = "https://pygpt.net"
 __email__ = "info@pygpt.net"
```

### Comparing `pygpt-net-0.9.4/src/pygpt_net/app.py` & `pygpt-net-0.9.5/src/pygpt_net/app.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/app.py` & `pygpt-net-0.9.5/src/pygpt_net/core/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Created By  : Marcin Szczygliński                  #
 # Updated Date: 2023.04.15 02:00:00                  #
 # ================================================== #
 
 import sys
 
 from PySide6.QtGui import QScreen
-from PySide6.QtCore import QTimer
+from PySide6.QtCore import QTimer, Signal, Slot
 from PySide6.QtWidgets import (QApplication, QMainWindow)
 from qt_material import QtStyleTools
 
 from .config import Config
 from .ui.main import UI
 from .controller.main import Controller
 from .debugger import Debug
@@ -24,17 +24,21 @@
 from .info import Info
 from .gpt import Gpt
 from .image import Image
 from .utils import get_init_value
 
 from .plugin.self_loop.plugin import Plugin as SelfLoopPlugin
 from .plugin.real_time.plugin import Plugin as RealTimePlugin
+from .plugin.web_search.plugin import Plugin as WebSearchPlugin
+from .plugin.audio_azure.plugin import Plugin as AudioAzurePlugin
 
 
 class MainWindow(QMainWindow, QtStyleTools):
+    statusChanged = Signal(str)
+
     def __init__(self):
         """App main window"""
         super().__init__()
         self.timer = None
         self.github = get_init_value("__github__")
         self.website = get_init_value("__website__")
         self.version = get_init_value("__version__")
@@ -62,14 +66,17 @@
 
         # setup UI
         self.ui = UI(self)
         self.ui.setup()
 
         self.setWindowTitle('PYGPT.net v{} | build {}'.format(self.version, self.build))
 
+        # setup signals
+        self.statusChanged.connect(self.update_status)
+
     def set_theme(self, theme='dark_teal.xml'):
         """
         Updates theme
 
         :param theme: theme name
         """
         label = "#ffffff"
@@ -114,14 +121,18 @@
         """
         Updates status text
 
         :param text: status text
         """
         self.data['status'].setText(str(text))
 
+    @Slot(str)
+    def update_status(self, text):
+        self.set_status(text)
+
     def closeEvent(self, event):
         """
         Handles close event
 
         :param event: close event
         """
         print("Closing...")
@@ -156,16 +167,17 @@
         self.window.setup_plugins()
 
     def run(self):
         """Runs app"""
         self.window.setup()
         available_geometry = self.window.screen().availableGeometry()
         pos = QScreen.availableGeometry(QApplication.primaryScreen()).topLeft()
-        self.window.resize(available_geometry.width(), available_geometry.height())
-        self.window.showMaximized()
+        self.window.resize(available_geometry.width() - 50, available_geometry.height() - 50)
+        # self.window.showMaximized()
+        self.window.show()
         self.window.move(pos)
 
         try:
             sys.exit(self.app.exec())
         except SystemExit:
             print("Closing...")
 
@@ -175,10 +187,12 @@
     # initialize app
     launcher = Launcher()
     launcher.init()
 
     # add plugins
     launcher.add_plugin(SelfLoopPlugin())
     launcher.add_plugin(RealTimePlugin())
+    launcher.add_plugin(WebSearchPlugin())
+    launcher.add_plugin(AudioAzurePlugin())
 
     # run app
     launcher.run()
```

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/config.py` & `pygpt-net-0.9.5/src/pygpt_net/core/config.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/context.py` & `pygpt-net-0.9.5/src/pygpt_net/core/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,16 +32,20 @@
 
     def load_list(self):
         """Loads contexts list from file"""
         path = os.path.join(self.config.path, 'context.json')
         try:
             if os.path.exists(path):
                 with open(path, 'r', encoding="utf-8") as file:
-                    self.contexts = json.load(file)['items']
+                    data = json.load(file)
                     file.close()
+                    if data == "" or data is None or 'items' not in data:
+                        self.contexts = {}
+                        return
+                    self.contexts = data['items']
         except Exception as e:
             print(e)
             self.contexts = {}
 
     def load(self, name):
         """
         Loads context from file
@@ -51,14 +55,16 @@
         """
         path = os.path.join(self.config.path, 'context', name + '.json')
         if os.path.exists(path):
             try:
                 with open(path, 'r', encoding="utf-8") as file:
                     data = self.parse(json.load(file))
                     file.close()
+                    if data == "" or data is None:
+                        return []
                     return data
             except Exception as e:
                 print("Error while loading context: {}".format(name))
                 print(e)
                 return []
         else:
             return []
```

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/controller/confirm.py` & `pygpt-net-0.9.5/src/pygpt_net/core/controller/confirm.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/controller/context.py` & `pygpt-net-0.9.5/src/pygpt_net/core/controller/context.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/controller/debug.py` & `pygpt-net-0.9.5/src/pygpt_net/core/controller/debug.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/controller/image.py` & `pygpt-net-0.9.5/src/pygpt_net/core/controller/image.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/controller/info.py` & `pygpt-net-0.9.5/src/pygpt_net/core/controller/info.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/controller/input.py` & `pygpt-net-0.9.5/src/pygpt_net/core/controller/input.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
 # Created Date: 2023.04.09 20:00:00                  #
 # ================================================== #
 
 from PySide6.QtGui import QTextCursor
+from PySide6.QtWidgets import QApplication
 
 from ..context import ContextItem
 from ..utils import trans
 
 
 class Input:
     def __init__(self, window=None):
@@ -58,15 +59,15 @@
 
     def send_text(self, text):
         """
         Sends text to GPT
 
         :param text: text to send
         """
-        self.window.set_status(trans('status.sending'))
+        self.window.statusChanged.emit(trans('status.sending'))
 
         # prepare names
         user_name = self.window.controller.plugins.apply('user.name', self.window.config.data['user_name'])
         ai_name = self.window.controller.plugins.apply('ai.name', self.window.config.data['ai_name'])
 
         # create ctx item
         ctx = ContextItem()
@@ -84,68 +85,76 @@
         self.window.controller.output.append_input(ctx)
 
         # call GPT
         try:
             try:
                 ctx = self.window.gpt.call(text, ctx)
             except Exception as e:
-                print(e)
+                print("Error in send text (GPT call): " + str(e))
                 self.window.ui.dialogs.alert(str(e))
                 self.window.set_status(trans('status.error'))
 
             ctx = self.window.controller.plugins.apply('ctx.after', ctx)  # apply plugins
             self.window.controller.output.append_output(ctx)
             self.window.gpt.context.store()
             self.window.set_status(
                 trans('status.tokens') + ": {} + {} = {}".format(ctx.input_tokens, ctx.output_tokens, ctx.total_tokens))
         except Exception as e:
-            print(e)
+            print("Error in send text: " + str(e))
             self.window.ui.dialogs.alert(str(e))
             self.window.set_status(trans('status.error'))
 
         return ctx
 
     def user_send(self, text=None):
         """Sends real user input"""
         text = self.window.controller.plugins.apply('user.send', text)
         self.send(text)
 
     def send(self, text=None):
         """
         Sends input text to API
         """
+        self.window.statusChanged.emit(trans('status.sending'))
+
         ctx = None
         if text is None:
             text = self.window.data['input'].toPlainText().strip()
         text = self.window.controller.plugins.apply('input.before', text)
 
         if len(text) > 0:
             if self.window.config.data['send_clear']:
                 self.window.data['input'].clear()
 
             # check API key
             if self.window.config.data['api_key'] is None or self.window.config.data['api_key'] == '':
                 self.window.controller.launcher.show_api_monit()
                 self.window.controller.ui.update()
+                self.window.statusChanged.emit("")
                 return
 
             # init api key if defined later
             self.window.gpt.init()
             self.window.images.init()
 
             # prepare context
             if len(self.window.gpt.context.contexts) == 0:
                 self.window.gpt.context.new()
                 self.window.controller.context.update()
 
+            # process events to update UI
+            QApplication.processEvents()
+
             # send to API
             if self.window.config.data['mode'] == 'img':
                 ctx = self.window.controller.image.send_text(text)
             else:
                 ctx = self.window.controller.input.send_text(text)
+        else:
+            self.window.statusChanged.emit("")
 
         ctx = self.window.controller.plugins.apply('ctx.end', ctx)  # apply plugins
         self.window.controller.ui.update()
 
     def append(self, text):
         """
         Appends text to input
```

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/controller/lang.py` & `pygpt-net-0.9.5/src/pygpt_net/core/controller/lang.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,15 +160,15 @@
         self.window.menu['menu.app'].setTitle(trans("menu.file"))
         self.window.menu['app.exit'].setText(trans("menu.file.exit"))
         self.window.menu['app.clear_history'].setText(trans("menu.file_clear_history"))
 
         self.window.menu['menu.plugins'].setTitle(trans("menu.plugins"))
 
         self.window.menu['menu.audio'].setTitle(trans("menu.audio"))
-        self.window.menu['audio.empty'].setText(trans("coming_soon"))
+        self.window.menu['audio.output'].setText(trans("menu.audio.output"))
 
         self.window.menu['menu.config'].setTitle(trans("menu.config"))
         self.window.menu['config.settings'].setText(trans("menu.config.settings"))
         self.window.menu['config.edit.config'].setText(trans("menu.config.edit.config"))
         self.window.menu['config.edit.models'].setText(trans("menu.config.edit.models"))
         self.window.menu['config.open_dir'].setText(trans("menu.config.open_dir"))
         self.window.menu['config.save'].setText(trans("menu.config.save"))
```

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/controller/launcher.py` & `pygpt-net-0.9.5/src/pygpt_net/core/controller/launcher.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/controller/main.py` & `pygpt-net-0.9.5/src/pygpt_net/core/controller/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2023.04.11 05:00:00                  #
+# Updated Date: 2023.04.16 06:00:00                  #
 # ================================================== #
 
 from .model import Model
 from .presets import Presets
 from .plugins import Plugins
 from .debug import Debug
 from .settings import Settings
@@ -20,14 +20,15 @@
 from .context import Context
 from .confirm import Confirm
 from .ui import UI
 from .launcher import Launcher
 from .lang import Lang
 from .image import Image
 from .theme import Theme
+from .audio import Audio
 
 
 class Controller:
     def __init__(self, window=None):
         """
         Main controller
 
@@ -45,14 +46,15 @@
         self.context = Context(window)
         self.confirm = Confirm(window)
         self.ui = UI(window)
         self.launcher = Launcher(window)
         self.lang = Lang(window)
         self.image = Image(window)
         self.theme = Theme(window)
+        self.audio = Audio(window)
 
     def setup(self):
         """Setups controller"""
         # setup plugins settings
         self.plugins.setup_settings()
 
         # init material theme
@@ -63,7 +65,8 @@
         self.model.setup()
         self.input.setup()
         self.output.setup()
         self.context.setup()
         self.ui.setup()
         self.info.setup()
         self.launcher.setup()
+        self.audio.setup()
```

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/controller/model.py` & `pygpt-net-0.9.5/src/pygpt_net/core/controller/model.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/controller/output.py` & `pygpt-net-0.9.5/src/pygpt_net/core/controller/output.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/controller/plugins.py` & `pygpt-net-0.9.5/src/pygpt_net/core/controller/plugins.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,16 +95,27 @@
                 option = options[key]
                 value = None
                 if option['type'] == 'int' or option['type'] == 'float':
                     if 'slider' in option and option['slider'] \
                             and (option['type'] == 'int' or option['type'] == 'float'):
                         value = self.window.plugin_option[id][key].slider.value()
                     else:
-                        value = self.window.plugin_option[id][key].input.text()
-                elif option['type'] == 'text' or option['type'] == 'textarea':
+                        if option['type'] == 'int':
+                            try:
+                                value = int(self.window.plugin_option[id][key].text())
+                            except ValueError:
+                                value = 0
+                        elif option['type'] == 'float':
+                            try:
+                                value = float(self.window.plugin_option[id][key].text())
+                            except ValueError:
+                                value = 0.0
+                elif option['type'] == 'text':
+                    value = self.window.plugin_option[id][key].text()
+                elif option['type'] == 'textarea':
                     value = self.window.plugin_option[id][key].toPlainText()
                 elif option['type'] == 'bool':
                     value = self.window.plugin_option[id][key].box.isChecked()
                 self.handler.plugins[id].options[key]['value'] = value
                 self.window.config.data['plugins'][id][key] = value
 
             # update config if option not exists
@@ -160,14 +171,18 @@
         """
         if self.handler.is_registered(id):
             self.enabled[id] = True
             self.handler.plugins[id].on_enable()  # call plugin enable method
             self.window.config.data['plugins_enabled'][id] = True
             self.window.config.save()
 
+            # update audio menu
+            if id == 'audio_azure':
+                self.window.controller.audio.update()
+
         self.update_info()
         self.update()
 
     def disable(self, id):
         """
         Disables plugin
 
@@ -175,14 +190,18 @@
         """
         if self.handler.is_registered(id):
             self.enabled[id] = False
             self.handler.plugins[id].on_disable()  # call plugin disable method
             self.window.config.data['plugins_enabled'][id] = False
             self.window.config.save()
 
+            # update audio menu
+            if id == 'audio_azure':
+                self.window.controller.audio.update()
+
         self.update_info()
         self.update()
 
     def is_enabled(self, id):
         """
         Checks if plugin is enabled
 
@@ -310,18 +329,19 @@
         option = self.get_option(self.current_plugin, key)
         if 'type' in option and option['type'] == 'int':
             value = round(int(value), 0)
         elif 'type' in option and option['type'] == 'float':
             value = float(value)
 
         if 'type' in option and option['type'] == 'int' or option['type'] == 'float':
-            if 'min' in option and value < option['min']:
-                value = option['min']
-            elif 'max' in option and value > option['max']:
-                value = option['max']
+            if value is not None:
+                if 'min' in option and option['min'] is not None and value < option['min']:
+                    value = option['min']
+                elif 'max' in option and option['max'] is not None and value > option['max']:
+                    value = option['max']
 
         self.window.plugin_option[self.current_plugin][key].setText('{}'.format(value))
 
     def config_slider(self, id, value, type=None):
         """
         Applies slider + input value
```

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/controller/presets.py` & `pygpt-net-0.9.5/src/pygpt_net/core/controller/presets.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/controller/settings.py` & `pygpt-net-0.9.5/src/pygpt_net/core/controller/settings.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/controller/theme.py` & `pygpt-net-0.9.5/src/pygpt_net/core/controller/theme.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
                         # checkbox
                         if option['type'] == 'bool':
                             if key in self.window.plugin_option[id]:
                                 self.window.plugin_option[id][key].box.setStyleSheet(self.get_style('checkbox'))
                         # text input
                         elif option['type'] == 'text':
                             if key in self.window.plugin_option[id]:
-                                self.window.plugin_option[id][key].input.setStyleSheet(self.get_style('line_edit'))
+                                self.window.plugin_option[id][key].setStyleSheet(self.get_style('line_edit'))
 
                         # input with slider
                         elif option['type'] == 'int' or option['type'] == 'float':
                             if key in self.window.plugin_option[id]:
                                 if 'slider' in option and option['slider']:
                                     self.window.plugin_option[id][key].input.setStyleSheet(self.get_style('line_edit'))
                                 else:
```

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/controller/ui.py` & `pygpt-net-0.9.5/src/pygpt_net/core/controller/ui.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/debug/config.py` & `pygpt-net-0.9.5/src/pygpt_net/core/debug/config.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/debug/context.py` & `pygpt-net-0.9.5/src/pygpt_net/core/debug/context.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/debug/models.py` & `pygpt-net-0.9.5/src/pygpt_net/core/debug/models.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/debug/plugins.py` & `pygpt-net-0.9.5/src/pygpt_net/core/debug/plugins.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/debug/presets.py` & `pygpt-net-0.9.5/src/pygpt_net/core/debug/presets.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/debugger.py` & `pygpt-net-0.9.5/src/pygpt_net/core/debugger.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/gpt.py` & `pygpt-net-0.9.5/src/pygpt_net/core/gpt.py`

 * *Files 8% similar despite different names*

```diff
@@ -85,30 +85,34 @@
             top_p=self.config.data['top_p'],
             frequency_penalty=self.config.data['frequency_penalty'],
             presence_penalty=self.config.data['presence_penalty'],
             stop=None,
         )
         return response
 
-    def build_chat_messages(self, prompt):
+    def build_chat_messages(self, prompt, system_prompt=None):
         """
         Builds chat messages dict
 
         :param prompt: Prompt
+        :param system_prompt: System prompt (optional)
         :return: Messages dict
         """
         messages = []
 
         model = self.config.data['model']
         used_tokens = self.count_used_tokens(prompt)
         max_tokens = self.config.data['max_total_tokens']
 
         # append initial (system) message
-        if self.system_prompt is not None and self.system_prompt != "":
-            messages.append({"role": "system", "content": self.system_prompt})
+        if system_prompt is not None and system_prompt != "":
+            messages.append({"role": "system", "content": system_prompt})
+        else:
+            if self.system_prompt is not None and self.system_prompt != "":
+                messages.append({"role": "system", "content": self.system_prompt})
 
         # append messages from context (memory)
         if self.config.data['use_context']:
             items = self.context.get_prompt_items(model, used_tokens, max_tokens)
             for item in items:
                 # input
                 if item.input is not None and item.input != "":
@@ -178,14 +182,44 @@
         tokens += num_tokens_prompt(self.system_prompt, self.user_name,
                                     model)  # init (system) prompt
         tokens += num_tokens_prompt(input_text, self.user_name, model)  # current input
         tokens += self.config.data['context_threshold']  # context threshold (reserved for next output)
         tokens += num_tokens_extra(model)  # extra tokens (required for output)
         return tokens
 
+    def quick_call(self, prompt, sys_prompt, append_context=False, max_tokens=500):
+        """
+        Calls OpenAI API with custom prompt
+
+        :param prompt: User input (prompt)
+        :param sys_prompt: System input (prompt)
+        :param max_tokens: Max output tokens
+        :return: Response text
+        """
+        if append_context:
+            messages = self.build_chat_messages(prompt, sys_prompt)
+        else:
+            messages = []
+            messages.append({"role": "system", "content": sys_prompt})
+            messages.append({"role": "user", "content": prompt})
+        try:
+            response = openai.ChatCompletion.create(
+                messages=messages,
+                model="gpt-3.5-turbo",
+                max_tokens=max_tokens,
+                temperature=1.0,
+                top_p=1.0,
+                frequency_penalty=0.0,
+                presence_penalty=0.0,
+                stop=None,
+            )
+            return response["choices"][0]["message"]["content"]
+        except Exception as e:
+            print("Error in custom call: " + str(e))
+
     def call(self, prompt, ctx=None):
         """
         Calls OpenAI API
 
         :param prompt: User input (prompt)
         :param ctx: Context item (memory)
         :return: Context item (memory)
```

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/history.py` & `pygpt-net-0.9.5/src/pygpt_net/core/history.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/image.py` & `pygpt-net-0.9.5/src/pygpt_net/core/image.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/info.py` & `pygpt-net-0.9.5/src/pygpt_net/core/info.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/locale.py` & `pygpt-net-0.9.5/src/pygpt_net/core/locale.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/plugin/base_plugin.py` & `pygpt-net-0.9.5/src/pygpt_net/core/plugin/base_plugin.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/plugin/real_time/plugin.py` & `pygpt-net-0.9.5/src/pygpt_net/core/plugin/real_time/plugin.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/plugin/self_loop/plugin.py` & `pygpt-net-0.9.5/src/pygpt_net/core/plugin/self_loop/plugin.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/plugins.py` & `pygpt-net-0.9.5/src/pygpt_net/core/plugins.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/settings.py` & `pygpt-net-0.9.5/src/pygpt_net/core/settings.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/tokens.py` & `pygpt-net-0.9.5/src/pygpt_net/core/tokens.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/ui/chatbox.py` & `pygpt-net-0.9.5/src/pygpt_net/core/ui/chatbox.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/ui/contexts.py` & `pygpt-net-0.9.5/src/pygpt_net/core/ui/contexts.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/ui/dialog/about.py` & `pygpt-net-0.9.5/src/pygpt_net/core/ui/dialog/about.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/ui/dialog/changelog.py` & `pygpt-net-0.9.5/src/pygpt_net/core/ui/dialog/changelog.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/ui/dialog/ctx_rename.py` & `pygpt-net-0.9.5/src/pygpt_net/core/ui/dialog/ctx_rename.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/ui/dialog/debug.py` & `pygpt-net-0.9.5/src/pygpt_net/core/ui/dialog/debug.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/ui/dialog/editor.py` & `pygpt-net-0.9.5/src/pygpt_net/core/ui/dialog/editor.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/ui/dialog/image.py` & `pygpt-net-0.9.5/src/pygpt_net/core/ui/dialog/image.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/ui/dialog/plugins.py` & `pygpt-net-0.9.5/src/pygpt_net/core/ui/dialog/plugins.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
 # Updated Date: 2023.04.15 00:00:00                  #
 # ================================================== #
-
+from PySide6.QtCore import Qt
 from PySide6.QtWidgets import QPushButton, QHBoxLayout, QLabel, QVBoxLayout, QScrollArea, QWidget, QTabWidget
 
 from ..widgets import SettingsInput, SettingsSlider, SettingsCheckbox, PluginSettingsDialog, SettingsTextarea
 from ...utils import trans
 
 
 class Plugins:
@@ -114,16 +114,21 @@
                 scroll_content.addLayout(self.add_option(key, option, self.window.plugin_option[id][key]))
 
             # scroll widget
             scroll_widget = QWidget()
             scroll_widget.setLayout(scroll_content)
             scroll.setWidget(scroll_widget)
 
+            desc_label = QLabel(plugin.description)
+            desc_label.setWordWrap(True)
+            desc_label.setAlignment(Qt.AlignCenter)
+            desc_label.setStyleSheet("font-weight: bold;")
+
             area = QVBoxLayout()
-            area.addWidget(QLabel(plugin.description))
+            area.addWidget(desc_label)
             area.addWidget(scroll)
 
             area_widget = QWidget()
             area_widget.setLayout(area)
 
             # append to tab
             tabs.addTab(area_widget, plugin.name)
@@ -147,26 +152,28 @@
         :param option: option
         :param widget: widget
         :return: QVBoxLayout
         """
         widget.setToolTip(option['tooltip'])
         label_key = key + '.label'
         self.window.data[label_key] = QLabel(trans(option['label']))
+        self.window.data[label_key].setStyleSheet("font-weight: bold;")
 
         cols = QHBoxLayout()
         cols.addWidget(self.window.data[label_key])
         cols.addWidget(widget)
 
         cols_widget = QWidget()
         cols_widget.setLayout(cols)
         cols_widget.setMaximumHeight(90)
 
-        desc_label = QLabel(option['description'])
+        desc_label = QLabel('<i>' + option['description'] + '</i>')
         desc_label.setWordWrap(True)
         desc_label.setMaximumHeight(30)
+        desc_label.setStyleSheet("font-size: 10px;")
 
         layout = QVBoxLayout()
         layout.addWidget(cols_widget)
         layout.addWidget(desc_label)
 
         return layout
```

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/ui/dialog/preset.py` & `pygpt-net-0.9.5/src/pygpt_net/core/ui/dialog/preset.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/ui/dialog/settings.py` & `pygpt-net-0.9.5/src/pygpt_net/core/ui/dialog/settings.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/ui/dialog/start.py` & `pygpt-net-0.9.5/src/pygpt_net/core/ui/dialog/start.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/ui/dialog/update.py` & `pygpt-net-0.9.5/src/pygpt_net/core/ui/dialog/update.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/ui/dialogs.py` & `pygpt-net-0.9.5/src/pygpt_net/core/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/ui/input.py` & `pygpt-net-0.9.5/src/pygpt_net/core/ui/input.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/ui/main.py` & `pygpt-net-0.9.5/src/pygpt_net/core/ui/main.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/ui/menu.py` & `pygpt-net-0.9.5/src/pygpt_net/core/ui/menu.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,18 +63,22 @@
         self.window.menu['plugins'] = {}
         self.window.menu['menu.plugins'] = self.window.menuBar().addMenu(trans("menu.plugins"))
         self.window.menu['menu.plugins'].setStyleSheet(self.window.controller.theme.get_style('menu'))  # Windows fix
         self.window.menu['menu.plugins'].addAction(self.window.menu['plugins.settings'])
 
     def setup_audio(self):
         """Setups audio menu"""
-        self.window.menu['audio.empty'] = QAction(QIcon.fromTheme("help-about"), trans("coming_soon"),
-                                                  self.window)
+        self.window.menu['audio.output'] = QAction(trans("menu.audio.output"),
+                                                  self.window, checkable=True)
+
+        self.window.menu['audio.output'].triggered.connect(
+            lambda: self.window.controller.plugins.toggle('audio_azure'))
+
         self.window.menu['menu.audio'] = self.window.menuBar().addMenu(trans("menu.audio"))
-        self.window.menu['menu.audio'].addAction(self.window.menu['audio.empty'])
+        self.window.menu['menu.audio'].addAction(self.window.menu['audio.output'])
 
     def setup_config(self):
         """Setups config menu"""
         self.window.menu['config.settings'] = QAction(trans("menu.config.settings"),
                                                       self.window)
         self.window.menu['config.edit.config'] = QAction(trans("menu.config.edit.config"),
                                                          self.window)
```

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/ui/status.py` & `pygpt-net-0.9.5/src/pygpt_net/core/ui/status.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/ui/toolbox.py` & `pygpt-net-0.9.5/src/pygpt_net/core/ui/toolbox.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/ui/widgets.py` & `pygpt-net-0.9.5/src/pygpt_net/core/ui/widgets.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/updater.py` & `pygpt-net-0.9.5/src/pygpt_net/core/updater.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.4/src/pygpt_net/core/utils.py` & `pygpt-net-0.9.5/src/pygpt_net/core/utils.py`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.4/src/pygpt_net/data/config/config.json` & `pygpt-net-0.9.5/src/pygpt_net/data/config/config.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9930555555555556%*

 * *Differences: {"'__meta__'": "{'version': '0.9.5', 'app.version': '0.9.5', 'updated_at': '2023-04-16T06:25:00'}"}*

```diff
@@ -1,12 +1,12 @@
 {
     "__meta__": {
-        "app.version": "0.9.4",
-        "updated_at": "2023-04-15T07:25:00",
-        "version": "0.9.4"
+        "app.version": "0.9.5",
+        "updated_at": "2023-04-16T06:25:00",
+        "version": "0.9.5"
     },
     "ai_name": "",
     "api_key": "",
     "context_threshold": 200,
     "ctx": "",
     "current_model": {
         "chat": "gpt-3.5-turbo",
```

### Comparing `pygpt-net-0.9.4/src/pygpt_net/data/config/models.json` & `pygpt-net-0.9.5/src/pygpt_net/data/config/models.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'__meta__'": "{'version': '0.9.5', 'app.version': '0.9.5', 'updated_at': '2023-04-16T07:25:00'}"}*

```diff
@@ -1,12 +1,12 @@
 {
     "__meta__": {
-        "app.version": "0.9.4",
-        "updated_at": "2023-04-15T07:25:00",
-        "version": "0.9.4"
+        "app.version": "0.9.5",
+        "updated_at": "2023-04-16T07:25:00",
+        "version": "0.9.5"
     },
     "gpt-3.5-turbo": {
         "id": "gpt-3.5-turbo",
         "mode": [
             "chat"
         ],
         "name": "gpt-3.5-turbo",
```

### Comparing `pygpt-net-0.9.4/src/pygpt_net/data/config/presets/dalle_woman_photorealistic.json` & `pygpt-net-0.9.5/src/pygpt_net/data/config/presets/dalle_woman_photorealistic.json`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.4/src/pygpt_net/data/icon.ico` & `pygpt-net-0.9.5/src/pygpt_net/data/icon.ico`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.4/src/pygpt_net/data/icon.png` & `pygpt-net-0.9.5/src/pygpt_net/data/icon.png`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.4/src/pygpt_net/data/locale/locale.en.ini` & `pygpt-net-0.9.5/src/pygpt_net/data/locale/locale.en.ini`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 info.settings.saved = Settings saved
 input.btn.send = Send
 input.label = Input (Your prompt)
 input.radio.enter = Enter
 input.radio.enter_shift = Shift+Enter
 input.send_clear = Clear on send
 menu.audio = Audio / Voice
+menu.audio.output = Enable voice synthesis (output)
 menu.config = Config
 menu.config.edit.config = Edit config.json...
 menu.config.edit.models = Edit models.json...
 menu.config.open_dir = Open config dir...
 menu.config.save = Save config
 menu.config.settings = Settings...
 menu.debug = Debug
@@ -123,15 +124,15 @@
 settings.top_p = Top-p
 settings.use_context = Use context (memory)
 settings.font_size = Font size (chat window)
 status.img.saved = Image saved
 status.started = Ready
 status.saved = Saved
 status.error = Ooopss... error occurred :(
-status.sending = Sending...
+status.sending = Please wait...
 status.preset.cleared = Preset cleared
 status.preset.deleted = Preset deleted
 status.preset.duplicated = Preset duplicated
 status.preset.saved = Preset saved
 status.preset.empty_id = WARNING: Preset ID (filename) is empty! Aborting...
 status.tokens = Tokens
 theme.dark = Dark
```

### Comparing `pygpt-net-0.9.4/src/pygpt_net/data/locale/locale.pl.ini` & `pygpt-net-0.9.5/src/pygpt_net/data/locale/locale.pl.ini`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 info.settings.saved = Zapisano
 input.btn.send = Wyślij
 input.label = Wejście (Twój prompt)
 input.radio.enter = Enter
 input.radio.enter_shift = Shift+Enter
 input.send_clear = Wyczyść po wysłaniu
 menu.audio = Audio / Mowa
+menu.audio.output = Wł. syntezę mowy (wyjście)
 menu.config = Opcje
 menu.config.edit.config = Edytuj config.json...
 menu.config.edit.models = Edytuj models.json...
 menu.config.open_dir = Otwórz katalog z konfiguracją...
 menu.config.save = Zapisz ustawienia
 menu.config.settings = Ustawienia...
 menu.debug = Debug
@@ -123,15 +124,15 @@
 settings.top_p = Top-p
 settings.use_context = Włącz kontekst (pamięć)
 settings.font_size = Rozmiar czcionki (okno chatu)
 status.img.saved = Obraz został zapisany
 status.started = Gotowy
 status.saved = Zapisano
 status.error = Upsss... wystąpił błąd :(
-status.sending = Wysyłanie...
+status.sending = Czekaj...
 status.preset.cleared = Preset wyczyszczony
 status.preset.deleted = Preset usunięty
 status.preset.duplicated = Preset skopiowany
 status.preset.saved = Preset zapisany
 status.preset.empty_id = Uwaga: nie podano ID dla presetu!
 status.tokens = Tokenów
 theme.dark = Ciemny
```

### Comparing `pygpt-net-0.9.4/src/pygpt_net/data/logo.png` & `pygpt-net-0.9.5/src/pygpt_net/data/logo.png`

 * *Files identical despite different names*

### Comparing `pygpt-net-0.9.4/src/pygpt_net.egg-info/PKG-INFO` & `pygpt-net-0.9.5/src/pygpt_net.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pygpt-net
-Version: 0.9.4
-Summary: A GPT4, GPT3, ChatGPT and DALL-E 2 Desktop App with chatbot, text completion and image generation
+Version: 0.9.5
+Summary: GPT4, GPT3, ChatGPT and DALL-E 2 Desktop App with chatbot, text completion and image generation
 Home-page: https://github.com/szczyglis-dev/py-gpt
 Author: Marcin Szczygliński
 Author-email: Marcin Szczygliński <info@pygpt.net>
 Maintainer: Marcin Szczygliński
 Maintainer-email: info@pygpt.net
 License: MIT License
         
@@ -36,55 +36,58 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PYGPT
 
-Current release: **0.9.4** (build: **2023.04.15**) | Official website: https://pygpt.net | Docs: https://pygpt.readthedocs.io
+Current release: **0.9.5** (build: **2023.04.16**) | Official website: https://pygpt.net | Docs: https://pygpt.readthedocs.io
 
 PyPi: https://pypi.org/project/pygpt-net
 
-### **Compiled binary versions for Windows 10, 11 and Linux are available to download on project's page**: https://pygpt.net (in "Download" section)
+### **Compiled versions for Windows 10, 11 and Linux**: https://pygpt.net/#download
 
 ## What is PYGPT?
 
 **PYGPT** is a desktop application that allows you to talk to OpenAI\'s
-artificial intelligence models such as **GPT4** and **GPT3** using your
-own computer and `OpenAI API`. It allows you to talk in chat mode and in
-completion mode, as well as generate images using **DALL-E 2**.
-Moreover, the application has implemented context memory support,
+LLM models such as **GPT4** and **GPT3** using your own computer and `OpenAI API`. 
+It allows you to talk in chat mode and in completion mode, as well as generate images 
+using **DALL-E 2**. PYGPT also adds access to the Internet for GPT via Google Custom 
+Search API and Wikipedia API and includes voice synthesis using Microsoft Azure 
+Text-to-Speech API. Moreover, the application has implemented context memory support,
 context storage, history of contexts, which can be restored at any time
 and e.g. continue the conversation from point in history, and also has a
 convenient and intuitive system of presets that allows you to quickly
-and pleasantly create and manage your prompts.
+and pleasantly create and manage your prompts. Plugins support is also available.
 
 ![app1](https://user-images.githubusercontent.com/61396542/230803425-5035ccd8-50d9-4fef-9774-8843cf3ce5b0.jpg)
 
-You can download compiled application for Windows and Linux on: https://pygpt.net/#download
+You can download compiled version for Windows and Linux at: https://pygpt.net/#download
 
 ## Features
 
 - desktop application for `Windows` and `Linux`, written in Python
 - works similar to `ChatGPT`, but locally (on desktop)
 - 3 modes of operation: chatbot, text completion and image generation
 - supports multiple models: `GPT4` and `GPT3`
 - handles and stores full context of the conversation (short-term
   memory)
+- adds access to the Internet for GPT via Google Custom Search API and Wikipedia API
+- includes voice synthesis using Microsoft Azure Text-to-Speech API
 - stores the history of contexts with the ability to return to
   previous context (long-term memory)
 - allows you to easily manage prompts with handly editable presets
 - intuitive operation and interface
 - allows you to use all the powerful features of `GPT4` and `GPT3`
 - no knowledge of using AI models required
 - enables easy and convenient generation of images using `DALL-E 2`
 - has the ability to support future OpenAI models
 - fully configurable
 - plugins support
-- built-in tokens usage calculation
+- built-in token usage calculation
 - it\'s open source, source code is available on `GitHub`
 - **uses the user\'s API key**
 
 The application is free, open source and runs on PC with `Windows 10`,
 `Windows 11` and `Linux`. The full **Python** source code is available
 on `GitHub`.
 
@@ -338,15 +341,15 @@
 one go. To set the required number of variants that you want to be
 generated, use the slider located in the corner on the right at the
 bottom of the screen (appears in place of the slider with the
 conversation temperature when switching to the image generation mode).
 
 ![dalle](https://user-images.githubusercontent.com/61396542/230803477-8ca3b13b-080d-4acc-9f19-fc2f1762e8e4.jpg)
 
-## Images storage
+## Image storage
 
 The image generated in this way can then be easily saved anywhere on the
 disk (just right-click on it), deleted or displayed in full size in the
 browser.
 
 **Tip:** with presets, you can save prepared prompts and use them later
 when generating subsequent images.
@@ -356,20 +359,29 @@
 generate new content.
 
 ## Plugins
 
 The application allows you to use plugins to extend its functionality.
 Currently, the following plugins are available:
 
-- **SelfLoop** - allows to run GPT in a self-loop, which allows you to
+- **Self Loop** - allows to run GPT in a self-loop, which allows you to
   generate a continuous conversation between AI <> AI. In this mode model talks to itself.
 
-- **RealTime** - auto-append current date and time to the prompt. It tells
+- **Real Time** - auto-append current date and time to the prompt. It tells
   the model what time it is in real time.
 
+- **Web Search** - adds access to the Internet using Google Custom Search Engine and Wikipedia API
+
+- **Audio (Azure)** - adds voice synthesis using Microsoft Azure Text-to-Speech API
+
+## Audio / voice synthesis
+
+The application offers voice synthesis using the **Microsoft Azure Text-To-Speech** API.
+It required your own Microsoft Azure API Key. 
+You can get Api Key for free from [here](https://azure.microsoft.com/en-us/services/cognitive-services/text-to-speech/).
 
 # Tokens calculation
 
 ## Input tokens
 
 Calculation of tokens is implemented in the application. The application
 tries to predict the number of tokens that will be used for a given
@@ -506,24 +518,35 @@
 window.
 
 Simply download the new version and use it instead of the current one,
 all configuration such as context and history will survive between
 versions and will be available in the newly installed version.
 
 
-# Plugins and audio (coming soon)
-
 ## Next releases
 
-Support for plug-ins and voice recognition and synthesis will be added
-in future versions of the application.
+Support for voice recognition will be added in future versions of the application.
 
+## DISCLAIMER
+
+This application is not affiliated with OpenAI in any way.
+Author is not responsible for any damage caused by the use of this application.
+Application is provided as is, without any warranty.
+Please also remember about tokens usage - always check the number of tokens used by 
+the model on OpenAI website and use the application responsibly.
+Enabled plugins (like e.g. Web Search) may use additional tokens,
+not listed in main window. Always control your real token usage on OpenAI website.
 
 # CHANGELOG
 
+## v0.9.5 (2023.04.16)
+
+- added web plugin (adds access to the Internet using Google Custom Search Engine and Wikipedia API)
+- added voice output plugin (adds voice synthesis using Microsoft Azure)
+
 ## v0.9.4 (2023.04.15)
 
 - added plugins support
 
 ## v0.9.3 (2023.04.14)
 
 - packed into PyPI package
```

### Comparing `pygpt-net-0.9.4/src/pygpt_net.egg-info/SOURCES.txt` & `pygpt-net-0.9.5/src/pygpt_net.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 src/pygpt_net/core/locale.py
 src/pygpt_net/core/plugins.py
 src/pygpt_net/core/settings.py
 src/pygpt_net/core/tokens.py
 src/pygpt_net/core/updater.py
 src/pygpt_net/core/utils.py
 src/pygpt_net/core/controller/__init__.py
+src/pygpt_net/core/controller/audio.py
 src/pygpt_net/core/controller/confirm.py
 src/pygpt_net/core/controller/context.py
 src/pygpt_net/core/controller/debug.py
 src/pygpt_net/core/controller/image.py
 src/pygpt_net/core/controller/info.py
 src/pygpt_net/core/controller/input.py
 src/pygpt_net/core/controller/lang.py
@@ -47,18 +48,23 @@
 src/pygpt_net/core/debug/config.py
 src/pygpt_net/core/debug/context.py
 src/pygpt_net/core/debug/models.py
 src/pygpt_net/core/debug/plugins.py
 src/pygpt_net/core/debug/presets.py
 src/pygpt_net/core/plugin/__init__.py
 src/pygpt_net/core/plugin/base_plugin.py
+src/pygpt_net/core/plugin/audio_azure/__init__.py
+src/pygpt_net/core/plugin/audio_azure/plugin.py
 src/pygpt_net/core/plugin/real_time/__init__.py
 src/pygpt_net/core/plugin/real_time/plugin.py
 src/pygpt_net/core/plugin/self_loop/__init__.py
 src/pygpt_net/core/plugin/self_loop/plugin.py
+src/pygpt_net/core/plugin/web_search/__init__.py
+src/pygpt_net/core/plugin/web_search/plugin.py
+src/pygpt_net/core/plugin/web_search/websearch.py
 src/pygpt_net/core/ui/__init__.py
 src/pygpt_net/core/ui/chatbox.py
 src/pygpt_net/core/ui/contexts.py
 src/pygpt_net/core/ui/dialogs.py
 src/pygpt_net/core/ui/input.py
 src/pygpt_net/core/ui/main.py
 src/pygpt_net/core/ui/menu.py
```

