# Comparing `tmp/haupt-2.0.0rc7.tar.gz` & `tmp/haupt-2.0.0rc8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haupt-2.0.0rc7.tar", last modified: Wed Apr 12 14:22:06 2023, max compression
+gzip compressed data, was "haupt-2.0.0rc8.tar", last modified: Sun Apr 16 12:03:56 2023, max compression
```

## Comparing `haupt-2.0.0rc7.tar` & `haupt-2.0.0rc8.tar`

### file list

```diff
@@ -1,556 +1,556 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.624264 haupt-2.0.0rc7/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-04-12 14:22:06.624264 haupt-2.0.0rc7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.552262 haupt-2.0.0rc7/haupt/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.556262 haupt-2.0.0rc7/haupt/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/apis/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.556262 haupt-2.0.0rc7/haupt/apis/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/apis/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/apis/endpoints/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/apis/endpoints/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.556262 haupt-2.0.0rc7/haupt/apis/methods/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/apis/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/apis/methods/project_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/apis/methods/run_lineage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/apis/methods/runs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/apis/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.556262 haupt-2.0.0rc7/haupt/apis/project_resources/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/apis/project_resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/apis/project_resources/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/apis/project_resources/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.556262 haupt-2.0.0rc7/haupt/apis/projects/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/apis/projects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/apis/projects/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/apis/projects/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.556262 haupt-2.0.0rc7/haupt/apis/run_lineage/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/apis/run_lineage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/apis/run_lineage/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/apis/run_lineage/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.556262 haupt-2.0.0rc7/haupt/apis/runs/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/apis/runs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/apis/runs/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/apis/runs/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.556262 haupt-2.0.0rc7/haupt/apis/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/apis/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/apis/serializers/artifacts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.560262 haupt-2.0.0rc7/haupt/apis/serializers/base/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/apis/serializers/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/apis/serializers/base/cloning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/apis/serializers/base/is_managed.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/apis/serializers/base/names.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/apis/serializers/base/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/apis/serializers/base/project.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/apis/serializers/base/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/apis/serializers/base/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/apis/serializers/base/uuid_slug_related_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     6483 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/apis/serializers/project_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/apis/serializers/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/apis/serializers/runs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.560262 haupt-2.0.0rc7/haupt/apis/versions/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/apis/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/apis/versions/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/apis/versions/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.560262 haupt-2.0.0rc7/haupt/background/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/background/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.560262 haupt-2.0.0rc7/haupt/background/celeryp/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/background/celeryp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/background/celeryp/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/background/celeryp/polyaxon_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/background/celeryp/queues.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/background/celeryp/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/background/celeryp/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.560262 haupt-2.0.0rc7/haupt/background/queues/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/background/queues/scheduler
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.560262 haupt-2.0.0rc7/haupt/background/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/background/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/background/scheduler/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.560262 haupt-2.0.0rc7/haupt/background/scheduler/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/background/scheduler/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/background/scheduler/tasks/health.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/background/scheduler/tasks/runs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.560262 haupt-2.0.0rc7/haupt/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/cli/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.564262 haupt-2.0.0rc7/haupt/cli/runners/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/cli/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/cli/runners/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/cli/runners/sandbox.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/cli/runners/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/cli/runners/streams.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/cli/runners/viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/cli/sandbox.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/cli/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/cli/streams.py
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/cli/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.564262 haupt-2.0.0rc7/haupt/common/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.564262 haupt-2.0.0rc7/haupt/common/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/apis/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/apis/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/apis/gzip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.564262 haupt-2.0.0rc7/haupt/common/apis/index/
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/apis/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/apis/index/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/apis/index/health.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/apis/index/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/apis/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/apis/regex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.548262 haupt-2.0.0rc7/haupt/common/apis/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.564262 haupt-2.0.0rc7/haupt/common/apis/templates/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/apis/templates/admin/base_site.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.568262 haupt-2.0.0rc7/haupt/common/apis/templates/base/
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/apis/templates/base/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/apis/templates/base/modal_index.html
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/apis/templates/base/wizard_error.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.568262 haupt-2.0.0rc7/haupt/common/apis/templates/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/apis/templates/common/root.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.568262 haupt-2.0.0rc7/haupt/common/apis/urls/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/apis/urls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/apis/urls/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/apis/urls/runs.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/apis/urls/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.568262 haupt-2.0.0rc7/haupt/common/auditor/
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/auditor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/auditor/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/auditor/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.568262 haupt-2.0.0rc7/haupt/common/checks/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/checks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/checks/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/checks/health_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/checks/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.568262 haupt-2.0.0rc7/haupt/common/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/commands/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.568262 haupt-2.0.0rc7/haupt/common/commands/management/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/commands/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.568262 haupt-2.0.0rc7/haupt/common/commands/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/commands/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/commands/management/commands/create_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/commands/management/commands/createuser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/commands/management/commands/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.568262 haupt-2.0.0rc7/haupt/common/conf/
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/conf/conf_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/conf/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/conf/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.568262 haupt-2.0.0rc7/haupt/common/conf/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/conf/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/conf/handlers/env_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/conf/handlers/settings_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/conf/option_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/conf/option_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/conf/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/content_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/crypto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.568262 haupt-2.0.0rc7/haupt/common/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/endpoints/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/endpoints/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/endpoints/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/endpoints/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/endpoints/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/endpoints/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.572263 haupt-2.0.0rc7/haupt/common/events/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/events/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.572263 haupt-2.0.0rc7/haupt/common/events/auditor_subscriptions/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/events/auditor_subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/events/auditor_subscriptions/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     8159 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/events/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/events/event_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/events/event_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/events/event_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/events/event_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/events/event_subjects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.572263 haupt-2.0.0rc7/haupt/common/events/registry/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/events/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/events/registry/attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6525 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/events/registry/run.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/internal_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/json_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/memory_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.572263 haupt-2.0.0rc7/haupt/common/options/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/options/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/options/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.572263 haupt-2.0.0rc7/haupt/common/options/conf_subscriptions/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/options/conf_subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/options/conf_subscriptions/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/options/conf_subscriptions/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/options/conf_subscriptions/installation.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/options/conf_subscriptions/k8s.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/options/conf_subscriptions/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/options/conf_subscriptions/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/options/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/options/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/options/option.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/options/option_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/options/option_namespaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/options/option_owners.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/options/option_subjects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.572263 haupt-2.0.0rc7/haupt/common/options/registry/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/options/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/options/registry/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/options/registry/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/options/registry/installation.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/options/registry/k8s.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/options/registry/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/options/registry/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.576263 haupt-2.0.0rc7/haupt/common/query/
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/query/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/redis_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/service_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.576263 haupt-2.0.0rc7/haupt/common/settings/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/settings/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/settings/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/settings/assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/settings/celery.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/settings/context_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/settings/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/settings/cors.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/settings/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/settings/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/settings/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/settings/middlewares.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/settings/secrets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.576263 haupt-2.0.0rc7/haupt/common/settings/services/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/settings/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/settings/services/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/settings/services/background.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/settings/services/streams.py
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/settings/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.576263 haupt-2.0.0rc7/haupt/common/test_cases/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/test_cases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/test_cases/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.580263 haupt-2.0.0rc7/haupt/common/test_clients/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/test_clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/test_clients/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/user_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.580263 haupt-2.0.0rc7/haupt/common/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/validation/blacklist.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/validation/slugs.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/common/workers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.580263 haupt-2.0.0rc7/haupt/db/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.580263 haupt-2.0.0rc7/haupt/db/abstracts/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/abstracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/abstracts/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/abstracts/catalogs.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/abstracts/color.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/abstracts/describable.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/abstracts/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/abstracts/duration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/abstracts/getter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/abstracts/live_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/abstracts/nameable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/abstracts/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/abstracts/readme.py
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/abstracts/runs.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/abstracts/spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/abstracts/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/abstracts/state.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/abstracts/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/abstracts/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/abstracts/uid.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/abstracts/visibility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.580263 haupt-2.0.0rc7/haupt/db/administration/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/administration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/administration/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/administration/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/administration/register.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/administration/runs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/administration/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.580263 haupt-2.0.0rc7/haupt/db/factories/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/factories/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/factories/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/factories/runs.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/factories/users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.584263 haupt-2.0.0rc7/haupt/db/managers/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/managers/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/managers/deleted.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/managers/dummy_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/managers/runs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/managers/statuses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.584263 haupt-2.0.0rc7/haupt/db/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/mixins/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/mixins/singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/mixins/sub_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/mixins/unique_name.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.584263 haupt-2.0.0rc7/haupt/db/models/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/models/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/models/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/models/runs.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/models/users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.584263 haupt-2.0.0rc7/haupt/db/pgsql/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/pgsql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.584263 haupt-2.0.0rc7/haupt/db/pgsql/db/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/pgsql/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/pgsql/db/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.584263 haupt-2.0.0rc7/haupt/db/pgsql/db/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    20787 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/pgsql/db/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/pgsql/db/migrations/0002_auto_20200807_1247.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/pgsql/db/migrations/0003_run_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/pgsql/db/migrations/0004_auto_20200905_1523.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/pgsql/db/migrations/0005_auto_20201005_0913.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/pgsql/db/migrations/0006_auto_20201020_1705.py
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/pgsql/db/migrations/0007_auto_20201121_1332.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/pgsql/db/migrations/0008_run_wait_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/pgsql/db/migrations/0009_project_unique_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/pgsql/db/migrations/0010_auto_20210429_1539.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/pgsql/db/migrations/0011_alter_artifact_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/pgsql/db/migrations/0012_alter_artifact_updated_at_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/pgsql/db/migrations/0013_alter_artifact_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/pgsql/db/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/pgsql/db/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.588263 haupt-2.0.0rc7/haupt/db/queries/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/queries/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/queries/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/queries/runs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.588263 haupt-2.0.0rc7/haupt/db/query_managers/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/query_managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/query_managers/artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/query_managers/callback_conditions.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/query_managers/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/query_managers/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/query_managers/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.588263 haupt-2.0.0rc7/haupt/db/signals/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/signals/runs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.588263 haupt-2.0.0rc7/haupt/db/sqlite/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/sqlite/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.588263 haupt-2.0.0rc7/haupt/db/sqlite/db/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/sqlite/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/sqlite/db/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.588263 haupt-2.0.0rc7/haupt/db/sqlite/db/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    22205 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/sqlite/db/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/sqlite/db/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/db/sqlite/db/models.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1030 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.588263 haupt-2.0.0rc7/haupt/managers/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/managers/proxies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/managers/sandbox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.588263 haupt-2.0.0rc7/haupt/orchestration/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/orchestration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.588263 haupt-2.0.0rc7/haupt/orchestration/executor/
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/orchestration/executor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.588263 haupt-2.0.0rc7/haupt/orchestration/executor/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/orchestration/executor/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/orchestration/executor/handlers/run.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/orchestration/executor/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/orchestration/executor/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.588263 haupt-2.0.0rc7/haupt/orchestration/executor/subscriptions/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/orchestration/executor/subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/orchestration/executor/subscriptions/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.588263 haupt-2.0.0rc7/haupt/orchestration/operations/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/orchestration/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18171 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/orchestration/operations/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.588263 haupt-2.0.0rc7/haupt/orchestration/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/orchestration/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9211 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/orchestration/scheduler/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/orchestration/scheduler/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/pkg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.592263 haupt-2.0.0rc7/haupt/polyconf/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/polyconf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.592263 haupt-2.0.0rc7/haupt/polyconf/asgi/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/polyconf/asgi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/polyconf/asgi/sandbox.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/polyconf/asgi/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/polyconf/asgi/streams.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/polyconf/asgi/viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/polyconf/config_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.592263 haupt-2.0.0rc7/haupt/polyconf/config_settings/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/polyconf/config_settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/polyconf/config_settings/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/polyconf/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/polyconf/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/polyconf/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.592263 haupt-2.0.0rc7/haupt/proxies/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/proxies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.592263 haupt-2.0.0rc7/haupt/proxies/generators/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/proxies/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/proxies/generators/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/proxies/generators/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/proxies/generators/forward.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/proxies/generators/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/proxies/generators/streams.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.596263 haupt-2.0.0rc7/haupt/proxies/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/proxies/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.596263 haupt-2.0.0rc7/haupt/proxies/schemas/api/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/proxies/schemas/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/proxies/schemas/api/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/proxies/schemas/api/uwsgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/proxies/schemas/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/proxies/schemas/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/proxies/schemas/buffering.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/proxies/schemas/charset.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/proxies/schemas/dns.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/proxies/schemas/error_page.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/proxies/schemas/favicon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/proxies/schemas/forward.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.596263 haupt-2.0.0rc7/haupt/proxies/schemas/gateway/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/proxies/schemas/gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/proxies/schemas/gateway/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/proxies/schemas/gateway/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/proxies/schemas/gateway/healthz.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/proxies/schemas/gateway/redirect.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/proxies/schemas/gzip.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/proxies/schemas/listen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/proxies/schemas/locations.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/proxies/schemas/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/proxies/schemas/robots.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/proxies/schemas/scaffold.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/proxies/schemas/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     7967 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/proxies/schemas/services.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/proxies/schemas/ssl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.596263 haupt-2.0.0rc7/haupt/proxies/schemas/streams/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/proxies/schemas/streams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/proxies/schemas/streams/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/proxies/schemas/streams/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/proxies/schemas/streams/k8s.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/proxies/schemas/timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/proxies/schemas/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.596263 haupt-2.0.0rc7/haupt/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/schemas/proxies_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/schemas/sandbox_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.552262 haupt-2.0.0rc7/haupt/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.552262 haupt-2.0.0rc7/haupt/static/dist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.596263 haupt-2.0.0rc7/haupt/static/dist/css/
--rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/dist/css/global.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/dist/css/global_modal.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.604263 haupt-2.0.0rc7/haupt/static/dist/js/
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/dist/js/0.bundle.js
--rw-r--r--   0 runner    (1001) docker     (123)    25117 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/dist/js/1.bundle.js
--rw-r--r--   0 runner    (1001) docker     (123)   410687 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/dist/js/2.bundle.js
--rw-r--r--   0 runner    (1001) docker     (123)   155336 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/dist/js/3.bundle.js
--rw-r--r--   0 runner    (1001) docker     (123)    57910 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/dist/js/4.bundle.js
--rw-r--r--   0 runner    (1001) docker     (123)   411975 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/dist/js/5.bundle.js
--rw-r--r--   0 runner    (1001) docker     (123)  3963038 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/dist/js/6.bundle.js
--rw-r--r--   0 runner    (1001) docker     (123)  2314169 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/dist/js/7.bundle.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.608263 haupt-2.0.0rc7/haupt/static/errors/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/errors/404.html
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/errors/50x.html
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/errors/permission.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.608263 haupt-2.0.0rc7/haupt/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)    25380 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/images/403.svg
--rw-r--r--   0 runner    (1001) docker     (123)    13004 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/images/404.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15858 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/images/50x.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/images/favicon-danger.ico
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/images/favicon-danger.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/images/favicon-primary.ico
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/images/favicon-primary.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/images/favicon-running.ico
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/images/favicon-running.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/images/favicon-stopped.ico
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/images/favicon-stopped.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/images/favicon-success.ico
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/images/favicon-success.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/images/favicon-warning.ico
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/images/favicon-warning.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/images/favicon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/images/logo_small.png
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/images/logo_white.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.552262 haupt-2.0.0rc7/haupt/static/vendors/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.608263 haupt-2.0.0rc7/haupt/static/vendors/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.608263 haupt-2.0.0rc7/haupt/static/vendors/fonts/dosis/
--rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/vendors/fonts/dosis/OFL.txt
--rw-r--r--   0 runner    (1001) docker     (123)    27069 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/vendors/fonts/dosis/dosis-v8-latin-500.eot
--rw-r--r--   0 runner    (1001) docker     (123)    71085 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/vendors/fonts/dosis/dosis-v8-latin-500.svg
--rw-r--r--   0 runner    (1001) docker     (123)    66980 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/vendors/fonts/dosis/dosis-v8-latin-500.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    32948 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/vendors/fonts/dosis/dosis-v8-latin-500.woff
--rw-r--r--   0 runner    (1001) docker     (123)    26508 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/vendors/fonts/dosis/dosis-v8-latin-500.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/vendors/fonts/fonts.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.612264 haupt-2.0.0rc7/haupt/static/vendors/fonts/source-code-pro/
--rw-r--r--   0 runner    (1001) docker     (123)    15526 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/vendors/fonts/source-code-pro/source-code-pro-v10-latin-regular.eot
--rw-r--r--   0 runner    (1001) docker     (123)    61056 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/vendors/fonts/source-code-pro/source-code-pro-v10-latin-regular.svg
--rw-r--r--   0 runner    (1001) docker     (123)    30816 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/vendors/fonts/source-code-pro/source-code-pro-v10-latin-regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    17252 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/vendors/fonts/source-code-pro/source-code-pro-v10-latin-regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    13436 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/vendors/fonts/source-code-pro/source-code-pro-v10-latin-regular.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.612264 haupt-2.0.0rc7/haupt/static/vendors/fonts/source-sans-pro/
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/vendors/fonts/source-sans-pro/OFL.txt
--rw-r--r--   0 runner    (1001) docker     (123)    77083 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-300.eot
--rw-r--r--   0 runner    (1001) docker     (123)    60850 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-300.svg
--rw-r--r--   0 runner    (1001) docker     (123)   184424 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-300.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    80588 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-300.woff
--rw-r--r--   0 runner    (1001) docker     (123)    62208 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-300.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    77159 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-600.eot
--rw-r--r--   0 runner    (1001) docker     (123)    58839 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-600.svg
--rw-r--r--   0 runner    (1001) docker     (123)   183688 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-600.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    80556 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-600.woff
--rw-r--r--   0 runner    (1001) docker     (123)    62104 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-600.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    77546 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-regular.eot
--rw-r--r--   0 runner    (1001) docker     (123)    60072 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-regular.svg
--rw-r--r--   0 runner    (1001) docker     (123)   184592 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    81008 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    62688 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-regular.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.620264 haupt-2.0.0rc7/haupt/static/vendors/js/
--rw-r--r--   0 runner    (1001) docker     (123)   905027 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/vendors/js/bokeh.3.0.3.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    24977 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/vendors/js/create-plotly-component.2.6.0.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   100277 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/vendors/js/highlight.10.1.2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/vendors/js/moment-timezone.0.5.32.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    58024 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/vendors/js/moment.2.29.3.min.js
--rw-r--r--   0 runner    (1001) docker     (123)  3576301 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/vendors/js/plotly.2.18.2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   131882 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/vendors/js/react-dom.production.18.0.2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    10737 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/vendors/js/react.production.18.0.2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    56197 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/vendors/js/vega-embed@6.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   267407 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/vendors/js/vega-lite@4.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   494375 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/static/vendors/js/vega@5.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.624264 haupt-2.0.0rc7/haupt/streams/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/streams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/streams/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.624264 haupt-2.0.0rc7/haupt/streams/connections/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/streams/connections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/streams/connections/fs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.624264 haupt-2.0.0rc7/haupt/streams/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/streams/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8214 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/streams/controllers/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/streams/controllers/k8s_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/streams/controllers/k8s_crd.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/streams/controllers/k8s_pods.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/streams/controllers/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/streams/controllers/notebooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/streams/controllers/uploads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.624264 haupt-2.0.0rc7/haupt/streams/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/streams/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/streams/endpoints/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/streams/endpoints/auth_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/streams/endpoints/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/streams/endpoints/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/streams/endpoints/k8s.py
--rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/streams/endpoints/local_sandbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/streams/endpoints/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/streams/endpoints/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/streams/endpoints/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/streams/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.624264 haupt-2.0.0rc7/haupt/streams/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/streams/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/streams/tasks/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/haupt/streams/tasks/notification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:06.556262 haupt-2.0.0rc7/haupt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-04-12 14:22:06.000000 haupt-2.0.0rc7/haupt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17638 2023-04-12 14:22:06.000000 haupt-2.0.0rc7/haupt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 14:22:06.000000 haupt-2.0.0rc7/haupt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-12 14:22:06.000000 haupt-2.0.0rc7/haupt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-12 14:22:06.000000 haupt-2.0.0rc7/haupt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 14:22:06.000000 haupt-2.0.0rc7/haupt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-12 14:22:06.624264 haupt-2.0.0rc7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-04-12 14:21:57.000000 haupt-2.0.0rc7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.121009 haupt-2.0.0rc8/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-04-16 12:03:56.121009 haupt-2.0.0rc8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.069009 haupt-2.0.0rc8/haupt/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.069009 haupt-2.0.0rc8/haupt/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/apis/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.069009 haupt-2.0.0rc8/haupt/apis/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/apis/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/apis/endpoints/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/apis/endpoints/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.069009 haupt-2.0.0rc8/haupt/apis/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/apis/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/apis/methods/project_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/apis/methods/run_lineage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/apis/methods/runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/apis/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.069009 haupt-2.0.0rc8/haupt/apis/project_resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/apis/project_resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/apis/project_resources/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/apis/project_resources/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.069009 haupt-2.0.0rc8/haupt/apis/projects/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/apis/projects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/apis/projects/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/apis/projects/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.069009 haupt-2.0.0rc8/haupt/apis/run_lineage/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/apis/run_lineage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/apis/run_lineage/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/apis/run_lineage/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.069009 haupt-2.0.0rc8/haupt/apis/runs/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/apis/runs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/apis/runs/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/apis/runs/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.069009 haupt-2.0.0rc8/haupt/apis/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/apis/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/apis/serializers/artifacts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.073009 haupt-2.0.0rc8/haupt/apis/serializers/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/apis/serializers/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/apis/serializers/base/cloning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/apis/serializers/base/is_managed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/apis/serializers/base/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/apis/serializers/base/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/apis/serializers/base/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/apis/serializers/base/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/apis/serializers/base/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/apis/serializers/base/uuid_slug_related_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6483 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/apis/serializers/project_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/apis/serializers/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/apis/serializers/runs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.073009 haupt-2.0.0rc8/haupt/apis/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/apis/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/apis/versions/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/apis/versions/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.073009 haupt-2.0.0rc8/haupt/background/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/background/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.073009 haupt-2.0.0rc8/haupt/background/celeryp/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/background/celeryp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/background/celeryp/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/background/celeryp/polyaxon_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/background/celeryp/queues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/background/celeryp/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/background/celeryp/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.073009 haupt-2.0.0rc8/haupt/background/queues/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/background/queues/scheduler
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.073009 haupt-2.0.0rc8/haupt/background/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/background/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/background/scheduler/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.073009 haupt-2.0.0rc8/haupt/background/scheduler/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/background/scheduler/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/background/scheduler/tasks/health.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/background/scheduler/tasks/runs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.073009 haupt-2.0.0rc8/haupt/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/cli/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.073009 haupt-2.0.0rc8/haupt/cli/runners/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/cli/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/cli/runners/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/cli/runners/sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/cli/runners/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/cli/runners/streams.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/cli/runners/viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/cli/sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/cli/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/cli/streams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/cli/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.077009 haupt-2.0.0rc8/haupt/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.077009 haupt-2.0.0rc8/haupt/common/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/apis/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/apis/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/apis/gzip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.077009 haupt-2.0.0rc8/haupt/common/apis/index/
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/apis/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/apis/index/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/apis/index/health.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/apis/index/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/apis/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/apis/regex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.061009 haupt-2.0.0rc8/haupt/common/apis/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.077009 haupt-2.0.0rc8/haupt/common/apis/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/apis/templates/admin/base_site.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.077009 haupt-2.0.0rc8/haupt/common/apis/templates/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/apis/templates/base/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/apis/templates/base/modal_index.html
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/apis/templates/base/wizard_error.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.077009 haupt-2.0.0rc8/haupt/common/apis/templates/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/apis/templates/common/root.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.077009 haupt-2.0.0rc8/haupt/common/apis/urls/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/apis/urls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/apis/urls/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/apis/urls/runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/apis/urls/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.077009 haupt-2.0.0rc8/haupt/common/auditor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/auditor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/auditor/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/auditor/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.077009 haupt-2.0.0rc8/haupt/common/checks/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/checks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/checks/health_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/checks/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.077009 haupt-2.0.0rc8/haupt/common/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/commands/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.077009 haupt-2.0.0rc8/haupt/common/commands/management/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/commands/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.077009 haupt-2.0.0rc8/haupt/common/commands/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/commands/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/commands/management/commands/create_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/commands/management/commands/createuser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/commands/management/commands/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.077009 haupt-2.0.0rc8/haupt/common/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/conf/conf_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/conf/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/conf/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.077009 haupt-2.0.0rc8/haupt/common/conf/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/conf/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/conf/handlers/env_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/conf/handlers/settings_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/conf/option_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/conf/option_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/conf/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/content_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/crypto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.081009 haupt-2.0.0rc8/haupt/common/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/endpoints/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/endpoints/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/endpoints/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/endpoints/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/endpoints/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/endpoints/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.081009 haupt-2.0.0rc8/haupt/common/events/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/events/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.081009 haupt-2.0.0rc8/haupt/common/events/auditor_subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/events/auditor_subscriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/events/auditor_subscriptions/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8165 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/events/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/events/event_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/events/event_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/events/event_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/events/event_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/events/event_subjects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.081009 haupt-2.0.0rc8/haupt/common/events/registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/events/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/events/registry/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6525 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/events/registry/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/internal_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/memory_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.081009 haupt-2.0.0rc8/haupt/common/options/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/options/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/options/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.081009 haupt-2.0.0rc8/haupt/common/options/conf_subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/options/conf_subscriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/options/conf_subscriptions/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/options/conf_subscriptions/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/options/conf_subscriptions/installation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/options/conf_subscriptions/k8s.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/options/conf_subscriptions/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/options/conf_subscriptions/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/options/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/options/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/options/option.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/options/option_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/options/option_namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/options/option_owners.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/options/option_subjects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.081009 haupt-2.0.0rc8/haupt/common/options/registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/options/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/options/registry/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/options/registry/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/options/registry/installation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/options/registry/k8s.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/options/registry/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/options/registry/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.081009 haupt-2.0.0rc8/haupt/common/query/
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/query/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/redis_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/service_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.085009 haupt-2.0.0rc8/haupt/common/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/settings/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/settings/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/settings/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/settings/celery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/settings/context_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/settings/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/settings/cors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/settings/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/settings/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/settings/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/settings/middlewares.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/settings/secrets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.085009 haupt-2.0.0rc8/haupt/common/settings/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/settings/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/settings/services/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/settings/services/background.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/settings/services/streams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/settings/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.085009 haupt-2.0.0rc8/haupt/common/test_cases/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/test_cases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/test_cases/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.085009 haupt-2.0.0rc8/haupt/common/test_clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/test_clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/test_clients/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/user_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.085009 haupt-2.0.0rc8/haupt/common/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/validation/blacklist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/validation/slugs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/common/workers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.085009 haupt-2.0.0rc8/haupt/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.085009 haupt-2.0.0rc8/haupt/db/abstracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/abstracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/abstracts/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/abstracts/catalogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/abstracts/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/abstracts/describable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/abstracts/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/abstracts/duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/abstracts/getter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/abstracts/live_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/abstracts/nameable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/abstracts/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/abstracts/readme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/abstracts/runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/abstracts/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/abstracts/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/abstracts/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/abstracts/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/abstracts/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/abstracts/uid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/abstracts/visibility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.089009 haupt-2.0.0rc8/haupt/db/administration/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/administration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/administration/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/administration/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/administration/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/administration/runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/administration/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.089009 haupt-2.0.0rc8/haupt/db/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/factories/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/factories/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/factories/runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/factories/users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.089009 haupt-2.0.0rc8/haupt/db/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/managers/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/managers/deleted.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/managers/dummy_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/managers/runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/managers/statuses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.089009 haupt-2.0.0rc8/haupt/db/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/mixins/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/mixins/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/mixins/sub_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/mixins/unique_name.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.089009 haupt-2.0.0rc8/haupt/db/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/models/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/models/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/models/runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/models/users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.089009 haupt-2.0.0rc8/haupt/db/pgsql/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/pgsql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.089009 haupt-2.0.0rc8/haupt/db/pgsql/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/pgsql/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/pgsql/db/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.089009 haupt-2.0.0rc8/haupt/db/pgsql/db/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    20787 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/pgsql/db/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/pgsql/db/migrations/0002_auto_20200807_1247.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/pgsql/db/migrations/0003_run_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/pgsql/db/migrations/0004_auto_20200905_1523.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/pgsql/db/migrations/0005_auto_20201005_0913.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/pgsql/db/migrations/0006_auto_20201020_1705.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/pgsql/db/migrations/0007_auto_20201121_1332.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/pgsql/db/migrations/0008_run_wait_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/pgsql/db/migrations/0009_project_unique_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/pgsql/db/migrations/0010_auto_20210429_1539.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/pgsql/db/migrations/0011_alter_artifact_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/pgsql/db/migrations/0012_alter_artifact_updated_at_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/pgsql/db/migrations/0013_alter_artifact_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/pgsql/db/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/pgsql/db/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.093009 haupt-2.0.0rc8/haupt/db/queries/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/queries/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/queries/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/queries/runs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.093009 haupt-2.0.0rc8/haupt/db/query_managers/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/query_managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/query_managers/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/query_managers/callback_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/query_managers/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/query_managers/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/query_managers/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.093009 haupt-2.0.0rc8/haupt/db/signals/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/signals/runs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.093009 haupt-2.0.0rc8/haupt/db/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/sqlite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.093009 haupt-2.0.0rc8/haupt/db/sqlite/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/sqlite/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/sqlite/db/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.093009 haupt-2.0.0rc8/haupt/db/sqlite/db/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    22205 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/sqlite/db/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/sqlite/db/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/db/sqlite/db/models.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1030 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.093009 haupt-2.0.0rc8/haupt/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/managers/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/managers/sandbox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.093009 haupt-2.0.0rc8/haupt/orchestration/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/orchestration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.093009 haupt-2.0.0rc8/haupt/orchestration/executor/
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/orchestration/executor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.093009 haupt-2.0.0rc8/haupt/orchestration/executor/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/orchestration/executor/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/orchestration/executor/handlers/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/orchestration/executor/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/orchestration/executor/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.093009 haupt-2.0.0rc8/haupt/orchestration/executor/subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/orchestration/executor/subscriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/orchestration/executor/subscriptions/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.093009 haupt-2.0.0rc8/haupt/orchestration/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/orchestration/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18172 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/orchestration/operations/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.093009 haupt-2.0.0rc8/haupt/orchestration/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/orchestration/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9211 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/orchestration/scheduler/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/orchestration/scheduler/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/pkg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.093009 haupt-2.0.0rc8/haupt/polyconf/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/polyconf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.093009 haupt-2.0.0rc8/haupt/polyconf/asgi/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/polyconf/asgi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/polyconf/asgi/sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/polyconf/asgi/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/polyconf/asgi/streams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/polyconf/asgi/viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/polyconf/config_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.093009 haupt-2.0.0rc8/haupt/polyconf/config_settings/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/polyconf/config_settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/polyconf/config_settings/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/polyconf/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/polyconf/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/polyconf/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.093009 haupt-2.0.0rc8/haupt/proxies/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/proxies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.097009 haupt-2.0.0rc8/haupt/proxies/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/proxies/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/proxies/generators/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/proxies/generators/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/proxies/generators/forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/proxies/generators/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/proxies/generators/streams.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.097009 haupt-2.0.0rc8/haupt/proxies/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/proxies/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.097009 haupt-2.0.0rc8/haupt/proxies/schemas/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/proxies/schemas/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/proxies/schemas/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/proxies/schemas/api/uwsgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/proxies/schemas/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/proxies/schemas/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/proxies/schemas/buffering.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/proxies/schemas/charset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/proxies/schemas/dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/proxies/schemas/error_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/proxies/schemas/favicon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/proxies/schemas/forward.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.097009 haupt-2.0.0rc8/haupt/proxies/schemas/gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/proxies/schemas/gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/proxies/schemas/gateway/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/proxies/schemas/gateway/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/proxies/schemas/gateway/healthz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/proxies/schemas/gateway/redirect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/proxies/schemas/gzip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/proxies/schemas/listen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/proxies/schemas/locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/proxies/schemas/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/proxies/schemas/robots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/proxies/schemas/scaffold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/proxies/schemas/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7967 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/proxies/schemas/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/proxies/schemas/ssl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.097009 haupt-2.0.0rc8/haupt/proxies/schemas/streams/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/proxies/schemas/streams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/proxies/schemas/streams/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/proxies/schemas/streams/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/proxies/schemas/streams/k8s.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/proxies/schemas/timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/proxies/schemas/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.097009 haupt-2.0.0rc8/haupt/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/schemas/proxies_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/schemas/sandbox_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.065009 haupt-2.0.0rc8/haupt/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.065009 haupt-2.0.0rc8/haupt/static/dist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.097009 haupt-2.0.0rc8/haupt/static/dist/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/dist/css/global.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/dist/css/global_modal.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.105009 haupt-2.0.0rc8/haupt/static/dist/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/dist/js/0.bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123)    25117 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/dist/js/1.bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123)   410687 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/dist/js/2.bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123)   155336 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/dist/js/3.bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123)    57910 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/dist/js/4.bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123)   411975 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/dist/js/5.bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123)  3963038 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/dist/js/6.bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123)  2314169 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/dist/js/7.bundle.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.105009 haupt-2.0.0rc8/haupt/static/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/errors/404.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/errors/50x.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/errors/permission.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.109009 haupt-2.0.0rc8/haupt/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    25380 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/images/403.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    13004 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/images/404.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15858 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/images/50x.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/images/favicon-danger.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/images/favicon-danger.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/images/favicon-primary.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/images/favicon-primary.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/images/favicon-running.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/images/favicon-running.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/images/favicon-stopped.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/images/favicon-stopped.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/images/favicon-success.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/images/favicon-success.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/images/favicon-warning.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/images/favicon-warning.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/images/favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/images/logo_small.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/images/logo_white.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.065009 haupt-2.0.0rc8/haupt/static/vendors/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.109009 haupt-2.0.0rc8/haupt/static/vendors/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.109009 haupt-2.0.0rc8/haupt/static/vendors/fonts/dosis/
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/vendors/fonts/dosis/OFL.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    27069 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/vendors/fonts/dosis/dosis-v8-latin-500.eot
+-rw-r--r--   0 runner    (1001) docker     (123)    71085 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/vendors/fonts/dosis/dosis-v8-latin-500.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    66980 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/vendors/fonts/dosis/dosis-v8-latin-500.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    32948 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/vendors/fonts/dosis/dosis-v8-latin-500.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    26508 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/vendors/fonts/dosis/dosis-v8-latin-500.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/vendors/fonts/fonts.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.109009 haupt-2.0.0rc8/haupt/static/vendors/fonts/source-code-pro/
+-rw-r--r--   0 runner    (1001) docker     (123)    15526 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/vendors/fonts/source-code-pro/source-code-pro-v10-latin-regular.eot
+-rw-r--r--   0 runner    (1001) docker     (123)    61056 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/vendors/fonts/source-code-pro/source-code-pro-v10-latin-regular.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    30816 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/vendors/fonts/source-code-pro/source-code-pro-v10-latin-regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    17252 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/vendors/fonts/source-code-pro/source-code-pro-v10-latin-regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    13436 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/vendors/fonts/source-code-pro/source-code-pro-v10-latin-regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.113009 haupt-2.0.0rc8/haupt/static/vendors/fonts/source-sans-pro/
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/vendors/fonts/source-sans-pro/OFL.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    77083 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-300.eot
+-rw-r--r--   0 runner    (1001) docker     (123)    60850 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-300.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   184424 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-300.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    80588 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-300.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    62208 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-300.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    77159 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-600.eot
+-rw-r--r--   0 runner    (1001) docker     (123)    58839 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-600.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   183688 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-600.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    80556 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-600.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    62104 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-600.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    77546 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-regular.eot
+-rw-r--r--   0 runner    (1001) docker     (123)    60072 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-regular.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   184592 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    81008 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    62688 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.117009 haupt-2.0.0rc8/haupt/static/vendors/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   905027 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/vendors/js/bokeh.3.0.3.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    24977 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/vendors/js/create-plotly-component.2.6.0.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   100277 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/vendors/js/highlight.10.1.2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/vendors/js/moment-timezone.0.5.32.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    58024 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/vendors/js/moment.2.29.3.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)  3576301 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/vendors/js/plotly.2.18.2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   131882 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/vendors/js/react-dom.production.18.0.2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10737 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/vendors/js/react.production.18.0.2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    56197 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/vendors/js/vega-embed@6.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   267407 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/vendors/js/vega-lite@4.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   494375 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/static/vendors/js/vega@5.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.117009 haupt-2.0.0rc8/haupt/streams/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/streams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/streams/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.117009 haupt-2.0.0rc8/haupt/streams/connections/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/streams/connections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/streams/connections/fs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.121009 haupt-2.0.0rc8/haupt/streams/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/streams/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/streams/controllers/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/streams/controllers/k8s_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/streams/controllers/k8s_crd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/streams/controllers/k8s_pods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/streams/controllers/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/streams/controllers/notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/streams/controllers/uploads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.121009 haupt-2.0.0rc8/haupt/streams/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/streams/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8576 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/streams/endpoints/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/streams/endpoints/auth_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/streams/endpoints/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6820 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/streams/endpoints/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/streams/endpoints/k8s.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/streams/endpoints/local_sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/streams/endpoints/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/streams/endpoints/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/streams/endpoints/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/streams/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.121009 haupt-2.0.0rc8/haupt/streams/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/streams/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/streams/tasks/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/haupt/streams/tasks/notification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:56.069009 haupt-2.0.0rc8/haupt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-04-16 12:03:55.000000 haupt-2.0.0rc8/haupt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17638 2023-04-16 12:03:56.000000 haupt-2.0.0rc8/haupt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 12:03:55.000000 haupt-2.0.0rc8/haupt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-16 12:03:55.000000 haupt-2.0.0rc8/haupt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-16 12:03:55.000000 haupt-2.0.0rc8/haupt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-16 12:03:55.000000 haupt-2.0.0rc8/haupt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-16 12:03:56.121009 haupt-2.0.0rc8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-04-16 12:03:48.000000 haupt-2.0.0rc8/setup.py
```

### Comparing `haupt-2.0.0rc7/PKG-INFO` & `haupt-2.0.0rc8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haupt
-Version: 2.0.0rc7
+Version: 2.0.0rc8
 Summary: Lineage metadata API, artifacts streams, sandbox, ML-API, and spaces for Polyaxon.
 Home-page: https://github.com/polyaxon/haupt
 Author: Polyaxon, Inc.
 Author-email: contact@polyaxon.com
 Maintainer: Polyaxon, Inc.
 Maintainer-email: contact@polyaxon.com
 License: AGPLv3
```

### Comparing `haupt-2.0.0rc7/haupt/apis/apps.py` & `haupt-2.0.0rc8/haupt/apis/apps.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/apis/endpoints/project.py` & `haupt-2.0.0rc8/haupt/apis/endpoints/project.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/apis/endpoints/run.py` & `haupt-2.0.0rc8/haupt/apis/endpoints/run.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/apis/methods/project_resources.py` & `haupt-2.0.0rc8/haupt/apis/methods/project_resources.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/apis/methods/run_lineage.py` & `haupt-2.0.0rc8/haupt/apis/methods/run_lineage.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/python
 #
 # Copyright 2018-2023 Polyaxon, Inc.
 # This file and its contents are licensed under the AGPLv3 License.
 # Please see the included NOTICE for copyright information and
 # LICENSE-AGPL for a copy of the license.
 
-from clipped.list_utils import to_list
+from clipped.utils.lists import to_list
 from pydantic import ValidationError as PydanticValidationError
 from rest_framework import status
 from rest_framework.exceptions import ValidationError
 from rest_framework.response import Response
 
 from traceml.artifacts import V1RunArtifact
```

### Comparing `haupt-2.0.0rc7/haupt/apis/methods/runs.py` & `haupt-2.0.0rc8/haupt/apis/methods/runs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/python
 #
 # Copyright 2018-2023 Polyaxon, Inc.
 # This file and its contents are licensed under the AGPLv3 License.
 # Please see the included NOTICE for copyright information and
 # LICENSE-AGPL for a copy of the license.
-import orjson
 
+from clipped.utils.json import orjson_loads
 from pydantic import ValidationError as PydanticValidationError
 from rest_framework import status
 from rest_framework.exceptions import ValidationError
 from rest_framework.response import Response
 
 from haupt.db.managers.runs import base_approve_run
 from haupt.db.managers.statuses import new_run_status, new_run_stopping_status
@@ -21,15 +21,15 @@
     view.run = view.get_object()
     run = view.pre_validate(view.run)
     content = None
     if "content" in request.data:
         content = request.data["content"]
     if content and not isinstance(content, dict):
         try:
-            content = orjson.loads(content)
+            content = orjson_loads(content)
         except Exception as e:
             raise ValidationError("Cloning was not successful, error: {}".format(e))
     try:
         new_obj = view.clone(
             obj=run,
             content=content,
             name=request.data.get("name"),
```

### Comparing `haupt-2.0.0rc7/haupt/apis/patterns.py` & `haupt-2.0.0rc8/haupt/apis/patterns.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/apis/project_resources/urls.py` & `haupt-2.0.0rc8/haupt/apis/project_resources/urls.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/apis/project_resources/views.py` & `haupt-2.0.0rc8/haupt/apis/project_resources/views.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/apis/projects/urls.py` & `haupt-2.0.0rc8/haupt/apis/projects/urls.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/apis/projects/views.py` & `haupt-2.0.0rc8/haupt/apis/projects/views.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/apis/run_lineage/urls.py` & `haupt-2.0.0rc8/haupt/apis/run_lineage/urls.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/apis/run_lineage/views.py` & `haupt-2.0.0rc8/haupt/apis/run_lineage/views.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/apis/runs/urls.py` & `haupt-2.0.0rc8/haupt/apis/runs/urls.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/apis/runs/views.py` & `haupt-2.0.0rc8/haupt/apis/runs/views.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/apis/serializers/artifacts.py` & `haupt-2.0.0rc8/haupt/apis/serializers/artifacts.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/apis/serializers/base/cloning.py` & `haupt-2.0.0rc8/haupt/apis/serializers/base/cloning.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/apis/serializers/base/is_managed.py` & `haupt-2.0.0rc8/haupt/apis/serializers/base/is_managed.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/apis/serializers/base/names.py` & `haupt-2.0.0rc8/haupt/apis/serializers/base/names.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/apis/serializers/base/pipeline.py` & `haupt-2.0.0rc8/haupt/apis/serializers/base/pipeline.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/apis/serializers/base/settings.py` & `haupt-2.0.0rc8/haupt/apis/serializers/base/settings.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/apis/serializers/base/tags.py` & `haupt-2.0.0rc8/haupt/apis/serializers/base/tags.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # This file and its contents are licensed under the AGPLv3 License.
 # Please see the included NOTICE for copyright information and
 # LICENSE-AGPL for a copy of the license.
 
 from collections.abc import Mapping
 from typing import Dict, List, Optional
 
-from clipped.list_utils import to_list
+from clipped.utils.lists import to_list
 
 from django.conf import settings
 
 
 class TagsMixin:
     def to_representation(self, instance):
         representation = super().to_representation(instance)
```

### Comparing `haupt-2.0.0rc7/haupt/apis/serializers/project_resources.py` & `haupt-2.0.0rc8/haupt/apis/serializers/project_resources.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/apis/serializers/projects.py` & `haupt-2.0.0rc8/haupt/apis/serializers/projects.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/apis/serializers/runs.py` & `haupt-2.0.0rc8/haupt/apis/serializers/runs.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/apis/versions/urls.py` & `haupt-2.0.0rc8/haupt/apis/versions/urls.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/apis/versions/views.py` & `haupt-2.0.0rc8/haupt/apis/versions/views.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/background/celeryp/polyaxon_task.py` & `haupt-2.0.0rc8/haupt/background/celeryp/polyaxon_task.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/background/celeryp/queues.py` & `haupt-2.0.0rc8/haupt/background/celeryp/queues.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/background/celeryp/routes.py` & `haupt-2.0.0rc8/haupt/background/celeryp/routes.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/background/celeryp/tasks.py` & `haupt-2.0.0rc8/haupt/background/celeryp/tasks.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/background/scheduler/apps.py` & `haupt-2.0.0rc8/haupt/background/scheduler/apps.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/background/scheduler/tasks/health.py` & `haupt-2.0.0rc8/haupt/background/scheduler/tasks/health.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/background/scheduler/tasks/runs.py` & `haupt-2.0.0rc8/haupt/background/scheduler/tasks/runs.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/cli/proxies.py` & `haupt-2.0.0rc8/haupt/cli/proxies.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/cli/runners/base.py` & `haupt-2.0.0rc8/haupt/cli/runners/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Please see the included NOTICE for copyright information and
 # LICENSE-AGPL for a copy of the license.
 import logging
 import os
 
 from typing import Optional
 
-from clipped.workers_utils import get_core_workers
+from clipped.utils.workers import get_core_workers
 
 import uvicorn
 
 from polyaxon.env_vars.keys import EV_KEYS_PROXY_LOCAL_PORT
 
 _logger = logging.getLogger("haupt.cli")
```

### Comparing `haupt-2.0.0rc7/haupt/cli/runners/sandbox.py` & `haupt-2.0.0rc8/haupt/cli/runners/sandbox.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/cli/runners/server.py` & `haupt-2.0.0rc8/haupt/cli/runners/server.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/cli/runners/streams.py` & `haupt-2.0.0rc8/haupt/cli/runners/streams.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/cli/runners/viewer.py` & `haupt-2.0.0rc8/haupt/cli/runners/viewer.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/cli/sandbox.py` & `haupt-2.0.0rc8/haupt/cli/sandbox.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/cli/server.py` & `haupt-2.0.0rc8/haupt/cli/server.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/cli/streams.py` & `haupt-2.0.0rc8/haupt/cli/streams.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/cli/viewer.py` & `haupt-2.0.0rc8/haupt/cli/viewer.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/common/apis/filters.py` & `haupt-2.0.0rc8/haupt/common/apis/filters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/python
 #
 # Copyright 2018-2023 Polyaxon, Inc.
 # This file and its contents are licensed under the AGPLv3 License.
 # Please see the included NOTICE for copyright information and
 # LICENSE-AGPL for a copy of the license.
-from clipped.string_utils import strip_spaces
+from clipped.utils.strings import strip_spaces
 from rest_framework.exceptions import ValidationError
 from rest_framework.filters import BaseFilterBackend
 from rest_framework.filters import OrderingFilter as BaseOrderingFilter
 
 from django.core.exceptions import ImproperlyConfigured
 from django.db.models import F
 from django.db.models.fields.json import KeyTransform
```

### Comparing `haupt-2.0.0rc7/haupt/common/apis/gzip.py` & `haupt-2.0.0rc8/haupt/common/apis/gzip.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/common/apis/index/__init__.py` & `haupt-2.0.0rc8/haupt/common/apis/index/__init__.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/common/apis/index/errors.py` & `haupt-2.0.0rc8/haupt/common/apis/index/errors.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/common/apis/index/health.py` & `haupt-2.0.0rc8/haupt/common/apis/index/health.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/python
 #
 # Copyright 2018-2023 Polyaxon, Inc.
 # This file and its contents are licensed under the AGPLv3 License.
 # Please see the included NOTICE for copyright information and
 # LICENSE-AGPL for a copy of the license.
 
-from clipped.tz_utils import now
+from clipped.utils.tz import now
 from rest_framework import status
 from rest_framework.response import Response
 from rest_framework.views import APIView
 
 from haupt import pkg
 from haupt.common import conf
 from haupt.common.options.registry.installation import ORGANIZATION_KEY
```

### Comparing `haupt-2.0.0rc7/haupt/common/apis/paginator.py` & `haupt-2.0.0rc8/haupt/common/apis/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/python
 #
 # Copyright 2018-2023 Polyaxon, Inc.
 # This file and its contents are licensed under the AGPLv3 License.
 # Please see the included NOTICE for copyright information and
 # LICENSE-AGPL for a copy of the license.
 
-from clipped.bool_utils import to_bool
+from clipped.utils.bools import to_bool
 from rest_framework.pagination import LimitOffsetPagination
 
 
 class PolyaxonBasePagination(LimitOffsetPagination):
     no_page_query_param = "no_page"
 
     def get_no_page(self, request):
```

### Comparing `haupt-2.0.0rc7/haupt/common/apis/regex.py` & `haupt-2.0.0rc8/haupt/common/apis/regex.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/common/apis/templates/admin/base_site.html` & `haupt-2.0.0rc8/haupt/common/apis/templates/admin/base_site.html`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/common/apis/templates/base/index.html` & `haupt-2.0.0rc8/haupt/common/apis/templates/base/index.html`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/common/apis/templates/base/modal_index.html` & `haupt-2.0.0rc8/haupt/common/apis/templates/base/modal_index.html`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/common/apis/templates/common/root.html` & `haupt-2.0.0rc8/haupt/common/apis/templates/common/root.html`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/common/apis/urls/projects.py` & `haupt-2.0.0rc8/haupt/common/apis/urls/projects.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/common/apis/urls/runs.py` & `haupt-2.0.0rc8/haupt/common/apis/urls/runs.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/common/apis/urls/versions.py` & `haupt-2.0.0rc8/haupt/common/apis/urls/versions.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/common/auditor/__init__.py` & `haupt-2.0.0rc8/haupt/common/auditor/__init__.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/common/auditor/service.py` & `haupt-2.0.0rc8/haupt/common/auditor/service.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # Copyright 2018-2023 Polyaxon, Inc.
 # This file and its contents are licensed under the AGPLv3 License.
 # Please see the included NOTICE for copyright information and
 # LICENSE-AGPL for a copy of the license.
 import copy
 
-from clipped.imports import import_string
+from clipped.utils.imports import import_string
 
 from haupt.common.auditor.manager import event_manager
 from haupt.common.events.event import Event
 from haupt.common.events.event_service import EventService
 
 
 class AuditorService(EventService):
```

### Comparing `haupt-2.0.0rc7/haupt/common/checks/results.py` & `haupt-2.0.0rc8/haupt/common/checks/results.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/common/commands/management/commands/create_exchange.py` & `haupt-2.0.0rc8/haupt/common/commands/management/commands/create_exchange.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/common/commands/management/commands/createuser.py` & `haupt-2.0.0rc8/haupt/common/commands/management/commands/createuser.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Please see the included NOTICE for copyright information and
 # LICENSE-AGPL for a copy of the license.
 
 import logging
 
 from typing import Dict
 
-from clipped.bool_utils import to_bool
+from clipped.utils.bools import to_bool
 
 from django.contrib.auth import get_user_model
 from django.contrib.auth.password_validation import validate_password
 from django.core import exceptions
 from django.core.exceptions import ValidationError
 from django.core.management.base import BaseCommand, CommandError
```

### Comparing `haupt-2.0.0rc7/haupt/common/commands/management/commands/tables.py` & `haupt-2.0.0rc8/haupt/common/commands/management/commands/tables.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/common/conf/__init__.py` & `haupt-2.0.0rc8/haupt/common/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/common/conf/handler.py` & `haupt-2.0.0rc8/haupt/common/conf/handler.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/common/conf/handlers/env_handler.py` & `haupt-2.0.0rc8/haupt/common/conf/handlers/env_handler.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/common/conf/handlers/settings_handler.py` & `haupt-2.0.0rc8/haupt/common/conf/handlers/settings_handler.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/common/conf/option_service.py` & `haupt-2.0.0rc8/haupt/common/conf/option_service.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/common/conf/service.py` & `haupt-2.0.0rc8/haupt/common/conf/service.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/common/config_manager.py` & `haupt-2.0.0rc8/haupt/common/config_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,70 +7,82 @@
 
 import os
 
 from pathlib import Path
 from typing import List
 
 from haupt import pkg
-from polyaxon.config_reader.manager import ConfigManager as BaseConfigManager
+from polyaxon.config.manager import ConfigManager as BaseConfigManager
 from polyaxon.env_vars.keys import (
     EV_KEYS_DEBUG,
     EV_KEYS_ENVIRONMENT,
     EV_KEYS_LOG_LEVEL,
     EV_KEYS_PLATFORM_CONFIG,
     EV_KEYS_SERVICE,
     EV_KEYS_TIME_ZONE,
 )
 from polyaxon.k8s.namespace import DEFAULT_NAMESPACE
 
 
 class ConfigManager(BaseConfigManager):
     def __init__(self, **params):
         super().__init__(**params)
-        self._env = self.get_string(
-            EV_KEYS_ENVIRONMENT, is_optional=True, default="local"
+        self._env = self.get(
+            EV_KEYS_ENVIRONMENT, "str", is_optional=True, default="local"
         )
-        self._config_module = self.get_string(
-            "POLYAXON_CONFIG_MODULE", is_optional=True, default="polyconf"
+        self._config_module = self.get(
+            "POLYAXON_CONFIG_MODULE", "str", is_optional=True, default="polyconf"
         )
         self._root_dir = self.get_value("POLYAXON_CONFIG_ROOT_DIR")
-        self._service = self.get_string(
-            EV_KEYS_SERVICE, is_local=True, is_optional=True
+        self._service = self.get(
+            EV_KEYS_SERVICE, "str", is_local=True, is_optional=True
         )
-        self._is_debug_mode = self.get_boolean(
-            EV_KEYS_DEBUG, is_optional=True, default=False
+        self._is_debug_mode = self.get(
+            EV_KEYS_DEBUG, "bool", is_optional=True, default=False
         )
-        self._db_engine_name = self.get_string(
-            "POLYAXON_DB_ENGINE", default="sqlite", is_optional=True
+        self._db_engine_name = self.get(
+            "POLYAXON_DB_ENGINE", "str", default="sqlite", is_optional=True
         )
-        self._namespace = self.get_string(
-            "POLYAXON_K8S_NAMESPACE", is_optional=True, default=DEFAULT_NAMESPACE
+        self._namespace = self.get(
+            "POLYAXON_K8S_NAMESPACE",
+            "str",
+            is_optional=True,
+            default=DEFAULT_NAMESPACE,
         )
-        self._log_level = self.get_string(
-            EV_KEYS_LOG_LEVEL, is_local=True, is_optional=True, default="WARNING"
+        self._log_level = self.get(
+            EV_KEYS_LOG_LEVEL,
+            "str",
+            is_local=True,
+            is_optional=True,
+            default="WARNING",
         ).upper()
-        self._timezone = self.get_string(
-            EV_KEYS_TIME_ZONE, is_optional=True, default="UTC"
+        self._timezone = self.get(
+            EV_KEYS_TIME_ZONE, "str", is_optional=True, default="UTC"
         )
-        self._scheduler_enabled = self.get_boolean(
-            "POLYAXON_SCHEDULER_ENABLED", is_optional=True, default=False
+        self._scheduler_enabled = self.get(
+            "POLYAXON_SCHEDULER_ENABLED", "bool", is_optional=True, default=False
         )
-        self._chart_version = self.get_string(
-            "POLYAXON_CHART_VERSION", is_optional=True, default=pkg.VERSION
+        self._chart_version = self.get(
+            "POLYAXON_CHART_VERSION", "str", is_optional=True, default=pkg.VERSION
         )
-        self._redis_protocol = self.get_string(
-            "POLYAXON_REDIS_PROTOCOL", is_optional=True, default="redis"
+        self._redis_protocol = self.get(
+            "POLYAXON_REDIS_PROTOCOL", "str", is_optional=True, default="redis"
         )
-        self._broker_backend = self.get_string(
+        self._broker_backend = self.get(
             "POLYAXON_BROKER_BACKEND",
+            "str",
             is_optional=True,
             options=["redis", "rabbitmq"],
         )
-        self._redis_password = self.get_string(
-            "POLYAXON_REDIS_PASSWORD", is_optional=True, is_secret=True, is_local=True
+        self._redis_password = self.get(
+            "POLYAXON_REDIS_PASSWORD",
+            "str",
+            is_optional=True,
+            is_secret=True,
+            is_local=True,
         )
 
     @property
     def namespace(self) -> str:
         return self._namespace
 
     @property
@@ -176,24 +188,25 @@
         return self.broker_backend == "redis"
 
     @property
     def is_rabbitmq_broker(self):
         return self.broker_backend == "rabbitmq"
 
     def get_redis_url(self, env_url_name) -> str:
-        redis_url = self.get_string(env_url_name)
+        redis_url = self.get(env_url_name, "str")
         if self._redis_password:
             redis_url = ":{}@{}".format(self._redis_password, redis_url)
         return "{}://{}".format(self._redis_protocol, redis_url)
 
     def _get_rabbitmq_broker_url(self) -> str:
-        amqp_url = self.get_string("POLYAXON_AMQP_URL")
-        rabbitmq_user = self.get_string("POLYAXON_RABBITMQ_USER", is_optional=True)
-        rabbitmq_password = self.get_string(
+        amqp_url = self.get("POLYAXON_AMQP_URL", "str")
+        rabbitmq_user = self.get("POLYAXON_RABBITMQ_USER", "str", is_optional=True)
+        rabbitmq_password = self.get(
             "POLYAXON_RABBITMQ_PASSWORD",
+            "str",
             is_secret=True,
             is_local=True,
             is_optional=True,
         )
         if rabbitmq_user and rabbitmq_password:
             return "amqp://{user}:{password}@{url}".format(
                 user=rabbitmq_user, password=rabbitmq_password, url=amqp_url
```

### Comparing `haupt-2.0.0rc7/haupt/common/endpoints/base.py` & `haupt-2.0.0rc8/haupt/common/endpoints/base.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/common/endpoints/files.py` & `haupt-2.0.0rc8/haupt/common/endpoints/files.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # LICENSE-AGPL for a copy of the license.
 
 import os
 
 from email.utils import formatdate
 from typing import Dict, Optional
 
-from clipped.hashing import hash_value
+from clipped.utils.hashing import hash_value
 
 from django.http import FileResponse
 
 
 class FilePathResponse(FileResponse):
     def __init__(self, *args, as_attachment=False, filepath="", **kwargs):
         filename = os.path.basename(filepath) if filepath else ""
```

### Comparing `haupt-2.0.0rc7/haupt/common/endpoints/mixins.py` & `haupt-2.0.0rc8/haupt/common/endpoints/mixins.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/common/endpoints/validation.py` & `haupt-2.0.0rc8/haupt/common/endpoints/validation.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/common/events/auditor_subscriptions/run.py` & `haupt-2.0.0rc8/haupt/common/events/auditor_subscriptions/run.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/common/events/event.py` & `haupt-2.0.0rc8/haupt/common/events/event.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 #
 # Copyright 2018-2023 Polyaxon, Inc.
 # This file and its contents are licensed under the AGPLv3 License.
 # Please see the included NOTICE for copyright information and
 # LICENSE-AGPL for a copy of the license.
 
 import copy
+import datetime as _datetime
 
 from typing import Any, Dict, Iterable, Mapping, Optional, Union
 from uuid import UUID, uuid1
 
-from clipped.date_utils import to_datetime, to_timestamp
+from clipped.utils.dates import to_datetime, to_timestamp
 
 from django.db.models import Model
 from django.utils import timezone
 
 from haupt.common import user_system
 from haupt.common.events import event_context
 from haupt.common.json_utils import dumps_htmlsafe
-from polyaxon.types import AwareDT
 
 
 class Attribute:
     def __init__(
         self,
         name: str,
         attr_type: Any = str,
@@ -78,15 +78,15 @@
                 Attribute(cls.actor_name, is_required=False),
             )
         return attributes
 
     def __init__(
         self,
         uid: Optional[str] = None,
-        datetime: AwareDT = None,
+        datetime: _datetime.datetime = None,
         instance: Any = None,
         instance_id: Optional[int] = None,
         instance_uuid: Optional[str] = None,
         ref_id: Optional[str] = None,
         event_data: Mapping = None,
         **items
     ):
```

### Comparing `haupt-2.0.0rc7/haupt/common/events/event_actions.py` & `haupt-2.0.0rc8/haupt/common/events/event_actions.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/common/events/event_context.py` & `haupt-2.0.0rc8/haupt/common/events/event_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # This file and its contents are licensed under the AGPLv3 License.
 # Please see the included NOTICE for copyright information and
 # LICENSE-AGPL for a copy of the license.
 
 from collections import namedtuple
 from typing import Any, Optional
 
-from clipped.http_utils import absolute_uri
+from clipped.utils.http import absolute_uri
 
 from haupt.common import user_system
 from haupt.common.events import event_subjects
 from polyaxon.utils.urls_utils import get_fqn_run_url, get_owner_url, get_project_url
 
 
 class EventItemContextSpec(namedtuple("EventItemContextSpec", "name url object_id")):
```

### Comparing `haupt-2.0.0rc7/haupt/common/events/event_manager.py` & `haupt-2.0.0rc8/haupt/common/events/event_manager.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/common/events/event_service.py` & `haupt-2.0.0rc8/haupt/common/events/event_service.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/common/events/registry/attributes.py` & `haupt-2.0.0rc8/haupt/common/events/registry/attributes.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/common/events/registry/run.py` & `haupt-2.0.0rc8/haupt/common/events/registry/run.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/common/hashing.py` & `haupt-2.0.0rc8/haupt/common/hashing.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/common/headers.py` & `haupt-2.0.0rc8/haupt/common/headers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/python
 #
 # Copyright 2018-2023 Polyaxon, Inc.
 # This file and its contents are licensed under the AGPLv3 License.
 # Please see the included NOTICE for copyright information and
 # LICENSE-AGPL for a copy of the license.
 
-from clipped.enums_utils import get_enum_value
+from clipped.utils.enums import get_enum_value
 
 from django.http import HttpRequest
 
 from polyaxon.services.headers import PolyaxonServiceHeaders
 
 try:
     from rest_framework import HTTP_HEADER_ENCODING
```

### Comparing `haupt-2.0.0rc7/haupt/common/internal_auth.py` & `haupt-2.0.0rc8/haupt/common/internal_auth.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/common/json_utils.py` & `haupt-2.0.0rc8/haupt/common/json_utils.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/common/memory_manager.py` & `haupt-2.0.0rc8/haupt/common/memory_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #!/usr/bin/python
 #
 # Copyright 2018-2023 Polyaxon, Inc.
 # This file and its contents are licensed under the AGPLv3 License.
 # Please see the included NOTICE for copyright information and
 # LICENSE-AGPL for a copy of the license.
+import datetime
 
 from collections import namedtuple
 from datetime import timedelta
 from typing import Any, Optional
 
 from django.utils import timezone
 
 from haupt.common.options.option_owners import OptionOwners
-from polyaxon.types import AwareDT
 
 
 class CachedOptionSpec(namedtuple("CachedOptionSpec", "value datetime")):
     pass
 
 
 class MemoryCacheManager:
@@ -34,15 +34,15 @@
         self._state = {}
 
     @classmethod
     def is_valid_value(cls, value: Any):
         return value != cls.INVALIDED_OPTION
 
     @staticmethod
-    def is_valid_cache(value_datetime: AwareDT) -> bool:
+    def is_valid_cache(value_datetime: datetime.datetime) -> bool:
         return timezone.now() < value_datetime
 
     def get_from_cache(self, key: str, owners: Optional[OptionOwners] = None) -> Any:
         if owners:
             key = f"{key}:{owners}"
         cached_option = self._state.get(key)
         if cached_option and self.is_valid_cache(cached_option.datetime):
```

### Comparing `haupt-2.0.0rc7/haupt/common/options/conf_subscriptions/core.py` & `haupt-2.0.0rc8/haupt/common/options/conf_subscriptions/core.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/common/options/conf_subscriptions/installation.py` & `haupt-2.0.0rc8/haupt/common/options/conf_subscriptions/installation.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/common/options/feature.py` & `haupt-2.0.0rc8/haupt/common/options/feature.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,24 +13,23 @@
 from haupt.common.options.option import (
     NAMESPACE_DB_OPTION_MARKER,
     Option,
     OptionScope,
     OptionStores,
 )
 from haupt.common.options.option_namespaces import FEATURES
-from polyaxon import types
 
 
 class Feature(Option):
     scope = OptionScope.USER
     is_secret = False
     is_optional = True
     is_list = False
     store = OptionStores(settings.STORE_OPTION)
-    typing = types.BOOL
+    typing = "bool"
     default = True
     options = [True, False]
     immutable = False  # If immutable, the feature cannot be update by the user
     description = None
 
     @classmethod
     def get_marker(cls) -> str:
```

### Comparing `haupt-2.0.0rc7/haupt/common/options/option.py` & `haupt-2.0.0rc8/haupt/common/options/option.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 # Copyright 2018-2023 Polyaxon, Inc.
 # This file and its contents are licensed under the AGPLv3 License.
 # Please see the included NOTICE for copyright information and
 # LICENSE-AGPL for a copy of the license.
 
 from typing import Optional, Tuple
 
-from clipped.enums_utils import PEnum
+from clipped.utils.enums import PEnum
 
 from haupt.common.options.exceptions import OptionException
-from polyaxon.parser import parser
+from polyaxon.config.parser import Parser
 
 NAMESPACE_DB_OPTION_MARKER = ":"
 NAMESPACE_DB_CONFIG_MARKER = "__"
 NAMESPACE_SETTINGS_MARKER = "__"
 NAMESPACE_ENV_MARKER = ":"
 
 
@@ -102,15 +102,15 @@
 
     @classmethod
     def _extra_processing(cls, value):
         return value
 
     @classmethod
     def parse(cls, value):
-        _value = parser.TYPE_MAPPING[cls.typing](
+        _value = Parser.parse(cls.typing)(
             key=cls.key,
             value=value,
             is_list=cls.is_list,
             is_optional=cls.is_optional,
             default=cls.default,
             options=cls.options,
         )
```

### Comparing `haupt-2.0.0rc7/haupt/common/options/option_manager.py` & `haupt-2.0.0rc8/haupt/common/options/option_manager.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/common/options/option_owners.py` & `haupt-2.0.0rc8/haupt/common/options/option_owners.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/common/options/registry/containers.py` & `haupt-2.0.0rc8/haupt/common/options/registry/containers.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright 2018-2023 Polyaxon, Inc.
 # This file and its contents are licensed under the AGPLv3 License.
 # Please see the included NOTICE for copyright information and
 # LICENSE-AGPL for a copy of the license.
 
 from haupt.common.options import option_namespaces, option_subjects
 from haupt.common.options.option import Option, OptionScope, OptionStores
-from polyaxon import types
 from polyaxon.auxiliaries import (
     V1PolyaxonInitContainer,
     V1PolyaxonSidecarContainer,
     get_default_init_container,
     get_default_sidecar_container,
 )
 
@@ -27,15 +26,15 @@
 class PolyaxonInitContainer(Option):
     key = INIT_CONTAINER
     description = "The docker image to use for init container"
     scope = OptionScope.GLOBAL
     is_secret = False
     is_optional = True
     is_list = False
-    typing = types.STR
+    typing = "str"
     store = OptionStores.SETTINGS
     options = None
 
     @staticmethod
     def get_default_value():
         return get_default_init_container(schema=False)
 
@@ -50,15 +49,15 @@
 class PolyaxonSidecarContainer(Option):
     key = SIDECAR_CONTAINER
     description = "Sidecar container definition"
     scope = OptionScope.GLOBAL
     is_secret = False
     is_optional = True
     is_list = False
-    typing = types.DICT
+    typing = "dict"
     store = OptionStores.SETTINGS
     options = None
 
     @staticmethod
     def get_default_value():
         return get_default_sidecar_container(schema=False)
```

### Comparing `haupt-2.0.0rc7/haupt/common/options/registry/core.py` & `haupt-2.0.0rc8/haupt/common/options/registry/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 #
 # Copyright 2018-2023 Polyaxon, Inc.
 # This file and its contents are licensed under the AGPLv3 License.
 # Please see the included NOTICE for copyright information and
 # LICENSE-AGPL for a copy of the license.
 
 from haupt.common.options.option import Option, OptionScope, OptionStores
-from polyaxon import types
 
 LOGGING = "LOGGING"
 DEBUG = "DEBUG"
 PROTOCOL = "PROTOCOL"
 CELERY_BROKER_BACKEND = "CELERY_BROKER_BACKEND"
 CELERY_BROKER_URL = "CELERY_BROKER_URL"
 SECRET_INTERNAL_TOKEN = "SECRET_INTERNAL_TOKEN"  # noqa
@@ -44,166 +43,166 @@
 class Logging(Option):
     key = LOGGING
     scope = OptionScope.GLOBAL
     is_secret = False
     is_optional = False
     is_list = False
     store = OptionStores.SETTINGS
-    typing = types.DICT
+    typing = "dict"
     default = None
     options = None
 
 
 class Debug(Option):
     key = DEBUG
     scope = OptionScope.GLOBAL
     is_secret = False
     is_optional = False
     is_list = False
     store = OptionStores.SETTINGS
-    typing = types.DICT
+    typing = "dict"
     default = None
     options = None
 
 
 class Protocol(Option):
     key = PROTOCOL
     scope = OptionScope.GLOBAL
     is_secret = False
     is_optional = False
     is_list = False
     store = OptionStores.SETTINGS
-    typing = types.STR
+    typing = "str"
     default = None
     options = None
 
 
 class CeleryBrokerBackend(Option):
     key = CELERY_BROKER_BACKEND
     scope = OptionScope.GLOBAL
     is_secret = False
     is_optional = False
     is_list = False
     store = OptionStores.SETTINGS
-    typing = types.STR
+    typing = "str"
     default = None
     options = None
 
 
 class CeleryBrokerUrl(Option):
     key = CELERY_BROKER_URL
     scope = OptionScope.GLOBAL
     is_secret = False
     is_optional = False
     is_list = False
     store = OptionStores.SETTINGS
-    typing = types.STR
+    typing = "str"
     default = None
     options = None
 
 
 class SecretInternalToken(Option):
     key = SECRET_INTERNAL_TOKEN
     scope = OptionScope.GLOBAL
     is_secret = True
     is_optional = False
     is_list = False
     store = OptionStores.SETTINGS
-    typing = types.STR
+    typing = "str"
     default = None
     options = None
 
 
 class HealthCheckWorkerTimeout(Option):
     key = HEALTH_CHECK_WORKER_TIMEOUT
     scope = OptionScope.GLOBAL
     is_secret = False
     is_optional = True
     is_list = False
     store = OptionStores.SETTINGS
-    typing = types.INT
+    typing = "int"
     default = 4
     options = None
 
 
 class SchedulerEnabled(Option):
     key = SCHEDULER_ENABLED
     scope = OptionScope.GLOBAL
     is_secret = False
     is_optional = True
     is_list = False
     store = OptionStores.SETTINGS
-    typing = types.BOOL
+    typing = "bool"
     default = True
     options = None
 
 
 class UiAdminEnabled(Option):
     key = UI_ADMIN_ENABLED
     scope = OptionScope.GLOBAL
     is_secret = False
     is_optional = True
     is_list = False
     store = OptionStores.SETTINGS
-    typing = types.BOOL
+    typing = "bool"
     default = True
     options = None
 
 
 class UiAssetsVersion(Option):
     key = UI_ASSETS_VERSION
     scope = OptionScope.GLOBAL
     is_secret = False
     is_optional = True
     is_list = False
     store = OptionStores.SETTINGS
-    typing = types.STR
+    typing = "str"
     default = ""
     options = None
 
 
 class UiBaseUrl(Option):
     key = UI_BASE_URL
     scope = OptionScope.GLOBAL
     is_secret = False
     is_optional = True
     is_list = False
     store = OptionStores.SETTINGS
-    typing = types.STR
+    typing = "str"
     default = "/"
     options = None
 
 
 class UiOffline(Option):
     key = UI_OFFLINE
     scope = OptionScope.GLOBAL
     is_secret = False
     is_optional = True
     is_list = False
     store = OptionStores.SETTINGS
-    typing = types.BOOL
+    typing = "bool"
     default = False
     options = None
 
 
 class UiEnabled(Option):
     key = UI_ENABLED
     scope = OptionScope.GLOBAL
     is_secret = False
     is_optional = True
     is_list = False
     store = OptionStores.SETTINGS
-    typing = types.BOOL
+    typing = "bool"
     default = False
     options = None
 
 
 class UiInSandbox(Option):
     key = UI_IN_SANDBOX
     scope = OptionScope.GLOBAL
     is_secret = False
     is_optional = True
     is_list = False
     store = OptionStores.SETTINGS
-    typing = types.BOOL
+    typing = "bool"
     default = False
     options = None
```

### Comparing `haupt-2.0.0rc7/haupt/common/options/registry/installation.py` & `haupt-2.0.0rc8/haupt/common/options/registry/installation.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 #
 # Copyright 2018-2023 Polyaxon, Inc.
 # This file and its contents are licensed under the AGPLv3 License.
 # Please see the included NOTICE for copyright information and
 # LICENSE-AGPL for a copy of the license.
 
 from haupt.common.options.option import Option, OptionScope, OptionStores
-from polyaxon import types
 
 POLYAXON_ENVIRONMENT = "POLYAXON_ENVIRONMENT"
 PLATFORM_VERSION = "PLATFORM_VERSION"
 PLATFORM_DIST = "PLATFORM_DIST"
 PLATFORM_HOST = "PLATFORM_HOST"
 CHART_VERSION = "CHART_VERSION"
 ORGANIZATION_KEY = "POLYAXON_ORGANIZATION_KEY"
@@ -27,71 +26,71 @@
 
 class PlatformEnvironmentVersion(Option):
     key = POLYAXON_ENVIRONMENT
     scope = OptionScope.GLOBAL
     is_secret = False
     is_optional = True
     is_list = False
-    typing = types.STR
+    typing = "str"
     store = OptionStores.SETTINGS
     default = None
     options = None
 
 
 class PlatformVersion(Option):
     key = PLATFORM_VERSION
     scope = OptionScope.GLOBAL
     is_secret = False
     is_optional = True
     is_list = False
-    typing = types.STR
+    typing = "str"
     store = OptionStores.SETTINGS
     default = None
     options = None
 
 
 class PlatformDist(Option):
     key = PLATFORM_DIST
     scope = OptionScope.GLOBAL
     is_secret = False
     is_optional = True
     is_list = False
-    typing = types.STR
+    typing = "str"
     store = OptionStores.SETTINGS
     default = None
     options = None
 
 
 class PlatformHost(Option):
     key = PLATFORM_HOST
     scope = OptionScope.GLOBAL
     is_secret = False
     is_optional = True
     is_list = False
     store = OptionStores.SETTINGS
-    typing = types.STR
+    typing = "str"
     default = None
     options = None
 
 
 class ChartVersion(Option):
     key = CHART_VERSION
     scope = OptionScope.GLOBAL
     is_secret = False
     is_optional = True
     is_list = False
-    typing = types.STR
+    typing = "str"
     store = OptionStores.SETTINGS
     default = None
     options = None
 
 
 class OrganizationKey(Option):
     key = ORGANIZATION_KEY
     scope = OptionScope.GLOBAL
     is_secret = False
     is_optional = True
     is_list = False
-    typing = types.STR
+    typing = "str"
     store = OptionStores.ENV
     default = None
     options = None
```

### Comparing `haupt-2.0.0rc7/haupt/common/options/registry/k8s.py` & `haupt-2.0.0rc8/haupt/common/options/registry/k8s.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,37 +2,36 @@
 #
 # Copyright 2018-2023 Polyaxon, Inc.
 # This file and its contents are licensed under the AGPLv3 License.
 # Please see the included NOTICE for copyright information and
 # LICENSE-AGPL for a copy of the license.
 
 from haupt.common.options.option import Option, OptionScope, OptionStores
-from polyaxon import types
 
 K8S_NAMESPACE = "K8S_NAMESPACE"
 K8S_IN_CLUSTER = "K8S_IN_CLUSTER"
 
 OPTIONS = {K8S_NAMESPACE, K8S_IN_CLUSTER}
 
 
 class K8SNamespace(Option):
     key = K8S_NAMESPACE
     scope = OptionScope.GLOBAL
     is_secret = False
     is_optional = False
     is_list = False
-    typing = types.STR
+    typing = "str"
     store = OptionStores.SETTINGS
     default = None
     options = None
 
 
 class K8SInCluster(Option):
     key = K8S_IN_CLUSTER
     scope = OptionScope.GLOBAL
     is_secret = False
     is_optional = False
     is_list = False
-    typing = types.BOOL
+    typing = "bool"
     store = OptionStores.SETTINGS
     default = None
     options = None
```

### Comparing `haupt-2.0.0rc7/haupt/common/options/registry/scheduler.py` & `haupt-2.0.0rc8/haupt/common/options/registry/scheduler.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright 2018-2023 Polyaxon, Inc.
 # This file and its contents are licensed under the AGPLv3 License.
 # Please see the included NOTICE for copyright information and
 # LICENSE-AGPL for a copy of the license.
 
 from haupt.common.options import option_namespaces, option_subjects
 from haupt.common.options.option import Option, OptionScope, OptionStores
-from polyaxon import types
 
 # Global Async Countdown
 SCHEDULER_GLOBAL_COUNTDOWN = "{}_{}".format(
     option_namespaces.SCHEDULER,
     option_subjects.GLOBAL_COUNTDOWN,
 )
 
@@ -22,12 +21,12 @@
 
 class SchedulerCountdown(Option):
     key = SCHEDULER_GLOBAL_COUNTDOWN
     scope = OptionScope.GLOBAL
     is_secret = False
     is_optional = True
     is_list = False
-    typing = types.INT
+    typing = "int"
     store = OptionStores.SETTINGS
     default = 1
     options = None
     description = "Global count down for scheduler"
```

### Comparing `haupt-2.0.0rc7/haupt/common/options/registry/stats.py` & `haupt-2.0.0rc8/haupt/common/options/registry/stats.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,27 +11,26 @@
 from haupt.common.options.cache import LONG_CACHE_TTL
 from haupt.common.options.option import (
     NAMESPACE_DB_OPTION_MARKER,
     Option,
     OptionScope,
     OptionStores,
 )
-from polyaxon import types
 
 STATS_DEFAULT_PREFIX = "{}{}{}".format(
     option_namespaces.STATS, NAMESPACE_DB_OPTION_MARKER, option_subjects.DEFAULT_PREFIX
 )
 
 OPTIONS = {STATS_DEFAULT_PREFIX}
 
 
 class StatsDefaultPrefix(Option):
     key = STATS_DEFAULT_PREFIX
     scope = OptionScope.GLOBAL
     is_secret = False
     is_optional = True
     is_list = False
-    typing = types.STR
+    typing = "str"
     store = OptionStores(settings.STORE_OPTION)
     default = None
     options = None
     cache_ttl = LONG_CACHE_TTL
```

### Comparing `haupt-2.0.0rc7/haupt/common/query/service.py` & `haupt-2.0.0rc8/haupt/common/query/service.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/common/redis_db.py` & `haupt-2.0.0rc8/haupt/common/redis_db.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/common/service_interface.py` & `haupt-2.0.0rc8/haupt/common/service_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # This file and its contents are licensed under the AGPLv3 License.
 # Please see the included NOTICE for copyright information and
 # LICENSE-AGPL for a copy of the license.
 
 import inspect
 import itertools
 
-from clipped.imports import import_string
+from clipped.utils.imports import import_string
 
 try:
     from django.utils.functional import LazyObject, empty  # pylint:disable=import-error
 except ImportError:
     raise ImportError("This module depends on django.")
```

### Comparing `haupt-2.0.0rc7/haupt/common/settings/admin.py` & `haupt-2.0.0rc8/haupt/common/settings/admin.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,14 @@
 # Please see the included NOTICE for copyright information and
 # LICENSE-AGPL for a copy of the license.
 
 from haupt.common.config_manager import ConfigManager
 
 
 def set_admin(context, config: ConfigManager):
-    admin_name = config.get_string("POLYAXON_ADMIN_NAME", is_optional=True)
-    admin_mail = config.get_string("POLYAXON_ADMIN_MAIL", is_optional=True)
+    admin_name = config.get("POLYAXON_ADMIN_NAME", "str", is_optional=True)
+    admin_mail = config.get("POLYAXON_ADMIN_MAIL", "str", is_optional=True)
 
     if admin_mail and admin_mail:
         admins = ((admin_name, admin_mail),)
         context["ADMINS"] = admins
         context["MANAGERS"] = admins
```

### Comparing `haupt-2.0.0rc7/haupt/common/settings/apps.py` & `haupt-2.0.0rc8/haupt/common/settings/apps.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,16 @@
     third_party_apps: Optional[Tuple],
     project_apps: Tuple,
     db_app: Optional[str] = None,
     use_db_apps: bool = True,
     use_admin_apps: bool = False,
     use_staticfiles_app: bool = True,
 ):
-    extra_apps = config.get_string(
-        "POLYAXON_EXTRA_APPS", is_list=True, is_optional=True
+    extra_apps = config.get(
+        "POLYAXON_EXTRA_APPS", "str", is_list=True, is_optional=True
     )
     extra_apps = tuple(extra_apps) if extra_apps else ()
 
     apps = ()
     if use_db_apps:
         apps += (
             "django.contrib.auth",
```

### Comparing `haupt-2.0.0rc7/haupt/common/settings/assets.py` & `haupt-2.0.0rc8/haupt/common/settings/assets.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,26 +11,30 @@
     EV_KEYS_ARTIFACTS_ROOT,
     EV_KEYS_STATIC_ROOT,
     EV_KEYS_STATIC_URL,
 )
 
 
 def set_assets(context, config: ConfigManager):
-    context["MEDIA_ROOT"] = config.get_string(
-        "POLYAXON_MEDIA_ROOT", is_optional=True, default=""
+    context["MEDIA_ROOT"] = config.get(
+        "POLYAXON_MEDIA_ROOT", "str", is_optional=True, default=""
     )
-    context["MEDIA_URL"] = config.get_string(
-        "POLYAXON_MEDIA_URL", is_optional=True, default=""
+    context["MEDIA_URL"] = config.get(
+        "POLYAXON_MEDIA_URL", "str", is_optional=True, default=""
     )
 
-    context["STATIC_ROOT"] = config.get_string(
-        EV_KEYS_STATIC_ROOT, is_optional=True, default=str(config.root_dir / "static")
+    context["STATIC_ROOT"] = config.get(
+        EV_KEYS_STATIC_ROOT,
+        "str",
+        is_optional=True,
+        default=str(config.root_dir / "static"),
     )
-    context["STATIC_URL"] = config.get_string(
+    context["STATIC_URL"] = config.get(
         EV_KEYS_STATIC_URL,
+        "str",
         is_optional=True,
         default="/static/",
     )
 
     # Additional locations of static files
     context["STATICFILES_DIRS"] = (str(config.root_dir / "public"),)
 
@@ -43,15 +47,19 @@
         str(config.root_dir / "locale"),
         str(config.root_dir / "client" / "js" / "libs" / "locale"),
     )
 
     context["STATICI18N_ROOT"] = STATIC_V1
     context["STATICI18N_OUTPUT_DIR"] = "jsi18n"
 
-    context["ARTIFACTS_ROOT"] = config.get_string(
+    context["ARTIFACTS_ROOT"] = config.get(
         EV_KEYS_ARTIFACTS_ROOT,
+        "str",
         is_optional=True,
         default="/tmp/plx/artifacts_uploads",
     )
-    context["ARCHIVES_ROOT"] = config.get_string(
-        "POLYAXON_ARCHIVES_ROOT", is_optional=True, default="/tmp/plx/archives"
+    context["ARCHIVES_ROOT"] = config.get(
+        "POLYAXON_ARCHIVES_ROOT",
+        "str",
+        is_optional=True,
+        default="/tmp/plx/archives",
     )
```

### Comparing `haupt-2.0.0rc7/haupt/common/settings/celery.py` & `haupt-2.0.0rc8/haupt/common/settings/celery.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,89 +8,104 @@
 
 from haupt.common.config_manager import ConfigManager
 
 
 def set_celery(
     context, config: ConfigManager, routes: Dict, schedules: Optional[Dict] = None
 ):
-    context["CELERY_TASK_TRACK_STARTED"] = config.get_boolean(
-        "POLYAXON_CELERY_TASK_TRACK_STARTED", is_optional=True, default=True
+    context["CELERY_TASK_TRACK_STARTED"] = config.get(
+        "POLYAXON_CELERY_TASK_TRACK_STARTED", "bool", is_optional=True, default=True
     )
 
-    context["CELERY_BROKER_POOL_LIMIT"] = config.get_int(
-        "POLYAXON_CELERY_BROKER_POOL_LIMIT", is_optional=True, default=100
+    context["CELERY_BROKER_POOL_LIMIT"] = config.get(
+        "POLYAXON_CELERY_BROKER_POOL_LIMIT", "int", is_optional=True, default=100
     )
 
     context["CELERY_BROKER_BACKEND"] = config.broker_backend
-    confirm_publish = config.get_boolean(
-        "POLYAXON_CELERY_CONFIRM_PUBLISH", is_optional=True, default=True
+    confirm_publish = config.get(
+        "POLYAXON_CELERY_CONFIRM_PUBLISH", "bool", is_optional=True, default=True
     )
     context["CELERY_CONFIRM_PUBLISH"] = confirm_publish
     if config.is_rabbitmq_broker and confirm_publish:
         # see https://github.com/celery/celery/issues/5410 for details
         context["CELERY_BROKER_TRANSPORT_OPTIONS"] = {"confirm_publish": True}
 
     context["CELERY_BROKER_URL"] = config.get_broker_url()
 
-    context["INTERNAL_EXCHANGE"] = config.get_string(
-        "POLYAXON_INTERNAL_EXCHANGE", is_optional=True, default="internal"
+    context["INTERNAL_EXCHANGE"] = config.get(
+        "POLYAXON_INTERNAL_EXCHANGE", "str", is_optional=True, default="internal"
     )
 
-    result_bucked = config.get_string(
+    result_bucked = config.get(
         "POLYAXON_REDIS_CELERY_RESULT_BACKEND_URL",
+        "str",
         is_optional=True,
     )
     if result_bucked:
         context["CELERY_RESULT_BACKEND"] = config.get_redis_url(
             "POLYAXON_REDIS_CELERY_RESULT_BACKEND_URL"
         )
 
-    context["CELERY_WORKER_PREFETCH_MULTIPLIER"] = config.get_int(
-        "POLYAXON_CELERY_WORKER_PREFETCH_MULTIPLIER", is_optional=True, default=4
+    context["CELERY_WORKER_PREFETCH_MULTIPLIER"] = config.get(
+        "POLYAXON_CELERY_WORKER_PREFETCH_MULTIPLIER",
+        "int",
+        is_optional=True,
+        default=4,
     )
 
-    eager_mode = config.get_boolean(
-        "POLYAXON_CELERY_TASK_ALWAYS_EAGER", is_optional=True, default=False
+    eager_mode = config.get(
+        "POLYAXON_CELERY_TASK_ALWAYS_EAGER", "bool", is_optional=True, default=False
     )
     context["CELERY_TASK_ALWAYS_EAGER"] = eager_mode
     if eager_mode:
         context["CELERY_BROKER_TRANSPORT"] = "memory"
 
     context["CELERY_ACCEPT_CONTENT"] = ["application/json"]
     context["CELERY_TASK_DEFAULT_PRIORITY"] = 10
     context["CELERY_TASK_SERIALIZER"] = "json"
     context["CELERY_RESULT_SERIALIZER"] = "json"
     context["CELERY_TASK_IGNORE_RESULT"] = True
     context["CELERY_TIMEZONE"] = config.timezone
-    context["CELERY_HARD_TIME_LIMIT_DELAY"] = config.get_int(
-        "POLYAXON_CELERY_HARD_TIME_LIMIT_DELAY", is_optional=True, default=180
+    context["CELERY_HARD_TIME_LIMIT_DELAY"] = config.get(
+        "POLYAXON_CELERY_HARD_TIME_LIMIT_DELAY",
+        "int",
+        is_optional=True,
+        default=180,
     )
 
-    context["CELERY_WORKER_MAX_TASKS_PER_CHILD"] = config.get_int(
-        "POLYAXON_CELERY_WORKER_MAX_TASKS_PER_CHILD", is_optional=True, default=100
+    context["CELERY_WORKER_MAX_TASKS_PER_CHILD"] = config.get(
+        "POLYAXON_CELERY_WORKER_MAX_TASKS_PER_CHILD",
+        "int",
+        is_optional=True,
+        default=100,
     )
 
-    context["CELERY_WORKER_MAX_MEMORY_PER_CHILD"] = config.get_int(
-        "POLYAXON_CELERY_WORKER_MAX_MEMORY_PER_CHILD", is_optional=True, default=400000
+    context["CELERY_WORKER_MAX_MEMORY_PER_CHILD"] = config.get(
+        "POLYAXON_CELERY_WORKER_MAX_MEMORY_PER_CHILD",
+        "int",
+        is_optional=True,
+        default=400000,
     )
 
     class Intervals:
         """All intervals are in seconds"""
 
-        OPERATIONS_DEFAULT_RETRY_DELAY = config.get_int(
+        OPERATIONS_DEFAULT_RETRY_DELAY = config.get(
             "POLYAXON_INTERVALS_OPERATIONS_DEFAULT_RETRY_DELAY",
+            "int",
             is_optional=True,
             default=60,
         )
-        OPERATIONS_MAX_RETRY_DELAY = config.get_int(
+        OPERATIONS_MAX_RETRY_DELAY = config.get(
             "POLYAXON_INTERVALS_OPERATIONS_MAX_RETRY_DELAY",
+            "int",
             is_optional=True,
             default=60 * 60,
         )
-        RUNS_SCHEDULER = config.get_int(
-            "POLYAXON_INTERVALS_RUNS_SCHEDULER", is_optional=True, default=30
+        RUNS_SCHEDULER = config.get(
+            "POLYAXON_INTERVALS_RUNS_SCHEDULER", "int", is_optional=True, default=30
         )
 
     context["Intervals"] = Intervals
     context["CELERY_TASK_ROUTES"] = routes
     if schedules:
         context["CELERY_BEAT_SCHEDULE"] = schedules
```

### Comparing `haupt-2.0.0rc7/haupt/common/settings/context_processors.py` & `haupt-2.0.0rc8/haupt/common/settings/context_processors.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/common/settings/core.py` & `haupt-2.0.0rc8/haupt/common/settings/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,32 +36,33 @@
             "django.db.backends.sqlite3"
             if config.is_sqlite_db_engine
             else "django.db.backends.postgresql"
         )
         context["AUTH_USER_MODEL"] = "db.User"
         context["DB_ENGINE_NAME"] = config.db_engine_name
         context["DEFAULT_DB_ENGINE"] = db_engine
-        db_name = config.get_string("POLYAXON_DB_NAME", is_optional=True)
+        db_name = config.get("POLYAXON_DB_NAME", "str", is_optional=True)
         if not db_name:
             db_name = "/tmp/plxdb" if config.is_sqlite_db_engine else "polyaxon"
         db_definition = {
             "ENGINE": db_engine,
             "NAME": db_name,
-            "USER": config.get_string("POLYAXON_DB_USER", is_optional=True),
-            "PASSWORD": config.get_string(
-                "POLYAXON_DB_PASSWORD", is_secret=True, is_optional=True
+            "USER": config.get("POLYAXON_DB_USER", "str", is_optional=True),
+            "PASSWORD": config.get(
+                "POLYAXON_DB_PASSWORD", "str", is_secret=True, is_optional=True
             ),
-            "HOST": config.get_string("POLYAXON_DB_HOST", is_optional=True),
-            "PORT": config.get_string("POLYAXON_DB_PORT", is_optional=True),
+            "HOST": config.get("POLYAXON_DB_HOST", "str", is_optional=True),
+            "PORT": config.get("POLYAXON_DB_PORT", "str", is_optional=True),
             "ATOMIC_REQUESTS": True,
-            "CONN_MAX_AGE": config.get_int(
+            "CONN_MAX_AGE": config.get(
                 "POLYAXON_DB_CONN_MAX_AGE",
+                "int",
                 is_optional=True,
                 default=60,
             ),
         }
-        db_options = config.get_dict(
-            "POLYAXON_DB_OPTIONS", is_optional=True, default={}
+        db_options = config.get(
+            "POLYAXON_DB_OPTIONS", "dict", is_optional=True, default={}
         )
         if db_options:
             db_definition["OPTIONS"] = db_options
         context["DATABASES"] = {"default": db_definition}
```

### Comparing `haupt-2.0.0rc7/haupt/common/settings/cors.py` & `haupt-2.0.0rc8/haupt/common/settings/cors.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,29 +10,29 @@
 from haupt.common.config_manager import ConfigManager
 from polyaxon.services.headers import PolyaxonServiceHeaders
 
 
 def set_cors(context, config: ConfigManager):
     # session settings
     context["CORS_ALLOW_CREDENTIALS"] = True
-    allowed_list = config.get_list(
-        "POLYAXON_CORS_ALLOWED_ORIGINS", is_optional=True, default=[]
+    allowed_list = config.get(
+        "POLYAXON_CORS_ALLOWED_ORIGINS", "list", is_optional=True, default=[]
     )
     context["CORS_ALLOWED_ORIGINS"] = allowed_list
     context["CORS_ALLOW_ALL_ORIGINS"] = False if allowed_list else True
 
     context["CORS_ALLOW_HEADERS"] = (
         default_headers + PolyaxonServiceHeaders.get_headers()
     )
 
-    ssl_enabled = config.get_boolean(
-        "POLYAXON_SSL_ENABLED", is_optional=True, default=False
+    ssl_enabled = config.get(
+        "POLYAXON_SSL_ENABLED", "bool", is_optional=True, default=False
     )
-    ssl_redirect_enabled = config.get_boolean(
-        "POLYAXON_SSL_REDIRECT_ENABLED", is_optional=True, default=False
+    ssl_redirect_enabled = config.get(
+        "POLYAXON_SSL_REDIRECT_ENABLED", "bool", is_optional=True, default=False
     )
     context["SSL_ENABLED"] = ssl_enabled
     context["PROTOCOL"] = "http"
     context["WS_PROTOCOL"] = "ws"
     if ssl_enabled:
         context["SESSION_COOKIE_SECURE"] = True
         context["CSRF_COOKIE_SECURE"] = True
```

### Comparing `haupt-2.0.0rc7/haupt/common/settings/defaults.py` & `haupt-2.0.0rc8/haupt/common/settings/defaults.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/common/settings/encryption.py` & `haupt-2.0.0rc8/haupt/common/settings/secrets.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 #
 # Copyright 2018-2023 Polyaxon, Inc.
 # This file and its contents are licensed under the AGPLv3 License.
 # Please see the included NOTICE for copyright information and
 # LICENSE-AGPL for a copy of the license.
 
 from haupt.common.config_manager import ConfigManager
+from polyaxon.env_vars.keys import EV_KEYS_SECRET_KEY
 
 
-def set_encryption(context, config: ConfigManager):
-    context["ENCRYPTION_KEY"] = config.get_string(
-        "POLYAXON_ENCRYPTION_KEY", is_optional=True
+def set_secrets(context, config: ConfigManager):
+    context["SECRET_KEY"] = config.get(
+        EV_KEYS_SECRET_KEY,
+        "str",
+        is_secret=True,
+        is_optional=True,
+        default="default-secret",
     )
-    context["ENCRYPTION_SECRET"] = config.get_string(
-        "POLYAXON_ENCRYPTION_SECRET", is_optional=True
-    )
-    context["ENCRYPTION_BACKEND"] = config.get_string(
-        "POLYAXON_ENCRYPTION_BACKEND", is_optional=True
+    context["SECRET_INTERNAL_TOKEN"] = config.get(
+        "POLYAXON_SECRET_INTERNAL_TOKEN", "str", is_secret=True, is_optional=True
     )
```

### Comparing `haupt-2.0.0rc7/haupt/common/settings/logging.py` & `haupt-2.0.0rc8/haupt/common/settings/logging.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 # Please see the included NOTICE for copyright information and
 # LICENSE-AGPL for a copy of the license.
 
 import os
 
 from typing import Dict
 
-from clipped.logging_utils import DEFAULT_LOGS_ROOT
+from clipped.utils.logging import DEFAULT_LOGS_ROOT
 
 from haupt.common.config_manager import ConfigManager
 from polyaxon.env_vars.keys import EV_KEYS_LOGS_ROOT
 
 
 def set_logging(
     context,
     config: ConfigManager,
 ) -> Dict:
-    log_dir = config.get_string(
-        EV_KEYS_LOGS_ROOT, is_optional=True, default=DEFAULT_LOGS_ROOT
+    log_dir = config.get(
+        EV_KEYS_LOGS_ROOT, "str", is_optional=True, default=DEFAULT_LOGS_ROOT
     )
     context["LOG_DIRECTORY"] = log_dir
     if not os.path.exists(log_dir):
         os.makedirs(log_dir)
     logging_spec = {
         "version": 1,
         "disable_existing_loggers": False,
```

### Comparing `haupt-2.0.0rc7/haupt/common/settings/middlewares.py` & `haupt-2.0.0rc8/haupt/common/settings/middlewares.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/common/settings/services/api.py` & `haupt-2.0.0rc8/haupt/common/settings/services/api.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/common/settings/services/background.py` & `haupt-2.0.0rc8/haupt/common/settings/services/background.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/common/settings/services/streams.py` & `haupt-2.0.0rc8/haupt/common/settings/services/streams.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/python
 #
 # Copyright 2018-2023 Polyaxon, Inc.
 # This file and its contents are licensed under the AGPLv3 License.
 # Please see the included NOTICE for copyright information and
 # LICENSE-AGPL for a copy of the license.
+
 from haupt.common.config_manager import ConfigManager
 from haupt.common.settings.apps import set_apps
 from haupt.common.settings.assets import set_assets
 from haupt.common.settings.core import set_core
 from haupt.common.settings.cors import set_cors
 from haupt.common.settings.middlewares import set_base_middlewares
 from haupt.common.settings.ui import set_ui
@@ -26,16 +27,16 @@
         use_db_apps=False,
         use_staticfiles_app=context["UI_IN_SANDBOX"],
     )
 
 
 def set_service(context, config: ConfigManager):
     # This is repeated because it's required for using the staticfiles app
-    context["UI_IN_SANDBOX"] = config.get_boolean(
-        EV_KEYS_UI_IN_SANDBOX, is_optional=True, default=False
+    context["UI_IN_SANDBOX"] = config.get(
+        EV_KEYS_UI_IN_SANDBOX, "bool", is_optional=True, default=False
     )
     set_streams_apps(context, config)
     set_core(context=context, config=config, use_db=False)
     set_cors(context=context, config=config)
     set_ui(context=context, config=config)
     set_base_middlewares(context=context, config=config)
     set_assets(context=context, config=config)
```

### Comparing `haupt-2.0.0rc7/haupt/common/settings/ui.py` & `haupt-2.0.0rc8/haupt/common/settings/ui.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,29 +16,33 @@
     EV_KEYS_UI_IN_SANDBOX,
     EV_KEYS_UI_OFFLINE,
 )
 
 
 def set_ui(context, config: ConfigManager, processors: Optional[List[str]] = None):
     context["ROOT_URLCONF"] = "{}.urls".format(config.config_module)
-    platform_host = config.get_string(EV_KEYS_PLATFORM_HOST, is_optional=True)
+    platform_host = config.get(EV_KEYS_PLATFORM_HOST, "str", is_optional=True)
     context["PLATFORM_HOST"] = platform_host
 
     def get_allowed_hosts():
-        allowed_hosts = config.get_string(
-            "POLYAXON_ALLOWED_HOSTS", is_optional=True, is_list=True, default=["*"]
+        allowed_hosts = config.get(
+            "POLYAXON_ALLOWED_HOSTS",
+            "str",
+            is_optional=True,
+            is_list=True,
+            default=["*"],
         )  # type: list
         if platform_host:
             allowed_hosts.append(platform_host)
         if ".polyaxon.com" not in allowed_hosts:
             allowed_hosts.append(".polyaxon.com")
-        pod_ip = config.get_string("POLYAXON_POD_IP", is_optional=True)
+        pod_ip = config.get("POLYAXON_POD_IP", "str", is_optional=True)
         if pod_ip:
             allowed_hosts.append(pod_ip)
-        host_ip = config.get_string("POLYAXON_HOST_IP", is_optional=True)
+        host_ip = config.get("POLYAXON_HOST_IP", "str", is_optional=True)
         if host_ip:
             host_cidr = ".".join(host_ip.split(".")[:-1])
             allowed_hosts += ["{}.{}".format(host_cidr, i) for i in range(255)]
 
         return allowed_hosts
 
     context["ALLOWED_HOSTS"] = get_allowed_hosts()
@@ -59,42 +63,42 @@
         "haupt.common.settings.context_processors.ui_assets_version",
         "haupt.common.settings.context_processors.ui_base_url",
         "haupt.common.settings.context_processors.ui_offline",
         "haupt.common.settings.context_processors.ui_enabled",
         "haupt.common.settings.context_processors.ui_in_sandbox",
     ] + processors
 
-    context["FRONTEND_DEBUG"] = config.get_boolean(
-        "POLYAXON_FRONTEND_DEBUG", is_optional=True, default=False
+    context["FRONTEND_DEBUG"] = config.get(
+        "POLYAXON_FRONTEND_DEBUG", "bool", is_optional=True, default=False
     )
 
     template_debug = (
-        config.get_boolean("DJANGO_TEMPLATE_DEBUG", is_optional=True)
+        config.get("DJANGO_TEMPLATE_DEBUG", "bool", is_optional=True)
         or config.is_debug_mode
     )
-    context["UI_ADMIN_ENABLED"] = config.get_boolean(
-        EV_KEYS_UI_ADMIN_ENABLED, is_optional=True, default=False
+    context["UI_ADMIN_ENABLED"] = config.get(
+        EV_KEYS_UI_ADMIN_ENABLED, "bool", is_optional=True, default=False
     )
-    base_url = config.get_string(EV_KEYS_UI_BASE_URL, is_optional=True)
+    base_url = config.get(EV_KEYS_UI_BASE_URL, "str", is_optional=True)
     if base_url:
         context["UI_BASE_URL"] = base_url
         context["FORCE_SCRIPT_NAME"] = base_url
     else:
         context["UI_BASE_URL"] = "/"
-    context["UI_ASSETS_VERSION"] = config.get_string(
-        EV_KEYS_UI_ASSETS_VERSION, is_optional=True, default=""
+    context["UI_ASSETS_VERSION"] = config.get(
+        EV_KEYS_UI_ASSETS_VERSION, "str", is_optional=True, default=""
     )
-    context["UI_OFFLINE"] = config.get_boolean(
-        EV_KEYS_UI_OFFLINE, is_optional=True, default=False
+    context["UI_OFFLINE"] = config.get(
+        EV_KEYS_UI_OFFLINE, "bool", is_optional=True, default=False
     )
-    context["UI_ENABLED"] = config.get_boolean(
-        EV_KEYS_UI_ENABLED, is_optional=True, default=True
+    context["UI_ENABLED"] = config.get(
+        EV_KEYS_UI_ENABLED, "bool", is_optional=True, default=True
     )
-    context["UI_IN_SANDBOX"] = config.get_boolean(
-        EV_KEYS_UI_IN_SANDBOX, is_optional=True, default=False
+    context["UI_IN_SANDBOX"] = config.get(
+        EV_KEYS_UI_IN_SANDBOX, "bool", is_optional=True, default=False
     )
     context["TEMPLATES_DEBUG"] = template_debug
     context["LIST_TEMPLATE_CONTEXT_PROCESSORS"] = processors
     context["TEMPLATES"] = [
         {
             "BACKEND": "django.template.backends.django.DjangoTemplates",
             "APP_DIRS": True,
```

### Comparing `haupt-2.0.0rc7/haupt/common/test_cases/base.py` & `haupt-2.0.0rc8/haupt/common/test_cases/base.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/common/test_clients/base.py` & `haupt-2.0.0rc8/haupt/common/test_clients/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 #
 # Copyright 2018-2023 Polyaxon, Inc.
 # This file and its contents are licensed under the AGPLv3 License.
 # Please see the included NOTICE for copyright information and
 # LICENSE-AGPL for a copy of the license.
 
 import datetime
-import json
 import uuid
 
 from collections.abc import Mapping
 from urllib.parse import urlparse
 
+from clipped.utils.json import orjson_dumps
+
 from django.test import Client
 from django.test.client import FakePayload
 
 CONTENT_TYPE_APPLICATION_JSON = "application/json"
 
 
 class BaseClient(Client):
@@ -47,15 +48,15 @@
         if isinstance(data, list):
             for d in data:
                 validate_data(d)
         else:
             validate_data(data)
 
         if content_type == CONTENT_TYPE_APPLICATION_JSON:
-            data = json.dumps(data)
+            data = orjson_dumps(data)
 
         request = self.encode_data(method, path, data, content_type, **extra)
         return self.request(**request)
 
     def put(self, path, data=None, content_type=CONTENT_TYPE_APPLICATION_JSON, **extra):
         """Construct a PUT request."""
         return self.do_request("PUT", path, data, content_type, **extra)
```

### Comparing `haupt-2.0.0rc7/haupt/common/validation/blacklist.py` & `haupt-2.0.0rc8/haupt/common/validation/blacklist.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/common/validation/slugs.py` & `haupt-2.0.0rc8/haupt/common/validation/slugs.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 try:
     from django.utils.safestring import mark_safe
 except ImportError:
     raise ImportError("This module depends on django.")
 
 
-from clipped.string_utils import slugify as core_slugify
+from clipped.utils.strings import slugify as core_slugify
 
 
 def slugify(value: str) -> str:
     return core_slugify(value, mark_safe)
 
 
 slug_dots_re = _lazy_re_compile(r"^[-a-zA-Z0-9_.]+\Z")
```

### Comparing `haupt-2.0.0rc7/haupt/common/workers.py` & `haupt-2.0.0rc8/haupt/common/workers.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/db/abstracts/artifacts.py` & `haupt-2.0.0rc8/haupt/db/abstracts/artifacts.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/db/abstracts/catalogs.py` & `haupt-2.0.0rc8/haupt/db/abstracts/catalogs.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/db/abstracts/duration.py` & `haupt-2.0.0rc8/haupt/db/abstracts/duration.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/db/abstracts/getter.py` & `haupt-2.0.0rc8/haupt/db/abstracts/getter.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/db/abstracts/live_state.py` & `haupt-2.0.0rc8/haupt/db/abstracts/live_state.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/db/abstracts/nameable.py` & `haupt-2.0.0rc8/haupt/db/abstracts/nameable.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/db/abstracts/projects.py` & `haupt-2.0.0rc8/haupt/db/abstracts/projects.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/db/abstracts/runs.py` & `haupt-2.0.0rc8/haupt/db/abstracts/runs.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/db/abstracts/spec.py` & `haupt-2.0.0rc8/haupt/db/abstracts/spec.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/db/abstracts/stage.py` & `haupt-2.0.0rc8/haupt/db/abstracts/stage.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/db/abstracts/state.py` & `haupt-2.0.0rc8/haupt/db/abstracts/state.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/db/abstracts/status.py` & `haupt-2.0.0rc8/haupt/db/abstracts/status.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/db/abstracts/tag.py` & `haupt-2.0.0rc8/haupt/db/abstracts/tag.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/db/administration/artifacts.py` & `haupt-2.0.0rc8/haupt/db/administration/artifacts.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/db/administration/projects.py` & `haupt-2.0.0rc8/haupt/db/administration/projects.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/db/administration/register.py` & `haupt-2.0.0rc8/haupt/db/administration/register.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/db/administration/runs.py` & `haupt-2.0.0rc8/haupt/db/administration/runs.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/db/administration/utils.py` & `haupt-2.0.0rc8/haupt/db/administration/utils.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/db/factories/artifacts.py` & `haupt-2.0.0rc8/haupt/db/factories/artifacts.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/db/factories/runs.py` & `haupt-2.0.0rc8/haupt/db/factories/runs.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/db/factories/users.py` & `haupt-2.0.0rc8/haupt/db/factories/users.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/db/managers/artifacts.py` & `haupt-2.0.0rc8/haupt/db/managers/artifacts.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/db/managers/deleted.py` & `haupt-2.0.0rc8/haupt/db/managers/deleted.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/db/managers/dummy_key.py` & `haupt-2.0.0rc8/haupt/db/managers/dummy_key.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/db/managers/runs.py` & `haupt-2.0.0rc8/haupt/db/managers/runs.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/db/managers/statuses.py` & `haupt-2.0.0rc8/haupt/db/managers/statuses.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # Copyright 2018-2023 Polyaxon, Inc.
 # This file and its contents are licensed under the AGPLv3 License.
 # Please see the included NOTICE for copyright information and
 # LICENSE-AGPL for a copy of the license.
 from typing import Any, List, Optional
 
-from clipped.list_utils import to_list
+from clipped.utils.lists import to_list
 
 from haupt.common import auditor
 from haupt.common.events.registry.run import (
     RUN_DONE,
     RUN_FAILED,
     RUN_NEW_STATUS,
     RUN_RESUMED,
```

### Comparing `haupt-2.0.0rc7/haupt/db/mixins/cache.py` & `haupt-2.0.0rc8/haupt/db/mixins/cache.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/db/mixins/singleton.py` & `haupt-2.0.0rc8/haupt/db/mixins/singleton.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/db/models/artifacts.py` & `haupt-2.0.0rc8/haupt/db/models/artifacts.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/db/pgsql/db/migrations/0001_initial.py` & `haupt-2.0.0rc8/haupt/db/pgsql/db/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/db/pgsql/db/migrations/0002_auto_20200807_1247.py` & `haupt-2.0.0rc8/haupt/db/pgsql/db/migrations/0002_auto_20200807_1247.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/db/pgsql/db/migrations/0003_run_pipeline.py` & `haupt-2.0.0rc8/haupt/db/pgsql/db/migrations/0003_run_pipeline.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/db/pgsql/db/migrations/0004_auto_20200905_1523.py` & `haupt-2.0.0rc8/haupt/db/pgsql/db/migrations/0004_auto_20200905_1523.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/db/pgsql/db/migrations/0005_auto_20201005_0913.py` & `haupt-2.0.0rc8/haupt/db/pgsql/db/migrations/0005_auto_20201005_0913.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/db/pgsql/db/migrations/0006_auto_20201020_1705.py` & `haupt-2.0.0rc8/haupt/db/pgsql/db/migrations/0006_auto_20201020_1705.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/db/pgsql/db/migrations/0007_auto_20201121_1332.py` & `haupt-2.0.0rc8/haupt/db/pgsql/db/migrations/0007_auto_20201121_1332.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/db/pgsql/db/migrations/0008_run_wait_time.py` & `haupt-2.0.0rc8/haupt/db/pgsql/db/migrations/0008_run_wait_time.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/db/pgsql/db/migrations/0009_project_unique_name.py` & `haupt-2.0.0rc8/haupt/db/pgsql/db/migrations/0009_project_unique_name.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/db/pgsql/db/migrations/0010_auto_20210429_1539.py` & `haupt-2.0.0rc8/haupt/db/pgsql/db/migrations/0010_auto_20210429_1539.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/db/pgsql/db/migrations/0011_alter_artifact_state.py` & `haupt-2.0.0rc8/haupt/db/pgsql/db/migrations/0011_alter_artifact_state.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/db/pgsql/db/migrations/0012_alter_artifact_updated_at_and_more.py` & `haupt-2.0.0rc8/haupt/db/pgsql/db/migrations/0012_alter_artifact_updated_at_and_more.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/db/pgsql/db/migrations/0013_alter_artifact_name.py` & `haupt-2.0.0rc8/haupt/db/pgsql/db/migrations/0013_alter_artifact_name.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/db/queries/artifacts.py` & `haupt-2.0.0rc8/haupt/db/queries/artifacts.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/db/queries/runs.py` & `haupt-2.0.0rc8/haupt/db/queries/runs.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/db/query_managers/artifact.py` & `haupt-2.0.0rc8/haupt/db/query_managers/artifact.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/db/query_managers/callback_conditions.py` & `haupt-2.0.0rc8/haupt/db/query_managers/callback_conditions.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 # Copyright 2018-2023 Polyaxon, Inc.
 # This file and its contents are licensed under the AGPLv3 License.
 # Please see the included NOTICE for copyright information and
 # LICENSE-AGPL for a copy of the license.
 
 from typing import Any, Iterable, Optional, Union
 
-from clipped.bool_utils import to_bool
-from clipped.list_utils import to_list
+from clipped.utils.bools import to_bool
+from clipped.utils.lists import to_list
 
 from polyaxon import live_state
 from traceml.artifacts import V1ArtifactKind
 
 
 def archived_condition(
     params: Union[str, Iterable],
```

### Comparing `haupt-2.0.0rc7/haupt/db/query_managers/project.py` & `haupt-2.0.0rc8/haupt/db/query_managers/project.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/db/query_managers/run.py` & `haupt-2.0.0rc8/haupt/db/query_managers/run.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/db/signals/runs.py` & `haupt-2.0.0rc8/haupt/db/signals/runs.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/python
 #
 # Copyright 2018-2023 Polyaxon, Inc.
 # This file and its contents are licensed under the AGPLv3 License.
 # Please see the included NOTICE for copyright information and
 # LICENSE-AGPL for a copy of the license.
 
-from clipped.signal_decorators import ignore_raw, ignore_updates
+from clipped.decorators.signals import ignore_raw, ignore_updates
 from rest_framework.exceptions import ValidationError
 
 from django.db.models.signals import post_save
 from django.dispatch import receiver
 
 from haupt.common import auditor
 from haupt.common.events.registry.run import RUN_CREATED
```

### Comparing `haupt-2.0.0rc7/haupt/db/sqlite/db/migrations/0001_initial.py` & `haupt-2.0.0rc8/haupt/db/sqlite/db/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/main.py` & `haupt-2.0.0rc8/haupt/main.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/managers/proxies.py` & `haupt-2.0.0rc8/haupt/managers/proxies.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # This file and its contents are licensed under the AGPLv3 License.
 # Please see the included NOTICE for copyright information and
 # LICENSE-AGPL for a copy of the license.
 
 import os
 
 from haupt.schemas.proxies_config import ProxiesConfig
-from polyaxon.config_reader.manager import ConfigManager
+from polyaxon.config.manager import ConfigManager
 from polyaxon.managers.base import BaseConfigManager, ManagerVisibility
 
 
 class ProxiesManager(BaseConfigManager):
     """Manages proxies configuration file."""
 
     VISIBILITY = ManagerVisibility.GLOBAL
```

### Comparing `haupt-2.0.0rc7/haupt/managers/sandbox.py` & `haupt-2.0.0rc8/haupt/managers/sandbox.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # This file and its contents are licensed under the AGPLv3 License.
 # Please see the included NOTICE for copyright information and
 # LICENSE-AGPL for a copy of the license.
 
 import os
 
 from haupt.schemas.sandbox_config import SandboxConfig
-from polyaxon.config_reader.manager import ConfigManager
+from polyaxon.config.manager import ConfigManager
 from polyaxon.managers.base import BaseConfigManager, ManagerVisibility
 
 
 class SandboxConfigManager(BaseConfigManager):
     """Manages sandbox configuration .sandbox file."""
 
     VISIBILITY = ManagerVisibility.ALL
```

### Comparing `haupt-2.0.0rc7/haupt/orchestration/executor/__init__.py` & `haupt-2.0.0rc8/haupt/orchestration/executor/__init__.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/orchestration/executor/handlers/run.py` & `haupt-2.0.0rc8/haupt/orchestration/executor/handlers/run.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/orchestration/executor/service.py` & `haupt-2.0.0rc8/haupt/orchestration/executor/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/python
 #
 # Copyright 2018-2023 Polyaxon, Inc.
 # This file and its contents are licensed under the AGPLv3 License.
 # Please see the included NOTICE for copyright information and
 # LICENSE-AGPL for a copy of the license.
 
-from clipped.imports import import_string
+from clipped.utils.imports import import_string
 
 from haupt.common.events.event_service import EventService
 from haupt.common.events.registry import run
 from haupt.orchestration.executor.handlers import run as run_handlers
 from haupt.orchestration.executor.manager import event_manager
```

### Comparing `haupt-2.0.0rc7/haupt/orchestration/executor/subscriptions/run.py` & `haupt-2.0.0rc8/haupt/orchestration/executor/subscriptions/run.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/orchestration/operations/__init__.py` & `haupt-2.0.0rc8/haupt/orchestration/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/orchestration/operations/service.py` & `haupt-2.0.0rc8/haupt/orchestration/operations/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # This file and its contents are licensed under the AGPLv3 License.
 # Please see the included NOTICE for copyright information and
 # LICENSE-AGPL for a copy of the license.
 
 from collections import namedtuple
 from typing import Dict, List, Optional, Set, Tuple, Union
 
-from clipped.list_utils import to_list
+from clipped.utils.lists import to_list
 
 from haupt.common.service_interface import Service
 from haupt.db.abstracts.getter import get_run_model
 from haupt.db.abstracts.runs import BaseRun
 from haupt.db.managers.statuses import new_run_status
 from polyaxon.constants.metadata import (
     META_COPY_ARTIFACTS,
```

### Comparing `haupt-2.0.0rc7/haupt/orchestration/scheduler/manager.py` & `haupt-2.0.0rc8/haupt/orchestration/scheduler/manager.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/orchestration/scheduler/resolver.py` & `haupt-2.0.0rc8/haupt/orchestration/scheduler/resolver.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/polyconf/asgi/sandbox.py` & `haupt-2.0.0rc8/haupt/polyconf/asgi/sandbox.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/polyconf/asgi/server.py` & `haupt-2.0.0rc8/haupt/polyconf/asgi/server.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/polyconf/asgi/streams.py` & `haupt-2.0.0rc8/haupt/polyconf/asgi/streams.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/polyconf/asgi/viewer.py` & `haupt-2.0.0rc8/haupt/polyconf/asgi/viewer.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/polyconf/config_settings/__init__.py` & `haupt-2.0.0rc8/haupt/polyconf/config_settings/__init__.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/polyconf/config_settings/rest.py` & `haupt-2.0.0rc8/haupt/polyconf/config_settings/rest.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/polyconf/wsgi.py` & `haupt-2.0.0rc8/haupt/polyconf/wsgi.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/proxies/generators/api.py` & `haupt-2.0.0rc8/haupt/proxies/generators/api.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/proxies/generators/forward.py` & `haupt-2.0.0rc8/haupt/proxies/generators/forward.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/proxies/generators/gateway.py` & `haupt-2.0.0rc8/haupt/proxies/generators/gateway.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/proxies/generators/streams.py` & `haupt-2.0.0rc8/haupt/proxies/generators/streams.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/proxies/schemas/api/base.py` & `haupt-2.0.0rc8/haupt/proxies/schemas/api/base.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/proxies/schemas/api/uwsgi.py` & `haupt-2.0.0rc8/haupt/proxies/schemas/api/uwsgi.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/proxies/schemas/auth.py` & `haupt-2.0.0rc8/haupt/proxies/schemas/auth.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/proxies/schemas/base.py` & `haupt-2.0.0rc8/haupt/proxies/schemas/base.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/proxies/schemas/dns.py` & `haupt-2.0.0rc8/haupt/proxies/schemas/dns.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/proxies/schemas/error_page.py` & `haupt-2.0.0rc8/haupt/proxies/schemas/error_page.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/proxies/schemas/forward.py` & `haupt-2.0.0rc8/haupt/proxies/schemas/forward.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/proxies/schemas/gateway/api.py` & `haupt-2.0.0rc8/haupt/proxies/schemas/gateway/api.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/proxies/schemas/gateway/base.py` & `haupt-2.0.0rc8/haupt/proxies/schemas/gateway/base.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/proxies/schemas/gateway/healthz.py` & `haupt-2.0.0rc8/haupt/proxies/schemas/gateway/healthz.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/proxies/schemas/gateway/redirect.py` & `haupt-2.0.0rc8/haupt/proxies/schemas/gateway/redirect.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/proxies/schemas/listen.py` & `haupt-2.0.0rc8/haupt/proxies/schemas/listen.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/proxies/schemas/locations.py` & `haupt-2.0.0rc8/haupt/proxies/schemas/locations.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/proxies/schemas/logging.py` & `haupt-2.0.0rc8/haupt/proxies/schemas/logging.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/proxies/schemas/scaffold.py` & `haupt-2.0.0rc8/haupt/proxies/schemas/scaffold.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/proxies/schemas/server.py` & `haupt-2.0.0rc8/haupt/proxies/schemas/server.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/proxies/schemas/services.py` & `haupt-2.0.0rc8/haupt/proxies/schemas/services.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/proxies/schemas/ssl.py` & `haupt-2.0.0rc8/haupt/proxies/schemas/ssl.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/proxies/schemas/streams/api.py` & `haupt-2.0.0rc8/haupt/proxies/schemas/streams/api.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/proxies/schemas/streams/base.py` & `haupt-2.0.0rc8/haupt/proxies/schemas/streams/base.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/proxies/schemas/streams/k8s.py` & `haupt-2.0.0rc8/haupt/proxies/schemas/streams/k8s.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/proxies/schemas/timeout.py` & `haupt-2.0.0rc8/haupt/proxies/schemas/timeout.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/proxies/schemas/urls.py` & `haupt-2.0.0rc8/haupt/proxies/schemas/urls.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/schemas/proxies_config.py` & `haupt-2.0.0rc8/haupt/schemas/proxies_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright 2018-2023 Polyaxon, Inc.
 # This file and its contents are licensed under the AGPLv3 License.
 # Please see the included NOTICE for copyright information and
 # LICENSE-AGPL for a copy of the license.
 from typing import List, Optional
 from typing_extensions import Literal
 
-from clipped.logging_utils import DEFAULT_LOGS_ROOT
+from clipped.utils.logging import DEFAULT_LOGS_ROOT
 from pydantic import Extra, Field, validator
 
 from polyaxon.api import STATIC_V1
 from polyaxon.contexts import paths as ctx_paths
 from polyaxon.env_vars.keys import (
     EV_KEYS_ARCHIVES_ROOT,
     EV_KEYS_DNS_BACKEND,
```

### Comparing `haupt-2.0.0rc7/haupt/schemas/sandbox_config.py` & `haupt-2.0.0rc8/haupt/schemas/sandbox_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # Copyright 2018-2023 Polyaxon, Inc.
 # This file and its contents are licensed under the AGPLv3 License.
 # Please see the included NOTICE for copyright information and
 # LICENSE-AGPL for a copy of the license.
 from typing import Optional
 
-from clipped.http_utils import clean_host
+from clipped.utils.http import clean_host
 from pydantic import Field, StrictInt, StrictStr
 
 from polyaxon.env_vars.keys import (
     EV_KEYS_K8S_NAMESPACE,
     EV_KEYS_SANDBOX_DEBUG,
     EV_KEYS_SANDBOX_HOST,
     EV_KEYS_SANDBOX_IS_LOCAL,
```

### Comparing `haupt-2.0.0rc7/haupt/settings.py` & `haupt-2.0.0rc8/haupt/settings.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/dist/css/global.min.css` & `haupt-2.0.0rc8/haupt/static/dist/css/global.min.css`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/dist/css/global_modal.min.css` & `haupt-2.0.0rc8/haupt/static/dist/css/global_modal.min.css`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/dist/js/0.bundle.js` & `haupt-2.0.0rc8/haupt/static/dist/js/0.bundle.js`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/dist/js/1.bundle.js` & `haupt-2.0.0rc8/haupt/static/dist/js/1.bundle.js`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/dist/js/2.bundle.js` & `haupt-2.0.0rc8/haupt/static/dist/js/2.bundle.js`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/dist/js/3.bundle.js` & `haupt-2.0.0rc8/haupt/static/dist/js/3.bundle.js`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/dist/js/4.bundle.js` & `haupt-2.0.0rc8/haupt/static/dist/js/4.bundle.js`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/dist/js/5.bundle.js` & `haupt-2.0.0rc8/haupt/static/dist/js/5.bundle.js`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/dist/js/6.bundle.js` & `haupt-2.0.0rc8/haupt/static/dist/js/6.bundle.js`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/dist/js/7.bundle.js` & `haupt-2.0.0rc8/haupt/static/dist/js/7.bundle.js`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/errors/404.html` & `haupt-2.0.0rc8/haupt/static/errors/404.html`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/errors/50x.html` & `haupt-2.0.0rc8/haupt/static/errors/50x.html`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/errors/permission.html` & `haupt-2.0.0rc8/haupt/static/errors/permission.html`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/images/403.svg` & `haupt-2.0.0rc8/haupt/static/images/403.svg`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/images/404.svg` & `haupt-2.0.0rc8/haupt/static/images/404.svg`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/images/50x.svg` & `haupt-2.0.0rc8/haupt/static/images/50x.svg`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/images/favicon-danger.ico` & `haupt-2.0.0rc8/haupt/static/images/favicon-danger.ico`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/images/favicon-danger.svg` & `haupt-2.0.0rc8/haupt/static/images/favicon-danger.svg`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/images/favicon-primary.ico` & `haupt-2.0.0rc8/haupt/static/images/favicon-primary.ico`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/images/favicon-primary.svg` & `haupt-2.0.0rc8/haupt/static/images/favicon-primary.svg`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/images/favicon-running.ico` & `haupt-2.0.0rc8/haupt/static/images/favicon-running.ico`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/images/favicon-running.svg` & `haupt-2.0.0rc8/haupt/static/images/favicon-running.svg`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/images/favicon-stopped.ico` & `haupt-2.0.0rc8/haupt/static/images/favicon-stopped.ico`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/images/favicon-stopped.svg` & `haupt-2.0.0rc8/haupt/static/images/favicon-stopped.svg`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/images/favicon-success.ico` & `haupt-2.0.0rc8/haupt/static/images/favicon-success.ico`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/images/favicon-success.svg` & `haupt-2.0.0rc8/haupt/static/images/favicon-success.svg`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/images/favicon-warning.ico` & `haupt-2.0.0rc8/haupt/static/images/favicon-warning.ico`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/images/favicon-warning.svg` & `haupt-2.0.0rc8/haupt/static/images/favicon-warning.svg`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/images/favicon.ico` & `haupt-2.0.0rc8/haupt/static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/images/favicon.svg` & `haupt-2.0.0rc8/haupt/static/images/favicon.svg`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/images/logo_small.png` & `haupt-2.0.0rc8/haupt/static/images/logo_small.png`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/images/logo_white.svg` & `haupt-2.0.0rc8/haupt/static/images/logo_white.svg`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/vendors/fonts/dosis/OFL.txt` & `haupt-2.0.0rc8/haupt/static/vendors/fonts/dosis/OFL.txt`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/vendors/fonts/dosis/dosis-v8-latin-500.eot` & `haupt-2.0.0rc8/haupt/static/vendors/fonts/dosis/dosis-v8-latin-500.eot`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/vendors/fonts/dosis/dosis-v8-latin-500.svg` & `haupt-2.0.0rc8/haupt/static/vendors/fonts/dosis/dosis-v8-latin-500.svg`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/vendors/fonts/dosis/dosis-v8-latin-500.ttf` & `haupt-2.0.0rc8/haupt/static/vendors/fonts/dosis/dosis-v8-latin-500.ttf`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/vendors/fonts/dosis/dosis-v8-latin-500.woff` & `haupt-2.0.0rc8/haupt/static/vendors/fonts/dosis/dosis-v8-latin-500.woff`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/vendors/fonts/dosis/dosis-v8-latin-500.woff2` & `haupt-2.0.0rc8/haupt/static/vendors/fonts/dosis/dosis-v8-latin-500.woff2`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/vendors/fonts/fonts.css` & `haupt-2.0.0rc8/haupt/static/vendors/fonts/fonts.css`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/vendors/fonts/source-code-pro/source-code-pro-v10-latin-regular.eot` & `haupt-2.0.0rc8/haupt/static/vendors/fonts/source-code-pro/source-code-pro-v10-latin-regular.eot`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/vendors/fonts/source-code-pro/source-code-pro-v10-latin-regular.svg` & `haupt-2.0.0rc8/haupt/static/vendors/fonts/source-code-pro/source-code-pro-v10-latin-regular.svg`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/vendors/fonts/source-code-pro/source-code-pro-v10-latin-regular.ttf` & `haupt-2.0.0rc8/haupt/static/vendors/fonts/source-code-pro/source-code-pro-v10-latin-regular.ttf`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/vendors/fonts/source-code-pro/source-code-pro-v10-latin-regular.woff` & `haupt-2.0.0rc8/haupt/static/vendors/fonts/source-code-pro/source-code-pro-v10-latin-regular.woff`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/vendors/fonts/source-code-pro/source-code-pro-v10-latin-regular.woff2` & `haupt-2.0.0rc8/haupt/static/vendors/fonts/source-code-pro/source-code-pro-v10-latin-regular.woff2`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/vendors/fonts/source-sans-pro/OFL.txt` & `haupt-2.0.0rc8/haupt/static/vendors/fonts/source-sans-pro/OFL.txt`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-300.eot` & `haupt-2.0.0rc8/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-300.eot`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-300.svg` & `haupt-2.0.0rc8/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-300.svg`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-300.ttf` & `haupt-2.0.0rc8/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-300.ttf`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-300.woff` & `haupt-2.0.0rc8/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-300.woff`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-300.woff2` & `haupt-2.0.0rc8/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-300.woff2`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-600.eot` & `haupt-2.0.0rc8/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-600.eot`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-600.svg` & `haupt-2.0.0rc8/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-600.svg`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-600.ttf` & `haupt-2.0.0rc8/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-600.ttf`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-600.woff` & `haupt-2.0.0rc8/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-600.woff`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-600.woff2` & `haupt-2.0.0rc8/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-600.woff2`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-regular.eot` & `haupt-2.0.0rc8/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-regular.eot`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-regular.svg` & `haupt-2.0.0rc8/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-regular.svg`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-regular.ttf` & `haupt-2.0.0rc8/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-regular.ttf`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-regular.woff` & `haupt-2.0.0rc8/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-regular.woff`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-regular.woff2` & `haupt-2.0.0rc8/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-regular.woff2`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/vendors/js/bokeh.3.0.3.min.js` & `haupt-2.0.0rc8/haupt/static/vendors/js/bokeh.3.0.3.min.js`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/vendors/js/create-plotly-component.2.6.0.min.js` & `haupt-2.0.0rc8/haupt/static/vendors/js/create-plotly-component.2.6.0.min.js`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/vendors/js/highlight.10.1.2.min.js` & `haupt-2.0.0rc8/haupt/static/vendors/js/highlight.10.1.2.min.js`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/vendors/js/moment-timezone.0.5.32.min.js` & `haupt-2.0.0rc8/haupt/static/vendors/js/moment-timezone.0.5.32.min.js`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/vendors/js/moment.2.29.3.min.js` & `haupt-2.0.0rc8/haupt/static/vendors/js/moment.2.29.3.min.js`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/vendors/js/plotly.2.18.2.min.js` & `haupt-2.0.0rc8/haupt/static/vendors/js/plotly.2.18.2.min.js`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/vendors/js/react-dom.production.18.0.2.min.js` & `haupt-2.0.0rc8/haupt/static/vendors/js/react-dom.production.18.0.2.min.js`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/vendors/js/react.production.18.0.2.min.js` & `haupt-2.0.0rc8/haupt/static/vendors/js/react.production.18.0.2.min.js`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/vendors/js/vega-embed@6.min.js` & `haupt-2.0.0rc8/haupt/static/vendors/js/vega-embed@6.min.js`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/vendors/js/vega-lite@4.min.js` & `haupt-2.0.0rc8/haupt/static/vendors/js/vega-lite@4.min.js`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/static/vendors/js/vega@5.min.js` & `haupt-2.0.0rc8/haupt/static/vendors/js/vega@5.min.js`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/streams/apps.py` & `haupt-2.0.0rc8/haupt/streams/apps.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/streams/connections/fs.py` & `haupt-2.0.0rc8/haupt/streams/connections/fs.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/streams/controllers/events.py` & `haupt-2.0.0rc8/haupt/streams/controllers/events.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Please see the included NOTICE for copyright information and
 # LICENSE-AGPL for a copy of the license.
 import logging
 import os
 
 from typing import Dict, List, Optional, Set
 
-import orjson
+from clipped.utils.json import orjson_loads
 
 import aiofiles
 
 from asgiref.sync import sync_to_async
 from polyaxon.fs.async_manager import (
     download_file,
     download_files,
@@ -150,15 +150,15 @@
         to_dict=False,
     )
     if not event:
         logger.warning("During the packaging of %s, the event download failed.")
         return []
     df = event["data"].df
     try:
-        files = df[event_kind].map(lambda f: orjson.loads(f).get("path")).tolist()
+        files = df[event_kind].map(lambda f: orjson_loads(f).get("path")).tolist()
     except Exception as e:
         logger.warning(
             "During the packaging of %s, the event format found was not correct. "
             "Error %s" % (event_path, e)
         )
         return pkg_files
     subpaths = []
```

### Comparing `haupt-2.0.0rc7/haupt/streams/controllers/k8s_check.py` & `haupt-2.0.0rc8/haupt/streams/controllers/k8s_check.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/streams/controllers/k8s_crd.py` & `haupt-2.0.0rc8/haupt/streams/controllers/k8s_crd.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/streams/controllers/k8s_pods.py` & `haupt-2.0.0rc8/haupt/streams/controllers/k8s_pods.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/streams/controllers/logs.py` & `haupt-2.0.0rc8/haupt/streams/controllers/logs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/python
 #
 # Copyright 2018-2023 Polyaxon, Inc.
 # This file and its contents are licensed under the AGPLv3 License.
 # Please see the included NOTICE for copyright information and
 # LICENSE-AGPL for a copy of the license.
-
+import datetime
 import os
 
 from typing import List, Optional, Tuple
 
 import aiofiles
 
 from haupt.streams.tasks.logs import (
@@ -16,15 +16,14 @@
     download_logs_file,
     download_tmp_logs,
 )
 from polyaxon.fs.async_manager import list_files
 from polyaxon.fs.types import FSSystem
 from polyaxon.k8s.async_manager import AsyncK8SManager
 from polyaxon.k8s.logging.async_monitor import query_k8s_operation_logs
-from polyaxon.types import AwareDT
 from traceml.logging import V1Log
 
 
 async def get_logs_files(fs: FSSystem, run_uuid: str) -> List[str]:
     files = await list_files(fs=fs, subpath="{}/plxlogs".format(run_uuid))
     if not files["files"]:
         return []
@@ -73,16 +72,16 @@
         fs=fs, run_uuid=run_uuid, last_file=last_file, check_cache=check_cache
     )
 
     return logs, last_file, files
 
 
 async def get_tmp_operation_logs(
-    fs: FSSystem, run_uuid: str, last_time: Optional[AwareDT]
-) -> Tuple[List[V1Log], Optional[AwareDT]]:
+    fs: FSSystem, run_uuid: str, last_time: Optional[datetime.datetime]
+) -> Tuple[List[V1Log], Optional[datetime.datetime]]:
     logs = []
 
     tmp_logs = await download_tmp_logs(fs=fs, run_uuid=run_uuid)
 
     if not tmp_logs or not os.path.exists(tmp_logs):
         return logs, None
 
@@ -102,15 +101,15 @@
     return [l.to_dict() for l in logs], last_time
 
 
 async def get_operation_logs(
     k8s_manager: AsyncK8SManager,
     k8s_operation: any,
     instance: str,
-    last_time: Optional[AwareDT],
+    last_time: Optional[datetime.datetime],
 ):
     previous_last = last_time
     operation_logs, last_time = await query_k8s_operation_logs(
         instance=instance,
         last_time=None,
         k8s_manager=k8s_manager,
         stream=True,
```

### Comparing `haupt-2.0.0rc7/haupt/streams/controllers/notebooks.py` & `haupt-2.0.0rc8/haupt/streams/controllers/notebooks.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/streams/controllers/uploads.py` & `haupt-2.0.0rc8/haupt/streams/controllers/uploads.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,16 @@
 #
 # Copyright 2018-2023 Polyaxon, Inc.
 # This file and its contents are licensed under the AGPLv3 License.
 # Please see the included NOTICE for copyright information and
 # LICENSE-AGPL for a copy of the license.
 import os
 
-import orjson
-
-from clipped.path_utils import check_or_create_path, delete_path, untar_file
+from clipped.utils.json import orjson_loads
+from clipped.utils.paths import check_or_create_path, delete_path, untar_file
 from rest_framework import status
 
 from django.core.handlers.asgi import ASGIRequest
 from django.http import HttpResponse
 
 from asgiref.sync import sync_to_async
 from polyaxon import settings
@@ -83,15 +82,15 @@
 
 
 async def handle_upload(
     fs: FSSystem, request: ASGIRequest, run_uuid: str, is_file: bool
 ) -> HttpResponse:
     content_file = request.FILES["upload_file"]
     content_json = request.POST.get("json")
-    content_json = orjson.loads(content_json) if content_json else {}
+    content_json = orjson_loads(content_json) if content_json else {}
     overwrite = content_json.get("overwrite", True)
     untar = content_json.get("untar", True)
     path = content_json.get("path", "")
     try:
         archived_path = await handle_posted_data(
             fs=fs,
             content_file=content_file,
```

### Comparing `haupt-2.0.0rc7/haupt/streams/endpoints/artifacts.py` & `haupt-2.0.0rc8/haupt/streams/endpoints/artifacts.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # Copyright 2018-2023 Polyaxon, Inc.
 # This file and its contents are licensed under the AGPLv3 License.
 # Please see the included NOTICE for copyright information and
 # LICENSE-AGPL for a copy of the license.
 from typing import Dict, Optional, Union
 
-from clipped.bool_utils import to_bool
+from clipped.utils.bools import to_bool
 from rest_framework import status
 
 from django.core.handlers.asgi import ASGIRequest
 from django.db import transaction
 from django.http import FileResponse, HttpResponse
 from django.urls import path
```

### Comparing `haupt-2.0.0rc7/haupt/streams/endpoints/auth_request.py` & `haupt-2.0.0rc8/haupt/streams/endpoints/auth_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,21 +5,19 @@
 # Please see the included NOTICE for copyright information and
 # LICENSE-AGPL for a copy of the license.
 import logging
 import os
 
 from typing import Dict, Optional
 
-import orjson
-
-from clipped.date_utils import DateTimeFormatter
-from clipped.hashing import hash_value
-from clipped.json_utils import orjson_dumps
-from clipped.path_utils import check_or_create_path
-from clipped.tz_utils import now
+from clipped.utils.dates import DateTimeFormatter
+from clipped.utils.hashing import hash_value
+from clipped.utils.json import orjson_dumps, orjson_loads
+from clipped.utils.paths import check_or_create_path
+from clipped.utils.tz import now
 from rest_framework import status
 
 from django.core.handlers.asgi import ASGIRequest
 from django.db import transaction
 from django.http import HttpResponse
 from django.urls import path
 
@@ -49,15 +47,15 @@
 
 
 async def _check_auth_cache(request_cache: str) -> bool:
     cache_path = _get_auth_cache_path(request_cache)
     if os.path.isfile(cache_path):
         try:
             async with aiofiles.open(cache_path, mode="r") as f:
-                last_value = orjson.loads(await f.read())
+                last_value = orjson_loads(await f.read())
                 last_time = DateTimeFormatter.extract_timestamp(
                     last_value["time"],
                     dt_format=DateTimeFormatter.DATETIME_FORMAT,
                     timezone=settings.CLIENT_CONFIG.timezone,
                     force_tz=True,
                 )
                 interval = 60 if last_value["response"] else 30
```

### Comparing `haupt-2.0.0rc7/haupt/streams/endpoints/base.py` & `haupt-2.0.0rc8/haupt/streams/endpoints/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/python
 #
 # Copyright 2018-2023 Polyaxon, Inc.
 # This file and its contents are licensed under the AGPLv3 License.
 # Please see the included NOTICE for copyright information and
 # LICENSE-AGPL for a copy of the license.
 
-from clipped.json_utils import orjson_dumps
+from clipped.utils.json import orjson_dumps
 from rest_framework import status
 
 from django.core.handlers.asgi import ASGIRequest
 from django.http import HttpResponse
 from django.urls import re_path
```

### Comparing `haupt-2.0.0rc7/haupt/streams/endpoints/events.py` & `haupt-2.0.0rc8/haupt/streams/endpoints/events.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright 2018-2023 Polyaxon, Inc.
 # This file and its contents are licensed under the AGPLv3 License.
 # Please see the included NOTICE for copyright information and
 # LICENSE-AGPL for a copy of the license.
 
 from typing import Dict, Optional, Set, Union
 
-from clipped.bool_utils import to_bool
+from clipped.utils.bools import to_bool
 from rest_framework import status
 
 from django.core.handlers.asgi import ASGIRequest
 from django.db import transaction
 from django.http import HttpResponse
 from django.urls import path
```

### Comparing `haupt-2.0.0rc7/haupt/streams/endpoints/k8s.py` & `haupt-2.0.0rc8/haupt/streams/endpoints/k8s.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/streams/endpoints/local_sandbox.py` & `haupt-2.0.0rc8/haupt/streams/endpoints/local_sandbox.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/streams/endpoints/logs.py` & `haupt-2.0.0rc8/haupt/streams/endpoints/logs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 # This file and its contents are licensed under the AGPLv3 License.
 # Please see the included NOTICE for copyright information and
 # LICENSE-AGPL for a copy of the license.
 import logging
 
 from typing import Dict, Optional
 
-from clipped.bool_utils import to_bool
-from clipped.date_utils import parse_datetime
-from clipped.serialization import datetime_serialize
+from clipped.utils.bools import to_bool
+from clipped.utils.dates import parse_datetime
+from clipped.utils.serialization import datetime_serialize
 from rest_framework import status
 
 from django.core.handlers.asgi import ASGIRequest
 from django.db import transaction
 from django.http import HttpResponse
 from django.urls import path
```

### Comparing `haupt-2.0.0rc7/haupt/streams/endpoints/notifications.py` & `haupt-2.0.0rc8/haupt/streams/endpoints/notifications.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 # This file and its contents are licensed under the AGPLv3 License.
 # Please see the included NOTICE for copyright information and
 # LICENSE-AGPL for a copy of the license.
 import logging
 
 from typing import Dict, Optional
 
-import orjson
-
+from clipped.utils.json import orjson_loads
 from rest_framework import status
 
 from django.core.handlers.asgi import ASGIRequest
 from django.db import transaction
 from django.http import HttpResponse
 from django.urls import path
 
@@ -32,15 +31,15 @@
     namespace: str,
     owner: str,
     project: str,
     run_uuid: str,
     methods: Optional[Dict] = None,
 ) -> HttpResponse:
     validate_methods(request, methods)
-    body = orjson.loads(request.body)
+    body = orjson_loads(request.body)
     run_name = body.get("name")
     condition = body.get("condition")
     if not condition:
         errors = "Received a notification request without condition."
         logger.warning(errors)
         return UJSONResponse(
             data={"errors": errors},
```

### Comparing `haupt-2.0.0rc7/haupt/streams/endpoints/utils.py` & `haupt-2.0.0rc8/haupt/streams/endpoints/utils.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/streams/patterns.py` & `haupt-2.0.0rc8/haupt/streams/patterns.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt/streams/tasks/logs.py` & `haupt-2.0.0rc8/haupt/streams/tasks/logs.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 # Copyright 2018-2023 Polyaxon, Inc.
 # This file and its contents are licensed under the AGPLv3 License.
 # Please see the included NOTICE for copyright information and
 # LICENSE-AGPL for a copy of the license.
 from datetime import datetime
 from typing import List
 
-import orjson
-
-from clipped.path_utils import delete_path
+from clipped.utils.json import orjson_loads
+from clipped.utils.paths import delete_path
 
 from django.core.exceptions import BadRequest
 
 from asgiref.sync import sync_to_async
 from polyaxon import settings
 from polyaxon.fs.async_manager import (
     delete_file_or_dir,
@@ -55,16 +54,16 @@
         return []
 
     @sync_to_async
     def convert():
         # Version handling
         if ".plx" in logs_path:
             return V1Logs.read_csv(content).logs
-        # Legacy logs
-        return orjson.loads(content).get("logs", [])
+        # Chunked logs
+        return orjson_loads(content).get("logs", [])
 
     return await convert()
 
 
 async def download_logs_file(
     fs: FSSystem, run_uuid: str, last_file: str, check_cache: bool = True
 ) -> (str, str):
```

### Comparing `haupt-2.0.0rc7/haupt/streams/tasks/notification.py` & `haupt-2.0.0rc8/haupt/streams/tasks/notification.py`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/haupt.egg-info/PKG-INFO` & `haupt-2.0.0rc8/haupt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haupt
-Version: 2.0.0rc7
+Version: 2.0.0rc8
 Summary: Lineage metadata API, artifacts streams, sandbox, ML-API, and spaces for Polyaxon.
 Home-page: https://github.com/polyaxon/haupt
 Author: Polyaxon, Inc.
 Author-email: contact@polyaxon.com
 Maintainer: Polyaxon, Inc.
 Maintainer-email: contact@polyaxon.com
 License: AGPLv3
```

### Comparing `haupt-2.0.0rc7/haupt.egg-info/SOURCES.txt` & `haupt-2.0.0rc8/haupt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/setup.cfg` & `haupt-2.0.0rc8/setup.cfg`

 * *Files identical despite different names*

### Comparing `haupt-2.0.0rc7/setup.py` & `haupt-2.0.0rc8/setup.py`

 * *Files identical despite different names*

