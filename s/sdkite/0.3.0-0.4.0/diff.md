# Comparing `tmp/sdkite-0.3.0.tar.gz` & `tmp/sdkite-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdkite-0.3.0.tar", last modified: Sun Feb 26 19:00:18 2023, max compression
+gzip compressed data, was "sdkite-0.4.0.tar", last modified: Sun Apr 16 19:04:13 2023, max compression
```

## Comparing `sdkite-0.3.0.tar` & `sdkite-0.4.0.tar`

### file list

```diff
@@ -1,103 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 19:00:18.463701 sdkite-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-02-26 19:00:13.000000 sdkite-0.3.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 19:00:18.451701 sdkite-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 19:00:18.455701 sdkite-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-02-26 19:00:13.000000 sdkite-0.3.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-02-26 19:00:13.000000 sdkite-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-02-26 19:00:13.000000 sdkite-0.3.0/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-02-26 19:00:13.000000 sdkite-0.3.0/.prettierrc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-02-26 19:00:13.000000 sdkite-0.3.0/.pylintrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 19:00:18.455701 sdkite-0.3.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-02-26 19:00:13.000000 sdkite-0.3.0/.vscode/env
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-02-26 19:00:13.000000 sdkite-0.3.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-02-26 19:00:13.000000 sdkite-0.3.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-02-26 19:00:13.000000 sdkite-0.3.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-02-26 19:00:13.000000 sdkite-0.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-02-26 19:00:18.463701 sdkite-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-02-26 19:00:13.000000 sdkite-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-02-26 19:00:13.000000 sdkite-0.3.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 19:00:18.455701 sdkite-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-02-26 19:00:13.000000 sdkite-0.3.0/docs/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-02-26 19:00:13.000000 sdkite-0.3.0/docs/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 19:00:18.455701 sdkite-0.3.0/docs/src/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-26 19:00:13.000000 sdkite-0.3.0/docs/src/CNAME
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 19:00:18.455701 sdkite-0.3.0/docs/src/css/
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-02-26 19:00:13.000000 sdkite-0.3.0/docs/src/css/extra.css
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-02-26 19:00:13.000000 sdkite-0.3.0/docs/src/http_auth.md
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-02-26 19:00:13.000000 sdkite-0.3.0/docs/src/http_engine.md
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-02-26 19:00:13.000000 sdkite-0.3.0/docs/src/http_replay.md
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-02-26 19:00:13.000000 sdkite-0.3.0/docs/src/http_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-02-26 19:00:13.000000 sdkite-0.3.0/docs/src/http_response.md
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-02-26 19:00:13.000000 sdkite-0.3.0/docs/src/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-02-26 19:00:13.000000 sdkite-0.3.0/docs/src/pagination.md
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-02-26 19:00:13.000000 sdkite-0.3.0/docs/src/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-02-26 19:00:13.000000 sdkite-0.3.0/docs/src/typing.md
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-02-26 19:00:13.000000 sdkite-0.3.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-02-26 19:00:13.000000 sdkite-0.3.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-02-26 19:00:18.463701 sdkite-0.3.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      196 2023-02-26 19:00:13.000000 sdkite-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 19:00:18.451701 sdkite-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 19:00:18.455701 sdkite-0.3.0/src/sdkite/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-02-26 19:00:13.000000 sdkite-0.3.0/src/sdkite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-26 19:00:18.000000 sdkite-0.3.0/src/sdkite/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-02-26 19:00:13.000000 sdkite-0.3.0/src/sdkite/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-02-26 19:00:13.000000 sdkite-0.3.0/src/sdkite/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 19:00:18.459701 sdkite-0.3.0/src/sdkite/http/
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-02-26 19:00:13.000000 sdkite-0.3.0/src/sdkite/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-02-26 19:00:13.000000 sdkite-0.3.0/src/sdkite/http/_stringescape.py
--rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-02-26 19:00:13.000000 sdkite-0.3.0/src/sdkite/http/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-02-26 19:00:13.000000 sdkite-0.3.0/src/sdkite/http/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     8569 2023-02-26 19:00:13.000000 sdkite-0.3.0/src/sdkite/http/engine_replay.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-02-26 19:00:13.000000 sdkite-0.3.0/src/sdkite/http/engine_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-02-26 19:00:13.000000 sdkite-0.3.0/src/sdkite/http/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-02-26 19:00:13.000000 sdkite-0.3.0/src/sdkite/http/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5848 2023-02-26 19:00:13.000000 sdkite-0.3.0/src/sdkite/pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-26 19:00:13.000000 sdkite-0.3.0/src/sdkite/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-02-26 19:00:13.000000 sdkite-0.3.0/src/sdkite/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 19:00:18.459701 sdkite-0.3.0/src/sdkite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-02-26 19:00:18.000000 sdkite-0.3.0/src/sdkite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-02-26 19:00:18.000000 sdkite-0.3.0/src/sdkite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-26 19:00:18.000000 sdkite-0.3.0/src/sdkite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-02-26 19:00:18.000000 sdkite-0.3.0/src/sdkite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-26 19:00:18.000000 sdkite-0.3.0/src/sdkite.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 19:00:18.459701 sdkite-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-02-26 19:00:13.000000 sdkite-0.3.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 19:00:18.459701 sdkite-0.3.0/tests/integration/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 19:00:18.459701 sdkite-0.3.0/tests/integration/recorded/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-02-26 19:00:13.000000 sdkite-0.3.0/tests/integration/recorded/public_version.json
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-02-26 19:00:13.000000 sdkite-0.3.0/tests/integration/recorded/users_1337.json
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-02-26 19:00:13.000000 sdkite-0.3.0/tests/integration/recorded/users_all_1.json
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-02-26 19:00:13.000000 sdkite-0.3.0/tests/integration/recorded/users_all_2.json
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-02-26 19:00:13.000000 sdkite-0.3.0/tests/integration/recorded/users_all_3.json
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-02-26 19:00:13.000000 sdkite-0.3.0/tests/integration/test_adapter_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-02-26 19:00:13.000000 sdkite-0.3.0/tests/integration/test_http.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 19:00:18.459701 sdkite-0.3.0/tests/unit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 19:00:18.459701 sdkite-0.3.0/tests/unit/http/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-02-26 19:00:13.000000 sdkite-0.3.0/tests/unit/http/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 19:00:18.455701 sdkite-0.3.0/tests/unit/http/engine_replay/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 19:00:18.459701 sdkite-0.3.0/tests/unit/http/engine_replay/base/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-02-26 19:00:13.000000 sdkite-0.3.0/tests/unit/http/engine_replay/base/get_foo.json
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-02-26 19:00:13.000000 sdkite-0.3.0/tests/unit/http/engine_replay/base/get_root.json
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-02-26 19:00:13.000000 sdkite-0.3.0/tests/unit/http/engine_replay/base/post_encoding.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 19:00:18.459701 sdkite-0.3.0/tests/unit/http/engine_replay/base/subfolder/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-02-26 19:00:13.000000 sdkite-0.3.0/tests/unit/http/engine_replay/base/subfolder/in_subfolder.json
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-02-26 19:00:13.000000 sdkite-0.3.0/tests/unit/http/engine_replay/base/wrong_ext.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 19:00:18.463701 sdkite-0.3.0/tests/unit/http/engine_replay/extra/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-02-26 19:00:13.000000 sdkite-0.3.0/tests/unit/http/engine_replay/extra/get_bar.json
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-02-26 19:00:13.000000 sdkite-0.3.0/tests/unit/http/engine_replay/extra/get_foo.json
--rw-r--r--   0 runner    (1001) docker     (123)     9803 2023-02-26 19:00:13.000000 sdkite-0.3.0/tests/unit/http/test_adapter_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-02-26 19:00:13.000000 sdkite-0.3.0/tests/unit/http/test_adapter_adapter_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-02-26 19:00:13.000000 sdkite-0.3.0/tests/unit/http/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     9349 2023-02-26 19:00:13.000000 sdkite-0.3.0/tests/unit/http/test_engine_replay.py
--rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-02-26 19:00:13.000000 sdkite-0.3.0/tests/unit/http/test_engine_replay_recording.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-02-26 19:00:13.000000 sdkite-0.3.0/tests/unit/http/test_engine_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-02-26 19:00:13.000000 sdkite-0.3.0/tests/unit/http/test_model_httpheaderdict.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-02-26 19:00:13.000000 sdkite-0.3.0/tests/unit/http/test_stringescape.py
--rw-r--r--   0 runner    (1001) docker     (123)    12450 2023-02-26 19:00:13.000000 sdkite-0.3.0/tests/unit/http/test_utils_encode_request_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-02-26 19:00:13.000000 sdkite-0.3.0/tests/unit/http/test_utils_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-02-26 19:00:13.000000 sdkite-0.3.0/tests/unit/test_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-02-26 19:00:13.000000 sdkite-0.3.0/tests/unit/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16117 2023-02-26 19:00:13.000000 sdkite-0.3.0/tests/unit/test_pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-02-26 19:00:13.000000 sdkite-0.3.0/tests/unit/test_pagination_pep570.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-02-26 19:00:13.000000 sdkite-0.3.0/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-02-26 19:00:13.000000 sdkite-0.3.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:04:13.957939 sdkite-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-16 19:04:04.000000 sdkite-0.4.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:04:13.949939 sdkite-0.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:04:13.949939 sdkite-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-16 19:04:04.000000 sdkite-0.4.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-16 19:04:04.000000 sdkite-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-16 19:04:04.000000 sdkite-0.4.0/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-16 19:04:04.000000 sdkite-0.4.0/.prettierrc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-16 19:04:04.000000 sdkite-0.4.0/.pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:04:13.953939 sdkite-0.4.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-16 19:04:04.000000 sdkite-0.4.0/.vscode/env
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-16 19:04:04.000000 sdkite-0.4.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-16 19:04:04.000000 sdkite-0.4.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-04-16 19:04:04.000000 sdkite-0.4.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-16 19:04:04.000000 sdkite-0.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-16 19:04:13.957939 sdkite-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-16 19:04:04.000000 sdkite-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-16 19:04:04.000000 sdkite-0.4.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:04:13.953939 sdkite-0.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-04-16 19:04:04.000000 sdkite-0.4.0/docs/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-16 19:04:04.000000 sdkite-0.4.0/docs/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:04:13.953939 sdkite-0.4.0/docs/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-16 19:04:04.000000 sdkite-0.4.0/docs/src/CNAME
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:04:13.953939 sdkite-0.4.0/docs/src/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-16 19:04:04.000000 sdkite-0.4.0/docs/src/css/extra.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-16 19:04:04.000000 sdkite-0.4.0/docs/src/http_auth.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-04-16 19:04:04.000000 sdkite-0.4.0/docs/src/http_engine.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-04-16 19:04:04.000000 sdkite-0.4.0/docs/src/http_replay.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-16 19:04:04.000000 sdkite-0.4.0/docs/src/http_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-16 19:04:04.000000 sdkite-0.4.0/docs/src/http_response.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-04-16 19:04:04.000000 sdkite-0.4.0/docs/src/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-04-16 19:04:04.000000 sdkite-0.4.0/docs/src/pagination.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-04-16 19:04:04.000000 sdkite-0.4.0/docs/src/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-16 19:04:04.000000 sdkite-0.4.0/docs/src/typing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-16 19:04:04.000000 sdkite-0.4.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-16 19:04:04.000000 sdkite-0.4.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-16 19:04:04.000000 sdkite-0.4.0/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-04-16 19:04:13.957939 sdkite-0.4.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      196 2023-04-16 19:04:04.000000 sdkite-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:04:13.949939 sdkite-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:04:13.953939 sdkite-0.4.0/src/sdkite/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-16 19:04:04.000000 sdkite-0.4.0/src/sdkite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-16 19:04:13.000000 sdkite-0.4.0/src/sdkite/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-04-16 19:04:04.000000 sdkite-0.4.0/src/sdkite/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-16 19:04:04.000000 sdkite-0.4.0/src/sdkite/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:04:13.953939 sdkite-0.4.0/src/sdkite/http/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-16 19:04:04.000000 sdkite-0.4.0/src/sdkite/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-16 19:04:04.000000 sdkite-0.4.0/src/sdkite/http/_stringescape.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11488 2023-04-16 19:04:04.000000 sdkite-0.4.0/src/sdkite/http/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-04-16 19:04:04.000000 sdkite-0.4.0/src/sdkite/http/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8533 2023-04-16 19:04:04.000000 sdkite-0.4.0/src/sdkite/http/engine_replay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-04-16 19:04:04.000000 sdkite-0.4.0/src/sdkite/http/engine_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-04-16 19:04:04.000000 sdkite-0.4.0/src/sdkite/http/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10059 2023-04-16 19:04:04.000000 sdkite-0.4.0/src/sdkite/http/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-04-16 19:04:04.000000 sdkite-0.4.0/src/sdkite/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 19:04:04.000000 sdkite-0.4.0/src/sdkite/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-16 19:04:04.000000 sdkite-0.4.0/src/sdkite/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:04:13.953939 sdkite-0.4.0/src/sdkite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-16 19:04:13.000000 sdkite-0.4.0/src/sdkite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-04-16 19:04:13.000000 sdkite-0.4.0/src/sdkite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 19:04:13.000000 sdkite-0.4.0/src/sdkite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-16 19:04:13.000000 sdkite-0.4.0/src/sdkite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-16 19:04:13.000000 sdkite-0.4.0/src/sdkite.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:04:13.953939 sdkite-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:04:13.953939 sdkite-0.4.0/tests/integration/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:04:13.953939 sdkite-0.4.0/tests/integration/recorded/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/integration/recorded/public_version.json
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/integration/recorded/users_1337.json
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/integration/recorded/users_all_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/integration/recorded/users_all_2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/integration/recorded/users_all_3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/integration/test_adapter_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/integration/test_http.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:04:13.957939 sdkite-0.4.0/tests/unit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:04:13.957939 sdkite-0.4.0/tests/unit/http/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/unit/http/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:04:13.949939 sdkite-0.4.0/tests/unit/http/engine_replay/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:04:13.957939 sdkite-0.4.0/tests/unit/http/engine_replay/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/unit/http/engine_replay/base/get_foo.json
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/unit/http/engine_replay/base/get_root.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/unit/http/engine_replay/base/post_encoding.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:04:13.957939 sdkite-0.4.0/tests/unit/http/engine_replay/base/subfolder/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/unit/http/engine_replay/base/subfolder/in_subfolder.json
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/unit/http/engine_replay/base/wrong_ext.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:04:13.957939 sdkite-0.4.0/tests/unit/http/engine_replay/extra/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/unit/http/engine_replay/extra/get_bar.json
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/unit/http/engine_replay/extra/get_foo.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13507 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/unit/http/test_adapter_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12512 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/unit/http/test_adapter_adapter_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/unit/http/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/unit/http/test_engine_replay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7408 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/unit/http/test_engine_replay_recording.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/unit/http/test_engine_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/unit/http/test_model_httpheaderdict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/unit/http/test_stringescape.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12470 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/unit/http/test_utils_encode_request_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/unit/http/test_utils_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/unit/test_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/unit/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16119 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/unit/test_pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/unit/test_pagination_pep570.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-16 19:04:04.000000 sdkite-0.4.0/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-16 19:04:04.000000 sdkite-0.4.0/tox.ini
```

### Comparing `sdkite-0.3.0/.github/workflows/build.yml` & `sdkite-0.4.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `sdkite-0.3.0/.vscode/settings.json` & `sdkite-0.4.0/.vscode/settings.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9259259259259259%*

 * *Differences: {"'files.exclude'": "{'.mypy_cache': True, '.ruff_cache': True}",*

 * * 'delete': "['python.sortImports.args']"}*

```diff
@@ -24,20 +24,19 @@
     "editor.insertSpaces": true,
     "editor.tabSize": 4,
     "files.exclude": {
         "**/*.egg-info": true,
         "**/__pycache__": true,
         ".coverage": true,
         ".eggs": true,
+        ".mypy_cache": true,
         ".pytest_cache": true,
+        ".ruff_cache": true,
         ".tox": true,
         "env": true
     },
     "files.insertFinalNewline": true,
     "python.envFile": "${workspaceFolder}/.vscode/env",
     "python.formatting.provider": "black",
     "python.linting.pylintEnabled": true,
-    "python.sortImports.args": [
-        "-sp .isort.cfg"
-    ],
     "python.testing.pytestEnabled": true
 }
```

### Comparing `sdkite-0.3.0/CHANGELOG.md` & `sdkite-0.4.0/CHANGELOG.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,45 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/), and this project
 adheres to [Semantic Versioning](https://semver.org/).
 
+## [0.4.0] - 2023-04-16
+
+[0.4.0]: https://github.com/rogdham/sdkite/compare/v0.3.0...v0.4.0
+
+v0.4.0 introduces request retrying and timeout
+
+### :boom: Breaking changes
+
+- The requests HTTP engine is now using a timeout of 40 seconds for connection and 30
+  seconds afterwards (or 10 minutes in case of streaming)
+- `HTTPAdapterSpec`'s `headers` parameter is now keyword-only
+
+### :rocket: Added
+
+- HTTP requests are now retried several times in case of exception; this behavior can be
+  modified with the following parameters: `retry_nb_attempts`, `retry_wait_initial`,
+  `retry_wait_max`, `retry_wait_jitter`, and `retry_callback` allows to be notified when
+  a retry is performed
+
+### :bug: Fixes
+
+- Warnings due to wrong usage are now using `UserWarning` instead of `RuntimeWarning`
+
+### :house: Internal
+
+- Add `Adapter._from_adapter_hierarchy` to get easy access to values from the adapter
+  hierarchy
+- Simplify `assert_type` imports following `typing-extensions` requirement on Python up
+  to 3.10
+- Necessary code changes following dev dependency update: mypy
+
 ## [0.3.0] - 2023-02-26
 
 [0.3.0]: https://github.com/rogdham/sdkite/compare/v0.2.0...v0.3.0
 
 v0.3.0 allows HTTP responses to be recorded to be replayed later
 
 ### :rocket: Added
```

### Comparing `sdkite-0.3.0/LICENSE.txt` & `sdkite-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sdkite-0.3.0/PKG-INFO` & `sdkite-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdkite
-Version: 0.3.0
+Version: 0.4.0
 Summary: Simple framework for building SDKs and API clients
 Home-page: https://github.com/rogdham/sdkite
 Author: Rogdham
 Author-email: contact@rogdham.net
 License: MIT
 Project-URL: Documentation, https://sdkite.rogdham.net/
 Project-URL: Source, https://github.com/rogdham/sdkite
@@ -55,18 +55,18 @@
 This project is under heavy development. Breaking changes in future versions are to be
 expected.
 
 Main points before alpha version:
 
 - [x] Minimal documentation
 - [ ] Complete documentation
-- [ ] Handle retrying
 - [ ] Improve HTTP adapter
   - [x] Support for more request body types (basic types)
   - [ ] Support for even more request body types (files, iterables)
+  - [x] Handle retrying
   - [ ] Handle _bad_ status codes
   - [x] Builtin auth handlers like basic auth
   - [x] Usual shortcuts like `.get(...)` for `.request('get', ...)`
   - [ ] Allow to disable interceptors on a specific request
   - [ ] Wrapt `requests`' exceptions
   - [ ] Support more HTTP adapters
 - [ ] Remove `requests` from dependencies
```

### Comparing `sdkite-0.3.0/README.md` & `sdkite-0.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -21,18 +21,18 @@
 This project is under heavy development. Breaking changes in future versions are to be
 expected.
 
 Main points before alpha version:
 
 - [x] Minimal documentation
 - [ ] Complete documentation
-- [ ] Handle retrying
 - [ ] Improve HTTP adapter
   - [x] Support for more request body types (basic types)
   - [ ] Support for even more request body types (files, iterables)
+  - [x] Handle retrying
   - [ ] Handle _bad_ status codes
   - [x] Builtin auth handlers like basic auth
   - [x] Usual shortcuts like `.get(...)` for `.request('get', ...)`
   - [ ] Allow to disable interceptors on a specific request
   - [ ] Wrapt `requests`' exceptions
   - [ ] Support more HTTP adapters
 - [ ] Remove `requests` from dependencies
```

### Comparing `sdkite-0.3.0/docs/conftest.py` & `sdkite-0.4.0/docs/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from requests_mock import Mocker
 
 from sdkite import Client
 from sdkite.http import HTTPRequest, HTTPResponse
 
 
 @pytest.fixture(scope="module", autouse=True)
-def import_pytest(doctest_namespace: Dict[str, object]) -> None:
+def _import_pytest(doctest_namespace: Dict[str, object]) -> None:
     doctest_namespace["Iterator"] = Iterator
     doctest_namespace["Path"] = Path
 
     doctest_namespace["Client"] = Client
 
     def list_spells(
         max_price: int,
@@ -54,15 +54,15 @@
 
     doctest_namespace["list_spells"] = list_spells
     doctest_namespace["list_spells_with_ref"] = list_spells_with_ref
     doctest_namespace["ExampleEngine"] = ExampleEngine
 
 
 @pytest.fixture(autouse=True)
-def patch_http(requests_mock: Mocker) -> None:
+def _patch_http(requests_mock: Mocker) -> None:
     #
     # quickstart
     #
     requests_mock.register_uri(
         "GET",
         "https://api.example.com/world/npc/interact?name=ranis",
         text="Have you found the Telvanni spy?",
@@ -97,15 +97,15 @@
         "https://api.example.com/noauth",
         additional_matcher=lambda request: "Authorization" not in request.headers,
         text="The /noauth endpoint has been called without auth",
     )
 
 
 @pytest.fixture(autouse=True)
-def create_replay_store(tmp_path: Path) -> None:
+def _create_replay_store(tmp_path: Path) -> None:
     store = tmp_path / "replay"
     store.mkdir()
     (store / "ping.json").write_bytes(
         rb"""{
   "request": {
     "method": "GET",
     "url": "https://api.example.com/ping",
@@ -120,14 +120,14 @@
   }
 }
 """
     )
 
 
 @pytest.fixture(autouse=True)
-def change_directory(tmp_path: Path) -> Iterator[None]:
+def _change_directory(tmp_path: Path) -> Iterator[None]:
     cwd = getcwd()
     try:
         chdir(tmp_path)
         yield
     finally:
         chdir(cwd)
```

### Comparing `sdkite-0.3.0/docs/mkdocs.yml` & `sdkite-0.4.0/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `sdkite-0.3.0/docs/src/css/extra.css` & `sdkite-0.4.0/docs/src/css/extra.css`

 * *Files identical despite different names*

### Comparing `sdkite-0.3.0/docs/src/http_auth.md` & `sdkite-0.4.0/docs/src/http_auth.md`

 * *Files identical despite different names*

### Comparing `sdkite-0.3.0/docs/src/http_engine.md` & `sdkite-0.4.0/docs/src/http_engine.md`

 * *Files identical despite different names*

### Comparing `sdkite-0.3.0/docs/src/http_replay.md` & `sdkite-0.4.0/docs/src/http_replay.md`

 * *Files identical despite different names*

### Comparing `sdkite-0.3.0/docs/src/http_request.md` & `sdkite-0.4.0/docs/src/http_request.md`

 * *Files 18% similar despite different names*

```diff
@@ -66,7 +66,27 @@
 
 ## Stream mode
 
 To ask the server to stream the response, set the `stream_response` parameter to `True`.
 
 It is then recommended to use the `data_stream` attribute of
 [the response object](http_response.md).
+
+## Retry options
+
+If an exception is raised when performing the request, 2 more attempts will be made with
+some wait time between them.
+
+This can be customized by passing some arguments:
+
+- `retry_nb_attempts` to specify the total number of attempts (defaults to 3 attempts)
+- `retry_wait_initial`, `retry_wait_max` and `retry_wait_jitter` allow to specify the
+  exponential backoff parameters for the retry (they default to 1s, 60s and 1s
+  respectively)
+
+Finally, a `retry_callback` can be passed to be notified when a retry is performed. This
+can be used for logging purposes for instance.
+
+All these parameters can be specified (by order of precedence):
+
+- When calling a request method (or get, post, etc.)
+- On the HTTPAdapterSpec of each client
```

### Comparing `sdkite-0.3.0/docs/src/http_response.md` & `sdkite-0.4.0/docs/src/http_response.md`

 * *Files identical despite different names*

### Comparing `sdkite-0.3.0/docs/src/index.md` & `sdkite-0.4.0/docs/src/index.md`

 * *Files identical despite different names*

### Comparing `sdkite-0.3.0/docs/src/pagination.md` & `sdkite-0.4.0/docs/src/pagination.md`

 * *Files identical despite different names*

### Comparing `sdkite-0.3.0/docs/src/quickstart.md` & `sdkite-0.4.0/docs/src/quickstart.md`

 * *Files identical despite different names*

### Comparing `sdkite-0.3.0/docs/src/typing.md` & `sdkite-0.4.0/docs/src/typing.md`

 * *Files identical despite different names*

### Comparing `sdkite-0.3.0/mypy.ini` & `sdkite-0.4.0/mypy.ini`

 * *Files identical despite different names*

### Comparing `sdkite-0.3.0/setup.cfg` & `sdkite-0.4.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -40,13 +40,14 @@
 python_requires = >=3.7
 setup_requires = 
 	setuptools_scm
 	wheel
 install_requires = 
 	requests>=2.28.1
 	backports.cached-property>=1.0.2;python_version<"3.8"
+	tenacity>=8.2.2
 	typing-extensions>=4.5.0;python_version<"3.11"
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `sdkite-0.3.0/src/sdkite/adapter.py` & `sdkite-0.4.0/src/sdkite/adapter.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,26 +30,27 @@
     _attr_name: str
     _clients: Tuple[Client, ...]
 
     @property
     def _adapters(self) -> Tuple[Self, ...]:
         return tuple(getattr(client, self._attr_name) for client in self._clients)
 
+    def _from_adapter_hierarchy(self, attr_name: str, *values: Any) -> Tuple[Any, ...]:
+        return tuple(getattr(adapter, attr_name) for adapter in self._adapters) + values
+
 
 def create_adapter_proxy(
     adapter: A,
     attr_name: str,
     clients: Tuple[Client, ...],
     context: Dict[str, Any],
 ) -> A:
     klass = type(adapter)
 
-    # pylint: disable=unused-argument
-
-    def init(self: Any) -> None:
+    def init(_: Any) -> None:
         pass
 
     def getattribute(self: Any, name: str) -> Any:
         if name == "_attr_name":
             return attr_name
         if name == "_clients":
             return clients
@@ -57,15 +58,15 @@
             return context[name]
         try:
             attr = super(type(self), self).__getattribute__(name)
         except AttributeError:
             attr = getattr(adapter, name)
         return attr
 
-    def setattribute(self: Any, name: str, value: Any) -> None:
+    def setattribute(_: Any, name: str, value: Any) -> None:
         if name in ("_attr_name", "_clients"):
             raise RuntimeError(f"Attribute {name} is read-only")  # pragma: no cover
         if name in context:
             context[name] = value
         else:
             setattr(adapter, name, value)
 
@@ -138,16 +139,16 @@
                         raise TypeError(
                             f"Client '{type(clients[-1]).__name__}' has a wrong adapter spec:"
                             f" got '{last_descriptor_type.__name__}'"
                             f" instead of '{type(descriptor).__name__}'"
                         )
                     last_descriptor_type = type(descriptor)
                     clients.append(current_client)
-                if current_client._parent:
-                    current_client = current_client._parent
+                if current_client._parent:  # noqa: SLF001
+                    current_client = current_client._parent  # noqa: SLF001
                 else:
                     if sys.version_info < (3, 10):  # pragma: no cover
                         # fix coverage issue on some Python versions
                         # see https://github.com/nedbat/coveragepy/issues/1480
                         pass
                     break
             clients.reverse()
```

### Comparing `sdkite-0.3.0/src/sdkite/client.py` & `sdkite-0.4.0/src/sdkite/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,9 +19,9 @@
                 try:
                     client = attr_type()
                 except RecursionError as ex:
                     raise TypeError(
                         "Clients refer each other (found for"
                         f" {attr_type.__name__} used as {cls.__name__}.{attr_name})"
                     ) from ex
-                client._parent = self
+                client._parent = self  # noqa: SLF001
                 setattr(self, attr_name, client)
```

### Comparing `sdkite-0.3.0/src/sdkite/http/__init__.py` & `sdkite-0.4.0/src/sdkite/http/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from sdkite.http.adapter import HTTPAdapter, HTTPAdapterSendRequest, HTTPAdapterSpec
 from sdkite.http.auth import BasicAuth, NoAuth
 from sdkite.http.model import (
     HTTPBodyEncoding,
     HTTPHeaderDict,
     HTTPRequest,
+    HTTPRequestAttemptInfo,
     HTTPResponse,
 )
 
 __all__ = (
     # sdkite.http.adapter
     "HTTPAdapter",
     "HTTPAdapterSendRequest",
@@ -15,9 +16,10 @@
     # sdkite.http.auth
     "BasicAuth",
     "NoAuth",
     # sdkite.http.model
     "HTTPBodyEncoding",
     "HTTPHeaderDict",
     "HTTPRequest",
+    "HTTPRequestAttemptInfo",
     "HTTPResponse",
 )
```

### Comparing `sdkite-0.3.0/src/sdkite/http/_stringescape.py` & `sdkite-0.4.0/src/sdkite/http/_stringescape.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # see also: https://github.com/python/cpython/issues/74773
 
 _dumps_table: Dict[int, str] = {}
 _loads_table: Dict[bytes, int] = {}
 for _i in range(256):
     _value = f"\\x{_i:02x}"
     _loads_table[_value.encode("ascii")] = _i
-    if 32 <= _i <= 126 and _i != 92:
+    if ord(" ") <= _i <= ord("~") and _i != ord("\\"):
         _value = chr(_i)
         _loads_table[_value.encode("ascii")] = _i
     _dumps_table[_i] = _value
 for _i, _value in [
     (0, "\\0"),
     (9, "\\t"),
     (10, "\\n"),
```

### Comparing `sdkite-0.3.0/src/sdkite/http/auth.py` & `sdkite-0.4.0/src/sdkite/http/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,17 +64,15 @@
         # pylint: disable=line-too-long
 
         # UTF-8 encoding seems to be the de-facto standard in browsers
         # see e.g. https://developer.mozilla.org/en-US/docs/Web/HTTP/Authentication#character_encoding_of_http_authentication
 
         # pylint: enable=line-too-long
 
-        credentials = b64encode(
-            f"{self.username}:{self.password}".encode("utf8")
-        ).decode()
+        credentials = b64encode(f"{self.username}:{self.password}".encode()).decode()
         request.headers["Authorization"] = f"Basic {credentials}"
         return request
 
 
 class NoAuth(Auth):
     def __call__(self, request: HTTPRequest, _: HTTPAdapter) -> HTTPRequest:
         return request
```

### Comparing `sdkite-0.3.0/src/sdkite/http/engine_replay.py` & `sdkite-0.4.0/src/sdkite/http/engine_replay.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,19 +63,18 @@
     def data_stream(self) -> Iterator[bytes]:
         return iter(self.recorded_response["body"])
 
     @property
     def data_bytes(self) -> bytes:
         try:
             parts = [next(self.data_stream)]
-        except Exception:
-            # pylint: disable=raise-missing-from
+        except StopIteration:
             raise ValueError(
                 "The data_xxx attributes can be only accessed once with the replay engine"
-            )
+            ) from None
         parts.extend(self.data_stream)
         return b"".join(parts)
 
     @property
     def data_str(self) -> str:
         return self.data_bytes.decode()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `sdkite-0.3.0/src/sdkite/http/engine_requests.py` & `sdkite-0.4.0/src/sdkite/http/engine_requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 if sys.version_info < (3, 9):  # pragma: no cover
     from typing import Iterator
 else:  # pragma: no cover
     from collections.abc import Iterator
 
 
 class HTTPResponseRequests(HTTPResponse):
-    def __init__(self, response: Response):
+    def __init__(self, response: Response) -> None:
         self._response = response
 
     @property
     def raw(self) -> Response:
         return self._response
 
     @property
@@ -68,10 +68,11 @@
         response = self.session.request(
             method=request.method,
             url=request.url,
             headers=headers,
             data=request.body,
             stream=request.stream_response,
             allow_redirects=False,
+            timeout=(40, 600 if request.stream_response else 30),
         )
 
         return HTTPResponseRequests(response)
```

### Comparing `sdkite-0.3.0/src/sdkite/http/model.py` & `sdkite-0.4.0/src/sdkite/http/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     def __len__(self) -> int:
         return len(self._contents)
 
     def __getitem__(self, key: str) -> str:
         try:
             return ", ".join(self._contents[key.lower()][1:])
         except KeyError:
-            raise KeyError(key)  # pylint: disable=raise-missing-from
+            raise KeyError(key) from None
 
     def __setitem__(self, key: str, value: str) -> None:
         self._contents[key.lower()] = [key, value]
 
     def __delitem__(self, key: str) -> None:
         del self._contents[key.lower()]
 
@@ -124,7 +124,15 @@
 
     @property
     @abstractmethod
     def data_json(self) -> object:
         """
         The body of the response JSON-decoded, for easier access.
         """
+
+
+@dataclass
+class HTTPRequestAttemptInfo:
+    attempt_number: int
+    exception: BaseException
+    initial_request: HTTPRequest
+    seconds_since_start: float
```

### Comparing `sdkite-0.3.0/src/sdkite/http/utils.py` & `sdkite-0.4.0/src/sdkite/http/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,81 +65,89 @@
 
 
 @contextmanager
 def _visitor_obj(path: str, obj: object) -> Iterator[None]:
     try:
         yield
     except _VisitorTypeError as ex:
-        raise ex.context(path)
+        raise ex.context(path) from None
     except TypeError:
-        raise _VisitorTypeError(path, obj=obj)  # pylint: disable=raise-missing-from
+        raise _VisitorTypeError(path, obj=obj) from None
 
 
 class _Visitor:
     def visit(self, obj: object) -> Iterator[bytes]:
         try:
             for klass in (NoneType, str, bytes, bool, int, float):
                 if isinstance(obj, klass):
                     yield from self._visit_raw(obj)
                     return
             if isinstance(obj, (list, tuple, set)):
                 yield from self._visit_sequence_start()
                 first = True
                 for i, value in enumerate(sorted(obj) if isinstance(obj, set) else obj):
                     with _visitor_obj(repr(i), obj=value):
-                        yield from self._visit_sequence_item_start(first)
+                        yield from self._visit_sequence_item_start(first=first)
                         yield from self.visit(value)
-                        yield from self._visit_sequence_item_end(first)
+                        yield from self._visit_sequence_item_end(first=first)
                     first = False
                 yield from self._visit_sequence_end()
                 return
             if isinstance(obj, dict):
                 yield from self._visit_mapping_start()
                 first = True
                 for key in sorted(obj):
                     with _visitor_obj(repr(key), obj=obj[key]):
-                        yield from self._visit_mapping_item_start(key, first)
+                        yield from self._visit_mapping_item_start(key, first=first)
                         yield from self.visit(obj[key])
-                        yield from self._visit_mapping_item_end(key, first)
+                        yield from self._visit_mapping_item_end(key, first=first)
                     first = False
                 yield from self._visit_mapping_end()
                 return
             raise TypeError
         except _VisitorTypeError:
             raise
         except TypeError:
-            raise _VisitorTypeError(obj=obj)  # pylint: disable=raise-missing-from
+            raise _VisitorTypeError(obj=obj) from None
 
     # pylint: disable=unused-argument
 
-    def _visit_raw(self, obj: object) -> Iterator[bytes]:
+    def _visit_raw(self, obj: object) -> Iterator[bytes]:  # noqa: ARG002
         return _EMPTY_ITERATOR  # pragma: no cover
 
     def _visit_sequence_start(self) -> Iterator[bytes]:
         return _EMPTY_ITERATOR  # pragma: no cover
 
     def _visit_sequence_end(self) -> Iterator[bytes]:
         return _EMPTY_ITERATOR  # pragma: no cover
 
-    def _visit_sequence_item_start(self, first: bool) -> Iterator[bytes]:
+    def _visit_sequence_item_start(
+        self, *, first: bool  # noqa: ARG002
+    ) -> Iterator[bytes]:
         return _EMPTY_ITERATOR  # pragma: no cover
 
-    def _visit_sequence_item_end(self, first: bool) -> Iterator[bytes]:
+    def _visit_sequence_item_end(
+        self, *, first: bool  # noqa: ARG002
+    ) -> Iterator[bytes]:
         return _EMPTY_ITERATOR  # pragma: no cover
 
     def _visit_mapping_start(self) -> Iterator[bytes]:
         return _EMPTY_ITERATOR  # pragma: no cover
 
     def _visit_mapping_end(self) -> Iterator[bytes]:
         return _EMPTY_ITERATOR  # pragma: no cover
 
-    def _visit_mapping_item_start(self, key: object, first: bool) -> Iterator[bytes]:
+    def _visit_mapping_item_start(
+        self, key: object, *, first: bool  # noqa: ARG002
+    ) -> Iterator[bytes]:
         return _EMPTY_ITERATOR  # pragma: no cover
 
-    def _visit_mapping_item_end(self, key: object, first: bool) -> Iterator[bytes]:
+    def _visit_mapping_item_end(
+        self, key: object, *, first: bool  # noqa: ARG002
+    ) -> Iterator[bytes]:
         return _EMPTY_ITERATOR  # pragma: no cover
 
 
 class _VisitorNone(_Visitor):
     def _visit_raw(self, obj: object) -> Iterator[bytes]:
         if obj is None:
             return
@@ -164,25 +172,25 @@
 
     def _visit_sequence_start(self) -> Iterator[bytes]:
         yield b"["
 
     def _visit_sequence_end(self) -> Iterator[bytes]:
         yield b"]"
 
-    def _visit_sequence_item_start(self, first: bool) -> Iterator[bytes]:
+    def _visit_sequence_item_start(self, *, first: bool) -> Iterator[bytes]:
         if not first:
             yield b","
 
     def _visit_mapping_start(self) -> Iterator[bytes]:
         yield b"{"
 
     def _visit_mapping_end(self) -> Iterator[bytes]:
         yield b"}"
 
-    def _visit_mapping_item_start(self, key: object, first: bool) -> Iterator[bytes]:
+    def _visit_mapping_item_start(self, key: object, *, first: bool) -> Iterator[bytes]:
         if not first:
             yield b","
         with _visitor_obj(_VisitorTypeError.MAPPING_KEY_PATH, obj=key):
             yield from self._visit_raw(key)
         yield b":"
 
 
@@ -204,15 +212,15 @@
 
     def _visit_mapping_start(self) -> Iterator[bytes]:
         if not self.root:
             raise TypeError
         self.root = False
         return _EMPTY_ITERATOR
 
-    def _visit_mapping_item_start(self, key: object, first: bool) -> Iterator[bytes]:
+    def _visit_mapping_item_start(self, key: object, *, first: bool) -> Iterator[bytes]:
         if not first:
             yield b"&"
         with _visitor_obj(_VisitorTypeError.MAPPING_KEY_PATH, obj=key):
             yield from self._visit_raw(key)
         yield b"="
 
 
@@ -238,28 +246,32 @@
 
     def _visit_mapping_start(self) -> Iterator[bytes]:
         if not self.root:
             raise TypeError
         self.root = False
         return _EMPTY_ITERATOR
 
-    def _visit_mapping_item_start(self, key: object, first: bool) -> Iterator[bytes]:
+    def _visit_mapping_item_start(
+        self, key: object, *, first: bool  # noqa: ARG002
+    ) -> Iterator[bytes]:
         with _visitor_obj(_VisitorTypeError.MAPPING_KEY_PATH, obj=key):
             name = b"".join(self._visit_raw(key))
         yield (
             b"--%s\r\n"
             b'Content-Disposition: form-data; name="%s"\r\n'
             b"Content-Type: application/octet-stream\r\n"
             b"\r\n"
         ) % (
             self.boundary,
             urlencode(name),
         )
 
-    def _visit_mapping_item_end(self, key: object, first: bool) -> Iterator[bytes]:
+    def _visit_mapping_item_end(
+        self, key: object, *, first: bool  # noqa: ARG002
+    ) -> Iterator[bytes]:
         yield b"\r\n"
 
     def _visit_mapping_end(self) -> Iterator[bytes]:
         yield b"--%s--\r\n" % self.boundary
 
 
 def encode_request_body(
@@ -269,17 +281,16 @@
     content_type: Optional[str] = None
     original_encoding = encoding
 
     if encoding == HTTPBodyEncoding.AUTO:
         encoding = HTTPBodyEncoding.JSON
         if isinstance(body, (bytes, str, NoneType)):
             encoding = HTTPBodyEncoding.NONE
-        elif isinstance(body, dict):
-            if any(isinstance(key, bytes) for key in body):
-                encoding = HTTPBodyEncoding.URLENCODE
+        elif isinstance(body, dict) and any(isinstance(key, bytes) for key in body):
+            encoding = HTTPBodyEncoding.URLENCODE
 
     visitor: _Visitor
     if encoding == HTTPBodyEncoding.NONE:
         visitor = _VisitorNone()
     elif encoding == HTTPBodyEncoding.JSON:
         visitor = _VisitorJSON()
         content_type = "application/json"
@@ -297,10 +308,10 @@
         data = b"".join(iterator)
     except _VisitorTypeError as ex:
         error_msg = "Cannot encode body"
         if ex.path:
             error_msg += f" ({'>'.join(ex.path)})"
         error_msg += f" of type '{type(ex.obj).__name__}'"
         error_msg += f" with '{original_encoding.name}' encoding"
-        raise TypeError(error_msg)  # pylint: disable=raise-missing-from
+        raise TypeError(error_msg) from None
 
     return data, content_type
```

### Comparing `sdkite-0.3.0/src/sdkite/pagination.py` & `sdkite-0.4.0/src/sdkite/pagination.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from contextlib import suppress
 from functools import wraps
 from inspect import Parameter, signature
 import sys
 from typing import Any, TypeVar, Union, overload
 
 if sys.version_info < (3, 8):  # pragma: no cover
     from typing_extensions import Protocol
@@ -154,36 +155,35 @@
                 raise  # pragma: no cover
             arguments.apply_defaults()
 
             while not pagination.finished:
                 iterable = fct(*arguments.args, **arguments.kwargs)
                 empty = True
                 for item in iterable:
-                    pagination._offset += 1
+                    pagination._offset += 1  # noqa: SLF001
                     empty = False
                     yield item
                 if empty and stop_when_empty:
                     pagination.finish()
                     break
-                pagination._page += 1
+                pagination._page += 1  # noqa: SLF001
 
         # fix the signature and annotations
 
         # the return value hint is complex to compute exactly from fct's return value
         # e.g. consider 'list[int] | str' should be transformed to 'Iterator[int | str]'
         # so we are just using 'Iterator[Any]'
 
         # see https://github.com/python/mypy/issues/12472 for ignore below
-        wrapped.__signature__ = sig.replace(  # type: ignore
+        wrapped.__signature__ = sig.replace(  # type: ignore[attr-defined]
             parameters=parameters[:param_pos] + parameters[param_pos + 1 :],
             return_annotation=Iterator[Any],
         )
 
-        try:
+        with suppress(KeyError):  # maybe no type hint
             del wrapped.__annotations__["pagination"]
-        except KeyError:
-            pass  # maybe no type hint
         wrapped.__annotations__["return"] = Iterator[Any]
 
         return wrapped
 
-    return paginated_decorator
+    # see https://github.com/python/mypy/issues/15065 for the ignore below
+    return paginated_decorator  # type: ignore[return-value]
```

### Comparing `sdkite-0.3.0/src/sdkite.egg-info/PKG-INFO` & `sdkite-0.4.0/src/sdkite.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdkite
-Version: 0.3.0
+Version: 0.4.0
 Summary: Simple framework for building SDKs and API clients
 Home-page: https://github.com/rogdham/sdkite
 Author: Rogdham
 Author-email: contact@rogdham.net
 License: MIT
 Project-URL: Documentation, https://sdkite.rogdham.net/
 Project-URL: Source, https://github.com/rogdham/sdkite
@@ -55,18 +55,18 @@
 This project is under heavy development. Breaking changes in future versions are to be
 expected.
 
 Main points before alpha version:
 
 - [x] Minimal documentation
 - [ ] Complete documentation
-- [ ] Handle retrying
 - [ ] Improve HTTP adapter
   - [x] Support for more request body types (basic types)
   - [ ] Support for even more request body types (files, iterables)
+  - [x] Handle retrying
   - [ ] Handle _bad_ status codes
   - [x] Builtin auth handlers like basic auth
   - [x] Usual shortcuts like `.get(...)` for `.request('get', ...)`
   - [ ] Allow to disable interceptors on a specific request
   - [ ] Wrapt `requests`' exceptions
   - [ ] Support more HTTP adapters
 - [ ] Remove `requests` from dependencies
```

### Comparing `sdkite-0.3.0/src/sdkite.egg-info/SOURCES.txt` & `sdkite-0.4.0/src/sdkite.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 .pylintrc
 CHANGELOG.md
 LICENSE.txt
 README.md
 dev-requirements.txt
 mypy.ini
 pytest.ini
+ruff.toml
 setup.cfg
 setup.py
 tox.ini
 .github/workflows/build.yml
 .vscode/env
 .vscode/launch.json
 .vscode/settings.json
```

### Comparing `sdkite-0.3.0/tests/conftest.py` & `sdkite-0.4.0/tests/conftest.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import List
 
 import pytest
 
 
 def pytest_collection_modifyitems(
     # pylint: disable=unused-argument
-    config: pytest.Config,
+    config: pytest.Config,  # noqa: ARG001
     items: List[pytest.Item],
 ) -> None:
     root = Path(__file__).parent.parent
     for item in items:
         relative = Path(item.fspath).parent.relative_to(root)
         mark = next(part for part in relative.parts if part != "tests")
         item.add_marker(getattr(pytest.mark, mark))
```

### Comparing `sdkite-0.3.0/tests/integration/test_adapter_simple.py` & `sdkite-0.4.0/tests/integration/test_adapter_simple.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 from io import SEEK_END, StringIO
-from typing import TYPE_CHECKING, Any
+import sys
 
 from sdkite import AdapterSpec, Client
 
-if TYPE_CHECKING:
+if sys.version_info < (3, 11):  # pragma: no cover
     from typing_extensions import assert_type
-else:
-    # no need to have typing_extensions installed
-    def assert_type(val: Any, _: Any) -> Any:
-        return val
+else:  # pragma: no cover
+    from typing import assert_type
 
 
 class ValueSpec(AdapterSpec[StringIO]):
     def _create_adapter(self) -> StringIO:
         return StringIO()  # not an Adapter instance
 
 
@@ -58,28 +56,28 @@
     assert isinstance(assert_type(client.read._value, StringIO), StringIO)
 
     assert isinstance(assert_type(RootClient._value, ValueSpec), ValueSpec)
 
 
 def test_complete() -> None:
     client = RootClient()
-    assert client.read.normal() == ""
-    assert client.read.upper() == ""
+    assert not client.read.normal()
+    assert not client.read.upper()
 
     client.write.append("Hello")
     assert client.read.normal() == "Hello"
     assert client.read.upper() == "HELLO"
 
     client.write.append(", world!")
     assert client.read.normal() == "Hello, world!"
     assert client.read.upper() == "HELLO, WORLD!"
 
     client.write.erase()
-    assert client.read.normal() == ""
-    assert client.read.upper() == ""
+    assert not client.read.normal()
+    assert not client.read.upper()
 
 
 def test_two_clients() -> None:
     # two client instances are independent
     client0 = RootClient()
     client1 = RootClient()
     client0.write.append("Hello!")
@@ -91,10 +89,10 @@
 class RootClientMissingValue(Client):
     read: ReadClient
     write: WriteClient
 
 
 def test_root_client_missing_value() -> None:
     client = RootClientMissingValue()
-    assert client.read.normal() == ""
+    assert not client.read.normal()
     client.write.append("Hello")
-    assert client.read.normal() == ""  # did not change
+    assert not client.read.normal()  # did not change
```

### Comparing `sdkite-0.3.0/tests/integration/test_http.py` & `sdkite-0.4.0/tests/integration/test_http.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     def __init__(self, url: str, password: str) -> None:
         super().__init__()
         self._http.url = url
         self._auth.password = password
 
 
 @pytest.fixture
-def mock_http_requests(requests_mock: Mocker) -> None:
+def _mock_http_requests(requests_mock: Mocker) -> None:
     common_response: Any = {
         "reason": "OK",
         "headers": {"server": "nginx"},
     }
 
     requests_mock.register_uri(
         # request
@@ -110,17 +110,16 @@
         request_headers={"authorization": "Basic dGVzdHM6czNjcjN0"},
         # response
         content=b"[]",
         **common_response,
     )
 
 
-def test_http(
-    mock_http_requests: object,  # pylint: disable=redefined-outer-name,unused-argument
-) -> None:
+@pytest.mark.usefixtures("_mock_http_requests")
+def test_http() -> None:
     client = Api("https://www.example.com/api/v1", "s3cr3t")
 
     assert client.public.version() == "1.2.3"
 
     user = client.users.get(1337)
     assert user == User(name="John Doe", age=42)
 
@@ -136,17 +135,17 @@
 def replay_request_modifier(request: HTTPRequest) -> HTTPRequest:
     if "Authorization" in request.headers:
         request.headers["Authorization"] = "Basic redacted"
     return request
 
 
 def test_http_replay_replay(
-    # notice how we don't use `mock_http_requests` here
+    # notice how we don't use `_mock_http_requests` here
     # still patching requests just in case
-    requests_mock: Mocker,  # pylint: disable=unused-argument
+    requests_mock: Mocker,  # pylint: disable=unused-argument # noqa: ARG001
 ) -> None:
     Api._http.set_engine(  # pylint: disable=protected-access
         HTTPEngineReplay,
         [REPLAY_PATH],
         replay_request_modifier=replay_request_modifier,
     )
 
@@ -165,18 +164,16 @@
         User(name="John Doe", age=42),
         User(name="Alice Doe", age=41),
         User(name="Bob Doe", age=10),
         User(name="Carole Doe", age=12),
     ]
 
 
-def test_http_replay_record(
-    mock_http_requests: object,  # pylint: disable=redefined-outer-name,unused-argument
-    tmp_path: Path,
-) -> None:
+@pytest.mark.usefixtures("_mock_http_requests")
+def test_http_replay_record(tmp_path: Path) -> None:
     def recording_response_modifier(response: HTTPResponseReplay) -> HTTPResponseReplay:
         return response.replace(
             headers={
                 **response.headers,
                 "server": "apache",
             }
         )
```

### Comparing `sdkite-0.3.0/tests/unit/http/engine_replay/base/post_encoding.json` & `sdkite-0.4.0/tests/unit/http/engine_replay/base/post_encoding.json`

 * *Files identical despite different names*

### Comparing `sdkite-0.3.0/tests/unit/http/test_adapter_adapter_spec.py` & `sdkite-0.4.0/tests/unit/http/test_adapter_adapter_spec.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,25 @@
+from contextlib import nullcontext
 import re
-from typing import TYPE_CHECKING
-from unittest.mock import Mock
+from typing import TYPE_CHECKING, Any
+from unittest.mock import Mock, call
 
 import pytest
 
 from sdkite.http import (
     HTTPAdapter,
     HTTPAdapterSendRequest,
     HTTPAdapterSpec,
     HTTPBodyEncoding,
     HTTPHeaderDict,
     HTTPRequest,
     HTTPResponse,
 )
 from sdkite.http import adapter as adapter_module
+from sdkite.http.adapter import _BeforeSleep
 
 if TYPE_CHECKING:
     from sdkite import Client
 else:
     # we want independent unit tests
     Client = object
 
@@ -47,49 +49,138 @@
     data_stream = iter(())
     data_bytes = b""
     data_str = ""
     data_json = None
 
 
 @pytest.fixture(autouse=True)
-def patched_adapter(monkeypatch: pytest.MonkeyPatch) -> None:
+def _patched_adapter(monkeypatch: pytest.MonkeyPatch) -> None:
     engine = Mock()
     engine.return_value = lambda request: FakeResponse("send_request", request)
     monkeypatch.setattr(adapter_module, "HTTPEngineRequests", engine)
 
 
-def test_no_interceptor() -> None:
+@pytest.fixture
+def patched_tenacity(monkeypatch: pytest.MonkeyPatch) -> Mock:
+    tenacity = Mock()
+
+    tenacity.Retrying.return_value = [nullcontext()]
+    tenacity.stop_after_attempt.side_effect = call
+    tenacity.wait_exponential_jitter.side_effect = call
+
+    for attr in ["Retrying", "stop_after_attempt", "wait_exponential_jitter"]:
+        monkeypatch.setattr(adapter_module, attr, getattr(tenacity, attr))
+
+    return tenacity
+
+
+def test_base(
+    patched_tenacity: Mock,  # pylint: disable=redefined-outer-name
+) -> None:
     class Klass(Client):
         _parent = None
 
         xxx = HTTPAdapterSpec(url="https://www.example.com/xxx")
 
+    expected_request = HTTPRequest(
+        method="GET",
+        url="https://www.example.com/xxx/uvw",
+        headers=HTTPHeaderDict(),
+        body=b"",
+        stream_response=False,
+    )
+
     client = Klass()
     response = client.xxx.request("GET", "uvw")
-    assert response == FakeResponse(
-        "send_request",
-        HTTPRequest(
-            method="GET",
-            url="https://www.example.com/xxx/uvw",
-            headers=HTTPHeaderDict(),
-            body=b"",
-            stream_response=False,
-        ),
+    assert response == FakeResponse("send_request", expected_request)
+
+    assert patched_tenacity.Retrying.call_args_list == [
+        call(
+            stop=patched_tenacity.stop_after_attempt(3),
+            wait=patched_tenacity.wait_exponential_jitter(
+                initial=1.0, max=60.0, jitter=1.0
+            ),
+            before_sleep=_BeforeSleep(None, expected_request),
+            reraise=True,
+        )
+    ]
+
+
+def test_retry_at_spec_level(
+    patched_tenacity: Mock,  # pylint: disable=redefined-outer-name
+) -> None:
+    # these get deepcopy-ed so Mock() would not work
+    retry_callback0: Any = "retry_callback0"
+    retry_callback1: Any = "retry_callback1"
+
+    class Klass(Client):
+        _parent = None
+
+        xxx = HTTPAdapterSpec(
+            url="https://www.example.com/xxx",
+            retry_nb_attempts=1,
+            retry_wait_initial=2.0,
+            retry_wait_max=3.0,
+            retry_wait_jitter=4.0,
+            retry_callback=retry_callback0,
+        )
+
+    expected_request = HTTPRequest(
+        method="GET",
+        url="https://www.example.com/xxx/uvw",
+        headers=HTTPHeaderDict(),
+        body=b"",
+        stream_response=False,
     )
 
+    client = Klass()
+
+    client.xxx.request("GET", "uvw")
+    assert patched_tenacity.Retrying.call_args_list == [
+        call(
+            stop=patched_tenacity.stop_after_attempt(1),
+            wait=patched_tenacity.wait_exponential_jitter(
+                initial=2.0, max=3.0, jitter=4.0
+            ),
+            before_sleep=_BeforeSleep(retry_callback0, expected_request),
+            reraise=True,
+        )
+    ]
+    patched_tenacity.Retrying.reset_mock()
+
+    client.xxx.request(
+        "GET",
+        "uvw",
+        retry_nb_attempts=6,
+        retry_wait_initial=7.0,
+        retry_wait_max=8.0,
+        retry_wait_jitter=9.0,
+        retry_callback=retry_callback1,
+    )
+    assert patched_tenacity.Retrying.call_args_list == [
+        call(
+            stop=patched_tenacity.stop_after_attempt(6),
+            wait=patched_tenacity.wait_exponential_jitter(
+                initial=7.0, max=8.0, jitter=9.0
+            ),
+            before_sleep=_BeforeSleep(retry_callback1, expected_request),
+            reraise=True,
+        )
+    ]
+
 
 def test_overidden_content_type() -> None:
     class Klass(Client):
         _parent = None
 
         xxx = HTTPAdapterSpec(url="https://www.example.com/xxx")
 
     client = Klass()
     with pytest.warns(
-        RuntimeWarning,
+        UserWarning,
         match=re.escape(
             "The 'content-type' header is being overridden due to request body encoding"
             " HTTPBodyEncoding.JSON (from 'custom' to 'application/json')"
         ),
     ):
         response = client.xxx.request(
             "GET",
@@ -246,24 +337,24 @@
             return request
 
         @xxx.intercept_response(1)
         def xxx_resp(self, response: HTTPResponse, _: HTTPAdapter) -> HTTPResponse:
             return FakeResponse("xxx_resp", response)
 
     with pytest.warns(
-        RuntimeWarning,
+        UserWarning,
         match=re.escape(
             "Interceptor 'xxx_req' of 'xxx' has already been registered"
             " with order 0, ignoring new registration with order 42"
         ),
     ):
         Klass.xxx.register_interceptor("request_interceptor", "xxx_req", 42)
 
     with pytest.warns(
-        RuntimeWarning,
+        UserWarning,
         match=re.escape(
             "Interceptor 'xxx_resp' of 'xxx' has already been registered"
             " with order 1, ignoring new registration with order 42"
         ),
     ):
         Klass.xxx.register_interceptor("response_interceptor", "xxx_resp", 42)
```

### Comparing `sdkite-0.3.0/tests/unit/http/test_auth.py` & `sdkite-0.4.0/tests/unit/http/test_auth.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,23 +14,23 @@
 
     client0 = WithBasicAuth()
     client1 = WithBasicAuth()
     adapter = Mock()
 
     # modify creds on one client instance
     client1.auth.username = "Alice"
-    client1.auth.password = "$ecr3t"
+    client1.auth.password = "$ecr3t"  # noqa: S105
 
     # did not modify creds on class instance
     assert WithBasicAuth.auth.username == "user"
-    assert WithBasicAuth.auth.password == "password"
+    assert WithBasicAuth.auth.password == "password"  # noqa: S105
 
     # did not modify creds on other client instance
     assert client0.auth.username == "user"
-    assert client0.auth.password == "password"
+    assert client0.auth.password == "password"  # noqa: S105
 
     for i, client, cred in [
         (0, client0, "dXNlcjpwYXNzd29yZA=="),
         (1, client1, "QWxpY2U6JGVjcjN0"),
     ]:
         request = HTTPRequest(
             method="GET",
```

### Comparing `sdkite-0.3.0/tests/unit/http/test_engine_replay.py` & `sdkite-0.4.0/tests/unit/http/test_engine_replay.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from dataclasses import replace
 from pathlib import Path
+import re
 from typing import Dict, cast
 
 import pytest
 
 from sdkite.http import HTTPHeaderDict, HTTPRequest
 from sdkite.http.engine_replay import (
     HTTPEngineReplay,
@@ -20,16 +21,19 @@
         "reason": "OK",
         "headers": {"content-type": "application/json"},
         "body": [b'{"msg":', b" 4", b"2}"],
     }
     expected_headers = HTTPHeaderDict({"content-type": "application/json"})
 
     response_replay = HTTPResponseReplay(recorded_response)
-    with pytest.raises(ValueError):
-        response_replay.raw  # pylint: disable=pointless-statement
+    with pytest.raises(
+        ValueError,
+        match=re.escape("The 'raw' attribute is not available with the replay engine"),
+    ):
+        response_replay.raw  # pylint: disable=pointless-statement  # noqa: B018
     assert response_replay.status_code == 200
     assert response_replay.reason == "OK"
     assert response_replay.headers == expected_headers
 
     response_replay = HTTPResponseReplay(recorded_response)
     data_stream = response_replay.data_stream
     assert next(data_stream) == b'{"msg":'
@@ -41,21 +45,31 @@
     assert next(response_replay.data_stream) == b'{"msg":'
     assert next(response_replay.data_stream) == b" 4"
     assert next(response_replay.data_stream) == b"2}"
     assert next(response_replay.data_stream, None) is None
 
     response_replay = HTTPResponseReplay(recorded_response)
     assert response_replay.data_bytes == b'{"msg": 42}'
-    with pytest.raises(ValueError):
-        response_replay.data_bytes  # pylint: disable=pointless-statement
+    with pytest.raises(
+        ValueError,
+        match=re.escape(
+            "The data_xxx attributes can be only accessed once with the replay engine"
+        ),
+    ):
+        response_replay.data_bytes  # pylint: disable=pointless-statement  # noqa: B018
 
     response_replay = HTTPResponseReplay(recorded_response)
     assert response_replay.data_str == '{"msg": 42}'
-    with pytest.raises(ValueError):
-        response_replay.data_str  # pylint: disable=pointless-statement
+    with pytest.raises(
+        ValueError,
+        match=re.escape(
+            "The data_xxx attributes can be only accessed once with the replay engine"
+        ),
+    ):
+        response_replay.data_str  # pylint: disable=pointless-statement  # noqa: B018
 
     response_replay = HTTPResponseReplay(recorded_response)
     assert response_replay.data_json == {"msg": 42}
     assert response_replay.data_json == {"msg": 42}
 
     # modify headers
     response_replay = HTTPResponseReplay(recorded_response)
@@ -138,66 +152,83 @@
     )
     for response in [engine(request), engine(replace(request, stream_response=True))]:
         assert response.status_code == 200
         assert response.reason == "OK"
         assert response.headers == HTTPHeaderDict({"server": "nginx"})
         assert response.data_json == {"msg": 42}
 
-    with pytest.raises(ValueError) as excinfo:
+    with pytest.raises(
+        ValueError,
+        match=re.escape(
+            "No response have been recorded for request: {"
+            "'method': 'HEAD', "
+            "'url': 'https://example.com/', "
+            "'headers': {}, "
+            "'body': b''}"
+        ),
+    ):
         engine(replace(request, method="HEAD"))
-    assert str(excinfo.value) == (
-        "No response have been recorded for request: {"
-        "'method': 'HEAD', "
-        "'url': 'https://example.com/', "
-        "'headers': {}, "
-        "'body': b''}"
-    )
 
-    with pytest.raises(ValueError) as excinfo:
+    with pytest.raises(
+        ValueError,
+        match=re.escape(
+            "No response have been recorded for request: {"
+            "'method': 'GET', "
+            "'url': 'https://example.com/foobar', "
+            "'headers': {}, "
+            "'body': b''}"
+        ),
+    ):
         engine(replace(request, url="https://example.com/foobar"))
-    assert str(excinfo.value) == (
-        "No response have been recorded for request: {"
-        "'method': 'GET', "
-        "'url': 'https://example.com/foobar', "
-        "'headers': {}, "
-        "'body': b''}"
-    )
 
-    with pytest.raises(ValueError) as excinfo:
+    with pytest.raises(
+        ValueError,
+        match=re.escape(
+            "No response have been recorded for request: {"
+            "'method': 'GET', "
+            "'url': 'https://example.com/', "
+            "'headers': {'foo': 'bar'}, "
+            "'body': b''}"
+        ),
+    ):
         engine(replace(request, headers=HTTPHeaderDict({"foo": "bar"})))
-    assert str(excinfo.value) == (
-        "No response have been recorded for request: {"
-        "'method': 'GET', "
-        "'url': 'https://example.com/', "
-        "'headers': {'foo': 'bar'}, "
-        "'body': b''}"
-    )
 
-    with pytest.raises(ValueError) as excinfo:
+    with pytest.raises(
+        ValueError,
+        match=re.escape(
+            "No response have been recorded for request: {"
+            "'method': 'GET', "
+            "'url': 'https://example.com/', "
+            "'headers': {}, "
+            "'body': b'foobar'}"
+        ),
+    ):
         engine(replace(request, body=b"foobar"))
-    assert str(excinfo.value) == (
-        "No response have been recorded for request: {"
-        "'method': 'GET', "
-        "'url': 'https://example.com/', "
-        "'headers': {}, "
-        "'body': b'foobar'}"
-    )
 
 
 @pytest.mark.parametrize("url_end", ["wrong_ext", "in_subfolder"])
 def test_replay_miss(url_end: str) -> None:
     engine = HTTPEngineReplay([REPLAY_PATH / "base"])
     request = HTTPRequest(
         method="GET",
         url=f"https://example.com/{url_end}",
         headers=HTTPHeaderDict(),
         body=b"",
         stream_response=False,
     )
-    with pytest.raises(ValueError):
+    with pytest.raises(
+        ValueError,
+        match=re.escape(
+            "No response have been recorded for request: {"
+            "'method': 'GET', "
+            f"'url': 'https://example.com/{url_end}', "
+            "'headers': {}, "
+            "'body': b''}"
+        ),
+    ):
         engine(request)
 
 
 def test_replay_multiple_paths() -> None:
     engine = HTTPEngineReplay([REPLAY_PATH / "base", REPLAY_PATH / "extra"])
     request = HTTPRequest(
         method="GET",
@@ -216,15 +247,24 @@
     assert response.data_json == {"msg": 13}
 
     # in both base and extra: keep extra
     response = engine(replace(request, url="https://example.com/foo"))
     assert response.data_json == {"msg": 37}
 
     # in none
-    with pytest.raises(ValueError):
+    with pytest.raises(
+        ValueError,
+        match=re.escape(
+            "No response have been recorded for request: {"
+            "'method': 'GET', "
+            "'url': 'https://example.com/miss', "
+            "'headers': {}, "
+            "'body': b''}"
+        ),
+    ):
         engine(replace(request, url="https://example.com/miss"))
 
 
 def test_replay_encoding() -> None:
     data = bytes(range(256))
     engine = HTTPEngineReplay([REPLAY_PATH / "base"])
     request = HTTPRequest(
```

### Comparing `sdkite-0.3.0/tests/unit/http/test_engine_replay_recording.py` & `sdkite-0.4.0/tests/unit/http/test_engine_replay_recording.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from pathlib import Path
+import re
 import time
 from typing import Set
 
 import pytest
 from requests_mock import Mocker, NoMockAddress
 
 from sdkite.http import HTTPHeaderDict, HTTPRequest
 from sdkite.http.engine_replay import HTTPEngineReplay, HTTPResponseReplay
 
 REPLAY_PATH = Path(__file__).parent / "engine_replay"
 
 
 @pytest.fixture(autouse=True)
-def patched_time(monkeypatch: pytest.MonkeyPatch) -> None:
+def _patched_time(monkeypatch: pytest.MonkeyPatch) -> None:
     def mocked_time() -> int:
         return 1234567890
 
     monkeypatch.setattr(time, "time", mocked_time)
 
 
 def list_files(src: Path) -> Set[Path]:
@@ -140,15 +141,18 @@
     request = HTTPRequest(
         method="GET",
         url="https://example.com/",
         headers=HTTPHeaderDict(),
         body=b"",
         stream_response=False,
     )
-    with pytest.raises(NoMockAddress):
+    with pytest.raises(
+        NoMockAddress,
+        match=re.escape("No mock address: GET https://example.com/"),
+    ):
         response = engine(request)
 
 
 @pytest.mark.parametrize("recording", [True, False])
 def test_recording_modifiers(
     tmp_path: Path, requests_mock: Mocker, recording: bool
 ) -> None:
```

### Comparing `sdkite-0.3.0/tests/unit/http/test_engine_requests.py` & `sdkite-0.4.0/tests/unit/http/test_engine_requests.py`

 * *Files identical despite different names*

### Comparing `sdkite-0.3.0/tests/unit/http/test_model_httpheaderdict.py` & `sdkite-0.4.0/tests/unit/http/test_model_httpheaderdict.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import re
 from typing import Dict, List, Tuple, Union
 
 import pytest
 
 from sdkite.http import HTTPHeaderDict
 
 keys_cases = {
@@ -17,17 +18,16 @@
 )
 def test_getitem(key: str) -> None:
     value = "aBc01!$"
     hdict = HTTPHeaderDict()
     assert repr(hdict) == r"HTTPHeaderDict{}"
 
     for key2 in keys_cases.values():
-        with pytest.raises(KeyError) as exc_info:
+        with pytest.raises(KeyError, match=re.escape(f"'{key2}'")):
             hdict[key2]  # pylint: disable=pointless-statement
-        assert exc_info.value.args == (key2,)
 
     hdict[key] = value
     assert repr(hdict) == f"HTTPHeaderDict{{'{key}': ['{value}']}}"
 
     for key2 in keys_cases.values():
         assert key2 in hdict
         assert hdict[key2] == value
```

### Comparing `sdkite-0.3.0/tests/unit/http/test_utils_encode_request_body.py` & `sdkite-0.4.0/tests/unit/http/test_utils_encode_request_body.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from dataclasses import dataclass
+import re
 import secrets
 from typing import Dict, List, Optional, Tuple, Union
 
 import pytest
 
 from sdkite.http import HTTPBodyEncoding
 from sdkite.http.utils import encode_request_body
 
 
 @pytest.fixture(autouse=True)
-def patched_adapter(monkeypatch: pytest.MonkeyPatch) -> None:
+def _patched_adapter(monkeypatch: pytest.MonkeyPatch) -> None:
     monkeypatch.setattr(secrets, "token_hex", lambda size: "0" * size)
 
 
 @dataclass
 class Ok:
     data: Optional[bytes]
     content_type: Optional[str] = None
@@ -332,15 +333,15 @@
             HTTPBodyEncoding.MULTIPART: Ko("CustomClass"),
         },
     ),
 ]
 
 
 @pytest.mark.parametrize(
-    "body, encoding, expected",
+    ["body", "encoding", "expected"],
     [
         pytest.param(
             body,
             encoding,
             value,
             id=f"{encoding.name}-{name}",
         )
@@ -358,17 +359,18 @@
         assert isinstance(data, bytes) != expected.is_iterator
         if not isinstance(data, bytes):
             data = b"".join(data)
         assert data == expected.data, "Invalid data"
         assert content_type == expected.content_type, "Invalid content type"
 
     else:
-        with pytest.raises(TypeError) as excinfo:
+        with pytest.raises(
+            TypeError, match=re.escape(expected.msg(encoding))
+        ) as excinfo:
             encode_request_body(body, encoding)
 
         assert excinfo.type is TypeError
-        assert str(excinfo.value) == expected.msg(encoding)
 
 
 def test_invalid_encoding_type() -> None:
     with pytest.raises(TypeError):
         encode_request_body(None, "oops")  # type: ignore[arg-type]
```

### Comparing `sdkite-0.3.0/tests/unit/http/test_utils_url.py` & `sdkite-0.4.0/tests/unit/http/test_utils_url.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import pytest
 
 from sdkite.http.utils import urljoin, urlsjoin
 
 
 @pytest.mark.parametrize(
-    "base, url, expected",
+    ["base", "url", "expected"],
     [
         (None, None, None),
         ("", "", None),
         ("https://perdu.com", None, "https://perdu.com"),
         ("https://perdu.com/", None, "https://perdu.com/"),
         ("https://perdu.com", "", "https://perdu.com"),
         ("https://perdu.com/", "", "https://perdu.com/"),
@@ -33,15 +33,15 @@
 def test_urljoin(
     base: Optional[str], url: Optional[str], expected: Optional[str]
 ) -> None:
     assert urljoin(base, url) == expected
 
 
 @pytest.mark.parametrize(
-    "urls, expected",
+    ["urls", "expected"],
     [
         (
             [],
             None,
         ),
         (
             [None, None, None],
```

### Comparing `sdkite-0.3.0/tests/unit/test_adapter.py` & `sdkite-0.4.0/tests/unit/test_adapter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import TYPE_CHECKING, Any, List, cast
+import re
+from typing import TYPE_CHECKING, Any, List, Optional, Tuple, cast
 
 import pytest
 
 from sdkite import Adapter, AdapterSpec
 
 if TYPE_CHECKING:
     from sdkite import Client
@@ -43,30 +44,31 @@
 
     client0 = ClientSimple0()
     client1 = ClientSimple1()
     client1._parent = client0  # pylint: disable=protected-access
 
     # different order of adp instantiation
     if swap_order:
-        client1.adp  # pylint: disable=pointless-statement
-        client0.adp  # pylint: disable=pointless-statement
+        client1.adp  # pylint: disable=pointless-statement  # noqa: B018
+        client0.adp  # pylint: disable=pointless-statement  # noqa: B018
     else:
-        client0.adp  # pylint: disable=pointless-statement
-        client1.adp  # pylint: disable=pointless-statement
+        client0.adp  # pylint: disable=pointless-statement  # noqa: B018
+        client1.adp  # pylint: disable=pointless-statement  # noqa: B018
 
     assert isinstance(client0.adp, AdapterSimple)
     assert isinstance(client1.adp, AdapterSimple)
     assert client0.adp is client1.adp
 
 
 class AdapterComplex(Adapter):
     """A complex adapter"""
 
     uvw: List[int]
     xyz: List[str]
+    ijk: Optional[str]
 
     no_instance = True
 
     def __init__(self) -> None:
         assert AdapterComplex.no_instance
         AdapterComplex.no_instance = False
         self.var = True
@@ -77,23 +79,27 @@
     def get_client_names(self) -> List[str]:
         return [client.__class__.__name__ for client in self._clients]
 
     def get_adp_attrs(self) -> List[List[str]]:
         assert self._adapters[-1] == self
         return [adp.xyz for adp in self._adapters]
 
+    def get_adp_hierarchy(self, *args: Optional[str]) -> Tuple[Optional[str], ...]:
+        return self._from_adapter_hierarchy("ijk", *args)
+
     def __repr__(self) -> str:
         return f"AC<{self.uvw},{self.xyz}>"
 
 
 class AdapterSpecComplex(AdapterSpec[AdapterComplex]):
     uvw = [42]
 
     def __init__(self, *xyz: str) -> None:
         self.xyz = list(xyz)
+        self.ijk = self.xyz[1] if len(self.xyz) > 1 else None
 
     def _create_adapter(self) -> AdapterComplex:
         return AdapterComplex()
 
 
 class ClientComplex0(Client):
     _parent: Any = None
@@ -118,19 +124,19 @@
 
     client0 = ClientComplex0()
     client1 = ClientComplex1()
     client1._parent = client0  # pylint: disable=protected-access
 
     # different order of adp instantiation
     if swap_order:
-        client1.adp  # pylint: disable=pointless-statement
-        client0.adp  # pylint: disable=pointless-statement
+        client1.adp  # pylint: disable=pointless-statement  # noqa: B018
+        client0.adp  # pylint: disable=pointless-statement  # noqa: B018
     else:
-        client0.adp  # pylint: disable=pointless-statement
-        client1.adp  # pylint: disable=pointless-statement
+        client0.adp  # pylint: disable=pointless-statement  # noqa: B018
+        client1.adp  # pylint: disable=pointless-statement  # noqa: B018
 
     assert isinstance(client0.adp, AdapterComplex)
     assert isinstance(client1.adp, AdapterComplex)
 
     assert client0.adp.__doc__ == "A complex adapter"
     assert repr(client0.adp) == "AC<[42],['13', '37']>"
 
@@ -162,17 +168,29 @@
 
     assert client0.adp.get_attr_name() == "adp"
     assert client1.adp.get_attr_name() == "adp"
     assert client0.adp.get_client_names() == ["ClientComplex0"]
     assert client1.adp.get_client_names() == ["ClientComplex0", "ClientComplex1"]
     assert client0.adp.get_adp_attrs() == [["13", "37", "end"]]
     assert client1.adp.get_adp_attrs() == [["13", "37", "end"], ["42"]]
+    assert client0.adp.get_adp_hierarchy() == ("37",)
+    assert client1.adp.get_adp_hierarchy() == ("37", None)
+    assert client1.adp.get_adp_hierarchy("4", None, "2") == ("37", None, "4", None, "2")
 
     assert client0bis.adp.get_adp_attrs() == [["13", "37"]]
     assert client1bis.adp.get_adp_attrs() == [["13", "37"], ["42"]]
+    assert client0bis.adp.get_adp_hierarchy() == ("37",)
+    assert client1bis.adp.get_adp_hierarchy() == ("37", None)
+    assert client1bis.adp.get_adp_hierarchy("4", None, "2") == (
+        "37",
+        None,
+        "4",
+        None,
+        "2",
+    )
 
 
 class ClientNoAdapter(Client):
     _parent: Any = None
 
 
 def test_client_middle_no_adapter() -> None:
@@ -180,19 +198,20 @@
 
     client0 = ClientComplex0()
     client1 = ClientNoAdapter()
     client1._parent = client0  # pylint: disable=protected-access
     client2 = ClientComplex1()
     client2._parent = client1  # pylint: disable=protected-access
 
-    client0.adp  # pylint: disable=pointless-statement
-    with pytest.raises(TypeError) as excinfo:
-        client2.adp  # pylint: disable=pointless-statement
-
-    assert str(excinfo.value) == "Client 'ClientComplex1' is missing adapter spec 'adp'"
+    client0.adp  # pylint: disable=pointless-statement  # noqa: B018
+    with pytest.raises(
+        TypeError,
+        match=re.escape("Client 'ClientComplex1' is missing adapter spec 'adp'"),
+    ):
+        client2.adp  # pylint: disable=pointless-statement  # noqa: B018
 
 
 class ClientMixed1(Client):
     _parent: Any = None
     adp = AdapterSpecComplex("37")
 
 
@@ -200,15 +219,16 @@
     AdapterSimple.no_instance = True
     AdapterComplex.no_instance = True
 
     client0 = ClientSimple0()
     client1 = ClientMixed1()
     client1._parent = client0  # pylint: disable=protected-access
 
-    client0.adp  # pylint: disable=pointless-statement
-    with pytest.raises(TypeError) as excinfo:
-        client1.adp  # pylint: disable=pointless-statement
-
-    assert str(excinfo.value) == (
-        "Client 'ClientMixed1' has a wrong adapter spec: got 'AdapterSpecComplex' "
-        "instead of 'AdapterSpecSimple'"
-    )
+    client0.adp  # pylint: disable=pointless-statement  # noqa: B018
+    with pytest.raises(
+        TypeError,
+        match=re.escape(
+            "Client 'ClientMixed1' has a wrong adapter spec: got 'AdapterSpecComplex' "
+            "instead of 'AdapterSpecSimple'"
+        ),
+    ):
+        client1.adp  # pylint: disable=pointless-statement  # noqa: B018
```

### Comparing `sdkite-0.3.0/tests/unit/test_client.py` & `sdkite-0.4.0/tests/unit/test_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 
 def test_subclients() -> None:
     client = ClientC()
 
     assert client.var_a == 42
     with pytest.raises(AttributeError):
-        client.var_b  # pylint: disable=pointless-statement
+        client.var_b  # pylint: disable=pointless-statement  # noqa: B018
     assert isinstance(client, ClientC)
 
     assert isinstance(client.var_c, ClientA)
     assert isinstance(client.var_d, ClientA)
     assert isinstance(client.var_e, ClientB)
 
     assert isinstance(client.var_e.xyz, ClientA)
```

### Comparing `sdkite-0.3.0/tests/unit/test_pagination.py` & `sdkite-0.4.0/tests/unit/test_pagination.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from binascii import crc32
 from inspect import Parameter, signature
+import re
 import sys
-from typing import TYPE_CHECKING, Any, List, Optional, Union, cast, get_type_hints
+from typing import Any, List, Optional, Union, cast, get_type_hints
 from unittest.mock import Mock, call
 
 import pytest
 
 from sdkite import Pagination, paginated
 
 if sys.version_info < (3, 8):  # pragma: no cover
@@ -14,21 +15,18 @@
     from typing import Protocol
 
 if sys.version_info < (3, 9):  # pragma: no cover
     from typing import Iterable, Iterator
 else:  # pragma: no cover
     from collections.abc import Iterable, Iterator
 
-
-if TYPE_CHECKING:
+if sys.version_info < (3, 11):  # pragma: no cover
     from typing_extensions import assert_type
-else:
-    # no need to have typing_extensions installed
-    def assert_type(val: Any, _: Any) -> Any:
-        return val
+else:  # pragma: no cover
+    from typing import assert_type
 
 
 def test_paginated_page() -> None:
     mock_range = Mock(side_effect=range)
 
     @paginated()
     def fct(pagination: Pagination) -> Iterable[int]:
@@ -72,15 +70,14 @@
     ]
 
 
 def test_paginated_offset_during_iteration() -> None:
     @paginated()
     def fct(pagination: Pagination) -> Iterable[int]:
         for _ in range(10):
-            print(pagination.offset)
             yield pagination.offset
             if pagination.offset == 42:
                 pagination.finish()
                 break
 
     assert list(fct()) == list(range(42))
 
@@ -109,15 +106,15 @@
         "d21ba58f",
         "131d3482",
         "cf8a06b5",
         "0e995f9f",
     ]
 
 
-@pytest.mark.parametrize("stop_when_empty", (None, True, False))
+@pytest.mark.parametrize("stop_when_empty", [None, True, False])
 def test_paginated_stop_when_empty(stop_when_empty: Optional[bool]) -> None:
     mock_range = Mock(side_effect=range)
     sizes = [30, 10, 20, 0, 40, 50]
 
     if stop_when_empty is None:
         decorator = paginated()
     else:
@@ -130,15 +127,15 @@
             stop = start + sizes[pagination.page]
         except IndexError:
             pagination.finish()
             return []
         return cast(range, mock_range(start, stop))
 
     # contrary to 'paginated', 'decorator' is not in pylint's 'signature-mutators'
-    # pylint: disable-next=no-value-for-parameter
+    # pylint: disable-next=no-value-for-parameter
     return_value = fct()
 
     if stop_when_empty is False:
         assert list(return_value) == list(range(150))
         assert mock_range.call_args_list == [
             call(0, 30),
             call(30, 40),
@@ -466,90 +463,88 @@
     def fct(pagination: Pagination) -> Union[Iterable[int], int]:
         if pagination.page < 10:
             return [pagination.page]
         return 42
 
     output = fct()
 
-    with pytest.raises(TypeError) as excinfo:
+    with pytest.raises(TypeError, match=re.escape("'int' object is not iterable")):
         list(output)
 
-    assert str(excinfo.value) == "'int' object is not iterable"
-
 
 def test_paginated_no_param() -> None:
-    with pytest.raises(TypeError) as excinfo:
+    with pytest.raises(
+        TypeError,
+        match=re.escape(
+            "Paginated function 'fct' must have 'pagination' as first parameter"
+        ),
+    ):
 
         @paginated()  # type: ignore[arg-type]
         def fct() -> Iterable[int]:
             yield 42
 
-    assert (
-        str(excinfo.value)
-        == "Paginated function 'fct' must have 'pagination' as first parameter"
-    )
-
 
 def test_paginated_wrong_param_name() -> None:
-    with pytest.raises(TypeError) as excinfo:
+    with pytest.raises(
+        TypeError,
+        match=re.escape(
+            "Paginated function 'fct' must have 'pagination' as first parameter"
+        ),
+    ):
 
         @paginated()
         def fct(
             # pylint: disable=unused-argument
-            param0: Pagination,
-            param1: int,
+            param0: Pagination,  # noqa: ARG001
+            param1: int,  # noqa: ARG001
         ) -> Iterable[int]:
             yield 42
 
-    assert (
-        str(excinfo.value)
-        == "Paginated function 'fct' must have 'pagination' as first parameter"
-    )
-
 
 def test_paginated_wrong_param_kind() -> None:
-    with pytest.raises(TypeError) as excinfo:
+    with pytest.raises(
+        TypeError,
+        match=re.escape(
+            "Paginated function 'fct' must have 'pagination' as first parameter"
+        ),
+    ):
 
         @paginated()  # type: ignore[arg-type]
         def fct(
             # pylint: disable=unused-argument
             *,
-            pagination: Pagination,
+            pagination: Pagination,  # noqa: ARG001
         ) -> Iterable[int]:
             yield 42
 
-    assert (
-        str(excinfo.value)
-        == "Paginated function 'fct' must have 'pagination' as first parameter"
-    )
-
 
 def test_paginated_called_with_pagination_param() -> None:
     @paginated()
     def fct(
         # pylint: disable=unused-argument
         pagination: Pagination,
-        *args: int,
-        **kwargs: int,
+        *args: int,  # noqa: ARG001
+        **kwargs: int,  # noqa: ARG001
     ) -> Iterable[int]:
         if pagination.page == 0:
             yield 42
 
     assert list(fct(13, param=37)) == [42]
 
-    with pytest.raises(TypeError) as excinfo:
+    with pytest.raises(
+        TypeError,
+        match=re.escape(
+            "Paginated function 'fct' cannot be called with a 'pagination' parameter"
+        ),
+    ):
         list(fct(13, pagination=37))
 
-    assert (
-        str(excinfo.value)
-        == "Paginated function 'fct' cannot be called with a 'pagination' parameter"
-    )
-
 
 def test_paginated_no_type_hint() -> None:
     @paginated()
-    def fct(pagination):  # type: ignore
+    def fct(pagination):  # type: ignore[no-untyped-def,misc]  # noqa: ANN001,ANN202
         if pagination.page == 4:
             pagination.finish()
         return range(pagination.offset, pagination.offset + 10)
 
     assert list(fct()) == list(range(50))
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `sdkite-0.3.0/tests/unit/test_pagination_pep570.py` & `sdkite-0.4.0/tests/unit/test_pagination_pep570.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 # this file requires Python 3.8
 
 from inspect import Parameter, signature
 import sys
-from typing import TYPE_CHECKING, Any, List, Protocol, get_type_hints
+from typing import Any, List, Protocol, get_type_hints
 
 from sdkite import Pagination, paginated
 
 if sys.version_info < (3, 9):  # pragma: no cover
     from typing import Iterator
 else:  # pragma: no cover
     from collections.abc import Iterator
 
-
-if TYPE_CHECKING:
+if sys.version_info < (3, 11):  # pragma: no cover
     from typing_extensions import assert_type
-else:
-    # no need to have typing_extensions installed
-    def assert_type(val: Any, _: Any) -> Any:
-        return val
+else:  # pragma: no cover
+    from typing import assert_type
 
 
 # this file uses positional-only parameters (PEP 570)
 # which is only supported from Python 3.8
 
 # this needs to be merged with regular test file
 # when support for Python 3.7 is dropped
```

### Comparing `sdkite-0.3.0/tox.ini` & `sdkite-0.4.0/tox.ini`

 * *Files 14% similar despite different names*

```diff
@@ -27,24 +27,24 @@
     mypy --explicit-package-bases docs tests
 
 [testenv:lint]
 deps =
     pylint
     pytest # to avoid import errors
     requests_mock
+    ruff==0.0.261
 commands =
+    ruff src docs tests
     pylint src
     pylint -d duplicate-code,too-many-statements docs tests
 
 [testenv:format]
 skip_install = true
 deps =
     black
-    isort
 commands =
     black {posargs:--check --diff} docs src tests
-    isort {posargs:--check --diff} docs src tests
 
 [testenv:docs]
 skip_install = true
 deps = mkdocs
 commands = mkdocs {posargs:build} -f docs/mkdocs.yml
```

