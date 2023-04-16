# Comparing `tmp/alnoda_wrk-0.3.9.tar.gz` & `tmp/alnoda_wrk-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alnoda_wrk-0.3.9.tar", max compression
+gzip compressed data, was "alnoda_wrk-0.4.1.tar", max compression
```

## Comparing `alnoda_wrk-0.3.9.tar` & `alnoda_wrk-0.4.1.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0    34523 2022-08-26 16:21:54.054721 alnoda_wrk-0.3.9/LICENSE
--rw-r--r--   0        0        0       50 2022-08-26 16:21:54.054721 alnoda_wrk-0.3.9/README.md
--rw-r--r--   0        0        0       21 2022-08-26 16:21:54.054721 alnoda_wrk-0.3.9/alnoda_wrk/__init__.py
--rw-r--r--   0        0        0     2160 2023-03-15 17:54:18.518943 alnoda_wrk-0.3.9/alnoda_wrk/alnoda_api.py
--rw-r--r--   0        0        0     5250 2023-03-15 17:54:18.519943 alnoda_wrk-0.3.9/alnoda_wrk/builder.py
--rw-r--r--   0        0        0     7796 2023-03-15 17:54:18.520943 alnoda_wrk-0.3.9/alnoda_wrk/cheatsheet.py
--rw-r--r--   0        0        0     7143 2022-08-26 16:21:54.055721 alnoda_wrk-0.3.9/alnoda_wrk/conf_parser.py
--rw-r--r--   0        0        0     7706 2023-03-15 17:46:54.959179 alnoda_wrk-0.3.9/alnoda_wrk/config_schema.py
--rw-r--r--   0        0        0     7833 2022-09-07 14:40:58.132314 alnoda_wrk-0.3.9/alnoda_wrk/fileops.py
--rw-r--r--   0        0        0     1946 2023-03-15 17:54:18.520943 alnoda_wrk-0.3.9/alnoda_wrk/globals.py
--rw-r--r--   0        0        0     9557 2023-03-16 13:51:32.291104 alnoda_wrk-0.3.9/alnoda_wrk/install_app.py
--rw-r--r--   0        0        0     7523 2023-03-15 17:54:18.520943 alnoda_wrk-0.3.9/alnoda_wrk/links.py
--rw-r--r--   0        0        0     2679 2023-03-16 14:07:19.759204 alnoda_wrk-0.3.9/alnoda_wrk/main.py
--rw-r--r--   0        0        0    10786 2023-03-16 00:32:13.902598 alnoda_wrk-0.3.9/alnoda_wrk/meta_about.py
--rw-r--r--   0        0        0     1668 2022-11-01 14:08:08.668939 alnoda_wrk-0.3.9/alnoda_wrk/processes.py
--rw-r--r--   0        0        0     5362 2023-03-15 17:54:18.522943 alnoda_wrk-0.3.9/alnoda_wrk/share.py
--rw-r--r--   0        0        0     2351 2023-03-15 17:54:18.522943 alnoda_wrk-0.3.9/alnoda_wrk/sign_in.py
--rw-r--r--   0        0        0     3537 2022-10-24 16:31:09.586727 alnoda_wrk-0.3.9/alnoda_wrk/templates.py
--rw-r--r--   0        0        0        0 2022-09-03 08:06:50.028562 alnoda_wrk-0.3.9/alnoda_wrk/tui/__init__.py
--rw-r--r--   0        0        0     4641 2023-03-15 18:04:22.771086 alnoda_wrk-0.3.9/alnoda_wrk/tui/admin.py
--rw-r--r--   0        0        0     5969 2023-03-15 17:54:18.523943 alnoda_wrk-0.3.9/alnoda_wrk/tui/aliases_widget.py
--rw-r--r--   0        0        0    12260 2022-11-01 14:08:08.671939 alnoda_wrk-0.3.9/alnoda_wrk/tui/appearance_widget.py
--rw-r--r--   0        0        0     7166 2022-10-26 09:15:48.183939 alnoda_wrk-0.3.9/alnoda_wrk/tui/apps_services.py
--rw-r--r--   0        0        0    13400 2022-10-26 08:48:00.804887 alnoda_wrk-0.3.9/alnoda_wrk/tui/cheatsheet_widget.py
--rw-r--r--   0        0        0     2357 2022-09-04 16:06:07.306059 alnoda_wrk-0.3.9/alnoda_wrk/tui/description_widget.py
--rw-r--r--   0        0        0     5984 2023-03-15 17:54:18.523943 alnoda_wrk-0.3.9/alnoda_wrk/tui/env_vars_widget.py
--rw-r--r--   0        0        0     3135 2022-09-09 09:42:06.101097 alnoda_wrk-0.3.9/alnoda_wrk/tui/features_widget.py
--rw-r--r--   0        0        0      235 2022-09-03 08:06:50.032562 alnoda_wrk-0.3.9/alnoda_wrk/tui/gvars.py
--rw-r--r--   0        0        0      710 2022-09-06 16:00:47.678829 alnoda_wrk-0.3.9/alnoda_wrk/tui/helper_vidgets.py
--rw-r--r--   0        0        0     8471 2022-09-03 08:06:50.034562 alnoda_wrk-0.3.9/alnoda_wrk/tui/home.py
--rw-r--r--   0        0        0    13540 2022-10-26 09:27:26.705899 alnoda_wrk-0.3.9/alnoda_wrk/tui/interface_widget.py
--rw-r--r--   0        0        0    15046 2022-10-26 08:48:43.025601 alnoda_wrk-0.3.9/alnoda_wrk/tui/links_widget.py
--rw-r--r--   0        0        0      630 2023-03-15 17:54:18.524943 alnoda_wrk-0.3.9/alnoda_wrk/tui/my_notes_widget.py
--rw-r--r--   0        0        0     7868 2022-11-01 14:08:08.673939 alnoda_wrk-0.3.9/alnoda_wrk/tui/processes_widget.py
--rw-r--r--   0        0        0     8546 2023-03-15 17:54:18.524943 alnoda_wrk-0.3.9/alnoda_wrk/tui/share_widget.py
--rw-r--r--   0        0        0     3692 2023-03-15 17:54:18.524943 alnoda_wrk-0.3.9/alnoda_wrk/tui/signin_widget.py
--rw-r--r--   0        0        0      619 2023-03-15 17:54:18.524943 alnoda_wrk-0.3.9/alnoda_wrk/tui/zsh_widget.py
--rw-r--r--   0        0        0    13918 2022-10-27 12:16:55.545298 alnoda_wrk-0.3.9/alnoda_wrk/ui_builder.py
--rw-r--r--   0        0        0     1469 2022-09-10 20:05:49.819958 alnoda_wrk-0.3.9/alnoda_wrk/ui_styles.py
--rw-r--r--   0        0        0     8696 2022-10-31 11:25:28.357936 alnoda_wrk-0.3.9/alnoda_wrk/wrk/cheatsheet.json
--rw-r--r--   0        0        0      291 2022-10-11 08:46:44.470361 alnoda_wrk-0.3.9/alnoda_wrk/wrk/lineage.json
--rw-r--r--   0        0        0     1185 2022-10-24 16:31:09.598727 alnoda_wrk-0.3.9/alnoda_wrk/wrk/links.json
--rw-r--r--   0        0        0      253 2022-09-09 09:42:06.104097 alnoda_wrk-0.3.9/alnoda_wrk/wrk/meta.json
--rw-r--r--   0        0        0       86 2022-08-26 16:21:54.058721 alnoda_wrk-0.3.9/alnoda_wrk/wrk/requires/deps.txt
--rw-r--r--   0        0        0       13 2022-08-26 16:21:54.059721 alnoda_wrk-0.3.9/alnoda_wrk/wrk/requires/mkdocs.txt
--rw-r--r--   0        0        0      803 2022-08-26 16:21:54.059721 alnoda_wrk-0.3.9/alnoda_wrk/wrk/ui/.gitignore
--rw-r--r--   0        0        0     1056 2022-10-27 10:25:21.242272 alnoda_wrk-0.3.9/alnoda_wrk/wrk/ui/conf/ui-apps.json
--rw-r--r--   0        0        0      489 2022-08-26 16:21:54.059721 alnoda_wrk-0.3.9/alnoda_wrk/wrk/ui/docs/README.md
--rw-r--r--   0        0        0      287 2022-08-26 16:21:54.059721 alnoda_wrk-0.3.9/alnoda_wrk/wrk/ui/docs/about.md
--rw-r--r--   0        0        0    10831 2022-08-26 16:21:54.059721 alnoda_wrk-0.3.9/alnoda_wrk/wrk/ui/docs/assets/Alnoda-logo.svg
--rw-r--r--   0        0        0    15406 2022-08-26 16:21:54.060721 alnoda_wrk-0.3.9/alnoda_wrk/wrk/ui/docs/assets/favicon.ico
--rw-r--r--   0        0        0   256110 2022-08-26 16:21:54.061721 alnoda_wrk-0.3.9/alnoda_wrk/wrk/ui/docs/assets/home/Cronicle.jpg
--rw-r--r--   0        0        0   291683 2022-08-26 16:21:54.064721 alnoda_wrk-0.3.9/alnoda_wrk/wrk/ui/docs/assets/home/Filebrowser.png
--rw-r--r--   0        0        0   145945 2022-08-26 16:21:54.066721 alnoda_wrk-0.3.9/alnoda_wrk/wrk/ui/docs/assets/home/Htop.jpg
--rw-r--r--   0        0        0   110933 2022-08-26 16:21:54.072721 alnoda_wrk-0.3.9/alnoda_wrk/wrk/ui/docs/assets/home/MC.jpg
--rw-r--r--   0        0        0    52554 2022-08-26 16:21:54.074721 alnoda_wrk-0.3.9/alnoda_wrk/wrk/ui/docs/assets/home/Static-server.png
--rw-r--r--   0        0        0   158518 2022-08-26 16:21:54.075721 alnoda_wrk-0.3.9/alnoda_wrk/wrk/ui/docs/assets/home/Ungit.jpg
--rw-r--r--   0        0        0    58658 2022-08-26 16:21:54.075721 alnoda_wrk-0.3.9/alnoda_wrk/wrk/ui/docs/assets/home/terminal.png
--rw-r--r--   0        0        0     3322 2022-08-26 16:21:54.075721 alnoda_wrk-0.3.9/alnoda_wrk/wrk/ui/docs/assets/laptop-circle-white.svg
--rw-r--r--   0        0        0     3303 2022-08-26 16:21:54.076721 alnoda_wrk-0.3.9/alnoda_wrk/wrk/ui/docs/assets/laptop-circle.svg
--rw-r--r--   0        0        0        0 2022-10-11 08:46:44.472361 alnoda_wrk-0.3.9/alnoda_wrk/wrk/ui/docs/cheatsheet.md
--rw-r--r--   0        0        0      300 2022-08-26 16:21:54.076721 alnoda_wrk-0.3.9/alnoda_wrk/wrk/ui/docs/javascript/config.js
--rw-r--r--   0        0        0        0 2022-09-03 08:06:50.051562 alnoda_wrk-0.3.9/alnoda_wrk/wrk/ui/docs/manifest.txt
--rw-r--r--   0        0        0    28614 2022-10-25 08:07:27.499000 alnoda_wrk-0.3.9/alnoda_wrk/wrk/ui/docs/pages/my_apps/port-8029.png
--rw-r--r--   0        0        0    26222 2022-08-26 16:21:54.085721 alnoda_wrk-0.3.9/alnoda_wrk/wrk/ui/docs/pages/my_apps/port-8030.png
--rw-r--r--   0        0        0      491 2022-08-26 16:21:54.078721 alnoda_wrk-0.3.9/alnoda_wrk/wrk/ui/docs/pages/my_apps.md
--rw-r--r--   0        0        0      774 2022-09-10 20:04:56.132714 alnoda_wrk-0.3.9/alnoda_wrk/wrk/ui/docs/stylesheets/extra.css
--rw-r--r--   0        0        0     1112 2022-08-26 16:21:54.087721 alnoda_wrk-0.3.9/alnoda_wrk/wrk/ui/docs/stylesheets/quickstart.css
--rw-r--r--   0        0        0     3875 2022-09-17 17:03:25.346026 alnoda_wrk-0.3.9/alnoda_wrk/wrk/ui/macros/helpers.py
--rw-r--r--   0        0        0     1528 2023-03-16 00:41:16.909935 alnoda_wrk-0.3.9/alnoda_wrk/wrk/ui/mkdocs.yml
--rw-r--r--   0        0        0        0 2022-08-26 16:21:54.088721 alnoda_wrk-0.3.9/alnoda_wrk/wrk/ui/overrides/partials/footer.html
--rw-r--r--   0        0        0     4417 2022-09-07 10:58:08.492351 alnoda_wrk-0.3.9/alnoda_wrk/wrk_supervisor.py
--rw-r--r--   0        0        0     2916 2023-03-16 14:04:52.728745 alnoda_wrk-0.3.9/alnoda_wrk/zsh.py
--rw-r--r--   0        0        0      688 2023-03-16 14:08:32.774619 alnoda_wrk-0.3.9/pyproject.toml
--rw-r--r--   0        0        0     1509 2023-03-16 14:08:39.433625 alnoda_wrk-0.3.9/setup.py
--rw-r--r--   0        0        0      869 2023-03-16 14:08:39.434056 alnoda_wrk-0.3.9/PKG-INFO
+-rw-r--r--   0        0        0    34523 2022-08-26 16:21:54.054721 alnoda_wrk-0.4.1/LICENSE
+-rw-r--r--   0        0        0       50 2022-08-26 16:21:54.054721 alnoda_wrk-0.4.1/README.md
+-rw-r--r--   0        0        0       21 2022-08-26 16:21:54.054721 alnoda_wrk-0.4.1/alnoda_wrk/__init__.py
+-rw-r--r--   0        0        0     2159 2023-03-28 22:36:26.036464 alnoda_wrk-0.4.1/alnoda_wrk/alnoda_api.py
+-rw-r--r--   0        0        0     5250 2023-03-15 17:54:18.519943 alnoda_wrk-0.4.1/alnoda_wrk/builder.py
+-rw-r--r--   0        0        0     7796 2023-03-15 17:54:18.520943 alnoda_wrk-0.4.1/alnoda_wrk/cheatsheet.py
+-rw-r--r--   0        0        0     7143 2022-08-26 16:21:54.055721 alnoda_wrk-0.4.1/alnoda_wrk/conf_parser.py
+-rw-r--r--   0        0        0     7706 2023-03-15 17:46:54.959179 alnoda_wrk-0.4.1/alnoda_wrk/config_schema.py
+-rw-r--r--   0        0        0     7853 2023-04-14 20:52:02.650230 alnoda_wrk-0.4.1/alnoda_wrk/fileops.py
+-rw-r--r--   0        0        0     1946 2023-03-15 17:54:18.520943 alnoda_wrk-0.4.1/alnoda_wrk/globals.py
+-rw-r--r--   0        0        0    21886 2023-04-16 17:43:23.917433 alnoda_wrk-0.4.1/alnoda_wrk/install_app.py
+-rw-r--r--   0        0        0     7523 2023-03-15 17:54:18.520943 alnoda_wrk-0.4.1/alnoda_wrk/links.py
+-rw-r--r--   0        0        0     4055 2023-04-16 17:42:07.910514 alnoda_wrk-0.4.1/alnoda_wrk/main.py
+-rw-r--r--   0        0        0    11315 2023-03-28 22:36:26.039464 alnoda_wrk-0.4.1/alnoda_wrk/meta_about.py
+-rw-r--r--   0        0        0     1668 2022-11-01 14:08:08.668939 alnoda_wrk-0.4.1/alnoda_wrk/processes.py
+-rw-r--r--   0        0        0     5362 2023-03-15 17:54:18.522943 alnoda_wrk-0.4.1/alnoda_wrk/share.py
+-rw-r--r--   0        0        0     2351 2023-03-15 17:54:18.522943 alnoda_wrk-0.4.1/alnoda_wrk/sign_in.py
+-rw-r--r--   0        0        0     3537 2022-10-24 16:31:09.586727 alnoda_wrk-0.4.1/alnoda_wrk/templates.py
+-rw-r--r--   0        0        0        0 2022-09-03 08:06:50.028562 alnoda_wrk-0.4.1/alnoda_wrk/tui/__init__.py
+-rw-r--r--   0        0        0     4641 2023-03-15 18:04:22.771086 alnoda_wrk-0.4.1/alnoda_wrk/tui/admin.py
+-rw-r--r--   0        0        0     5969 2023-03-15 17:54:18.523943 alnoda_wrk-0.4.1/alnoda_wrk/tui/aliases_widget.py
+-rw-r--r--   0        0        0    12260 2022-11-01 14:08:08.671939 alnoda_wrk-0.4.1/alnoda_wrk/tui/appearance_widget.py
+-rw-r--r--   0        0        0     7166 2022-10-26 09:15:48.183939 alnoda_wrk-0.4.1/alnoda_wrk/tui/apps_services.py
+-rw-r--r--   0        0        0    13400 2022-10-26 08:48:00.804887 alnoda_wrk-0.4.1/alnoda_wrk/tui/cheatsheet_widget.py
+-rw-r--r--   0        0        0     2357 2022-09-04 16:06:07.306059 alnoda_wrk-0.4.1/alnoda_wrk/tui/description_widget.py
+-rw-r--r--   0        0        0     5984 2023-03-15 17:54:18.523943 alnoda_wrk-0.4.1/alnoda_wrk/tui/env_vars_widget.py
+-rw-r--r--   0        0        0     3135 2022-09-09 09:42:06.101097 alnoda_wrk-0.4.1/alnoda_wrk/tui/features_widget.py
+-rw-r--r--   0        0        0      235 2022-09-03 08:06:50.032562 alnoda_wrk-0.4.1/alnoda_wrk/tui/gvars.py
+-rw-r--r--   0        0        0      710 2022-09-06 16:00:47.678829 alnoda_wrk-0.4.1/alnoda_wrk/tui/helper_vidgets.py
+-rw-r--r--   0        0        0     8471 2022-09-03 08:06:50.034562 alnoda_wrk-0.4.1/alnoda_wrk/tui/home.py
+-rw-r--r--   0        0        0    13540 2022-10-26 09:27:26.705899 alnoda_wrk-0.4.1/alnoda_wrk/tui/interface_widget.py
+-rw-r--r--   0        0        0    15046 2022-10-26 08:48:43.025601 alnoda_wrk-0.4.1/alnoda_wrk/tui/links_widget.py
+-rw-r--r--   0        0        0      630 2023-03-15 17:54:18.524943 alnoda_wrk-0.4.1/alnoda_wrk/tui/my_notes_widget.py
+-rw-r--r--   0        0        0     7868 2022-11-01 14:08:08.673939 alnoda_wrk-0.4.1/alnoda_wrk/tui/processes_widget.py
+-rw-r--r--   0        0        0     8546 2023-03-15 17:54:18.524943 alnoda_wrk-0.4.1/alnoda_wrk/tui/share_widget.py
+-rw-r--r--   0        0        0     3692 2023-03-15 17:54:18.524943 alnoda_wrk-0.4.1/alnoda_wrk/tui/signin_widget.py
+-rw-r--r--   0        0        0      619 2023-03-15 17:54:18.524943 alnoda_wrk-0.4.1/alnoda_wrk/tui/zsh_widget.py
+-rw-r--r--   0        0        0    13918 2022-10-27 12:16:55.545298 alnoda_wrk-0.4.1/alnoda_wrk/ui_builder.py
+-rw-r--r--   0        0        0     1469 2022-09-10 20:05:49.819958 alnoda_wrk-0.4.1/alnoda_wrk/ui_styles.py
+-rw-r--r--   0        0        0     9485 2023-04-13 18:51:15.320292 alnoda_wrk-0.4.1/alnoda_wrk/wrk/cheatsheet.json
+-rw-r--r--   0        0        0      286 2023-04-12 21:27:02.421900 alnoda_wrk-0.4.1/alnoda_wrk/wrk/lineage.json
+-rw-r--r--   0        0        0     1947 2023-03-19 22:28:40.727499 alnoda_wrk-0.4.1/alnoda_wrk/wrk/links.json
+-rw-r--r--   0        0        0      253 2022-09-09 09:42:06.104097 alnoda_wrk-0.4.1/alnoda_wrk/wrk/meta.json
+-rw-r--r--   0        0        0       86 2022-08-26 16:21:54.058721 alnoda_wrk-0.4.1/alnoda_wrk/wrk/requires/deps.txt
+-rw-r--r--   0        0        0       13 2022-08-26 16:21:54.059721 alnoda_wrk-0.4.1/alnoda_wrk/wrk/requires/mkdocs.txt
+-rw-r--r--   0        0        0      803 2022-08-26 16:21:54.059721 alnoda_wrk-0.4.1/alnoda_wrk/wrk/ui/.gitignore
+-rw-r--r--   0        0        0     1056 2022-10-27 10:25:21.242272 alnoda_wrk-0.4.1/alnoda_wrk/wrk/ui/conf/ui-apps.json
+-rw-r--r--   0        0        0      489 2022-08-26 16:21:54.059721 alnoda_wrk-0.4.1/alnoda_wrk/wrk/ui/docs/README.md
+-rw-r--r--   0        0        0      287 2022-08-26 16:21:54.059721 alnoda_wrk-0.4.1/alnoda_wrk/wrk/ui/docs/about.md
+-rw-r--r--   0        0        0    10831 2022-08-26 16:21:54.059721 alnoda_wrk-0.4.1/alnoda_wrk/wrk/ui/docs/assets/Alnoda-logo.svg
+-rw-r--r--   0        0        0    15406 2022-08-26 16:21:54.060721 alnoda_wrk-0.4.1/alnoda_wrk/wrk/ui/docs/assets/favicon.ico
+-rw-r--r--   0        0        0   256110 2022-08-26 16:21:54.061721 alnoda_wrk-0.4.1/alnoda_wrk/wrk/ui/docs/assets/home/Cronicle.jpg
+-rw-r--r--   0        0        0   291683 2022-08-26 16:21:54.064721 alnoda_wrk-0.4.1/alnoda_wrk/wrk/ui/docs/assets/home/Filebrowser.png
+-rw-r--r--   0        0        0   145945 2022-08-26 16:21:54.066721 alnoda_wrk-0.4.1/alnoda_wrk/wrk/ui/docs/assets/home/Htop.jpg
+-rw-r--r--   0        0        0   110933 2022-08-26 16:21:54.072721 alnoda_wrk-0.4.1/alnoda_wrk/wrk/ui/docs/assets/home/MC.jpg
+-rw-r--r--   0        0        0    52554 2022-08-26 16:21:54.074721 alnoda_wrk-0.4.1/alnoda_wrk/wrk/ui/docs/assets/home/Static-server.png
+-rw-r--r--   0        0        0   158518 2022-08-26 16:21:54.075721 alnoda_wrk-0.4.1/alnoda_wrk/wrk/ui/docs/assets/home/Ungit.jpg
+-rw-r--r--   0        0        0    58658 2022-08-26 16:21:54.075721 alnoda_wrk-0.4.1/alnoda_wrk/wrk/ui/docs/assets/home/terminal.png
+-rw-r--r--   0        0        0     3322 2022-08-26 16:21:54.075721 alnoda_wrk-0.4.1/alnoda_wrk/wrk/ui/docs/assets/laptop-circle-white.svg
+-rw-r--r--   0        0        0     3303 2022-08-26 16:21:54.076721 alnoda_wrk-0.4.1/alnoda_wrk/wrk/ui/docs/assets/laptop-circle.svg
+-rw-r--r--   0        0        0        0 2022-10-11 08:46:44.472361 alnoda_wrk-0.4.1/alnoda_wrk/wrk/ui/docs/cheatsheet.md
+-rw-r--r--   0        0        0      300 2022-08-26 16:21:54.076721 alnoda_wrk-0.4.1/alnoda_wrk/wrk/ui/docs/javascript/config.js
+-rw-r--r--   0        0        0        0 2022-09-03 08:06:50.051562 alnoda_wrk-0.4.1/alnoda_wrk/wrk/ui/docs/manifest.txt
+-rw-r--r--   0        0        0    28614 2022-10-25 08:07:27.499000 alnoda_wrk-0.4.1/alnoda_wrk/wrk/ui/docs/pages/my_apps/port-8029.png
+-rw-r--r--   0        0        0    26222 2022-08-26 16:21:54.085721 alnoda_wrk-0.4.1/alnoda_wrk/wrk/ui/docs/pages/my_apps/port-8030.png
+-rw-r--r--   0        0        0      491 2022-08-26 16:21:54.078721 alnoda_wrk-0.4.1/alnoda_wrk/wrk/ui/docs/pages/my_apps.md
+-rw-r--r--   0        0        0      774 2022-09-10 20:04:56.132714 alnoda_wrk-0.4.1/alnoda_wrk/wrk/ui/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0     1112 2022-08-26 16:21:54.087721 alnoda_wrk-0.4.1/alnoda_wrk/wrk/ui/docs/stylesheets/quickstart.css
+-rw-r--r--   0        0        0     3875 2022-09-17 17:03:25.346026 alnoda_wrk-0.4.1/alnoda_wrk/wrk/ui/macros/helpers.py
+-rw-r--r--   0        0        0     1528 2023-03-16 00:41:16.909935 alnoda_wrk-0.4.1/alnoda_wrk/wrk/ui/mkdocs.yml
+-rw-r--r--   0        0        0        0 2022-08-26 16:21:54.088721 alnoda_wrk-0.4.1/alnoda_wrk/wrk/ui/overrides/partials/footer.html
+-rw-r--r--   0        0        0     4428 2023-03-17 00:44:50.092440 alnoda_wrk-0.4.1/alnoda_wrk/wrk_supervisor.py
+-rw-r--r--   0        0        0     2916 2023-03-16 14:04:52.728745 alnoda_wrk-0.4.1/alnoda_wrk/zsh.py
+-rw-r--r--   0        0        0      688 2023-04-16 17:45:03.395610 alnoda_wrk-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1509 2023-04-16 17:45:18.272915 alnoda_wrk-0.4.1/setup.py
+-rw-r--r--   0        0        0      869 2023-04-16 17:45:18.273174 alnoda_wrk-0.4.1/PKG-INFO
```

### Comparing `alnoda_wrk-0.3.9/LICENSE` & `alnoda_wrk-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alnoda_wrk-0.3.9/alnoda_wrk/alnoda_api.py` & `alnoda_wrk-0.4.1/alnoda_wrk/alnoda_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,14 @@
                 'workspace_id': meta['workspace_id'], 
                 'workspace_name': meta['name'],
                 'workspace_version': meta['version'],
                 'workspace_created': meta['created']
                 }
             self.authenticated = True
         except: pass
-
     def fetch(self, data):
         if not self.authenticated:
             return False, {'error': 'Not authenticated at alnoda.org'} 
         self.payload.update(data)
         try:
             headers = {'Content-type': 'application/json'}
             response = requests.post(self.url, json=self.payload, headers=headers)
```

### Comparing `alnoda_wrk-0.3.9/alnoda_wrk/builder.py` & `alnoda_wrk-0.4.1/alnoda_wrk/builder.py`

 * *Files identical despite different names*

### Comparing `alnoda_wrk-0.3.9/alnoda_wrk/cheatsheet.py` & `alnoda_wrk-0.4.1/alnoda_wrk/cheatsheet.py`

 * *Files identical despite different names*

### Comparing `alnoda_wrk-0.3.9/alnoda_wrk/conf_parser.py` & `alnoda_wrk-0.4.1/alnoda_wrk/conf_parser.py`

 * *Files identical despite different names*

### Comparing `alnoda_wrk-0.3.9/alnoda_wrk/config_schema.py` & `alnoda_wrk-0.4.1/alnoda_wrk/config_schema.py`

 * *Files identical despite different names*

### Comparing `alnoda_wrk-0.3.9/alnoda_wrk/fileops.py` & `alnoda_wrk-0.4.1/alnoda_wrk/fileops.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,27 +161,25 @@
             if "#" in p: colpart = p
         col_ = colpart.replace(";","")
         col_ = col_.replace("\n","")
         col_ = col_.replace("\t","")
         col_ = col_.replace("!important","")
         col_ = col_.strip()
         return col_
-
     def col_map(line, group, styles_dict):
         if "--md-primary-fg-color" in line:             styles_dict[group]["primary"] = get_color(line)
         elif "--md-accent-fg-color" in line:            styles_dict[group]["accent"] = get_color(line)
         elif "--md-default-bg-color" in line:           styles_dict[group]["background"] = get_color(line)
         elif "--md-default-fg-color--light" in line:    styles_dict[group]["subtitle"] = get_color(line)
         elif "--md-typeset-color" in line:              styles_dict[group]["text"] = get_color(line)
         elif "--md-typeset-a-color" in line:            styles_dict[group]["title"] = get_color(line)
         elif "--md-code-bg-color" in line:              styles_dict[group]["code_background"] = get_color(line)
         elif "--md-code-fg-color" in line:              styles_dict[group]["code_text"] = get_color(line)
         elif "--md-code-fg-color" in line:              styles_dict[group]["code_text"] = get_color(line)
         return styles_dict
-
     with open(WORKSPACE_UI_SCSS_STYLES_FILE) as styles_file:
         styles_lines = styles_file.readlines()
     styles_dict = {}
     group = ""
     for idx, line in enumerate(styles_lines):
         if 'data-md-color-scheme="workspace"' in line:
             group = "light"
@@ -253,8 +251,9 @@
     Add line to the ~/.zshrc file
     :param line: new line to add to the  ~/.zshrc file 
     :type line: str
     """
     with open(ZSHRC_FILE, "a") as f:
         # Append 'hello' at the end of file
         f.write(line)
+        f.write("\n")
     return
```

### Comparing `alnoda_wrk-0.3.9/alnoda_wrk/globals.py` & `alnoda_wrk-0.4.1/alnoda_wrk/globals.py`

 * *Files identical despite different names*

### Comparing `alnoda_wrk-0.3.9/alnoda_wrk/links.py` & `alnoda_wrk-0.4.1/alnoda_wrk/links.py`

 * *Files identical despite different names*

### Comparing `alnoda_wrk-0.3.9/alnoda_wrk/main.py` & `alnoda_wrk-0.4.1/alnoda_wrk/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 import os
+from typing import Optional
 import typer
 from .builder import init_wrk, build_workspace, delete_wrk, install_mkdocs_deps
 from .ui_builder import get_mkdocs_yml, update_mkdocs_yml
 from .meta_about import *
-from .wrk_supervisor import create_supervisord_file
+from .wrk_supervisor import create_supervisord_file, stop_app
 from .tui.admin import open_admin
 from .install_app import add_app
-from .zsh import add_user_env_var
+from .zsh import add_user_env_var, add_user_alias
+from .sign_in import add_token, delete_auth
+from .cheatsheet import add_cheatsheet_section, add_cheatsheet_command
+from .links import add_links_section, add_links_url
 
 app = typer.Typer()
 
 def cls():
     """ Clean (terminal) screen """
     os.system('cls' if os.name == 'nt' else 'clear')
     return
 
 @app.command()
 def deps():
-    """ Install/Update mkdocs dependencies """
+    """ Install/Update wrk dependencies """
     install_mkdocs_deps()
     return
     
 @app.command()
 def init():
     """ Initialize workspace folder """
     typer.echo("Initializing $HOME/.wrk")
@@ -73,41 +77,97 @@
     refresh_from_meta()
     refresh_about()
     return
 
 @app.command()
 def start(name: str, cmd: str):
     """
-    Start application
+    Start application or service as daemon
     """
     create_supervisord_file(name, cmd)
     return
 
 @app.command()
+def stop(name: str):
+    """
+    Stop daemonnized application or service 
+    """
+    stop_app(name)
+
+@app.command()
 def admin():
     """
     Open Admin TUI
     """
     open_admin()
 
 @app.command()
-def install(application):
+def install(application, page: Optional[str] = typer.Argument("home"), silent: Optional[bool] = typer.Argument(False)):
     """
     Install app from alnoda.org
     """
     if '==' in application:
         app_ = application.split('==')
         app_code = app_[0]
         version = app_[1] 
-        add_app(app_code, version=version, silent=False)
+        add_app(app_code, version=version, page=page, silent=silent)
     else:
         app_code = application 
-        add_app(app_code, version=None, silent=False)
+        add_app(app_code, version=None, page=page, silent=silent)
     return
 
 @app.command()
 def setvar(name, value):
     """
-    Set environmental variable name='value'
+    Set terminal environmental variable name='value'
     """
     add_user_env_var(name, value)
     return
+
+@app.command()
+def alias(name, cmd):
+    """
+    Set alias for zsh name='value'
+    """
+    add_user_alias(name, cmd)
+
+@app.command()
+def signin(token):
+    """
+    Autheticate workspace at alnoda.org 
+    """
+    add_token(token)
+
+@app.command()
+def signout():
+    """
+    Log out workspace from alnoda.org 
+    """
+    delete_auth()
+
+@app.command()
+def cheatsec(name):
+    """
+    Add cheatsheet section 
+    """
+    add_cheatsheet_section(name)
+
+@app.command()
+def cheat(section, cmd, description):
+    """
+    Add cheatsheet command to some section
+    """
+    add_cheatsheet_command(section, cmd, description)
+
+@app.command()
+def linksec(name):
+    """
+    Add links section 
+    """
+    add_links_section(name)
+
+@app.command()
+def link(section, url, name, description):
+    """
+    Add new record to the existing link section  
+    """
+    add_links_url(section, url, name, description)
```

### Comparing `alnoda_wrk-0.3.9/alnoda_wrk/meta_about.py` & `alnoda_wrk-0.4.1/alnoda_wrk/meta_about.py`

 * *Files 3% similar despite different names*

```diff
@@ -140,19 +140,22 @@
     :type version: str
     :param author: workspace author
     :type author: str
     :param description: workspace description
     :type description: str
     :param docs: link to the workspace documentation
     :type docs: str
+    :param tags: workspace tags. String of comma-separated tags
+    :type tags: str
     :param repository: link to the workspace source code
     :type repository: str
     :param update_created: should 'created' be updated in the meta.json? (Default is True)
     :type update_created: bool
     """
+    # first read existing meta
     meta_dict = read_meta()
     # if workspace_id not yet in meta - generate new, and add it to meta
     if 'workspace_id' not in meta_dict: meta_dict['workspace_id'] = get_code(length=16)
     if 'created' not in meta_dict: meta_dict['created'] = datetime.today().strftime('%Y-%m-%d')
     # update meta_dict with the respective input
     if name is not None:
         meta_dict['name'] = name
@@ -314,37 +317,49 @@
     if ALNODA_APPS_KEY not in meta_dict: return False
     else:
         if app_code in meta_dict[ALNODA_APPS_KEY]:
             return True
     return False
 
 
-def log_app_installed(app_code, name, version, desctiption):
+def is_port_in_app_use(port):
+    """ Check if alnoda apps do not use this port """
+    meta_dict = read_meta()
+    if "alnoda.org.apps" not in meta_dict: return False
+    for k,v in meta_dict['alnoda.org.apps'].items():
+        if "port" in v and v['port'] == port: return True
+    return False
+
+
+def log_app_installed(app_code, name, version, desctiption, app_port=None):
     """  ->> str
     Log in meta that some app is installed
 
     :param app_code: app code on the alnoda.org
     :type app_code: str
     :param name:  app name on the alnoda.org
     :type name: str
     :param version:  app version on the alnoda.org
     :type version: str
     :param desctiption:  app description on the alnoda.org
     :type desctiption: str
+    : param app_port: port app is listening to
+    :type app_port: int
     """
     meta_dict = read_meta()
     # if apps is not yet present in meta - add it
     if ALNODA_APPS_KEY not in meta_dict:
         meta_dict[ALNODA_APPS_KEY] = {}
     # if this app is already present - return
     if app_code in meta_dict[ALNODA_APPS_KEY]: return
     # add app to meta and save meta
     meta_dict[ALNODA_APPS_KEY][app_code] = {
         'name': name,
         'version': version,
         'desctiption': desctiption,
-        'date': datetime.today().strftime('%Y-%m-%d')
+        'date': datetime.today().strftime('%Y-%m-%d'),
+        'app_port': app_port
     }
     write_meta(meta_dict)
     return
```

### Comparing `alnoda_wrk-0.3.9/alnoda_wrk/processes.py` & `alnoda_wrk-0.4.1/alnoda_wrk/processes.py`

 * *Files identical despite different names*

### Comparing `alnoda_wrk-0.3.9/alnoda_wrk/share.py` & `alnoda_wrk-0.4.1/alnoda_wrk/share.py`

 * *Files identical despite different names*

### Comparing `alnoda_wrk-0.3.9/alnoda_wrk/sign_in.py` & `alnoda_wrk-0.4.1/alnoda_wrk/sign_in.py`

 * *Files identical despite different names*

### Comparing `alnoda_wrk-0.3.9/alnoda_wrk/templates.py` & `alnoda_wrk-0.4.1/alnoda_wrk/templates.py`

 * *Files identical despite different names*

### Comparing `alnoda_wrk-0.3.9/alnoda_wrk/tui/admin.py` & `alnoda_wrk-0.4.1/alnoda_wrk/tui/admin.py`

 * *Files identical despite different names*

### Comparing `alnoda_wrk-0.3.9/alnoda_wrk/tui/aliases_widget.py` & `alnoda_wrk-0.4.1/alnoda_wrk/tui/aliases_widget.py`

 * *Files identical despite different names*

### Comparing `alnoda_wrk-0.3.9/alnoda_wrk/tui/appearance_widget.py` & `alnoda_wrk-0.4.1/alnoda_wrk/tui/appearance_widget.py`

 * *Files identical despite different names*

### Comparing `alnoda_wrk-0.3.9/alnoda_wrk/tui/apps_services.py` & `alnoda_wrk-0.4.1/alnoda_wrk/tui/apps_services.py`

 * *Files identical despite different names*

### Comparing `alnoda_wrk-0.3.9/alnoda_wrk/tui/cheatsheet_widget.py` & `alnoda_wrk-0.4.1/alnoda_wrk/tui/cheatsheet_widget.py`

 * *Files identical despite different names*

### Comparing `alnoda_wrk-0.3.9/alnoda_wrk/tui/description_widget.py` & `alnoda_wrk-0.4.1/alnoda_wrk/tui/description_widget.py`

 * *Files identical despite different names*

### Comparing `alnoda_wrk-0.3.9/alnoda_wrk/tui/env_vars_widget.py` & `alnoda_wrk-0.4.1/alnoda_wrk/tui/env_vars_widget.py`

 * *Files identical despite different names*

### Comparing `alnoda_wrk-0.3.9/alnoda_wrk/tui/features_widget.py` & `alnoda_wrk-0.4.1/alnoda_wrk/tui/features_widget.py`

 * *Files identical despite different names*

### Comparing `alnoda_wrk-0.3.9/alnoda_wrk/tui/helper_vidgets.py` & `alnoda_wrk-0.4.1/alnoda_wrk/tui/helper_vidgets.py`

 * *Files identical despite different names*

### Comparing `alnoda_wrk-0.3.9/alnoda_wrk/tui/home.py` & `alnoda_wrk-0.4.1/alnoda_wrk/tui/home.py`

 * *Files identical despite different names*

### Comparing `alnoda_wrk-0.3.9/alnoda_wrk/tui/interface_widget.py` & `alnoda_wrk-0.4.1/alnoda_wrk/tui/interface_widget.py`

 * *Files identical despite different names*

### Comparing `alnoda_wrk-0.3.9/alnoda_wrk/tui/links_widget.py` & `alnoda_wrk-0.4.1/alnoda_wrk/tui/links_widget.py`

 * *Files identical despite different names*

### Comparing `alnoda_wrk-0.3.9/alnoda_wrk/tui/my_notes_widget.py` & `alnoda_wrk-0.4.1/alnoda_wrk/tui/my_notes_widget.py`

 * *Files identical despite different names*

### Comparing `alnoda_wrk-0.3.9/alnoda_wrk/tui/processes_widget.py` & `alnoda_wrk-0.4.1/alnoda_wrk/tui/processes_widget.py`

 * *Files identical despite different names*

### Comparing `alnoda_wrk-0.3.9/alnoda_wrk/tui/share_widget.py` & `alnoda_wrk-0.4.1/alnoda_wrk/tui/share_widget.py`

 * *Files identical despite different names*

### Comparing `alnoda_wrk-0.3.9/alnoda_wrk/tui/signin_widget.py` & `alnoda_wrk-0.4.1/alnoda_wrk/tui/signin_widget.py`

 * *Files identical despite different names*

### Comparing `alnoda_wrk-0.3.9/alnoda_wrk/tui/zsh_widget.py` & `alnoda_wrk-0.4.1/alnoda_wrk/tui/zsh_widget.py`

 * *Files identical despite different names*

### Comparing `alnoda_wrk-0.3.9/alnoda_wrk/ui_builder.py` & `alnoda_wrk-0.4.1/alnoda_wrk/ui_builder.py`

 * *Files identical despite different names*

### Comparing `alnoda_wrk-0.3.9/alnoda_wrk/ui_styles.py` & `alnoda_wrk-0.4.1/alnoda_wrk/ui_styles.py`

 * *Files identical despite different names*

### Comparing `alnoda_wrk-0.3.9/alnoda_wrk/wrk/cheatsheet.json` & `alnoda_wrk-0.4.1/alnoda_wrk/wrk/cheatsheet.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8790178571428571%*

 * *Differences: {"'Alnoda workspace'": "OrderedDict([('bpphdlrf', OrderedDict([('cmd', 'wrk signin [security "*

 * *                       "token]'), ('description', 'Authenticate workspace at alnoda.org')])), "*

 * *                       "('xxphjxxf', OrderedDict([('cmd', 'wrk signout'), ('description', 'Log out "*

 * *                       "workspace from alnoda.org')])), ('asahyfjk', OrderedDict([('cmd', 'wrk "*

 * *                       "install [alnoda.org app id]'), ('description', 'Install application from "*

 * *                       " […]*

```diff
@@ -25,14 +25,52 @@
             "description": "Open glances system processes and resources monitor"
         },
         "wwwibstd": {
             "cmd": "crontab -l",
             "description": "list scheduled tasks"
         }
     },
+    "Alnoda workspace": {
+        "asahyfjk": {
+            "cmd": "wrk install [alnoda.org app id]",
+            "description": "Install application from alnoda.org. Sometimes workspace restart is required!"
+        },
+        "bnlppcwl": {
+            "cmd": "wrk setvar [name] '[value]'",
+            "description": "Set ENV variable tor interactive terminal. Restart terminal session to apply."
+        },
+        "bnphpprl": {
+            "cmd": "wrk alias [name] '[command]'",
+            "description": "Set alias tor interactive terminal. Restart terminal session to apply."
+        },
+        "bpphdlrf": {
+            "cmd": "wrk signin [security token]",
+            "description": "Authenticate workspace at alnoda.org"
+        },
+        "dsuuyggg": {
+            "cmd": "wrk admin",
+            "description": "Launch workspace admin in terminal"
+        },
+        "fdfhygrg": {
+            "cmd": "wrk start [service name] '[service start command]'",
+            "description": "Start application or service as daemon. Workspace restart is required!"
+        },
+        "popnfggg": {
+            "cmd": "wrk stop [service name] ",
+            "description": "Stop service that runs as daemon. Workspace restart is required!"
+        },
+        "vsphygrh": {
+            "cmd": "wrk update [name,description,author,version] 'new value text'",
+            "description": "Change workspace name, description, author or version"
+        },
+        "xxphjxxf": {
+            "cmd": "wrk signout",
+            "description": "Log out workspace from alnoda.org"
+        }
+    },
     "Common": {
         "ckbjjweo": {
             "cmd": "tar -xzf [tar.gz file]",
             "description": "unzip tar.gz archeive file"
         },
         "dofffltf": {
             "cmd": "find . -name [file name]",
@@ -140,30 +178,14 @@
             "cmd": "Ctrl + b d",
             "description": "dettach from tmux session"
         },
         "bxkbmsba": {
             "cmd": "tmux kill-session -a",
             "description": "kill all mux sessions"
         },
-        "dugqmnbq": {
-            "cmd": "pm2 start [application] --name [name] -- [flags]",
-            "description": "start application with flags"
-        },
-        "jkgrmegv": {
-            "cmd": "pm2 monit",
-            "description": "open UI for the running processes"
-        },
-        "lktpjikg": {
-            "cmd": "pm2 stop [application]",
-            "description": "stop application daemonized by pm2 process manager"
-        },
-        "mxjnjuii": {
-            "cmd": "pm2 start [application] --name [name]",
-            "description": "start application and daemonize with pm2 process manager"
-        },
         "pdbtvvph": {
             "cmd": "tmux ls",
             "description": "list tmux sessions"
         },
         "qamevqks": {
             "cmd": "ps axf",
             "description": "list all running processes (in forest)"
@@ -176,18 +198,14 @@
             "cmd": "tmux new -s [session name]",
             "description": "start new tmux session"
         },
         "wcyunsel": {
             "cmd": "tmux kill-session -t [session name]",
             "description": "kill tmux session"
         },
-        "xdqeqjpu": {
-            "cmd": "pm2 ls",
-            "description": "lits processes started with pm2 process manager"
-        },
         "zmlewwmt": {
             "cmd": "tmux a -t [session name]",
             "description": "attach to tmux session [session name]"
         }
     },
     "Node": {
         "hqgnoqoy": {
@@ -211,15 +229,15 @@
         "kqrgdgwm": {
             "cmd": "pip install [package name]",
             "description": "istall python package [package name]"
         }
     },
     "Shortcuts": {
         "hyfxrxqx": {
-            "cmd": "pm2 start python --name http-server --  -m http.server 8030",
+            "cmd": "python -m http.server 8030",
             "description": "launch static web server on port 8030 (My app o 8030)"
         },
         "solbshdg": {
             "cmd": "cd ~p",
             "description": "go to /home/project/"
         }
     },
```

### Comparing `alnoda_wrk-0.3.9/alnoda_wrk/wrk/ui/.gitignore` & `alnoda_wrk-0.4.1/alnoda_wrk/wrk/ui/.gitignore`

 * *Files identical despite different names*

### Comparing `alnoda_wrk-0.3.9/alnoda_wrk/wrk/ui/conf/ui-apps.json` & `alnoda_wrk-0.4.1/alnoda_wrk/wrk/ui/conf/ui-apps.json`

 * *Files identical despite different names*

### Comparing `alnoda_wrk-0.3.9/alnoda_wrk/wrk/ui/docs/assets/Alnoda-logo.svg` & `alnoda_wrk-0.4.1/alnoda_wrk/wrk/ui/docs/assets/Alnoda-logo.svg`

 * *Files identical despite different names*

### Comparing `alnoda_wrk-0.3.9/alnoda_wrk/wrk/ui/docs/assets/favicon.ico` & `alnoda_wrk-0.4.1/alnoda_wrk/wrk/ui/docs/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `alnoda_wrk-0.3.9/alnoda_wrk/wrk/ui/docs/assets/home/Cronicle.jpg` & `alnoda_wrk-0.4.1/alnoda_wrk/wrk/ui/docs/assets/home/Cronicle.jpg`

 * *Files identical despite different names*

### Comparing `alnoda_wrk-0.3.9/alnoda_wrk/wrk/ui/docs/assets/home/Filebrowser.png` & `alnoda_wrk-0.4.1/alnoda_wrk/wrk/ui/docs/assets/home/Filebrowser.png`

 * *Files identical despite different names*

### Comparing `alnoda_wrk-0.3.9/alnoda_wrk/wrk/ui/docs/assets/home/Htop.jpg` & `alnoda_wrk-0.4.1/alnoda_wrk/wrk/ui/docs/assets/home/Htop.jpg`

 * *Files identical despite different names*

### Comparing `alnoda_wrk-0.3.9/alnoda_wrk/wrk/ui/docs/assets/home/MC.jpg` & `alnoda_wrk-0.4.1/alnoda_wrk/wrk/ui/docs/assets/home/MC.jpg`

 * *Files identical despite different names*

### Comparing `alnoda_wrk-0.3.9/alnoda_wrk/wrk/ui/docs/assets/home/Static-server.png` & `alnoda_wrk-0.4.1/alnoda_wrk/wrk/ui/docs/assets/home/Static-server.png`

 * *Files identical despite different names*

### Comparing `alnoda_wrk-0.3.9/alnoda_wrk/wrk/ui/docs/assets/home/Ungit.jpg` & `alnoda_wrk-0.4.1/alnoda_wrk/wrk/ui/docs/assets/home/Ungit.jpg`

 * *Files identical despite different names*

### Comparing `alnoda_wrk-0.3.9/alnoda_wrk/wrk/ui/docs/assets/home/terminal.png` & `alnoda_wrk-0.4.1/alnoda_wrk/wrk/ui/docs/assets/home/terminal.png`

 * *Files identical despite different names*

### Comparing `alnoda_wrk-0.3.9/alnoda_wrk/wrk/ui/docs/assets/laptop-circle-white.svg` & `alnoda_wrk-0.4.1/alnoda_wrk/wrk/ui/docs/assets/laptop-circle-white.svg`

 * *Files identical despite different names*

### Comparing `alnoda_wrk-0.3.9/alnoda_wrk/wrk/ui/docs/assets/laptop-circle.svg` & `alnoda_wrk-0.4.1/alnoda_wrk/wrk/ui/docs/assets/laptop-circle.svg`

 * *Files identical despite different names*

### Comparing `alnoda_wrk-0.3.9/alnoda_wrk/wrk/ui/docs/pages/my_apps/port-8029.png` & `alnoda_wrk-0.4.1/alnoda_wrk/wrk/ui/docs/pages/my_apps/port-8029.png`

 * *Files identical despite different names*

### Comparing `alnoda_wrk-0.3.9/alnoda_wrk/wrk/ui/docs/pages/my_apps/port-8030.png` & `alnoda_wrk-0.4.1/alnoda_wrk/wrk/ui/docs/pages/my_apps/port-8030.png`

 * *Files identical despite different names*

### Comparing `alnoda_wrk-0.3.9/alnoda_wrk/wrk/ui/docs/stylesheets/extra.css` & `alnoda_wrk-0.4.1/alnoda_wrk/wrk/ui/docs/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `alnoda_wrk-0.3.9/alnoda_wrk/wrk/ui/docs/stylesheets/quickstart.css` & `alnoda_wrk-0.4.1/alnoda_wrk/wrk/ui/docs/stylesheets/quickstart.css`

 * *Files identical despite different names*

### Comparing `alnoda_wrk-0.3.9/alnoda_wrk/wrk/ui/macros/helpers.py` & `alnoda_wrk-0.4.1/alnoda_wrk/wrk/ui/macros/helpers.py`

 * *Files identical despite different names*

### Comparing `alnoda_wrk-0.3.9/alnoda_wrk/wrk/ui/mkdocs.yml` & `alnoda_wrk-0.4.1/alnoda_wrk/wrk/ui/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `alnoda_wrk-0.3.9/alnoda_wrk/wrk_supervisor.py` & `alnoda_wrk-0.4.1/alnoda_wrk/wrk_supervisor.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     :param folder: folder in where application should be started
     :type folder: str
     :param env_vars: env var definitions, i.e. ["TERM=xterm", "EDITOR=mc"]
     :type env_vars: list
     """
     init_supervisord() # <- make sure folders exist
     # make sure name is safestring 
-    name = safestring(name)
+    name = safestring(name, length=35)
     params = {"name": name, "cmd": cmd}
     if folder: params["folder"] = folder
     if env_vars: params["env_vars"] = env_vars
     tm = Template(supervisord_template)
     supervisord_file = tm.render(params)
     # write file to the supervisord folder
     supervisor_file = os.path.join(SUPERVISORD_FOLDER, f"{name}.conf")
```

### Comparing `alnoda_wrk-0.3.9/alnoda_wrk/zsh.py` & `alnoda_wrk-0.4.1/alnoda_wrk/zsh.py`

 * *Files identical despite different names*

### Comparing `alnoda_wrk-0.3.9/pyproject.toml` & `alnoda_wrk-0.4.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alnoda_wrk"
-version = "0.3.9"
+version = "0.4.1"
 description = "A tool to build Alnoda workspaces"
 authors = ["bluxmit <bluxmit@gmail.com>"]
 license = "GNU Affero General Public License v3.0"
 readme = "README.md"
 
 [tool.poetry.scripts]
 "alnoda-wrk" = "alnoda_wrk.main:app"
```

### Comparing `alnoda_wrk-0.3.9/setup.py` & `alnoda_wrk-0.4.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 entry_points = \
 {'console_scripts': ['alnoda-wrk = alnoda_wrk.main:app',
                      'wrk = alnoda_wrk.main:app']}
 
 setup_kwargs = {
     'name': 'alnoda-wrk',
-    'version': '0.3.9',
+    'version': '0.4.1',
     'description': 'A tool to build Alnoda workspaces',
     'long_description': '# alnoda-wrk\n\nA tool to build alnoda workspaces\n\n\n',
     'author': 'bluxmit',
     'author_email': 'bluxmit@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `alnoda_wrk-0.3.9/PKG-INFO` & `alnoda_wrk-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alnoda-wrk
-Version: 0.3.9
+Version: 0.4.1
 Summary: A tool to build Alnoda workspaces
 License: AGPL-3.0
 Author: bluxmit
 Author-email: bluxmit@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
```

