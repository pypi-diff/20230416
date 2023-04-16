# Comparing `tmp/py_ocpi-0.3.0.tar.gz` & `tmp/py_ocpi-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_ocpi-0.3.0.tar", max compression
+gzip compressed data, was "py_ocpi-0.3.1.tar", max compression
```

## Comparing `py_ocpi-0.3.0.tar` & `py_ocpi-0.3.1.tar`

### file list

```diff
@@ -1,72 +1,71 @@
--rw-r--r--   0        0        0     1086 2022-12-20 07:05:04.548821 py_ocpi-0.3.0/LICENSE
--rw-r--r--   0        0        0     1546 2022-12-20 07:05:04.548821 py_ocpi-0.3.0/README.rst
--rw-r--r--   0        0        0      130 2022-12-20 07:05:04.548821 py_ocpi-0.3.0/py_ocpi/__init__.py
--rw-r--r--   0        0        0        0 2022-12-20 07:05:04.548821 py_ocpi-0.3.0/py_ocpi/core/__init__.py
--rw-r--r--   0        0        0     4165 2022-12-20 07:05:04.548821 py_ocpi-0.3.0/py_ocpi/core/adapter.py
--rw-r--r--   0        0        0      805 2022-12-20 07:05:04.548821 py_ocpi-0.3.0/py_ocpi/core/config.py
--rw-r--r--   0        0        0     4667 2022-12-20 07:05:04.548821 py_ocpi-0.3.0/py_ocpi/core/crud.py
--rw-r--r--   0        0        0     5767 2022-12-20 07:05:04.548821 py_ocpi-0.3.0/py_ocpi/core/data_types.py
--rw-r--r--   0        0        0      958 2022-12-20 07:05:04.548821 py_ocpi-0.3.0/py_ocpi/core/dependencies.py
--rw-r--r--   0        0        0     4072 2022-12-20 07:05:04.548821 py_ocpi-0.3.0/py_ocpi/core/endpoints.py
--rw-r--r--   0        0        0     1339 2022-12-20 07:05:04.548821 py_ocpi-0.3.0/py_ocpi/core/enums.py
--rw-r--r--   0        0        0      278 2022-12-20 07:05:04.548821 py_ocpi-0.3.0/py_ocpi/core/exceptions.py
--rw-r--r--   0        0        0     5043 2022-12-20 07:05:04.548821 py_ocpi-0.3.0/py_ocpi/core/push.py
--rw-r--r--   0        0        0      814 2022-12-20 07:05:04.548821 py_ocpi-0.3.0/py_ocpi/core/schemas.py
--rw-r--r--   0        0        0     1834 2022-12-20 07:05:04.548821 py_ocpi-0.3.0/py_ocpi/core/status.py
--rw-r--r--   0        0        0     1450 2022-12-20 07:05:04.548821 py_ocpi-0.3.0/py_ocpi/core/utils.py
--rw-r--r--   0        0        0     4254 2022-12-20 07:05:04.548821 py_ocpi-0.3.0/py_ocpi/main.py
--rw-r--r--   0        0        0        0 2022-12-20 07:05:04.548821 py_ocpi-0.3.0/py_ocpi/modules/__init__.py
--rw-r--r--   0        0        0        0 2022-12-20 07:05:04.548821 py_ocpi-0.3.0/py_ocpi/modules/cdrs/__init__.py
--rw-r--r--   0        0        0       78 2022-12-20 07:05:04.548821 py_ocpi-0.3.0/py_ocpi/modules/cdrs/v_2_2_1/api/__init__.py
--rw-r--r--   0        0        0     1197 2022-12-20 07:05:04.548821 py_ocpi-0.3.0/py_ocpi/modules/cdrs/v_2_2_1/api/cpo.py
--rw-r--r--   0        0        0     1906 2022-12-20 07:05:04.548821 py_ocpi-0.3.0/py_ocpi/modules/cdrs/v_2_2_1/api/emsp.py
--rw-r--r--   0        0        0     2675 2022-12-20 07:05:04.548821 py_ocpi-0.3.0/py_ocpi/modules/cdrs/v_2_2_1/enums.py
--rw-r--r--   0        0        0     3360 2022-12-20 07:05:04.548821 py_ocpi-0.3.0/py_ocpi/modules/cdrs/v_2_2_1/schemas.py
--rw-r--r--   0        0        0        0 2022-12-20 07:05:04.548821 py_ocpi-0.3.0/py_ocpi/modules/commands/__init__.py
--rw-r--r--   0        0        0       78 2022-12-20 07:05:04.548821 py_ocpi-0.3.0/py_ocpi/modules/commands/v_2_2_1/api/__init__.py
--rw-r--r--   0        0        0     4291 2022-12-20 07:05:04.548821 py_ocpi-0.3.0/py_ocpi/modules/commands/v_2_2_1/api/cpo.py
--rw-r--r--   0        0        0     1082 2022-12-20 07:05:04.548821 py_ocpi-0.3.0/py_ocpi/modules/commands/v_2_2_1/api/emsp.py
--rw-r--r--   0        0        0     2443 2022-12-20 07:05:04.548821 py_ocpi-0.3.0/py_ocpi/modules/commands/v_2_2_1/enums.py
--rw-r--r--   0        0        0     2060 2022-12-20 07:05:04.548821 py_ocpi-0.3.0/py_ocpi/modules/commands/v_2_2_1/schemas.py
--rw-r--r--   0        0        0        0 2022-12-20 07:05:04.548821 py_ocpi-0.3.0/py_ocpi/modules/credentials/__init__.py
--rw-r--r--   0        0        0       78 2022-12-20 07:05:04.548821 py_ocpi-0.3.0/py_ocpi/modules/credentials/v_2_2_1/api/__init__.py
--rw-r--r--   0        0        0     7137 2022-12-20 07:05:04.548821 py_ocpi-0.3.0/py_ocpi/modules/credentials/v_2_2_1/api/cpo.py
--rw-r--r--   0        0        0     7173 2022-12-20 07:05:04.548821 py_ocpi-0.3.0/py_ocpi/modules/credentials/v_2_2_1/api/emsp.py
--rw-r--r--   0        0        0        0 2022-12-20 07:05:04.548821 py_ocpi-0.3.0/py_ocpi/modules/credentials/v_2_2_1/enums.py
--rw-r--r--   0        0        0      684 2022-12-20 07:05:04.548821 py_ocpi-0.3.0/py_ocpi/modules/credentials/v_2_2_1/schemas.py
--rw-r--r--   0        0        0        0 2022-12-20 07:05:04.552821 py_ocpi-0.3.0/py_ocpi/modules/locations/__init__.py
--rw-r--r--   0        0        0       78 2022-12-20 07:05:04.552821 py_ocpi-0.3.0/py_ocpi/modules/locations/v_2_2_1/api/__init__.py
--rw-r--r--   0        0        0     3433 2022-12-20 07:05:04.552821 py_ocpi-0.3.0/py_ocpi/modules/locations/v_2_2_1/api/cpo.py
--rw-r--r--   0        0        0    11596 2022-12-20 07:05:04.552821 py_ocpi-0.3.0/py_ocpi/modules/locations/v_2_2_1/api/emsp.py
--rw-r--r--   0        0        0    11811 2022-12-20 07:05:04.552821 py_ocpi-0.3.0/py_ocpi/modules/locations/v_2_2_1/enums.py
--rw-r--r--   0        0        0     7869 2022-12-20 07:05:04.552821 py_ocpi-0.3.0/py_ocpi/modules/locations/v_2_2_1/schemas.py
--rw-r--r--   0        0        0        0 2022-12-20 07:05:04.552821 py_ocpi-0.3.0/py_ocpi/modules/sessions/__init__.py
--rw-r--r--   0        0        0       78 2022-12-20 07:05:04.552821 py_ocpi-0.3.0/py_ocpi/modules/sessions/v_2_2_1/api/__init__.py
--rw-r--r--   0        0        0     2142 2022-12-20 07:05:04.552821 py_ocpi-0.3.0/py_ocpi/modules/sessions/v_2_2_1/api/cpo.py
--rw-r--r--   0        0        0     3793 2022-12-20 07:05:04.552821 py_ocpi-0.3.0/py_ocpi/modules/sessions/v_2_2_1/api/emsp.py
--rw-r--r--   0        0        0     2488 2022-12-20 07:05:04.552821 py_ocpi-0.3.0/py_ocpi/modules/sessions/v_2_2_1/enums.py
--rw-r--r--   0        0        0     2146 2022-12-20 07:05:04.552821 py_ocpi-0.3.0/py_ocpi/modules/sessions/v_2_2_1/schemas.py
--rw-r--r--   0        0        0        0 2022-12-20 07:05:04.552821 py_ocpi-0.3.0/py_ocpi/modules/tariffs/__init__.py
--rw-r--r--   0        0        0       78 2022-12-20 07:05:04.552821 py_ocpi-0.3.0/py_ocpi/modules/tariffs/v_2_2_1/api/__init__.py
--rw-r--r--   0        0        0     1230 2022-12-20 07:05:04.552821 py_ocpi-0.3.0/py_ocpi/modules/tariffs/v_2_2_1/api/cpo.py
--rw-r--r--   0        0        0     3163 2022-12-20 07:05:04.552821 py_ocpi-0.3.0/py_ocpi/modules/tariffs/v_2_2_1/api/emsp.py
--rw-r--r--   0        0        0     2321 2022-12-20 07:05:04.552821 py_ocpi-0.3.0/py_ocpi/modules/tariffs/v_2_2_1/enums.py
--rw-r--r--   0        0        0     2023 2022-12-20 07:05:04.552821 py_ocpi-0.3.0/py_ocpi/modules/tariffs/v_2_2_1/schemas.py
--rw-r--r--   0        0        0        0 2022-12-20 07:05:04.552821 py_ocpi-0.3.0/py_ocpi/modules/tokens/__init__.py
--rw-r--r--   0        0        0       78 2022-12-20 07:05:04.552821 py_ocpi-0.3.0/py_ocpi/modules/tokens/v_2_2_1/api/__init__.py
--rw-r--r--   0        0        0     4128 2022-12-20 07:05:04.552821 py_ocpi-0.3.0/py_ocpi/modules/tokens/v_2_2_1/api/cpo.py
--rw-r--r--   0        0        0     3212 2022-12-20 07:05:04.552821 py_ocpi-0.3.0/py_ocpi/modules/tokens/v_2_2_1/api/emsp.py
--rw-r--r--   0        0        0     1367 2022-12-20 07:05:04.552821 py_ocpi-0.3.0/py_ocpi/modules/tokens/v_2_2_1/enums.py
--rw-r--r--   0        0        0     2139 2022-12-20 07:05:04.552821 py_ocpi-0.3.0/py_ocpi/modules/tokens/v_2_2_1/schemas.py
--rw-r--r--   0        0        0        0 2022-12-20 07:05:04.552821 py_ocpi-0.3.0/py_ocpi/modules/versions/__init__.py
--rw-r--r--   0        0        0       80 2022-12-20 07:05:04.552821 py_ocpi-0.3.0/py_ocpi/modules/versions/api/__init__.py
--rw-r--r--   0        0        0      423 2022-12-20 07:05:04.552821 py_ocpi-0.3.0/py_ocpi/modules/versions/api/main.py
--rw-r--r--   0        0        0      646 2022-12-20 07:05:04.552821 py_ocpi-0.3.0/py_ocpi/modules/versions/api/v_2_2_1.py
--rw-r--r--   0        0        0      817 2022-12-20 07:05:04.552821 py_ocpi-0.3.0/py_ocpi/modules/versions/enums.py
--rw-r--r--   0        0        0      790 2022-12-20 07:05:04.552821 py_ocpi-0.3.0/py_ocpi/modules/versions/schemas.py
--rw-r--r--   0        0        0      110 2022-12-20 07:05:04.552821 py_ocpi-0.3.0/py_ocpi/routers/__init__.py
--rw-r--r--   0        0        0     1054 2022-12-20 07:05:04.552821 py_ocpi-0.3.0/py_ocpi/routers/v_2_2_1/cpo.py
--rw-r--r--   0        0        0     1075 2022-12-20 07:05:04.552821 py_ocpi-0.3.0/py_ocpi/routers/v_2_2_1/emsp.py
--rw-r--r--   0        0        0      624 2022-12-20 07:05:04.552821 py_ocpi-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3173 1970-01-01 00:00:00.000000 py_ocpi-0.3.0/setup.py
--rw-r--r--   0        0        0     2180 1970-01-01 00:00:00.000000 py_ocpi-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-04-16 07:48:47.840749 py_ocpi-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1546 2023-04-16 07:48:47.840749 py_ocpi-0.3.1/README.rst
+-rw-r--r--   0        0        0      130 2023-04-16 07:48:47.840749 py_ocpi-0.3.1/py_ocpi/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-16 07:48:47.840749 py_ocpi-0.3.1/py_ocpi/core/__init__.py
+-rw-r--r--   0        0        0     4165 2023-04-16 07:48:47.840749 py_ocpi-0.3.1/py_ocpi/core/adapter.py
+-rw-r--r--   0        0        0      805 2023-04-16 07:48:47.840749 py_ocpi-0.3.1/py_ocpi/core/config.py
+-rw-r--r--   0        0        0     4667 2023-04-16 07:48:47.840749 py_ocpi-0.3.1/py_ocpi/core/crud.py
+-rw-r--r--   0        0        0     5767 2023-04-16 07:48:47.840749 py_ocpi-0.3.1/py_ocpi/core/data_types.py
+-rw-r--r--   0        0        0     1001 2023-04-16 07:48:47.840749 py_ocpi-0.3.1/py_ocpi/core/dependencies.py
+-rw-r--r--   0        0        0     4669 2023-04-16 07:48:47.840749 py_ocpi-0.3.1/py_ocpi/core/endpoints.py
+-rw-r--r--   0        0        0     1339 2023-04-16 07:48:47.840749 py_ocpi-0.3.1/py_ocpi/core/enums.py
+-rw-r--r--   0        0        0      278 2023-04-16 07:48:47.840749 py_ocpi-0.3.1/py_ocpi/core/exceptions.py
+-rw-r--r--   0        0        0     5087 2023-04-16 07:48:47.840749 py_ocpi-0.3.1/py_ocpi/core/push.py
+-rw-r--r--   0        0        0      834 2023-04-16 07:48:47.840749 py_ocpi-0.3.1/py_ocpi/core/schemas.py
+-rw-r--r--   0        0        0     1834 2023-04-16 07:48:47.840749 py_ocpi-0.3.1/py_ocpi/core/status.py
+-rw-r--r--   0        0        0     1845 2023-04-16 07:48:47.840749 py_ocpi-0.3.1/py_ocpi/core/utils.py
+-rw-r--r--   0        0        0     4481 2023-04-16 07:48:47.840749 py_ocpi-0.3.1/py_ocpi/main.py
+-rw-r--r--   0        0        0        0 2023-04-16 07:48:47.840749 py_ocpi-0.3.1/py_ocpi/modules/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-16 07:48:47.840749 py_ocpi-0.3.1/py_ocpi/modules/cdrs/__init__.py
+-rw-r--r--   0        0        0       78 2023-04-16 07:48:47.844749 py_ocpi-0.3.1/py_ocpi/modules/cdrs/v_2_2_1/api/__init__.py
+-rw-r--r--   0        0        0     1197 2023-04-16 07:48:47.844749 py_ocpi-0.3.1/py_ocpi/modules/cdrs/v_2_2_1/api/cpo.py
+-rw-r--r--   0        0        0     1906 2023-04-16 07:48:47.844749 py_ocpi-0.3.1/py_ocpi/modules/cdrs/v_2_2_1/api/emsp.py
+-rw-r--r--   0        0        0     2675 2023-04-16 07:48:47.844749 py_ocpi-0.3.1/py_ocpi/modules/cdrs/v_2_2_1/enums.py
+-rw-r--r--   0        0        0     3360 2023-04-16 07:48:47.844749 py_ocpi-0.3.1/py_ocpi/modules/cdrs/v_2_2_1/schemas.py
+-rw-r--r--   0        0        0        0 2023-04-16 07:48:47.844749 py_ocpi-0.3.1/py_ocpi/modules/commands/__init__.py
+-rw-r--r--   0        0        0       78 2023-04-16 07:48:47.844749 py_ocpi-0.3.1/py_ocpi/modules/commands/v_2_2_1/api/__init__.py
+-rw-r--r--   0        0        0     4335 2023-04-16 07:48:47.844749 py_ocpi-0.3.1/py_ocpi/modules/commands/v_2_2_1/api/cpo.py
+-rw-r--r--   0        0        0     1082 2023-04-16 07:48:47.844749 py_ocpi-0.3.1/py_ocpi/modules/commands/v_2_2_1/api/emsp.py
+-rw-r--r--   0        0        0     2443 2023-04-16 07:48:47.844749 py_ocpi-0.3.1/py_ocpi/modules/commands/v_2_2_1/enums.py
+-rw-r--r--   0        0        0     2060 2023-04-16 07:48:47.844749 py_ocpi-0.3.1/py_ocpi/modules/commands/v_2_2_1/schemas.py
+-rw-r--r--   0        0        0        0 2023-04-16 07:48:47.844749 py_ocpi-0.3.1/py_ocpi/modules/credentials/__init__.py
+-rw-r--r--   0        0        0       78 2023-04-16 07:48:47.844749 py_ocpi-0.3.1/py_ocpi/modules/credentials/v_2_2_1/api/__init__.py
+-rw-r--r--   0        0        0     7194 2023-04-16 07:48:47.844749 py_ocpi-0.3.1/py_ocpi/modules/credentials/v_2_2_1/api/cpo.py
+-rw-r--r--   0        0        0     7230 2023-04-16 07:48:47.844749 py_ocpi-0.3.1/py_ocpi/modules/credentials/v_2_2_1/api/emsp.py
+-rw-r--r--   0        0        0        0 2023-04-16 07:48:47.844749 py_ocpi-0.3.1/py_ocpi/modules/credentials/v_2_2_1/enums.py
+-rw-r--r--   0        0        0      684 2023-04-16 07:48:47.844749 py_ocpi-0.3.1/py_ocpi/modules/credentials/v_2_2_1/schemas.py
+-rw-r--r--   0        0        0        0 2023-04-16 07:48:47.844749 py_ocpi-0.3.1/py_ocpi/modules/locations/__init__.py
+-rw-r--r--   0        0        0       78 2023-04-16 07:48:47.844749 py_ocpi-0.3.1/py_ocpi/modules/locations/v_2_2_1/api/__init__.py
+-rw-r--r--   0        0        0     3433 2023-04-16 07:48:47.844749 py_ocpi-0.3.1/py_ocpi/modules/locations/v_2_2_1/api/cpo.py
+-rw-r--r--   0        0        0    11596 2023-04-16 07:48:47.844749 py_ocpi-0.3.1/py_ocpi/modules/locations/v_2_2_1/api/emsp.py
+-rw-r--r--   0        0        0    11811 2023-04-16 07:48:47.844749 py_ocpi-0.3.1/py_ocpi/modules/locations/v_2_2_1/enums.py
+-rw-r--r--   0        0        0     7869 2023-04-16 07:48:47.844749 py_ocpi-0.3.1/py_ocpi/modules/locations/v_2_2_1/schemas.py
+-rw-r--r--   0        0        0        0 2023-04-16 07:48:47.844749 py_ocpi-0.3.1/py_ocpi/modules/sessions/__init__.py
+-rw-r--r--   0        0        0       78 2023-04-16 07:48:47.844749 py_ocpi-0.3.1/py_ocpi/modules/sessions/v_2_2_1/api/__init__.py
+-rw-r--r--   0        0        0     2142 2023-04-16 07:48:47.844749 py_ocpi-0.3.1/py_ocpi/modules/sessions/v_2_2_1/api/cpo.py
+-rw-r--r--   0        0        0     3793 2023-04-16 07:48:47.844749 py_ocpi-0.3.1/py_ocpi/modules/sessions/v_2_2_1/api/emsp.py
+-rw-r--r--   0        0        0     2488 2023-04-16 07:48:47.844749 py_ocpi-0.3.1/py_ocpi/modules/sessions/v_2_2_1/enums.py
+-rw-r--r--   0        0        0     2146 2023-04-16 07:48:47.844749 py_ocpi-0.3.1/py_ocpi/modules/sessions/v_2_2_1/schemas.py
+-rw-r--r--   0        0        0        0 2023-04-16 07:48:47.844749 py_ocpi-0.3.1/py_ocpi/modules/tariffs/__init__.py
+-rw-r--r--   0        0        0       78 2023-04-16 07:48:47.844749 py_ocpi-0.3.1/py_ocpi/modules/tariffs/v_2_2_1/api/__init__.py
+-rw-r--r--   0        0        0     1230 2023-04-16 07:48:47.844749 py_ocpi-0.3.1/py_ocpi/modules/tariffs/v_2_2_1/api/cpo.py
+-rw-r--r--   0        0        0     3163 2023-04-16 07:48:47.844749 py_ocpi-0.3.1/py_ocpi/modules/tariffs/v_2_2_1/api/emsp.py
+-rw-r--r--   0        0        0     2321 2023-04-16 07:48:47.844749 py_ocpi-0.3.1/py_ocpi/modules/tariffs/v_2_2_1/enums.py
+-rw-r--r--   0        0        0     2023 2023-04-16 07:48:47.844749 py_ocpi-0.3.1/py_ocpi/modules/tariffs/v_2_2_1/schemas.py
+-rw-r--r--   0        0        0        0 2023-04-16 07:48:47.844749 py_ocpi-0.3.1/py_ocpi/modules/tokens/__init__.py
+-rw-r--r--   0        0        0       78 2023-04-16 07:48:47.844749 py_ocpi-0.3.1/py_ocpi/modules/tokens/v_2_2_1/api/__init__.py
+-rw-r--r--   0        0        0     4128 2023-04-16 07:48:47.844749 py_ocpi-0.3.1/py_ocpi/modules/tokens/v_2_2_1/api/cpo.py
+-rw-r--r--   0        0        0     3212 2023-04-16 07:48:47.844749 py_ocpi-0.3.1/py_ocpi/modules/tokens/v_2_2_1/api/emsp.py
+-rw-r--r--   0        0        0     1367 2023-04-16 07:48:47.844749 py_ocpi-0.3.1/py_ocpi/modules/tokens/v_2_2_1/enums.py
+-rw-r--r--   0        0        0     2139 2023-04-16 07:48:47.844749 py_ocpi-0.3.1/py_ocpi/modules/tokens/v_2_2_1/schemas.py
+-rw-r--r--   0        0        0        0 2023-04-16 07:48:47.844749 py_ocpi-0.3.1/py_ocpi/modules/versions/__init__.py
+-rw-r--r--   0        0        0       80 2023-04-16 07:48:47.844749 py_ocpi-0.3.1/py_ocpi/modules/versions/api/__init__.py
+-rw-r--r--   0        0        0      423 2023-04-16 07:48:47.844749 py_ocpi-0.3.1/py_ocpi/modules/versions/api/main.py
+-rw-r--r--   0        0        0     1233 2023-04-16 07:48:47.844749 py_ocpi-0.3.1/py_ocpi/modules/versions/api/v_2_2_1.py
+-rw-r--r--   0        0        0      817 2023-04-16 07:48:47.844749 py_ocpi-0.3.1/py_ocpi/modules/versions/enums.py
+-rw-r--r--   0        0        0      790 2023-04-16 07:48:47.844749 py_ocpi-0.3.1/py_ocpi/modules/versions/schemas.py
+-rw-r--r--   0        0        0      110 2023-04-16 07:48:47.844749 py_ocpi-0.3.1/py_ocpi/routers/__init__.py
+-rw-r--r--   0        0        0     1054 2023-04-16 07:48:47.844749 py_ocpi-0.3.1/py_ocpi/routers/v_2_2_1/cpo.py
+-rw-r--r--   0        0        0     1075 2023-04-16 07:48:47.844749 py_ocpi-0.3.1/py_ocpi/routers/v_2_2_1/emsp.py
+-rw-r--r--   0        0        0      624 2023-04-16 07:48:47.844749 py_ocpi-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2180 1970-01-01 00:00:00.000000 py_ocpi-0.3.1/PKG-INFO
```

### Comparing `py_ocpi-0.3.0/LICENSE` & `py_ocpi-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py_ocpi-0.3.0/README.rst` & `py_ocpi-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `py_ocpi-0.3.0/py_ocpi/core/adapter.py` & `py_ocpi-0.3.1/py_ocpi/core/adapter.py`

 * *Files identical despite different names*

### Comparing `py_ocpi-0.3.0/py_ocpi/core/config.py` & `py_ocpi-0.3.1/py_ocpi/core/config.py`

 * *Files identical despite different names*

### Comparing `py_ocpi-0.3.0/py_ocpi/core/crud.py` & `py_ocpi-0.3.1/py_ocpi/core/crud.py`

 * *Files identical despite different names*

### Comparing `py_ocpi-0.3.0/py_ocpi/core/data_types.py` & `py_ocpi-0.3.1/py_ocpi/core/data_types.py`

 * *Files identical despite different names*

### Comparing `py_ocpi-0.3.0/py_ocpi/core/dependencies.py` & `py_ocpi-0.3.1/py_ocpi/core/dependencies.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,19 +18,23 @@
     return Adapter
 
 
 def get_versions():
     return [
         Version(
             version=VersionNumber.v_2_2_1,
-            url=URL(f'https://{settings.OCPI_HOST}/{settings.OCPI_PREFIX}/{VersionNumber.v_2_2_1}/details')
+            url=URL(f'https://{settings.OCPI_HOST}/{settings.OCPI_PREFIX}/{VersionNumber.v_2_2_1.value}/details')
         ).dict(),
     ]
 
 
+def get_endpoints():
+    return {}
+
+
 def pagination_filters(
     date_from: datetime = Query(default=None),
     date_to: datetime = Query(default=datetime.now()),
     offset: int = Query(default=0),
     limit: int = Query(default=50),
 ):
     return {
```

### Comparing `py_ocpi-0.3.0/py_ocpi/core/enums.py` & `py_ocpi-0.3.1/py_ocpi/core/enums.py`

 * *Files identical despite different names*

### Comparing `py_ocpi-0.3.0/py_ocpi/core/push.py` & `py_ocpi-0.3.1/py_ocpi/core/push.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import httpx
 from fastapi import APIRouter, Request, WebSocket, Depends
 
 from py_ocpi.core.adapter import Adapter
 from py_ocpi.core.crud import Crud
 from py_ocpi.core.schemas import Push, PushResponse, ReceiverResponse
-from py_ocpi.core.utils import get_auth_token
+from py_ocpi.core.utils import encode_string_base64, get_auth_token
 from py_ocpi.core.dependencies import get_crud, get_adapter
 from py_ocpi.core.enums import ModuleID, RoleEnum
 from py_ocpi.core.config import settings
 from py_ocpi.modules.versions.enums import InterfaceRole, VersionNumber
 
 
 def client_url(module_id: ModuleID, object_id: str, base_url: str) -> str:
@@ -62,15 +62,15 @@
 
 
 async def push_object(version: VersionNumber, push: Push, crud: Crud, adapter: Adapter,
                       auth_token: str = None) -> PushResponse:
     receiver_responses = []
     for receiver in push.receivers:
         # get client endpoints
-        client_auth_token = f'Token {receiver.auth_token}'
+        client_auth_token = f'Token {encode_string_base64(receiver.auth_token)}'
         async with httpx.AsyncClient() as client:
             response = await client.get(receiver.endpoints_url,
                                         headers={'authorization': client_auth_token})
             endpoints = response.json()['data'][0]['endpoints']
 
         # get object data
         if push.module_id == ModuleID.tokens:
```

### Comparing `py_ocpi-0.3.0/py_ocpi/core/schemas.py` & `py_ocpi-0.3.1/py_ocpi/core/schemas.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from datetime import datetime, timezone
-from typing import List
+from typing import List, Union
 
 from pydantic import BaseModel
 
 from py_ocpi.core.data_types import String, DateTime, URL
 from py_ocpi.core.enums import ModuleID
 
 
 class OCPIResponse(BaseModel):
     """
     https://github.com/ocpi/ocpi/blob/2.2.1/transport_and_format.asciidoc#117-response-format
     """
-    data: list
+    data: Union[list, dict]
     status_code: int
     status_message: String(255)
     timestamp: DateTime = str(datetime.now(timezone.utc))
 
 
 class Receiver(BaseModel):
     endpoints_url: URL
```

### Comparing `py_ocpi-0.3.0/py_ocpi/core/status.py` & `py_ocpi-0.3.1/py_ocpi/core/status.py`

 * *Files identical despite different names*

### Comparing `py_ocpi-0.3.0/py_ocpi/core/utils.py` & `py_ocpi-0.3.1/py_ocpi/core/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import urllib
+import base64
 
 from fastapi import Response, Request
 from pydantic import BaseModel
 
 from py_ocpi.core.enums import ModuleID, RoleEnum
 from py_ocpi.core.config import settings
 from py_ocpi.modules.versions.enums import VersionNumber
@@ -14,15 +15,18 @@
     response.headers['X-Limit'] = str(limit)
     return response
 
 
 def get_auth_token(request: Request) -> str:
     headers = request.headers
     headers_token = headers.get('authorization', 'Token Null')
-    return headers_token.split()[1]
+    token = headers_token.split()[1]
+    if token == 'Null':  # nosec
+        return None
+    return decode_string_base64(token)
 
 
 async def get_list(response: Response, filters: dict, module: ModuleID, role: RoleEnum,
                    version: VersionNumber, crud, *args, **kwargs):
     data_list, total, is_last_page = await crud.list(module, role, filters, *args, version=version, **kwargs)
 
     link = ''
@@ -36,7 +40,17 @@
 
     return data_list
 
 
 def partially_update_attributes(instance: BaseModel, attributes: dict):
     for key, value in attributes.items():
         setattr(instance, key, value)
+
+
+def encode_string_base64(input: str) -> str:
+    input_bytes = base64.b64encode(bytes(input, 'utf-8'))
+    return input_bytes.decode('utf-8')
+
+
+def decode_string_base64(input: str) -> str:
+    input_bytes = base64.b64decode(bytes(input, 'utf-8'))
+    return input_bytes.decode('utf-8')
```

### Comparing `py_ocpi-0.3.0/py_ocpi/main.py` & `py_ocpi-0.3.1/py_ocpi/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from typing import Any, List
 
 from fastapi import FastAPI, Request, HTTPException
 from fastapi.responses import JSONResponse
 from fastapi.middleware.cors import CORSMiddleware
 from pydantic import ValidationError
 from starlette.middleware.base import BaseHTTPMiddleware, RequestResponseEndpoint
+from py_ocpi.core.endpoints import ENDPOINTS
 
 from py_ocpi.modules.versions.api import router as versions_router, versions_v_2_2_1_router
 from py_ocpi.modules.versions.enums import VersionNumber
 from py_ocpi.modules.versions.schemas import Version
-from py_ocpi.core.dependencies import get_crud, get_adapter, get_versions
+from py_ocpi.core.dependencies import get_crud, get_adapter, get_versions, get_endpoints
 from py_ocpi.core import status
 from py_ocpi.core.enums import RoleEnum
 from py_ocpi.core.config import settings
 from py_ocpi.core.data_types import URL
 from py_ocpi.core.schemas import OCPIResponse
 from py_ocpi.core.exceptions import AuthorizationOCPIError, NotFoundOCPIError
 from py_ocpi.core.push import http_router as http_push_router, websocket_router as websocket_push_router
@@ -78,48 +79,46 @@
     if websocket_push:
         _app.include_router(
             websocket_push_router,
             prefix=f'/{settings.PUSH_PREFIX}',
         )
 
     versions = []
+    version_endpoints = {}
 
     if VersionNumber.v_2_2_1 in version_numbers:
         _app.include_router(
             versions_v_2_2_1_router,
             prefix=f'/{settings.OCPI_PREFIX}',
         )
 
+        versions.append(
+            Version(
+                version=VersionNumber.v_2_2_1,
+                url=URL(f'https://{settings.OCPI_HOST}/{settings.OCPI_PREFIX}/{VersionNumber.v_2_2_1.value}/details')
+            ).dict(),
+        )
+
+        version_endpoints[VersionNumber.v_2_2_1] = []
+
         if RoleEnum.cpo in roles:
             _app.include_router(
                 v_2_2_1_cpo_router,
-                prefix=f'/{settings.OCPI_PREFIX}/cpo/{VersionNumber.v_2_2_1}',
+                prefix=f'/{settings.OCPI_PREFIX}/cpo/{VersionNumber.v_2_2_1.value}',
                 tags=['CPO']
             )
-
-            versions.append(
-                Version(
-                    version=VersionNumber.v_2_2_1,
-                    url=URL(f'https://{settings.OCPI_HOST}/{settings.OCPI_PREFIX}/cpo/{VersionNumber.v_2_2_1}')
-                ).dict(),
-            )
+            version_endpoints[VersionNumber.v_2_2_1] += ENDPOINTS[VersionNumber.v_2_2_1][RoleEnum.cpo]
 
         if RoleEnum.emsp in roles:
             _app.include_router(
                 v_2_2_1_emsp_router,
-                prefix=f'/{settings.OCPI_PREFIX}/emsp/{VersionNumber.v_2_2_1}',
+                prefix=f'/{settings.OCPI_PREFIX}/emsp/{VersionNumber.v_2_2_1.value}',
                 tags=['EMSP']
             )
-
-            versions.append(
-                Version(
-                    version=VersionNumber.v_2_2_1,
-                    url=URL(f'https://{settings.OCPI_HOST}/{settings.OCPI_PREFIX}/emsp/{VersionNumber.v_2_2_1}')
-                ).dict(),
-            )
+            version_endpoints[VersionNumber.v_2_2_1] += ENDPOINTS[VersionNumber.v_2_2_1][RoleEnum.emsp]
 
     def override_get_crud():
         return crud
 
     _app.dependency_overrides[get_crud] = override_get_crud
 
     def override_get_adapter():
@@ -128,8 +127,13 @@
     _app.dependency_overrides[get_adapter] = override_get_adapter
 
     def override_get_versions():
         return versions
 
     _app.dependency_overrides[get_versions] = override_get_versions
 
+    def override_get_endpoints():
+        return version_endpoints
+
+    _app.dependency_overrides[get_endpoints] = override_get_endpoints
+
     return _app
```

### Comparing `py_ocpi-0.3.0/py_ocpi/modules/cdrs/v_2_2_1/api/cpo.py` & `py_ocpi-0.3.1/py_ocpi/modules/cdrs/v_2_2_1/api/cpo.py`

 * *Files identical despite different names*

### Comparing `py_ocpi-0.3.0/py_ocpi/modules/cdrs/v_2_2_1/api/emsp.py` & `py_ocpi-0.3.1/py_ocpi/modules/cdrs/v_2_2_1/api/emsp.py`

 * *Files identical despite different names*

### Comparing `py_ocpi-0.3.0/py_ocpi/modules/cdrs/v_2_2_1/enums.py` & `py_ocpi-0.3.1/py_ocpi/modules/cdrs/v_2_2_1/enums.py`

 * *Files identical despite different names*

### Comparing `py_ocpi-0.3.0/py_ocpi/modules/cdrs/v_2_2_1/schemas.py` & `py_ocpi-0.3.1/py_ocpi/modules/cdrs/v_2_2_1/schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 
 class ChargingPeriod(BaseModel):
     """
     https://github.com/ocpi/ocpi/blob/2.2.1/mod_cdrs.asciidoc#146-chargingperiod-class
     """
     start_date_time: DateTime
-    diemnsions: List[CdrDimension]
+    dimensions: List[CdrDimension]
     tariff_id: Optional[CiString(36)]
 
 
 class CdrToken(BaseModel):
     """
     https://github.com/ocpi/ocpi/blob/2.2.1/mod_cdrs.asciidoc#145-cdrtoken-class
     """
```

### Comparing `py_ocpi-0.3.0/py_ocpi/modules/commands/v_2_2_1/api/cpo.py` & `py_ocpi-0.3.1/py_ocpi/modules/commands/v_2_2_1/api/cpo.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from py_ocpi.core.dependencies import get_crud, get_adapter
 from py_ocpi.core.enums import ModuleID, RoleEnum, Action
 from py_ocpi.core.exceptions import NotFoundOCPIError
 from py_ocpi.core.schemas import OCPIResponse
 from py_ocpi.core.adapter import Adapter
 from py_ocpi.core.crud import Crud
 from py_ocpi.core import status
-from py_ocpi.core.utils import get_auth_token
+from py_ocpi.core.utils import encode_string_base64, get_auth_token
 from py_ocpi.modules.versions.enums import VersionNumber
 from py_ocpi.modules.commands.v_2_2_1.enums import CommandType
 from py_ocpi.modules.commands.v_2_2_1.schemas import (
     CancelReservation, ReserveNow, StartSession,
     StopSession, UnlockConnector, CommandResult,
     CommandResultType, CommandResponse, CommandResponseType
 )
@@ -55,15 +55,15 @@
 
     if not command_result:
         command_result = CommandResult(result=CommandResultType.failed)
     else:
         command_result = adapter.command_result_adapter(command_result, VersionNumber.v_2_2_1)
 
     async with httpx.AsyncClient() as client:
-        authorization_token = f'Token {client_auth_token}'
+        authorization_token = f'Token {encode_string_base64(client_auth_token)}'
         await client.post(response_url, json=command_result.dict(), headers={'authorization': authorization_token})
 
 
 @router.post("/{command}", response_model=OCPIResponse)
 async def receive_command(request: Request, command: CommandType, data: dict, background_tasks: BackgroundTasks,
                           crud: Crud = Depends(get_crud), adapter: Adapter = Depends(get_adapter)):
     auth_token = get_auth_token(request)
```

### Comparing `py_ocpi-0.3.0/py_ocpi/modules/commands/v_2_2_1/api/emsp.py` & `py_ocpi-0.3.1/py_ocpi/modules/commands/v_2_2_1/api/emsp.py`

 * *Files identical despite different names*

### Comparing `py_ocpi-0.3.0/py_ocpi/modules/commands/v_2_2_1/enums.py` & `py_ocpi-0.3.1/py_ocpi/modules/commands/v_2_2_1/enums.py`

 * *Files identical despite different names*

### Comparing `py_ocpi-0.3.0/py_ocpi/modules/commands/v_2_2_1/schemas.py` & `py_ocpi-0.3.1/py_ocpi/modules/commands/v_2_2_1/schemas.py`

 * *Files identical despite different names*

### Comparing `py_ocpi-0.3.0/py_ocpi/modules/credentials/v_2_2_1/api/cpo.py` & `py_ocpi-0.3.1/py_ocpi/modules/credentials/v_2_2_1/api/cpo.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import httpx
 
 from fastapi import APIRouter, Depends, HTTPException, Request, status as fastapistatus
 
 from py_ocpi.core.schemas import OCPIResponse
 from py_ocpi.core.adapter import Adapter
 from py_ocpi.core.crud import Crud
-from py_ocpi.core.utils import get_auth_token
+from py_ocpi.core.utils import encode_string_base64, get_auth_token
 from py_ocpi.core.dependencies import get_crud, get_adapter
 from py_ocpi.core import status
 from py_ocpi.core.enums import Action, ModuleID, RoleEnum
 from py_ocpi.modules.versions.enums import VersionNumber
 from py_ocpi.modules.credentials.v_2_2_1.schemas import Credentials
 
 router = APIRouter(
@@ -20,15 +20,15 @@
 @router.get("/", response_model=OCPIResponse)
 async def get_credentials(request: Request, crud: Crud = Depends(get_crud), adapter: Adapter = Depends(get_adapter)):
     auth_token = get_auth_token(request)
 
     data = await crud.get(ModuleID.credentials_and_registration, RoleEnum.cpo,
                           auth_token, auth_token=auth_token, version=VersionNumber.v_2_2_1)
     return OCPIResponse(
-        data=[adapter.credentials_adapter(data).dict()],
+        data=adapter.credentials_adapter(data).dict(),
         **status.OCPI_1000_GENERIC_SUCESS_CODE,
     )
 
 
 @router.post("/", response_model=OCPIResponse)
 async def post_credentials(request: Request, credentials: Credentials,
                            crud: Crud = Depends(get_crud), adapter: Adapter = Depends(get_adapter)):
@@ -39,15 +39,15 @@
     server_cred = await crud.do(ModuleID.credentials_and_registration, RoleEnum.cpo, Action.get_client_token,
                                 version=VersionNumber.v_2_2_1, auth_token=auth_token)
     if server_cred:
         raise HTTPException(fastapistatus.HTTP_405_METHOD_NOT_ALLOWED, "Client is already registered")
 
     # Retrieve the versions and endpoints from the client
     async with httpx.AsyncClient() as client:
-        authorization_token = f'Token {credentials_client_token}'
+        authorization_token = f'Token {encode_string_base64(credentials_client_token)}'
         response_versions = await client.get(credentials.url,
                                              headers={'authorization': authorization_token})
 
         if response_versions.status_code == fastapistatus.HTTP_200_OK:
             version_url = None
             versions = response_versions.json()['data']
 
@@ -62,27 +62,27 @@
                 )
 
             response_endpoints = await client.get(version_url,
                                                   headers={'authorization': authorization_token})
 
             if response_endpoints.status_code == fastapistatus.HTTP_200_OK:
                 # Store client credentials and generate new credentials for sender
-                endpoints = response_endpoints.json()['data'][0]
+                endpoints = response_endpoints.json()['data']
                 new_credentials = await crud.create(
                     ModuleID.credentials_and_registration, RoleEnum.cpo,
                     {
                         "credentials": credentials.dict(),
                         "endpoints": endpoints
                     },
                     auth_token=auth_token,
                     version=VersionNumber.v_2_2_1
                 )
 
                 return OCPIResponse(
-                    data=[adapter.credentials_adapter(new_credentials).dict()],
+                    data=adapter.credentials_adapter(new_credentials).dict(),
                     **status.OCPI_1000_GENERIC_SUCESS_CODE
                 )
 
     return OCPIResponse(
         data=[],
         **status.OCPI_3001_UNABLE_TO_USE_CLIENTS_API,
     )
@@ -98,15 +98,15 @@
     server_cred = await crud.do(ModuleID.credentials_and_registration, RoleEnum.cpo, Action.get_client_token,
                                 version=VersionNumber.v_2_2_1, auth_token=auth_token)
     if not server_cred:
         raise HTTPException(fastapistatus.HTTP_405_METHOD_NOT_ALLOWED, "Client is not registered")
 
     # Retrieve the versions and endpoints from the client
     async with httpx.AsyncClient() as client:
-        authorization_token = f'Token {credentials_client_token}'
+        authorization_token = f'Token {encode_string_base64(credentials_client_token)}'
         response_versions = await client.get(credentials.url, headers={'authorization': authorization_token})
 
         if response_versions.status_code == fastapistatus.HTTP_200_OK:
             version_url = None
             versions = response_versions.json()['data']
 
             for version in versions:
@@ -130,15 +130,15 @@
                                                         "credentials": credentials.dict(),
                                                         "endpoints": endpoints
                                                     },
                                                     auth_token=auth_token,
                                                     version=VersionNumber.v_2_2_1)
 
                 return OCPIResponse(
-                    data=[adapter.credentials_adapter(new_credentials).dict()],
+                    data=adapter.credentials_adapter(new_credentials).dict(),
                     **status.OCPI_1000_GENERIC_SUCESS_CODE
                 )
 
     return OCPIResponse(
         data=[],
         **status.OCPI_3001_UNABLE_TO_USE_CLIENTS_API,
     )
```

### Comparing `py_ocpi-0.3.0/py_ocpi/modules/credentials/v_2_2_1/api/emsp.py` & `py_ocpi-0.3.1/py_ocpi/modules/credentials/v_2_2_1/api/emsp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import httpx
 
 from fastapi import APIRouter, Depends, HTTPException, Request, status as fastapistatus
 
 from py_ocpi.core.schemas import OCPIResponse
 from py_ocpi.core.adapter import Adapter
 from py_ocpi.core.crud import Crud
-from py_ocpi.core.utils import get_auth_token
+from py_ocpi.core.utils import encode_string_base64, get_auth_token
 from py_ocpi.core.dependencies import get_crud, get_adapter
 from py_ocpi.core import status
 from py_ocpi.core.enums import Action, ModuleID, RoleEnum
 from py_ocpi.modules.versions.enums import VersionNumber
 from py_ocpi.modules.credentials.v_2_2_1.schemas import Credentials
 
 router = APIRouter(
@@ -20,15 +20,15 @@
 @router.get("/", response_model=OCPIResponse)
 async def get_credentials(request: Request, crud: Crud = Depends(get_crud), adapter: Adapter = Depends(get_adapter)):
     auth_token = get_auth_token(request)
 
     data = await crud.get(ModuleID.credentials_and_registration, RoleEnum.emsp,
                           auth_token, auth_token=auth_token, version=VersionNumber.v_2_2_1)
     return OCPIResponse(
-        data=[adapter.credentials_adapter(data).dict()],
+        data=adapter.credentials_adapter(data).dict(),
         **status.OCPI_1000_GENERIC_SUCESS_CODE,
     )
 
 
 @router.post("/", response_model=OCPIResponse)
 async def post_credentials(request: Request, credentials: Credentials,
                            crud: Crud = Depends(get_crud), adapter: Adapter = Depends(get_adapter)):
@@ -39,15 +39,15 @@
     server_cred = await crud.do(ModuleID.credentials_and_registration, RoleEnum.emsp, Action.get_client_token,
                                 version=VersionNumber.v_2_2_1, auth_token=auth_token)
     if server_cred:
         raise HTTPException(fastapistatus.HTTP_405_METHOD_NOT_ALLOWED, "Client is already registered")
 
     # Retrieve the versions and endpoints from the client
     async with httpx.AsyncClient() as client:
-        authorization_token = f'Token {credentials_client_token}'
+        authorization_token = f'Token {encode_string_base64(credentials_client_token)}'
         response_versions = await client.get(credentials.url,
                                              headers={'authorization': authorization_token})
 
         if response_versions.status_code == fastapistatus.HTTP_200_OK:
             version_url = None
             versions = response_versions.json()['data']
 
@@ -62,27 +62,27 @@
                 )
 
             response_endpoints = await client.get(version_url,
                                                   headers={'authorization': authorization_token})
 
             if response_endpoints.status_code == fastapistatus.HTTP_200_OK:
                 # Store client credentials and generate new credentials for sender
-                endpoints = response_endpoints.json()['data'][0]
+                endpoints = response_endpoints.json()['data']
                 new_credentials = await crud.create(
                     ModuleID.credentials_and_registration, RoleEnum.emsp,
                     {
                         "credentials": credentials.dict(),
                         "endpoints": endpoints
                     },
                     auth_token=auth_token,
                     version=VersionNumber.v_2_2_1
                 )
 
                 return OCPIResponse(
-                    data=[adapter.credentials_adapter(new_credentials).dict()],
+                    data=adapter.credentials_adapter(new_credentials).dict(),
                     **status.OCPI_1000_GENERIC_SUCESS_CODE
                 )
 
     return OCPIResponse(
         data=[],
         **status.OCPI_3001_UNABLE_TO_USE_CLIENTS_API,
     )
@@ -98,15 +98,15 @@
     server_cred = await crud.do(ModuleID.credentials_and_registration, RoleEnum.emsp, Action.get_client_token,
                                 version=VersionNumber.v_2_2_1, auth_token=auth_token)
     if not server_cred:
         raise HTTPException(fastapistatus.HTTP_405_METHOD_NOT_ALLOWED, "Client is not registered")
 
     # Retrieve the versions and endpoints from the client
     async with httpx.AsyncClient() as client:
-        authorization_token = f'Token {credentials_client_token}'
+        authorization_token = f'Token {encode_string_base64(credentials_client_token)}'
         response_versions = await client.get(credentials.url, headers={'authorization': authorization_token})
 
         if response_versions.status_code == fastapistatus.HTTP_200_OK:
             version_url = None
             versions = response_versions.json()['data']
 
             for version in versions:
@@ -130,15 +130,15 @@
                                                         "credentials": credentials.dict(),
                                                         "endpoints": endpoints
                                                     },
                                                     auth_token=auth_token,
                                                     version=VersionNumber.v_2_2_1)
 
                 return OCPIResponse(
-                    data=[adapter.credentials_adapter(new_credentials).dict()],
+                    data=adapter.credentials_adapter(new_credentials).dict(),
                     **status.OCPI_1000_GENERIC_SUCESS_CODE
                 )
 
     return OCPIResponse(
         data=[],
         **status.OCPI_3001_UNABLE_TO_USE_CLIENTS_API,
     )
```

### Comparing `py_ocpi-0.3.0/py_ocpi/modules/credentials/v_2_2_1/schemas.py` & `py_ocpi-0.3.1/py_ocpi/modules/credentials/v_2_2_1/schemas.py`

 * *Files identical despite different names*

### Comparing `py_ocpi-0.3.0/py_ocpi/modules/locations/v_2_2_1/api/cpo.py` & `py_ocpi-0.3.1/py_ocpi/modules/locations/v_2_2_1/api/cpo.py`

 * *Files identical despite different names*

### Comparing `py_ocpi-0.3.0/py_ocpi/modules/locations/v_2_2_1/api/emsp.py` & `py_ocpi-0.3.1/py_ocpi/modules/locations/v_2_2_1/api/emsp.py`

 * *Files identical despite different names*

### Comparing `py_ocpi-0.3.0/py_ocpi/modules/locations/v_2_2_1/enums.py` & `py_ocpi-0.3.1/py_ocpi/modules/locations/v_2_2_1/enums.py`

 * *Files identical despite different names*

### Comparing `py_ocpi-0.3.0/py_ocpi/modules/locations/v_2_2_1/schemas.py` & `py_ocpi-0.3.1/py_ocpi/modules/locations/v_2_2_1/schemas.py`

 * *Files identical despite different names*

### Comparing `py_ocpi-0.3.0/py_ocpi/modules/sessions/v_2_2_1/api/cpo.py` & `py_ocpi-0.3.1/py_ocpi/modules/sessions/v_2_2_1/api/cpo.py`

 * *Files identical despite different names*

### Comparing `py_ocpi-0.3.0/py_ocpi/modules/sessions/v_2_2_1/api/emsp.py` & `py_ocpi-0.3.1/py_ocpi/modules/sessions/v_2_2_1/api/emsp.py`

 * *Files identical despite different names*

### Comparing `py_ocpi-0.3.0/py_ocpi/modules/sessions/v_2_2_1/enums.py` & `py_ocpi-0.3.1/py_ocpi/modules/sessions/v_2_2_1/enums.py`

 * *Files identical despite different names*

### Comparing `py_ocpi-0.3.0/py_ocpi/modules/sessions/v_2_2_1/schemas.py` & `py_ocpi-0.3.1/py_ocpi/modules/sessions/v_2_2_1/schemas.py`

 * *Files identical despite different names*

### Comparing `py_ocpi-0.3.0/py_ocpi/modules/tariffs/v_2_2_1/api/cpo.py` & `py_ocpi-0.3.1/py_ocpi/modules/tariffs/v_2_2_1/api/cpo.py`

 * *Files identical despite different names*

### Comparing `py_ocpi-0.3.0/py_ocpi/modules/tariffs/v_2_2_1/api/emsp.py` & `py_ocpi-0.3.1/py_ocpi/modules/tariffs/v_2_2_1/api/emsp.py`

 * *Files identical despite different names*

### Comparing `py_ocpi-0.3.0/py_ocpi/modules/tariffs/v_2_2_1/enums.py` & `py_ocpi-0.3.1/py_ocpi/modules/tariffs/v_2_2_1/enums.py`

 * *Files identical despite different names*

### Comparing `py_ocpi-0.3.0/py_ocpi/modules/tariffs/v_2_2_1/schemas.py` & `py_ocpi-0.3.1/py_ocpi/modules/tariffs/v_2_2_1/schemas.py`

 * *Files identical despite different names*

### Comparing `py_ocpi-0.3.0/py_ocpi/modules/tokens/v_2_2_1/api/cpo.py` & `py_ocpi-0.3.1/py_ocpi/modules/tokens/v_2_2_1/api/cpo.py`

 * *Files identical despite different names*

### Comparing `py_ocpi-0.3.0/py_ocpi/modules/tokens/v_2_2_1/api/emsp.py` & `py_ocpi-0.3.1/py_ocpi/modules/tokens/v_2_2_1/api/emsp.py`

 * *Files identical despite different names*

### Comparing `py_ocpi-0.3.0/py_ocpi/modules/tokens/v_2_2_1/enums.py` & `py_ocpi-0.3.1/py_ocpi/modules/tokens/v_2_2_1/enums.py`

 * *Files identical despite different names*

### Comparing `py_ocpi-0.3.0/py_ocpi/modules/tokens/v_2_2_1/schemas.py` & `py_ocpi-0.3.1/py_ocpi/modules/tokens/v_2_2_1/schemas.py`

 * *Files identical despite different names*

### Comparing `py_ocpi-0.3.0/py_ocpi/modules/versions/enums.py` & `py_ocpi-0.3.1/py_ocpi/modules/versions/enums.py`

 * *Files identical despite different names*

### Comparing `py_ocpi-0.3.0/py_ocpi/modules/versions/schemas.py` & `py_ocpi-0.3.1/py_ocpi/modules/versions/schemas.py`

 * *Files identical despite different names*

### Comparing `py_ocpi-0.3.0/py_ocpi/routers/v_2_2_1/cpo.py` & `py_ocpi-0.3.1/py_ocpi/routers/v_2_2_1/cpo.py`

 * *Files identical despite different names*

### Comparing `py_ocpi-0.3.0/py_ocpi/routers/v_2_2_1/emsp.py` & `py_ocpi-0.3.1/py_ocpi/routers/v_2_2_1/emsp.py`

 * *Files identical despite different names*

### Comparing `py_ocpi-0.3.0/pyproject.toml` & `py_ocpi-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py_ocpi"
-version = "0.3.0"
+version = "0.3.1"
 description = "Python Implementation of OCPI"
 authors = ["HAkhavan71 <hakh.27@gmail.com>"]
 readme = "README.rst"
 homepage = "https://github.com/TECHS-Technological-Solutions/ocpi"
 license = "MIT"
 include = [
     "LICENSE",
```

### Comparing `py_ocpi-0.3.0/PKG-INFO` & `py_ocpi-0.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-ocpi
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python Implementation of OCPI
 Home-page: https://github.com/TECHS-Technological-Solutions/ocpi
 License: MIT
 Keywords: ocpi
 Author: HAkhavan71
 Author-email: hakh.27@gmail.com
 Requires-Python: >=3.9,<4.0
```

