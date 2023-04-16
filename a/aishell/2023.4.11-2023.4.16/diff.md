# Comparing `tmp/aishell-2023.4.11.tar.gz` & `tmp/aishell-2023.4.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aishell-2023.4.11.tar", max compression
+gzip compressed data, was "aishell-2023.4.16.tar", max compression
```

## Comparing `aishell-2023.4.11.tar` & `aishell-2023.4.16.tar`

### file list

```diff
@@ -1,38 +1,15 @@
--rw-r--r--   0        0        0     1064 2023-04-11 07:50:18.503513 aishell-2023.4.11/LICENSE
--rw-r--r--   0        0        0     2959 2023-04-11 07:50:18.503513 aishell-2023.4.11/README.md
--rw-r--r--   0        0        0       53 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/__init__.py
--rw-r--r--   0        0        0      128 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/__main__.py
--rw-r--r--   0        0        0       78 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/adapters/__init__.py
--rw-r--r--   0        0        0     1151 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/adapters/openai_cookie_adapter.py
--rw-r--r--   0        0        0        0 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/adapters/test/__init__.py
--rw-r--r--   0        0        0      707 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/adapters/test/test_openai_chatgpt_adapter.py
--rw-r--r--   0        0        0       90 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/cli/__init__.py
--rw-r--r--   0        0        0     2787 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/cli/aishell.py
--rw-r--r--   0        0        0       43 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/cli/cli_app.py
--rw-r--r--   0        0        0     2675 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/cli/config_aishell.py
--rw-r--r--   0        0        0        0 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/cli/test/__init__.py
--rw-r--r--   0        0        0     2614 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/cli/test/test_config_aishell.py
--rw-r--r--   0        0        0       90 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/exceptions/__init__.py
--rw-r--r--   0        0        0       51 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/exceptions/unauthorized_access_error.py
--rw-r--r--   0        0        0      323 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/models/__init__.py
--rw-r--r--   0        0        0     1058 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/models/aishell_config_model.py
--rw-r--r--   0        0        0      173 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/models/language_model.py
--rw-r--r--   0        0        0      505 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/models/open_ai_response_model.py
--rw-r--r--   0        0        0      705 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/models/revchatgpt_chatbot_config_model.py
--rw-r--r--   0        0        0      403 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/models/str_enum.py
--rw-r--r--   0        0        0        0 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/py.typed
--rw-r--r--   0        0        0      299 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/query_clients/__init__.py
--rw-r--r--   0        0        0     1330 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/query_clients/gpt3_client.py
--rw-r--r--   0        0        0     1150 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/query_clients/official_chatgpt_client.py
--rw-r--r--   0        0        0      155 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/query_clients/query_client.py
--rw-r--r--   0        0        0     2069 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/query_clients/reverse_engineered_chatgpt_client.py
--rw-r--r--   0        0        0        0 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/tests/__init__.py
--rw-r--r--   0        0        0       77 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/tests/sample_test.py
--rw-r--r--   0        0        0      171 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/utils/__init__.py
--rw-r--r--   0        0        0     1708 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/utils/aishell_config_manager.py
--rw-r--r--   0        0        0      389 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/utils/make_executable_command.py
--rw-r--r--   0        0        0        0 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/utils/test/__init__.py
--rw-r--r--   0        0        0      349 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/utils/test/test_aishell_config_manager.py
--rw-r--r--   0        0        0      884 2023-04-11 07:50:18.503513 aishell-2023.4.11/aishell/utils/test/test_make_executable_command.py
--rw-r--r--   0        0        0     1433 2023-04-11 07:50:44.415679 aishell-2023.4.11/pyproject.toml
--rw-r--r--   0        0        0     3547 1970-01-01 00:00:00.000000 aishell-2023.4.11/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-16 07:58:01.571269 aishell-2023.4.16/LICENSE
+-rw-r--r--   0        0        0     2828 2023-04-16 07:58:01.571269 aishell-2023.4.16/README.md
+-rw-r--r--   0        0        0       53 2023-04-16 07:58:01.571269 aishell-2023.4.16/aishell/__init__.py
+-rw-r--r--   0        0        0      128 2023-04-16 07:58:01.571269 aishell-2023.4.16/aishell/__main__.py
+-rw-r--r--   0        0        0       90 2023-04-16 07:58:01.571269 aishell-2023.4.16/aishell/cli/__init__.py
+-rw-r--r--   0        0        0     1571 2023-04-16 07:58:01.571269 aishell-2023.4.16/aishell/cli/aishell.py
+-rw-r--r--   0        0        0       43 2023-04-16 07:58:01.571269 aishell-2023.4.16/aishell/cli/cli_app.py
+-rw-r--r--   0        0        0     1305 2023-04-16 07:58:01.571269 aishell-2023.4.16/aishell/cli/config_aishell.py
+-rw-r--r--   0        0        0        0 2023-04-16 07:58:01.571269 aishell-2023.4.16/aishell/py.typed
+-rw-r--r--   0        0        0        0 2023-04-16 07:58:01.571269 aishell-2023.4.16/aishell/tests/__init__.py
+-rw-r--r--   0        0        0       77 2023-04-16 07:58:01.571269 aishell-2023.4.16/aishell/tests/sample_test.py
+-rw-r--r--   0        0        0       68 2023-04-16 07:58:01.571269 aishell-2023.4.16/aishell/utils/__init__.py
+-rw-r--r--   0        0        0      269 2023-04-16 07:58:01.571269 aishell-2023.4.16/aishell/utils/construct_prompt.py
+-rw-r--r--   0        0        0     1406 2023-04-16 07:58:24.391304 aishell-2023.4.16/pyproject.toml
+-rw-r--r--   0        0        0     3349 1970-01-01 00:00:00.000000 aishell-2023.4.16/PKG-INFO
```

### Comparing `aishell-2023.4.11/LICENSE` & `aishell-2023.4.16/LICENSE`

 * *Files identical despite different names*

### Comparing `aishell-2023.4.11/README.md` & `aishell-2023.4.16/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: aishell
+Version: 2023.4.16
+Summary: 
+Requires-Python: >=3.9,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: poetry (>=1.4.0,<2.0.0)
+Requires-Dist: revchatgptauth (>=2023.4.16,<2024.0.0)
+Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
+Requires-Dist: ygka (>=2023.4.16.post1,<2024.0.0)
+Description-Content-Type: text/markdown
+
 # AiShell 🤖
 
 [![codecov](https://codecov.io/gh/code-yeongyu/AiShell/branch/master/graph/badge.svg?token=MR72XGUQWJ)](https://codecov.io/gh/code-yeongyu/AiShell)
 [![Release Package to PyPI](https://github.com/code-yeongyu/AiShell/actions/workflows/release.yml/badge.svg)](https://github.com/code-yeongyu/AiShell/actions/workflows/release.yml)
 [![PyPI version](https://badge.fury.io/py/aishell.svg)](https://badge.fury.io/py/aishell)
 [![Downloads](https://static.pepy.tech/personalized-badge/aishell?period=month&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/aishell)
 
@@ -45,22 +60,23 @@
 
 ## Advanced Settings 🛠
 
 By default, `AiShell` is configured to use the reverse-engineered ChatGPT client and retrieve login information from your browser, so you don't need to configure anything to use `AiShell`. However, for those who want to use different models with an OpenAI API Key, you can configure it as follows:
 
 1. Create an account on OpenAI.
 1. Go to <https://platform.openai.com/account/api-keys> and copy your API key.
-1. Modify or create the `~/.aishell_config.json` file as follows:
+1. Modify or create the `~/.ygka_openai_config.json` file as follows:
 
   ```json
   {
       ...
-      "language_model": <language model of your preference>, //"official_chatgpt" or "gpt3"
-      "openai_api_key": <your OpenAI API key>
+      "language_model": "official_chatgpt",
+      "openai_api_key": "<your OpenAI API key>"
   }
   ```
 
-Here, you can specify the language model of your preference, such as "official_chatgpt" or "gpt3", and add your OpenAI API key. This will enable AiShell to use the specified language model and API key when executing commands.
+Here, you can add your OpenAI API key. This will enable AiShell to use the official chatgpt api and the API key when executing commands.
 
 ## Contributions 💬
 
 Feel free to contribute to `AiShell` by adding more functionality or fixing bugs.
+
```

### Comparing `aishell-2023.4.11/pyproject.toml` & `aishell-2023.4.16/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "aishell"
-version = "2023.04.11"
+version = "2023.04.16"
 description = ""
 authors = []
 readme = "README.md"
 
 [tool.pyright]
 typeCheckingMode = "strict"
 pythonPlatform = "All"
@@ -27,26 +27,24 @@
 spaces_before_comment = 2
 split_before_logical_operator = true
 column_limit = 119
 allow_split_before_dict_value = false
 
 [tool.ruff]
 line-length = 119
-select = [ "PLE", "PLR", "PLW", "E", "W", "F", "I", "Q", "C", "B",]
+select = [ "PLE", "PLW", "E", "W", "F", "I", "Q",]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 poetry = "^1.4.0"
-revchatgpt = "^4.1.6"
-openai = "^0.27.4"
-pydantic = "^1.10.5"
-yt-dlp = "^2023.3.3"
+ygka = "^2023.4.16.post1"
+revchatgptauth = "^2023.4.16"
 
 [tool.poetry.scripts]
-aishell = "aishell:main"
+ygka = "ygka:main"
 
 [tool.ruff.flake8-quotes]
 inline-quotes = "single"
 docstring-quotes = "single"
 multiline-quotes = "single"
 
 [tool.pytest.ini_options]
@@ -54,15 +52,16 @@
 
 [tool.poetry.dependencies.typer]
 extras = [ "all",]
 version = "^0.7.0"
 
 [tool.poetry.group.dev.dependencies]
 toml = "^0.10.2"
+types-toml = "^0.10.8.6"
+invoke = "^2.0.0"
+types-invoke = "^2.0.0.6"
+ruff = "^0.0.261"
 yapf = "^0.32.0"
+pyright = "^1.1.302"
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
-invoke = "^1.7.3"
-ruff = "^0.0.199"
-types-invoke = "^1.7.3.16"
-types-toml = "^0.10.8.5"
-pyright = "^1.1.296"
+pytest-sugar = "^0.9.7"
```

