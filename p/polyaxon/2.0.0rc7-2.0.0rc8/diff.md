# Comparing `tmp/polyaxon-2.0.0rc7.tar.gz` & `tmp/polyaxon-2.0.0rc8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyaxon-2.0.0rc7.tar", last modified: Wed Apr 12 14:22:01 2023, max compression
+gzip compressed data, was "polyaxon-2.0.0rc8.tar", last modified: Sun Apr 16 12:03:59 2023, max compression
```

## Comparing `polyaxon-2.0.0rc7.tar` & `polyaxon-2.0.0rc8.tar`

### file list

```diff
@@ -1,748 +1,733 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.112076 polyaxon-2.0.0rc7/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10054 2023-04-12 14:22:01.112076 polyaxon-2.0.0rc7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.056076 polyaxon-2.0.0rc7/polyaxon/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.060076 polyaxon-2.0.0rc7/polyaxon/agents/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/agents/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    16634 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/agents/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/agents/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/agents/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.060076 polyaxon-2.0.0rc7/polyaxon/agents/spawners/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/agents/spawners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/agents/spawners/async_spawner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/agents/spawners/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/agents/spawners/spawner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.060076 polyaxon-2.0.0rc7/polyaxon/auxiliaries/
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/auxiliaries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/auxiliaries/cleaner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/auxiliaries/default_scheduling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/auxiliaries/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     6387 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/auxiliaries/notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/auxiliaries/sidecar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/auxiliaries/tuner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.060076 polyaxon-2.0.0rc7/polyaxon/builds/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/builds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9202 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/builds/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.060076 polyaxon-2.0.0rc7/polyaxon/builds/generator/
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/builds/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/builds/generator/dockerfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/builds/generator/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.060076 polyaxon-2.0.0rc7/polyaxon/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9423 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/cli/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)    16965 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/cli/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/cli/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/cli/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/cli/completion.py
--rw-r--r--   0 runner    (1001) docker     (123)    18387 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/cli/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/cli/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/cli/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.060076 polyaxon-2.0.0rc7/polyaxon/cli/executor/
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/cli/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/cli/executor/conda.py
--rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/cli/executor/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/cli/executor/k8s.py
--rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/cli/executor/platform.py
--rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/cli/init.py
--rw-r--r--   0 runner    (1001) docker     (123)    16604 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/cli/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    62005 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/cli/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/cli/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/cli/port_forward.py
--rw-r--r--   0 runner    (1001) docker     (123)    17141 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/cli/project_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12230 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/cli/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)    12689 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/cli/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.064076 polyaxon-2.0.0rc7/polyaxon/cli/services/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/cli/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/cli/services/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/cli/services/clean_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/cli/services/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)    10332 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/cli/services/initializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/cli/services/notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/cli/services/sidecar.py
--rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/cli/services/tuner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/cli/services/wait.py
--rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/cli/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.064076 polyaxon-2.0.0rc7/polyaxon/client/
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.064076 polyaxon-2.0.0rc7/polyaxon/client/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/client/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/client/decorators/client_call_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/client/decorators/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/client/decorators/is_managed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/client/impersonate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/client/init.py
--rw-r--r--   0 runner    (1001) docker     (123)    58660 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/client/project.py
--rw-r--r--   0 runner    (1001) docker     (123)   108175 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/client/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.064076 polyaxon-2.0.0rc7/polyaxon/client/transport/
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/client/transport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/client/transport/http_transport.py
--rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/client/transport/periodic_transport.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/client/transport/retry_transport.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/client/transport/socket_transport.py
--rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/client/transport/threaded_transport.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/client/transport/ws_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.064076 polyaxon-2.0.0rc7/polyaxon/client/workers/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/client/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/client/workers/base_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/client/workers/periodic_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/client/workers/queue_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.064076 polyaxon-2.0.0rc7/polyaxon/config_reader/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/config_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13126 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/config_reader/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     9758 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/config_reader/spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.064076 polyaxon-2.0.0rc7/polyaxon/connections/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/connections/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.064076 polyaxon-2.0.0rc7/polyaxon/connections/aws/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/connections/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/connections/aws/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7381 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/connections/aws/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.064076 polyaxon-2.0.0rc7/polyaxon/connections/azure/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/connections/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/connections/azure/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/connections/azure/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/connections/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.064076 polyaxon-2.0.0rc7/polyaxon/connections/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/connections/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/connections/gcp/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/connections/gcp/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/connections/kinds.py
--rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/connections/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.068076 polyaxon-2.0.0rc7/polyaxon/connections/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/connections/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/connections/schemas/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/connections/schemas/k8s_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.068076 polyaxon-2.0.0rc7/polyaxon/constants/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/constants/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/constants/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.068076 polyaxon-2.0.0rc7/polyaxon/containers/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/containers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/containers/names.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/containers/pull_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/containers/statuses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.068076 polyaxon-2.0.0rc7/polyaxon/contexts/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/contexts/keys.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/contexts/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/contexts/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/contexts/refs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/contexts/sections.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.068076 polyaxon-2.0.0rc7/polyaxon/deploy/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/deploy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.068076 polyaxon-2.0.0rc7/polyaxon/deploy/operators/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/deploy/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/deploy/operators/cmd_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/deploy/operators/compose.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/deploy/operators/conda.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/deploy/operators/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/deploy/operators/helm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/deploy/operators/kubectl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/deploy/operators/pip.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/deploy/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.068076 polyaxon-2.0.0rc7/polyaxon/deploy/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/deploy/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/deploy/schemas/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/deploy/schemas/celery.py
--rw-r--r--   0 runner    (1001) docker     (123)    13189 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/deploy/schemas/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/deploy/schemas/deployment_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/deploy/schemas/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/deploy/schemas/ingress.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/deploy/schemas/intervals.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/deploy/schemas/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/deploy/schemas/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/deploy/schemas/rbac.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/deploy/schemas/root_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/deploy/schemas/security_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/deploy/schemas/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/deploy/schemas/service_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/deploy/schemas/ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/deploy/schemas/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/dist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.068076 polyaxon-2.0.0rc7/polyaxon/env_vars/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/env_vars/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.072076 polyaxon-2.0.0rc7/polyaxon/env_vars/getters/
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/env_vars/getters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/env_vars/getters/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/env_vars/getters/owner_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/env_vars/getters/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/env_vars/getters/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/env_vars/getters/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/env_vars/getters/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/env_vars/getters/versioned_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/env_vars/keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.072076 polyaxon-2.0.0rc7/polyaxon/fs/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/fs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11138 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/fs/async_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/fs/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/fs/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/fs/gcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/fs/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/fs/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/fs/tar.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/fs/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/fs/watcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.072076 polyaxon-2.0.0rc7/polyaxon/init/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/init/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/init/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/init/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/init/dockerfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/init/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/init/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/init/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.072076 polyaxon-2.0.0rc7/polyaxon/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9513 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/k8s/async_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/k8s/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.072076 polyaxon-2.0.0rc7/polyaxon/k8s/custom_resources/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/k8s/custom_resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/k8s/custom_resources/crd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/k8s/custom_resources/operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/k8s/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/k8s/k8s_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/k8s/k8s_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.072076 polyaxon-2.0.0rc7/polyaxon/k8s/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/k8s/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/k8s/logging/async_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/k8s/logging/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    27030 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/k8s/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/k8s/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/k8s/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/k8s/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/k8s/pods.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/k8s/run_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    11533 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/lifecycle.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/live_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/logger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6167 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.076076 polyaxon-2.0.0rc7/polyaxon/managers/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/managers/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/managers/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     8853 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/managers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/managers/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/managers/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/managers/compose.py
--rw-r--r--   0 runner    (1001) docker     (123)    14583 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/managers/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/managers/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/managers/home.py
--rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/managers/ignore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/managers/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/managers/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/managers/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.076076 polyaxon-2.0.0rc7/polyaxon/notifiers/
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/notifiers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/notifiers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/notifiers/discord_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/notifiers/hipchat_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/notifiers/keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/notifiers/mattermost_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/notifiers/pagerduty_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/notifiers/slack_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/notifiers/spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/notifiers/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.076076 polyaxon-2.0.0rc7/polyaxon/operations/
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/operations/cleaner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/operations/notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/operations/tuner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.076076 polyaxon-2.0.0rc7/polyaxon/parser/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/parser/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    40787 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/parser/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/pkg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.076076 polyaxon-2.0.0rc7/polyaxon/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/plugins/sentry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.076076 polyaxon-2.0.0rc7/polyaxon/polyaxonfile/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyaxonfile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9818 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyaxonfile/check.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.076076 polyaxon-2.0.0rc7/polyaxon/polyaxonfile/manager/
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyaxonfile/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyaxonfile/manager/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyaxonfile/manager/workflows.py
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyaxonfile/params.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.076076 polyaxon-2.0.0rc7/polyaxon/polyaxonfile/specs/
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyaxonfile/specs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyaxonfile/specs/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    34545 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyaxonfile/specs/compiled_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyaxonfile/specs/component.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyaxonfile/specs/kinds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.076076 polyaxon-2.0.0rc7/polyaxon/polyaxonfile/specs/libs/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyaxonfile/specs/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyaxonfile/specs/libs/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyaxonfile/specs/libs/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyaxonfile/specs/libs/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyaxonfile/specs/operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyaxonfile/specs/sections.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.080076 polyaxon-2.0.0rc7/polyaxon/polyboard/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyboard/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyboard/events.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyboard/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.080076 polyaxon-2.0.0rc7/polyaxon/polyflow/
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.080076 polyaxon-2.0.0rc7/polyaxon/polyflow/builds/
--rw-r--r--   0 runner    (1001) docker     (123)     7345 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/builds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.080076 polyaxon-2.0.0rc7/polyaxon/polyflow/cache/
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/cache/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.080076 polyaxon-2.0.0rc7/polyaxon/polyflow/component/
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/component/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12553 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/component/component.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/component/component_reference.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.080076 polyaxon-2.0.0rc7/polyaxon/polyflow/containers/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/containers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/containers/container.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.080076 polyaxon-2.0.0rc7/polyaxon/polyflow/dags/
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/dags/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.080076 polyaxon-2.0.0rc7/polyaxon/polyflow/early_stopping/
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/early_stopping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7133 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/early_stopping/policies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.080076 polyaxon-2.0.0rc7/polyaxon/polyflow/environment/
--rw-r--r--   0 runner    (1001) docker     (123)    15301 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/environment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.080076 polyaxon-2.0.0rc7/polyaxon/polyflow/events/
--rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/events/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.080076 polyaxon-2.0.0rc7/polyaxon/polyflow/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/hooks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.080076 polyaxon-2.0.0rc7/polyaxon/polyflow/init/
--rw-r--r--   0 runner    (1001) docker     (123)    11450 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/init/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.080076 polyaxon-2.0.0rc7/polyaxon/polyflow/io/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15956 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/io/io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.080076 polyaxon-2.0.0rc7/polyaxon/polyflow/joins/
--rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/joins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.080076 polyaxon-2.0.0rc7/polyaxon/polyflow/matrix/
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/matrix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/matrix/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    14534 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/matrix/bayes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/matrix/grid_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/matrix/hyperband.py
--rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/matrix/hyperopt.py
--rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/matrix/iterative.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/matrix/kinds.py
--rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/matrix/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    27049 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/matrix/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/matrix/random_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/matrix/tuner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.080076 polyaxon-2.0.0rc7/polyaxon/polyflow/mounts/
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/mounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/mounts/artifacts_mounts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.080076 polyaxon-2.0.0rc7/polyaxon/polyflow/notifications/
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/notifications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.080076 polyaxon-2.0.0rc7/polyaxon/polyflow/operations/
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/operations/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/operations/compiled_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)    23776 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/operations/operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.080076 polyaxon-2.0.0rc7/polyaxon/polyflow/optimization/
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/optimization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.084076 polyaxon-2.0.0rc7/polyaxon/polyflow/params/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/params/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12382 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/params/ops_params.py
--rw-r--r--   0 runner    (1001) docker     (123)    19135 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/params/params.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.084076 polyaxon-2.0.0rc7/polyaxon/polyflow/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     9323 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.084076 polyaxon-2.0.0rc7/polyaxon/polyflow/references/
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/references/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/references/dag.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/references/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/references/mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/references/path.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/references/url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.084076 polyaxon-2.0.0rc7/polyaxon/polyflow/run/
--rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/run/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/run/cleaner.py
--rw-r--r--   0 runner    (1001) docker     (123)    23693 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/run/dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     9497 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/run/dask.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/run/flink.py
--rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/run/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/run/kinds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.084076 polyaxon-2.0.0rc7/polyaxon/polyflow/run/kubeflow/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/run/kubeflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/run/kubeflow/clean_pod_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/run/kubeflow/mpi_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     9391 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/run/kubeflow/mx_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/run/kubeflow/paddle_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/run/kubeflow/pytorch_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/run/kubeflow/replica.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/run/kubeflow/scheduling_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/run/kubeflow/tf_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/run/kubeflow/xgboost_job.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/run/notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/run/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/run/ray.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/run/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    10132 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/run/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.084076 polyaxon-2.0.0rc7/polyaxon/polyflow/run/spark/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/run/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/run/spark/replica.py
--rw-r--r--   0 runner    (1001) docker     (123)     8732 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/run/spark/spark.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/run/tuner.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/run/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.084076 polyaxon-2.0.0rc7/polyaxon/polyflow/schedules/
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/schedules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/schedules/cron.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/schedules/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/schedules/interval.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/schedules/kinds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.084076 polyaxon-2.0.0rc7/polyaxon/polyflow/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.084076 polyaxon-2.0.0rc7/polyaxon/polyflow/termination/
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/termination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyflow/trigger_policies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.084076 polyaxon-2.0.0rc7/polyaxon/polyplot/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polyplot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.084076 polyaxon-2.0.0rc7/polyaxon/polypod/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.088076 polyaxon-2.0.0rc7/polyaxon/polypod/common/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/common/accelerators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/common/annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/common/container_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4322 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/common/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12347 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/common/env_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/common/mounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/common/setter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/common/stores.py
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/common/volumes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.088076 polyaxon-2.0.0rc7/polyaxon/polypod/compiler/
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/compiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/compiler/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.088076 polyaxon-2.0.0rc7/polyaxon/polypod/compiler/contexts/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/compiler/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/compiler/contexts/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7030 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/compiler/contexts/contexts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/compiler/contexts/job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.088076 polyaxon-2.0.0rc7/polyaxon/polypod/compiler/contexts/kubeflow/
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/compiler/contexts/kubeflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/compiler/contexts/kubeflow/mpi_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/compiler/contexts/kubeflow/mx_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/compiler/contexts/kubeflow/paddle_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/compiler/contexts/kubeflow/pytroch_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/compiler/contexts/kubeflow/tf_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/compiler/contexts/kubeflow/xgb_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/compiler/contexts/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/compiler/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.088076 polyaxon-2.0.0rc7/polyaxon/polypod/compiler/converters/
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/compiler/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30602 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/compiler/converters/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/compiler/converters/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/compiler/converters/job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.088076 polyaxon-2.0.0rc7/polyaxon/polypod/compiler/converters/kubeflow/
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/compiler/converters/kubeflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/compiler/converters/kubeflow/mpi_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/compiler/converters/kubeflow/mx_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/compiler/converters/kubeflow/paddle_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/compiler/converters/kubeflow/pytroch_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/compiler/converters/kubeflow/tf_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/compiler/converters/kubeflow/xgboost_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/compiler/converters/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.088076 polyaxon-2.0.0rc7/polyaxon/polypod/compiler/lineage/
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/compiler/lineage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/compiler/lineage/artifacts_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/compiler/lineage/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/compiler/lineage/io_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/compiler/lineage/params_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.088076 polyaxon-2.0.0rc7/polyaxon/polypod/compiler/resolver/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/compiler/resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10334 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/compiler/resolver/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/compiler/resolver/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.088076 polyaxon-2.0.0rc7/polyaxon/polypod/custom_resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/custom_resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/custom_resources/job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.092076 polyaxon-2.0.0rc7/polyaxon/polypod/custom_resources/kubeflow/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/custom_resources/kubeflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/custom_resources/kubeflow/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/custom_resources/kubeflow/mpi_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/custom_resources/kubeflow/mx_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/custom_resources/kubeflow/paddle_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/custom_resources/kubeflow/pytorch_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/custom_resources/kubeflow/tf_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/custom_resources/kubeflow/xgb_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/custom_resources/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.092076 polyaxon-2.0.0rc7/polyaxon/polypod/init/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/init/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/init/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/init/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/init/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/init/dockerfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/init/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/init/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     9973 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/init/store.py
--rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/init/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.092076 polyaxon-2.0.0rc7/polyaxon/polypod/main/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/main/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/main/env_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/main/k8s_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/main/volumes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.092076 polyaxon-2.0.0rc7/polyaxon/polypod/pod/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/pod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/pod/spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/pod/volumes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.092076 polyaxon-2.0.0rc7/polyaxon/polypod/sidecar/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/sidecar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/sidecar/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/sidecar/env_vars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.092076 polyaxon-2.0.0rc7/polyaxon/polypod/specs/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/specs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/specs/contexts.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polypod/specs/replica.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.092076 polyaxon-2.0.0rc7/polyaxon/polytune/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polytune/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.092076 polyaxon-2.0.0rc7/polyaxon/polytune/search_managers/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polytune/search_managers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.092076 polyaxon-2.0.0rc7/polyaxon/polytune/search_managers/bayesian_optimization/
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polytune/search_managers/bayesian_optimization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.092076 polyaxon-2.0.0rc7/polyaxon/polytune/search_managers/grid_search/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polytune/search_managers/grid_search/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.092076 polyaxon-2.0.0rc7/polyaxon/polytune/search_managers/hyperband/
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polytune/search_managers/hyperband/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.092076 polyaxon-2.0.0rc7/polyaxon/polytune/search_managers/hyperopt/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polytune/search_managers/hyperopt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.092076 polyaxon-2.0.0rc7/polyaxon/polytune/search_managers/mapping/
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polytune/search_managers/mapping/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.092076 polyaxon-2.0.0rc7/polyaxon/polytune/search_managers/random_search/
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/polytune/search_managers/random_search/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.092076 polyaxon-2.0.0rc7/polyaxon/pql/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/pql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17927 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/pql/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/pql/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    14513 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/pql/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.096076 polyaxon-2.0.0rc7/polyaxon/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.096076 polyaxon-2.0.0rc7/polyaxon/schemas/api/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/api/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/api/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/api/home.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/api/installation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/api/log_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/api/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/api/user.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/api/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    15349 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.096076 polyaxon-2.0.0rc7/polyaxon/schemas/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11028 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/cli/agent_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/cli/checks_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/cli/cli_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7848 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/cli/client_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.096076 polyaxon-2.0.0rc7/polyaxon/schemas/fields/
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/fields/docker_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/fields/email.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/fields/number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/fields/ref_or_obj.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/fields/uuids.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/patch_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/pending.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.100076 polyaxon-2.0.0rc7/polyaxon/schemas/responses/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_activity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_agent_state_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_agent_state_response_agent_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_agent_status_body_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_analytics_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_artifact_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_cloning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_connection_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_dashboard_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_entities_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_entities_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_entity_notification_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_entity_stage_body_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_entity_status_body_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_events_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_list_activities_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_list_agents_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_list_bookmarks_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_list_connections_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_list_dashboards_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_list_organization_members_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_list_organizations_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_list_presets_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_list_project_versions_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_list_projects_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_list_queues_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_list_run_artifacts_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_list_run_connections_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_list_run_edges_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_list_runs_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_list_searches_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_list_service_accounts_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_list_tags_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_list_team_members_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_list_teams_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_list_token_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_operation_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_organization_member.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_password_change.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_preset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_project_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_project_user_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_project_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_run.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_run_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_run_edge.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_run_reference_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_run_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_search_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_section_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_service_account.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_settings_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_team.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_team_member.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_team_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_trial_start.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_user_email.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_user_singup.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_uuids.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/services.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.104076 polyaxon-2.0.0rc7/polyaxon/schemas/types/
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5570 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/types/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/types/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/types/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13572 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/types/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/types/dockerfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/types/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/types/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/types/gcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/types/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/types/k8s_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/types/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/types/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/types/uri.py
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/schemas/types/wasb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.104076 polyaxon-2.0.0rc7/polyaxon/sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.108076 polyaxon-2.0.0rc7/polyaxon/sdk/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/sdk/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   111064 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/sdk/api/agents_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8995 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/sdk/api/artifacts_stores_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    36422 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/sdk/api/auth_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    54976 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/sdk/api/connections_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    54413 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/sdk/api/dashboards_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   277371 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/sdk/api/organizations_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    55532 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/sdk/api/presets_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    66019 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/sdk/api/project_dashboards_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    65660 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/sdk/api/project_searches_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   245065 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/sdk/api/projects_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    77685 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/sdk/api/queues_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   489214 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/sdk/api/runs_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    53886 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/sdk/api/searches_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   101617 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/sdk/api/service_accounts_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    60519 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/sdk/api/tags_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    99633 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/sdk/api/teams_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    73259 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/sdk/api/users_v1_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19041 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/sdk/api/versions_v1_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.108076 polyaxon-2.0.0rc7/polyaxon/sdk/async_client/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/sdk/async_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7357 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/sdk/async_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9814 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/sdk/async_client/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/sdk/base_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    15722 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/sdk/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4776 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/sdk/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/sdk/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.108076 polyaxon-2.0.0rc7/polyaxon/sdk/sync_client/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/sdk/sync_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29097 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/sdk/sync_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13225 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/sdk/sync_client/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.108076 polyaxon-2.0.0rc7/polyaxon/services/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/services/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/services/ephemeral.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/services/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/services/values.py
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.108076 polyaxon-2.0.0rc7/polyaxon/sidecar/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/sidecar/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.108076 polyaxon-2.0.0rc7/polyaxon/sidecar/container/
--rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/sidecar/container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/sidecar/container/intervals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.108076 polyaxon-2.0.0rc7/polyaxon/sidecar/container/monitors/
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/sidecar/container/monitors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/sidecar/container/monitors/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/sidecar/container/monitors/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/sidecar/ignore.py
--rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/sidecar/processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.108076 polyaxon-2.0.0rc7/polyaxon/stores/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/stores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/stores/polyaxon_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.108076 polyaxon-2.0.0rc7/polyaxon/tracking/
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/tracking/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.108076 polyaxon-2.0.0rc7/polyaxon/tracking/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/tracking/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/tracking/contrib/fastai.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/tracking/contrib/fastai_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/tracking/contrib/hugging_face.py
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/tracking/contrib/ignite.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/tracking/contrib/keras.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/tracking/contrib/lightgbm.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/tracking/contrib/pytorch_lightning.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/tracking/contrib/scikit.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/tracking/contrib/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/tracking/contrib/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/tracking/contrib/xgboost.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/tracking/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.112076 polyaxon-2.0.0rc7/polyaxon/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/utils/cli_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.112076 polyaxon-2.0.0rc7/polyaxon/utils/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/utils/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/utils/fixtures/backfill.py
--rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/utils/fixtures/bo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/utils/fixtures/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/utils/fixtures/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     9711 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/utils/fixtures/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/utils/fixtures/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    22732 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/utils/fixtures/pipelines.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/utils/fixtures/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/utils/fixtures/services.py
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/utils/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/utils/fqn_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/utils/host_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7192 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/utils/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/utils/urls_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.112076 polyaxon-2.0.0rc7/polyaxon/vendor/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/vendor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon/vendor/shell_pty.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.056076 polyaxon-2.0.0rc7/polyaxon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10054 2023-04-12 14:22:00.000000 polyaxon-2.0.0rc7/polyaxon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23047 2023-04-12 14:22:01.000000 polyaxon-2.0.0rc7/polyaxon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 14:22:00.000000 polyaxon-2.0.0rc7/polyaxon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-12 14:22:00.000000 polyaxon-2.0.0rc7/polyaxon.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-12 14:22:00.000000 polyaxon-2.0.0rc7/polyaxon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-12 14:22:00.000000 polyaxon-2.0.0rc7/polyaxon.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:01.112076 polyaxon-2.0.0rc7/polyaxon_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/polyaxon_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-12 14:22:01.112076 polyaxon-2.0.0rc7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-04-12 14:21:52.000000 polyaxon-2.0.0rc7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.515668 polyaxon-2.0.0rc8/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10054 2023-04-16 12:03:59.515668 polyaxon-2.0.0rc8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.455667 polyaxon-2.0.0rc8/polyaxon/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.459667 polyaxon-2.0.0rc8/polyaxon/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/agents/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16634 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/agents/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/agents/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/agents/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.459667 polyaxon-2.0.0rc8/polyaxon/agents/spawners/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/agents/spawners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/agents/spawners/async_spawner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/agents/spawners/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/agents/spawners/spawner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.459667 polyaxon-2.0.0rc8/polyaxon/auxiliaries/
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/auxiliaries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/auxiliaries/cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/auxiliaries/default_scheduling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/auxiliaries/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6387 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/auxiliaries/notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/auxiliaries/sidecar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/auxiliaries/tuner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.459667 polyaxon-2.0.0rc8/polyaxon/builds/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/builds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9207 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/builds/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.459667 polyaxon-2.0.0rc8/polyaxon/builds/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/builds/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/builds/generator/dockerfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/builds/generator/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.463667 polyaxon-2.0.0rc8/polyaxon/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9430 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/cli/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16965 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/cli/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/cli/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/cli/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/cli/completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18388 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/cli/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/cli/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/cli/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.463667 polyaxon-2.0.0rc8/polyaxon/cli/executor/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/cli/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/cli/executor/conda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/cli/executor/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/cli/executor/k8s.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/cli/executor/platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8310 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/cli/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16604 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/cli/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62014 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/cli/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/cli/port_forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17155 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/cli/project_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12238 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/cli/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12708 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/cli/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.463667 polyaxon-2.0.0rc8/polyaxon/cli/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/cli/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/cli/services/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/cli/services/clean_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/cli/services/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10322 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/cli/services/initializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/cli/services/notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/cli/services/sidecar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/cli/services/tuner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/cli/services/wait.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/cli/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.463667 polyaxon-2.0.0rc8/polyaxon/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.463667 polyaxon-2.0.0rc8/polyaxon/client/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/client/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/client/decorators/client_call_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/client/decorators/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/client/decorators/is_managed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/client/impersonate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/client/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58673 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/client/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)   108195 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/client/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.463667 polyaxon-2.0.0rc8/polyaxon/client/transport/
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/client/transport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/client/transport/http_transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/client/transport/periodic_transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/client/transport/retry_transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/client/transport/socket_transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/client/transport/threaded_transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/client/transport/ws_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.463667 polyaxon-2.0.0rc8/polyaxon/client/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/client/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/client/workers/base_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/client/workers/periodic_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/client/workers/queue_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.467667 polyaxon-2.0.0rc8/polyaxon/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/config/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/config/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/config/spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.467667 polyaxon-2.0.0rc8/polyaxon/connections/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/connections/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.467667 polyaxon-2.0.0rc8/polyaxon/connections/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/connections/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/connections/aws/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7381 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/connections/aws/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.467667 polyaxon-2.0.0rc8/polyaxon/connections/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/connections/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/connections/azure/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/connections/azure/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/connections/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.467667 polyaxon-2.0.0rc8/polyaxon/connections/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/connections/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/connections/gcp/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/connections/gcp/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/connections/kinds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/connections/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.467667 polyaxon-2.0.0rc8/polyaxon/connections/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/connections/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/connections/schemas/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/connections/schemas/k8s_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.467667 polyaxon-2.0.0rc8/polyaxon/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/constants/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/constants/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.467667 polyaxon-2.0.0rc8/polyaxon/containers/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/containers/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/containers/pull_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/containers/statuses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.467667 polyaxon-2.0.0rc8/polyaxon/contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/contexts/keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/contexts/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/contexts/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/contexts/refs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/contexts/sections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.467667 polyaxon-2.0.0rc8/polyaxon/deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/deploy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.467667 polyaxon-2.0.0rc8/polyaxon/deploy/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/deploy/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/deploy/operators/cmd_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/deploy/operators/compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/deploy/operators/conda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/deploy/operators/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/deploy/operators/helm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/deploy/operators/kubectl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/deploy/operators/pip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/deploy/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.471667 polyaxon-2.0.0rc8/polyaxon/deploy/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/deploy/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/deploy/schemas/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/deploy/schemas/celery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13189 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/deploy/schemas/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/deploy/schemas/deployment_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/deploy/schemas/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/deploy/schemas/ingress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/deploy/schemas/intervals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/deploy/schemas/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/deploy/schemas/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/deploy/schemas/rbac.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/deploy/schemas/root_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/deploy/schemas/security_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/deploy/schemas/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/deploy/schemas/service_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/deploy/schemas/ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/deploy/schemas/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/dist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.471667 polyaxon-2.0.0rc8/polyaxon/env_vars/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/env_vars/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.471667 polyaxon-2.0.0rc8/polyaxon/env_vars/getters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/env_vars/getters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/env_vars/getters/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/env_vars/getters/owner_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/env_vars/getters/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/env_vars/getters/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/env_vars/getters/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/env_vars/getters/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/env_vars/getters/versioned_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/env_vars/keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.471667 polyaxon-2.0.0rc8/polyaxon/fs/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/fs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11152 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/fs/async_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/fs/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/fs/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/fs/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/fs/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/fs/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/fs/tar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/fs/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/fs/watcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.471667 polyaxon-2.0.0rc8/polyaxon/init/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/init/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/init/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/init/dockerfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/init/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/init/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/init/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.475667 polyaxon-2.0.0rc8/polyaxon/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9513 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/k8s/async_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/k8s/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.475667 polyaxon-2.0.0rc8/polyaxon/k8s/custom_resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/k8s/custom_resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/k8s/custom_resources/crd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/k8s/custom_resources/operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/k8s/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/k8s/k8s_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5329 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/k8s/k8s_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.475667 polyaxon-2.0.0rc8/polyaxon/k8s/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/k8s/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/k8s/logging/async_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/k8s/logging/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27030 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/k8s/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/k8s/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/k8s/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/k8s/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/k8s/pods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/k8s/run_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11534 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/lifecycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/live_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6168 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.475667 polyaxon-2.0.0rc8/polyaxon/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/managers/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/managers/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8853 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/managers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/managers/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/managers/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/managers/compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14583 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/managers/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/managers/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/managers/home.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/managers/ignore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/managers/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/managers/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/managers/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.475667 polyaxon-2.0.0rc8/polyaxon/notifiers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/notifiers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/notifiers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/notifiers/discord_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/notifiers/hipchat_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/notifiers/keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/notifiers/mattermost_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/notifiers/pagerduty_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/notifiers/slack_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/notifiers/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/notifiers/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.479667 polyaxon-2.0.0rc8/polyaxon/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/operations/cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/operations/notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/operations/tuner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/pkg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.479667 polyaxon-2.0.0rc8/polyaxon/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/plugins/sentry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.479667 polyaxon-2.0.0rc8/polyaxon/polyaxonfile/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyaxonfile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyaxonfile/check.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.479667 polyaxon-2.0.0rc8/polyaxon/polyaxonfile/manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyaxonfile/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyaxonfile/manager/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyaxonfile/manager/workflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyaxonfile/params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.479667 polyaxon-2.0.0rc8/polyaxon/polyaxonfile/specs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyaxonfile/specs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyaxonfile/specs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34514 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyaxonfile/specs/compiled_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyaxonfile/specs/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyaxonfile/specs/kinds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.479667 polyaxon-2.0.0rc8/polyaxon/polyaxonfile/specs/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyaxonfile/specs/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyaxonfile/specs/libs/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11000 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyaxonfile/specs/libs/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyaxonfile/specs/libs/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyaxonfile/specs/operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyaxonfile/specs/sections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.479667 polyaxon-2.0.0rc8/polyaxon/polyboard/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyboard/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyboard/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyboard/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.479667 polyaxon-2.0.0rc8/polyaxon/polyflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.479667 polyaxon-2.0.0rc8/polyaxon/polyflow/builds/
+-rw-r--r--   0 runner    (1001) docker     (123)     7344 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/builds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.479667 polyaxon-2.0.0rc8/polyaxon/polyflow/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/cache/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.479667 polyaxon-2.0.0rc8/polyaxon/polyflow/component/
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/component/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12553 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/component/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/component/component_reference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.479667 polyaxon-2.0.0rc8/polyaxon/polyflow/containers/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/containers/container.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.479667 polyaxon-2.0.0rc8/polyaxon/polyflow/dags/
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/dags/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.479667 polyaxon-2.0.0rc8/polyaxon/polyflow/early_stopping/
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/early_stopping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/early_stopping/policies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.483667 polyaxon-2.0.0rc8/polyaxon/polyflow/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)    15301 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/environment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.483667 polyaxon-2.0.0rc8/polyaxon/polyflow/events/
+-rw-r--r--   0 runner    (1001) docker     (123)     7706 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/events/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.483667 polyaxon-2.0.0rc8/polyaxon/polyflow/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/hooks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.483667 polyaxon-2.0.0rc8/polyaxon/polyflow/init/
+-rw-r--r--   0 runner    (1001) docker     (123)    11473 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/init/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.483667 polyaxon-2.0.0rc8/polyaxon/polyflow/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15393 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/io/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.483667 polyaxon-2.0.0rc8/polyaxon/polyflow/joins/
+-rw-r--r--   0 runner    (1001) docker     (123)     6890 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/joins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.483667 polyaxon-2.0.0rc8/polyaxon/polyflow/matrix/
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/matrix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/matrix/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14568 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/matrix/bayes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/matrix/grid_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15378 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/matrix/hyperband.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/matrix/hyperopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/matrix/iterative.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/matrix/kinds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/matrix/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27192 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/matrix/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/matrix/random_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/matrix/tuner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.483667 polyaxon-2.0.0rc8/polyaxon/polyflow/mounts/
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/mounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/mounts/artifacts_mounts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.483667 polyaxon-2.0.0rc8/polyaxon/polyflow/notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/notifications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.483667 polyaxon-2.0.0rc8/polyaxon/polyflow/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/operations/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/operations/compiled_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23762 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/operations/operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.483667 polyaxon-2.0.0rc8/polyaxon/polyflow/optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/optimization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.483667 polyaxon-2.0.0rc8/polyaxon/polyflow/params/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/params/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12382 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/params/ops_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19144 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/params/params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.483667 polyaxon-2.0.0rc8/polyaxon/polyflow/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     9313 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.487667 polyaxon-2.0.0rc8/polyaxon/polyflow/references/
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/references/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/references/dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/references/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/references/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/references/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/references/url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.487667 polyaxon-2.0.0rc8/polyaxon/polyflow/run/
+-rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/run/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/run/cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23493 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/run/dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9498 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/run/dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/run/flink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/run/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/run/kinds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.487667 polyaxon-2.0.0rc8/polyaxon/polyflow/run/kubeflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/run/kubeflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/run/kubeflow/clean_pod_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/run/kubeflow/mpi_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9392 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/run/kubeflow/mx_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/run/kubeflow/paddle_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/run/kubeflow/pytorch_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7828 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/run/kubeflow/replica.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/run/kubeflow/scheduling_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7510 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/run/kubeflow/tf_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/run/kubeflow/xgboost_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/run/notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/run/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/run/ray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/run/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10122 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/run/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.487667 polyaxon-2.0.0rc8/polyaxon/polyflow/run/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/run/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/run/spark/replica.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/run/spark/spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/run/tuner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/run/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.487667 polyaxon-2.0.0rc8/polyaxon/polyflow/schedules/
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/schedules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/schedules/cron.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/schedules/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/schedules/interval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/schedules/kinds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.487667 polyaxon-2.0.0rc8/polyaxon/polyflow/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.487667 polyaxon-2.0.0rc8/polyaxon/polyflow/termination/
+-rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/termination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyflow/trigger_policies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.487667 polyaxon-2.0.0rc8/polyaxon/polyplot/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polyplot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.487667 polyaxon-2.0.0rc8/polyaxon/polypod/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.491668 polyaxon-2.0.0rc8/polyaxon/polypod/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/common/accelerators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/common/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/common/container_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/common/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12384 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/common/env_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/common/mounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/common/setter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/common/stores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/common/volumes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.491668 polyaxon-2.0.0rc8/polyaxon/polypod/compiler/
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/compiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/compiler/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.491668 polyaxon-2.0.0rc8/polyaxon/polypod/compiler/contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/compiler/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/compiler/contexts/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7030 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/compiler/contexts/contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/compiler/contexts/job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.491668 polyaxon-2.0.0rc8/polyaxon/polypod/compiler/contexts/kubeflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/compiler/contexts/kubeflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/compiler/contexts/kubeflow/mpi_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/compiler/contexts/kubeflow/mx_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/compiler/contexts/kubeflow/paddle_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/compiler/contexts/kubeflow/pytroch_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/compiler/contexts/kubeflow/tf_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/compiler/contexts/kubeflow/xgb_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/compiler/contexts/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/compiler/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.491668 polyaxon-2.0.0rc8/polyaxon/polypod/compiler/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/compiler/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30610 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/compiler/converters/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/compiler/converters/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/compiler/converters/job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.491668 polyaxon-2.0.0rc8/polyaxon/polypod/compiler/converters/kubeflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/compiler/converters/kubeflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/compiler/converters/kubeflow/mpi_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/compiler/converters/kubeflow/mx_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/compiler/converters/kubeflow/paddle_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/compiler/converters/kubeflow/pytroch_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/compiler/converters/kubeflow/tf_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/compiler/converters/kubeflow/xgboost_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/compiler/converters/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.491668 polyaxon-2.0.0rc8/polyaxon/polypod/compiler/lineage/
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/compiler/lineage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/compiler/lineage/artifacts_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/compiler/lineage/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/compiler/lineage/io_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/compiler/lineage/params_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.491668 polyaxon-2.0.0rc8/polyaxon/polypod/compiler/resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/compiler/resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10334 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/compiler/resolver/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/compiler/resolver/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.495668 polyaxon-2.0.0rc8/polyaxon/polypod/custom_resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/custom_resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/custom_resources/job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.495668 polyaxon-2.0.0rc8/polyaxon/polypod/custom_resources/kubeflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/custom_resources/kubeflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/custom_resources/kubeflow/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/custom_resources/kubeflow/mpi_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/custom_resources/kubeflow/mx_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/custom_resources/kubeflow/paddle_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/custom_resources/kubeflow/pytorch_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/custom_resources/kubeflow/tf_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/custom_resources/kubeflow/xgb_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/custom_resources/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.495668 polyaxon-2.0.0rc8/polyaxon/polypod/init/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/init/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/init/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/init/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/init/dockerfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/init/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/init/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/init/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/init/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.495668 polyaxon-2.0.0rc8/polyaxon/polypod/main/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/main/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/main/env_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/main/k8s_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/main/volumes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.495668 polyaxon-2.0.0rc8/polyaxon/polypod/pod/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/pod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/pod/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/pod/volumes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.495668 polyaxon-2.0.0rc8/polyaxon/polypod/sidecar/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/sidecar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/sidecar/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/sidecar/env_vars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.495668 polyaxon-2.0.0rc8/polyaxon/polypod/specs/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/specs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/specs/contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polypod/specs/replica.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.495668 polyaxon-2.0.0rc8/polyaxon/polytune/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polytune/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.495668 polyaxon-2.0.0rc8/polyaxon/polytune/search_managers/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polytune/search_managers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.495668 polyaxon-2.0.0rc8/polyaxon/polytune/search_managers/bayesian_optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polytune/search_managers/bayesian_optimization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.495668 polyaxon-2.0.0rc8/polyaxon/polytune/search_managers/grid_search/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polytune/search_managers/grid_search/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.495668 polyaxon-2.0.0rc8/polyaxon/polytune/search_managers/hyperband/
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polytune/search_managers/hyperband/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.495668 polyaxon-2.0.0rc8/polyaxon/polytune/search_managers/hyperopt/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polytune/search_managers/hyperopt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.495668 polyaxon-2.0.0rc8/polyaxon/polytune/search_managers/mapping/
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polytune/search_managers/mapping/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.495668 polyaxon-2.0.0rc8/polyaxon/polytune/search_managers/random_search/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/polytune/search_managers/random_search/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.499668 polyaxon-2.0.0rc8/polyaxon/pql/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/pql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17930 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/pql/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/pql/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14531 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/pql/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.499668 polyaxon-2.0.0rc8/polyaxon/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.499668 polyaxon-2.0.0rc8/polyaxon/schemas/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/api/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/api/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/api/home.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/api/installation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/api/log_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/api/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/api/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/api/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.499668 polyaxon-2.0.0rc8/polyaxon/schemas/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/cli/agent_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/cli/checks_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/cli/cli_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7848 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/cli/client_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/pending.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.507668 polyaxon-2.0.0rc8/polyaxon/schemas/responses/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_agent_state_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_agent_state_response_agent_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_agent_status_body_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_analytics_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_artifact_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_cloning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_connection_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_dashboard_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_entities_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_entities_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_entity_notification_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_entity_stage_body_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_entity_status_body_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_events_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_list_activities_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_list_agents_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_list_bookmarks_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_list_connections_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_list_dashboards_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_list_organization_members_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_list_organizations_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_list_presets_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_list_project_versions_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_list_projects_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_list_queues_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_list_run_artifacts_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_list_run_connections_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_list_run_edges_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_list_runs_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_list_searches_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_list_service_accounts_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_list_tags_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_list_team_members_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_list_teams_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_list_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_operation_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_organization_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_password_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_preset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_project_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_project_user_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_project_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_run_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_run_edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_run_reference_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_run_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_search_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_section_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_service_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_settings_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_team_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_team_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_trial_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_user_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_user_singup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_uuids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/services.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.507668 polyaxon-2.0.0rc8/polyaxon/schemas/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5474 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/types/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/types/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/types/clipped.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13661 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/types/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/types/dockerfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/types/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/types/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/types/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/types/k8s_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/schemas/types/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.507668 polyaxon-2.0.0rc8/polyaxon/sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.511668 polyaxon-2.0.0rc8/polyaxon/sdk/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/sdk/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   111064 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/sdk/api/agents_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8995 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/sdk/api/artifacts_stores_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36422 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/sdk/api/auth_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54976 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/sdk/api/connections_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54413 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/sdk/api/dashboards_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   277371 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/sdk/api/organizations_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55532 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/sdk/api/presets_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66019 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/sdk/api/project_dashboards_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65660 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/sdk/api/project_searches_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   245065 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/sdk/api/projects_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77685 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/sdk/api/queues_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   489214 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/sdk/api/runs_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53886 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/sdk/api/searches_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   101617 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/sdk/api/service_accounts_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60519 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/sdk/api/tags_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99633 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/sdk/api/teams_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73259 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/sdk/api/users_v1_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19041 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/sdk/api/versions_v1_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.511668 polyaxon-2.0.0rc8/polyaxon/sdk/async_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/sdk/async_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7357 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/sdk/async_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9849 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/sdk/async_client/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/sdk/base_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15722 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/sdk/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4776 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/sdk/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/sdk/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.511668 polyaxon-2.0.0rc8/polyaxon/sdk/sync_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/sdk/sync_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29147 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/sdk/sync_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13260 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/sdk/sync_client/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.511668 polyaxon-2.0.0rc8/polyaxon/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/services/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/services/ephemeral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/services/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/services/values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.511668 polyaxon-2.0.0rc8/polyaxon/sidecar/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/sidecar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.511668 polyaxon-2.0.0rc8/polyaxon/sidecar/container/
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/sidecar/container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/sidecar/container/intervals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.511668 polyaxon-2.0.0rc8/polyaxon/sidecar/container/monitors/
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/sidecar/container/monitors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/sidecar/container/monitors/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/sidecar/container/monitors/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/sidecar/ignore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/sidecar/processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.515668 polyaxon-2.0.0rc8/polyaxon/stores/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/stores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11678 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/stores/polyaxon_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.515668 polyaxon-2.0.0rc8/polyaxon/tracking/
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/tracking/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.515668 polyaxon-2.0.0rc8/polyaxon/tracking/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/tracking/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/tracking/contrib/fastai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/tracking/contrib/fastai_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/tracking/contrib/hugging_face.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/tracking/contrib/ignite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/tracking/contrib/keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/tracking/contrib/lightgbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/tracking/contrib/pytorch_lightning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/tracking/contrib/scikit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/tracking/contrib/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/tracking/contrib/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/tracking/contrib/xgboost.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/tracking/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.515668 polyaxon-2.0.0rc8/polyaxon/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/utils/cli_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.515668 polyaxon-2.0.0rc8/polyaxon/utils/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/utils/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/utils/fixtures/backfill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/utils/fixtures/bo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/utils/fixtures/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/utils/fixtures/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9711 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/utils/fixtures/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/utils/fixtures/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22732 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/utils/fixtures/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/utils/fixtures/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/utils/fixtures/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/utils/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/utils/fqn_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/utils/host_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/utils/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/utils/urls_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.515668 polyaxon-2.0.0rc8/polyaxon/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/vendor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon/vendor/shell_pty.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.459667 polyaxon-2.0.0rc8/polyaxon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10054 2023-04-16 12:03:59.000000 polyaxon-2.0.0rc8/polyaxon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22603 2023-04-16 12:03:59.000000 polyaxon-2.0.0rc8/polyaxon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 12:03:59.000000 polyaxon-2.0.0rc8/polyaxon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-16 12:03:59.000000 polyaxon-2.0.0rc8/polyaxon.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-16 12:03:59.000000 polyaxon-2.0.0rc8/polyaxon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-16 12:03:59.000000 polyaxon-2.0.0rc8/polyaxon.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.515668 polyaxon-2.0.0rc8/polyaxon_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/polyaxon_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-16 12:03:59.519668 polyaxon-2.0.0rc8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-04-16 12:03:47.000000 polyaxon-2.0.0rc8/setup.py
```

### Comparing `polyaxon-2.0.0rc7/PKG-INFO` & `polyaxon-2.0.0rc8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyaxon
-Version: 2.0.0rc7
+Version: 2.0.0rc8
 Summary: Command Line Interface (CLI) and client to interact with Polyaxon API.
 Home-page: https://github.com/polyaxon/polyaxon
 Author: Polyaxon, Inc.
 Author-email: contact@polyaxon.com
 Maintainer: Polyaxon, Inc.
 Maintainer-email: contact@polyaxon.com
 License: Apache 2.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: polyaxon Version: 2.0.0rc7 Summary: Command Line
+Metadata-Version: 2.1 Name: polyaxon Version: 2.0.0rc8 Summary: Command Line
 Interface (CLI) and client to interact with Polyaxon API. Home-page: https://
 github.com/polyaxon/polyaxon Author: Polyaxon, Inc. Author-email:
 contact@polyaxon.com Maintainer: Polyaxon, Inc. Maintainer-email:
 contact@polyaxon.com License: Apache 2.0 Keywords:
 polyaxon,aws,s3,microsoft,azure,google cloud storage,gcs,deep-learning,machine-
 learning,data-science,neural-networks,artificial-intelligence,ai,reinforcement-
 learning,kubernetes,aws,microsoft,azure,google cloud,tensorFlow,pytorch
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/__main__.py` & `polyaxon-2.0.0rc8/polyaxon/__main__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/agents/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/agents/agent.py` & `polyaxon-2.0.0rc8/polyaxon/agents/agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 import atexit
 import sys
 import time
 
 from typing import Dict, Optional
 
-from clipped.versions import clean_version_for_check
+from clipped.utils.versions import clean_version_for_check
 from urllib3.exceptions import HTTPError
 
 from polyaxon import pkg, settings
 from polyaxon.agents.base import BaseAgent
 from polyaxon.auxiliaries import V1PolyaxonInitContainer, V1PolyaxonSidecarContainer
 from polyaxon.lifecycle import V1StatusCondition, V1Statuses
 from polyaxon.schemas.responses.v1_agent import V1Agent
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/agents/base.py` & `polyaxon-2.0.0rc8/polyaxon/agents/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 # limitations under the License.
 import time
 import traceback
 
 from concurrent.futures import ThreadPoolExecutor
 from typing import Dict, Optional, Tuple
 
-from clipped.tz_utils import now
-from clipped.workers_utils import exit_context, get_pool_workers, get_wait
+from clipped.utils.tz import now
+from clipped.utils.workers import exit_context, get_pool_workers, get_wait
 from kubernetes.client.rest import ApiException
 
 from polyaxon import live_state, settings
 from polyaxon.agents import converter
 from polyaxon.agents.spawners.spawner import Spawner
 from polyaxon.client import PolyaxonClient
 from polyaxon.env_vars.getters import get_run_info
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/agents/converter.py` & `polyaxon-2.0.0rc8/polyaxon/agents/converter.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/agents/manager.py` & `polyaxon-2.0.0rc8/polyaxon/agents/manager.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/agents/spawners/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/agents/spawners/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/agents/spawners/async_spawner.py` & `polyaxon-2.0.0rc8/polyaxon/agents/spawners/async_spawner.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/agents/spawners/base.py` & `polyaxon-2.0.0rc8/polyaxon/agents/spawners/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Optional
 
-from clipped.enums_utils import get_enum_value
+from clipped.utils.enums import get_enum_value
 from kubernetes.client import Configuration
 
 from polyaxon import settings
 from polyaxon.exceptions import PolyaxonAgentError
 from polyaxon.polypod.mixins import MIXIN_MAPPING, BaseMixin
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/agents/spawners/spawner.py` & `polyaxon-2.0.0rc8/polyaxon/agents/spawners/spawner.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/api.py` & `polyaxon-2.0.0rc8/polyaxon/api.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/auxiliaries/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/auxiliaries/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/auxiliaries/cleaner.py` & `polyaxon-2.0.0rc8/polyaxon/auxiliaries/cleaner.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
 
 from typing import List, Optional
 
-from clipped.enums_utils import get_enum_value
+from clipped.utils.enums import get_enum_value
 
 from polyaxon import pkg
 from polyaxon.containers.names import MAIN_JOB_CONTAINER
 from polyaxon.containers.pull_policy import PullPolicy
 from polyaxon.k8s import k8s_schemas
 from polyaxon.schemas.services import BaseServiceConfig
 from polyaxon.schemas.types import V1ConnectionType
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/auxiliaries/default_scheduling.py` & `polyaxon-2.0.0rc8/polyaxon/auxiliaries/default_scheduling.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/auxiliaries/init.py` & `polyaxon-2.0.0rc8/polyaxon/auxiliaries/init.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/auxiliaries/notifier.py` & `polyaxon-2.0.0rc8/polyaxon/auxiliaries/notifier.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/auxiliaries/sidecar.py` & `polyaxon-2.0.0rc8/polyaxon/auxiliaries/sidecar.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Any, Dict, Optional, Union
 
+from clipped.types.ref_or_obj import BoolOrRef, IntOrRef, RefField
 from pydantic import Field, StrictStr
 
 from polyaxon import pkg
 from polyaxon.containers.pull_policy import PullPolicy
 from polyaxon.k8s import k8s_schemas
 from polyaxon.schemas.base import BaseSchemaModel
-from polyaxon.schemas.fields import BoolOrRef, IntOrRef, RefField
 
 
 def get_sidecar_resources() -> k8s_schemas.V1ResourceRequirements:
     return k8s_schemas.V1ResourceRequirements(
         limits={"cpu": "1", "memory": "500Mi"},
         requests={"cpu": "0.1", "memory": "60Mi"},
     )
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/auxiliaries/tuner.py` & `polyaxon-2.0.0rc8/polyaxon/auxiliaries/tuner.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/builds/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/builds/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/builds/builder.py` & `polyaxon-2.0.0rc8/polyaxon/builds/builder.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,43 +9,44 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-import json
 import logging
 import time
 
-from typing import Dict, List, Optional
+from typing import Dict, List, Optional, Union
+
+import orjson
 
-from clipped.logging_utils import LogLevels
+from clipped.utils.json import orjson_loads
+from clipped.utils.logging import LogLevels
 from docker import APIClient
 from docker.errors import APIError, BuildError
 from urllib3.exceptions import ReadTimeoutError
 
-from polyaxon.exceptions import PolyaxonBuildException
-from polyaxon.schemas.types import V1UriType
+from polyaxon.exceptions import PolyaxonBuildException, PolyaxonSchemaError
+from polyaxon.schemas.types import Uri
 
 _logger = logging.getLogger("polyaxon.dockerizer")
 
 
 class DockerMixin:
     IS_BUILD: Optional[bool] = None
 
     def _prepare_log_lines(self, log_line):  # pylint:disable=too-many-branches
         raw = log_line.decode("utf-8").strip()
         raw_lines = raw.split("\n")
         log_lines = []
         status = True
         for raw_line in raw_lines:
             try:
-                json_line = json.loads(raw_line)
+                json_line = orjson_loads(raw_line)
 
                 if json_line.get("error"):
                     log_lines.append(
                         "{}: {}".format(
                             LogLevels.ERROR, str(json_line.get("error", json_line))
                         )
                     )
@@ -61,15 +62,15 @@
                             log_lines.append("Pushing ...")
                     elif json_line.get("aux"):
                         log_lines.append(
                             "Pushing finished: {}".format(json_line.get("aux"))
                         )
                     else:
                         log_lines.append(str(json_line))
-            except json.JSONDecodeError:
+            except orjson.JSONDecodeError:
                 log_lines.append("JSON decode error: {}".format(raw_line))
         return log_lines, status
 
     def _handle_logs(self, log_lines):
         for log_line in log_lines:
             print(log_line)  # pylint:disable=superfluous-parens
 
@@ -103,49 +104,45 @@
     IS_BUILD = True
 
     def __init__(
         self,
         context: str,
         destination: str,
         credstore_env: Optional[Dict] = None,
-        registries: Optional[List[V1UriType]] = None,
+        registries: Optional[List[Union[Uri, str]]] = None,
         docker: Optional[APIClient] = None,
     ):
+        from polyaxon.config.parser import Parser
+
+        get_uri = Parser.parse(Uri)
         self.destination = destination
 
         self.context = context
-        self._validate_registries(registries)
-        self.registries = registries
-        self.docker = docker or APIClient(version="auto", credstore_env=credstore_env)
-        self.is_pushing = False
-
-    @staticmethod
-    def _validate_registries(registries: Optional[List[V1UriType]]):
-        if not registries or isinstance(registries, V1UriType):
-            return True
-
-        for registry in registries:
-            if not isinstance(registry, V1UriType):
+        self.registries = []
+        for r in registries or []:
+            try:
+                self.registries.append(get_uri(value=r, key="DockerBuilder"))
+            except PolyaxonSchemaError:
                 raise PolyaxonBuildException(
-                    "A registry `{}` is not valid Urispec.".format(registry)
+                    "Registry `{}` is not valid Uri.".format(r)
                 )
-
-        return True
+        self.docker = docker or APIClient(version="auto", credstore_env=credstore_env)
+        self.is_pushing = False
 
     def check_image(self):
         return self.docker.images(self.destination)
 
     def login_private_registries(self):
         if not self.registries:
             return
         for registry in self.registries:
             self.docker.login(
                 username=registry.user,
                 password=registry.password,
-                registry=registry.host,
+                registry=registry.host_port,
                 reauth=True,
             )
 
     def build(self, nocache: bool = False, memory_limit: Optional[int] = None):
         limits = {
             # Disable memory swap for building
             "memswap": -1
@@ -185,15 +182,15 @@
 
 def _build(
     context: str,
     destination: str,
     nocache: bool,
     docker: Optional[APIClient] = None,
     credstore_env: Optional[Dict] = None,
-    registries: Optional[List[V1UriType]] = None,
+    registries: Optional[List[Union[Uri, str]]] = None,
 ):
     """Build necessary code for a job to run"""
     _logger.info("Starting build ...")
 
     # Build the image
     docker_builder = DockerBuilder(
         context=context,
@@ -213,15 +210,15 @@
 
 def build(
     context: str,
     destination: str,
     nocache: bool,
     docker: Optional[APIClient] = None,
     credstore_env: Optional[Dict] = None,
-    registries: Optional[List[V1UriType]] = None,
+    registries: Optional[List[Union[Uri, str]]] = None,
     max_retries: int = 3,
     sleep_interval: int = 1,
 ):
     """Build necessary code for a job to run"""
     retry = 0
     is_done = False
     while retry < max_retries and not is_done:
@@ -273,15 +270,15 @@
 
 
 def build_and_push(
     context: str,
     destination: str,
     nocache: bool,
     credstore_env: Optional[Dict] = None,
-    registries: Optional[List[V1UriType]] = None,
+    registries: Optional[List[Union[Uri, str]]] = None,
     max_retries: int = 3,
     sleep_interval: int = 1,
 ):
     """Build necessary code for a job to run and push it."""
     # Build the image
     docker_builder = build(
         context=context,
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/builds/generator/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/builds/generator/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/builds/generator/dockerfile.py` & `polyaxon-2.0.0rc8/polyaxon/builds/generator/dockerfile.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/builds/generator/generator.py` & `polyaxon-2.0.0rc8/polyaxon/builds/generator/generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import jinja2
 import os
 
 from typing import List, Tuple, Union
 
-from clipped.list_utils import to_list
+from clipped.utils.lists import to_list
 
 from polyaxon.builds.generator.dockerfile import POLYAXON_DOCKER_TEMPLATE
 from polyaxon.schemas.types import V1DockerfileType
 
 
 class DockerFileGenerator:
     def __init__(self, build_context: V1DockerfileType, destination: str = "."):
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/cli/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/cli/admin.py` & `polyaxon-2.0.0rc8/polyaxon/cli/admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 
 import os
 import time
 
 import click
 
 from clipped.formatting import Printer
-from clipped.list_utils import to_list
-from clipped.validation import validate_tags
+from clipped.utils.lists import to_list
+from clipped.utils.validation import validate_tags
 
 from polyaxon.cli.dashboard import get_dashboard, get_dashboard_url
 from polyaxon.cli.errors import handle_cli_error
 from polyaxon.logger import clean_outputs
 from polyaxon.managers.deploy import DeployConfigManager
 from polyaxon.utils.fqn_utils import get_resource_name
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/cli/artifacts.py` & `polyaxon-2.0.0rc8/polyaxon/cli/artifacts.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/cli/auth.py` & `polyaxon-2.0.0rc8/polyaxon/cli/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import sys
 
 import click
 
-from clipped.dict_utils import dict_to_tabulate
 from clipped.formatting import Printer
+from clipped.utils.dicts import dict_to_tabulate
 from urllib3.exceptions import HTTPError
 
 from polyaxon import settings
 from polyaxon.cli.dashboard import get_dashboard_url
 from polyaxon.cli.errors import handle_cli_error, handle_command_not_in_ce
 from polyaxon.cli.session import ensure_cli_config, session_expired, set_versions_config
 from polyaxon.client import PolyaxonClient
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/cli/check.py` & `polyaxon-2.0.0rc8/polyaxon/cli/check.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/cli/completion.py` & `polyaxon-2.0.0rc8/polyaxon/cli/completion.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/cli/components.py` & `polyaxon-2.0.0rc8/polyaxon/cli/components.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
 import sys
 
 import click
 
-from clipped.dict_utils import list_dicts_to_tabulate
 from clipped.formatting import Printer
+from clipped.utils.dicts import list_dicts_to_tabulate
 
 from polyaxon import settings
 from polyaxon.cli.errors import handle_cli_error
 from polyaxon.cli.options import (
     OPTIONS_COMPONENT_VERSION,
     OPTIONS_NAME,
     OPTIONS_PROJECT,
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/cli/config.py` & `polyaxon-2.0.0rc8/polyaxon/cli/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import sys
 
 import click
 
-from clipped.dict_utils import dict_to_tabulate
 from clipped.formatting import Printer
+from clipped.utils.dicts import dict_to_tabulate
 
 from polyaxon import settings
 from polyaxon.cli.errors import handle_cli_error
 from polyaxon.cli.session import set_versions_config
 from polyaxon.logger import clean_outputs, logger
 from polyaxon.managers.cli import CliConfigManager
 from polyaxon.managers.client import ClientConfigManager
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/cli/dashboard.py` & `polyaxon-2.0.0rc8/polyaxon/cli/dashboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # limitations under the License.
 
 import sys
 
 import click
 
 from clipped.formatting import Printer
-from clipped.http_utils import clean_host
+from clipped.utils.http import clean_host
 
 from polyaxon import settings
 from polyaxon.api import POLYAXON_CLOUD_HOST
 from polyaxon.logger import clean_outputs
 
 
 def get_dashboard_url(
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/cli/errors.py` & `polyaxon-2.0.0rc8/polyaxon/cli/errors.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/cli/executor/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/cli/executor/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/cli/executor/conda.py` & `polyaxon-2.0.0rc8/polyaxon/cli/executor/conda.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # limitations under the License.
 
 import os
 import subprocess
 import sys
 
 from clipped.formatting import Printer
-from clipped.hashing import hash_value
+from clipped.utils.hashing import hash_value
 
 from polyaxon.cli.errors import handle_cli_error
 from polyaxon.deploy.operators.conda import CondaOperator
 from polyaxon.exceptions import (
     PolyaxonClientException,
     PolyaxonException,
     PolyaxonHTTPError,
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/cli/executor/docker.py` & `polyaxon-2.0.0rc8/polyaxon/cli/executor/docker.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,21 +10,21 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import json
 import os
 import sys
 
 from typing import List
 
 from clipped.formatting import Printer
+from clipped.utils.json import orjson_dumps
 
 from polyaxon.cli.errors import handle_cli_error
 from polyaxon.contexts import paths as ctx_paths
 from polyaxon.deploy.operators.docker import DockerOperator
 from polyaxon.env_vars.keys import EV_KEYS_NO_OP
 from polyaxon.exceptions import (
     PolyaxonClientException,
@@ -41,15 +41,15 @@
 
 def _get_env_vars(project, experiment_id, params, data_paths=None):
     env_vars = [
         ("POLYAXON_IS_MANAGED", "true"),
         ("POLYAXON_IS_LOCAL", "true"),
         (
             "POLYAXON_EXPERIMENT_INFO",
-            json.dumps(
+            orjson_dumps(
                 {
                     "project_name": project,
                     "experiment_name": "{}.{}".format(project, experiment_id),
                 }
             ),
         ),
     ]
@@ -59,16 +59,16 @@
         env_vars += [("POLYAXON_IS_OFFLINE", "true")]
 
     paths = {"local": "/tmp"}
 
     if data_paths:
         paths.update(data_paths)
 
-    env_vars += [("POLYAXON_PARAMS", json.dumps(params))]
-    env_vars += [("POLYAXON_RUN_DATA_PATHS", json.dumps(paths))]
+    env_vars += [("POLYAXON_PARAMS", orjson_dumps(params))]
+    env_vars += [("POLYAXON_RUN_DATA_PATHS", orjson_dumps(paths))]
     env_vars += [("POLYAXON_RUN_OUTPUTS_PATH", "/tmp/artifacts")]
 
     return env_vars
 
 
 def _get_config_volume():
     return [
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/cli/executor/k8s.py` & `polyaxon-2.0.0rc8/polyaxon/cli/executor/k8s.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/cli/executor/platform.py` & `polyaxon-2.0.0rc8/polyaxon/cli/executor/platform.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/cli/init.py` & `polyaxon-2.0.0rc8/polyaxon/cli/init.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 # limitations under the License.
 
 import os
 import sys
 
 import click
 
-from clipped import indentation
 from clipped.formatting import Printer
+from clipped.utils import indentation
 from urllib3.exceptions import HTTPError
 
 from polyaxon.cli.errors import handle_cli_error
 from polyaxon.cli.options import OPTIONS_PROJECT
 from polyaxon.client import ProjectClient
 from polyaxon.env_vars.getters import get_project_or_local
 from polyaxon.logger import clean_outputs
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/cli/models.py` & `polyaxon-2.0.0rc8/polyaxon/cli/models.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/cli/operations.py` & `polyaxon-2.0.0rc8/polyaxon/cli/operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,26 +16,26 @@
 import os
 import sys
 
 from typing import Any
 
 import click
 
-from clipped.csv_utils import write_csv
-from clipped.dict_utils import (
+from clipped.formatting import Printer
+from clipped.utils.csv import write_csv
+from clipped.utils.dicts import (
     dict_to_tabulate,
     flatten_keys,
     list_dicts_to_csv,
     list_dicts_to_tabulate,
 )
-from clipped.formatting import Printer
-from clipped.json_utils import orjson_dumps
-from clipped.list_utils import to_list
-from clipped.response_utils import get_meta_response
-from clipped.validation import validate_tags
+from clipped.utils.json import orjson_dumps
+from clipped.utils.lists import to_list
+from clipped.utils.responses import get_meta_response
+from clipped.utils.validation import validate_tags
 from urllib3.exceptions import HTTPError
 
 from polyaxon.api import (
     EXTERNAL_V1,
     REWRITE_EXTERNAL_V1,
     REWRITE_SERVICES_V1,
     SERVICES_V1,
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/cli/options.py` & `polyaxon-2.0.0rc8/polyaxon/cli/options.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/cli/port_forward.py` & `polyaxon-2.0.0rc8/polyaxon/cli/port_forward.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/cli/project_versions.py` & `polyaxon-2.0.0rc8/polyaxon/cli/project_versions.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 # limitations under the License.
 import sys
 
 from typing import Callable, List, Optional, Union
 
 import click
 
-from clipped.dict_utils import dict_to_tabulate, list_dicts_to_tabulate
 from clipped.formatting import Printer
-from clipped.query_params import get_query_params
-from clipped.response_utils import get_meta_response
-from clipped.validation import validate_tags
+from clipped.utils.dicts import dict_to_tabulate, list_dicts_to_tabulate
+from clipped.utils.query_params import get_query_params
+from clipped.utils.responses import get_meta_response
+from clipped.utils.validation import validate_tags
 from urllib3.exceptions import HTTPError
 
 from polyaxon.cli.dashboard import get_dashboard_url
 from polyaxon.cli.errors import handle_cli_error
 from polyaxon.client import PolyaxonClient, ProjectClient
 from polyaxon.lifecycle import V1ProjectVersionKind
 from polyaxon.sdk.exceptions import ApiException
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/cli/projects.py` & `polyaxon-2.0.0rc8/polyaxon/cli/projects.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import sys
 
 import click
 
-from clipped.dict_utils import list_dicts_to_tabulate
 from clipped.formatting import Printer
-from clipped.response_utils import get_meta_response
-from clipped.validation import validate_tags
+from clipped.utils.dicts import list_dicts_to_tabulate
+from clipped.utils.responses import get_meta_response
+from clipped.utils.validation import validate_tags
 from urllib3.exceptions import HTTPError
 
 from polyaxon.cli.dashboard import get_dashboard_url
 from polyaxon.cli.errors import handle_cli_error
 from polyaxon.cli.init import init as init_project
 from polyaxon.cli.options import OPTIONS_NAME, OPTIONS_OWNER, OPTIONS_PROJECT
 from polyaxon.cli.utils import get_entity_details
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/cli/run.py` & `polyaxon-2.0.0rc8/polyaxon/cli/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import sys
 
 import click
 
-from clipped import git_utils
 from clipped.formatting import Printer
-from clipped.validation import validate_tags
+from clipped.utils import git as git_utils
+from clipped.utils.validation import validate_tags
 from pydantic import ValidationError
 
 from polyaxon import settings
 from polyaxon.cli.executor import docker_run, k8s_run, platform_run
 from polyaxon.cli.options import OPTIONS_NAME, OPTIONS_PROJECT
 from polyaxon.env_vars.getters import get_project_or_local
 from polyaxon.exceptions import PolyaxonSchemaError
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/cli/services/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/cli/services/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/cli/services/agent.py` & `polyaxon-2.0.0rc8/polyaxon/cli/services/agent.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/cli/services/clean_artifacts.py` & `polyaxon-2.0.0rc8/polyaxon/cli/services/clean_artifacts.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import List, Union
 
 import click
 
 from clipped.formatting import Printer
-from clipped.list_utils import to_list
+from clipped.utils.lists import to_list
 
 from polyaxon.connections.kinds import V1ConnectionKind
 from polyaxon.schemas.types import V1ConnectionType
 
 
 @click.group()
 def clean_artifacts():
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/cli/services/docker.py` & `polyaxon-2.0.0rc8/polyaxon/cli/services/docker.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,24 +14,24 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import sys
 
 import click
 
 from clipped.formatting import Printer
-from clipped.path_utils import copy_file
+from clipped.types.docker_image import validate_image
+from clipped.utils.paths import copy_file
 from pydantic import ValidationError
 
 from polyaxon.builds.generator import DockerFileGenerator
 from polyaxon.cli.check import check_polyaxonfile
 from polyaxon.cli.errors import handle_cli_error
-from polyaxon.config_reader.spec import ConfigSpec
+from polyaxon.config.spec import ConfigSpec
 from polyaxon.exceptions import PolyaxonBuildException, PolyaxonSchemaError
 from polyaxon.polyaxonfile import CompiledOperationSpecification, OperationSpecification
-from polyaxon.schemas.fields.docker_image import validate_image
 from polyaxon.schemas.types import V1DockerfileType
 
 
 @click.group()
 def docker():
     pass
 
@@ -73,15 +73,15 @@
     default=False,
     help="Flag to track or not the file content.",
 )
 def generate(
     polyaxonfile, python_module, build_context, destination, copy_path, params, track
 ):
     """Generate a dockerfile given the polyaxonfile."""
-    from clipped.hashing import hash_value
+    from clipped.utils.hashing import hash_value
 
     from polyaxon.init.dockerfile import create_dockerfile_lineage
 
     if all([polyaxonfile, build_context]):
         Printer.error("Only a polyaxonfile or a build context option is required.")
         sys.exit(1)
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/cli/services/initializer.py` & `polyaxon-2.0.0rc8/polyaxon/cli/services/initializer.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,18 +16,19 @@
 import os
 import subprocess
 import sys
 
 import click
 
 from clipped.formatting import Printer
-from clipped.path_utils import check_or_create_path, copy_file
+from clipped.utils.lists import to_list
+from clipped.utils.paths import check_or_create_path, copy_file
 from pydantic import ValidationError
 
-from polyaxon.config_reader.spec import ConfigSpec
+from polyaxon.config.spec import ConfigSpec
 from polyaxon.connections.kinds import V1ConnectionKind
 from polyaxon.exceptions import PolyaxonSchemaError
 from polyaxon.schemas.types import V1FileType
 
 
 @click.group()
 def initializer():
@@ -50,15 +51,15 @@
     "--track",
     is_flag=True,
     default=False,
     help="Flag to track or not the file content.",
 )
 def file(file_context, filepath, copy_path, track):
     """Create auth context."""
-    from clipped.hashing import hash_value
+    from clipped.utils.hashing import hash_value
 
     from polyaxon.init.file import create_file_lineage
 
     try:
         file_context = V1FileType.from_dict(ConfigSpec.read_from(file_context))
     except (PolyaxonSchemaError, ValidationError) as e:
         Printer.error("received a non valid file context.")
@@ -94,18 +95,17 @@
 @click.option("--revision", help="The revision(commit/branch/treeish) to pull.")
 @click.option("--repo-path", help="The path to where to pull the repos.")
 @click.option("--connection", help="The connection used for pulling this repo.")
 @click.option("--flags", help="Additional flags for pulling this repo.")
 def git(url, repo_path, revision, connection, flags):
     """Create auth context."""
     from polyaxon.init.git import create_code_repo
-    from polyaxon.parser import parser
 
     if flags:
-        flags = parser.get_string("flags", flags, is_list=True)
+        flags = to_list(flags, check_str=True)
 
     create_code_repo(
         repo_path=repo_path,
         url=url,
         revision=revision,
         connection=connection,
         flags=flags,
@@ -331,15 +331,15 @@
     context_to,
     uuids,
     use_names,
     path_prefix,
     plugins,
 ):
     """Create path context."""
-    from clipped.validation import validate_tags
+    from clipped.utils.validation import validate_tags
 
     from polyaxon.init.tensorboard import initialize_tensorboard
 
     uuids = validate_tags(uuids)
     plugins = validate_tags(plugins)
     initialize_tensorboard(
         port=port,
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/cli/services/notifier.py` & `polyaxon-2.0.0rc8/polyaxon/cli/services/notifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import click
 
+from clipped.utils.json import orjson_loads
+
 from polyaxon.cli.options import OPTIONS_NAME
 
 
 @click.command()
 @click.option(
     "--backend",
     help="The notifier backend.",
@@ -74,20 +76,19 @@
     status,
     wait_time,
     duration,
     inputs,
     outputs,
 ):
     """Notifier command."""
-    import orjson
 
     from polyaxon.lifecycle import V1StatusCondition
     from polyaxon.notifiers import NOTIFIERS, NotificationSpec
 
-    condition = orjson.loads(condition)
+    condition = orjson_loads(condition)
     condition = V1StatusCondition.get_condition(**condition)
     status = status or condition.type
     notification = NotificationSpec(
         kind=kind,
         owner=owner,
         project=project,
         uuid=uuid,
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/cli/services/sidecar.py` & `polyaxon-2.0.0rc8/polyaxon/cli/services/sidecar.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import asyncio
 
 import click
 
-from clipped.coroutine import coroutine
+from clipped.utils.coroutine import coroutine
 
 from polyaxon.logger import logger
 
 
 @click.command()
 @click.option(
     "--container-id",
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/cli/services/tuner.py` & `polyaxon-2.0.0rc8/polyaxon/cli/services/tuner.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import time
 
 import click
-import orjson
+
+from clipped.utils.json import orjson_loads
 
 from polyaxon.logger import logger
 
 
 @click.group()
 def tuner():
     logger.info("Creating new suggestions...")
@@ -48,17 +49,17 @@
         BayesSearchManager,
     )
     from polyaxon.client import RunClient
     from polyaxon.polyflow import V1Bayes
 
     matrix = V1Bayes.read(matrix)
     if configs:
-        configs = orjson.loads(configs)
+        configs = orjson_loads(configs)
     if metrics:
-        metrics = orjson.loads(metrics)
+        metrics = orjson_loads(metrics)
 
     client = RunClient()
 
     retry = 0
     exp = None
     suggestions = None
     while retry < 3:
@@ -110,17 +111,17 @@
     from hypertune.search_managers.hyperband.manager import HyperbandManager
     from polyaxon.client import RunClient
     from polyaxon.polyflow import V1Hyperband
 
     matrix = V1Hyperband.read(matrix)
     matrix.set_tuning_params()
     if configs:
-        configs = orjson.loads(configs)
+        configs = orjson_loads(configs)
     if metrics:
-        metrics = orjson.loads(metrics)
+        metrics = orjson_loads(metrics)
 
     client = RunClient()
 
     retry = 0
     exp = None
     suggestions = None
     while retry < 3:
@@ -167,17 +168,17 @@
     from hypertune.iteration_lineage import handle_iteration, handle_iteration_failure
     from hypertune.search_managers.hyperopt.manager import HyperoptManager
     from polyaxon.client import RunClient
     from polyaxon.polyflow import V1Hyperopt
 
     matrix = V1Hyperopt.read(matrix)
     if configs:
-        configs = orjson.loads(configs)
+        configs = orjson_loads(configs)
     if metrics:
-        metrics = orjson.loads(metrics)
+        metrics = orjson_loads(metrics)
 
     client = RunClient()
 
     retry = 0
     exp = None
     suggestions = None
     while retry < 3:
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/cli/services/wait.py` & `polyaxon-2.0.0rc8/polyaxon/cli/services/wait.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/cli/session.py` & `polyaxon-2.0.0rc8/polyaxon/cli/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 # limitations under the License.
 
 import sys
 import uuid
 
 from typing import Optional
 
-from clipped.enums_utils import get_enum_value
 from clipped.formatting import Printer
-from clipped.tz_utils import now
-from clipped.versions import clean_version_for_compatibility
+from clipped.utils.enums import get_enum_value
+from clipped.utils.tz import now
+from clipped.utils.versions import clean_version_for_compatibility
 from urllib3.exceptions import HTTPError
 
 from polyaxon import pkg
 from polyaxon.cli.errors import handle_cli_error
 from polyaxon.client import PolyaxonClient
 from polyaxon.constants.globals import NO_AUTH
 from polyaxon.managers.auth import AuthConfigManager
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/cli/utils.py` & `polyaxon-2.0.0rc8/polyaxon/cli/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from clipped.dict_utils import dict_to_tabulate
 from clipped.formatting import Printer
-from clipped.json_utils import orjson_dumps
+from clipped.utils.dicts import dict_to_tabulate
+from clipped.utils.json import orjson_dumps
 
 
 def get_entity_details(entity: any, entity_name: str):
     if entity.description:
         Printer.heading("{} description:".format(entity_name))
         Printer.print("{}\n".format(entity.description))
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/cli/version.py` & `polyaxon-2.0.0rc8/polyaxon/cli/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import sys
 
 import click
 
-from clipped import indentation
-from clipped.dict_utils import dict_to_tabulate
 from clipped.formatting import Printer
-from clipped.versions import clean_version_for_check, compare_versions
+from clipped.utils import indentation
+from clipped.utils.dicts import dict_to_tabulate
+from clipped.utils.versions import clean_version_for_check, compare_versions
 
 from polyaxon import pkg
 from polyaxon.cli.session import set_versions_config
 from polyaxon.deploy.operators.pip import PipOperator
 from polyaxon.logger import clean_outputs, logger
 
 PROJECT_CLI_NAME = "polyaxon"
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/client/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/client/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/client/client.py` & `polyaxon-2.0.0rc8/polyaxon/client/client.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/client/decorators/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/client/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/client/decorators/client_call_handler.py` & `polyaxon-2.0.0rc8/polyaxon/client/decorators/client_call_handler.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/client/decorators/errors.py` & `polyaxon-2.0.0rc8/polyaxon/client/decorators/errors.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/client/decorators/is_managed.py` & `polyaxon-2.0.0rc8/polyaxon/client/decorators/is_managed.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/client/impersonate.py` & `polyaxon-2.0.0rc8/polyaxon/client/impersonate.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/client/init.py` & `polyaxon-2.0.0rc8/polyaxon/client/init.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/client/project.py` & `polyaxon-2.0.0rc8/polyaxon/client/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 # limitations under the License.
 import os
 
 from datetime import datetime
 from requests import HTTPError
 from typing import Dict, List, Optional, Tuple, Union
 
-from clipped.json_utils import orjson_dumps
-from clipped.path_utils import check_or_create_path, delete_path
-from clipped.query_params import get_query_params
-from clipped.tz_utils import now
-from clipped.validation import validate_tags
+from clipped.utils.json import orjson_dumps
+from clipped.utils.paths import check_or_create_path, delete_path
+from clipped.utils.query_params import get_query_params
+from clipped.utils.tz import now
+from clipped.utils.validation import validate_tags
 
 from polyaxon.client.client import PolyaxonClient
 from polyaxon.client.decorators import client_handler, get_global_or_inline_config
 from polyaxon.constants.globals import DEFAULT
 from polyaxon.contexts import paths as ctx_paths
 from polyaxon.env_vars.getters.user import get_local_owner
 from polyaxon.exceptions import PolyaxonClientException
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/client/run.py` & `polyaxon-2.0.0rc8/polyaxon/client/run.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,33 +20,31 @@
 import uuid
 
 from collections.abc import Mapping
 from datetime import datetime
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 from urllib.parse import urlparse
 
-import orjson
-
-from clipped.date_utils import file_modified_since
 from clipped.formatting import Printer
-from clipped.git_utils import get_code_reference
-from clipped.hashing import hash_dir, hash_file, hash_value
-from clipped.http_utils import absolute_uri
-from clipped.json_utils import orjson_dumps
-from clipped.list_utils import to_list
-from clipped.path_utils import (
+from clipped.utils.dates import file_modified_since
+from clipped.utils.git import get_code_reference
+from clipped.utils.hashing import hash_dir, hash_file, hash_value
+from clipped.utils.http import absolute_uri
+from clipped.utils.json import orjson_dumps, orjson_loads
+from clipped.utils.lists import to_list
+from clipped.utils.paths import (
     check_or_create_path,
     delete_path,
     get_base_filename,
     get_dirs_under_path,
     get_files_in_path_context,
 )
-from clipped.query_params import get_logs_params, get_query_params
-from clipped.tz_utils import now
-from clipped.validation import validate_tags
+from clipped.utils.query_params import get_logs_params, get_query_params
+from clipped.utils.tz import now
+from clipped.utils.validation import validate_tags
 from urllib3.exceptions import HTTPError
 
 from polyaxon import settings
 from polyaxon.api import K8S_V1_LOCATION, STREAMS_V1_LOCATION
 from polyaxon.cli.errors import handle_cli_error
 from polyaxon.client.client import PolyaxonClient
 from polyaxon.client.decorators import client_handler, get_global_or_inline_config
@@ -2618,15 +2616,15 @@
                 raise PolyaxonClientException(f"Offline data was not found: {run_path}")
             else:
                 logger.info(f"Offline data was not found: {run_path}")
                 return None
 
         with open(run_path, "r") as config_file:
             config_str = config_file.read()
-            run_config = V1Run(**orjson.loads(config_str))
+            run_config = V1Run(**orjson_loads(config_str))
             owner = run_config.owner
             project = run_config.project
             if run_client:
                 if reset_project or not owner:
                     owner = run_client.owner
                 if reset_project or not project:
                     project = run_client.project
@@ -2644,15 +2642,15 @@
 
         lineages_path = "{}/{}".format(path, ctx_paths.CONTEXT_LOCAL_LINEAGES)
         if not os.path.isfile(lineages_path):
             logger.info(f"Offline lineage data was not found: {lineages_path}")
             return run_client
         with open(lineages_path, "r") as config_file:
             config_str = config_file.read()
-            lineages = [V1RunArtifact.from_dict(l) for l in orjson.loads(config_str)]
+            lineages = [V1RunArtifact.from_dict(l) for l in orjson_loads(config_str)]
             run_client._artifacts_lineage = {l.name: l for l in lineages}  # type: ignore
             logger.info(f"Offline lineage data loaded from: {lineages_path}")
 
         return run_client
 
     @client_handler(check_no_op=True)
     def pull_remote_run(
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/client/transport/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/client/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/client/transport/http_transport.py` & `polyaxon-2.0.0rc8/polyaxon/client/transport/http_transport.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/client/transport/periodic_transport.py` & `polyaxon-2.0.0rc8/polyaxon/client/transport/periodic_transport.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/client/transport/retry_transport.py` & `polyaxon-2.0.0rc8/polyaxon/client/transport/retry_transport.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/client/transport/socket_transport.py` & `polyaxon-2.0.0rc8/polyaxon/client/transport/socket_transport.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,17 +10,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import json
 import websocket
 
+from clipped.utils.json import orjson_loads
+
 from polyaxon.logger import logger
 
 
 class SocketTransportMixin:
     """Socket operations transport."""
 
     def socket(self, url, message_handler, headers=None):
@@ -37,15 +38,15 @@
         webs = self.socket(url=url, message_handler=message_handler, headers=headers)
         webs.run_forever(ping_interval=30, ping_timeout=10)
 
     def _on_message(self, message_handler, message):
         if message_handler and message:
             if not isinstance(message, str):
                 message = message.decode("utf-8")
-            message_handler(json.loads(message))
+            message_handler(orjson_loads(message))
 
     @staticmethod
     def _on_error(ws, error):
         if isinstance(error, (KeyboardInterrupt, SystemExit)):
             logger.info("Quitting... The session will be running in the background.")
         else:
             logger.debug("Termination cause: %s", error)
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/client/transport/threaded_transport.py` & `polyaxon-2.0.0rc8/polyaxon/client/transport/threaded_transport.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/client/transport/ws_client.py` & `polyaxon-2.0.0rc8/polyaxon/client/transport/ws_client.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/client/workers/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/client/workers/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/client/workers/base_worker.py` & `polyaxon-2.0.0rc8/polyaxon/client/workers/base_worker.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/client/workers/periodic_worker.py` & `polyaxon-2.0.0rc8/polyaxon/client/workers/periodic_worker.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/client/workers/queue_worker.py` & `polyaxon-2.0.0rc8/polyaxon/client/workers/queue_worker.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/config_reader/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/config/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/config_reader/spec.py` & `polyaxon-2.0.0rc8/polyaxon/polyaxonfile/check.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,281 +10,265 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import json
 import os
-import sys
-import yaml
 
-from collections.abc import Mapping
-from requests import HTTPError
-from yaml.parser import ParserError
-from yaml.scanner import ScannerError
-
-from clipped.dict_utils import deep_update
-from clipped.list_utils import to_list
-
-from polyaxon.env_vars.keys import EV_KEYS_PUBLIC_REGISTRY, EV_KEYS_USE_GIT_REGISTRY
-from polyaxon.exceptions import PolyaxonClientException, PolyaxonSchemaError
-from polyaxon.sdk.exceptions import ApiException
-
-
-class ConfigSpec:
-    def __init__(self, value, config_type=None, check_if_exists=True):
-        self.value = value
-        self.config_type = config_type
-        self.check_if_exists = check_if_exists
-
-    @classmethod
-    def get_from(cls, value: object, config_type: object = None) -> "ConfigSpec":
-        if isinstance(value, cls):
-            return value
-
-        return cls(value=value, config_type=config_type)
-
-    def check_type(self):
-        type_check = self.config_type is None and not isinstance(
-            self.value, (Mapping, str)
-        )
-        if type_check:
-            raise PolyaxonSchemaError(
-                "Expects Mapping, string, or list of Mapping/string instances, "
-                "received {} instead".format(type(self.value))
-            )
-
-    def read(self):
-        if isinstance(self.value, Mapping):
-            return self.value
-
-        # try a python file
-        if isinstance(self.value, str) and (
-            self.config_type == ".py" or ".py" in self.value
-        ):
-            _f_path, _f_module = _get_python_file_def(self.value)
-            if _f_path and _f_module:
-                return _read_from_python(_f_path, _f_module)
+from collections import OrderedDict
+from typing import Dict, List, Optional, Union
 
-        if os.path.isfile(self.value):
-            return _read_from_file(self.value, self.config_type)
+from clipped.formatting import Printer
+from clipped.utils.lists import to_list
 
-        # try reading a stream of yaml or json
-        if not self.config_type or self.config_type in (".json", ".yml", ".yaml"):
+from polyaxon.cli.errors import handle_cli_error
+from polyaxon.config.spec import ConfigSpec
+from polyaxon.exceptions import PolyaxonfileError, PolyaxonSchemaError
+from polyaxon.polyaxonfile.manager import (
+    get_op_specification,
+    is_supported_in_eager_mode,
+)
+from polyaxon.polyaxonfile.params import parse_hparams, parse_params
+from polyaxon.polyaxonfile.specs import get_specification, kinds
+from polyaxon.polyflow import V1Dag, V1Init, V1Matrix, V1Operation
+
+
+def collect_dag_components(dag: V1Dag, path_context: Optional[str] = None):
+    """Collect components that cannot be resolved by the scheduler"""
+    for op in dag.operations:
+        op_name = op.name
+        if op.has_url_reference or op.has_path_reference or op.has_hub_reference:
             try:
-                return _read_from_stream(self.value)
-            except (ScannerError, ParserError):
+                op = collect_references(op, path_context)
+            except Exception as e:
                 raise PolyaxonSchemaError(
-                    "Received an invalid yaml stream: `{}`".format(self.value)
+                    "Pipeline op with name `{}` requires a component with ref `{}`, "
+                    "the reference could not be resolved. Error: {}".format(
+                        op_name, op.hub_ref or op.url_ref or op.path_ref, e
+                    )
                 )
 
-        if self.config_type == "url":
-            return _read_from_url(self.value)
-
-        if self.config_type == "hub":
-            if os.environ.get(EV_KEYS_USE_GIT_REGISTRY, False):
-                return _read_from_public_hub(self.value)
-            return _read_from_polyaxon_hub(self.value)
-
-        raise PolyaxonSchemaError(
-            "Received an invalid configuration: `{}`".format(self.value)
-        )
 
-    @classmethod
-    def read_from(cls, config_values, config_type=None):
-        """
-        Reads an ordered list of configuration values and
-        deep merge the values in reverse order.
-        """
-        if not config_values:
-            raise PolyaxonSchemaError(
-                "Cannot read config_value: `{}`".format(config_values)
+def collect_references(config: V1Operation, path_context: Optional[str] = None):
+    if config.has_component_reference:
+        return config
+    elif config.has_hub_reference:
+        component = ConfigSpec.get_from(config.hub_ref, "hub").read()
+    elif config.has_url_reference:
+        component = ConfigSpec.get_from(config.url_ref, "url").read()
+    elif config.has_path_reference:
+        path_ref = config.path_ref
+        if path_context:
+            path_ref = os.path.join(
+                os.path.dirname(os.path.abspath(path_context)), path_ref
             )
-
-        config_values = to_list(config_values, check_none=True)
-
-        config = {}
-        for config_value in config_values:
-            config_value = ConfigSpec.get_from(
-                value=config_value, config_type=config_type
+        component = ConfigSpec.get_from(path_ref).read()
+        path_context = path_ref
+    else:
+        raise PolyaxonfileError("Operation found without component")
+    component = get_specification(data=component)
+    if component.kind != kinds.COMPONENT:
+        if config.has_url_reference:
+            ref_type = "Url ref"
+            ref = config.url_ref
+        else:
+            ref_type = "Path ref"
+            ref = config.path_ref
+        raise PolyaxonfileError(
+            "the reference ({}) `{}` is of kind `{}`, it should be a `{}`".format(
+                ref, ref_type, component.kind, kinds.COMPONENT
             )
-            config_value.check_type()
-            config_results = config_value.read()
-            if config_results and isinstance(config_results, Mapping):
-                config = deep_update(config, config_results)
-            elif config_value.check_if_exists:
-                raise PolyaxonSchemaError(
-                    "Cannot read config_value: `{}`".format(config_value.value)
-                )
-
-        return config
-
-
-def _read_from_url(url: str):
-    from clipped.requests_utils import safe_request
-
-    resp = safe_request(url)
-    resp.raise_for_status()
-    return _read_from_stream(resp.content.decode())
-
+        )
+    config.component = component
+    if component.is_dag_run:
+        collect_dag_components(component.run, path_context)
+    return config
+
+
+def check_polyaxonfile(
+    polyaxonfile: Optional[str] = None,
+    python_module: Optional[str] = None,
+    url: Optional[str] = None,
+    hub: Optional[str] = None,
+    params: Optional[Union[List[str], Dict]] = None,
+    hparams: Optional[Union[List[str], Dict]] = None,
+    matrix_kind: Optional[str] = None,
+    matrix_concurrency: Optional[int] = None,
+    matrix_num_runs: Optional[int] = None,
+    matrix: Optional[Union[Dict, V1Matrix]] = None,
+    presets: Optional[List[str]] = None,
+    queue: Optional[str] = None,
+    nocache: Optional[bool] = None,
+    cache: Optional[Union[int, str, bool]] = None,
+    verbose: bool = True,
+    is_cli: bool = True,
+    to_op: bool = True,
+    validate_params: bool = True,
+    approved: Optional[Union[int, str, bool]] = None,
+    eager: bool = False,
+    git_init: Optional[V1Init] = None,
+    ignore_template: bool = False,
+):
+    if sum([1 for i in [python_module, url, hub] if i]) > 1:
+        message = (
+            "You can only use one and only one option: "
+            "hub, url, or a python module.".format(hub)
+        )
+        if is_cli:
+            Printer.error(message, sys_exit=True)
+        else:
+            raise PolyaxonfileError(message)
+    if not any([polyaxonfile, python_module, url, hub]):
+        polyaxonfile = check_default_path(path=".")
+    if not any([polyaxonfile, python_module, url, hub]):
+        message = (
+            "Something went wrong, `check_polyaxonfile` was called without a polyaxonfile, "
+            "a hub component reference, a url or a python module."
+        )
+        if is_cli:
+            Printer.error(message, sys_exit=True)
+        else:
+            raise PolyaxonfileError(message)
+    if hub and not to_op:
+        message = "Something went wrong, calling hub component `{}` without operation.".format(
+            hub
+        )
+        if is_cli:
+            Printer.error(message, sys_exit=True)
+        else:
+            raise PolyaxonfileError(message)
 
-def get_default_registry():
-    return os.environ.get(
-        EV_KEYS_PUBLIC_REGISTRY,
-        "https://raw.githubusercontent.com/polyaxon/polyaxon-hub/master",
-    )
+    polyaxonfile = to_list(polyaxonfile, check_none=True)
 
+    parsed_params = None
+    if params:
+        parsed_params = parse_params(params, is_cli=is_cli)
+    parsed_hparams = None
+    if hparams:
+        parsed_hparams = parse_hparams(hparams, is_cli=is_cli)
+
+    if not any([os.path.isfile(f) for f in polyaxonfile]) and not any(
+        [python_module, url, hub]
+    ):
+        message = "Please pass a valid polyaxonfile, a python module, a url, or a component name"
+        if is_cli:
+            Printer.error(message, sys_exit=True)
+        else:
+            raise PolyaxonfileError(message)
 
-def _read_from_public_hub(hub: str):
-    hub_values = hub.split(":")
-    if len(hub_values) > 2:
-        raise PolyaxonSchemaError("Received an invalid hub reference: `{}`".format(hub))
-    if len(hub_values) == 2:
-        hub_name, version = hub_values
-    else:
-        hub_name, version = hub_values[0], "latest"
-    version = version or "latest"
-    registry = get_default_registry()
-    url = "{}/{}/{}.yaml".format(registry, hub_name, version)
     try:
-        return _read_from_url(url)
-    except HTTPError as e:
-        if e.response.status_code == 404:
-            raise PolyaxonClientException(
-                "Component `{}` was not found, "
-                "please check that the name and tag are valid".format(hub)
-            )
-        raise PolyaxonClientException(
-            "Component `{}` could not be fetched, "
-            "an error was encountered {}".format(hub, e)
-        )
+        path_context = None
 
+        if python_module:
+            path_context = python_module
+            plx_file = (
+                ConfigSpec.get_from(python_module, config_type=".py")
+                .read()
+                .to_dict(include_kind=True, include_version=True)
+            )
+        elif url:
+            plx_file = ConfigSpec.get_from(url, "url").read()
+        elif hub:
+            plx_file = ConfigSpec.get_from(hub, "hub").read()
+        else:
+            path_context = polyaxonfile.pop(0)
+            plx_file = ConfigSpec.read_from(path_context)
 
-def _read_from_polyaxon_hub(hub: str):
-    from polyaxon.client import PolyaxonClient, ProjectClient
-    from polyaxon.constants.globals import DEFAULT_HUB, NO_AUTH
-    from polyaxon.env_vars.getters import get_component_info
-    from polyaxon.lifecycle import V1ProjectVersionKind
-    from polyaxon.schemas.cli.client_config import ClientConfig
+        plx_file = get_specification(data=plx_file)
+        if plx_file.kind == kinds.OPERATION:
+            plx_file = collect_references(plx_file, path_context)
+            plx_component = plx_file.component
+        else:
+            plx_component = plx_file
 
-    owner, component, version = get_component_info(hub)
+        if plx_component.is_dag_run:
+            collect_dag_components(plx_component.run, path_context)
 
-    try:
-        if owner == DEFAULT_HUB:
-            client = PolyaxonClient(
-                config=ClientConfig(use_cloud_host=True, verify_ssl=False),
-                token=NO_AUTH,
+        if to_op or hub:
+            plx_file = get_op_specification(
+                hub=hub,
+                config=plx_file,
+                params=parsed_params,
+                hparams=parsed_hparams,
+                matrix_kind=matrix_kind,
+                matrix_concurrency=matrix_concurrency,
+                matrix_num_runs=matrix_num_runs,
+                matrix=matrix,
+                presets=presets,
+                queue=queue,
+                nocache=nocache,
+                cache=cache,
+                approved=approved,
+                validate_params=validate_params,
+                preset_files=polyaxonfile,
+                git_init=git_init,
             )
+        if verbose and is_cli:
+            Printer.success("Polyaxonfile valid")
+        if ignore_template:
+            plx_file.disable_template()
+        if plx_file.is_template():
+            template_message = "This polyaxonfile was marked as template by the owner:"
+            if plx_file.template.description:
+                template_message += "\ntemplate description: {}".format(
+                    plx_file.template.description
+                )
+            if plx_file.template.fields:
+                template_message += "\ntemplate fields that need changes: {}".format(
+                    plx_file.template.fields
+                )
+            Printer.warning(template_message)
+        if eager:
+            is_supported_in_eager_mode(spec=plx_file)
+        return plx_file
+    except Exception as e:
+        message = "Polyaxonfile is not valid."
+        if is_cli:
+            handle_cli_error(e, message=message, sys_exit=True)
         else:
-            client = PolyaxonClient()
-        project_client = ProjectClient(owner=owner, project=component, client=client)
-        response = project_client.get_version(
-            kind=V1ProjectVersionKind.COMPONENT, version=version
-        )
-        return _read_from_stream(response.content)
-    except (ApiException, HTTPError) as e:
-        raise PolyaxonClientException(
-            "Component `{}` could not be fetched, "
-            "an error was encountered {}".format(hub, e)
-        )
+            raise PolyaxonfileError(message) from e
 
 
-def _read_from_stream(stream):
-    results = _read_from_yml(stream, is_stream=True)
-    if not results:
-        results = _read_from_json(stream, is_stream=True)
-    return results
-
-
-def _get_python_file_def(f_path):
-    if not isinstance(f_path, str) or ".py" not in f_path:
-        return None, None
-    results = f_path.split(":")
-
-    if len(results) == 1:  # Default case
-        return f_path, "main"
-
-    if len(results) != 2 or not results[1]:
-        return None, None
-
-    _f_path = results[0].strip("")
-    _module_name = results[1].strip("")
-    if not os.path.exists(_f_path):
-        raise PolyaxonSchemaError(
-            "Received non existing python file: `{}`".format(f_path)
-        )
-    if not _module_name:
-        raise PolyaxonSchemaError(
-            "Received an invalid python module: `{}`".format(f_path)
+def check_polyaxonfile_kind(specification, kind):
+    if specification.kind != kind:
+        Printer.error(
+            "Your polyaxonfile must be of kind: `{}`, "
+            "received: `{}`.".format(kind, specification.kind),
+            sys_exit=True,
         )
-    return _f_path, _module_name
-
 
-def _import_py_module(f_path, f_module):
-    import importlib.util
 
-    spec = importlib.util.spec_from_file_location(f_module, f_path)
-    if sys.modules.get(spec.name) and sys.modules[
-        spec.name
-    ].__file__ == os.path.abspath(spec.origin):
-        module = sys.modules[spec.name]
-    else:
-        module = importlib.util.module_from_spec(spec)
-        sys.modules[spec.name] = module
-        spec.loader.exec_module(module)
-    return module
-
-
-def _read_from_python(f_path, f_module):
-    f_path = os.path.abspath(f_path)
-    file_directory = os.path.dirname(f_path)
-    if file_directory not in sys.path:
-        sys.path.append(file_directory)
-
-    module_name = os.path.splitext(os.path.basename(f_path))[0]
-    module = _import_py_module(f_path, module_name)
-    return getattr(module, f_module)
-
-
-def _read_from_file(f_path, file_type):
-    _, ext = os.path.splitext(f_path)
-    if ext in (".yml", ".yaml") or file_type in (None, ".yml", ".yaml"):
-        return _read_from_yml(f_path)
-    elif ext == ".json" or file_type == ".json":
-        return _read_from_json(f_path)
-    elif ext == ".py" or file_type == ".py":
-        _f_path, _f_module = _get_python_file_def(f_path)
-        if _f_path and _f_module:
-            return _read_from_python(_f_path, _f_module)
-    raise PolyaxonSchemaError(
-        "Expects a file with extension: `.yml`, `.yaml`, `.py`, or `json`, "
-        "received instead `{}`".format(ext)
+def get_matrix_info(kind, concurrency, early_stopping=False, **kwargs):
+    info = OrderedDict()
+    info["Matrix kind"] = kind.lower()
+    info["Concurrency"] = (
+        "{} runs".format("sequential")
+        if concurrency == 1
+        else "{} concurrent runs".format(concurrency)
     )
-
-
-def _read_from_yml(f_path, is_stream=False):
-    try:
-        if is_stream:
-            return yaml.safe_load(f_path)
-        with open(f_path) as f:
-            return yaml.safe_load(f)
-    except (ScannerError, ParserError) as e:
-        raise PolyaxonSchemaError(
-            "Received non valid yaml: `%s`.\n" "Yaml error %s" % (f_path, e)
-        ) from e
-
-
-def _read_from_json(f_path, is_stream=False):
-    if is_stream:
-        try:
-            return json.loads(f_path)
-        except ValueError as e:
-            raise PolyaxonSchemaError("Json error: %s" % e) from e
-    try:
-        with open(f_path) as f:
-            return json.loads(f.read())
-    except ValueError as e:
-        raise PolyaxonSchemaError(
-            "Received non valid json: `%s`.\n" "Json error %s" % (f_path, e)
-        ) from e
+    info["Early stopping"] = "activated" if early_stopping else "deactivated"
+    if "num_runs" in kwargs:
+        info["Num of runs to create"] = kwargs["num_runs"]
+
+    Printer.dict_tabulate(info)
+
+
+DEFAULT_POLYAXON_FILE_NAME = [
+    "polyaxon",
+    "polyaxonci",
+    "polyaxon-ci",
+    "polyaxon.ci",
+    "polyaxonfile",
+]
+
+DEFAULT_POLYAXON_FILE_EXTENSION = ["yaml", "yml", "json"]
+
+
+def check_default_path(path):
+    path = os.path.abspath(path)
+    for filename in DEFAULT_POLYAXON_FILE_NAME:
+        for ext in DEFAULT_POLYAXON_FILE_EXTENSION:
+            filepath = os.path.join(path, "{}.{}".format(filename, ext))
+            if os.path.isfile(filepath):
+                return filepath
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/connections/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/connections/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/connections/aws/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/connections/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/connections/aws/base.py` & `polyaxon-2.0.0rc8/polyaxon/connections/aws/base.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/connections/aws/service.py` & `polyaxon-2.0.0rc8/polyaxon/connections/aws/service.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/connections/azure/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/connections/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/connections/azure/base.py` & `polyaxon-2.0.0rc8/polyaxon/connections/azure/base.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/connections/azure/service.py` & `polyaxon-2.0.0rc8/polyaxon/connections/azure/service.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/connections/base.py` & `polyaxon-2.0.0rc8/polyaxon/connections/base.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/connections/gcp/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/connections/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/connections/gcp/base.py` & `polyaxon-2.0.0rc8/polyaxon/connections/gcp/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import json
 import os
 
 from collections.abc import Mapping
 from typing import Any, Dict, List, Optional, Union
 
 import google.auth
 import google.oauth2.service_account
 
+from clipped.utils.json import orjson_loads
 from google.oauth2.service_account import Credentials
 
 from polyaxon.connections.reader import read_keys
 from polyaxon.contexts import paths as ctx_paths
 from polyaxon.exceptions import PolyaxonStoresException
 from polyaxon.logger import logger
 
@@ -122,15 +122,15 @@
             )
         else:
             raise PolyaxonStoresException("Unrecognised extension for key file.")
     else:
         # Get credentials from JSON data.
         try:
             if not isinstance(keyfile_dict, Mapping):
-                keyfile_dict = json.loads(keyfile_dict)  # type: ignore
+                keyfile_dict = orjson_loads(keyfile_dict)  # type: ignore
 
             # Convert escaped newlines to actual newlines if any.
             keyfile_dict["private_key"] = keyfile_dict["private_key"].replace(
                 "\\n", "\n"
             )
 
             credentials = Credentials.from_service_account_info(
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/connections/gcp/service.py` & `polyaxon-2.0.0rc8/polyaxon/connections/gcp/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # limitations under the License.
 
 import json
 import os
 
 from typing import TYPE_CHECKING, List, Optional
 
-from clipped.path_utils import create_project_tmp
+from clipped.utils.paths import create_project_tmp
 
 from polyaxon.connections.base import BaseService
 from polyaxon.connections.gcp.base import get_gc_client
 from polyaxon.connections.reader import get_connection_context_path
 from polyaxon.contexts import paths as ctx_paths
 
 if TYPE_CHECKING:
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/connections/kinds.py` & `polyaxon-2.0.0rc8/polyaxon/connections/kinds.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from clipped.enums_utils import PEnum
+from clipped.utils.enums import PEnum
 
 
 class V1ConnectionKind(str, PEnum):
     HOST_PATH = "host_path"
     VOLUME_CLAIM = "volume_claim"
     GCS = "gcs"
     S3 = "s3"
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/connections/reader.py` & `polyaxon-2.0.0rc8/polyaxon/connections/reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 
 from typing import Any, List, Optional, Set, Union
 
-from clipped.path_utils import check_dirname_exists
+from clipped.utils.paths import check_dirname_exists
 from pydantic import ValidationError
 
 from polyaxon.env_vars.keys import (
     EV_KEYS_CONNECTION_CONTEXT_PATH_FORMAT,
     EV_KEYS_CONNECTION_SCHEMA_FORMAT,
 )
 from polyaxon.logger import logger
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/connections/schemas/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/connections/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/connections/schemas/connections.py` & `polyaxon-2.0.0rc8/polyaxon/connections/schemas/connections.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Dict, List, Optional, Union
 
+from clipped.types.ref_or_obj import RefField
 from pydantic import Field, StrictStr
 
 from polyaxon.connections.kinds import V1ConnectionKind
 from polyaxon.schemas.base import BaseSchemaModel
-from polyaxon.schemas.fields.ref_or_obj import RefField
 
 
 class V1BucketConnection(BaseSchemaModel):
     _IDENTIFIER = "bucket"
 
     bucket: StrictStr
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/connections/schemas/k8s_resources.py` & `polyaxon-2.0.0rc8/polyaxon/connections/schemas/k8s_resources.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/constants/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/constants/globals.py` & `polyaxon-2.0.0rc8/polyaxon/constants/globals.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/constants/metadata.py` & `polyaxon-2.0.0rc8/polyaxon/constants/metadata.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/containers/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/containers/names.py` & `polyaxon-2.0.0rc8/polyaxon/containers/names.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/containers/pull_policy.py` & `polyaxon-2.0.0rc8/polyaxon/containers/pull_policy.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/containers/statuses.py` & `polyaxon-2.0.0rc8/polyaxon/containers/statuses.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/contexts/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/contexts/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/contexts/keys.py` & `polyaxon-2.0.0rc8/polyaxon/contexts/keys.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/contexts/params.py` & `polyaxon-2.0.0rc8/polyaxon/contexts/params.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/contexts/paths.py` & `polyaxon-2.0.0rc8/polyaxon/contexts/paths.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 
 from typing import Optional
 
-from clipped.enums_utils import get_enum_value
+from clipped.utils.enums import get_enum_value
 
 from polyaxon.env_vars.keys import (
     EV_KEYS_ARCHIVES_ROOT,
     EV_KEYS_ARTIFACTS_ROOT,
     EV_KEYS_CONTEXT_ROOT,
     EV_KEYS_OFFLINE_ROOT,
     EV_KEYS_SANDBOX_ROOT,
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/contexts/refs.py` & `polyaxon-2.0.0rc8/polyaxon/contexts/refs.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/contexts/sections.py` & `polyaxon-2.0.0rc8/polyaxon/contexts/sections.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/deploy/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/deploy/operators/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/deploy/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/deploy/operators/cmd_operator.py` & `polyaxon-2.0.0rc8/polyaxon/deploy/operators/cmd_operator.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/deploy/operators/compose.py` & `polyaxon-2.0.0rc8/polyaxon/deploy/operators/compose.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/deploy/operators/conda.py` & `polyaxon-2.0.0rc8/polyaxon/deploy/operators/conda.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/deploy/operators/docker.py` & `polyaxon-2.0.0rc8/polyaxon/deploy/operators/docker.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/deploy/operators/helm.py` & `polyaxon-2.0.0rc8/polyaxon/deploy/operators/helm.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/deploy/operators/kubectl.py` & `polyaxon-2.0.0rc8/polyaxon/deploy/operators/kubectl.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/deploy/operators/pip.py` & `polyaxon-2.0.0rc8/polyaxon/deploy/operators/pip.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/deploy/reader.py` & `polyaxon-2.0.0rc8/polyaxon/deploy/reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from polyaxon.config_reader.spec import ConfigSpec
+from polyaxon.config.spec import ConfigSpec
 from polyaxon.deploy.schemas.deployment import DeploymentConfig
 
 
 def read(filepaths):
     data = ConfigSpec.read_from(filepaths)
     return DeploymentConfig.from_dict(data)
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/deploy/schemas/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/deploy/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/deploy/schemas/auth.py` & `polyaxon-2.0.0rc8/polyaxon/deploy/schemas/auth.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/deploy/schemas/celery.py` & `polyaxon-2.0.0rc8/polyaxon/deploy/schemas/celery.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/deploy/schemas/deployment.py` & `polyaxon-2.0.0rc8/polyaxon/deploy/schemas/deployment.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/deploy/schemas/deployment_types.py` & `polyaxon-2.0.0rc8/polyaxon/deploy/schemas/deployment_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from clipped.enums_utils import PEnum
+from clipped.utils.enums import PEnum
 
 
 class DeploymentTypes(str, PEnum):
     KUBERNETES = "kubernetes"
     MINIKUBE = "minikube"
     MICRO_K8S = "microk8s"
     DOCKER_COMPOSE = "docker-compose"
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/deploy/schemas/email.py` & `polyaxon-2.0.0rc8/polyaxon/deploy/schemas/email.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/deploy/schemas/ingress.py` & `polyaxon-2.0.0rc8/polyaxon/deploy/schemas/ingress.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/deploy/schemas/intervals.py` & `polyaxon-2.0.0rc8/polyaxon/deploy/schemas/intervals.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/deploy/schemas/operators.py` & `polyaxon-2.0.0rc8/polyaxon/deploy/schemas/operators.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/deploy/schemas/proxy.py` & `polyaxon-2.0.0rc8/polyaxon/deploy/schemas/proxy.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/deploy/schemas/rbac.py` & `polyaxon-2.0.0rc8/polyaxon/deploy/schemas/rbac.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/deploy/schemas/root_user.py` & `polyaxon-2.0.0rc8/polyaxon/deploy/schemas/root_user.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Optional
 
+from clipped.types.email import EmailStr
 from pydantic import StrictStr, constr
 
 from polyaxon.schemas.base import NAME_REGEX, BaseSchemaModel
-from polyaxon.schemas.fields.email import EmailStr
 
 
 class RootUserConfig(BaseSchemaModel):
     username: Optional[constr(regex=NAME_REGEX)]  # type: ignore[valid-type]
     password: Optional[StrictStr]
     email: Optional[EmailStr]
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/deploy/schemas/security_context.py` & `polyaxon-2.0.0rc8/polyaxon/deploy/schemas/security_context.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,17 +12,18 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Optional
 
+from clipped.config.schema import skip_partial
 from pydantic import Field, StrictInt, StrictStr, root_validator
 
-from polyaxon.schemas.base import BaseSchemaModel, skip_partial
+from polyaxon.schemas.base import BaseSchemaModel
 
 
 def validate_security_context(user, group):
     if any([user, group]) and not all([user, group]):
         raise ValueError("Security context requires both `user` and `group` or none.")
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/deploy/schemas/service.py` & `polyaxon-2.0.0rc8/polyaxon/deploy/schemas/service.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/deploy/schemas/service_types.py` & `polyaxon-2.0.0rc8/polyaxon/deploy/schemas/service_types.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from clipped.enums_utils import PEnum
+from clipped.utils.enums import PEnum
 
 
 class ServiceTypes(str, PEnum):
     LOAD_BALANCER = "LoadBalancer"
     NODE_PORT = "NodePort"
     CLUSTER_IP = "ClusterIP"
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/deploy/schemas/ssl.py` & `polyaxon-2.0.0rc8/polyaxon/deploy/schemas/ssl.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/deploy/schemas/ui.py` & `polyaxon-2.0.0rc8/polyaxon/deploy/schemas/ui.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/dist.py` & `polyaxon-2.0.0rc8/polyaxon/dist.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/env_vars/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/env_vars/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/env_vars/getters/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/env_vars/getters/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/env_vars/getters/agent.py` & `polyaxon-2.0.0rc8/polyaxon/env_vars/getters/agent.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/env_vars/getters/owner_entity.py` & `polyaxon-2.0.0rc8/polyaxon/env_vars/getters/owner_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import sys
 
 from clipped.formatting import Printer
-from clipped.string_utils import validate_slug
+from clipped.utils.strings import validate_slug
 
 from polyaxon.constants.globals import DEFAULT
 from polyaxon.env_vars.getters.user import get_local_owner
 from polyaxon.exceptions import PolyaxonClientException, PolyaxonSchemaError
 from polyaxon.utils.fqn_utils import get_entity_info
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/env_vars/getters/project.py` & `polyaxon-2.0.0rc8/polyaxon/env_vars/getters/project.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import sys
 
 from clipped.formatting import Printer
-from clipped.string_utils import validate_slug
+from clipped.utils.strings import validate_slug
 
 from polyaxon.constants.globals import DEFAULT
 from polyaxon.env_vars.getters.user import get_local_owner
 from polyaxon.exceptions import PolyaxonClientException, PolyaxonSchemaError
 from polyaxon.managers.project import ProjectConfigManager
 from polyaxon.utils.cache import get_local_project
 from polyaxon.utils.fqn_utils import get_entity_info
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/env_vars/getters/queue.py` & `polyaxon-2.0.0rc8/polyaxon/env_vars/getters/queue.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/env_vars/getters/run.py` & `polyaxon-2.0.0rc8/polyaxon/env_vars/getters/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 
 from typing import Optional
 
-from clipped.bool_utils import to_bool
 from clipped.formatting import Printer
+from clipped.utils.bools import to_bool
 
 from polyaxon import settings
 from polyaxon.env_vars.getters.project import get_project_or_local
 from polyaxon.env_vars.keys import (
     EV_KEYS_COLLECT_ARTIFACTS,
     EV_KEYS_COLLECT_RESOURCES,
     EV_KEYS_RUN_INSTANCE,
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/env_vars/getters/user.py` & `polyaxon-2.0.0rc8/polyaxon/env_vars/getters/user.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/env_vars/getters/versioned_entity.py` & `polyaxon-2.0.0rc8/polyaxon/env_vars/getters/versioned_entity.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/env_vars/keys.py` & `polyaxon-2.0.0rc8/polyaxon/env_vars/keys.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/exceptions.py` & `polyaxon-2.0.0rc8/polyaxon/exceptions.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/fs/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/fs/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/fs/async_manager.py` & `polyaxon-2.0.0rc8/polyaxon/fs/async_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 # limitations under the License.
 import os
 
 from typing import Any, Dict, List, Optional, Union
 
 import aiofiles
 
-from clipped.coroutine import run_sync
-from clipped.hashing import hash_value
-from clipped.list_utils import to_list
-from clipped.path_utils import check_or_create_path
+from clipped.utils.coroutine import run_sync
+from clipped.utils.hashing import hash_value
+from clipped.utils.lists import to_list
+from clipped.utils.paths import check_or_create_path
 
 from polyaxon import settings
 from polyaxon.fs.tar import tar_dir
 from polyaxon.fs.tar import tar_files as sync_tar_files
 from polyaxon.fs.types import FSSystem
 from polyaxon.lifecycle import V1ProjectFeature
 from polyaxon.logger import logger
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/fs/azure.py` & `polyaxon-2.0.0rc8/polyaxon/fs/azure.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/fs/fs.py` & `polyaxon-2.0.0rc8/polyaxon/fs/fs.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/fs/gcs.py` & `polyaxon-2.0.0rc8/polyaxon/fs/gcs.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/fs/manager.py` & `polyaxon-2.0.0rc8/polyaxon/fs/manager.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import List, Union
 
-from clipped.list_utils import to_list
-from clipped.path_utils import check_or_create_path
+from clipped.utils.lists import to_list
+from clipped.utils.paths import check_or_create_path
 from fsspec import AbstractFileSystem
 
 from polyaxon.logger import logger
 
 
 def download_file_or_dir(
     fs: AbstractFileSystem,
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/fs/s3.py` & `polyaxon-2.0.0rc8/polyaxon/fs/s3.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/fs/tar.py` & `polyaxon-2.0.0rc8/polyaxon/fs/tar.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 
 from typing import List, Optional
 
-from clipped.path_utils import create_tarfile, get_files_in_path
+from clipped.utils.paths import create_tarfile, get_files_in_path
 
 from polyaxon import settings
 
 
 def tar_dir(download_path: str) -> str:
     outputs_files = get_files_in_path(download_path)
     tar_base_name = os.path.basename(download_path)
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/fs/types.py` & `polyaxon-2.0.0rc8/polyaxon/fs/types.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/fs/watcher.py` & `polyaxon-2.0.0rc8/polyaxon/fs/watcher.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,125 +9,96 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import json
 import os
 
-from collections import namedtuple
 from datetime import datetime
-from typing import Dict, List, Optional, Set
+from typing import Dict, List, Optional, Set, Tuple
 
-from clipped.date_utils import path_last_modified
-from clipped.path_utils import get_files_and_dirs_in_path
+from clipped.utils.dates import path_last_modified
+from clipped.utils.json import orjson_dumps
+from clipped.utils.paths import get_files_and_dirs_in_path
 
 from polyaxon.contexts import paths as ctx_paths
 from polyaxon.schemas.base import BaseSchemaModel
 
 
-class PathData(namedtuple("PathData", "base ts op")):
-    pass
+class PathData(BaseSchemaModel):
+    __root__: Tuple[str, datetime, str]
 
+    @property
+    def base(self) -> str:
+        return self.__root__[0]
 
-class FSWatcherConfig(BaseSchemaModel):
+    @property
+    def ts(self) -> datetime:
+        return self.__root__[1]
+
+    @property
+    def op(self) -> str:
+        return self.__root__[2]
+
+
+class FSWatcher(BaseSchemaModel):
     _IDENTIFIER = "fswatcher"
 
-    dir_mapping: Optional[Dict]
-    file_mapping: Optional[Dict]
+    _PUT = "put"
+    _RM = "rm"
+    _NOOP = ""
 
-    @staticmethod
-    def _datetime_handler(value: datetime) -> str:
-        if isinstance(value, datetime):
-            return value.isoformat()
-        raise TypeError("Unknown type")
+    dir_mapping: Optional[Dict[str, PathData]]
+    file_mapping: Optional[Dict[str, PathData]]
+
+    class Config(BaseSchemaModel.Config):
+        validate_assignment = False
 
     @classmethod
     def _dump(cls, obj_dict: Dict) -> str:
-        return json.dumps(obj_dict, default=cls._datetime_handler)
-
-    @staticmethod
-    def _parse_mapping(mapping: Optional[Dict]) -> Optional[Dict]:
-        if not mapping:
-            return None
-        return {
-            k: PathData(v[0], datetime.fromisoformat(v[1]), v[2])
-            for k, v in mapping.items()
-        }
+        return orjson_dumps(obj_dict)
 
     @staticmethod
     def delete(path: str):
         if os.path.exists(path):
             os.remove(path)
 
-    def get_dir_mapping(self) -> Optional[Dict]:
-        return self._parse_mapping(self.dir_mapping)
-
-    def get_file_mapping(self) -> Optional[Dict]:
-        return self._parse_mapping(self.file_mapping)
-
-
-class FSWatcher:
-    PUT = "put"
-    RM = "rm"
-    NOOP = ""
-
-    def __init__(
-        self, dir_mapping: Optional[Dict] = None, file_mapping: Optional[Dict] = None
-    ):
-        self._dir_mapping = dir_mapping or {}
-        self._file_mapping = file_mapping or {}
-
-    @classmethod
-    def read(
-        cls, config_path: str = ctx_paths.CONTEXT_MOUNT_FILE_WATCHER
-    ) -> "FSWatcher":
-        if not os.path.exists(config_path):
-            return cls()
-        config = FSWatcherConfig.read(config_path)
-        return cls(
-            dir_mapping=config.get_dir_mapping(), file_mapping=config.get_file_mapping()
-        )
-
-    def write(self, config_path: str = ctx_paths.CONTEXT_MOUNT_FILE_WATCHER):
-        config = FSWatcherConfig.read(
-            {
-                "dir_mapping": self._dir_mapping,
-                "file_mapping": self._file_mapping,
-            }
-        )
-        return config.write(config_path)
+    def write(self, filepath: str, mode: Optional[int] = None):
+        filepath = filepath or ctx_paths.CONTEXT_MOUNT_FILE_WATCHER
+        return super().write(filepath=filepath, mode=mode)
 
     def _sync_path(self, path: str, base_path: str, mapping: Dict) -> Dict:
         current_ts = path_last_modified(path)
         rel_path = os.path.relpath(path, base_path)
         data = mapping.get(rel_path)
         if data:
             if current_ts > data.ts:
-                mapping[rel_path] = PathData(base_path, current_ts, self.PUT)
+                mapping[rel_path] = PathData.construct(base_path, current_ts, self._PUT)
             else:
-                mapping[rel_path] = PathData(base_path, data.ts, self.NOOP)
+                mapping[rel_path] = PathData.construct(base_path, data.ts, self._NOOP)
         else:
-            mapping[rel_path] = PathData(base_path, current_ts, self.PUT)
+            mapping[rel_path] = PathData.construct(base_path, current_ts, self._PUT)
         return mapping
 
     def sync_file(self, path: str, base_path: str):
-        self._file_mapping = self._sync_path(path, base_path, self._file_mapping)
+        self.file_mapping = self._sync_path(path, base_path, self.file_mapping)
 
     def sync_dir(self, path: str, base_path: str):
-        self._dir_mapping = self._sync_path(path, base_path, self._dir_mapping)
+        self.dir_mapping = self._sync_path(path, base_path, self.dir_mapping)
 
     def init(self):
-        self._dir_mapping = {
-            p: PathData(d.base, d.ts, self.RM) for p, d in self._dir_mapping.items()
+        self.dir_mapping = {
+            p: PathData.construct(d.base, d.ts, self._RM)
+            for p, d in self.dir_mapping.items()
         }
-        self._file_mapping = {
-            p: PathData(d.base, d.ts, self.RM) for p, d in self._file_mapping.items()
+        self.file_mapping = {
+            p: PathData.construct(d.base, d.ts, self._RM)
+            for p, d in self.file_mapping.items()
         }
 
     def sync(self, path: str, exclude: Optional[List[str]] = None):
         files, dirs = get_files_and_dirs_in_path(
             path, exclude=exclude, collect_dirs=True
         )
         base_path, prefix_path = os.path.split(path)
@@ -140,21 +111,21 @@
     def _get_mapping_by_op(self, mapping: Dict, op: str) -> Set:
         return {(p.base, k) for k, p in mapping.items() if p.op == op}
 
     def _clean_by_op(self, mapping: Dict, op: str) -> Dict:
         return {k: p for k, p in mapping.items() if p.op != op}
 
     def get_files_to_put(self) -> Set:
-        return self._get_mapping_by_op(self._file_mapping, self.PUT)
+        return self._get_mapping_by_op(self.file_mapping, self._PUT)
 
     def get_files_to_rm(self) -> Set:
-        results = self._get_mapping_by_op(self._file_mapping, self.RM)
-        self._file_mapping = self._clean_by_op(self._file_mapping, self.RM)
+        results = self._get_mapping_by_op(self.file_mapping, self._RM)
+        self.file_mapping = self._clean_by_op(self.file_mapping, self._RM)
         return results
 
     def get_dirs_to_put(self) -> Set:
-        return self._get_mapping_by_op(self._dir_mapping, self.PUT)
+        return self._get_mapping_by_op(self.dir_mapping, self._PUT)
 
     def get_dirs_to_rm(self) -> Set:
-        results = self._get_mapping_by_op(self._dir_mapping, self.RM)
-        self._file_mapping = self._clean_by_op(self._file_mapping, self.RM)
+        results = self._get_mapping_by_op(self.dir_mapping, self._RM)
+        self.file_mapping = self._clean_by_op(self.file_mapping, self._RM)
         return results
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/init/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/init/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/init/artifacts.py` & `polyaxon-2.0.0rc8/polyaxon/init/artifacts.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import TYPE_CHECKING, Union
 
-from clipped.enums_utils import get_enum_value
 from clipped.formatting import Printer
+from clipped.utils.enums import get_enum_value
 
 from polyaxon.contexts import paths as ctx_paths
 from polyaxon.fs.watcher import FSWatcher
 from polyaxon.logger import logger
 from polyaxon.schemas.types import V1ConnectionType
 
 if TYPE_CHECKING:
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/init/auth.py` & `polyaxon-2.0.0rc8/polyaxon/init/auth.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/init/dockerfile.py` & `polyaxon-2.0.0rc8/polyaxon/init/dockerfile.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/init/file.py` & `polyaxon-2.0.0rc8/polyaxon/init/file.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/init/git.py` & `polyaxon-2.0.0rc8/polyaxon/init/git.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,24 +14,24 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 
 from typing import List, Optional
 
-from clipped.git_utils import (
+from clipped.utils.git import (
     add_remote,
     checkout_revision,
     get_code_reference,
     git_fetch,
     git_init,
     set_remote,
     update_submodules,
 )
-from clipped.path_utils import check_or_create_path
+from clipped.utils.paths import check_or_create_path
 from git import Repo as GitRepo
 
 from polyaxon.client.init import get_client_or_raise
 from polyaxon.env_vars.keys import (
     EV_KEYS_GIT_CREDENTIALS,
     EV_KEYS_GIT_CREDENTIALS_STORE,
     EV_KEYS_SSH_PATH,
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/init/tensorboard.py` & `polyaxon-2.0.0rc8/polyaxon/init/tensorboard.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/k8s/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/k8s/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/k8s/async_manager.py` & `polyaxon-2.0.0rc8/polyaxon/k8s/async_manager.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/k8s/constants.py` & `polyaxon-2.0.0rc8/polyaxon/k8s/constants.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/k8s/custom_resources/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/k8s/custom_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/k8s/custom_resources/crd.py` & `polyaxon-2.0.0rc8/polyaxon/k8s/custom_resources/crd.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/k8s/custom_resources/operation.py` & `polyaxon-2.0.0rc8/polyaxon/k8s/custom_resources/operation.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/k8s/events.py` & `polyaxon-2.0.0rc8/polyaxon/k8s/events.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/k8s/k8s_schemas.py` & `polyaxon-2.0.0rc8/polyaxon/k8s/k8s_schemas.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/k8s/k8s_validation.py` & `polyaxon-2.0.0rc8/polyaxon/k8s/k8s_validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Dict, Optional, Type, TypeVar, Union
 
-from clipped.string_utils import to_snake_case
+from clipped.utils.strings import to_snake_case
 
 from polyaxon.k8s import k8s_schemas
 
 Swagger = TypeVar("Swagger")
 
 
 def _validate_schema(value: Optional[Union[Swagger, Dict]], cls: Type[Swagger]):
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/k8s/logging/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/k8s/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/k8s/logging/async_monitor.py` & `polyaxon-2.0.0rc8/polyaxon/k8s/logging/async_monitor.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import datetime
 
 from typing import List, Optional, Tuple
 
-from clipped.tz_utils import now
+from clipped.utils.tz import now
 from kubernetes_asyncio.client.models import V1Pod
 from kubernetes_asyncio.client.rest import ApiException
 
 from polyaxon.k8s.async_manager import AsyncK8SManager
-from polyaxon.types import AwareDT
 from traceml.logging import V1Log, V1Logs
 
 
 async def handle_container_logs(
     k8s_manager: AsyncK8SManager, pod: V1Pod, container_name: str, **params
 ) -> List[V1Log]:
     resp = None
@@ -70,17 +70,17 @@
         )
     return logs
 
 
 async def query_k8s_operation_logs(
     k8s_manager: AsyncK8SManager,
     instance: str,
-    last_time: Optional[AwareDT],
+    last_time: Optional[datetime.datetime],
     stream: bool = False,
-) -> Tuple[List[V1Log], Optional[AwareDT]]:
+) -> Tuple[List[V1Log], Optional[datetime.datetime]]:
     new_time = now()
     params = {}
     if last_time:
         since_seconds = (new_time - last_time).total_seconds() - 1
         params["since_seconds"] = int(since_seconds)
     if stream:
         params["tail_lines"] = V1Logs._CHUNK_SIZE
@@ -99,17 +99,17 @@
 
     return logs, new_time
 
 
 async def query_k8s_pod_logs(
     k8s_manager: AsyncK8SManager,
     pod: V1Pod,
-    last_time: Optional[AwareDT],
+    last_time: Optional[datetime.datetime],
     stream: bool = False,
-) -> Tuple[List[V1Log], Optional[AwareDT]]:
+) -> Tuple[List[V1Log], Optional[datetime.datetime]]:
     new_time = now()
     params = {}
     if last_time:
         since_seconds = (new_time - last_time).total_seconds() - 1
         params["since_seconds"] = int(since_seconds)
     if stream:
         params["tail_lines"] = V1Logs._CHUNK_SIZE
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/k8s/logging/monitor.py` & `polyaxon-2.0.0rc8/polyaxon/k8s/logging/monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from datetime import datetime
 from typing import Any, Dict, Iterable, Optional
 
-from clipped.tz_utils import now
+from clipped.utils.tz import now
 from kubernetes.client.rest import ApiException
 
 from polyaxon.client import RunClient
 from polyaxon.exceptions import PolyaxonK8SError
 from polyaxon.k8s.manager import K8SManager
 from traceml.logging import V1Log
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/k8s/manager.py` & `polyaxon-2.0.0rc8/polyaxon/k8s/manager.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/k8s/monitor.py` & `polyaxon-2.0.0rc8/polyaxon/k8s/monitor.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/k8s/namespace.py` & `polyaxon-2.0.0rc8/polyaxon/k8s/namespace.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/k8s/nodes.py` & `polyaxon-2.0.0rc8/polyaxon/k8s/nodes.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,16 +10,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from clipped.utils.units import to_cpu_value, to_memory_bytes
+
 from polyaxon.constants.globals import UNKNOWN
-from traceml.processors.units_processors import to_cpu_value, to_memory_bytes
 
 
 class NodeLifeCycle:
     UNKNOWN = UNKNOWN
     READY = "ready"
     NOT_READY = "notReady"
     DELETED = "deleted"
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/k8s/pods.py` & `polyaxon-2.0.0rc8/polyaxon/k8s/pods.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/k8s/run_instance.py` & `polyaxon-2.0.0rc8/polyaxon/k8s/run_instance.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/lifecycle.py` & `polyaxon-2.0.0rc8/polyaxon/lifecycle.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import datetime
 
 from typing import Any, Dict, List, Optional, Union
 
-from clipped.date_utils import parse_datetime
-from clipped.enums_utils import PEnum
-from clipped.tz_utils import now
+from clipped.utils.dates import parse_datetime
+from clipped.utils.enums import PEnum
+from clipped.utils.tz import now
 from pydantic import StrictStr
 
 from polyaxon.schemas.base import BaseSchemaModel
 
 
 class V1Stages(str, PEnum):
     """Stage is the information that represents the current stage of an entity's version.
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/live_state.py` & `polyaxon-2.0.0rc8/polyaxon/live_state.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/logger.py` & `polyaxon-2.0.0rc8/polyaxon/logger.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/main.py` & `polyaxon-2.0.0rc8/polyaxon/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 
 import click
 
-from clipped.bool_utils import to_bool
 from clipped.formatting import Printer
+from clipped.utils.bools import to_bool
 
 from polyaxon import settings
 from polyaxon.cli.admin import admin
 from polyaxon.cli.artifacts import artifacts
 from polyaxon.cli.auth import login, logout, whoami
 from polyaxon.cli.check import check
 from polyaxon.cli.completion import completion
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/managers/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/managers/agent.py` & `polyaxon-2.0.0rc8/polyaxon/managers/agent.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
 
 from typing import Type
 
-from polyaxon.config_reader.manager import ConfigManager
-from polyaxon.config_reader.spec import ConfigSpec
+from polyaxon.config.manager import ConfigManager
+from polyaxon.config.spec import ConfigSpec
 from polyaxon.k8s.namespace import DEFAULT_NAMESPACE
 from polyaxon.managers.base import BaseConfigManager, ManagerVisibility
 from polyaxon.schemas.cli.agent_config import AgentConfig
 
 
 class AgentConfigManager(BaseConfigManager):
     """Manages agent configuration .agent file."""
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/managers/auth.py` & `polyaxon-2.0.0rc8/polyaxon/managers/auth.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
 
 from typing import Type
 
-from polyaxon.config_reader.manager import ConfigManager
-from polyaxon.config_reader.spec import ConfigSpec
+from polyaxon.config.manager import ConfigManager
+from polyaxon.config.spec import ConfigSpec
 from polyaxon.contexts import paths as ctx_paths
 from polyaxon.managers.base import BaseConfigManager, ManagerVisibility
 from polyaxon.schemas.api.authentication import AccessTokenConfig
 
 
 class AuthConfigManager(BaseConfigManager):
     """Manages access token configuration .auth file."""
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/managers/base.py` & `polyaxon-2.0.0rc8/polyaxon/managers/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,19 +15,17 @@
 # limitations under the License.
 
 import os
 
 from collections.abc import Mapping
 from typing import Any, Dict, Optional, Type
 
-import orjson
-
-from clipped.enums_utils import PEnum
-from clipped.json_utils import orjson_dumps
-from clipped.path_utils import check_or_create_path
+from clipped.utils.enums import PEnum
+from clipped.utils.json import orjson_dumps, orjson_loads
+from clipped.utils.paths import check_or_create_path
 
 from polyaxon.contexts import paths as ctx_paths
 from polyaxon.logger import logger
 from polyaxon.schemas.base import BaseSchemaModel
 
 
 class ManagerVisibility(str, PEnum):
@@ -204,15 +202,15 @@
 
     @classmethod
     def read_from_path(cls, config_filepath: str) -> Optional[Any]:
         if issubclass(cls.CONFIG, BaseSchemaModel):
             return cls.CONFIG.read(config_filepath)
         with open(config_filepath, "r") as config_file:
             config_str = config_file.read()
-        return cls.CONFIG(**orjson.loads(config_str))
+        return cls.CONFIG(**orjson_loads(config_str))
 
     @classmethod
     def get_config_defaults(cls) -> Dict:
         return {}
 
     @classmethod
     def get_config_or_default(cls) -> Any:
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/managers/cli.py` & `polyaxon-2.0.0rc8/polyaxon/managers/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import datetime
 
 from typing import TYPE_CHECKING, Optional, Type
 
-from clipped.tz_utils import now
+from clipped.utils.tz import now
 
 from polyaxon.managers.base import BaseConfigManager, ManagerVisibility
 from polyaxon.schemas.cli.cli_config import CliConfig
 
 if TYPE_CHECKING:
     from polyaxon.schemas.api.compatibility import V1Compatibility
     from polyaxon.schemas.api.installation import V1Installation
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/managers/client.py` & `polyaxon-2.0.0rc8/polyaxon/managers/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
 
 from typing import Type
 
-from polyaxon.config_reader.manager import ConfigManager
-from polyaxon.config_reader.spec import ConfigSpec
+from polyaxon.config.manager import ConfigManager
+from polyaxon.config.spec import ConfigSpec
 from polyaxon.managers.base import BaseConfigManager, ManagerVisibility
 from polyaxon.schemas.cli.client_config import ClientConfig
 
 
 class ClientConfigManager(BaseConfigManager):
     """Manages client configuration .client file."""
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/managers/compose.py` & `polyaxon-2.0.0rc8/polyaxon/managers/compose.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/managers/deploy.py` & `polyaxon-2.0.0rc8/polyaxon/managers/deploy.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/managers/git.py` & `polyaxon-2.0.0rc8/polyaxon/managers/git.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/managers/home.py` & `polyaxon-2.0.0rc8/polyaxon/managers/home.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
 
 from typing import Dict, Type
 
-from polyaxon.config_reader.manager import ConfigManager
-from polyaxon.config_reader.spec import ConfigSpec
+from polyaxon.config.manager import ConfigManager
+from polyaxon.config.spec import ConfigSpec
 from polyaxon.managers.base import BaseConfigManager, ManagerVisibility
 from polyaxon.schemas.api.home import HomeConfig
 
 
 class HomeConfigManager(BaseConfigManager):
     """Manages home configuration .home file."""
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/managers/ignore.py` & `polyaxon-2.0.0rc8/polyaxon/managers/ignore.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 import os
 import re
 
 from collections import namedtuple
 from pathlib import PurePath
 from typing import List, Optional
 
-from clipped.list_utils import to_list
-from clipped.path_utils import unix_style_path
+from clipped.utils.lists import to_list
+from clipped.utils.paths import unix_style_path
 
 from polyaxon.logger import logger
 from polyaxon.managers.base import BaseConfigManager, ManagerVisibility
 from polyaxon.utils import cli_constants
 
 
 class Pattern(namedtuple("Pattern", "pattern is_exclude re")):
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/managers/project.py` & `polyaxon-2.0.0rc8/polyaxon/managers/project.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/managers/run.py` & `polyaxon-2.0.0rc8/polyaxon/managers/run.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/managers/user.py` & `polyaxon-2.0.0rc8/polyaxon/managers/user.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/notifiers/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/notifiers/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/notifiers/base.py` & `polyaxon-2.0.0rc8/polyaxon/notifiers/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
 
 from typing import Any, Dict, List, Optional, Union
 
-from clipped.http_utils import add_notification_referrer_param, clean_host
-from clipped.list_utils import to_list
+from clipped.utils.http import add_notification_referrer_param, clean_host
+from clipped.utils.lists import to_list
 
 from polyaxon import settings
+from polyaxon.config.parser import Parser
 from polyaxon.exceptions import PolyaxonNotificationException
 from polyaxon.logger import logger
 from polyaxon.notifiers.spec import NotificationSpec
-from polyaxon.parser import parser
 from polyaxon.utils.urls_utils import validate_url
 
 ConfigType = Union[Dict, List[Dict]]
 
 
 class BaseNotifier:
     notification_key = None
@@ -108,15 +108,15 @@
         """
         value = os.environ.get(cls.config_key)
         if not value:
             raise PolyaxonNotificationException(
                 "Could not validate config for notifier {}".format(cls.name)
             )
 
-        return parser.get_dict(key=cls.config_key, value=value, is_list=True)
+        return Parser.parse(Dict)(key=cls.config_key, value=value, is_list=True)
 
     @classmethod
     def get_config(cls, config: ConfigType = None) -> ConfigType:
         config = config or cls._get_config()
         config = cls._validate_config(config)
         return config
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/notifiers/discord_webhook.py` & `polyaxon-2.0.0rc8/polyaxon/notifiers/discord_webhook.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/notifiers/hipchat_webhook.py` & `polyaxon-2.0.0rc8/polyaxon/notifiers/hipchat_webhook.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/notifiers/keys.py` & `polyaxon-2.0.0rc8/polyaxon/notifiers/keys.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/notifiers/mattermost_webhook.py` & `polyaxon-2.0.0rc8/polyaxon/notifiers/mattermost_webhook.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/notifiers/pagerduty_webhook.py` & `polyaxon-2.0.0rc8/polyaxon/notifiers/pagerduty_webhook.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/notifiers/slack_webhook.py` & `polyaxon-2.0.0rc8/polyaxon/notifiers/slack_webhook.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Dict
 
-from clipped.date_utils import to_timestamp
+from clipped.utils.dates import to_timestamp
 
 from polyaxon.connections.kinds import V1ConnectionKind
 from polyaxon.notifiers.keys import INTEGRATIONS_WEBHOOKS_SLACK
 from polyaxon.notifiers.spec import NotificationSpec
 from polyaxon.notifiers.webhook import WebHookNotifier
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/notifiers/spec.py` & `polyaxon-2.0.0rc8/polyaxon/notifiers/spec.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License
 
 from collections import namedtuple
 from typing import Optional
 
-from clipped.enums_utils import get_enum_value
+from clipped.utils.enums import get_enum_value
 
 from polyaxon.lifecycle import StatusColor
 from polyaxon.utils.urls_utils import get_run_url
 
 
 class NotificationSpec(
     namedtuple(
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/notifiers/webhook.py` & `polyaxon-2.0.0rc8/polyaxon/notifiers/webhook.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from requests import RequestException
 from typing import Dict, List
 
-from clipped.requests_utils import safe_request
+from clipped.utils.requests import safe_request
 
 from polyaxon.connections.kinds import V1ConnectionKind
 from polyaxon.logger import logger
 from polyaxon.notifiers.base import BaseNotifier
 from polyaxon.notifiers.keys import INTEGRATIONS_WEBHOOKS_GENERIC
 from polyaxon.notifiers.spec import NotificationSpec
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/operations/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/operations/cleaner.py` & `polyaxon-2.0.0rc8/polyaxon/operations/cleaner.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/operations/notifier.py` & `polyaxon-2.0.0rc8/polyaxon/operations/notifier.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Dict, Union
 
-from polyaxon import types
 from polyaxon.auxiliaries import get_default_notification_container
 from polyaxon.polyflow import (
     V1IO,
     V1Component,
     V1NotifierJob,
     V1Operation,
     V1Param,
@@ -55,21 +54,21 @@
                 collect_artifacts=False,
                 collect_resources=False,
                 auto_resume=False,
                 sync_statuses=False,
                 external_host=True,
             ),
             inputs=[
-                V1IO.construct(name="backend", type=types.STR, is_optional=False),
-                V1IO.construct(name="owner", type=types.STR, is_optional=False),
-                V1IO.construct(name="project", type=types.STR, is_optional=False),
-                V1IO.construct(name="uuid", type=types.STR, is_optional=False),
-                V1IO.construct(name="name", type=types.STR, is_optional=True),
-                V1IO.construct(name="condition", type=types.DICT, is_optional=True),
-                V1IO.construct(name="connection", type=types.STR, is_optional=True),
+                V1IO.construct(name="backend", type="str", is_optional=False),
+                V1IO.construct(name="owner", type="str", is_optional=False),
+                V1IO.construct(name="project", type="str", is_optional=False),
+                V1IO.construct(name="uuid", type="str", is_optional=False),
+                V1IO.construct(name="name", type="str", is_optional=True),
+                V1IO.construct(name="condition", type="dict", is_optional=True),
+                V1IO.construct(name="connection", type="str", is_optional=True),
             ],
             run=V1NotifierJob.construct(
                 connections=[connection],
                 container=get_default_notification_container(),
             ),
         ),
     )
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/operations/tuner.py` & `polyaxon-2.0.0rc8/polyaxon/operations/tuner.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/parser/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/parser/constants.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/mounts/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-NO_VALUE_FOUND = "_NO_VALUE_FOUND"
+from polyaxon.polyflow.mounts.artifacts_mounts import V1ArtifactsMount
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/pkg.py` & `polyaxon-2.0.0rc8/polyaxon/pkg.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 NAME = "polyaxon"
-VERSION = "2.0.0-rc7"
+VERSION = "2.0.0-rc8"
 SCHEMA_VERSION = 1.1
 DESC = "Command Line Interface (CLI) and client to interact with Polyaxon API."
 URL = "https://github.com/polyaxon/polyaxon"
 AUTHOR = "Polyaxon, Inc."
 EMAIL = "contact@polyaxon.com"
 LICENSE = "Apache 2.0"
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/plugins/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polyaxonfile/specs/libs/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/plugins/sentry.py` & `polyaxon-2.0.0rc8/polyaxon/plugins/sentry.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyaxonfile/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polyaxonfile/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyaxonfile/manager/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polyaxonfile/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyaxonfile/manager/operations.py` & `polyaxon-2.0.0rc8/polyaxon/polyaxonfile/manager/operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,27 +14,27 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import copy
 
 from collections.abc import Mapping
 from typing import Dict, List, Optional, Union
 
-from clipped.bool_utils import to_bool
+from clipped.config.patch_strategy import PatchStrategy
+from clipped.utils.bools import to_bool
 
 from polyaxon import pkg
 from polyaxon.env_vars.getters.queue import get_queue_info
 from polyaxon.exceptions import PolyaxonfileError
 from polyaxon.polyaxonfile.specs import (
     CompiledOperationSpecification,
     OperationSpecification,
     get_specification,
     kinds,
 )
 from polyaxon.polyflow import V1Component, V1Init, V1Matrix, V1MatrixKind, V1Operation
-from polyaxon.schemas import V1PatchStrategy
 
 
 def get_op_specification(
     config: Optional[Union[V1Component, V1Operation]] = None,
     hub: Optional[str] = None,
     params: Optional[Dict] = None,
     hparams: Optional[Dict] = None,
@@ -110,15 +110,15 @@
         preset_plx_file = OperationSpecification.read(preset_plx_file, is_preset=True)
         config = config.patch(preset_plx_file, strategy=preset_plx_file.patch_strategy)
     # Turn git_init to a pre_merge preset
     if git_init:
         git_preset = V1Operation(
             run_patch={"init": [git_init.to_dict()]}, is_preset=True
         )
-        config = config.patch(git_preset, strategy=V1PatchStrategy.PRE_MERGE)
+        config = config.patch(git_preset, strategy=PatchStrategy.PRE_MERGE)
 
     # Sanity check if params were passed and we are not dealing with a hub component
     params = copy.deepcopy(config.params)
     if validate_params:
         # Avoid in-place patch
         run_config = get_specification(config.to_dict())
         run_config = OperationSpecification.compile_operation(run_config)
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyaxonfile/manager/workflows.py` & `polyaxon-2.0.0rc8/polyaxon/polyaxonfile/manager/workflows.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyaxonfile/params.py` & `polyaxon-2.0.0rc8/polyaxon/polyaxonfile/params.py`

 * *Files 5% similar despite different names*

```diff
@@ -83,17 +83,17 @@
             )
             if is_cli:
                 Printer.error(message, sys_exit=True)
             else:
                 raise PolyaxonfileError(message)
         kind = values[0]
         try:
-            from polyaxon.config_reader.spec import _read_from_stream  # noqa
+            from polyaxon.config.spec import ConfigSpec
 
-            value = _read_from_stream(":".join(values[1:]))
+            value = ConfigSpec.read_from_stream(":".join(values[1:]))
         except Exception as e:
             message = (
                 "Hyper-parameter: `{}` with kind `{}` received an incorrect value `{}`. "
                 "Parsing error: {}".format(name, kind, value, e)
             )
             if is_cli:
                 Printer.error(message, sys_exit=True)
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyaxonfile/specs/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polyaxonfile/specs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from collections.abc import Mapping
 
-from polyaxon.config_reader.spec import ConfigSpec
+from polyaxon.config.spec import ConfigSpec
 from polyaxon.polyaxonfile.specs import kinds as spec_kinds
 from polyaxon.polyaxonfile.specs.base import BaseSpecification
 from polyaxon.polyaxonfile.specs.compiled_operation import (
     CompiledOperationSpecification,
 )
 from polyaxon.polyaxonfile.specs.component import ComponentSpecification
 from polyaxon.polyaxonfile.specs.operation import OperationSpecification
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyaxonfile/specs/base.py` & `polyaxon-2.0.0rc8/polyaxon/polyaxonfile/specs/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import copy
 
 from collections.abc import Mapping
 
-from clipped.list_utils import to_list
+from clipped.utils.lists import to_list
 
-from polyaxon.config_reader.spec import ConfigSpec
+from polyaxon.config.spec import ConfigSpec
 from polyaxon.exceptions import PolyaxonfileError, PolyaxonValidationError
 from polyaxon.pkg import SCHEMA_VERSION
 from polyaxon.polyaxonfile.specs import kinds
 from polyaxon.polyaxonfile.specs.sections import Sections
 
 
 class BaseSpecification(Sections):
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyaxonfile/specs/compiled_operation.py` & `polyaxon-2.0.0rc8/polyaxon/polyaxonfile/specs/compiled_operation.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import copy
 
 from typing import Dict, List, Optional, Set, Type, Union
 
-from polyaxon import types
 from polyaxon.exceptions import PolyaxonfileError, PolyaxonSchemaError
 from polyaxon.polyaxonfile.specs import kinds
 from polyaxon.polyaxonfile.specs.base import BaseSpecification
 from polyaxon.polyaxonfile.specs.libs.parser import Parser
 from polyaxon.polyaxonfile.specs.operation import OperationSpecification
 from polyaxon.polyflow import (
     ParamSpec,
@@ -44,15 +43,15 @@
     @staticmethod
     def dict_to_param_spec(contexts: Optional[Dict] = None, is_context: bool = False):
         contexts = contexts or {}
         return {
             k: ParamSpec(
                 name=k,
                 param=V1Param(value=v),
-                type=types.ANY,
+                type="Any",
                 is_flag=False,
                 is_list=None,
                 is_context=is_context,
                 arg_format=None,
             )
             for k, v in contexts.items()
         }
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyaxonfile/specs/component.py` & `polyaxon-2.0.0rc8/polyaxon/polyaxonfile/specs/component.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyaxonfile/specs/kinds.py` & `polyaxon-2.0.0rc8/polyaxon/polyaxonfile/specs/kinds.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyaxonfile/specs/libs/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polyboard/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyaxonfile/specs/libs/engine.py` & `polyaxon-2.0.0rc8/polyaxon/polyaxonfile/specs/libs/engine.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyaxonfile/specs/libs/parser.py` & `polyaxon-2.0.0rc8/polyaxon/polyaxonfile/specs/libs/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from collections.abc import Mapping
 from datetime import date, datetime, timedelta
 from enum import Enum
 from typing import Dict
 from uuid import UUID
 
-from clipped.serialization import (
+from clipped.utils.serialization import (
     date_serialize,
     datetime_serialize,
     timedelta_serialize,
     uuid_serialize,
 )
 
 from polyaxon.exceptions import PolyaxonSchemaError
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyaxonfile/specs/libs/validator.py` & `polyaxon-2.0.0rc8/polyaxon/polyaxonfile/specs/libs/validator.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyaxonfile/specs/operation.py` & `polyaxon-2.0.0rc8/polyaxon/polyaxonfile/specs/operation.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Dict, Optional, Type
 
-from clipped.list_utils import to_list
+from clipped.utils.lists import to_list
 
 from polyaxon.exceptions import PolyaxonSchemaError
 from polyaxon.polyaxonfile.specs import kinds
 from polyaxon.polyaxonfile.specs.base import BaseSpecification
 from polyaxon.polyflow import (
     V1IO,
     V1CompiledOperation,
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyaxonfile/specs/sections.py` & `polyaxon-2.0.0rc8/polyaxon/polyaxonfile/specs/sections.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyboard/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/run/kubeflow/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyboard/artifacts.py` & `polyaxon-2.0.0rc8/polyaxon/polyboard/artifacts.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyboard/events.py` & `polyaxon-2.0.0rc8/polyaxon/polyboard/events.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyboard/logging.py` & `polyaxon-2.0.0rc8/polyaxon/polyboard/logging.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/builds/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/builds/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Any, Dict, List, Optional, Union
 
+from clipped.config.patch_strategy import PatchStrategy
+from clipped.types.ref_or_obj import RefField
 from pydantic import Field, StrictStr
 
 from polyaxon.polyflow.cache import V1Cache
 from polyaxon.polyflow.params import V1Param
-from polyaxon.schemas import V1PatchStrategy
 from polyaxon.schemas.base import BaseSchemaModel
-from polyaxon.schemas.fields.ref_or_obj import RefField
 
 
 class V1Build(BaseSchemaModel):
     """You can configure Polyaxon to automatically trigger a build process anytime
     the component or operation is instantiated.
 
     the build section allows to dynamically recreate a new docker image
@@ -228,10 +228,10 @@
     hub_ref: StrictStr = Field(alias="hubRef")
     connection: Optional[StrictStr]
     queue: Optional[StrictStr]
     presets: Optional[Union[List[StrictStr], RefField]]
     cache: Optional[Union[V1Cache, RefField]]
     params: Optional[Dict[str, Union[V1Param, RefField]]]
     run_patch: Optional[Dict[str, Any]] = Field(alias="runPatch")
-    patch_strategy: Optional[Union[V1PatchStrategy, RefField]] = Field(
+    patch_strategy: Optional[Union[PatchStrategy, RefField]] = Field(
         alias="patchStrategy"
     )
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/cache/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/cache/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import List, Optional, Union
 
-from clipped.enums_utils import PEnum
+from clipped.types.ref_or_obj import BoolOrRef, IntOrRef, RefField
+from clipped.utils.enums import PEnum
 from pydantic import StrictStr
 
 from polyaxon.schemas.base import BaseSchemaModel
-from polyaxon.schemas.fields.ref_or_obj import BoolOrRef, IntOrRef, RefField
 
 
 class V1Cache(BaseSchemaModel):
     """Polyaxon provides a caching layer for operation executions,
     this behavior is enabled by default for all runs executed in the context of a DAG,
     a hyperparameter tuning, or a mapping.
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/component/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/component/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/component/base.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/component/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,24 +11,24 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import List, Optional, Union
 
+from clipped.types.ref_or_obj import BoolOrRef, FloatOrRef, RefField
+from clipped.utils.lists import to_list
 from pydantic import Field, StrictStr, constr, validator
 
-from polyaxon.parser import parser
 from polyaxon.polyflow.builds import V1Build
 from polyaxon.polyflow.cache import V1Cache
 from polyaxon.polyflow.hooks import V1Hook
 from polyaxon.polyflow.plugins import V1Plugins
 from polyaxon.polyflow.termination import V1Termination
 from polyaxon.schemas.base import NAME_REGEX, BaseSchemaModel
-from polyaxon.schemas.fields.ref_or_obj import BoolOrRef, FloatOrRef, RefField
 
 
 class BaseComponent(BaseSchemaModel):
     version: Optional[float]
     kind: Optional[StrictStr]
     name: Optional[Union[constr(regex=NAME_REGEX), RefField]]
     description: Optional[StrictStr]
@@ -40,11 +40,11 @@
     plugins: Optional[Union[V1Plugins, RefField]]
     build: Optional[Union[V1Build, RefField]]
     hooks: Optional[Union[List[V1Hook], RefField]]
     is_approved: Optional[BoolOrRef] = Field(alias="isApproved")
     cost: Optional[FloatOrRef]
 
     @validator("tags", "presets", pre=True)
-    def validate_str_list(cls, v, field):
+    def validate_str_list(cls, v):
         if isinstance(v, str):
-            return parser.get_string(field, v, is_list=True)
+            return to_list(v, check_str=True)
         return v
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/component/component.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/component/component.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/component/component_reference.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/component/component_reference.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/containers/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/containers/container.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/containers/container.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from clipped.list_utils import to_list
-from clipped.string_utils import strip_spaces
+from clipped.utils.lists import to_list
+from clipped.utils.strings import strip_spaces
 
 
 def get_container_command_args(config):
     def sanitize_str(value):
         if not value:
             return
         value = strip_spaces(value=value, join=False)
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/dags/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/dags/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/early_stopping/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/early_stopping/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/early_stopping/policies.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/early_stopping/policies.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,42 +12,43 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Optional, Union
 from typing_extensions import Annotated, Literal
 
+from clipped.types.ref_or_obj import BoolOrRef, FloatOrRef, IntOrRef
 from pydantic import Field, StrictFloat, StrictStr
 
 from polyaxon.polyflow.optimization import V1Optimization
-from polyaxon.schemas.base import BaseDiscriminatedModel
-from polyaxon.schemas.fields.ref_or_obj import BoolOrRef, FloatOrRef, IntOrRef
+from polyaxon.schemas.base import BaseSchemaModel
 
 
-class V1MedianStoppingPolicy(BaseDiscriminatedModel):
+class V1MedianStoppingPolicy(BaseSchemaModel):
     _IDENTIFIER = "median"
+    _USE_DISCRIMINATOR = True
 
     kind: Literal[_IDENTIFIER] = _IDENTIFIER
     evaluation_interval: IntOrRef = Field(alias="evaluationInterval")
     min_interval: Optional[IntOrRef] = Field(alias="minInterval")
     min_samples: Optional[IntOrRef] = Field(alias="minSamples")
 
 
-class V1TruncationStoppingPolicy(BaseDiscriminatedModel):
+class V1TruncationStoppingPolicy(BaseSchemaModel):
     _IDENTIFIER = "truncation"
 
     kind: Literal[_IDENTIFIER] = _IDENTIFIER
     percent: FloatOrRef
     evaluation_interval: IntOrRef = Field(alias="evaluationInterval")
     min_interval: Optional[IntOrRef] = Field(alias="minInterval")
     min_samples: Optional[IntOrRef] = Field(alias="minSamples")
     include_succeeded: Optional[BoolOrRef] = Field(alias="includeSucceeded")
 
 
-class V1DiffStoppingPolicy(BaseDiscriminatedModel):
+class V1DiffStoppingPolicy(BaseSchemaModel):
     _IDENTIFIER = "diff"
 
     kind: Literal[_IDENTIFIER] = _IDENTIFIER
     percent: FloatOrRef
     evaluation_interval: IntOrRef = Field(alias="evaluationInterval")
     min_interval: Optional[IntOrRef] = Field(alias="minInterval")
     min_samples: Optional[IntOrRef] = Field(alias="minSamples")
@@ -55,15 +56,15 @@
 
 V1EarlyStoppingPolicy = Annotated[
     Union[V1MedianStoppingPolicy, V1TruncationStoppingPolicy, V1DiffStoppingPolicy],
     Field(discriminator="kind", alias="earlyStopping"),
 ]
 
 
-class V1MetricEarlyStopping(BaseDiscriminatedModel):
+class V1MetricEarlyStopping(BaseSchemaModel):
     """Metric early stopping is an early stopping strategy based on metrics of runs,
     it allows to terminate a dag, a mapping, or hyperparameter tuning when a run's metric(s)
     meet(s) one or multiple conditions.
 
     If no policy is set and a metric early stopping condition is met the pipeline will be marked
     as succeeded and all pending or running operations will be stopped.
 
@@ -163,15 +164,15 @@
     kind: Literal[_IDENTIFIER] = _IDENTIFIER
     metric: StrictStr
     value: FloatOrRef
     optimization: Union[StrictFloat, V1Optimization]
     policy: Optional[V1EarlyStoppingPolicy]
 
 
-class V1FailureEarlyStopping(BaseDiscriminatedModel):
+class V1FailureEarlyStopping(BaseSchemaModel):
     """Failure early stopping is an early stopping strategy based on statuses of runs that allows
     to terminate a dag, a mapping, or hyperparameter tuning group
     when they reach a certain level of failures.
 
     If a percentage of the runs in the pipeline fail,
     the pipeline will be marked as failed as well,
     and all pending or running operations will be stopped.
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/environment/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/events/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/events/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import List, Union
 
-from clipped.enums_utils import PEnum
+from clipped.types.ref_or_obj import RefField
+from clipped.utils.enums import PEnum
 from pydantic import StrictStr
 
 from polyaxon.contexts import refs as ctx_refs
 from polyaxon.lifecycle import V1Statuses
 from polyaxon.schemas.base import BaseSchemaModel
-from polyaxon.schemas.fields.ref_or_obj import RefField
 
 
 class V1EventKind(str, PEnum):
     RUN_STATUS_CREATED = "run_status_created"
     RUN_STATUS_RESUMING = "run_status_resuming"
     RUN_STATUS_COMPILED = "run_status_compiled"
     RUN_STATUS_ON_SCHEDULE = "run_status_on_schedule"
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/hooks/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/hooks/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Dict, List, Optional, Union
 
+from clipped.types.ref_or_obj import BoolOrRef, RefField
 from pydantic import Field, StrictStr, validator
 
 from polyaxon.lifecycle import V1Statuses
 from polyaxon.polyflow.params import V1Param
 from polyaxon.schemas.base import BaseSchemaModel
-from polyaxon.schemas.fields.ref_or_obj import BoolOrRef, RefField
 
 
 class V1Hook(BaseSchemaModel):
     """You can configure Polyaxon to send notifications and webhooks to users and systems
     when operations reaches a final state,
     or trigger any logic that is tightly coupled with a class of operations.
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/init/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/init/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,19 +11,20 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import List, Optional, Union
 
+from clipped.config.schema import skip_partial
+from clipped.types.ref_or_obj import RefField
 from pydantic import Field, StrictStr, root_validator, validator
 
 from polyaxon.k8s import k8s_schemas, k8s_validation
-from polyaxon.schemas.base import BaseSchemaModel, skip_partial
-from polyaxon.schemas.fields.ref_or_obj import RefField
+from polyaxon.schemas.base import BaseSchemaModel
 from polyaxon.schemas.types import (
     V1ArtifactsType,
     V1DockerfileType,
     V1FileType,
     V1GitType,
     V1TensorboardType,
 )
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/io/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/io/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/io/io.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/io/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Any, List, Optional
 
+from clipped.config.schema import skip_partial
 from pydantic import Field, StrictStr, root_validator, validator
 
-from polyaxon import types
+from polyaxon.config.parser import Parser
 from polyaxon.exceptions import PolyaxonSchemaError, PolyaxonValidationError
-from polyaxon.parser import parser
-from polyaxon.schemas.base import BaseSchemaModel, skip_partial
+from polyaxon.schemas.base import BaseSchemaModel
 
 IO_NAME_BLACK_LIST = ["globals", "params", "connections"]
 IO_NAME_ERROR = (
     "Received an input/output with a name in {}, "
     "please use a different name that does "
     "not already taken by the context".format(IO_NAME_BLACK_LIST)
 )
@@ -37,15 +37,15 @@
     default: Any,
     is_optional: bool,
     is_list: bool,
     options: List[Any],
     parse: bool = True,
 ):
     try:
-        parsed_value = parser.TYPE_MAPPING[type](
+        parsed_value = Parser.parse(type)(
             key=name,
             value=value,
             is_list=is_list,
             is_optional=is_optional,
             default=default,
             options=options,
         )
@@ -80,18 +80,18 @@
         raise ValueError(
             "IO `{}` is not optional and has default value `{}`. "
             "Please either make it optional or remove the default value.".format(
                 name, value
             )
         )
 
-    if is_flag and type != types.BOOL:
+    if is_flag and type != "bool":
         raise TypeError(
             "IO type `{}` cannot be a flag, it must be of type `{}`".format(
-                type, types.BOOL
+                type, "bool"
             )
         )
 
     return value
 
 
 class V1IO(BaseSchemaModel):
@@ -123,15 +123,15 @@
 
     To learn how to pass valid values,
     please check the [param section](/docs/core/specification/params/).
 
     Args:
         name: str
         description: str, optional
-        type: str, one of: [any, int, float, bool, str, dict, dict_of_dicts, uri, auth, list, gcs, s3, wasb, dockerfile, git, image, event, artifacts, path, metric, metadata, date, datetime]  # noqa
+        type: str, any python type hint, pydantic built-in types, and gcs, s3, wasb, dockerfile, git, image, event, artifacts, path, metric, metadata, date, datetime.
         value: any, optional
         is_optional: bool, optional
         is_list: bool, optional
         is_flag: bool, optional
         arg_format: str, optional
         delay_validation: bool, optional
         options: List[any], optional
@@ -160,29 +160,29 @@
 
     ```python
     >>> from polyaxon import types
     >>> from polyaxon.polyflow import V1IO
     >>> inputs = [
     >>>     V1IO(
     >>>         name="loss",
-    >>>         type=types.STR,
+    >>>         type='str',
     >>>         description="Loss to use for training my model",
     >>>         is_optional=True,
     >>>         value="MeanSquaredError"
     >>>     ),
     >>>     V1IO(
     >>>         name="preprocess",
-    >>>         type=types.BOOL,
+    >>>         type='bool',
     >>>         description="A flag to preprocess data before training",
     >>>     )
     >>> ]
     >>> outputs = [
     >>>     V1IO(
     >>>         name="accuracy",
-    >>>         type=types.FLOAT,
+    >>>         type='float',
     >>>     ),
     >>>     V1IO(
     >>>         name="outputs-path",
     >>>         type=types.PATH,
     >>>     )
     >>> ]
     ```
@@ -223,38 +223,28 @@
     >>>   - name: learning_rate
     >>>     description: A short description about this input
     >>>     type: float
     ```
 
     for more details about composite type validation and schema,
     please check the [types section](/docs/core/specification/types/),
-    possible types:
-        * ANY: "any"
-        * INT: "int"
-        * FLOAT: "float"
-        * BOOL: "bool"
-        * STR: "str"
-        * DICT: "dict"
-        * DICT_OF_DICTS: "dict_of_dicts"
+    possible types include any python type hint, pydantic built-in types, and:
         * URI: "uri"
-        * AUTH: "auth"
         * LIST: "list"
         * GCS: "gcs"
         * S3: "s3"
         * WASB: "wasb"
         * DOCKERFILE: "dockerfile"
         * GIT: "git"
         * IMAGE: "image"
         * EVENT: "event"
         * ARTIFACTS: "artifacts"
         * PATH: "path"
         * METRIC: "metric"
         * METADATA: "metadata"
-        * DATE: "date"
-        * DATETIME: "datetime"
 
     ### value
 
     If an input is optional you should assign it a value.
     If an output is optional you can assign it a value.
 
     ```yaml
@@ -512,23 +502,14 @@
 
     @validator("name", always=True)
     def validate_name(cls, v):
         if v in IO_NAME_BLACK_LIST:
             raise ValueError(IO_NAME_ERROR)
         return v
 
-    @validator("type", always=True)
-    def validate_type(cls, v):
-        if v and v not in types.VALUES:
-            raise ValueError(
-                "Received an input/output with an invalid type `{}`, "
-                "please use one of the following types: {}".format(v, types.VALUES)
-            )
-        return v
-
     @root_validator
     @skip_partial
     def validate_io(cls, values):
         validate_io(
             name=values.get("name"),
             type=values.get("type"),
             value=values.get("value"),
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/joins/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/joins/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Dict, Optional, Union
 
+from clipped.types.ref_or_obj import IntOrRef, RefField
 from pydantic import StrictStr
 
 from polyaxon.polyflow.params.params import ParamValueMixin, V1Param
 from polyaxon.schemas.base import BaseSchemaModel
-from polyaxon.schemas.fields.ref_or_obj import IntOrRef, RefField
 
 
 class V1JoinParam(V1Param, ParamValueMixin):
     _IDENTIFIER = "join_param"
 
     @property
     def is_literal(self):
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/matrix/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/matrix/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/matrix/base.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/matrix/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,16 +10,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from polyaxon.schemas.base import BaseDiscriminatedModel
+from polyaxon.schemas.base import BaseSchemaModel
 
 
-class BaseSearchConfig(BaseDiscriminatedModel):
+class BaseSearchConfig(BaseSchemaModel):
+    _USE_DISCRIMINATOR = True
+
     def create_iteration(self, **kwargs) -> int:
         return 0
 
     def should_reschedule(self, **kwargs) -> bool:
         return False
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/matrix/bayes.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/matrix/bayes.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,25 +12,26 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Dict, List, Optional, Union
 from typing_extensions import Literal
 
-from clipped.enums_utils import PEnum
+from clipped.config.schema import skip_partial
+from clipped.types.ref_or_obj import RefField
+from clipped.utils.enums import PEnum
 from pydantic import Field, PositiveInt, StrictInt, root_validator, validator
 
 from polyaxon.polyflow.early_stopping import V1EarlyStopping
 from polyaxon.polyflow.matrix.base import BaseSearchConfig
 from polyaxon.polyflow.matrix.kinds import V1MatrixKind
 from polyaxon.polyflow.matrix.params import V1HpParam
 from polyaxon.polyflow.matrix.tuner import V1Tuner
 from polyaxon.polyflow.optimization import V1OptimizationMetric
-from polyaxon.schemas.base import BaseSchemaModel, skip_partial
-from polyaxon.schemas.fields import RefField
+from polyaxon.schemas.base import BaseSchemaModel
 
 
 class AcquisitionFunctions(str, PEnum):
     UCB = "ucb"
     EI = "ei"
     POI = "poi"
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/matrix/grid_search.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/matrix/grid_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,22 +12,22 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Dict, List, Optional, Union
 from typing_extensions import Literal
 
+from clipped.config.schema import skip_partial
+from clipped.types.ref_or_obj import RefField
 from pydantic import Field, PositiveInt, validator
 
 from polyaxon.polyflow.early_stopping import V1EarlyStopping
 from polyaxon.polyflow.matrix.base import BaseSearchConfig
 from polyaxon.polyflow.matrix.kinds import V1MatrixKind
 from polyaxon.polyflow.matrix.params import V1HpParam
-from polyaxon.schemas.base import skip_partial
-from polyaxon.schemas.fields.ref_or_obj import RefField
 
 
 def validate_matrix(matrix):
     if not matrix:
         return None
 
     for key, value in matrix.items():
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/matrix/hyperband.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/matrix/hyperband.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,23 +14,23 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import math
 
 from typing import Dict, List, Optional, Tuple, Union
 from typing_extensions import Literal
 
+from clipped.types.ref_or_obj import BoolOrRef, IntOrRef, RefField
 from pydantic import Field, NonNegativeFloat, PositiveInt, PrivateAttr
 
 from polyaxon.polyflow.early_stopping import V1EarlyStopping
 from polyaxon.polyflow.matrix.base import BaseSearchConfig
 from polyaxon.polyflow.matrix.kinds import V1MatrixKind
 from polyaxon.polyflow.matrix.params import V1HpParam
 from polyaxon.polyflow.matrix.tuner import V1Tuner
 from polyaxon.polyflow.optimization import V1OptimizationMetric, V1OptimizationResource
-from polyaxon.schemas.fields.ref_or_obj import BoolOrRef, IntOrRef, RefField
 
 
 class V1Hyperband(BaseSearchConfig):
     """Hyperband is a relatively new method for tuning iterative algorithms.
     It performs random sampling and attempts to gain an edge
     by using time spent optimizing in the best way.
 
@@ -82,25 +82,24 @@
     >>>   tuner:
     >>>   earlyStopping:
     ```
 
     ## Python usage
 
     ```python
-    >>> from polyaxon import types
     >>> from polyaxon.polyflow import (
     >>>     V1Hyperband, V1HpLogSpace, V1HpChoice, V1FailureEarlyStopping, V1MetricEarlyStopping,
     >>>     V1OptimizationMetric, V1Optimization, V1OptimizationResource,
     >>> )
     >>> matrix = V1Hyperband(
     >>>   concurrency=20,
     >>>   params={"param1": V1HpLogSpace(...), "param2": V1HpChoice(...), ... },
     >>>   resume=True,
     >>>   metric=V1OptimizationMetric(name="loss", optimization=V1Optimization.MINIMIZE),
-    >>>   resource=V1OptimizationResource(name="num_steps", type=types.INT),
+    >>>   resource=V1OptimizationResource(name="num_steps", type='int'),
     >>>   early_stopping=[V1FailureEarlyStopping(...), V1MetricEarlyStopping(...)]
     >>> )
     ```
 
     ## Fields
 
     ### kind
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/matrix/hyperopt.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/matrix/hyperopt.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,24 +12,24 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Dict, List, Optional, Union
 from typing_extensions import Literal
 
-from clipped.enums_utils import PEnum
+from clipped.types.ref_or_obj import IntOrRef, RefField
+from clipped.utils.enums import PEnum
 from pydantic import Field, PositiveInt, validator
 
 from polyaxon.polyflow.early_stopping import V1EarlyStopping
 from polyaxon.polyflow.matrix.base import BaseSearchConfig
 from polyaxon.polyflow.matrix.kinds import V1MatrixKind
 from polyaxon.polyflow.matrix.params import V1HpParam
 from polyaxon.polyflow.matrix.tuner import V1Tuner
 from polyaxon.polyflow.optimization import V1OptimizationMetric
-from polyaxon.schemas.fields.ref_or_obj import IntOrRef, RefField
 
 
 class V1HyperoptAlgorithms(str, PEnum):
     TPE = "tpe"
     RAND = "rand"
     ANNEAL = "anneal"
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/matrix/iterative.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/matrix/iterative.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,22 +12,22 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Dict, List, Optional, Union
 from typing_extensions import Literal
 
+from clipped.types.ref_or_obj import IntOrRef, RefField
 from pydantic import Field, PositiveInt, validator
 
 from polyaxon.polyflow.early_stopping import V1EarlyStopping
 from polyaxon.polyflow.matrix.base import BaseSearchConfig
 from polyaxon.polyflow.matrix.kinds import V1MatrixKind
 from polyaxon.polyflow.matrix.params import V1HpParam
 from polyaxon.polyflow.matrix.tuner import V1Tuner
-from polyaxon.schemas.fields.ref_or_obj import IntOrRef, RefField
 
 
 class V1Iterative(BaseSearchConfig):
     """To build a custom optimization algorithm, this interface lets you create an iterative
     process for creating suggestions and training your model based on those suggestions
 
     The iterative process expect a user defined a tuner that will generate the suggestions for
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/matrix/kinds.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/matrix/kinds.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from clipped.enums_utils import PEnum
+from clipped.utils.enums import PEnum
 
 
 class V1MatrixKind(str, PEnum):
     RANDOM = "random"
     GRID = "grid"
     HYPERBAND = "hyperband"
     BAYES = "bayes"
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/matrix/mapping.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/matrix/mapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,20 +12,20 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Dict, List, Optional, Union
 from typing_extensions import Literal
 
+from clipped.types.ref_or_obj import RefField
 from pydantic import Field, PositiveInt, validator
 
 from polyaxon.polyflow.early_stopping import V1EarlyStopping
 from polyaxon.polyflow.matrix.base import BaseSearchConfig
 from polyaxon.polyflow.matrix.kinds import V1MatrixKind
-from polyaxon.schemas.fields.ref_or_obj import RefField
 
 
 class V1Mapping(BaseSearchConfig):
     """Mapping is a flexible way for dynamically executing a component sequentially or in parallel
     based on a list of parameter combinations.
 
     Args:
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/matrix/params.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/matrix/params.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,23 +11,28 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from datetime import date, datetime, timedelta
-from typing import Any, List, Optional, Union
+from typing import TYPE_CHECKING, Any, List, Optional, Union
 from typing_extensions import Annotated, Literal
 
+from clipped.config.schema import skip_partial
+from clipped.types.numbers import StrictIntOrFloat
+from clipped.types.ref_or_obj import RefField
 from pydantic import Field, StrictStr, root_validator, validator
 
 from polyaxon import types
 from polyaxon.polyflow.matrix.kinds import V1HPKind
-from polyaxon.schemas.base import BaseDiscriminatedModel, BaseSchemaModel, skip_partial
-from polyaxon.schemas.fields import RefField, StrictIntOrFloat
+from polyaxon.schemas.base import BaseSchemaModel
+
+if TYPE_CHECKING:
+    from pydantic.typing import CallableGenerator
 
 try:
     import numpy as np
 except (ImportError, ModuleNotFoundError):
     np = None
 
 
@@ -347,18 +352,20 @@
     v = sum(map(lambda x: 1 if x else 0, values))
     if v == 0 or v > 1:
         raise ValueError(
             "Matrix element is not valid, one and only one option is required."
         )
 
 
-class BaseHpParamConfig(BaseDiscriminatedModel):
+class BaseHpParamConfig(BaseSchemaModel):
+    _USE_DISCRIMINATOR = True
+
     @staticmethod
     def validate_io(io: "V1IO"):  # noqa
-        if io.type not in [types.INT, types.FLOAT]:
+        if io.type not in ["int", "float"]:
             raise ValueError(
                 "Param `{}` has a an input type `{}` "
                 "and it does not correspond to hyper-param type `int or float`.".format(
                     io.name,
                     io.type,
                 )
             )
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/matrix/random_search.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/matrix/random_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,21 +12,21 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Dict, List, Optional, Union
 from typing_extensions import Literal
 
+from clipped.types.ref_or_obj import IntOrRef, RefField
 from pydantic import Field, PositiveInt, validator
 
 from polyaxon.polyflow.early_stopping import V1EarlyStopping
 from polyaxon.polyflow.matrix.base import BaseSearchConfig
 from polyaxon.polyflow.matrix.kinds import V1MatrixKind
 from polyaxon.polyflow.matrix.params import V1HpParam
-from polyaxon.schemas.fields.ref_or_obj import IntOrRef, RefField
 
 
 class V1RandomSearch(BaseSearchConfig):
     """Random search creates a number of unique experiments by sampling randomly
     from a search space.
     Random search is a competitive method for black-box parameter tuning in machine learning.
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/matrix/tuner.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/matrix/tuner.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Dict, List, Optional, Union
 
+from clipped.types.ref_or_obj import RefField
 from pydantic import Field, StrictStr
 
 from polyaxon.polyflow.params import V1Param
 from polyaxon.schemas.base import BaseSchemaModel
-from polyaxon.schemas.fields.ref_or_obj import RefField
 
 
 class V1Tuner(BaseSchemaModel):
     """You can configure Polyaxon to use a custom tuner to customize the built-in optimizers.
 
     The tuner allows you to customize the behavior of the operations that
     generate new suggestions based on the previous observations.
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/mounts/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/sidecar/container/monitors/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,8 +10,9 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from polyaxon.polyflow.mounts.artifacts_mounts import V1ArtifactsMount
+from polyaxon.sidecar.container.monitors.artifacts import sync_artifacts
+from polyaxon.sidecar.container.monitors.logs import sync_logs
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/mounts/artifacts_mounts.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/mounts/artifacts_mounts.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/notifications/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/operations/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/operations/base.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/operations/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,25 +11,25 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Dict, List, Optional, Set, Union
 
+from clipped.types.ref_or_obj import RefField
 from pydantic import Field, StrictStr
 
 from polyaxon.contexts import refs as ctx_refs
 from polyaxon.lifecycle import V1Statuses
 from polyaxon.polyflow.component.base import BaseComponent
 from polyaxon.polyflow.events import V1EventKind, V1EventTrigger
 from polyaxon.polyflow.joins import V1Join
 from polyaxon.polyflow.matrix import MatrixMixin, V1Matrix
 from polyaxon.polyflow.schedules import ScheduleMixin, V1Schedule
 from polyaxon.polyflow.trigger_policies import V1TriggerPolicy
-from polyaxon.schemas.fields import RefField
 
 
 class BaseOp(BaseComponent, MatrixMixin, ScheduleMixin):
     _FIELDS_SAME_KIND_PATCH = ["schedule", "matrix"]
 
     schedule: Optional[V1Schedule]
     events: Optional[Union[List[V1EventTrigger], RefField]]
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/operations/compiled_operation.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/operations/compiled_operation.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/operations/operation.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/operations/operation.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,26 +13,26 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from copy import copy
 from typing import Dict, Optional
 from typing_extensions import Literal
 
+from clipped.config.patch_strategy import PatchStrategy
+from clipped.config.schema import skip_partial, to_partial
 from pydantic import Field, StrictStr, root_validator, validator
 
 from polyaxon.polyflow.builds import V1Build
 from polyaxon.polyflow.component.component import V1Component
 from polyaxon.polyflow.hooks import V1Hook
 from polyaxon.polyflow.operations.base import BaseOp
 from polyaxon.polyflow.params import V1Param
 from polyaxon.polyflow.references import V1DagRef, V1HubRef, V1PathRef, V1UrlRef
 from polyaxon.polyflow.run.patch import validate_run_patch
 from polyaxon.polyflow.templates import TemplateMixinConfig, V1Template
-from polyaxon.schemas.base import skip_partial, to_partial
-from polyaxon.schemas.patch_strategy import V1PatchStrategy
 
 
 class V1Operation(BaseOp, TemplateMixinConfig):
     """An operation is how Polyaxon executes a component by passing parameters,
     connections, and a run environment.
 
     With an operation users can:
@@ -510,15 +510,15 @@
     kind: Literal[_IDENTIFIER] = _IDENTIFIER
     params: Optional[Dict[StrictStr, V1Param]]
     hub_ref: Optional[StrictStr] = Field(alias="hubRef")
     dag_ref: Optional[StrictStr] = Field(alias="dagRef")
     url_ref: Optional[StrictStr] = Field(alias="urlRef")
     path_ref: Optional[StrictStr] = Field(alias="pathRef")
     component: Optional[V1Component]
-    patch_strategy: Optional[V1PatchStrategy] = Field(alias="patchStrategy")
+    patch_strategy: Optional[PatchStrategy] = Field(alias="patchStrategy")
     is_preset: Optional[bool] = Field(alias="isPreset")
     run_patch: Optional[Dict] = Field(alias="runPatch")
     template: Optional[V1Template]
 
     @root_validator
     @skip_partial
     def validate_reference(cls, values):
@@ -608,16 +608,16 @@
         if self.has_url_reference:
             return V1UrlRef(url=self.url_ref)
 
     def set_definition(self, value):
         self.component = value
 
     @classmethod
-    def patch_obj(cls, config, values, strategy: V1PatchStrategy = None):
-        strategy = strategy or V1PatchStrategy.POST_MERGE
+    def patch_obj(cls, config, values, strategy: PatchStrategy = None):
+        strategy = strategy or PatchStrategy.POST_MERGE
 
         result = super().patch_obj(config, values, strategy)
         value = getattr(values, "run_patch", None)
         if value is None:
             return result
 
         current_value = getattr(config, "run_patch", None)
@@ -627,17 +627,17 @@
 
         if (
             not config.component
             or not config.component.run
             or not config.component.run.kind
         ):
             # We don't have a kind, we don't do anything
-            if V1PatchStrategy.is_null(strategy):
+            if PatchStrategy.is_null(strategy):
                 return result
-            if V1PatchStrategy.is_replace(strategy):
+            if PatchStrategy.is_replace(strategy):
                 setattr(result, "run_patch", value)
                 return result
             return result
 
         kind = config.component.run.kind
         value = validate_run_patch(value, kind)
         current_value = validate_run_patch(current_value, kind)
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/operators.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/operators.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/optimization/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/optimization/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Optional
 
-from clipped.enums_utils import PEnum
+from clipped.utils.enums import PEnum
 from pydantic import StrictStr
 
 from polyaxon.schemas.base import BaseSchemaModel
 
 
 class V1ResourceType(str, PEnum):
     INT = "int"
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/params/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/params/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/params/ops_params.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/params/ops_params.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/params/params.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/params/params.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,25 +14,26 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from collections import namedtuple
 from collections.abc import Mapping
 from typing import Any, Dict, Optional
 
-from clipped.list_utils import to_list
+from clipped.config.schema import skip_partial
+from clipped.utils.lists import to_list
+from clipped.utils.strings import to_string
 from pydantic import Field, StrictStr, validator
 
 from polyaxon import types
 from polyaxon.contexts import refs as ctx_refs
 from polyaxon.contexts import sections as ctx_sections
 from polyaxon.contexts.params import PARAM_REGEX
 from polyaxon.exceptions import PolyaxonValidationError
-from polyaxon.parser import parser
 from polyaxon.polyflow.init import V1Init
-from polyaxon.schemas.base import BaseSchemaModel, skip_partial
+from polyaxon.schemas.base import BaseSchemaModel
 
 
 def validate_param_value(value, ref):
     if ref and not isinstance(value, str):
         raise TypeError(
             "Value must be of type string when a ref is provided, received `{}` instead.".format(
                 value
@@ -420,31 +421,31 @@
         return ref
 
 
 class ParamSpec(
     namedtuple("ParamSpec", "name type param is_flag is_list is_context arg_format")
 ):
     def get_typed_param_value(self):
-        if self.type == types.STR:
+        if self.type == "str":
             if self.is_list:
                 value = self.param.value or []  # Handles the case of None
-                return [parser.parse_string(v) for v in value]
-            return parser.parse_string(self.param.value)
+                return [to_string(v) for v in value]
+            return to_string(self.param.value)
         return self.param.value
 
     def get_display_value(self):
         if self.is_flag:
             return "--{}".format(self.name) if self.param.value else ""
         return self.get_typed_param_value()
 
     def __repr__(self):
         value = self.get_display_value()
         if value is None:
             return ""
-        return parser.parse_string(value)
+        return to_string(value)
 
     def as_str(self):
         return str(self)
 
     def as_arg(self):
         if self.arg_format:
             from polyaxon.polyaxonfile.specs.libs.parser import Parser
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/plugins/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/plugins/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import List, Optional, Union
 
+from clipped.types.ref_or_obj import BoolOrRef, RefField
 from pydantic import Field, StrictStr
 
 from polyaxon.auxiliaries.sidecar import V1PolyaxonSidecarContainer
 from polyaxon.polyflow.notifications import V1Notification
 from polyaxon.schemas.base import BaseSchemaModel
-from polyaxon.schemas.fields.ref_or_obj import BoolOrRef, RefField
 
 
 class V1Plugins(BaseSchemaModel):
     """Plugins section provides a way to customize extra Polyaxon utilities.
 
     By default, Polyaxon injects some information for example an auth context
     and triggers some mechanisms for collecting logs and outputs.
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/references/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/references/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/references/dag.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/references/dag.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,18 +14,19 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing_extensions import Literal
 
 from pydantic import StrictStr
 
 from polyaxon.polyflow.references.mixin import RefMixin
-from polyaxon.schemas.base import BaseDiscriminatedModel
+from polyaxon.schemas.base import BaseSchemaModel
 
 
-class V1DagRef(BaseDiscriminatedModel, RefMixin):
+class V1DagRef(BaseSchemaModel, RefMixin):
     _IDENTIFIER = "dag_ref"
+    _USE_DISCRIMINATOR = True
 
     kind: Literal[_IDENTIFIER] = _IDENTIFIER
     name: StrictStr
 
     def get_kind_value(self):
         return self.name
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/references/hub.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/references/hub.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,18 +14,19 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing_extensions import Literal
 
 from pydantic import StrictStr
 
 from polyaxon.polyflow.references.mixin import RefMixin
-from polyaxon.schemas.base import BaseDiscriminatedModel
+from polyaxon.schemas.base import BaseSchemaModel
 
 
-class V1HubRef(BaseDiscriminatedModel, RefMixin):
+class V1HubRef(BaseSchemaModel, RefMixin):
     _IDENTIFIER = "hub_ref"
+    _USE_DISCRIMINATOR = True
 
     kind: Literal[_IDENTIFIER] = _IDENTIFIER
     name: StrictStr
 
     def get_kind_value(self):
         return self.name
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/references/mixin.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/references/mixin.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/references/path.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/references/url.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 from typing_extensions import Literal
 
 from pydantic import StrictStr
 
 from polyaxon.polyflow.references.mixin import RefMixin
-from polyaxon.schemas.base import BaseDiscriminatedModel
+from polyaxon.schemas.base import BaseSchemaModel
 
 
-class V1PathRef(BaseDiscriminatedModel, RefMixin):
-    _IDENTIFIER = "path_ref"
+class V1UrlRef(BaseSchemaModel, RefMixin):
+    _IDENTIFIER = "url_ref"
+    _USE_DISCRIMINATOR = True
 
     kind: Literal[_IDENTIFIER] = _IDENTIFIER
-    path: StrictStr
+    url: StrictStr
 
     def get_kind_value(self):
-        return self.path
+        return self.url
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/references/url.py` & `polyaxon-2.0.0rc8/polyaxon/tracking/run.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,23 +9,11 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from typing_extensions import Literal
 
-from pydantic import StrictStr
+# To keep backwards compatibility
 
-from polyaxon.polyflow.references.mixin import RefMixin
-from polyaxon.schemas.base import BaseDiscriminatedModel
-
-
-class V1UrlRef(BaseDiscriminatedModel, RefMixin):
-    _IDENTIFIER = "url_ref"
-
-    kind: Literal[_IDENTIFIER] = _IDENTIFIER
-    url: StrictStr
-
-    def get_kind_value(self):
-        return self.url
+from traceml.tracking.run import Run
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/run/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/run/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/run/base.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/run/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,18 +9,20 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from polyaxon.schemas.base import BaseDiscriminatedModel
+from polyaxon.schemas.base import BaseSchemaModel
 
 
-class BaseRun(BaseDiscriminatedModel):
+class BaseRun(BaseSchemaModel):
+    _USE_DISCRIMINATOR = True
+
     def get_resources(self):
         raise NotImplementedError
 
     def get_all_containers(self):
         raise NotImplementedError
 
     def get_all_connections(self):
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/run/cleaner.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/run/cleaner.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/run/dag.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/run/dag.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,29 +14,29 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from collections.abc import Mapping
 from typing import Any, Dict, ForwardRef, List, Optional, Set, Union
 from typing_extensions import Literal
 
+from clipped.types.ref_or_obj import RefField
 from pydantic import Field, PositiveInt, PrivateAttr, StrictStr, validator
 
 from polyaxon import types
 from polyaxon.contexts import sections as ctx_sections
 from polyaxon.exceptions import PolyaxonSchemaError
 from polyaxon.k8s import k8s_schemas, k8s_validation
 from polyaxon.pkg import SCHEMA_VERSION
 from polyaxon.polyflow import dags
 from polyaxon.polyflow.early_stopping import V1EarlyStopping
 from polyaxon.polyflow.environment import V1Environment
 from polyaxon.polyflow.io import V1IO
 from polyaxon.polyflow.params import ops_params
 from polyaxon.polyflow.run.base import BaseRun
 from polyaxon.polyflow.run.kinds import V1RunKind
-from polyaxon.schemas.fields.ref_or_obj import RefField
 
 V1Operation = ForwardRef("V1Operation")
 V1Component = ForwardRef("V1Component")
 
 
 class V1Dag(BaseRun):
     """Dag (Directed Acyclic Graphs) is
@@ -447,26 +447,24 @@
         during tests with hub_ref.
         """
         inputs = inputs or []
 
         for g_context in ctx_sections.GLOBALS_CONTEXTS:
             self._context[
                 "dag.{}.{}".format(ctx_sections.GLOBALS, g_context)
-            ] = V1IO.construct(
-                name=g_context, type=types.STR, value="", is_optional=True
-            )
+            ] = V1IO.construct(name=g_context, type="str", value="", is_optional=True)
 
         self._context["dag.{}".format(ctx_sections.INPUTS)] = V1IO.construct(
-            name="inputs", type=types.DICT, value={}, is_optional=True
+            name="inputs", type="dict", value={}, is_optional=True
         )
         self._context["dag.{}".format(ctx_sections.GLOBALS)] = V1IO.construct(
-            name="globals", type=types.STR, value="", is_optional=True
+            name="globals", type="str", value="", is_optional=True
         )
         self._context["dag.{}".format(ctx_sections.ARTIFACTS)] = V1IO.construct(
-            name="artifacts", type=types.STR, value="", is_optional=True
+            name="artifacts", type="str", value="", is_optional=True
         )
 
         for _input in inputs:
             self._context["dag.inputs.{}".format(_input.name)] = _input
 
         if not self.operations:
             raise PolyaxonSchemaError(
@@ -540,41 +538,33 @@
                                 op_name, ctx_sections.ARTIFACTS, cinput.name
                             )
                         ] = cinput
             for g_context in ctx_sections.GLOBALS_CONTEXTS:
                 self._context[
                     "ops.{}.{}.{}".format(op_name, ctx_sections.GLOBALS, g_context)
                 ] = V1IO.construct(
-                    name=g_context, type=types.STR, value="", is_optional=True
+                    name=g_context, type="str", value="", is_optional=True
                 )
 
             # We allow to resolve name, status, project, all outputs/inputs, iteration
             self._context[
                 "ops.{}.{}".format(op_name, ctx_sections.INPUTS)
-            ] = V1IO.construct(
-                name="inputs", type=types.DICT, value={}, is_optional=True
-            )
+            ] = V1IO.construct(name="inputs", type="dict", value={}, is_optional=True)
             self._context[
                 "ops.{}.{}".format(op_name, ctx_sections.OUTPUTS)
-            ] = V1IO.construct(
-                name="outputs", type=types.DICT, value={}, is_optional=True
-            )
+            ] = V1IO.construct(name="outputs", type="dict", value={}, is_optional=True)
             self._context[
                 "ops.{}.{}".format(op_name, ctx_sections.GLOBALS)
-            ] = V1IO.construct(
-                name="globals", type=types.STR, value="", is_optional=True
-            )
+            ] = V1IO.construct(name="globals", type="str", value="", is_optional=True)
             self._context[
                 "ops.{}.{}".format(op_name, ctx_sections.ARTIFACTS)
-            ] = V1IO.construct(
-                name="artifacts", type=types.STR, value="", is_optional=True
-            )
+            ] = V1IO.construct(name="artifacts", type="str", value="", is_optional=True)
             self._context[
                 "ops.{}.{}".format(op_name, ctx_sections.INPUTS_OUTPUTS)
-            ] = V1IO.construct(name="io", type=types.STR, value={}, is_optional=True)
+            ] = V1IO.construct(name="io", type="str", value={}, is_optional=True)
 
         for op in self.operations:
             if op.has_component_reference:
                 component_ref = op.definition.name
                 outputs = op.definition.outputs
                 inputs = op.definition.inputs
             elif op.has_dag_reference:
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/run/dask.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/run/dask.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,22 +12,22 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import List, Optional, Union
 from typing_extensions import Literal
 
+from clipped.types.ref_or_obj import IntOrRef, RefField
 from pydantic import Field, StrictStr, validator
 
 from polyaxon.k8s import k8s_schemas, k8s_validation
 from polyaxon.polyflow.environment import V1Environment
 from polyaxon.polyflow.init import V1Init
 from polyaxon.polyflow.run.base import BaseRun
 from polyaxon.polyflow.run.kinds import V1RunKind
-from polyaxon.schemas.fields import IntOrRef, RefField
 
 
 class V1Dask(BaseRun):
     """Dask jobs are used to run distributed jobs using a
     [Dask cluster](https://kubernetes.dask.org/en/latest/).
 
     > Dask Kubernetes deploys Dask workers on Kubernetes clusters using native Kubernetes APIs.
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/run/flink.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/run/flink.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,17 +12,18 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Dict, Union
 from typing_extensions import Literal
 
+from clipped.types.ref_or_obj import RefField
+
 from polyaxon.polyflow.run.base import BaseRun
 from polyaxon.polyflow.run.kinds import V1RunKind
-from polyaxon.schemas.fields.ref_or_obj import RefField
 
 
 class V1Flink(BaseRun):
     _IDENTIFIER = V1RunKind.FLINK
 
     kind: Literal[_IDENTIFIER] = _IDENTIFIER
     spec: Union[Dict, RefField]
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/run/job.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/run/job.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,24 +12,24 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import List, Optional, Union
 from typing_extensions import Literal
 
+from clipped.types.ref_or_obj import RefField
 from pydantic import StrictStr, validator
 
 from polyaxon.k8s import k8s_schemas, k8s_validation
 from polyaxon.polyflow.environment import V1Environment
 from polyaxon.polyflow.init import V1Init
 from polyaxon.polyflow.run.base import BaseRun
 from polyaxon.polyflow.run.kinds import V1RunKind
 from polyaxon.polyflow.run.resources import V1RunResources
 from polyaxon.polyflow.run.utils import DestinationImageMixin
-from polyaxon.schemas.fields import RefField
 
 
 class V1Job(BaseRun, DestinationImageMixin):
     """Jobs are used to train machine learning models,
     process a dataset, execute generic tasks and can be used to perform a variety of functions
     from compiling a model to running an ETL operation.
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/run/kinds.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/run/kinds.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from clipped.enums_utils import PEnum
+from clipped.utils.enums import PEnum
 
 
 class V1RunKind(str, PEnum):
     JOB = "job"
     SERVICE = "service"
     DAG = "dag"
     SPARK = "spark"
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/run/kubeflow/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/run/spark/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/run/kubeflow/clean_pod_policy.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_events_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from typing import Any, Dict, List, Optional
 
-from clipped.enums_utils import PEnum
+from polyaxon.schemas.base import BaseSchemaModel
 
 
-class V1CleanPodPolicy(str, PEnum):
-    ALL = "All"
-    RUNNING = "Running"
-    var_NONE = "None"
+class V1EventsResponse(BaseSchemaModel):
+    data: Optional[List[Dict[str, Any]]]
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/run/kubeflow/mpi_job.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/run/kubeflow/mpi_job.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,25 +12,25 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Optional, Union
 from typing_extensions import Literal
 
+from clipped.types.ref_or_obj import IntOrRef, RefField
 from pydantic import Field
 
 from polyaxon.k8s.k8s_schemas import V1Container
 from polyaxon.polyflow.run.base import BaseRun
 from polyaxon.polyflow.run.kinds import V1RunKind
 from polyaxon.polyflow.run.kubeflow.clean_pod_policy import V1CleanPodPolicy
 from polyaxon.polyflow.run.kubeflow.replica import V1KFReplica
 from polyaxon.polyflow.run.kubeflow.scheduling_policy import V1SchedulingPolicy
 from polyaxon.polyflow.run.resources import V1RunResources
 from polyaxon.polyflow.run.utils import DestinationImageMixin
-from polyaxon.schemas.fields import IntOrRef, RefField
 
 
 class V1MPIJob(BaseRun, DestinationImageMixin):
     """Kubeflow MPI-Job provides an interface to train distributed experiments with MPI.
 
     Args:
         kind: str, should be equal `mpijob`
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/run/kubeflow/mx_job.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/run/kubeflow/mx_job.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,26 +12,26 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Optional, Union
 from typing_extensions import Literal
 
-from clipped.enums_utils import PEnum
+from clipped.types.ref_or_obj import RefField
+from clipped.utils.enums import PEnum
 from pydantic import Field
 
 from polyaxon.k8s.k8s_schemas import V1Container
 from polyaxon.polyflow.run.base import BaseRun
 from polyaxon.polyflow.run.kinds import V1RunKind
 from polyaxon.polyflow.run.kubeflow.clean_pod_policy import V1CleanPodPolicy
 from polyaxon.polyflow.run.kubeflow.replica import V1KFReplica
 from polyaxon.polyflow.run.kubeflow.scheduling_policy import V1SchedulingPolicy
 from polyaxon.polyflow.run.resources import V1RunResources
 from polyaxon.polyflow.run.utils import DestinationImageMixin
-from polyaxon.schemas.fields import RefField
 
 
 class MXJobMode(str, PEnum):
     MX_TRAIN = "MXTrain"
     MX_TUNE = "MXTune"
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/run/kubeflow/paddle_job.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/run/kubeflow/paddle_job.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,25 +12,25 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Optional, Union
 from typing_extensions import Literal
 
+from clipped.types.ref_or_obj import RefField
 from pydantic import Field
 
 from polyaxon.k8s.k8s_schemas import V1Container
 from polyaxon.polyflow.run.base import BaseRun
 from polyaxon.polyflow.run.kinds import V1RunKind
 from polyaxon.polyflow.run.kubeflow.clean_pod_policy import V1CleanPodPolicy
 from polyaxon.polyflow.run.kubeflow.replica import V1KFReplica
 from polyaxon.polyflow.run.kubeflow.scheduling_policy import V1SchedulingPolicy
 from polyaxon.polyflow.run.resources import V1RunResources
 from polyaxon.polyflow.run.utils import DestinationImageMixin
-from polyaxon.schemas.fields import RefField
 
 
 class V1PaddleJob(BaseRun, DestinationImageMixin):
     """Kubeflow PaddlePaddle-Job provides an interface to train distributed
     experiments with PaddlePaddle.
 
     Args:
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/run/kubeflow/pytorch_job.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/run/kubeflow/pytorch_job.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,25 +12,25 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Optional, Union
 from typing_extensions import Literal
 
+from clipped.types.ref_or_obj import RefField
 from pydantic import Field
 
 from polyaxon.k8s.k8s_schemas import V1Container
 from polyaxon.polyflow.run.base import BaseRun
 from polyaxon.polyflow.run.kinds import V1RunKind
 from polyaxon.polyflow.run.kubeflow.clean_pod_policy import V1CleanPodPolicy
 from polyaxon.polyflow.run.kubeflow.replica import V1KFReplica
 from polyaxon.polyflow.run.kubeflow.scheduling_policy import V1SchedulingPolicy
 from polyaxon.polyflow.run.resources import V1RunResources
 from polyaxon.polyflow.run.utils import DestinationImageMixin
-from polyaxon.schemas.fields import RefField
 
 
 class V1PytorchJob(BaseRun, DestinationImageMixin):
     """Kubeflow Pytorch-Job provides an interface to train distributed experiments with Pytorch.
 
     Args:
         kind: str, should be equal `pytorchjob`
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/run/kubeflow/replica.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/run/kubeflow/replica.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import List, Optional, Union
 
+from clipped.types.ref_or_obj import IntOrRef, RefField
 from pydantic import StrictStr, validator
 
 from polyaxon.k8s import k8s_schemas, k8s_validation
 from polyaxon.polyflow.environment import V1Environment
 from polyaxon.polyflow.init import V1Init
 from polyaxon.polyflow.run.resources import V1RunResources
 from polyaxon.schemas.base import BaseSchemaModel
-from polyaxon.schemas.fields import IntOrRef, RefField
 
 
 class V1KFReplica(BaseSchemaModel):
     """Kubeflow-Replica provides an interface to define a replica for
     TFJob/MPIJob/PytorchJob/PaddleJob/MXJob/XGBoostJob.
 
     Args:
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/run/kubeflow/scheduling_policy.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/run/kubeflow/scheduling_policy.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Optional
 
+from clipped.types.ref_or_obj import IntOrRef
 from pydantic import Field, StrictStr
 
 from polyaxon.schemas.base import BaseSchemaModel
-from polyaxon.schemas.fields import IntOrRef
 
 
 class V1SchedulingPolicy(BaseSchemaModel):
     _IDENTIFIER = "schedulingPolicy"
 
     min_available: Optional[IntOrRef] = Field(alias="minAvailable")
     queue: Optional[StrictStr]
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/run/kubeflow/tf_job.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/run/kubeflow/tf_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,25 +12,25 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Optional, Union
 from typing_extensions import Literal
 
+from clipped.types.ref_or_obj import RefField
 from pydantic import Field
 
 from polyaxon.k8s.k8s_schemas import V1Container
 from polyaxon.polyflow.run.base import BaseRun
 from polyaxon.polyflow.run.kinds import V1RunKind
 from polyaxon.polyflow.run.kubeflow.clean_pod_policy import V1CleanPodPolicy
 from polyaxon.polyflow.run.kubeflow.replica import V1KFReplica
 from polyaxon.polyflow.run.kubeflow.scheduling_policy import V1SchedulingPolicy
 from polyaxon.polyflow.run.resources import V1RunResources
 from polyaxon.polyflow.run.utils import DestinationImageMixin
-from polyaxon.schemas.fields import RefField
 
 
 class V1TFJob(BaseRun, DestinationImageMixin):
     """Kubeflow TF-Job provides an interface to train distributed experiments with TensorFlow.
 
     Args:
         kind: str, should be equal `tfjob`
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/run/kubeflow/xgboost_job.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/run/kubeflow/xgboost_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,25 +12,25 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Optional, Union
 from typing_extensions import Literal
 
+from clipped.types.ref_or_obj import RefField
 from pydantic import Field
 
 from polyaxon.k8s.k8s_schemas import V1Container
 from polyaxon.polyflow.run.base import BaseRun
 from polyaxon.polyflow.run.kinds import V1RunKind
 from polyaxon.polyflow.run.kubeflow.clean_pod_policy import V1CleanPodPolicy
 from polyaxon.polyflow.run.kubeflow.replica import V1KFReplica
 from polyaxon.polyflow.run.kubeflow.scheduling_policy import V1SchedulingPolicy
 from polyaxon.polyflow.run.resources import V1RunResources
 from polyaxon.polyflow.run.utils import DestinationImageMixin
-from polyaxon.schemas.fields import RefField
 
 
 class V1XGBoostJob(BaseRun, DestinationImageMixin):
     """Kubeflow XGBoost-Job provides an interface to train distributed experiments with XGBoost.
 
     Args:
         kind: str, should be equal `xgbjob`
@@ -49,17 +49,17 @@
     >>>   master:
     >>>   worker:
     ```
 
     ## Python usage
 
     ```python
-    >>> from polyaxon.polyflow import V1KFReplica, V1XGBoost
+    >>> from polyaxon.polyflow import V1KFReplica, V1XGBoostJob
     >>> from polyaxon.k8s import k8s_schemas
-    >>> xgb_job = V1XGBoost(
+    >>> xgb_job = V1XGBoostJob(
     >>>     clean_pod_policy='All',
     >>>     master=V1KFReplica(...),
     >>>     worker=V1KFReplica(...),
     >>> )
     ```
 
     ## Fields
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/run/notifier.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/run/notifier.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/run/patch.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/run/patch.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/run/ray.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/run/ray.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,17 +12,18 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Dict, Union
 from typing_extensions import Literal
 
+from clipped.types.ref_or_obj import RefField
+
 from polyaxon.polyflow.run.base import BaseRun
 from polyaxon.polyflow.run.kinds import V1RunKind
-from polyaxon.schemas.fields.ref_or_obj import RefField
 
 
 class V1Ray(BaseRun):
     _IDENTIFIER = V1RunKind.FLINK
 
     kind: Literal[_IDENTIFIER] = _IDENTIFIER
     spec: Union[Dict, RefField]
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/run/resources.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/run/resources.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Optional, Union
 
+from clipped.types.numbers import StrictIntOrFloat
+from clipped.utils.units import to_cpu_value, to_memory_bytes
 from pydantic import StrictStr
 
 from polyaxon.k8s.k8s_schemas import V1Container
 from polyaxon.schemas.base import BaseSchemaModel
-from polyaxon.schemas.fields import StrictIntOrFloat
-from traceml.processors.units_processors import to_cpu_value, to_memory_bytes
 
 
 class V1RunResources(BaseSchemaModel):
     cpu: Optional[Union[StrictIntOrFloat, StrictStr]]
     memory: Optional[Union[StrictIntOrFloat, StrictStr]]
     gpu: Optional[Union[StrictIntOrFloat, StrictStr]]
     custom: Optional[Union[StrictIntOrFloat, StrictStr]]
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/run/service.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/run/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,24 +12,24 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import List, Optional, Union
 from typing_extensions import Literal
 
+from clipped.types.ref_or_obj import BoolOrRef, IntOrRef, RefField
 from pydantic import Field, StrictInt, StrictStr, validator
 
 from polyaxon.k8s import k8s_schemas, k8s_validation
 from polyaxon.polyflow.environment import V1Environment
 from polyaxon.polyflow.init import V1Init
 from polyaxon.polyflow.run.base import BaseRun
 from polyaxon.polyflow.run.kinds import V1RunKind
 from polyaxon.polyflow.run.resources import V1RunResources
 from polyaxon.polyflow.run.utils import DestinationImageMixin
-from polyaxon.schemas.fields.ref_or_obj import BoolOrRef, IntOrRef, RefField
 
 
 class V1Service(BaseRun, DestinationImageMixin):
     """Services are used to launch Tensorboards, Notebooks, JupyterHub apps,
     Streamlit/Voila/Bokeh apps, internal tools,
     and dashboards based on your models and data analysis.
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/run/spark/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/run/spark/replica.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/run/spark/replica.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import List, Optional, Union
 
+from clipped.types.ref_or_obj import RefField
 from pydantic import StrictInt, validator
 
 from polyaxon.k8s import k8s_schemas, k8s_validation
 from polyaxon.polyflow.environment import V1Environment
 from polyaxon.polyflow.init import V1Init
 from polyaxon.schemas.base import BaseSchemaModel
-from polyaxon.schemas.fields import RefField
 
 
 class V1SparkReplica(BaseSchemaModel):
     """Spark replica is the specification for a Spark executor or driver.
 
     Args:
         replicas: str, int
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/run/spark/spark.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/run/spark/spark.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,22 +12,22 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Dict, List, Optional, Union
 from typing_extensions import Literal
 
-from clipped.enums_utils import PEnum
+from clipped.types.ref_or_obj import RefField
+from clipped.utils.enums import PEnum
 from pydantic import Field, StrictStr
 
 from polyaxon.k8s import k8s_schemas
 from polyaxon.polyflow.run.base import BaseRun
 from polyaxon.polyflow.run.kinds import V1RunKind
 from polyaxon.polyflow.run.spark.replica import V1SparkReplica
-from polyaxon.schemas.fields import RefField
 
 
 class V1SparkType(str, PEnum):
     JAVA = "java"
     SCALA = "scala"
     PYTHON = "python"
     R = "r"
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/run/tuner.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/run/tuner.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/run/utils.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/run/utils.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/schedules/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/schedules/cron.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/schedules/cron.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,22 +12,22 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Optional
 from typing_extensions import Literal
 
+from clipped.types.ref_or_obj import BoolOrRef, DatetimeOrRef, IntOrRef
 from pydantic import Field, StrictStr
 
 from polyaxon.polyflow.schedules.kinds import V1ScheduleKind
-from polyaxon.schemas.base import BaseDiscriminatedModel
-from polyaxon.schemas.fields.ref_or_obj import BoolOrRef, DatetimeOrRef, IntOrRef
+from polyaxon.schemas.base import BaseSchemaModel
 
 
-class V1CronSchedule(BaseDiscriminatedModel):
+class V1CronSchedule(BaseSchemaModel):
     """Cron schedules is an interface to trigger components repeatedly using a cron definition.
 
     Args:
         kind: str, should be equal to `cron`
         start_at: datetime, optional
         end_at: datetime, optional
         max_runs: int, optional
@@ -121,14 +121,15 @@
     ```yaml
     >>> run:
     >>>   dependsOnPast: true
     ```
     """
 
     _IDENTIFIER = V1ScheduleKind.CRON
+    _USE_DISCRIMINATOR = True
 
     kind: Literal[_IDENTIFIER] = _IDENTIFIER
     cron: StrictStr
     start_at: Optional[DatetimeOrRef] = Field(alias="startAt")
     end_at: Optional[DatetimeOrRef] = Field(alias="endAt")
     max_runs: Optional[IntOrRef] = Field(alias="maxRuns")
     depends_on_past: Optional[BoolOrRef] = Field(alias="dependsOnPast")
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/schedules/datetime.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/schedules/datetime.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing_extensions import Literal
 
+from clipped.types.ref_or_obj import DatetimeOrRef
 from pydantic import Field
 
 from polyaxon.polyflow.schedules.kinds import V1ScheduleKind
-from polyaxon.schemas.base import BaseDiscriminatedModel
-from polyaxon.schemas.fields.ref_or_obj import DatetimeOrRef
+from polyaxon.schemas.base import BaseSchemaModel
 
 
-class V1DateTimeSchedule(BaseDiscriminatedModel):
+class V1DateTimeSchedule(BaseSchemaModel):
     """Date schedule is an interface to kick a component execution at a specific time.
 
     Args:
         kind: str, should be equal to `datetime`
         start_at: datetime, required
 
     ## YAML usage
@@ -70,14 +70,15 @@
     ```yaml
     >>> run:
     >>>   startAt: "2019-06-24T21:20:07+00:00"
     ```
     """
 
     _IDENTIFIER = V1ScheduleKind.DATETIME
+    _USE_DISCRIMINATOR = True
 
     kind: Literal[_IDENTIFIER] = _IDENTIFIER
     start_at: DatetimeOrRef = Field(alias="startAt")
 
     @property
     def max_runs(self):
         return 0
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/schedules/interval.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/schedules/interval.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,27 +12,22 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Optional
 from typing_extensions import Literal
 
+from clipped.types.ref_or_obj import BoolOrRef, DatetimeOrRef, IntOrRef, TimeDeltaOrRef
 from pydantic import Field
 
 from polyaxon.polyflow.schedules.kinds import V1ScheduleKind
-from polyaxon.schemas.base import BaseDiscriminatedModel
-from polyaxon.schemas.fields.ref_or_obj import (
-    BoolOrRef,
-    DatetimeOrRef,
-    IntOrRef,
-    TimeDeltaOrRef,
-)
+from polyaxon.schemas.base import BaseSchemaModel
 
 
-class V1IntervalSchedule(BaseDiscriminatedModel):
+class V1IntervalSchedule(BaseSchemaModel):
     """Interval schedules is an interface to trigger components following a frequency.
 
     Args:
         kind: str, should be equal to `interval`
         start_at: datetime, optional
         end_at: datetime, optional
         max_runs: int, optional
@@ -130,14 +125,15 @@
     ```yaml
     >>> run:
     >>>   dependsOnPast: true
     ```
     """
 
     _IDENTIFIER = V1ScheduleKind.INTERVAL
+    _USE_DISCRIMINATOR = True
 
     kind: Literal[_IDENTIFIER] = _IDENTIFIER
     start_at: Optional[DatetimeOrRef] = Field(alias="startAt")
     end_at: Optional[DatetimeOrRef] = Field(alias="endAt")
     max_runs: Optional[IntOrRef] = Field(alias="maxRuns")
     frequency: TimeDeltaOrRef
     depends_on_past: Optional[BoolOrRef] = Field(alias="dependsOnPast")
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/schedules/kinds.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/schedules/kinds.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from clipped.enums_utils import PEnum
+from clipped.utils.enums import PEnum
 
 
 class V1ScheduleKind(str, PEnum):
     CRON = "cron"
     INTERVAL = "interval"
     DATETIME = "datetime"
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/templates/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/templates/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import List, Optional, Union
 
+from clipped.types.ref_or_obj import BoolOrRef, RefField
 from pydantic import StrictStr
 
 from polyaxon.schemas.base import BaseSchemaModel
-from polyaxon.schemas.fields.ref_or_obj import BoolOrRef, RefField
 
 
 class V1Template(BaseSchemaModel):
     """A template is way for users to define
     specifications (components/operations) and signal to the CLI/API
     that they are not executable without modification.
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/termination/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/termination/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Optional
 
+from clipped.types.ref_or_obj import IntOrRef
 from pydantic import Field
 
 from polyaxon.schemas.base import BaseSchemaModel
-from polyaxon.schemas.fields.ref_or_obj import IntOrRef
 
 
 class V1Termination(BaseSchemaModel):
     """The termination section allows to define and control when
     to stop an operation and how long to keep its resources on the cluster.
 
     Args:
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyflow/trigger_policies.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/trigger_policies.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from clipped.enums_utils import PEnum
+from clipped.utils.enums import PEnum
 
 from polyaxon.lifecycle import V1Statuses
 
 
 class V1TriggerPolicy(str, PEnum):
     ALL_SUCCEEDED = "all_succeeded"
     ALL_FAILED = "all_failed"
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polyplot/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polyplot/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/common/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/common/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/compiler/lineage/params_collector.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/common/accelerators.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/common/accelerators.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/common/annotations.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/common/annotations.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Dict, List, Optional
 
-from clipped.list_utils import to_list
+from clipped.utils.lists import to_list
 
 from polyaxon.polyflow import V1Init
 from polyaxon.schemas.types import V1ConnectionType
 
 
 def get_connection_annotations(
     artifacts_store: Optional[V1ConnectionType],
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/common/constants.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/common/constants.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/common/container_resources.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/common/container_resources.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/common/containers.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/common/containers.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from collections.abc import Mapping
 from typing import Dict, List, Optional
 
-from clipped.list_utils import to_list
-from clipped.sanitizers import sanitize_value
+from clipped.utils.lists import to_list
+from clipped.utils.sanitizers import sanitize_value
 
 from polyaxon.containers.names import generate_container_name
 from polyaxon.k8s import k8s_schemas
 from polyaxon.polypod.common.container_resources import sanitize_resources
 
 
 def patch_container(
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/common/env_vars.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/common/env_vars.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,21 +10,21 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import json
 import os
 
 from typing import Any, Iterable, List, Optional
 
-from clipped.enums_utils import get_enum_value
-from clipped.list_utils import to_list
+from clipped.utils.enums import get_enum_value
+from clipped.utils.json import orjson_dumps
+from clipped.utils.lists import to_list
 
 from polyaxon.connections.reader import (
     get_connection_context_path_env_name,
     get_connection_schema_env_name,
 )
 from polyaxon.env_vars.keys import (
     EV_KEYS_API_VERSION,
@@ -48,24 +48,24 @@
 from polyaxon.schemas.types import V1ConnectionType, V1K8sResourceType
 from polyaxon.services.headers import PolyaxonServiceHeaders
 
 
 def get_str_var(value: Any) -> str:
     if value is not None and not isinstance(value, str):
         try:
-            value = json.dumps(value)
+            value = orjson_dumps(value)
         except (ValueError, TypeError) as e:
             raise PolypodException(e)
     return value or ""
 
 
 def get_env_var(name: str, value: Any) -> k8s_schemas.V1EnvVar:
     if not isinstance(value, str):
         try:
-            value = json.dumps(value)
+            value = orjson_dumps(value)
         except (ValueError, TypeError) as e:
             raise PolypodException(e)
 
     return k8s_schemas.V1EnvVar(name=name, value=value)
 
 
 def get_kv_env_vars(kv_env_vars: List[List]) -> List[k8s_schemas.V1EnvVar]:
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/common/mounts.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/common/mounts.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/common/setter.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/common/setter.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/common/stores.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/common/stores.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/common/volumes.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/common/volumes.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/compiler/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/compiler/config.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/compiler/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import TYPE_CHECKING, Dict, List, Optional
 
-from clipped.list_utils import to_list
+from clipped.utils.lists import to_list
 from pydantic import Field
 
 from polyaxon import settings
 from polyaxon.auxiliaries import (
     V1PolyaxonInitContainer,
     V1PolyaxonSidecarContainer,
     get_default_init_container,
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/compiler/contexts/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/compiler/contexts/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/compiler/contexts/base.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/compiler/contexts/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 from typing import Dict, List
 
-from clipped.list_utils import to_list
+from clipped.utils.lists import to_list
 
 from polyaxon.polyflow import V1CompiledOperation, V1Init
 from polyaxon.schemas.types import V1ConnectionType
 
 
 class BaseContextsManager:
     @classmethod
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/compiler/contexts/contexts.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/compiler/contexts/contexts.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/compiler/contexts/job.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/compiler/contexts/job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/compiler/contexts/kubeflow/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/compiler/contexts/kubeflow/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/compiler/contexts/kubeflow/mpi_job.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/compiler/contexts/kubeflow/mpi_job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/compiler/contexts/kubeflow/mx_job.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/compiler/contexts/kubeflow/mx_job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/compiler/contexts/kubeflow/paddle_job.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/compiler/contexts/kubeflow/paddle_job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/compiler/contexts/kubeflow/pytroch_job.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/compiler/contexts/kubeflow/pytroch_job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/compiler/contexts/kubeflow/tf_job.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/compiler/contexts/kubeflow/tf_job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/compiler/contexts/kubeflow/xgb_job.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/compiler/contexts/kubeflow/xgb_job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/compiler/contexts/service.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/compiler/contexts/service.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/compiler/converter.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/compiler/converter.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/compiler/converters/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/compiler/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/compiler/converters/base.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/compiler/converters/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import copy
 
 from typing import Any, Dict, Iterable, List, Optional
 
-from clipped.http_utils import clean_host
-from clipped.list_utils import to_list
-from clipped.sanitizers import sanitize_string_dict
-from clipped.string_utils import slugify
+from clipped.utils.http import clean_host
+from clipped.utils.lists import to_list
+from clipped.utils.sanitizers import sanitize_string_dict
+from clipped.utils.strings import slugify
 
 from polyaxon import pkg, settings
 from polyaxon.api import VERSION_V1
 from polyaxon.auxiliaries import V1PolyaxonInitContainer, V1PolyaxonSidecarContainer
 from polyaxon.connections.kinds import V1ConnectionKind
 from polyaxon.connections.schemas.connections import patch_git
 from polyaxon.containers.names import INIT_PREFIX, SIDECAR_PREFIX
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/compiler/converters/helpers.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/compiler/converters/helpers.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/compiler/converters/job.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/compiler/converters/job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/compiler/converters/kubeflow/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/compiler/converters/kubeflow/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/compiler/converters/kubeflow/mpi_job.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/compiler/converters/kubeflow/mpi_job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/compiler/converters/kubeflow/mx_job.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/compiler/converters/kubeflow/mx_job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/compiler/converters/kubeflow/paddle_job.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/compiler/converters/kubeflow/paddle_job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/compiler/converters/kubeflow/pytroch_job.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/compiler/converters/kubeflow/pytroch_job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/compiler/converters/kubeflow/tf_job.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/compiler/converters/kubeflow/tf_job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/compiler/converters/kubeflow/xgboost_job.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/compiler/converters/kubeflow/xgboost_job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/compiler/converters/service.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/compiler/converters/service.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/compiler/lineage/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/compiler/lineage/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/compiler/lineage/artifacts_collector.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/compiler/lineage/artifacts_collector.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/compiler/lineage/collector.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/compiler/lineage/collector.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/compiler/lineage/io_collector.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/compiler/lineage/io_collector.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Dict, List, Optional
 
-from clipped.list_utils import to_list
+from clipped.utils.lists import to_list
 
 from polyaxon.polyflow import V1IO, V1CompiledOperation
 from polyaxon.schemas.types import V1ConnectionType
 from polyaxon.types import IMAGE, LINEAGE_VALUES
 from traceml.artifacts import V1ArtifactKind, V1RunArtifact
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/compiler/lineage/params_collector.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/init/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/compiler/resolver/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/compiler/resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/compiler/resolver/base.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/compiler/resolver/base.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/compiler/resolver/resolver.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/compiler/resolver/resolver.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/custom_resources/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/custom_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/custom_resources/job.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/custom_resources/job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/custom_resources/kubeflow/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/custom_resources/kubeflow/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/custom_resources/kubeflow/common.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/custom_resources/kubeflow/common.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/custom_resources/kubeflow/mpi_job.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/custom_resources/kubeflow/mpi_job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/custom_resources/kubeflow/mx_job.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/custom_resources/kubeflow/mx_job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/custom_resources/kubeflow/paddle_job.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/custom_resources/kubeflow/paddle_job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/custom_resources/kubeflow/pytorch_job.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/custom_resources/kubeflow/pytorch_job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/custom_resources/kubeflow/tf_job.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/custom_resources/kubeflow/tf_job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/custom_resources/kubeflow/xgb_job.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/custom_resources/kubeflow/xgb_job.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/custom_resources/service.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/custom_resources/service.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/init/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/main/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/init/artifacts.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/init/artifacts.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import List, Optional
 
-from clipped.list_utils import to_list
+from clipped.utils.lists import to_list
 
 from polyaxon.auxiliaries import V1PolyaxonInitContainer
 from polyaxon.constants.globals import DEFAULT
 from polyaxon.containers.names import (
     INIT_ARTIFACTS_CONTAINER_PREFIX,
     generate_container_name,
 )
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/init/auth.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/init/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import List
 
-from clipped.list_utils import to_list
+from clipped.utils.lists import to_list
 
 from polyaxon.auxiliaries import V1PolyaxonInitContainer
 from polyaxon.containers.names import INIT_AUTH_CONTAINER
 from polyaxon.k8s import k8s_schemas
 from polyaxon.polypod.common.containers import patch_container
 from polyaxon.polypod.common.mounts import get_auth_context_mount
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/init/custom.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/init/custom.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import List, Optional
 
-from clipped.list_utils import to_list
+from clipped.utils.lists import to_list
 
 from polyaxon.containers.names import (
     INIT_CUSTOM_CONTAINER_PREFIX,
     generate_container_name,
 )
 from polyaxon.contexts import paths as ctx_paths
 from polyaxon.exceptions import PolypodException
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/init/dockerfile.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/init/dockerfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import List, Optional
 
-from clipped.list_utils import to_list
+from clipped.utils.lists import to_list
 
 from polyaxon.auxiliaries import V1PolyaxonInitContainer
 from polyaxon.containers.names import (
     INIT_DOCKERFILE_CONTAINER_PREFIX,
     generate_container_name,
 )
 from polyaxon.contexts import paths as ctx_paths
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/init/file.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/init/file.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import List, Optional
 
-from clipped.list_utils import to_list
+from clipped.utils.lists import to_list
 
 from polyaxon.auxiliaries import V1PolyaxonInitContainer
 from polyaxon.containers.names import (
     INIT_FILE_CONTAINER_PREFIX,
     generate_container_name,
 )
 from polyaxon.contexts import paths as ctx_paths
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/init/git.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/init/git.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
 
 from typing import List, Optional
 
-from clipped.json_utils import orjson_dumps
-from clipped.list_utils import to_list
+from clipped.utils.json import orjson_dumps
+from clipped.utils.lists import to_list
 
 from polyaxon.auxiliaries import V1PolyaxonInitContainer
 from polyaxon.connections.kinds import V1ConnectionKind
 from polyaxon.containers.names import INIT_GIT_CONTAINER_PREFIX, generate_container_name
 from polyaxon.contexts import paths as ctx_paths
 from polyaxon.env_vars.keys import EV_KEYS_SSH_PATH
 from polyaxon.exceptions import PolypodException
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/init/store.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/init/store.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 
 from typing import List, Optional, Tuple, Union
 
-from clipped.enums_utils import get_enum_value
-from clipped.list_utils import to_list
+from clipped.utils.enums import get_enum_value
+from clipped.utils.lists import to_list
 
 from polyaxon.auxiliaries import V1PolyaxonInitContainer
 from polyaxon.containers.names import (
     INIT_ARTIFACTS_CONTAINER_PREFIX,
     generate_container_name,
 )
 from polyaxon.contexts import paths as ctx_paths
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/init/tensorboard.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/init/tensorboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import List, Optional
 
-from clipped.enums_utils import get_enum_value
-from clipped.list_utils import to_list
-from clipped.validation import validate_tags
+from clipped.utils.enums import get_enum_value
+from clipped.utils.lists import to_list
+from clipped.utils.validation import validate_tags
 
 from polyaxon.auxiliaries import V1PolyaxonInitContainer
 from polyaxon.containers.names import (
     INIT_TENSORBOARD_CONTAINER_PREFIX,
     generate_container_name,
 )
 from polyaxon.contexts import paths as ctx_paths
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/main/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/pod/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/main/container.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/main/container.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Dict, Iterable, List, Optional
 
-from clipped.list_utils import to_list
+from clipped.utils.lists import to_list
 
 from polyaxon.exceptions import PolypodException
 from polyaxon.k8s import k8s_schemas
 from polyaxon.polyflow import V1Init
 from polyaxon.polypod.common.containers import patch_container
 from polyaxon.polypod.common.env_vars import get_env_from_k8s_resources
 from polyaxon.polypod.main.env_vars import get_env_vars
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/main/env_vars.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/main/env_vars.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Iterable, List
 
-from clipped.list_utils import to_list
+from clipped.utils.lists import to_list
 
 from polyaxon.env_vars.keys import (
     EV_KEYS_ARTIFACTS_STORE_NAME,
     EV_KEYS_COLLECT_ARTIFACTS,
     EV_KEYS_COLLECT_RESOURCES,
 )
 from polyaxon.exceptions import PolyaxonSchemaError, PolypodException
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/main/k8s_resources.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/main/k8s_resources.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/main/volumes.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/main/volumes.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Iterable, List, Optional
 
-from clipped.list_utils import to_list
+from clipped.utils.lists import to_list
 
 from polyaxon.contexts import paths as ctx_paths
 from polyaxon.k8s import k8s_schemas
 from polyaxon.polyflow import V1Init
 from polyaxon.polypod.common import constants
 from polyaxon.polypod.common.mounts import (
     get_artifacts_context_mount,
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/mixins.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/mixins.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/pod/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/sidecar/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/pod/spec.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/pod/spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Dict, List, Optional, Tuple
 
-from clipped.list_utils import to_list
-from clipped.sanitizers import sanitize_string_dict
+from clipped.utils.lists import to_list
+from clipped.utils.sanitizers import sanitize_string_dict
 
 from polyaxon.exceptions import PolypodException
 from polyaxon.k8s import k8s_schemas
 from polyaxon.polyflow import V1Environment
 
 
 def get_pod_spec(
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/pod/volumes.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/pod/volumes.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Dict, Iterable, List, Optional
 
-from clipped.list_utils import to_list
+from clipped.utils.lists import to_list
 
 from polyaxon.k8s import k8s_schemas
 from polyaxon.polyflow import V1Init
 from polyaxon.polypod.common import constants
 from polyaxon.polypod.common.volumes import (
     get_artifacts_context_volume,
     get_configs_context_volume,
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/sidecar/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/sidecar/container.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/sidecar/container.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import List, Optional
 
-from clipped.list_utils import to_list
+from clipped.utils.lists import to_list
 
 from polyaxon.auxiliaries import V1PolyaxonSidecarContainer
 from polyaxon.exceptions import PolypodException
 from polyaxon.k8s import k8s_schemas
 from polyaxon.polypod.common.containers import patch_container
 from polyaxon.polypod.common.env_vars import (
     get_connection_env_var,
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/sidecar/env_vars.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/sidecar/env_vars.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import List
 
-from clipped.list_utils import to_list
+from clipped.utils.lists import to_list
 
 from polyaxon.env_vars.keys import EV_KEYS_ARTIFACTS_STORE_NAME, EV_KEYS_CONTAINER_ID
 from polyaxon.k8s import k8s_schemas
 from polyaxon.polypod.common.env_vars import get_env_var
 
 
 def get_sidecar_env_vars(
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/specs/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/pql/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/specs/contexts.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/specs/contexts.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polypod/specs/replica.py` & `polyaxon-2.0.0rc8/polyaxon/polypod/specs/replica.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polytune/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polytune/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polytune/search_managers/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polytune/search_managers/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polytune/search_managers/bayesian_optimization/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polytune/search_managers/bayesian_optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polytune/search_managers/grid_search/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polytune/search_managers/grid_search/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polytune/search_managers/hyperband/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polytune/search_managers/hyperband/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polytune/search_managers/hyperopt/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polytune/search_managers/hyperopt/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polytune/search_managers/mapping/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polytune/search_managers/mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/polytune/search_managers/random_search/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/polytune/search_managers/random_search/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/pql/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/api/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/pql/builder.py` & `polyaxon-2.0.0rc8/polyaxon/pql/builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from collections import namedtuple
 from typing import Any, Callable, Optional
 
-from clipped.bool_utils import to_bool
-from clipped.date_utils import DateTimeFormatter, DateTimeFormatterException
-from clipped.list_utils import to_list
+from clipped.utils.bools import to_bool
+from clipped.utils.dates import DateTimeFormatter, DateTimeFormatterException
+from clipped.utils.lists import to_list
 
 from polyaxon.exceptions import PQLException
 
 
 class QueryCondSpec(namedtuple("QueryCondSpec", "cond params")):
     def items(self):
         return self._asdict().items()
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/pql/manager.py` & `polyaxon-2.0.0rc8/polyaxon/pql/manager.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/pql/parser.py` & `polyaxon-2.0.0rc8/polyaxon/pql/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,31 +10,31 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import json
-
 from collections import defaultdict, namedtuple
 from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple
 
+from clipped.utils.json import orjson_loads
+from clipped.utils.units import to_cpu_value, to_memory_bytes
+
 from polyaxon.exceptions import PQLException
-from traceml.processors.units_processors import to_cpu_value, to_memory_bytes
 
 
 class QueryOpSpec(namedtuple("QueryOpSpec", "op negation params")):
     def items(self):
         return self._asdict().items()
 
 
 def parse_operation_value(value: Any):
     try:
-        return json.loads(value)
+        return orjson_loads(value)
     except ValueError:
         return value
 
 
 def parse_negation_operation(operation: str) -> Tuple[bool, str]:
     """Parse the negation modifier in an operation."""
     _operation = operation.strip()
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/tracking/contrib/scikit.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,9 +10,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from polyaxon.schemas.patch_strategy import V1PatchStrategy
-from polyaxon.schemas.pending import V1RunPending
+# To keep backwards compatibility
+
+from traceml.integrations.scikit import log_classifier, log_regressor
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/api/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/api/authentication.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/api/authentication.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/api/compatibility.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/api/compatibility.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/api/home.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/api/home.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/api/installation.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/api/installation.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/api/log_handler.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/api/log_handler.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/api/resources.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/api/resources.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,18 +11,19 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Dict, List, Optional
 
+from clipped.types.numbers import StrictIntOrFloat
+from clipped.types.uuids import UUIDStr
 from pydantic import StrictInt, StrictStr
 
 from polyaxon.schemas.base import BaseSchemaModel
-from polyaxon.schemas.fields import StrictIntOrFloat, UUIDStr
 
 
 class ContainerGPUResourcesConfig(BaseSchemaModel):
     _IDENTIFIER = "ContainerGPUResources"
     _MEM_SIZE_ATTRIBUTES = ["memory_free", "memory_used", "memory_total"]
 
     index: StrictInt
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/api/user.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/api/user.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Optional
 
+from clipped.types.email import EmailStr
 from pydantic import StrictStr
 
 from polyaxon.schemas.base import BaseSchemaModel
-from polyaxon.schemas.fields import EmailStr
 
 
 class UserConfig(BaseSchemaModel):
     _IDENTIFIER = "user"
 
     username: StrictStr
     email: Optional[EmailStr]
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/api/version.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/api/version.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/cli/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/cli/agent_config.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/cli/agent_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,23 +13,25 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
 
 from typing import Dict, List, Optional
 
+from clipped.config.schema import skip_partial, to_partial
 from pydantic import Extra, Field, PrivateAttr, StrictStr, validator
 
 from polyaxon.auxiliaries import (
     V1DefaultScheduling,
     V1PolyaxonCleaner,
     V1PolyaxonInitContainer,
     V1PolyaxonNotifier,
     V1PolyaxonSidecarContainer,
 )
+from polyaxon.config.parser import Parser
 from polyaxon.contexts import paths as ctx_paths
 from polyaxon.env_vars.keys import (
     EV_KEYS_AGENT_ARTIFACTS_STORE,
     EV_KEYS_AGENT_CLEANER,
     EV_KEYS_AGENT_COMPRESSED_LOGS,
     EV_KEYS_AGENT_CONNECTIONS,
     EV_KEYS_AGENT_DEFAULT_IMAGE_PULL_SECRETS,
@@ -43,16 +45,15 @@
     EV_KEYS_AGENT_SPAWNER_REFRESH_INTERVAL,
     EV_KEYS_AGENT_USE_PROXY_ENV_VARS_IN_OPS,
     EV_KEYS_K8S_APP_SECRET_NAME,
     EV_KEYS_K8S_NAMESPACE,
 )
 from polyaxon.exceptions import PolyaxonSchemaError
 from polyaxon.lifecycle import V1ProjectFeature
-from polyaxon.parser import parser
-from polyaxon.schemas.base import BaseSchemaModel, skip_partial, to_partial
+from polyaxon.schemas.base import BaseSchemaModel
 from polyaxon.schemas.types import V1ConnectionType, V1K8sResourceType
 
 
 def validate_agent_config(
     artifacts_store, connections, required_artifacts_store: bool = True
 ) -> None:
     if required_artifacts_store and not artifacts_store:
@@ -106,29 +107,29 @@
         self._connections_by_names = {}
 
     @validator("connections", pre=True)
     def validate_json_list(cls, v):
         if not isinstance(v, str):
             return v
         try:
-            return parser.get_dict(
+            return Parser.parse(Dict)(
                 key=EV_KEYS_AGENT_CONNECTIONS,
                 value=v,
                 is_list=True,
                 is_optional=True,
             )
         except PolyaxonSchemaError as e:
             raise ValueError("Received an invalid connections") from e
 
     @validator("artifacts_store", pre=True)
     def validate_json(cls, v):
         if not isinstance(v, str):
             return v
         try:
-            return parser.get_dict(
+            return Parser.parse(Dict)(
                 key=EV_KEYS_AGENT_ARTIFACTS_STORE,
                 value=v,
                 is_optional=True,
             )
         except PolyaxonSchemaError as e:
             raise ValueError(
                 "Received an invalid artifacts store `{}`".format(v)
@@ -288,28 +289,28 @@
         "default_scheduling",
         pre=True,
     )
     def validate_json(cls, v, field):
         if not isinstance(v, str):
             return v
         try:
-            return parser.get_dict(
+            return Parser.parse(Dict)(
                 key=field.name,
                 value=v,
                 is_optional=True,
             )
         except PolyaxonSchemaError as e:
             raise ValueError(
                 "Received an invalid {} `{}`".format(field.alias, v)
             ) from e
 
     @validator("default_image_pull_secrets", pre=True)
     def validate_str_list(cls, v, field):
         try:
-            return parser.get_string(
+            return Parser.parse(str)(
                 key=field.alias,
                 value=v,
                 is_optional=True,
                 is_list=True,
             )
         except PolyaxonSchemaError as e:
             raise ValueError(
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/cli/checks_config.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/cli/checks_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
 
 from datetime import datetime, timedelta
 from typing import Optional
 
-from clipped.tz_utils import now
+from clipped.utils.tz import now
 
 from polyaxon.env_vars.keys import EV_KEYS_INTERVALS_COMPATIBILITY_CHECK
 from polyaxon.schemas.base import BaseSchemaModel
 
 
 class ChecksConfig(BaseSchemaModel):
     _IDENTIFIER = "checks"
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/cli/cli_config.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/cli/cli_config.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/cli/client_config.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/cli/client_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Dict, Optional, Union
 
 import urllib3
 
-from clipped.http_utils import clean_host
+from clipped.utils.http import clean_host
 from pydantic import Extra, Field, StrictStr
 
 from polyaxon.api import LOCALHOST, POLYAXON_CLOUD_HOST
 from polyaxon.contexts import paths as ctx_paths
 from polyaxon.env_vars.keys import (
     EV_KEYS_API_VERSION,
     EV_KEYS_ARCHIVES_ROOT,
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/fields/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_artifact_tree.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,16 +9,18 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from typing import Dict, List, Optional
 
-from polyaxon.schemas.fields.number import (  # noqa
-    IntOrFloat,
-    StrictIntOrFloat,
-)
-from polyaxon.schemas.fields.ref_or_obj import RefField  # noqa
-from polyaxon.schemas.fields.uuids import UUIDStr  # noqa
-from polyaxon.schemas.fields.ref_or_obj import BoolOrRef, IntOrRef, RefField  # noqa
-from polyaxon.schemas.fields.email import EmailStr  # noqa
+from pydantic import StrictStr
+
+from polyaxon.schemas.base import BaseSchemaModel
+
+
+class V1ArtifactTree(BaseSchemaModel):
+    files: Optional[Dict[str, StrictStr]]
+    dirs: Optional[List[StrictStr]]
+    is_done: Optional[bool]
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/fields/docker_image.py` & `polyaxon-2.0.0rc8/polyaxon/sidecar/container/intervals.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,28 +10,19 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from polyaxon.contexts.params import PARAM_REGEX
 
+def get_sync_interval(interval: int, sleep_interval: int) -> int:
+    # Infinite counter (wait until the end)
+    if interval <= 0:
+        return -1
 
-def validate_image(image, allow_none=False):
-    if not image:
-        if allow_none:
-            return
-        else:
-            raise ValueError("Image is required")
-    param = PARAM_REGEX.search(image)
-    if param:
-        return
-    if " " in image:
-        raise ValueError("Invalid docker image `{}`".format(image))
-    tagged_image = image.split(":")
-    if len(tagged_image) > 3:
-        raise ValueError("Invalid docker image `{}`".format(image))
-    if len(tagged_image) == 3 and (
-        "/" not in tagged_image[1] or tagged_image[1].startswith("/")
-    ):
-        raise ValueError("Invalid docker image `{}`".format(image))
+    # Infinite counter
+    if interval < sleep_interval:
+        return 0
+
+    # Use division to get counter
+    return (interval // sleep_interval) + 1
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/fields/number.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,13 +9,10 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from typing import Union
+from clipped.config.patch_strategy import PatchStrategy as V1PatchStrategy
 
-from pydantic import StrictFloat, StrictInt
-
-IntOrFloat = Union[int, float]
-StrictIntOrFloat = Union[StrictInt, StrictFloat, float]
+from polyaxon.schemas.pending import V1RunPending
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/fields/uuids.py` & `polyaxon-2.0.0rc8/polyaxon/utils/host_utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,31 +9,17 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import os
 
-from uuid import UUID
+from clipped.utils.http import clean_host
 
-from pydantic import StrictStr
+from polyaxon.api import LOCALHOST
+from polyaxon.env_vars.keys import EV_KEYS_PLATFORM_HOST
 
 
-class UUIDStr(StrictStr):
-    @classmethod
-    def __get_validators__(cls) -> "CallableGenerator":
-        yield cls.validate
-
-    @classmethod
-    def validate(cls, value, **kwargs):
-        if isinstance(value, str):
-            return UUID(value).hex
-        if isinstance(value, UUID):
-            return value.hex
-        if not value:
-            return value
-
-        field = kwargs.get("field")
-        raise TypeError(
-            f"Field `{field.name}` value be a valid UUID, received `{value}` instead."
-        )
+def get_api_host(default: str = LOCALHOST):
+    return clean_host(os.environ.get(EV_KEYS_PLATFORM_HOST, default))
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/pending.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/pending.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from clipped.enums_utils import PEnum
+from clipped.utils.enums import PEnum
 
 
 class V1RunPending(str, PEnum):
     APPROVAL = "approval"
     UPLOAD = "upload"
     CACHE = "cache"
     BUILD = "build"
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_activity.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_activity.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import datetime
 
 from typing import Optional
 
+from clipped.types.uuids import UUIDStr
 from pydantic import StrictStr
 
 from polyaxon.schemas.base import BaseSchemaModel
-from polyaxon.schemas.fields import UUIDStr
 
 
 class V1Activity(BaseSchemaModel):
     actor: Optional[StrictStr]
     owner: Optional[StrictStr]
     created_at: Optional[datetime.datetime]
     event_action: Optional[StrictStr]
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_agent.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import datetime
 
 from typing import Any, Dict, List, Optional
 
+from clipped.types.uuids import UUIDStr
 from pydantic import StrictStr
 
 from polyaxon.lifecycle import V1Statuses
 from polyaxon.schemas.base import BaseSchemaModel
-from polyaxon.schemas.fields import UUIDStr
 
 
 class V1Agent(BaseSchemaModel):
     uuid: Optional[UUIDStr]
     name: Optional[StrictStr]
     description: Optional[StrictStr]
     tags: Optional[List[StrictStr]]
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_agent_state_response.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_agent_state_response.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_agent_state_response_agent_state.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_agent_state_response_agent_state.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_agent_status_body_request.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_agent_status_body_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Optional
 
+from clipped.types.uuids import UUIDStr
 from pydantic import StrictStr
 
 from polyaxon.lifecycle import V1StatusCondition
 from polyaxon.schemas.base import BaseSchemaModel
-from polyaxon.schemas.fields import UUIDStr
 
 
 class V1AgentStatusBodyRequest(BaseSchemaModel):
     owner: Optional[StrictStr]
     uuid: Optional[UUIDStr]
     condition: Optional[V1StatusCondition]
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_analytics_spec.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_analytics_spec.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_artifact_tree.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_entities_tags.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from typing import Dict, List, Optional
+from typing import List, Optional
 
+from clipped.types.uuids import UUIDStr
 from pydantic import StrictStr
 
 from polyaxon.schemas.base import BaseSchemaModel
 
 
-class V1ArtifactTree(BaseSchemaModel):
-    files: Optional[Dict[str, StrictStr]]
-    dirs: Optional[List[StrictStr]]
-    is_done: Optional[bool]
+class V1EntitiesTags(BaseSchemaModel):
+    uuids: Optional[List[UUIDStr]]
+    tags: Optional[List[StrictStr]]
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_auth.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_auth.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_cloning.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_cloning.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Optional
 
+from clipped.types.uuids import UUIDStr
 from pydantic import StrictStr
 
 from polyaxon.polyflow import V1CloningKind
 from polyaxon.schemas.base import BaseSchemaModel
-from polyaxon.schemas.fields import UUIDStr
 
 
 class V1Cloning(BaseSchemaModel):
     uuid: Optional[UUIDStr]
     name: Optional[StrictStr]
     kind: Optional[V1CloningKind]
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_connection_response.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_connection_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import datetime
 
 from typing import List, Optional
 
+from clipped.types.uuids import UUIDStr
 from pydantic import StrictStr
 
 from polyaxon.connections.kinds import V1ConnectionKind
 from polyaxon.schemas.base import BaseSchemaModel
-from polyaxon.schemas.fields import UUIDStr
 
 
 class V1ConnectionResponse(BaseSchemaModel):
     uuid: Optional[UUIDStr]
     name: Optional[StrictStr]
     agent: Optional[StrictStr]
     description: Optional[StrictStr]
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_dashboard.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_dashboard.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import datetime
 
 from typing import List, Optional
 
+from clipped.types.uuids import UUIDStr
 from pydantic import StrictStr
 
 from polyaxon.schemas.base import BaseSchemaModel
-from polyaxon.schemas.fields import UUIDStr
 from polyaxon.schemas.responses.v1_dashboard_spec import V1DashboardSpec
 
 
 class V1Dashboard(BaseSchemaModel):
     uuid: Optional[UUIDStr]
     name: Optional[StrictStr]
     description: Optional[StrictStr]
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_dashboard_spec.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_dashboard_spec.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_entities_tags.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_entities_transfer.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import List, Optional
 
+from clipped.types.uuids import UUIDStr
 from pydantic import StrictStr
 
 from polyaxon.schemas.base import BaseSchemaModel
-from polyaxon.schemas.fields import UUIDStr
 
 
-class V1EntitiesTags(BaseSchemaModel):
+class V1EntitiesTransfer(BaseSchemaModel):
     uuids: Optional[List[UUIDStr]]
-    tags: Optional[List[StrictStr]]
+    project: Optional[StrictStr]
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_entities_transfer.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_list_service_accounts_response.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,13 +14,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import List, Optional
 
 from pydantic import StrictStr
 
 from polyaxon.schemas.base import BaseSchemaModel
-from polyaxon.schemas.fields import UUIDStr
+from polyaxon.schemas.responses.v1_service_account import V1ServiceAccount
 
 
-class V1EntitiesTransfer(BaseSchemaModel):
-    uuids: Optional[List[UUIDStr]]
-    project: Optional[StrictStr]
+class V1ListServiceAccountsResponse(BaseSchemaModel):
+    count: Optional[int]
+    results: Optional[List[V1ServiceAccount]]
+    previous: Optional[StrictStr]
+    next: Optional[StrictStr]
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_entity_notification_body.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_entity_notification_body.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import List, Optional
 
+from clipped.types.uuids import UUIDStr
 from pydantic import StrictStr
 
 from polyaxon.lifecycle import V1StatusCondition
 from polyaxon.schemas.base import BaseSchemaModel
-from polyaxon.schemas.fields import UUIDStr
 
 
 class V1EntityNotificationBody(BaseSchemaModel):
     namespace: Optional[StrictStr]
     owner: Optional[StrictStr]
     project: Optional[StrictStr]
     uuid: Optional[UUIDStr]
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_entity_stage_body_request.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_entity_stage_body_request.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_entity_status_body_request.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_entity_status_body_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Optional
 
+from clipped.types.uuids import UUIDStr
 from pydantic import StrictStr
 
 from polyaxon.lifecycle import V1StatusCondition
 from polyaxon.schemas.base import BaseSchemaModel
-from polyaxon.schemas.fields import UUIDStr
 
 
 class V1EntityStatusBodyRequest(BaseSchemaModel):
     owner: Optional[StrictStr]
     project: Optional[StrictStr]
     uuid: Optional[UUIDStr]
     condition: Optional[V1StatusCondition]
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_events_response.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_list_run_edges_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,14 +9,20 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from typing import Any, Dict, List, Optional
+from typing import List, Optional
+
+from pydantic import StrictStr
 
 from polyaxon.schemas.base import BaseSchemaModel
+from polyaxon.schemas.responses.v1_run_edge import V1RunEdge
 
 
-class V1EventsResponse(BaseSchemaModel):
-    data: Optional[List[Dict[str, Any]]]
+class V1ListRunEdgesResponse(BaseSchemaModel):
+    count: Optional[int]
+    results: Optional[List[V1RunEdge]]
+    previous: Optional[StrictStr]
+    next: Optional[StrictStr]
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_list_activities_response.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_list_activities_response.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_list_agents_response.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_list_agents_response.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_list_bookmarks_response.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_list_bookmarks_response.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_list_connections_response.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_list_connections_response.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_list_dashboards_response.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_list_dashboards_response.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_list_organization_members_response.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_list_organization_members_response.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_list_organizations_response.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_list_organizations_response.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_list_presets_response.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_list_presets_response.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_list_project_versions_response.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_list_project_versions_response.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_list_projects_response.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_list_projects_response.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_list_queues_response.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_list_queues_response.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_list_run_artifacts_response.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_list_run_artifacts_response.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_list_run_connections_response.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_list_run_connections_response.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_list_run_edges_response.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_list_token_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import List, Optional
 
 from pydantic import StrictStr
 
 from polyaxon.schemas.base import BaseSchemaModel
-from polyaxon.schemas.responses.v1_run_edge import V1RunEdge
+from polyaxon.schemas.responses.v1_token import V1Token
 
 
-class V1ListRunEdgesResponse(BaseSchemaModel):
+class V1ListTokenResponse(BaseSchemaModel):
     count: Optional[int]
-    results: Optional[List[V1RunEdge]]
+    results: Optional[List[V1Token]]
     previous: Optional[StrictStr]
     next: Optional[StrictStr]
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_list_runs_response.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_list_runs_response.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_list_searches_response.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_list_searches_response.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_list_service_accounts_response.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_list_tags_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import List, Optional
 
 from pydantic import StrictStr
 
 from polyaxon.schemas.base import BaseSchemaModel
-from polyaxon.schemas.responses.v1_service_account import V1ServiceAccount
+from polyaxon.schemas.responses.v1_tag import V1Tag
 
 
-class V1ListServiceAccountsResponse(BaseSchemaModel):
+class V1ListTagsResponse(BaseSchemaModel):
     count: Optional[int]
-    results: Optional[List[V1ServiceAccount]]
+    results: Optional[List[V1Tag]]
     previous: Optional[StrictStr]
     next: Optional[StrictStr]
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_list_tags_response.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_list_teams_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import List, Optional
 
 from pydantic import StrictStr
 
 from polyaxon.schemas.base import BaseSchemaModel
-from polyaxon.schemas.responses.v1_tag import V1Tag
+from polyaxon.schemas.responses.v1_team import V1Team
 
 
-class V1ListTagsResponse(BaseSchemaModel):
+class V1ListTeamsResponse(BaseSchemaModel):
     count: Optional[int]
-    results: Optional[List[V1Tag]]
+    results: Optional[List[V1Team]]
     previous: Optional[StrictStr]
     next: Optional[StrictStr]
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_list_team_members_response.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_list_team_members_response.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_list_teams_response.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_pipeline.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from typing import List, Optional
+from typing import Optional
 
+from clipped.types.uuids import UUIDStr
 from pydantic import StrictStr
 
+from polyaxon.polyflow.run.kinds import V1PipelineKind
 from polyaxon.schemas.base import BaseSchemaModel
-from polyaxon.schemas.responses.v1_team import V1Team
 
 
-class V1ListTeamsResponse(BaseSchemaModel):
-    count: Optional[int]
-    results: Optional[List[V1Team]]
-    previous: Optional[StrictStr]
-    next: Optional[StrictStr]
+class V1Pipeline(BaseSchemaModel):
+    uuid: Optional[UUIDStr]
+    name: Optional[StrictStr]
+    kind: Optional[V1PipelineKind]
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_list_token_response.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_trial_start.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,20 +9,22 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from typing import List, Optional
+from typing import Any, Dict, Optional
 
+from clipped.types.email import EmailStr
 from pydantic import StrictStr
 
 from polyaxon.schemas.base import BaseSchemaModel
-from polyaxon.schemas.responses.v1_token import V1Token
 
 
-class V1ListTokenResponse(BaseSchemaModel):
-    count: Optional[int]
-    results: Optional[List[V1Token]]
-    previous: Optional[StrictStr]
-    next: Optional[StrictStr]
+class V1TrialStart(BaseSchemaModel):
+    name: Optional[StrictStr]
+    email: Optional[EmailStr]
+    organization: Optional[StrictStr]
+    plan: Optional[StrictStr]
+    seats: Optional[int]
+    details: Optional[Dict[str, Any]]
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_operation_body.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_operation_body.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_organization.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_organization.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import datetime
 
 from typing import Any, Dict, Optional
 
+from clipped.types.email import EmailStr
 from pydantic import StrictStr
 
 from polyaxon.schemas.base import BaseSchemaModel
-from polyaxon.schemas.fields import EmailStr
 
 
 class V1Organization(BaseSchemaModel):
     user: Optional[StrictStr]
     user_email: Optional[EmailStr]
     name: Optional[StrictStr]
     is_public: Optional[bool]
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_organization_member.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_organization_member.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import datetime
 
 from typing import Optional
 
+from clipped.types.email import EmailStr
 from pydantic import StrictStr
 
 from polyaxon.schemas.base import BaseSchemaModel
-from polyaxon.schemas.fields import EmailStr
 
 
 class V1OrganizationMember(BaseSchemaModel):
     user: Optional[StrictStr]
     user_email: Optional[EmailStr]
     role: Optional[StrictStr]
     kind: Optional[StrictStr]
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_password_change.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_password_change.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_pipeline.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_run_connection.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,18 +11,17 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Optional
 
+from clipped.types.uuids import UUIDStr
 from pydantic import StrictStr
 
-from polyaxon.polyflow.run.kinds import V1PipelineKind
 from polyaxon.schemas.base import BaseSchemaModel
-from polyaxon.schemas.fields import UUIDStr
 
 
-class V1Pipeline(BaseSchemaModel):
+class V1RunConnection(BaseSchemaModel):
     uuid: Optional[UUIDStr]
     name: Optional[StrictStr]
-    kind: Optional[V1PipelineKind]
+    kind: Optional[StrictStr]
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_preset.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_team_member.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,25 +11,22 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import datetime
 
-from typing import List, Optional
+from typing import Optional
 
+from clipped.types.email import EmailStr
 from pydantic import StrictStr
 
 from polyaxon.schemas.base import BaseSchemaModel
-from polyaxon.schemas.fields import UUIDStr
 
 
-class V1Preset(BaseSchemaModel):
-    uuid: Optional[UUIDStr]
-    name: Optional[StrictStr]
-    description: Optional[StrictStr]
-    tags: Optional[List[StrictStr]]
+class V1TeamMember(BaseSchemaModel):
+    user: Optional[StrictStr]
+    user_email: Optional[EmailStr]
+    role: Optional[StrictStr]
+    org_role: Optional[StrictStr]
     created_at: Optional[datetime.datetime]
     updated_at: Optional[datetime.datetime]
-    frozen: Optional[bool]
-    live_state: Optional[int]
-    content: Optional[StrictStr]
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_project.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_project.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import datetime
 
 from typing import List, Optional
 
+from clipped.types.uuids import UUIDStr
 from pydantic import StrictStr
 
 from polyaxon.schemas.base import BaseSchemaModel
-from polyaxon.schemas.fields import UUIDStr
 from polyaxon.schemas.responses.v1_project_settings import V1ProjectSettings
 
 
 class V1Project(BaseSchemaModel):
     uuid: Optional[UUIDStr]
     owner: Optional[StrictStr]
     name: Optional[StrictStr]
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_project_settings.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_project_settings.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_project_user_access.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_project_user_access.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_project_version.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_project_version.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import datetime
 
 from typing import Any, Dict, List, Optional
 
+from clipped.types.uuids import UUIDStr
 from pydantic import StrictStr
 
 from polyaxon.lifecycle import V1ProjectVersionKind, V1StageCondition, V1Stages
 from polyaxon.schemas.base import BaseSchemaModel
-from polyaxon.schemas.fields import UUIDStr
 
 
 class V1ProjectVersion(BaseSchemaModel):
     uuid: Optional[UUIDStr]
     name: Optional[StrictStr]
     description: Optional[StrictStr]
     tags: Optional[List[StrictStr]]
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_queue.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_team.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,28 +11,25 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import datetime
 
-from typing import Any, Dict, List, Optional
+from typing import List, Optional
 
+from clipped.types.uuids import UUIDStr
 from pydantic import StrictStr
 
 from polyaxon.schemas.base import BaseSchemaModel
-from polyaxon.schemas.fields import UUIDStr
+from polyaxon.schemas.responses.v1_team_settings import V1TeamSettings
 
 
-class V1Queue(BaseSchemaModel):
+class V1Team(BaseSchemaModel):
     uuid: Optional[UUIDStr]
-    agent: Optional[StrictStr]
     name: Optional[StrictStr]
-    description: Optional[StrictStr]
-    tags: Optional[List[StrictStr]]
-    priority: Optional[int]
-    concurrency: Optional[int]
-    resource: Optional[StrictStr]
-    quota: Optional[StrictStr]
-    stats: Optional[Dict[str, Any]]
+    projects: Optional[List[StrictStr]]
+    component_hubs: Optional[List[StrictStr]]
+    model_registries: Optional[List[StrictStr]]
+    settings: Optional[V1TeamSettings]
     created_at: Optional[datetime.datetime]
     updated_at: Optional[datetime.datetime]
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_run.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import datetime
 
 from typing import Any, Dict, List, Optional
 
+from clipped.types.uuids import UUIDStr
 from pydantic import StrictStr
 
 from polyaxon.lifecycle import V1StatusCondition, V1Statuses
 from polyaxon.polyflow.run.kinds import V1RunKind
 from polyaxon.polyflow.run.resources import V1RunResources
 from polyaxon.schemas import V1RunPending
 from polyaxon.schemas.base import BaseSchemaModel
-from polyaxon.schemas.fields import UUIDStr
 from polyaxon.schemas.responses.v1_cloning import V1Cloning
 from polyaxon.schemas.responses.v1_pipeline import V1Pipeline
 from polyaxon.schemas.responses.v1_run_settings import V1RunSettings
 
 
 class V1Run(BaseSchemaModel):
     uuid: Optional[UUIDStr]
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_run_connection.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_settings_catalog.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,17 +11,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Optional
 
+from clipped.types.uuids import UUIDStr
 from pydantic import StrictStr
 
 from polyaxon.schemas.base import BaseSchemaModel
-from polyaxon.schemas.fields import UUIDStr
 
 
-class V1RunConnection(BaseSchemaModel):
+class V1SettingsCatalog(BaseSchemaModel):
     uuid: Optional[UUIDStr]
     name: Optional[StrictStr]
-    kind: Optional[StrictStr]
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_run_edge.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_run_edge.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_run_reference_catalog.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_run_reference_catalog.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_run_settings.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_run_settings.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_search.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_search.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import datetime
 
 from typing import List, Optional
 
+from clipped.types.uuids import UUIDStr
 from pydantic import StrictStr
 
 from polyaxon.schemas.base import BaseSchemaModel
-from polyaxon.schemas.fields import UUIDStr
 from polyaxon.schemas.responses.v1_search_spec import V1SearchSpec
 from traceml.events.schemas import SearchView
 
 
 class V1Search(BaseSchemaModel):
     uuid: Optional[UUIDStr]
     name: Optional[StrictStr]
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_search_spec.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_search_spec.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_section_spec.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_section_spec.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_service_account.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_service_account.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import datetime
 
 from typing import List, Optional
 
+from clipped.types.uuids import UUIDStr
 from pydantic import StrictStr
 
 from polyaxon.schemas.base import BaseSchemaModel
-from polyaxon.schemas.fields import UUIDStr
 
 
 class V1ServiceAccount(BaseSchemaModel):
     uuid: Optional[UUIDStr]
     name: Optional[StrictStr]
     description: Optional[StrictStr]
     tags: Optional[List[StrictStr]]
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_settings_catalog.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_uuids.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,18 +9,16 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from typing import Optional
+from typing import List, Optional
 
-from pydantic import StrictStr
+from clipped.types.uuids import UUIDStr
 
 from polyaxon.schemas.base import BaseSchemaModel
-from polyaxon.schemas.fields import UUIDStr
 
 
-class V1SettingsCatalog(BaseSchemaModel):
-    uuid: Optional[UUIDStr]
-    name: Optional[StrictStr]
+class V1Uuids(BaseSchemaModel):
+    uuids: Optional[List[UUIDStr]]
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_tag.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_tag.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Any, Dict, Optional
 
+from clipped.types.uuids import UUIDStr
 from pydantic import StrictStr
 
 from polyaxon.schemas.base import BaseSchemaModel
-from polyaxon.schemas.fields import UUIDStr
 
 
 class V1Tag(BaseSchemaModel):
     uuid: Optional[UUIDStr]
     name: Optional[StrictStr]
     color: Optional[StrictStr]
     description: Optional[StrictStr]
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_team.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_token.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,23 +13,24 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import datetime
 
 from typing import List, Optional
 
+from clipped.types.uuids import UUIDStr
 from pydantic import StrictStr
 
 from polyaxon.schemas.base import BaseSchemaModel
-from polyaxon.schemas.fields import UUIDStr
-from polyaxon.schemas.responses.v1_team_settings import V1TeamSettings
 
 
-class V1Team(BaseSchemaModel):
+class V1Token(BaseSchemaModel):
     uuid: Optional[UUIDStr]
+    key: Optional[StrictStr]
     name: Optional[StrictStr]
-    projects: Optional[List[StrictStr]]
-    component_hubs: Optional[List[StrictStr]]
-    model_registries: Optional[List[StrictStr]]
-    settings: Optional[V1TeamSettings]
+    scopes: Optional[List[StrictStr]]
+    services: Optional[List[StrictStr]]
+    started_at: Optional[datetime.datetime]
+    expires_at: Optional[datetime.datetime]
     created_at: Optional[datetime.datetime]
     updated_at: Optional[datetime.datetime]
+    expiration: Optional[int]
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_team_member.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_user.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,24 +9,22 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import datetime
-
 from typing import Optional
 
+from clipped.types.email import EmailStr
 from pydantic import StrictStr
 
 from polyaxon.schemas.base import BaseSchemaModel
-from polyaxon.schemas.fields import EmailStr
 
 
-class V1TeamMember(BaseSchemaModel):
-    user: Optional[StrictStr]
-    user_email: Optional[EmailStr]
-    role: Optional[StrictStr]
-    org_role: Optional[StrictStr]
-    created_at: Optional[datetime.datetime]
-    updated_at: Optional[datetime.datetime]
+class V1User(BaseSchemaModel):
+    username: Optional[StrictStr]
+    email: Optional[EmailStr]
+    name: Optional[StrictStr]
+    kind: Optional[StrictStr]
+    theme: Optional[int]
+    organization: Optional[StrictStr]
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_team_settings.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_team_settings.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_user_email.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_user_email.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,13 +11,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Optional
 
+from clipped.types.email import EmailStr
+
 from polyaxon.schemas.base import BaseSchemaModel
-from polyaxon.schemas.fields import EmailStr
 
 
 class V1UserEmail(BaseSchemaModel):
     email: Optional[EmailStr]
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_user_singup.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/responses/v1_user_singup.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Optional
 
+from clipped.types.email import EmailStr
 from pydantic import StrictStr
 
 from polyaxon.schemas.base import BaseSchemaModel
-from polyaxon.schemas.fields import EmailStr
 
 
 class V1UserSingup(BaseSchemaModel):
     username: Optional[StrictStr]
     email: Optional[EmailStr]
     organization: Optional[StrictStr]
     password: Optional[StrictStr]
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/responses/v1_uuids.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/types/event.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,15 +9,19 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from typing import List, Optional
+from typing import Optional
 
-from polyaxon.schemas.base import BaseSchemaModel
-from polyaxon.schemas.fields import UUIDStr
+from pydantic import StrictStr
 
+from polyaxon.schemas.types.base import BaseTypeConfig
 
-class V1Uuids(BaseSchemaModel):
-    uuids: Optional[List[UUIDStr]]
+
+class V1EventType(BaseTypeConfig):
+    _IDENTIFIER = "event"
+
+    name: Optional[StrictStr]
+    kind: Optional[StrictStr]
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/services.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/services.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/types/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/types/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,20 +10,25 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from clipped.types.gcs import GcsPath
+from clipped.types.s3 import S3Path
+from clipped.types.uri import Uri
+from clipped.types.wasb import WasbPath
+
 from polyaxon.schemas.types.artifacts import V1ArtifactsType
-from polyaxon.schemas.types.auth import V1AuthType
 from polyaxon.schemas.types.connections import V1ConnectionType
 from polyaxon.schemas.types.dockerfile import V1DockerfileType
 from polyaxon.schemas.types.event import V1EventType
 from polyaxon.schemas.types.file import V1FileType
-from polyaxon.schemas.types.gcs import V1GcsType
 from polyaxon.schemas.types.git import V1GitType
 from polyaxon.schemas.types.k8s_resources import V1K8sResourceType
-from polyaxon.schemas.types.s3 import V1S3Type
 from polyaxon.schemas.types.tensorboard import V1TensorboardType
-from polyaxon.schemas.types.uri import V1UriType
-from polyaxon.schemas.types.wasb import V1WasbType
+
+V1GcsType = GcsPath
+V1S3Type = S3Path
+V1UriType = Uri
+V1WasbType = WasbPath
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/types/artifacts.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/types/artifacts.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import List, Optional, Union
 
+from clipped.types.ref_or_obj import RefField
 from pydantic import StrictInt
 
-from polyaxon.schemas.fields.ref_or_obj import RefField
 from polyaxon.schemas.types.base import BaseTypeConfig
 
 
 class V1ArtifactsType(BaseTypeConfig):
     """Artifacts type allows to easily pass
     the files and directories to initialize as a single parameter.
 
@@ -99,15 +99,14 @@
 
     ### Usage in IO and params definition
 
     The inputs definition
 
     ```python
     >>> from polyaxon import types
-    >>> from polyaxon.schemas import types
     >>> from polyaxon.polyflow import V1IO
     >>> inputs = [
     >>>     V1IO(
     >>>         name="some-file-names",
     >>>         type=types.ARTIFACTS,
     >>>     ),
     >>>     V1IO(
@@ -121,15 +120,14 @@
     >>> ]
     ```
 
     The params usage
 
     ```python
     >>> from polyaxon import types
-    >>> from polyaxon.schemas import types
     >>> from polyaxon.polyflow import V1Param
     >>> params = {
     >>>     "test1": V1Param(value=types.V1ArtifactsType(files=["file1", "/path/to/file2"])),
     >>>     "test2": V1Param(
     >>>         value=types.V1ArtifactsType(dirs=["/tensorboard-logs"]),
     >>>         connection="foo",
     >>>         to_init=True
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/types/base.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/types/base.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/types/connections.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/types/connections.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Dict, List, Optional, Union
 
+from clipped.types.ref_or_obj import RefField
 from pydantic import Field, StrictStr
 
 from polyaxon.connections.kinds import V1ConnectionKind
 from polyaxon.connections.schemas import V1K8sResourceSchema
 from polyaxon.connections.schemas.connections import V1Connection
 from polyaxon.schemas.base import BaseSchemaModel
-from polyaxon.schemas.fields.ref_or_obj import RefField
 from polyaxon.schemas.types.k8s_resources import V1K8sResourceType
 
 
 class V1ConnectionType(BaseSchemaModel):
     """Connections are how Polyaxon connects several
     types of external systems and resources to your operations.
 
@@ -317,17 +317,20 @@
     @property
     def store_path(self) -> str:
         if self.is_mount:
             return self.schema_.mount_path.rstrip("/")
         if self.is_bucket:
             bucket = self.schema_.bucket.rstrip("/")
             if self.is_wasb:
-                from polyaxon.parser.parser import parse_wasbs_path
+                from polyaxon import types
+                from polyaxon.config.parser import Parser
 
-                return parse_wasbs_path(bucket).get_container_path()
+                return Parser.parse(types.WASB)(
+                    key="schema", value=bucket
+                ).get_container_path()
             return bucket
 
     @property
     def is_mount(self) -> bool:
         return V1ConnectionKind.is_mount(self.kind)
 
     @property
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/types/dockerfile.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/types/dockerfile.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Any, Dict, List, Optional, Tuple, Union
 
+from clipped.config.schema import skip_partial
+from clipped.types.docker_image import validate_image
+from clipped.types.ref_or_obj import RefField
 from pydantic import Field, StrictStr, validator
 
-from polyaxon.schemas.base import skip_partial
-from polyaxon.schemas.fields.docker_image import validate_image
-from polyaxon.schemas.fields.ref_or_obj import RefField
 from polyaxon.schemas.types.base import BaseTypeConfig
 
 POLYAXON_DOCKERFILE_NAME = "Dockerfile"
 POLYAXON_DOCKER_WORKDIR = "/code"
 POLYAXON_DOCKER_SHELL = "/bin/bash"
 
 
@@ -93,29 +93,27 @@
 
     ### Usage in IO and params definition
 
     The inputs definition
 
     ```python
     >>> from polyaxon import types
-    >>> from polyaxon.schemas import types
     >>> from polyaxon.polyflow import V1IO
     >>> inputs = [
     >>>     V1IO(
     >>>         name="test1",
     >>>         type=types.DOCKERFILE,
     >>>     ),
     >>> ]
     ```
 
     The params usage
 
     ```python
     >>> from polyaxon import types
-    >>> from polyaxon.schemas import types
     >>> from polyaxon.polyflow import V1Param
     >>> params = {
     >>>     "test1": V1Param(
     >>>         value=types.V1DockerfileType(
     >>>             image="test:version",
     >>>             run=["pip install package1"],
     >>>             env={'KEY1': 'en_US.UTF-8', 'KEY2':2}
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/types/event.py` & `polyaxon-2.0.0rc8/polyaxon/services/auth.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from typing import Optional
 
-from pydantic import StrictStr
 
-from polyaxon.schemas.types.base import BaseTypeConfig
+class AuthenticationError(Exception):
+    pass
 
 
-class V1EventType(BaseTypeConfig):
-    _IDENTIFIER = "event"
+class AuthenticationTypes:
+    TOKEN = "Token"
+    INTERNAL_TOKEN = "InternalToken"
+    EPHEMERAL_TOKEN = "EphemeralToken"
 
-    name: Optional[StrictStr]
-    kind: Optional[StrictStr]
+    VALUES = {TOKEN, INTERNAL_TOKEN, EPHEMERAL_TOKEN}
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/types/file.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/types/file.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Optional, Union
 
+from clipped.types.ref_or_obj import RefField
 from pydantic import StrictStr
 
-from polyaxon.schemas.fields.ref_or_obj import RefField
 from polyaxon.schemas.types.base import BaseTypeConfig
 from traceml.artifacts import V1ArtifactKind
 
 
 class V1FileType(BaseTypeConfig):
     """File type.
 
@@ -97,29 +97,27 @@
 
     ### Usage in IO and params definition
 
     The inputs definition
 
     ```python
     >>> from polyaxon import types
-    >>> from polyaxon.schemas import types
     >>> from polyaxon.polyflow import V1IO
     >>> inputs = [
     >>>     V1IO(
     >>>         name="test1",
     >>>         type=types.FILE,
     >>>     ),
     >>> ]
     ```
 
     The params usage
 
     ```python
     >>> from polyaxon import types
-    >>> from polyaxon.schemas import types
     >>> from polyaxon.polyflow import V1Param
     >>>
     >>> params = {
     >>>     "test1": V1Param(
     >>>         value=types.V1FileType(
     >>>             filename="script.sh",
     >>>             chmod="+x",
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/types/git.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/types/git.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import List, Optional, Union
 
+from clipped.types.ref_or_obj import RefField
 from pydantic import StrictStr
 
-from polyaxon.schemas.fields.ref_or_obj import RefField
 from polyaxon.schemas.types.base import BaseTypeConfig
 
 
 class V1GitType(BaseTypeConfig):
     """Git type allows you to pass a git repo as a parameter.
 
     If used as an input type, Polyaxon can resolve several git connections
@@ -82,15 +82,14 @@
 
     ### Usage in IO and params definition
 
     The inputs definition
 
     ```python
     >>> from polyaxon import types
-    >>> from polyaxon.schemas import types
     >>> from polyaxon.polyflow import V1IO
     >>> inputs = [
     >>>     V1IO(
     >>>         name="test1",
     >>>         type=types.GIT,
     >>>     ),
     >>>     V1IO(
@@ -100,15 +99,14 @@
     >>> ]
     ```
 
     The params usage
 
     ```python
     >>> from polyaxon import types
-    >>> from polyaxon.schemas import types
     >>> from polyaxon.polyflow import V1Param
     >>> params = {
     >>>     "test1": V1Param(
     >>>         value=types.V1GitType(url="https://github.com/tensorflow/models")
     >>>     ),
     >>>     "test2": V1Param(
     >>>         value=types.V1GitType(revision="branchA"),
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/types/k8s_resources.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/types/k8s_resources.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/schemas/types/tensorboard.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/types/tensorboard.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,17 +11,19 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import List, Optional, Union
 
+from clipped.types.ref_or_obj import RefField
+from clipped.types.uuids import UUIDStr
+from clipped.utils.lists import to_list
 from pydantic import Field, StrictInt, StrictStr, validator
 
-from polyaxon.schemas.fields import RefField, UUIDStr
 from polyaxon.schemas.types.base import BaseTypeConfig
 
 
 class V1TensorboardType(BaseTypeConfig):
     """Tensorboard type.
 
     This type allows to initialize Tensorboard logs foe one or multiple operations.
@@ -77,29 +79,27 @@
 
     ### Usage in IO and params definition
 
     The inputs definition
 
     ```python
     >>> from polyaxon import types
-    >>> from polyaxon.schemas import types
     >>> from polyaxon.polyflow import V1IO
     >>> inputs = [
     >>>     V1IO(
     >>>         name="tensorboard_content",
     >>>         type=types.TENSORBOARD,
     >>>     ),
     >>> ]
     ```
 
     The params usage
 
     ```python
     >>> from polyaxon import types
-    >>> from polyaxon.schemas import types
     >>> from polyaxon.polyflow import V1Param
     >>>
     >>> params = {
     >>>     "test1": V1Param(
     >>>         value=types.V1TensorboardType(
     >>>             port=6006,
     >>>             uuids="d1410a914d18457589b91926d8c23db4,56f1a7f20f1d4f7f9e1a108b3c6b6031",
@@ -147,12 +147,10 @@
     uuids: Optional[Union[List[UUIDStr], RefField]]
     use_names: Optional[Union[bool, RefField]] = Field(alias="useNames")
     path_prefix: Optional[StrictStr] = Field(alias="pathPrefix")
     plugins: Optional[Union[List[StrictStr], RefField]]
 
     @validator("uuids", "plugins", pre=True)
     def validate_str_list(cls, v, field):
-        from polyaxon.parser import parser
-
         if isinstance(v, str):
-            return parser.get_string(field, v, is_list=True)
+            return to_list(v, check_str=True)
         return v
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/sdk/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/sdk/async_client/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/sdk/api/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/sdk/api/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/sdk/api/agents_v1_api.py` & `polyaxon-2.0.0rc8/polyaxon/sdk/api/agents_v1_api.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/sdk/api/artifacts_stores_v1_api.py` & `polyaxon-2.0.0rc8/polyaxon/sdk/api/artifacts_stores_v1_api.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/sdk/api/auth_v1_api.py` & `polyaxon-2.0.0rc8/polyaxon/sdk/api/auth_v1_api.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/sdk/api/connections_v1_api.py` & `polyaxon-2.0.0rc8/polyaxon/sdk/api/connections_v1_api.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/sdk/api/dashboards_v1_api.py` & `polyaxon-2.0.0rc8/polyaxon/sdk/api/dashboards_v1_api.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/sdk/api/organizations_v1_api.py` & `polyaxon-2.0.0rc8/polyaxon/sdk/api/organizations_v1_api.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/sdk/api/presets_v1_api.py` & `polyaxon-2.0.0rc8/polyaxon/sdk/api/presets_v1_api.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/sdk/api/project_dashboards_v1_api.py` & `polyaxon-2.0.0rc8/polyaxon/sdk/api/project_dashboards_v1_api.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/sdk/api/project_searches_v1_api.py` & `polyaxon-2.0.0rc8/polyaxon/sdk/api/project_searches_v1_api.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/sdk/api/projects_v1_api.py` & `polyaxon-2.0.0rc8/polyaxon/sdk/api/projects_v1_api.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/sdk/api/queues_v1_api.py` & `polyaxon-2.0.0rc8/polyaxon/sdk/api/queues_v1_api.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/sdk/api/runs_v1_api.py` & `polyaxon-2.0.0rc8/polyaxon/sdk/api/runs_v1_api.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/sdk/api/searches_v1_api.py` & `polyaxon-2.0.0rc8/polyaxon/sdk/api/searches_v1_api.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/sdk/api/service_accounts_v1_api.py` & `polyaxon-2.0.0rc8/polyaxon/sdk/api/service_accounts_v1_api.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/sdk/api/tags_v1_api.py` & `polyaxon-2.0.0rc8/polyaxon/sdk/api/tags_v1_api.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/sdk/api/teams_v1_api.py` & `polyaxon-2.0.0rc8/polyaxon/sdk/api/teams_v1_api.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/sdk/api/users_v1_api.py` & `polyaxon-2.0.0rc8/polyaxon/sdk/api/users_v1_api.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/sdk/api/versions_v1_api.py` & `polyaxon-2.0.0rc8/polyaxon/sdk/api/versions_v1_api.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/sdk/async_client/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/sdk/sync_client/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/sdk/async_client/api_client.py` & `polyaxon-2.0.0rc8/polyaxon/sdk/async_client/api_client.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/sdk/async_client/rest.py` & `polyaxon-2.0.0rc8/polyaxon/sdk/async_client/rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,23 +11,24 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import io
-import json
 import logging
 import re
 import ssl
 
 from urllib.parse import urlencode
 
 import aiohttp
 
+from clipped.utils.json import orjson_dumps
+
 from polyaxon.sdk.exceptions import ApiException, ApiValueError
 
 logger = logging.getLogger(__name__)
 
 
 class RESTResponse(io.IOBase):
     def __init__(self, resp, data):
@@ -128,15 +129,15 @@
         if query_params:
             args["url"] += "?" + urlencode(query_params)
 
         # For `POST`, `PUT`, `PATCH`, `OPTIONS`, `DELETE`
         if method in ["POST", "PUT", "PATCH", "OPTIONS", "DELETE"]:
             if re.search("json", headers["Content-Type"], re.IGNORECASE):
                 if body is not None:
-                    body = json.dumps(body)
+                    body = orjson_dumps(body)
                 args["data"] = body
             elif (
                 headers["Content-Type"] == "application/x-www-form-urlencoded"
             ):  # noqa: E501
                 args["data"] = aiohttp.FormData(post_params)
             elif headers["Content-Type"] == "multipart/form-data":
                 # must del headers['Content-Type'], or the correct
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/sdk/base_api.py` & `polyaxon-2.0.0rc8/polyaxon/sdk/base_api.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/sdk/configuration.py` & `polyaxon-2.0.0rc8/polyaxon/sdk/configuration.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/sdk/exceptions.py` & `polyaxon-2.0.0rc8/polyaxon/sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/sdk/models.py` & `polyaxon-2.0.0rc8/polyaxon/sdk/models.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/sdk/sync_client/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/services/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/sdk/sync_client/api_client.py` & `polyaxon-2.0.0rc8/polyaxon/sdk/sync_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,23 +12,23 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import atexit
 import datetime
-import json
 import mimetypes
 import os
 import re
 import tempfile
 
 from multiprocessing.pool import ThreadPool
 from urllib.parse import quote
 
+from clipped.utils.json import orjson_dumps, orjson_loads
 from dateutil.parser import parse
 
 import polyaxon.sdk.models
 
 from polyaxon import pkg
 from polyaxon.sdk.configuration import Configuration
 from polyaxon.sdk.exceptions import ApiException, ApiValueError
@@ -332,15 +332,15 @@
         # handle file downloading
         # save response body into a tmp file and return the instance
         if response_type == "file":
             return self.__deserialize_file(response)
 
         # fetch data from response object
         try:
-            data = json.loads(response.data)
+            data = orjson_loads(response.data)
         except ValueError:
             data = response.data
 
         return self.__deserialize(data, response_type)
 
     def __deserialize(self, data, klass):
         """Deserializes dict, list, str into an object.
@@ -609,15 +609,15 @@
             params.items() if isinstance(params, dict) else params
         ):  # noqa: E501
             if isinstance(v, (int, float)):
                 v = str(v)
             if isinstance(v, bool):
                 v = str(v).lower()
             if isinstance(v, dict):
-                v = json.dumps(v)
+                v = orjson_dumps(v)
 
             if k in collection_formats:
                 collection_format = collection_formats[k]
                 if collection_format == "multi":
                     new_params.extend((k, value) for value in v)
                 else:
                     if collection_format == "ssv":
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/sdk/sync_client/rest.py` & `polyaxon-2.0.0rc8/polyaxon/sdk/sync_client/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,21 +12,22 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 import io
-import json
 import logging
 import re
 import ssl
 
 import urllib3
 
+from clipped.utils.json import orjson_dumps
+
 from polyaxon.sdk.exceptions import (
     ApiException,
     ApiValueError,
     ForbiddenException,
     NotFoundException,
     ServiceException,
     UnauthorizedException,
@@ -164,15 +165,15 @@
             if method in ["POST", "PUT", "PATCH", "OPTIONS", "DELETE"]:
                 # no content type provided or payload is json
                 if not headers.get("Content-Type") or re.search(
                     "json", headers["Content-Type"], re.IGNORECASE
                 ):
                     request_body = None
                     if body is not None:
-                        request_body = json.dumps(body)
+                        request_body = orjson_dumps(body)
                     r = self.pool_manager.request(
                         method,
                         url,
                         body=request_body,
                         preload_content=_preload_content,
                         timeout=timeout,
                         headers=headers,
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/services/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/sidecar/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/services/auth.py` & `polyaxon-2.0.0rc8/polyaxon/config/parser.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,19 +9,29 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from clipped.config.parser import Parser as _Parser
+from clipped.decorators.memoization import memoize
 
+from polyaxon.exceptions import PolyaxonSchemaError
 
-class AuthenticationError(Exception):
-    pass
 
+class Parser(_Parser):
+    _SCHEMA_EXCEPTION = PolyaxonSchemaError
 
-class AuthenticationTypes:
-    TOKEN = "Token"
-    INTERNAL_TOKEN = "InternalToken"
-    EPHEMERAL_TOKEN = "EphemeralToken"
+    @staticmethod
+    @memoize
+    def type_mapping():
+        from polyaxon import types
 
-    VALUES = {TOKEN, INTERNAL_TOKEN, EPHEMERAL_TOKEN}
+        return types.MAPPING
+
+    @staticmethod
+    @memoize
+    def type_forwarding():
+        from polyaxon import types
+
+        return types.FORWARDING
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/services/ephemeral.py` & `polyaxon-2.0.0rc8/polyaxon/services/ephemeral.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/services/headers.py` & `polyaxon-2.0.0rc8/polyaxon/services/headers.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Tuple
 
-from clipped.enums_utils import PEnum, get_enum_value
+from clipped.utils.enums import PEnum, get_enum_value
 
 
 class PolyaxonServiceHeaders(str, PEnum):
     CLI_VERSION = "X_POLYAXON_CLI_VERSION"
     CLIENT_VERSION = "X_POLYAXON_CLIENT_VERSION"
     INTERNAL = "X_POLYAXON_INTERNAL"
     SERVICE = "X_POLYAXON_SERVICE"
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/services/values.py` & `polyaxon-2.0.0rc8/polyaxon/services/values.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
 
 from typing import Optional
 
-from clipped.enums_utils import PEnum
+from clipped.utils.enums import PEnum
 
 from polyaxon.env_vars.keys import EV_KEYS_SERVICE
 
 SERVICE = None
 
 
 class PolyaxonServices(str, PEnum):
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/settings.py` & `polyaxon-2.0.0rc8/polyaxon/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 
 from typing import TYPE_CHECKING, Optional
 
-from clipped.bool_utils import to_bool
 from clipped.formatting import Printer
+from clipped.utils.bools import to_bool
 from pydantic import ValidationError
 
 from polyaxon.api import LOCALHOST
 from polyaxon.env_vars.keys import EV_KEYS_NO_CONFIG, EV_KEYS_SET_AGENT
 from polyaxon.managers.client import ClientConfigManager
 from polyaxon.managers.home import HomeConfigManager
 from polyaxon.managers.user import UserConfigManager
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/sidecar/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/stores/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/sidecar/container/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/sidecar/container/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import asyncio
 import os
 
-from clipped.tz_utils import now
+from clipped.utils.tz import now
 from kubernetes_asyncio.client.rest import ApiException
 
 from polyaxon.client import RunClient
 from polyaxon.contexts import paths as ctx_paths
 from polyaxon.env_vars.getters import get_run_info
 from polyaxon.env_vars.keys import EV_KEYS_K8S_POD_ID
 from polyaxon.exceptions import PolyaxonClientException, PolyaxonContainerException
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/sidecar/container/intervals.py` & `polyaxon-2.0.0rc8/polyaxon/tracking/contrib/xgboost.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,19 +10,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+# To keep backwards compatibility
 
-def get_sync_interval(interval: int, sleep_interval: int) -> int:
-    # Infinite counter (wait until the end)
-    if interval <= 0:
-        return -1
+from traceml.integrations.xgboost import Callback, callback
 
-    # Infinite counter
-    if interval < sleep_interval:
-        return 0
-
-    # Use division to get counter
-    return (interval // sleep_interval) + 1
+# alias
+polyaxon_callback = callback
+PolyaxonCallback = Callback
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/sidecar/container/monitors/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/tracking/contrib/hugging_face.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,9 +10,13 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from polyaxon.sidecar.container.monitors.artifacts import sync_artifacts
-from polyaxon.sidecar.container.monitors.logs import sync_logs
+# To keep backwards compatibility
+
+from traceml.integrations.hugging_face import Callback
+
+# alias
+PolyaxonCallback = Callback
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/sidecar/container/monitors/artifacts.py` & `polyaxon-2.0.0rc8/polyaxon/sidecar/container/monitors/artifacts.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/sidecar/container/monitors/logs.py` & `polyaxon-2.0.0rc8/polyaxon/sidecar/container/monitors/logs.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,34 +9,34 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import datetime
 
 from typing import Optional
 
 import aiofiles
 
-from clipped.path_utils import check_or_create_path, delete_path
+from clipped.utils.paths import check_or_create_path, delete_path
 from kubernetes_asyncio.client.models import V1Pod
 
 from polyaxon.contexts import paths as ctx_paths
 from polyaxon.k8s.async_manager import AsyncK8SManager
 from polyaxon.k8s.logging.async_monitor import query_k8s_pod_logs
-from polyaxon.types import AwareDT
 from traceml.logging import V1Logs
 
 
 async def sync_logs(
     run_uuid: str,
     k8s_manager: AsyncK8SManager,
     pod: V1Pod,
-    last_time: Optional[AwareDT],
+    last_time: Optional[datetime.datetime],
     stream: bool = False,
     is_running: bool = True,
 ):
     path_from = ctx_paths.CONTEXT_MOUNT_ARTIFACTS_FORMAT.format(run_uuid)
     path_from = "{}/.tmpplxlogs".format(path_from)
 
     if not is_running:
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/sidecar/ignore.py` & `polyaxon-2.0.0rc8/polyaxon/sidecar/ignore.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/sidecar/processor.py` & `polyaxon-2.0.0rc8/polyaxon/sidecar/processor.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/stores/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/tracking/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/stores/polyaxon_store.py` & `polyaxon-2.0.0rc8/polyaxon/stores/polyaxon_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,40 +9,40 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import json
 import os
 import requests
 
 from typing import Dict, List
 
 from clipped.formatting import Printer
-from clipped.list_utils import to_list
-from clipped.path_utils import (
+from clipped.utils.json import orjson_dumps
+from clipped.utils.lists import to_list
+from clipped.utils.paths import (
     check_or_create_path,
     create_tarfile_from_path,
     get_files_by_paths,
     untar_file,
 )
+from clipped.utils.units import format_sizeof
 from requests_toolbelt import MultipartEncoder, MultipartEncoderMonitor
 
 from polyaxon import settings
 from polyaxon.constants.globals import DEFAULT_UPLOADS_PATH
 from polyaxon.env_vars.keys import EV_KEYS_UPLOAD_SIZE
 from polyaxon.exceptions import (
     HTTP_ERROR_MESSAGES_MAPPING,
     PolyaxonClientException,
     PolyaxonShouldExitError,
 )
 from polyaxon.logger import logger
-from traceml.processors.units_processors import format_sizeof
 
 
 class PolyaxonStore:
     """
     Polyaxon filesystem store.
 
     Used to download data from Polyaxon streams apis.
@@ -122,15 +122,15 @@
                 "separately using `polyaxon data` command and remove them from here.\n".format(
                     format_sizeof(upload_size_max)
                 )
             )
 
         files = to_list(files)
         if json_data:
-            files.append(("json", json.dumps(json_data)))
+            files.append(("json", orjson_dumps(json_data)))
 
         multipart_encoder = MultipartEncoder(fields=files)
         request_headers = self._client.client.config.get_full_headers(headers=headers)
         request_headers.update({"Content-Type": multipart_encoder.content_type})
 
         timeout = timeout if timeout is not None else settings.LONG_REQUEST_TIMEOUT
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/tracking/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/tracking/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/tracking/contrib/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/tracking/contrib/fastai.py` & `polyaxon-2.0.0rc8/polyaxon/tracking/contrib/fastai.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/tracking/contrib/fastai_v1.py` & `polyaxon-2.0.0rc8/polyaxon/tracking/contrib/fastai_v1.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/tracking/contrib/hugging_face.py` & `polyaxon-2.0.0rc8/polyaxon/tracking/contrib/pytorch_lightning.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,11 +12,11 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # To keep backwards compatibility
 
-from traceml.integrations.hugging_face import Callback
+from traceml.integrations.pytorch_lightning import Callback
 
 # alias
 PolyaxonCallback = Callback
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/tracking/contrib/ignite.py` & `polyaxon-2.0.0rc8/polyaxon/tracking/contrib/ignite.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/tracking/contrib/keras.py` & `polyaxon-2.0.0rc8/polyaxon/tracking/contrib/keras.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/tracking/contrib/lightgbm.py` & `polyaxon-2.0.0rc8/polyaxon/tracking/contrib/lightgbm.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/tracking/contrib/pytorch_lightning.py` & `polyaxon-2.0.0rc8/polyaxon/tracking/contrib/tensorboard.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,11 +12,11 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # To keep backwards compatibility
 
-from traceml.integrations.pytorch_lightning import Callback
+from traceml.integrations.tensorboard import Logger
 
 # alias
-PolyaxonCallback = Callback
+PolyaxonTensorboardLogger = Logger
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/tracking/contrib/scikit.py` & `polyaxon-2.0.0rc8/polyaxon/polyflow/run/kubeflow/clean_pod_policy.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,10 +10,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-# To keep backwards compatibility
+from clipped.utils.enums import PEnum
 
-from traceml.integrations.scikit import log_classifier, log_regressor
+
+class V1CleanPodPolicy(str, PEnum):
+    ALL = "All"
+    RUNNING = "Running"
+    var_NONE = "None"
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/tracking/contrib/tensorboard.py` & `polyaxon-2.0.0rc8/polyaxon/tracking/contrib/tensorflow.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,11 +12,12 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # To keep backwards compatibility
 
-from traceml.integrations.tensorboard import Logger
+from traceml.integrations.tensorflow import Callback
 
 # alias
-PolyaxonTensorboardLogger = Logger
+PolyaxonCallback = Callback
+PolyaxonSessionRunHook = Callback
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/tracking/contrib/tensorflow.py` & `polyaxon-2.0.0rc8/polyaxon/config/manager.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from clipped.config.manager import ConfigManager as _ConfigManager
 
-# To keep backwards compatibility
+from polyaxon.config.spec import ConfigSpec
 
-from traceml.integrations.tensorflow import Callback
 
-# alias
-PolyaxonCallback = Callback
-PolyaxonSessionRunHook = Callback
+class ConfigManager(_ConfigManager):
+    _CONFIG_SPEC = ConfigSpec
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/tracking/run.py` & `polyaxon-2.0.0rc8/polyaxon/vendor/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,11 +9,7 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-# To keep backwards compatibility
-
-from traceml.tracking.run import Run
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/utils/cache.py` & `polyaxon-2.0.0rc8/polyaxon/utils/cache.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/utils/cli_constants.py` & `polyaxon-2.0.0rc8/polyaxon/utils/cli_constants.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/utils/fixtures/__init__.py` & `polyaxon-2.0.0rc8/polyaxon/utils/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/utils/fixtures/backfill.py` & `polyaxon-2.0.0rc8/polyaxon/utils/fixtures/backfill.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/utils/fixtures/bo.py` & `polyaxon-2.0.0rc8/polyaxon/utils/fixtures/bo.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/utils/fixtures/build.py` & `polyaxon-2.0.0rc8/polyaxon/utils/fixtures/build.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/utils/fixtures/grid.py` & `polyaxon-2.0.0rc8/polyaxon/utils/fixtures/grid.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/utils/fixtures/jobs.py` & `polyaxon-2.0.0rc8/polyaxon/utils/fixtures/jobs.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/utils/fixtures/mapping.py` & `polyaxon-2.0.0rc8/polyaxon/utils/fixtures/mapping.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/utils/fixtures/pipelines.py` & `polyaxon-2.0.0rc8/polyaxon/utils/fixtures/pipelines.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/utils/fixtures/schedule.py` & `polyaxon-2.0.0rc8/polyaxon/utils/fixtures/schedule.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from datetime import timedelta
 
-from clipped.tz_utils import now
+from clipped.utils.tz import now
 
 from polyaxon.polyflow import (
     V1HpRange,
     V1HpUniform,
     V1MatrixKind,
     V1Optimization,
     V1RunKind,
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/utils/fixtures/services.py` & `polyaxon-2.0.0rc8/polyaxon/utils/fixtures/services.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/utils/formatting.py` & `polyaxon-2.0.0rc8/polyaxon/utils/formatting.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import sys
 
 from typing import Dict, List, Union
 
 import click
 
 from clipped.formatting import Printer
-from clipped.list_utils import to_list
-from clipped.units_processors import to_percentage, to_unit_memory
+from clipped.utils.lists import to_list
+from clipped.utils.units import to_percentage, to_unit_memory
 
 from polyaxon.schemas.api.resources import ContainerResourcesConfig
 
 
 def resources(jobs_resources: Union[List[Dict], Dict]):
     jobs_resources = to_list(jobs_resources)
     click.clear()
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/utils/fqn_utils.py` & `polyaxon-2.0.0rc8/polyaxon/utils/fqn_utils.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/utils/host_utils.py` & `polyaxon-2.0.0rc8/polyaxon/schemas/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,17 +9,23 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import os
 
-from clipped.http_utils import clean_host
+from clipped.config.schema import BaseSchemaModel as _BaseSchemaModel
 
-from polyaxon.api import LOCALHOST
-from polyaxon.env_vars.keys import EV_KEYS_PLATFORM_HOST
+from polyaxon import pkg
+from polyaxon.config.spec import ConfigSpec
+from polyaxon.exceptions import PolyaxonSchemaError
 
 
-def get_api_host(default: str = LOCALHOST):
-    return clean_host(os.environ.get(EV_KEYS_PLATFORM_HOST, default))
+class BaseSchemaModel(_BaseSchemaModel):
+    _VERSION = pkg.SCHEMA_VERSION
+    _SCHEMA_EXCEPTION = PolyaxonSchemaError
+    _CONFIG_SPEC = ConfigSpec
+
+
+NAME_REGEX = r"^[-a-zA-Z0-9_]+\Z"
+FULLY_QUALIFIED_NAME_REGEX = r"^[-a-zA-Z0-9_]+(:[-a-zA-Z0-9_.]+)?\Z"
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/utils/test_utils.py` & `polyaxon-2.0.0rc8/polyaxon/utils/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 import os
 import tempfile
 
 from collections.abc import Mapping
 from typing import List, Optional
 from unittest import TestCase, mock
 
-from clipped.json_utils import orjson_dumps
-from clipped.path_utils import delete_path
+from clipped.utils.json import orjson_dumps
+from clipped.utils.paths import delete_path
 
 from polyaxon import dist, settings
 from polyaxon.connections.kinds import V1ConnectionKind
 from polyaxon.connections.schemas import V1HostPathConnection
 from polyaxon.contexts import paths as ctx_paths
 from polyaxon.schemas.api.authentication import AccessTokenConfig
 from polyaxon.schemas.cli.agent_config import AgentConfig
```

### Comparing `polyaxon-2.0.0rc7/polyaxon/utils/urls_utils.py` & `polyaxon-2.0.0rc8/polyaxon/utils/urls_utils.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/polyaxon/vendor/shell_pty.py` & `polyaxon-2.0.0rc8/polyaxon/vendor/shell_pty.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,23 +19,23 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
 import errno
 import fcntl
-import json
 import os
 import pty
 import select
 import signal
 import struct
 import termios
 import tty
 
+from clipped.utils.json import orjson_dumps
 from polyaxon.client.transport import ws_client
 
 
 class PseudoTerminal:
     """Wraps the pseudo-TTY (PTY) allocated to a container.
 
     The PTY is managed via the current process' TTY until it is closed.
@@ -101,15 +101,15 @@
         our own controlling terminal.
         """
         packed = fcntl.ioctl(
             pty.STDOUT_FILENO, termios.TIOCGWINSZ, struct.pack("HHHH", 0, 0, 0, 0)
         )
         rows, cols, h_pixels, v_pixels = struct.unpack("HHHH", packed)
         self.client_shell.write_channel(
-            ws_client.RESIZE_CHANNEL, json.dumps({"Height": rows, "Width": cols})
+            ws_client.RESIZE_CHANNEL, orjson_dumps({"Height": rows, "Width": cols})
         )
 
     def _loop(self):
         """
         Main select loop. Passes all data to self.master_read() or self.stdin_read().
         """
         assert self.client_shell is not None
```

### Comparing `polyaxon-2.0.0rc7/polyaxon.egg-info/PKG-INFO` & `polyaxon-2.0.0rc8/polyaxon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyaxon
-Version: 2.0.0rc7
+Version: 2.0.0rc8
 Summary: Command Line Interface (CLI) and client to interact with Polyaxon API.
 Home-page: https://github.com/polyaxon/polyaxon
 Author: Polyaxon, Inc.
 Author-email: contact@polyaxon.com
 Maintainer: Polyaxon, Inc.
 Maintainer-email: contact@polyaxon.com
 License: Apache 2.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: polyaxon Version: 2.0.0rc7 Summary: Command Line
+Metadata-Version: 2.1 Name: polyaxon Version: 2.0.0rc8 Summary: Command Line
 Interface (CLI) and client to interact with Polyaxon API. Home-page: https://
 github.com/polyaxon/polyaxon Author: Polyaxon, Inc. Author-email:
 contact@polyaxon.com Maintainer: Polyaxon, Inc. Maintainer-email:
 contact@polyaxon.com License: Apache 2.0 Keywords:
 polyaxon,aws,s3,microsoft,azure,google cloud storage,gcs,deep-learning,machine-
 learning,data-science,neural-networks,artificial-intelligence,ai,reinforcement-
 learning,kubernetes,aws,microsoft,azure,google cloud,tensorFlow,pytorch
```

### Comparing `polyaxon-2.0.0rc7/polyaxon.egg-info/SOURCES.txt` & `polyaxon-2.0.0rc8/polyaxon.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -95,17 +95,18 @@
 polyaxon/client/transport/socket_transport.py
 polyaxon/client/transport/threaded_transport.py
 polyaxon/client/transport/ws_client.py
 polyaxon/client/workers/__init__.py
 polyaxon/client/workers/base_worker.py
 polyaxon/client/workers/periodic_worker.py
 polyaxon/client/workers/queue_worker.py
-polyaxon/config_reader/__init__.py
-polyaxon/config_reader/manager.py
-polyaxon/config_reader/spec.py
+polyaxon/config/__init__.py
+polyaxon/config/manager.py
+polyaxon/config/parser.py
+polyaxon/config/spec.py
 polyaxon/connections/__init__.py
 polyaxon/connections/base.py
 polyaxon/connections/kinds.py
 polyaxon/connections/reader.py
 polyaxon/connections/aws/__init__.py
 polyaxon/connections/aws/base.py
 polyaxon/connections/aws/service.py
@@ -227,17 +228,14 @@
 polyaxon/notifiers/slack_webhook.py
 polyaxon/notifiers/spec.py
 polyaxon/notifiers/webhook.py
 polyaxon/operations/__init__.py
 polyaxon/operations/cleaner.py
 polyaxon/operations/notifier.py
 polyaxon/operations/tuner.py
-polyaxon/parser/__init__.py
-polyaxon/parser/constants.py
-polyaxon/parser/parser.py
 polyaxon/plugins/__init__.py
 polyaxon/plugins/sentry.py
 polyaxon/polyaxonfile/__init__.py
 polyaxon/polyaxonfile/check.py
 polyaxon/polyaxonfile/params.py
 polyaxon/polyaxonfile/manager/__init__.py
 polyaxon/polyaxonfile/manager/operations.py
@@ -436,15 +434,14 @@
 polyaxon/polytune/search_managers/random_search/__init__.py
 polyaxon/pql/__init__.py
 polyaxon/pql/builder.py
 polyaxon/pql/manager.py
 polyaxon/pql/parser.py
 polyaxon/schemas/__init__.py
 polyaxon/schemas/base.py
-polyaxon/schemas/patch_strategy.py
 polyaxon/schemas/pending.py
 polyaxon/schemas/services.py
 polyaxon/schemas/api/__init__.py
 polyaxon/schemas/api/authentication.py
 polyaxon/schemas/api/compatibility.py
 polyaxon/schemas/api/home.py
 polyaxon/schemas/api/installation.py
@@ -453,20 +450,14 @@
 polyaxon/schemas/api/user.py
 polyaxon/schemas/api/version.py
 polyaxon/schemas/cli/__init__.py
 polyaxon/schemas/cli/agent_config.py
 polyaxon/schemas/cli/checks_config.py
 polyaxon/schemas/cli/cli_config.py
 polyaxon/schemas/cli/client_config.py
-polyaxon/schemas/fields/__init__.py
-polyaxon/schemas/fields/docker_image.py
-polyaxon/schemas/fields/email.py
-polyaxon/schemas/fields/number.py
-polyaxon/schemas/fields/ref_or_obj.py
-polyaxon/schemas/fields/uuids.py
 polyaxon/schemas/responses/__init__.py
 polyaxon/schemas/responses/v1_activity.py
 polyaxon/schemas/responses/v1_agent.py
 polyaxon/schemas/responses/v1_agent_state_response.py
 polyaxon/schemas/responses/v1_agent_state_response_agent_state.py
 polyaxon/schemas/responses/v1_agent_status_body_request.py
 polyaxon/schemas/responses/v1_analytics_spec.py
@@ -532,27 +523,23 @@
 polyaxon/schemas/responses/v1_trial_start.py
 polyaxon/schemas/responses/v1_user.py
 polyaxon/schemas/responses/v1_user_email.py
 polyaxon/schemas/responses/v1_user_singup.py
 polyaxon/schemas/responses/v1_uuids.py
 polyaxon/schemas/types/__init__.py
 polyaxon/schemas/types/artifacts.py
-polyaxon/schemas/types/auth.py
 polyaxon/schemas/types/base.py
+polyaxon/schemas/types/clipped.py
 polyaxon/schemas/types/connections.py
 polyaxon/schemas/types/dockerfile.py
 polyaxon/schemas/types/event.py
 polyaxon/schemas/types/file.py
-polyaxon/schemas/types/gcs.py
 polyaxon/schemas/types/git.py
 polyaxon/schemas/types/k8s_resources.py
-polyaxon/schemas/types/s3.py
 polyaxon/schemas/types/tensorboard.py
-polyaxon/schemas/types/uri.py
-polyaxon/schemas/types/wasb.py
 polyaxon/sdk/__init__.py
 polyaxon/sdk/base_api.py
 polyaxon/sdk/configuration.py
 polyaxon/sdk/exceptions.py
 polyaxon/sdk/models.py
 polyaxon/sdk/api/__init__.py
 polyaxon/sdk/api/agents_v1_api.py
```

### Comparing `polyaxon-2.0.0rc7/polyaxon.egg-info/requires.txt` & `polyaxon-2.0.0rc8/polyaxon.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 click<9.0.0,>=7.1.1
-clipped<0.1
+clipped<0.2
 Jinja2<3.1.0,>=2.10.3
 kubernetes>=10.0.1
 python-dateutil>=2.7.3
 pytz>=2019.2
 PyYAML>=5.1
 orjson>=3.7
 psutil>=5.4.7
 requests>=2.20.1
 requests-toolbelt>=0.8.0
 rich>=12.0.0
 sentry-sdk>=1.2.0
 urllib3>=1.25.6
 certifi>=2022.12.7
 pydantic>=1.10.2
-traceml==1.1.0rc7
-hypertune==1.1.0rc7
+traceml==1.1.0rc8
+hypertune==1.1.0rc8
 
 [azure]
 adlfs
 
 [dev]
 moto==2.0.5
```

### Comparing `polyaxon-2.0.0rc7/polyaxon_sdk/__init__.py` & `polyaxon-2.0.0rc8/polyaxon_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/setup.cfg` & `polyaxon-2.0.0rc8/setup.cfg`

 * *Files identical despite different names*

### Comparing `polyaxon-2.0.0rc7/setup.py` & `polyaxon-2.0.0rc8/setup.py`

 * *Files identical despite different names*

