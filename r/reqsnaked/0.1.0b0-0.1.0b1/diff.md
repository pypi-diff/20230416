# Comparing `tmp/reqsnaked-0.1.0_beta0.tar.gz` & `tmp/reqsnaked-0.1.0_beta1.tar.gz`

## Comparing `reqsnaked-0.1.0_beta0.tar` & `reqsnaked-0.1.0_beta1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 reqsnaked-0.1.0_beta0/Cargo.toml
--rw-r--r--   0      501       20     1825 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/.github/workflows/CI.yml
--rw-r--r--   0      501       20      806 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/.github/workflows/deploy-gh-docs.yml
--rw-r--r--   0      501       20      694 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/.gitignore
--rw-r--r--   0      501       20       97 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/Makefile
--rw-r--r--   0      501       20     2020 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/README.md
--rw-r--r--   0      501       20    35310 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/assets/reqsnaked-black.png
--rw-r--r--   0      501       20    34542 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/assets/reqsnaked-white.png
--rw-r--r--   0      501       20   252614 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/assets/reqsnaked.psd
--rw-r--r--   0      501       20     2593 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/benchmarks/README.md
--rw-r--r--   0      501       20   686179 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/benchmarks/jsons/large.json
--rw-r--r--   0      501       20    68489 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/benchmarks/jsons/medium.json
--rw-r--r--   0      501       20     2564 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/benchmarks/jsons/small.json
--rw-r--r--   0      501       20     1115 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/benchmarks/test_libs.py
--rw-r--r--   0      501       20    35310 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/guide/assets/reqsnaked-black.png
--rw-r--r--   0      501       20    46481 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/guide/assets/reqsnaked-filled-white.png
--rw-r--r--   0      501       20   332852 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/guide/assets/reqsnaked-filled.psd
--rw-r--r--   0      501       20    34542 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/guide/assets/reqsnaked-white.png
--rw-r--r--   0      501       20   252614 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/guide/assets/reqsnaked.psd
--rw-r--r--   0      501       20        0 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/guide/coming-soon.md
--rw-r--r--   0      501       20      715 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/guide/contributing.md
--rw-r--r--   0      501       20      969 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/guide/css/theme.css
--rw-r--r--   0      501       20     2197 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/guide/index.md
--rw-r--r--   0      501       20      399 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/guide/support.md
--rw-r--r--   0      501       20     1767 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/guide/user-guide/auth.md
--rw-r--r--   0      501       20     2770 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/guide/user-guide/basics.md
--rw-r--r--   0      501       20     1208 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/guide/user-guide/chunks.md
--rw-r--r--   0      501       20      421 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/guide/user-guide/cookies.md
--rw-r--r--   0      501       20     1072 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/guide/user-guide/form.md
--rw-r--r--   0      501       20     4158 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/guide/user-guide/headers.md
--rw-r--r--   0      501       20      774 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/guide/user-guide/index.md
--rw-r--r--   0      501       20     3615 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/guide/user-guide/json.md
--rw-r--r--   0      501       20     1412 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/guide/user-guide/multipart.md
--rw-r--r--   0      501       20     1898 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/guide/user-guide/query-string.md
--rw-r--r--   0      501       20      980 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/guide/user-guide/raw-response.md
--rw-r--r--   0      501       20     3331 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/mkdocs.yml
--rw-r--r--   0      501       20      651 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/pyproject.toml
--rw-r--r--   0      501       20     3170 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/reqsnaked.pyi
--rw-r--r--   0      501       20      435 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/sandbox/bar.py
--rw-r--r--   0      501       20     1214 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/sandbox/bazz.py
--rw-r--r--   0      501       20      738 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/sandbox/eee.py
--rw-r--r--   0      501       20     1682 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/sandbox/fizz.py
--rw-r--r--   0      501       20      696 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/sandbox/foo.py
--rw-r--r--   0      501       20     2825 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/sandbox/rrr.py
--rw-r--r--   0      501       20     3043 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/src/aio/client.rs
--rw-r--r--   0      501       20      482 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/src/aio/mod.rs
--rw-r--r--   0      501       20     1357 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/src/aio/multipart/form.rs
--rw-r--r--   0      501       20      336 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/src/aio/multipart/mod.rs
--rw-r--r--   0      501       20     1392 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/src/aio/multipart/part.rs
--rw-r--r--   0      501       20     5363 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/src/aio/request.rs
--rw-r--r--   0      501       20     3659 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/src/aio/response.rs
--rw-r--r--   0      501       20     5271 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/src/exceptions.rs
--rw-r--r--   0      501       20     4079 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/src/json.rs
--rw-r--r--   0      501       20      326 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/src/lib.rs
--rw-r--r--   0      501       20      112 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/src/py2rs/base.rs
--rw-r--r--   0      501       20      666 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/src/py2rs/duration.rs
--rw-r--r--   0      501       20     1136 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/src/py2rs/http_method.rs
--rw-r--r--   0      501       20       81 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/src/py2rs/mod.rs
--rw-r--r--   0      501       20      410 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/src/py2rs/query.rs
--rw-r--r--   0      501       20      915 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/src/py2rs/url.rs
--rw-r--r--   0      501       20      542 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/src/rs2py/bytes.rs
--rw-r--r--   0      501       20      899 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/src/rs2py/header_map.rs
--rw-r--r--   0      501       20     1256 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/src/rs2py/http_version.rs
--rw-r--r--   0      501       20      376 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/src/rs2py/mod.rs
--rw-r--r--   0      501       20      110 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/tests/conftest.py
--rw-r--r--   0      501       20      968 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/tests/test_client.py
--rw-r--r--   0      501       20      677 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/tests/test_mess.py
--rw-r--r--   0      501       20     3118 2023-03-01 18:33:24.000000 reqsnaked-0.1.0_beta0/tests/test_request.py
--rw-r--r--   0        0        0     2927 1970-01-01 00:00:00.000000 reqsnaked-0.1.0_beta0/PKG-INFO
+-rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 reqsnaked-0.1.0_beta1/Cargo.toml
+-rw-r--r--   0      501       20     1825 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/.github/workflows/CI.yml
+-rw-r--r--   0      501       20      806 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/.github/workflows/deploy-gh-docs.yml
+-rw-r--r--   0      501       20      694 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/.gitignore
+-rw-r--r--   0      501       20       97 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/Makefile
+-rw-r--r--   0      501       20     2020 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/README.md
+-rw-r--r--   0      501       20    35310 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/assets/reqsnaked-black.png
+-rw-r--r--   0      501       20    34542 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/assets/reqsnaked-white.png
+-rw-r--r--   0      501       20   252614 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/assets/reqsnaked.psd
+-rw-r--r--   0      501       20     2593 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/benchmarks/README.md
+-rw-r--r--   0      501       20   686179 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/benchmarks/jsons/large.json
+-rw-r--r--   0      501       20    68489 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/benchmarks/jsons/medium.json
+-rw-r--r--   0      501       20     2564 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/benchmarks/jsons/small.json
+-rw-r--r--   0      501       20     1115 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/benchmarks/test_libs.py
+-rw-r--r--   0      501       20    35310 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/guide/assets/reqsnaked-black.png
+-rw-r--r--   0      501       20    46481 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/guide/assets/reqsnaked-filled-white.png
+-rw-r--r--   0      501       20   332852 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/guide/assets/reqsnaked-filled.psd
+-rw-r--r--   0      501       20    34542 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/guide/assets/reqsnaked-white.png
+-rw-r--r--   0      501       20   252614 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/guide/assets/reqsnaked.psd
+-rw-r--r--   0      501       20        0 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/guide/coming-soon.md
+-rw-r--r--   0      501       20      715 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/guide/contributing.md
+-rw-r--r--   0      501       20      969 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/guide/css/theme.css
+-rw-r--r--   0      501       20     2197 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/guide/index.md
+-rw-r--r--   0      501       20      399 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/guide/support.md
+-rw-r--r--   0      501       20     1767 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/guide/user-guide/auth.md
+-rw-r--r--   0      501       20     2770 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/guide/user-guide/basics.md
+-rw-r--r--   0      501       20     1208 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/guide/user-guide/chunks.md
+-rw-r--r--   0      501       20      421 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/guide/user-guide/cookies.md
+-rw-r--r--   0      501       20     1072 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/guide/user-guide/form.md
+-rw-r--r--   0      501       20     4158 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/guide/user-guide/headers.md
+-rw-r--r--   0      501       20      774 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/guide/user-guide/index.md
+-rw-r--r--   0      501       20     3615 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/guide/user-guide/json.md
+-rw-r--r--   0      501       20     1412 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/guide/user-guide/multipart.md
+-rw-r--r--   0      501       20     1898 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/guide/user-guide/query-string.md
+-rw-r--r--   0      501       20      980 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/guide/user-guide/raw-response.md
+-rw-r--r--   0      501       20     3331 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/mkdocs.yml
+-rw-r--r--   0      501       20      652 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/pyproject.toml
+-rw-r--r--   0      501       20     3170 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/reqsnaked.pyi
+-rw-r--r--   0      501       20      435 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/sandbox/bar.py
+-rw-r--r--   0      501       20     1214 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/sandbox/bazz.py
+-rw-r--r--   0      501       20      738 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/sandbox/eee.py
+-rw-r--r--   0      501       20     1682 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/sandbox/fizz.py
+-rw-r--r--   0      501       20      696 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/sandbox/foo.py
+-rw-r--r--   0      501       20     2825 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/sandbox/rrr.py
+-rw-r--r--   0      501       20     3043 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/src/aio/client.rs
+-rw-r--r--   0      501       20      482 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/src/aio/mod.rs
+-rw-r--r--   0      501       20     1357 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/src/aio/multipart/form.rs
+-rw-r--r--   0      501       20      336 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/src/aio/multipart/mod.rs
+-rw-r--r--   0      501       20     1392 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/src/aio/multipart/part.rs
+-rw-r--r--   0      501       20     5363 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/src/aio/request.rs
+-rw-r--r--   0      501       20     3659 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/src/aio/response.rs
+-rw-r--r--   0      501       20     5271 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/src/exceptions.rs
+-rw-r--r--   0      501       20     4079 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/src/json.rs
+-rw-r--r--   0      501       20      326 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/src/lib.rs
+-rw-r--r--   0      501       20      112 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/src/py2rs/base.rs
+-rw-r--r--   0      501       20      666 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/src/py2rs/duration.rs
+-rw-r--r--   0      501       20     1136 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/src/py2rs/http_method.rs
+-rw-r--r--   0      501       20       81 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/src/py2rs/mod.rs
+-rw-r--r--   0      501       20      410 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/src/py2rs/query.rs
+-rw-r--r--   0      501       20      915 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/src/py2rs/url.rs
+-rw-r--r--   0      501       20      542 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/src/rs2py/bytes.rs
+-rw-r--r--   0      501       20      899 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/src/rs2py/header_map.rs
+-rw-r--r--   0      501       20     1256 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/src/rs2py/http_version.rs
+-rw-r--r--   0      501       20      376 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/src/rs2py/mod.rs
+-rw-r--r--   0      501       20      110 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/tests/conftest.py
+-rw-r--r--   0      501       20      968 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/tests/test_client.py
+-rw-r--r--   0      501       20      677 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/tests/test_mess.py
+-rw-r--r--   0      501       20     3118 2023-04-16 14:50:46.000000 reqsnaked-0.1.0_beta1/tests/test_request.py
+-rw-r--r--   0        0        0     2927 1970-01-01 00:00:00.000000 reqsnaked-0.1.0_beta1/PKG-INFO
```

### Comparing `reqsnaked-0.1.0_beta0/Cargo.toml` & `reqsnaked-0.1.0_beta1/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "reqsnaked"
-version = "0.1.0-beta0"
+version = "0.1.0-beta1"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "reqsnaked"
 crate-type = ["cdylib"]
```

### Comparing `reqsnaked-0.1.0_beta0/.github/workflows/CI.yml` & `reqsnaked-0.1.0_beta1/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `reqsnaked-0.1.0_beta0/.github/workflows/deploy-gh-docs.yml` & `reqsnaked-0.1.0_beta1/.github/workflows/deploy-gh-docs.yml`

 * *Files identical despite different names*

### Comparing `reqsnaked-0.1.0_beta0/.gitignore` & `reqsnaked-0.1.0_beta1/.gitignore`

 * *Files identical despite different names*

### Comparing `reqsnaked-0.1.0_beta0/README.md` & `reqsnaked-0.1.0_beta1/README.md`

 * *Files identical despite different names*

### Comparing `reqsnaked-0.1.0_beta0/assets/reqsnaked-black.png` & `reqsnaked-0.1.0_beta1/assets/reqsnaked-black.png`

 * *Files identical despite different names*

### Comparing `reqsnaked-0.1.0_beta0/assets/reqsnaked-white.png` & `reqsnaked-0.1.0_beta1/assets/reqsnaked-white.png`

 * *Files identical despite different names*

### Comparing `reqsnaked-0.1.0_beta0/assets/reqsnaked.psd` & `reqsnaked-0.1.0_beta1/assets/reqsnaked.psd`

 * *Files identical despite different names*

### Comparing `reqsnaked-0.1.0_beta0/benchmarks/README.md` & `reqsnaked-0.1.0_beta1/benchmarks/README.md`

 * *Files identical despite different names*

### Comparing `reqsnaked-0.1.0_beta0/benchmarks/jsons/large.json` & `reqsnaked-0.1.0_beta1/benchmarks/jsons/large.json`

 * *Files identical despite different names*

### Comparing `reqsnaked-0.1.0_beta0/benchmarks/jsons/medium.json` & `reqsnaked-0.1.0_beta1/benchmarks/jsons/medium.json`

 * *Files identical despite different names*

### Comparing `reqsnaked-0.1.0_beta0/benchmarks/jsons/small.json` & `reqsnaked-0.1.0_beta1/benchmarks/jsons/small.json`

 * *Files identical despite different names*

### Comparing `reqsnaked-0.1.0_beta0/benchmarks/test_libs.py` & `reqsnaked-0.1.0_beta1/benchmarks/test_libs.py`

 * *Files identical despite different names*

### Comparing `reqsnaked-0.1.0_beta0/guide/assets/reqsnaked-black.png` & `reqsnaked-0.1.0_beta1/guide/assets/reqsnaked-black.png`

 * *Files identical despite different names*

### Comparing `reqsnaked-0.1.0_beta0/guide/assets/reqsnaked-filled-white.png` & `reqsnaked-0.1.0_beta1/guide/assets/reqsnaked-filled-white.png`

 * *Files identical despite different names*

### Comparing `reqsnaked-0.1.0_beta0/guide/assets/reqsnaked-filled.psd` & `reqsnaked-0.1.0_beta1/guide/assets/reqsnaked-filled.psd`

 * *Files identical despite different names*

### Comparing `reqsnaked-0.1.0_beta0/guide/assets/reqsnaked-white.png` & `reqsnaked-0.1.0_beta1/guide/assets/reqsnaked-white.png`

 * *Files identical despite different names*

### Comparing `reqsnaked-0.1.0_beta0/guide/assets/reqsnaked.psd` & `reqsnaked-0.1.0_beta1/guide/assets/reqsnaked.psd`

 * *Files identical despite different names*

### Comparing `reqsnaked-0.1.0_beta0/guide/contributing.md` & `reqsnaked-0.1.0_beta1/guide/contributing.md`

 * *Files identical despite different names*

### Comparing `reqsnaked-0.1.0_beta0/guide/css/theme.css` & `reqsnaked-0.1.0_beta1/guide/css/theme.css`

 * *Files identical despite different names*

### Comparing `reqsnaked-0.1.0_beta0/guide/index.md` & `reqsnaked-0.1.0_beta1/guide/index.md`

 * *Files identical despite different names*

### Comparing `reqsnaked-0.1.0_beta0/guide/user-guide/auth.md` & `reqsnaked-0.1.0_beta1/guide/user-guide/auth.md`

 * *Files identical despite different names*

### Comparing `reqsnaked-0.1.0_beta0/guide/user-guide/basics.md` & `reqsnaked-0.1.0_beta1/guide/user-guide/basics.md`

 * *Files identical despite different names*

### Comparing `reqsnaked-0.1.0_beta0/guide/user-guide/chunks.md` & `reqsnaked-0.1.0_beta1/guide/user-guide/chunks.md`

 * *Files identical despite different names*

### Comparing `reqsnaked-0.1.0_beta0/guide/user-guide/form.md` & `reqsnaked-0.1.0_beta1/guide/user-guide/form.md`

 * *Files identical despite different names*

### Comparing `reqsnaked-0.1.0_beta0/guide/user-guide/headers.md` & `reqsnaked-0.1.0_beta1/guide/user-guide/headers.md`

 * *Files identical despite different names*

### Comparing `reqsnaked-0.1.0_beta0/guide/user-guide/index.md` & `reqsnaked-0.1.0_beta1/guide/user-guide/index.md`

 * *Files identical despite different names*

### Comparing `reqsnaked-0.1.0_beta0/guide/user-guide/json.md` & `reqsnaked-0.1.0_beta1/guide/user-guide/json.md`

 * *Files identical despite different names*

### Comparing `reqsnaked-0.1.0_beta0/guide/user-guide/multipart.md` & `reqsnaked-0.1.0_beta1/guide/user-guide/multipart.md`

 * *Files identical despite different names*

### Comparing `reqsnaked-0.1.0_beta0/guide/user-guide/query-string.md` & `reqsnaked-0.1.0_beta1/guide/user-guide/query-string.md`

 * *Files identical despite different names*

### Comparing `reqsnaked-0.1.0_beta0/guide/user-guide/raw-response.md` & `reqsnaked-0.1.0_beta1/guide/user-guide/raw-response.md`

 * *Files identical despite different names*

### Comparing `reqsnaked-0.1.0_beta0/mkdocs.yml` & `reqsnaked-0.1.0_beta1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `reqsnaked-0.1.0_beta0/pyproject.toml` & `reqsnaked-0.1.0_beta1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=0.12,<0.13"]
 build-backend = "maturin"
 
 [project]
 name = "reqsnaked"
-version = "0.1.0-beta0"
+version = "0.1.0-beta1"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 
@@ -27,8 +27,8 @@
     "pytest-asyncio==0.20.3"
 ]
 
 benchmark = [
     "aiohttp==3.8.4",
     "httpx==0.23.3",
     "pytest-benchmark==4.0.0"
-]
+]
```

### Comparing `reqsnaked-0.1.0_beta0/reqsnaked.pyi` & `reqsnaked-0.1.0_beta1/reqsnaked.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     str, int, bool, None, typing.List[
         typing.Union[str, int, bool, None]
     ]
 ]
 
 
 class Bytes:
-    def to_bytes(self) -> bytes:
+    def as_bytes(self) -> bytes:
         pass
 
 
 class Stream:
     async def gnaw(self) -> typing.Optional[Bytes]:
         pass
```

### Comparing `reqsnaked-0.1.0_beta0/sandbox/bazz.py` & `reqsnaked-0.1.0_beta1/sandbox/bazz.py`

 * *Files identical despite different names*

### Comparing `reqsnaked-0.1.0_beta0/sandbox/eee.py` & `reqsnaked-0.1.0_beta1/sandbox/eee.py`

 * *Files identical despite different names*

### Comparing `reqsnaked-0.1.0_beta0/sandbox/fizz.py` & `reqsnaked-0.1.0_beta1/sandbox/fizz.py`

 * *Files identical despite different names*

### Comparing `reqsnaked-0.1.0_beta0/sandbox/foo.py` & `reqsnaked-0.1.0_beta1/sandbox/foo.py`

 * *Files identical despite different names*

### Comparing `reqsnaked-0.1.0_beta0/sandbox/rrr.py` & `reqsnaked-0.1.0_beta1/sandbox/rrr.py`

 * *Files identical despite different names*

### Comparing `reqsnaked-0.1.0_beta0/src/aio/client.rs` & `reqsnaked-0.1.0_beta1/src/aio/client.rs`

 * *Files identical despite different names*

### Comparing `reqsnaked-0.1.0_beta0/src/aio/multipart/form.rs` & `reqsnaked-0.1.0_beta1/src/aio/multipart/form.rs`

 * *Files identical despite different names*

### Comparing `reqsnaked-0.1.0_beta0/src/aio/multipart/part.rs` & `reqsnaked-0.1.0_beta1/src/aio/multipart/part.rs`

 * *Files identical despite different names*

### Comparing `reqsnaked-0.1.0_beta0/src/aio/request.rs` & `reqsnaked-0.1.0_beta1/src/aio/request.rs`

 * *Files identical despite different names*

### Comparing `reqsnaked-0.1.0_beta0/src/aio/response.rs` & `reqsnaked-0.1.0_beta1/src/aio/response.rs`

 * *Files identical despite different names*

### Comparing `reqsnaked-0.1.0_beta0/src/exceptions.rs` & `reqsnaked-0.1.0_beta1/src/exceptions.rs`

 * *Files identical despite different names*

### Comparing `reqsnaked-0.1.0_beta0/src/json.rs` & `reqsnaked-0.1.0_beta1/src/json.rs`

 * *Files identical despite different names*

### Comparing `reqsnaked-0.1.0_beta0/src/py2rs/duration.rs` & `reqsnaked-0.1.0_beta1/src/py2rs/duration.rs`

 * *Files identical despite different names*

### Comparing `reqsnaked-0.1.0_beta0/src/py2rs/http_method.rs` & `reqsnaked-0.1.0_beta1/src/py2rs/http_method.rs`

 * *Files identical despite different names*

### Comparing `reqsnaked-0.1.0_beta0/src/py2rs/url.rs` & `reqsnaked-0.1.0_beta1/src/py2rs/url.rs`

 * *Files identical despite different names*

### Comparing `reqsnaked-0.1.0_beta0/src/rs2py/bytes.rs` & `reqsnaked-0.1.0_beta1/src/rs2py/bytes.rs`

 * *Files identical despite different names*

### Comparing `reqsnaked-0.1.0_beta0/src/rs2py/header_map.rs` & `reqsnaked-0.1.0_beta1/src/rs2py/header_map.rs`

 * *Files identical despite different names*

### Comparing `reqsnaked-0.1.0_beta0/src/rs2py/http_version.rs` & `reqsnaked-0.1.0_beta1/src/rs2py/http_version.rs`

 * *Files identical despite different names*

### Comparing `reqsnaked-0.1.0_beta0/tests/test_client.py` & `reqsnaked-0.1.0_beta1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `reqsnaked-0.1.0_beta0/tests/test_mess.py` & `reqsnaked-0.1.0_beta1/tests/test_mess.py`

 * *Files identical despite different names*

### Comparing `reqsnaked-0.1.0_beta0/tests/test_request.py` & `reqsnaked-0.1.0_beta1/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `reqsnaked-0.1.0_beta0/PKG-INFO` & `reqsnaked-0.1.0_beta1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: reqsnaked
-Version: 0.1.0_beta0
+Version: 0.1.0_beta1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Dist: aiohttp==3.8.4; extra == 'benchmark'
-Requires-Dist: httpx==0.23.3; extra == 'benchmark'
-Requires-Dist: pytest-benchmark==4.0.0; extra == 'benchmark'
 Requires-Dist: mkdocs==1.4.2; extra == 'docs'
 Requires-Dist: mkdocs-material==9.0.14; extra == 'docs'
 Requires-Dist: mike==1.1.2; extra == 'docs'
 Requires-Dist: pillow==9.4.0; extra == 'docs'
 Requires-Dist: cairosvg==2.6.0; extra == 'docs'
 Requires-Dist: pytest==7.2.1; extra == 'test'
 Requires-Dist: pytest-asyncio==0.20.3; extra == 'test'
-Provides-Extra: benchmark
+Requires-Dist: aiohttp==3.8.4; extra == 'benchmark'
+Requires-Dist: httpx==0.23.3; extra == 'benchmark'
+Requires-Dist: pytest-benchmark==4.0.0; extra == 'benchmark'
 Provides-Extra: docs
 Provides-Extra: test
+Provides-Extra: benchmark
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # Reqsnaked
 Reqsnaked is a blazing fast async/await HTTP client for Python written on Rust using reqwests.
 
 * [Works 15% faster than `aiohttp` on average](./benchmarks)
```

