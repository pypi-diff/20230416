# Comparing `tmp/mylearn-0.0.2.tar.gz` & `tmp/mylearn-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mylearn-0.0.2.tar", max compression
+gzip compressed data, was "mylearn-0.0.3.tar", max compression
```

## Comparing `mylearn-0.0.2.tar` & `mylearn-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1071 2021-04-10 10:35:20.221948 mylearn-0.0.2/LICENSE
--rw-r--r--   0        0        0     2806 2022-10-30 12:22:45.911536 mylearn-0.0.2/README.md
--rw-r--r--   0        0        0        0 2021-04-10 10:19:02.727911 mylearn-0.0.2/mylearn/__init__.py
--rw-r--r--   0        0        0     4700 2022-10-30 12:27:31.945805 mylearn-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3643 1970-01-01 00:00:00.000000 mylearn-0.0.2/setup.py
--rw-r--r--   0        0        0     3532 1970-01-01 00:00:00.000000 mylearn-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2021-04-10 10:35:20.221948 mylearn-0.0.3/LICENSE
+-rw-r--r--   0        0        0     3791 2023-04-16 19:32:45.591184 mylearn-0.0.3/README.md
+-rw-r--r--   0        0        0        0 2021-04-10 10:19:02.727911 mylearn-0.0.3/mylearn/__init__.py
+-rw-r--r--   0        0        0     6079 2023-04-16 19:32:45.595184 mylearn-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4998 1970-01-01 00:00:00.000000 mylearn-0.0.3/PKG-INFO
```

### Comparing `mylearn-0.0.2/LICENSE` & `mylearn-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mylearn-0.0.2/README.md` & `mylearn-0.0.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -14,45 +14,81 @@
 [Airflow](https://github.com/apache/airflow) and [MLflow](https://github.com/mlflow/mlflow) for designing machine
 learning systems in a production perspective.
 
 **Work in progress... Stay tuned!**
 
 # Index
 
-1. [Prerequisites](#prerequisites)
+1. [Recommended prerequisites](#prerequisites)
 2. [Installation & Setup](#installation-setup)
 3. [Usage](#usage)
 
-# Prerequisites
+# Recommended prerequisites
+
+## Git
+
+```commandline
+sudo apt-get install git
+```
 
 ## pyenv
 
-To be completed with how to install and setup pyenv
+Install [binary dependencies and build tools](https://github.com/pyenv/pyenv/wiki#suggested-build-environment):
+```commandline
+sudo apt update
+sudo apt install build-essential libssl-dev zlib1g-dev libbz2-dev libreadline-dev libsqlite3-dev curl libncursesw5-dev xz-utils tk-dev libxml2-dev libxmlsec1-dev libffi-dev liblzma-dev
+```
+
+Install pyenv:
+```commandline
+curl https://pyenv.run | bash
+echo 'export PATH="$HOME/.pyenv/bin:$PATH"' >> ~/.bashrc
+echo 'eval "$(pyenv init -)"' >> ~/.bashrc
+echo 'eval "$(pyenv virtualenv-init -)"' >> ~/.bashrc
+source ~/.bashrc
+```
+
+Install a Python version and set it as default:
+```commandline
+pyenv install 3.11.2
+pyenv global 3.11.2
+```
 
 ## poetry
 
-To be completed with how to install and setup poetry
+```commandline
+curl -sSL https://install.python-poetry.org | python3 -
+echo 'export PATH="~/.local/bin:$PATH"' >> ~/.bashrc
+```
 
 # Installation & Setup
 
 mylearn leverages [poetry](https://github.com/python-poetry/poetry) and [poethepoet](https://github.com/nat-n/poethepoet)
 to make its installation and setup surprisingly simple.
 
 ## Installation
 
-It is recommended to install requirements within a virtualenv located at the project root level, although not required.
+It is recommended to install requirements within a `virtualenv` located at the project root level, although not required.
 ```commandline
 poetry config virtualenvs.in-project true
 ```
 
-Installation is run with
+Installation is run with:
 ```commandline
 poetry install
 ```
 
+Should you install from the `requirements.txt` file instead of the `poetry.lock` file:
+```commandline
+pyenv shell 3.11.2
+python -m venv .venv
+source .venv/bin/activate
+pip install -r requirements.txt
+```
+
 ## Airflow Setup
 
 Airflow setup is initialized via a `poe` command
 ```commandline
 poe airflow-init
 ```
```

#### html2text {}

```diff
@@ -3,31 +3,44 @@
  pyversions/mylearn.svg] [https://img.shields.io/pypi/l/mylearn.svg] [https://
        github.com/MichaelKarpe/mylearn/workflows/ci/badge.svg] [https://
               img.shields.io/badge/code%20style-black-000000.svg]
 ___ [mylearn](https://github.com/MichaelKarpe/mylearn) is a Machine Learning
 framework based on [Airflow](https://github.com/apache/airflow) and [MLflow]
 (https://github.com/mlflow/mlflow) for designing machine learning systems in a
 production perspective. **Work in progress... Stay tuned!** # Index 1.
-[Prerequisites](#prerequisites) 2. [Installation & Setup](#installation-setup)
-3. [Usage](#usage) # Prerequisites ## pyenv To be completed with how to install
-and setup pyenv ## poetry To be completed with how to install and setup poetry
-# Installation & Setup mylearn leverages [poetry](https://github.com/python-
-poetry/poetry) and [poethepoet](https://github.com/nat-n/poethepoet) to make
-its installation and setup surprisingly simple. ## Installation It is
-recommended to install requirements within a virtualenv located at the project
-root level, although not required. ```commandline poetry config virtualenvs.in-
-project true ``` Installation is run with ```commandline poetry install ``` ##
-Airflow Setup Airflow setup is initialized via a `poe` command ```commandline
-poe airflow-init ``` Airflow Scheduler & Webserver can be run with
-```commandline poe airflow-scheduler poe airflow-webserver ``` Airflow UI can
-be opened at [localhost](0.0.0.0:8080) (port 8080), and you can login with
-username and password `admin`. If you want to clean your Airflow setup before
-rerunning `poe airflow-init`, you need to kill Airflow Scheduler & Webserver
-and run ```commandline poe airflow-clean ``` ## MLflow Setup MLflow UI can be
-opened at [localhost](0.0.0.0:5000) (port 5000) after execution of the
-following command: ```commandline poe mlflow-ui ``` # Usage ## MLflow Pipelines
-Regression Template The *mlflow-template* pipeline, based on the [MLflow
-Pipelines Regression Template](https://github.com/mlflow/mlp-regression-
-template), can be run independently with ```commandline poe mlflow-run ``` or
-via an Airflow Directed Acyclic Graph (DAG) by triggering the *mlflow-template*
-DAG via Airflow UI or with ```commandline TO BE COMPLETED ``` ## Other examples
-**Work in progress... Stay tuned!**
+[Recommended prerequisites](#prerequisites) 2. [Installation & Setup]
+(#installation-setup) 3. [Usage](#usage) # Recommended prerequisites ## Git
+```commandline sudo apt-get install git ``` ## pyenv Install [binary
+dependencies and build tools](https://github.com/pyenv/pyenv/wiki#suggested-
+build-environment): ```commandline sudo apt update sudo apt install build-
+essential libssl-dev zlib1g-dev libbz2-dev libreadline-dev libsqlite3-dev curl
+libncursesw5-dev xz-utils tk-dev libxml2-dev libxmlsec1-dev libffi-dev liblzma-
+dev ``` Install pyenv: ```commandline curl https://pyenv.run | bash echo
+'export PATH="$HOME/.pyenv/bin:$PATH"' >> ~/.bashrc echo 'eval "$(pyenv init -
+)"' >> ~/.bashrc echo 'eval "$(pyenv virtualenv-init -)"' >> ~/.bashrc source
+~/.bashrc ``` Install a Python version and set it as default: ```commandline
+pyenv install 3.11.2 pyenv global 3.11.2 ``` ## poetry ```commandline curl -sSL
+https://install.python-poetry.org | python3 - echo 'export PATH="~/.local/bin:
+$PATH"' >> ~/.bashrc ``` # Installation & Setup mylearn leverages [poetry]
+(https://github.com/python-poetry/poetry) and [poethepoet](https://github.com/
+nat-n/poethepoet) to make its installation and setup surprisingly simple. ##
+Installation It is recommended to install requirements within a `virtualenv`
+located at the project root level, although not required. ```commandline poetry
+config virtualenvs.in-project true ``` Installation is run with: ```commandline
+poetry install ``` Should you install from the `requirements.txt` file instead
+of the `poetry.lock` file: ```commandline pyenv shell 3.11.2 python -m venv
+.venv source .venv/bin/activate pip install -r requirements.txt ``` ## Airflow
+Setup Airflow setup is initialized via a `poe` command ```commandline poe
+airflow-init ``` Airflow Scheduler & Webserver can be run with ```commandline
+poe airflow-scheduler poe airflow-webserver ``` Airflow UI can be opened at
+[localhost](0.0.0.0:8080) (port 8080), and you can login with username and
+password `admin`. If you want to clean your Airflow setup before rerunning `poe
+airflow-init`, you need to kill Airflow Scheduler & Webserver and run
+```commandline poe airflow-clean ``` ## MLflow Setup MLflow UI can be opened at
+[localhost](0.0.0.0:5000) (port 5000) after execution of the following command:
+```commandline poe mlflow-ui ``` # Usage ## MLflow Pipelines Regression
+Template The *mlflow-template* pipeline, based on the [MLflow Pipelines
+Regression Template](https://github.com/mlflow/mlp-regression-template), can be
+run independently with ```commandline poe mlflow-run ``` or via an Airflow
+Directed Acyclic Graph (DAG) by triggering the *mlflow-template* DAG via
+Airflow UI or with ```commandline TO BE COMPLETED ``` ## Other examples **Work
+in progress... Stay tuned!**
```

### Comparing `mylearn-0.0.2/pyproject.toml` & `mylearn-0.0.3/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,117 +1,146 @@
 [tool.poetry]
 name = "mylearn"
-version = "0.0.2"
+version = "0.0.3"
 description = "mylearn: my Machine Learning framework"
 license = "MIT"
 authors = [
     "Michael Karpe <michael.karpe@berkeley.edu>"
 ]
 readme = "README.md"
 repository = "https://github.com/MichaelKarpe/mylearn"
-homepage = ""
+homepage = "https://github.com/MichaelKarpe/mylearn"
 keywords = ["airflow", "mlflow"]
 classifiers = [
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11"
 ]
 
 [tool.poetry.dependencies]
-python = "^3.11,<3.12"  # Compatible python versions must be declared here
-apache-airflow = {version = "^2.4.2", extras = ["postgres"]}
-# mlflow = {version = "^1.30.0", extras = ["pipelines"]}
-pandas = "^1.5.1"
+python = "^3.8,<3.12"  # Compatible python versions must be declared here
+apache-airflow = {version = "^2.5.3", extras = ["postgres"]}
+llvmlite = "^0.40.0rc1"
+numba = "^0.57.0rc1"
+mlflow = {version = "^2.2.2", extras = ["pipelines"]}
+pandas = "^1.5.3"
+polars = "^0.17.3"
 psycopg2 = "^2.9.5"
 
 [tool.poetry.group.clustering.dependencies]
-# k-means-constrained = "^0.7.2"
+k-means-constrained = "^0.7.2"
 
 [tool.poetry.group.compvis.dependencies]
-opencv-python = "^4.6.0.66"
-# scikit-image = "^0.19.3"
+opencv-python = "^4.7.0.72"
+# scikit-image = "^0.20.0"
 
 [tool.poetry.group.dl.dependencies]
-keras = "^2.10.0"
-# tensorflow = "^2.10.0"
-# transformers = "^4.23.1"
+torch = "^2.0.0"
+accelerate = "^0.18.0"
+transformers = "^4.28.1"
 
 [tool.poetry.group.geo.dependencies]
 geopandas = "^0.11.1"
 
 [tool.poetry.group.gbms.dependencies]
-# catboost = "^1.1"
-lightgbm = "^3.3.3"
-xgboost = "^1.6.2"
+lightgbm = "^3.3.5"
+xgboost = "1.7.3"
+
+[tool.poetry.group.linux.dependencies]
+nmcli = "^1.2.0"
+
+[tool.poetry.group.misc.dependencies]
+youtube-transcript-api = "^0.5.0"
 
 [tool.poetry.group.ml.dependencies]
 hyperopt = "^0.2.7"
-mapie = "^0.4.2"
-scikit-learn = "^1.1.2"
+mapie = "^0.6.3"
+optuna = "^3.1.0"
+scikit-learn = "^1.2.2"
 
 [tool.poetry.group.nlp.dependencies]
-spacy = "^3.4.2"
+spacy = "^3.5.1"
+sentencepiece = "^0.1.97"
 
 [tool.poetry.group.plotting.dependencies]
 matplotlib = "^3.6.0"
 plotly = "^5.10.0"
 seaborn = "^0.12.1"
 
 [tool.poetry.group.sci.dependencies]
-scipy = "^1.9.3"
+scipy = "^1.10.1"
 fastcluster = "^1.2.6"
 
 [tool.poetry.group.scraping.dependencies]
 beautifulsoup4 = "^4.11.1"
 requests = "^2.28.1"
+scrapy = "^2.8.0"
 
 [tool.poetry.group.stats.dependencies]
-# statsmodels = "^0.13.2"
+# statsmodels = "^0.13.5"
+statsforecast = "^1.5.0"
+
+[tool.poetry.group.timeseries.dependencies]
+arch = "^5.3.1"
+# neuralprophet = "^0.5.4"
+prophet = "^1.1.2"
+sktime = "^0.16.1"
 
 [tool.poetry.group.qfinance.dependencies]
-empyrical = "^0.5.5"
-# tslearn = "^0.5.2"
+alphalens-reloaded = "^0.4.3"
+empyrical-reloaded = "^0.5.9"
+pyfolio-reloaded = "^0.9.5"
+pyod = "^1.0.9"
+quantstats = "^0.0.59"
 
 [tool.poetry.group.qscraping.dependencies]
 yfinance = "^0.1.79"
 
 [tool.poetry.dev-dependencies]
-black = {version = "^22.6", extras = ["jupyter"]}
+black = {version = "^23.1.0", extras = ["jupyter"]}
 flake8 = "^5.0.4"
 ipython-autotime = "^0.3.1"
 isort = "^5.10.1"
 jupyterlab = "^3.4.5"
-mypy = "^0.982"
-# pandas-stubs = "^1.5.0.221012"
-pip = "^22.2.2"
+mypy = "^1.1.1"
+pandas-stubs = "^1.5.3.230304"
+pip = "^23.0.1"
 poethepoet = "^0.16.0"
 pre-commit = "^2.20.0"
 pylint = "^2.15"
 pytest = "^7.1.2"
 pytest-cov = "^3.0"
 types-requests = "^2.28.11.1"
+tox = "^4.4.7"
+tox-gh-actions = "^3.1.0"
 
 [tool.poe.env]
-AIRFLOW_HOME = "${PWD}/airflow"
+AIRFLOW_HOME = "${PWD}/mlairflow"
 AIRFLOW__CORE__LOAD_EXAMPLES = "false"
 AIRFLOW__CORE__DEFAULT_TIMEZONE = "Europe/Amsterdam"
 AIRFLOW__CORE__EXECUTOR = "LocalExecutor"
 AIRFLOW__CORE__MAX_ACTIVE_RUNS_PER_DAG = "1"
-AIRFLOW__CORE__MAX_ACTIVE_TASKS_PER_DAG = "64"
+AIRFLOW__CORE__MAX_ACTIVE_TASKS_PER_DAG = "1"
 AIRFLOW__CORE__MAX_MAP_LENGTH = "65536"
-AIRFLOW__CORE__PARALLELISM = "64"
+AIRFLOW__CORE__PARALLELISM = "1"
 AIRFLOW__DATABASE__SQL_ALCHEMY_CONN = "postgresql+psycopg2://airflow:airflow@localhost/airflow"
 AIRFLOW__SCHEDULER__CATCHUP_BY_DEFAULT = "False"
-CODE_FOLDERS = "airflow/dags mylearn"  # mlflow tests
-MLFLOW_PIPELINES_PROFILE = "local"
+AIRFLOW__SCHEDULER__PARSING_PROCESSES = "1"
+AIRFLOW__SCHEDULER__PRINT_STATS_INTERVAL = "0"
+AIRFLOW__SCHEDULER__SCHEDULER_HEARTBEAT_SEC = "1"
+CODE_FOLDERS = "mlairflow/dags mylearn"  # mlflow tests
+MLFLOW_RECIPES_PROFILE = "local"
 
 [tool.poe.tasks.airflow-clean]
 sequence = [
-    {cmd = "rm -r airflow/logs"},
-    {cmd = "rm airflow/airflow.cfg"},
-    {cmd = "rm airflow/airflow.db"},  # comment this line if Airflow LocalExecutor and database are uncommented above
-    {cmd = "rm airflow/webserver_config.py"},
+    {shell = "rm -r mlairflow/logs"},
+    {shell = "rm mlairflow/airflow.cfg"},
+    {shell = "rm mlairflow/airflow.db"},  # comment this line if Airflow LocalExecutor and database are uncommented above
+    {shell = "rm mlairflow/webserver_config.py"},
 ]
 
 [tool.poe.tasks.airflow-init]
 sequence = [
     {cmd = "airflow db init"},
     {cmd = """
     airflow users create --role Admin --username admin --email admin --firstname admin --lastname admin --password admin
@@ -121,22 +150,23 @@
 [tool.poe.tasks.airflow-scheduler]
 cmd = "airflow scheduler"
 
 [tool.poe.tasks.airflow-webserver]
 cmd = "airflow webserver --port 8080"
 
 [tool.poe.tasks.mlflow-run]
-sequence = [
-    {cmd = "mlflow pipelines run --step ingest"},
-    {cmd = "mlflow pipelines run --step split"},
-    {cmd = "mlflow pipelines run --step transform"},
-    {cmd = "mlflow pipelines run --step train"},
-    {cmd = "mlflow pipelines run --step evaluate"},
-    {cmd = "mlflow pipelines run --step register"},
-]
+shell = """
+cd mlairflow
+mlflow recipes run --step ingest --profile $MLFLOW_RECIPES_PROFILE
+mlflow recipes run --step split --profile $MLFLOW_RECIPES_PROFILE
+mlflow recipes run --step transform --profile $MLFLOW_RECIPES_PROFILE
+mlflow recipes run --step train --profile $MLFLOW_RECIPES_PROFILE
+mlflow recipes run --step evaluate --profile $MLFLOW_RECIPES_PROFILE
+mlflow recipes run --step register --profile $MLFLOW_RECIPES_PROFILE
+"""
 
 [tool.poe.tasks.mlflow-ui]
 cmd = """
 mlflow ui \
    --backend-store-uri sqlite:///metadata/mlflow/mlruns.db \
    --default-artifact-root ./metadata/mlflow/mlartifacts \
    --host localhost
@@ -175,10 +205,36 @@
     {cmd = "poe mypy"},
     # {cmd = "poe test"}
 ]
 
 [tool.black]
 line-length = 120
 
+[tool.tox]
+legacy_tox_ini = """
+[tox]
+envlist = py{38,39,310,311}-{linux,macos,windows}
+isolated_build = true
+
+[gh-actions]
+python =
+    3.8: py38
+    3.9: py39
+    3.10: py310
+    3.11: py311
+
+[gh-actions:env]
+PLATFORM =
+    ubuntu-latest: linux
+    macos-latest: macos
+    windows-latest: windows
+
+[testenv]
+skip_install = true
+allowlist_externals = poetry
+commands_pre = poetry install
+commands = poetry run pytest tests
+"""
+
 [build-system]
-requires = ["poetry-core>=1.3.2"]
+requires = ["poetry-core>=1.5.2"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `mylearn-0.0.2/PKG-INFO` & `mylearn-0.0.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,33 @@
 Metadata-Version: 2.1
 Name: mylearn
-Version: 0.0.2
+Version: 0.0.3
 Summary: mylearn: my Machine Learning framework
 Home-page: https://github.com/MichaelKarpe/mylearn
 License: MIT
 Keywords: airflow,mlflow
 Author: Michael Karpe
 Author-email: michael.karpe@berkeley.edu
-Requires-Python: >=3.11,<3.12
+Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: apache-airflow[postgres] (>=2.4.2,<3.0.0)
-Requires-Dist: pandas (>=1.5.1,<2.0.0)
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: apache-airflow[postgres] (>=2.5.3,<3.0.0)
+Requires-Dist: llvmlite (>=0.40.0rc1,<0.41.0)
+Requires-Dist: mlflow[pipelines] (>=2.2.2,<3.0.0)
+Requires-Dist: numba (>=0.57.0rc1,<0.58.0)
+Requires-Dist: pandas (>=1.5.3,<2.0.0)
+Requires-Dist: polars (>=0.17.3,<0.18.0)
 Requires-Dist: psycopg2 (>=2.9.5,<3.0.0)
 Project-URL: Repository, https://github.com/MichaelKarpe/mylearn
 Description-Content-Type: text/markdown
 
 <h2 align="center">mylearn: my Machine Learning framework</h2>
 
 <p align="center">
@@ -34,45 +44,81 @@
 [Airflow](https://github.com/apache/airflow) and [MLflow](https://github.com/mlflow/mlflow) for designing machine
 learning systems in a production perspective.
 
 **Work in progress... Stay tuned!**
 
 # Index
 
-1. [Prerequisites](#prerequisites)
+1. [Recommended prerequisites](#prerequisites)
 2. [Installation & Setup](#installation-setup)
 3. [Usage](#usage)
 
-# Prerequisites
+# Recommended prerequisites
+
+## Git
+
+```commandline
+sudo apt-get install git
+```
 
 ## pyenv
 
-To be completed with how to install and setup pyenv
+Install [binary dependencies and build tools](https://github.com/pyenv/pyenv/wiki#suggested-build-environment):
+```commandline
+sudo apt update
+sudo apt install build-essential libssl-dev zlib1g-dev libbz2-dev libreadline-dev libsqlite3-dev curl libncursesw5-dev xz-utils tk-dev libxml2-dev libxmlsec1-dev libffi-dev liblzma-dev
+```
+
+Install pyenv:
+```commandline
+curl https://pyenv.run | bash
+echo 'export PATH="$HOME/.pyenv/bin:$PATH"' >> ~/.bashrc
+echo 'eval "$(pyenv init -)"' >> ~/.bashrc
+echo 'eval "$(pyenv virtualenv-init -)"' >> ~/.bashrc
+source ~/.bashrc
+```
+
+Install a Python version and set it as default:
+```commandline
+pyenv install 3.11.2
+pyenv global 3.11.2
+```
 
 ## poetry
 
-To be completed with how to install and setup poetry
+```commandline
+curl -sSL https://install.python-poetry.org | python3 -
+echo 'export PATH="~/.local/bin:$PATH"' >> ~/.bashrc
+```
 
 # Installation & Setup
 
 mylearn leverages [poetry](https://github.com/python-poetry/poetry) and [poethepoet](https://github.com/nat-n/poethepoet)
 to make its installation and setup surprisingly simple.
 
 ## Installation
 
-It is recommended to install requirements within a virtualenv located at the project root level, although not required.
+It is recommended to install requirements within a `virtualenv` located at the project root level, although not required.
 ```commandline
 poetry config virtualenvs.in-project true
 ```
 
-Installation is run with
+Installation is run with:
 ```commandline
 poetry install
 ```
 
+Should you install from the `requirements.txt` file instead of the `poetry.lock` file:
+```commandline
+pyenv shell 3.11.2
+python -m venv .venv
+source .venv/bin/activate
+pip install -r requirements.txt
+```
+
 ## Airflow Setup
 
 Airflow setup is initialized via a `poe` command
 ```commandline
 poe airflow-init
 ```
```

#### html2text {}

```diff
@@ -1,43 +1,62 @@
-Metadata-Version: 2.1 Name: mylearn Version: 0.0.2 Summary: mylearn: my Machine
+Metadata-Version: 2.1 Name: mylearn Version: 0.0.3 Summary: mylearn: my Machine
 Learning framework Home-page: https://github.com/MichaelKarpe/mylearn License:
 MIT Keywords: airflow,mlflow Author: Michael Karpe Author-email:
-michael.karpe@berkeley.edu Requires-Python: >=3.11,<3.12 Classifier: License ::
+michael.karpe@berkeley.edu Requires-Python: >=3.8,<3.12 Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
-Language :: Python :: 3.11 Requires-Dist: apache-airflow[postgres]
-(>=2.4.2,<3.0.0) Requires-Dist: pandas (>=1.5.1,<2.0.0) Requires-Dist: psycopg2
-(>=2.9.5,<3.0.0) Project-URL: Repository, https://github.com/MichaelKarpe/
-mylearn Description-Content-Type: text/markdown
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Requires-Dist: apache-airflow[postgres]
+(>=2.5.3,<3.0.0) Requires-Dist: llvmlite (>=0.40.0rc1,<0.41.0) Requires-Dist:
+mlflow[pipelines] (>=2.2.2,<3.0.0) Requires-Dist: numba (>=0.57.0rc1,<0.58.0)
+Requires-Dist: pandas (>=1.5.3,<2.0.0) Requires-Dist: polars (>=0.17.3,<0.18.0)
+Requires-Dist: psycopg2 (>=2.9.5,<3.0.0) Project-URL: Repository, https://
+github.com/MichaelKarpe/mylearn Description-Content-Type: text/markdown
               ***** mylearn: my Machine Learning framework *****
    [https://img.shields.io/pypi/v/mylearn.svg] [https://img.shields.io/pypi/
  pyversions/mylearn.svg] [https://img.shields.io/pypi/l/mylearn.svg] [https://
        github.com/MichaelKarpe/mylearn/workflows/ci/badge.svg] [https://
               img.shields.io/badge/code%20style-black-000000.svg]
 ___ [mylearn](https://github.com/MichaelKarpe/mylearn) is a Machine Learning
 framework based on [Airflow](https://github.com/apache/airflow) and [MLflow]
 (https://github.com/mlflow/mlflow) for designing machine learning systems in a
 production perspective. **Work in progress... Stay tuned!** # Index 1.
-[Prerequisites](#prerequisites) 2. [Installation & Setup](#installation-setup)
-3. [Usage](#usage) # Prerequisites ## pyenv To be completed with how to install
-and setup pyenv ## poetry To be completed with how to install and setup poetry
-# Installation & Setup mylearn leverages [poetry](https://github.com/python-
-poetry/poetry) and [poethepoet](https://github.com/nat-n/poethepoet) to make
-its installation and setup surprisingly simple. ## Installation It is
-recommended to install requirements within a virtualenv located at the project
-root level, although not required. ```commandline poetry config virtualenvs.in-
-project true ``` Installation is run with ```commandline poetry install ``` ##
-Airflow Setup Airflow setup is initialized via a `poe` command ```commandline
-poe airflow-init ``` Airflow Scheduler & Webserver can be run with
-```commandline poe airflow-scheduler poe airflow-webserver ``` Airflow UI can
-be opened at [localhost](0.0.0.0:8080) (port 8080), and you can login with
-username and password `admin`. If you want to clean your Airflow setup before
-rerunning `poe airflow-init`, you need to kill Airflow Scheduler & Webserver
-and run ```commandline poe airflow-clean ``` ## MLflow Setup MLflow UI can be
-opened at [localhost](0.0.0.0:5000) (port 5000) after execution of the
-following command: ```commandline poe mlflow-ui ``` # Usage ## MLflow Pipelines
-Regression Template The *mlflow-template* pipeline, based on the [MLflow
-Pipelines Regression Template](https://github.com/mlflow/mlp-regression-
-template), can be run independently with ```commandline poe mlflow-run ``` or
-via an Airflow Directed Acyclic Graph (DAG) by triggering the *mlflow-template*
-DAG via Airflow UI or with ```commandline TO BE COMPLETED ``` ## Other examples
-**Work in progress... Stay tuned!**
+[Recommended prerequisites](#prerequisites) 2. [Installation & Setup]
+(#installation-setup) 3. [Usage](#usage) # Recommended prerequisites ## Git
+```commandline sudo apt-get install git ``` ## pyenv Install [binary
+dependencies and build tools](https://github.com/pyenv/pyenv/wiki#suggested-
+build-environment): ```commandline sudo apt update sudo apt install build-
+essential libssl-dev zlib1g-dev libbz2-dev libreadline-dev libsqlite3-dev curl
+libncursesw5-dev xz-utils tk-dev libxml2-dev libxmlsec1-dev libffi-dev liblzma-
+dev ``` Install pyenv: ```commandline curl https://pyenv.run | bash echo
+'export PATH="$HOME/.pyenv/bin:$PATH"' >> ~/.bashrc echo 'eval "$(pyenv init -
+)"' >> ~/.bashrc echo 'eval "$(pyenv virtualenv-init -)"' >> ~/.bashrc source
+~/.bashrc ``` Install a Python version and set it as default: ```commandline
+pyenv install 3.11.2 pyenv global 3.11.2 ``` ## poetry ```commandline curl -sSL
+https://install.python-poetry.org | python3 - echo 'export PATH="~/.local/bin:
+$PATH"' >> ~/.bashrc ``` # Installation & Setup mylearn leverages [poetry]
+(https://github.com/python-poetry/poetry) and [poethepoet](https://github.com/
+nat-n/poethepoet) to make its installation and setup surprisingly simple. ##
+Installation It is recommended to install requirements within a `virtualenv`
+located at the project root level, although not required. ```commandline poetry
+config virtualenvs.in-project true ``` Installation is run with: ```commandline
+poetry install ``` Should you install from the `requirements.txt` file instead
+of the `poetry.lock` file: ```commandline pyenv shell 3.11.2 python -m venv
+.venv source .venv/bin/activate pip install -r requirements.txt ``` ## Airflow
+Setup Airflow setup is initialized via a `poe` command ```commandline poe
+airflow-init ``` Airflow Scheduler & Webserver can be run with ```commandline
+poe airflow-scheduler poe airflow-webserver ``` Airflow UI can be opened at
+[localhost](0.0.0.0:8080) (port 8080), and you can login with username and
+password `admin`. If you want to clean your Airflow setup before rerunning `poe
+airflow-init`, you need to kill Airflow Scheduler & Webserver and run
+```commandline poe airflow-clean ``` ## MLflow Setup MLflow UI can be opened at
+[localhost](0.0.0.0:5000) (port 5000) after execution of the following command:
+```commandline poe mlflow-ui ``` # Usage ## MLflow Pipelines Regression
+Template The *mlflow-template* pipeline, based on the [MLflow Pipelines
+Regression Template](https://github.com/mlflow/mlp-regression-template), can be
+run independently with ```commandline poe mlflow-run ``` or via an Airflow
+Directed Acyclic Graph (DAG) by triggering the *mlflow-template* DAG via
+Airflow UI or with ```commandline TO BE COMPLETED ``` ## Other examples **Work
+in progress... Stay tuned!**
```

