# Comparing `tmp/feed-archiver-1.0.0b11.tar.gz` & `tmp/feed-archiver-2.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feed-archiver-1.0.0b11.tar", last modified: Sat Apr 15 21:33:28 2023, max compression
+gzip compressed data, was "feed-archiver-2.0.0b0.tar", last modified: Sat Apr 15 22:29:47 2023, max compression
```

## Comparing `feed-archiver-1.0.0b11.tar` & `feed-archiver-2.0.0b0.tar`

### file list

```diff
@@ -1,251 +1,250 @@
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      543 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/.dir-locals.el.in
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1661 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/.dockerignore
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1115 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/.env.in
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/.github/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.833655 feed-archiver-1.0.0b11/.github/workflows/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4582 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/.github/workflows/build-test.yml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1661 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/.gitignore
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5189 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/.gitlab-ci.yml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      779 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/.pre-commit-config.yaml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2442 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/.prospector.yaml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4121 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/CONTRIBUTING.rst
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2482 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/Dockerfile
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2747 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/Dockerfile.devel
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1081 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/LICENSE
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    60978 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/Makefile
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      205 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/NEWS-VERSION.rst
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3447 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/NEWS.rst
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)    22912 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/PKG-INFO
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    21851 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/README.rst
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3876 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/TODO.rst
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.833655 feed-archiver-1.0.0b11/bin/
--rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)     2792 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/bin/cz-check-bump
--rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)      936 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/bin/entrypoint
--rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)     1101 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/bin/get-base-version
--rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)      321 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/bin/hadolint
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.833655 feed-archiver-1.0.0b11/build-host/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2002 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/build-host/Dockerfile
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1476 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/build-host/Makefile
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      746 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/build-host/README.rst
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.833655 feed-archiver-1.0.0b11/build-host/bin/
--rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)     2047 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/build-host/bin/entrypoint
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      731 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/build-host/requirements-py310.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      674 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/build-host/requirements-py311.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      948 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/build-host/requirements-py37.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      729 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/build-host/requirements-py38.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      729 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/build-host/requirements-py39.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)        4 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/build-host/requirements.txt.in
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.833655 feed-archiver-1.0.0b11/dist/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      122 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/dist/.gitignore
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      954 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/docker-compose-servarr.yml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5675 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/docker-compose.override.yml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      927 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/docker-compose.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.833655 feed-archiver-1.0.0b11/gitlab-runner/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       46 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/gitlab-runner/.gitignore
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.833655 feed-archiver-1.0.0b11/gitlab-runner/config/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1323 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/gitlab-runner/config/config.toml.in
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.833655 feed-archiver-1.0.0b11/home/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       64 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/home/.gitignore
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      327 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/home/.pypirc.in
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      111 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/link-fallbacks.feature.rst
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/nginx/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.833655 feed-archiver-1.0.0b11/nginx/templates/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1086 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/nginx/templates/default.conf.template
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2941 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/pyproject.toml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.833655 feed-archiver-1.0.0b11/requirements/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      578 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/requirements/build.txt.in
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.833655 feed-archiver-1.0.0b11/requirements/py310/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2414 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/requirements/py310/build.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     6331 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/requirements/py310/devel.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1183 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/requirements/py310/user.txt
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.833655 feed-archiver-1.0.0b11/requirements/py311/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2414 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/requirements/py311/build.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     6082 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/requirements/py311/devel.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1183 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/requirements/py311/user.txt
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.833655 feed-archiver-1.0.0b11/requirements/py37/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2645 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/requirements/py37/build.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     7030 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/requirements/py37/devel.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1530 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/requirements/py37/user.txt
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.833655 feed-archiver-1.0.0b11/requirements/py38/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2515 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/requirements/py38/build.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     6371 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/requirements/py38/devel.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1181 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/requirements/py38/user.txt
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.833655 feed-archiver-1.0.0b11/requirements/py39/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2412 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/requirements/py39/build.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     6358 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/requirements/py39/devel.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1181 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/requirements/py39/user.txt
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.833655 feed-archiver-1.0.0b11/server/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4397 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/server/docker-compose.yml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2120 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/setup.cfg
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.833655 feed-archiver-1.0.0b11/src/feed_archiver.egg-info/
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)    22912 2023-04-15 21:33:28.000000 feed-archiver-1.0.0b11/src/feed_archiver.egg-info/PKG-INFO
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     7365 2023-04-15 21:33:28.000000 feed-archiver-1.0.0b11/src/feed_archiver.egg-info/SOURCES.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)        1 2023-04-15 21:33:28.000000 feed-archiver-1.0.0b11/src/feed_archiver.egg-info/dependency_links.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      277 2023-04-15 21:33:28.000000 feed-archiver-1.0.0b11/src/feed_archiver.egg-info/entry_points.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      345 2023-04-15 21:33:28.000000 feed-archiver-1.0.0b11/src/feed_archiver.egg-info/requires.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)       13 2023-04-15 21:33:28.000000 feed-archiver-1.0.0b11/src/feed_archiver.egg-info/top_level.txt
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.833655 feed-archiver-1.0.0b11/src/feedarchiver/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5287 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/__init__.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      201 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/__main__.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    11802 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/archive.py
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.833655 feed-archiver-1.0.0b11/src/feedarchiver/enclosures/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3371 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/enclosures/__init__.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     8155 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/enclosures/servarr.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1968 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/enclosures/template.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    34925 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/feed.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     7074 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/formats.py
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.833655 feed-archiver-1.0.0b11/src/feedarchiver/newsfragments/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       91 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/newsfragments/.gitignore
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       58 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/newsfragments/request-timeouts.fix.rst
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.833655 feed-archiver-1.0.0b11/src/feedarchiver/tests/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     9888 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/__init__.py
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/archives/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.833655 feed-archiver-1.0.0b11/src/feedarchiver/tests/archives/downloads/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1349 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/archives/downloads/.feed-archiver.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.833655 feed-archiver-1.0.0b11/src/feedarchiver/tests/archives/empty/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       32 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/archives/empty/.gitignore
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/archives/empty-feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       60 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/archives/empty-feeds/.feed-archiver.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/archives/empty-items/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      337 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/archives/empty-items/.feed-archiver.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/archives/end-to-end/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      962 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/archives/end-to-end/.feed-archiver.yml.in
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/archives/relink/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      936 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/archives/relink/.feed-archiver.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/archives/relink-wo-suffix/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      932 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/archives/relink-wo-suffix/.feed-archiver.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/archives/simple/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      228 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/archives/simple/.feed-archiver.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/http/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      243 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/episode%3Fapikey=secret%26seriesId=7
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      224 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/episodeFile%3Fapikey=secret%26seriesId=7
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/series/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       91 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/series/7%3Fapikey=secret
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      105 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/series%3Fapikey=secret
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/common-id.mp3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/el-ni%25C3%25B1o.mp3
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/common-id.mp3
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/download.mp3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/index.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/download
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3435 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/el-ni%25C3%25B1o.png
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/index.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/fred-episode-title/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/fred-episode-title/download
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/garply-bonus-episode/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/garply-bonus-episode/download.mp3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5617 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/feed.rss
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3435 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/image.png
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/index.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/empty-items/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/empty-items/orig/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/empty-items/orig/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/empty-items/orig/https/foo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/empty-items/orig/https/foo.example.com/podcast/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      405 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/empty-items/orig/https/foo.example.com/podcast/empty.rss
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/added-item/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/added-item/http/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/1
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/2
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/main.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/added-item/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1186 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/feeds/waldo
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/empty/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/empty/http/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/1
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/2
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/main.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/empty/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/empty/https/foo-username%3Asecret@grault.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/empty/https/foo-username%3Asecret@grault.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       92 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/empty/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/feeds/waldo
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/orig/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/orig/http/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/1
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/2
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/main.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/orig/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      831 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/feeds/waldo
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/removed-item/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/removed-item/http/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/1
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/2
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/main.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/removed-item/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      841 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/feeds/waldo
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/reordered-item/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/reordered-item/http/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/1
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/2
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/main.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/reordered-item/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1550 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.829655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 21:33:28.837655 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-15 21:28:30.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/waldo
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3286 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/test_archive.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4257 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/test_cli.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    10833 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/test_download.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    15051 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/test_feed.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     7436 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/test_linking.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2165 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/tests/test_urls.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     8147 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/src/feedarchiver/utils.py
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      163 2023-04-15 21:33:28.000000 feed-archiver-1.0.0b11/src/feedarchiver/version.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3362 2023-04-15 21:32:20.000000 feed-archiver-1.0.0b11/tox.ini
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.214660 feed-archiver-2.0.0b0/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      543 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/.dir-locals.el.in
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1661 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/.dockerignore
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1115 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/.env.in
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.202660 feed-archiver-2.0.0b0/.github/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/.github/workflows/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3944 2023-04-15 21:45:16.000000 feed-archiver-2.0.0b0/.github/workflows/build-test.yml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1661 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/.gitignore
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4472 2023-04-15 21:45:16.000000 feed-archiver-2.0.0b0/.gitlab-ci.yml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      779 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/.pre-commit-config.yaml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2442 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/.prospector.yaml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4121 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/CONTRIBUTING.rst
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2482 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/Dockerfile
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2747 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/Dockerfile.devel
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1081 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/LICENSE
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    61264 2023-04-15 22:18:59.000000 feed-archiver-2.0.0b0/Makefile
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      205 2023-04-15 22:20:07.000000 feed-archiver-2.0.0b0/NEWS-VERSION.rst
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3823 2023-04-15 22:20:08.000000 feed-archiver-2.0.0b0/NEWS.rst
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)    22909 2023-04-15 22:29:47.214660 feed-archiver-2.0.0b0/PKG-INFO
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    21849 2023-04-15 21:45:16.000000 feed-archiver-2.0.0b0/README.rst
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3758 2023-04-15 21:45:16.000000 feed-archiver-2.0.0b0/TODO.rst
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/bin/
+-rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)     2792 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/bin/cz-check-bump
+-rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)      936 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/bin/entrypoint
+-rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)     1101 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/bin/get-base-version
+-rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)      321 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/bin/hadolint
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/build-host/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2002 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/build-host/Dockerfile
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1476 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/build-host/Makefile
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      746 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/build-host/README.rst
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/build-host/bin/
+-rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)     2047 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/build-host/bin/entrypoint
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      731 2023-04-15 22:20:35.000000 feed-archiver-2.0.0b0/build-host/requirements-py310.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      674 2023-04-15 22:20:35.000000 feed-archiver-2.0.0b0/build-host/requirements-py311.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      948 2023-04-15 22:20:35.000000 feed-archiver-2.0.0b0/build-host/requirements-py37.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      729 2023-04-15 22:20:35.000000 feed-archiver-2.0.0b0/build-host/requirements-py38.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      729 2023-04-15 22:20:35.000000 feed-archiver-2.0.0b0/build-host/requirements-py39.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)        4 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/build-host/requirements.txt.in
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/dist/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      122 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/dist/.gitignore
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      954 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/docker-compose-servarr.yml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5675 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/docker-compose.override.yml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      927 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/docker-compose.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/gitlab-runner/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       46 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/gitlab-runner/.gitignore
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/gitlab-runner/config/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1323 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/gitlab-runner/config/config.toml.in
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/home/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       64 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/home/.gitignore
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      327 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/home/.pypirc.in
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      111 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/link-fallbacks.feature.rst
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/nginx/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/nginx/templates/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1086 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/nginx/templates/default.conf.template
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2940 2023-04-15 22:20:09.000000 feed-archiver-2.0.0b0/pyproject.toml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/requirements/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      578 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/requirements/build.txt.in
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/requirements/py310/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2414 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/requirements/py310/build.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     6384 2023-04-15 22:20:35.000000 feed-archiver-2.0.0b0/requirements/py310/devel.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1140 2023-04-15 22:20:35.000000 feed-archiver-2.0.0b0/requirements/py310/user.txt
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/requirements/py311/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2414 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/requirements/py311/build.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     6135 2023-04-15 22:20:35.000000 feed-archiver-2.0.0b0/requirements/py311/devel.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1140 2023-04-15 22:20:35.000000 feed-archiver-2.0.0b0/requirements/py311/user.txt
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/requirements/py37/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2645 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/requirements/py37/build.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     7083 2023-04-15 22:20:35.000000 feed-archiver-2.0.0b0/requirements/py37/devel.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1487 2023-04-15 22:20:35.000000 feed-archiver-2.0.0b0/requirements/py37/user.txt
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/requirements/py38/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2515 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/requirements/py38/build.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     6424 2023-04-15 22:20:35.000000 feed-archiver-2.0.0b0/requirements/py38/devel.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1138 2023-04-15 22:20:35.000000 feed-archiver-2.0.0b0/requirements/py38/user.txt
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/requirements/py39/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2412 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/requirements/py39/build.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     6411 2023-04-15 22:20:35.000000 feed-archiver-2.0.0b0/requirements/py39/devel.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1138 2023-04-15 22:20:35.000000 feed-archiver-2.0.0b0/requirements/py39/user.txt
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/server/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4397 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/server/docker-compose.yml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2136 2023-04-15 22:29:47.214660 feed-archiver-2.0.0b0/setup.cfg
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/src/feed_archiver.egg-info/
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)    22909 2023-04-15 22:29:47.000000 feed-archiver-2.0.0b0/src/feed_archiver.egg-info/PKG-INFO
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     7309 2023-04-15 22:29:47.000000 feed-archiver-2.0.0b0/src/feed_archiver.egg-info/SOURCES.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)        1 2023-04-15 22:29:47.000000 feed-archiver-2.0.0b0/src/feed_archiver.egg-info/dependency_links.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      277 2023-04-15 22:29:47.000000 feed-archiver-2.0.0b0/src/feed_archiver.egg-info/entry_points.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      360 2023-04-15 22:29:47.000000 feed-archiver-2.0.0b0/src/feed_archiver.egg-info/requires.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)       13 2023-04-15 22:29:47.000000 feed-archiver-2.0.0b0/src/feed_archiver.egg-info/top_level.txt
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/src/feedarchiver/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5287 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/src/feedarchiver/__init__.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      201 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/__main__.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    11802 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/src/feedarchiver/archive.py
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/src/feedarchiver/enclosures/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3371 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/src/feedarchiver/enclosures/__init__.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     8155 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/src/feedarchiver/enclosures/servarr.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1968 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/src/feedarchiver/enclosures/template.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    34925 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/src/feedarchiver/feed.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     7074 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/src/feedarchiver/formats.py
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/src/feedarchiver/newsfragments/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       91 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/newsfragments/.gitignore
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/src/feedarchiver/tests/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     9888 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/__init__.py
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/archives/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/src/feedarchiver/tests/archives/downloads/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1349 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/archives/downloads/.feed-archiver.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/src/feedarchiver/tests/archives/empty/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       32 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/archives/empty/.gitignore
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/src/feedarchiver/tests/archives/empty-feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       60 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/archives/empty-feeds/.feed-archiver.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/src/feedarchiver/tests/archives/empty-items/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      337 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/archives/empty-items/.feed-archiver.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/src/feedarchiver/tests/archives/end-to-end/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      962 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/archives/end-to-end/.feed-archiver.yml.in
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/src/feedarchiver/tests/archives/relink/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      936 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/archives/relink/.feed-archiver.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/src/feedarchiver/tests/archives/relink-wo-suffix/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      932 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/archives/relink-wo-suffix/.feed-archiver.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/src/feedarchiver/tests/archives/simple/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      228 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/archives/simple/.feed-archiver.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/http/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      243 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/episode%3Fapikey=secret%26seriesId=7
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      224 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/episodeFile%3Fapikey=secret%26seriesId=7
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/series/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       91 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/series/7%3Fapikey=secret
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      105 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/series%3Fapikey=secret
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/common-id.mp3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/el-ni%25C3%25B1o.mp3
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/common-id.mp3
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/download.mp3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/index.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/download
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3435 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/el-ni%25C3%25B1o.png
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/index.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/fred-episode-title/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/fred-episode-title/download
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/garply-bonus-episode/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/garply-bonus-episode/download.mp3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5617 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/feed.rss
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3435 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/image.png
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/index.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/empty-items/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/empty-items/orig/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/empty-items/orig/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/empty-items/orig/https/foo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/empty-items/orig/https/foo.example.com/podcast/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      405 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/empty-items/orig/https/foo.example.com/podcast/empty.rss
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/added-item/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/added-item/http/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.214660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.214660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/1
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/2
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/main.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/added-item/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.214660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1186 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.214660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/feeds/waldo
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/empty/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/empty/http/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.214660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.214660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/1
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/2
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/main.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/empty/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/empty/https/foo-username%3Asecret@grault.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.214660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/empty/https/foo-username%3Asecret@grault.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       92 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/empty/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.214660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/feeds/waldo
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/orig/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/orig/http/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.214660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.214660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/1
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/2
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/main.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/orig/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.214660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      831 1980-11-25 08:31:00.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.214660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/feeds/waldo
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/removed-item/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/removed-item/http/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.214660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.214660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/1
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/2
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/main.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/removed-item/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.214660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      841 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.214660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/feeds/waldo
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/reordered-item/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.214660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.214660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/1
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/2
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/main.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/reordered-item/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.214660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1550 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.214660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/waldo
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3286 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/test_archive.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4257 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/test_cli.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    10833 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/test_download.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    15051 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/test_feed.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     7436 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/test_linking.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2165 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/test_urls.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     8147 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/src/feedarchiver/utils.py
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      162 2023-04-15 22:29:47.000000 feed-archiver-2.0.0b0/src/feedarchiver/version.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3362 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/tox.ini
```

### Comparing `feed-archiver-1.0.0b11/.dir-locals.el.in` & `feed-archiver-2.0.0b0/.dir-locals.el.in`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/.dockerignore` & `feed-archiver-2.0.0b0/.dockerignore`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/.env.in` & `feed-archiver-2.0.0b0/.env.in`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/.github/workflows/build-test.yml` & `feed-archiver-2.0.0b0/.github/workflows/build-test.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,9 @@
 name: "Build and Test"
 
-# TEMPLATE: If using GitHub Actions, then add the following secrets to the project:
-# - `CODECOV_TOKEN`:
-#   Add your project to https://app.codecov.io/gl and use the generated token
-# - `DOCKER_PASS`:
-#   A Docker Hub Personal Access Token
-# - `GPG_PASSPHRASE`:
-#   See the comments towards the bottom of the `./Makefile`
-# - `GPG_SIGNING_PRIVATE_KEY`:
-#   See the comments towards the bottom of the `./Makefile`
-# - `PROJECT_GITHUB_PAT`:
-#   A GitHub "Classic" Personal Access Token with scopes: `repo`, `workflow`,
-#   `packages`, and `project`
-# - `PYPI_PASSWORD`:
-#   A PyPI API token
-# - `TEST_PYPI_PASSWORD`:
-#   A PyPI API token
-
 on:
   # Only run on branches, not tags:
   # https://github.com/orgs/community/discussions/25615#discussioncomment-3397691
   push:
     branches:
       - "**"
     tags:
```

### Comparing `feed-archiver-1.0.0b11/.gitignore` & `feed-archiver-2.0.0b0/.gitignore`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/.pre-commit-config.yaml` & `feed-archiver-2.0.0b0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/.prospector.yaml` & `feed-archiver-2.0.0b0/.prospector.yaml`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/CONTRIBUTING.rst` & `feed-archiver-2.0.0b0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/Dockerfile` & `feed-archiver-2.0.0b0/Dockerfile`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/Dockerfile.devel` & `feed-archiver-2.0.0b0/Dockerfile.devel`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/LICENSE` & `feed-archiver-2.0.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/Makefile` & `feed-archiver-2.0.0b0/Makefile`

 * *Files 1% similar despite different names*

```diff
@@ -8,19 +8,22 @@
 
 # Variables used as options to control behavior:
 export TEMPLATE_IGNORE_EXISTING=false
 # https://devguide.python.org/versions/#supported-versions
 PYTHON_SUPPORTED_MINORS=3.11 3.10 3.9 3.8 3.7
 # Project-specific variables
 export DOCKER_USER=merpatterson
-# TEMPLATE: See comments towards the bottom and update.
 GPG_SIGNING_KEYID=2EFF7CCE6828E359
 CI_UPSTREAM_NAMESPACE=rpatterson
 CI_PROJECT_NAME=feed-archiver
 
+# Project-specific options:
+DEBUG=
+POST_MORTEM=
+
 
 ## "Private" Variables:
 
 # Variables that aren't likely to be of concern those just using and reading top-level
 # targets.  Mostly variables whose values are derived from the environment or other
 # values.  If adding a variable whose value isn't a literal constant or intended for use
 # on the CLI as an option, add it to the appropriate grouping below.  Unfortunately,
@@ -37,14 +40,15 @@
 .DELETE_ON_ERROR:
 MAKEFLAGS+=--warn-undefined-variables
 MAKEFLAGS+=--no-builtin-rules
 PS1?=$$
 EMPTY=
 COMMA=,
 
+# Values derived from the environment:
 USER_NAME:=$(shell id -u -n)
 USER_FULL_NAME:=$(shell \
     getent passwd "$(USER_NAME)" | cut -d ":" -f 5 | cut -d "," -f 1)
 ifeq ($(USER_FULL_NAME),)
 USER_FULL_NAME=$(USER_NAME)
 endif
 USER_EMAIL:=$(USER_NAME)@$(shell hostname -f)
@@ -1406,14 +1410,41 @@
 	elif [ "$(CI_IS_FORK)" != "true" ]
 	then
 	    echo "ERROR: PROJECT_GITHUB_PAT missing from ./.env or CI secrets"
 	    false
 	fi
 	date | tee -a "$(@)"
 
+# Static site server set up
+./server/.htpasswd: .SHELLFLAGS = -eu -o pipefail -c
+./server/.htpasswd:
+	echo "Enter a HTTP Basic authentication password for the static site server."
+	if ! which htpasswd
+	then
+	    sudo apt-get update
+	    sudo apt-get install -y apache2-utils
+	fi
+	htpasswd -c "$(@)" "feed-archiver"
+
+# Extract the Sonarr API key
+./sonarr/config/config.xml: ./var/log/docker-build.log
+	docker compose up -d sonarr
+	sleep 1
+	until [ -e "$(@)" ]
+	do
+	    sleep 0.1
+	done
+./src/feedarchiver/tests/archives/end-to-end/.feed-archiver.yml: \
+		./src/feedarchiver/tests/archives/end-to-end/.feed-archiver.yml.in \
+		./sonarr/config/config.xml
+	export SONARR_API_KEY=$$(
+	    sed -nE 's|.*<ApiKey>(.+)</ApiKey>.*|\1|p' "./sonarr/config/config.xml"
+	)
+	$(MAKE) "template=$(<)" "target=$(@)" expand-template
+
 # GPG signing key creation and management in CI
 export GPG_PASSPHRASE=
 GPG_SIGNING_PRIVATE_KEY=
 ./var/ci-cd-signing-subkey.asc:
 # We need a private key in the CI/CD environment for signing release commits and
 # artifacts.  Use a subkey so that it can be revoked without affecting your main key.
 # This recipe captures what I had to do to export a private signing subkey.  It's not
@@ -1462,18 +1493,14 @@
 	echo "ERROR: GPG_SIGNING_PRIVATE_KEY or GPG_PASSPHRASE " \
 	    "missing from ./.env or CI secrets"
 	false
 endif
 	date | tee -a "$(@)"
 endif
 
-# TEMPLATE: Optionally, use the following command to generate a GitLab CI/CD runner
-# configuration, register it with your project, compare it with the template
-# prerequisite, apply the appropriate changes and then  run using `$ docker compose up
-# gitlab-runner`.  Particularly useful to conserve shared runner minutes:
 ./gitlab-runner/config/config.toml: ./gitlab-runner/config/config.toml.in
 	docker compose run --rm gitlab-runner register \
 	    --url "https://gitlab.com/" --docker-image "docker" --executor "docker"
 
 
 ## Utility Targets:
 #
@@ -1516,17 +1543,14 @@
 	        fi
 	    done
 	done
 	set +x
 	echo "ERROR: Could not pull any existing docker image"
 	false
 
-# TEMPLATE: Run this once for your project.  See the `./var/log/docker-login*.log`
-# targets for the authentication environment variables that need to be set or just login
-# to those container registries manually and touch these targets.
 .PHONY: bootstrap-project
 ### Run any tasks needed to be run once for a given project by a maintainer
 bootstrap-project: \
 		./var/log/docker-login-GITLAB.log \
 		./var/log/docker-login-GITHUB.log
 # Initially seed the build host Docker image to bootstrap CI/CD environments
 # GitLab CI/CD:
```

### Comparing `feed-archiver-1.0.0b11/NEWS.rst` & `feed-archiver-2.0.0b0/NEWS.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+feed-archiver 2.0.0b0 (2023-04-15)
+==================================
+
+Bugfixes
+--------
+
+- Restore correct versions going forward.  Versions from here to v1.0.0 below are
+  incorrect. (correct-versions)
+
+
 feed-archiver 1.0.0b11 (2023-04-15)
 ===================================
 
 Bugfixes
 --------
 
 - Upgrade all requirements to the latest versions as of Sat Apr 15 06:11:17 PM UTC 2023. (upgrade-requirements)
@@ -9,14 +19,15 @@
 
 Feedarchiver 1.0.0b10 (2023-03-15)
 ==================================
 
 Features
 --------
 
+- Address a Bandit warning about requests without timeouts. (request-timeouts)
 - Write an ``./index.html`` file listing links to archived feeds. (archive-index)
 - Rename the ``link-paths`` plugin system to a more accurate name, ``enclosures``.  Note
   that this requires an update to existing archive configurations using ``link-paths``
   plugins. (enclosure-plugin-rename)
 - Replace ``content`` term with more correct ``enclosure`` term.  Requires running the ``$
   feed-archiver relink`` sub-command to update existing archives. (enclosure-term)
 - Avoid unintended sub-directories in link path plugin template paths, add support for
@@ -67,14 +78,20 @@
 
 Bugfixes
 --------
 
 - Don't report results from the ``update`` sub-command when there are none. (empty-results)
 
 
+Feedarchiver 1.0.0 (2022-12-16)
+===============================
+
+No significant changes.
+
+
 Feedarchiver 1.0.0b0 (2022-12-16)
 =================================
 
 Features
 --------
 
 - First stable release. (initial-release)
```

### Comparing `feed-archiver-1.0.0b11/PKG-INFO` & `feed-archiver-2.0.0b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feed-archiver
-Version: 1.0.0b11
+Version: 2.0.0b0
 Summary: Archive the full contents of RSS/Atom syndication feeds including enclosures and assets.
 Home-page: https://gitlab.com/rpatterson/feed-archiver
 Author: Ross Patterson
 Author-email: me@rpatterson.net
 License: MIT
 Keywords: template,structure
 Classifier: Development Status :: 4 - Beta
@@ -452,15 +452,15 @@
 .. _Sonarr: https://sonarr.tv
 .. _connect to the Sonarr API: https://github.com/Sonarr/Sonarr/wiki/API#url
 .. _look up the TV show/series: https://github.com/Sonarr/Sonarr/wiki/Series#getid
 .. _lookup the episode file: https://github.com/Sonarr/Sonarr/wiki/Episode#get
 
 .. _the Docker image: https://hub.docker.com/r/merpatterson/feed-archiver
 .. _`the example ./docker-compose.yml file`:
-   https://gitlab.com/rpatterson/feed-archiver/blob/master/docker-compose.yml
+   https://gitlab.com/rpatterson/feed-archiver/blob/main/docker-compose.yml
 
 .. _`This project is hosted on GitLab`:
    https://gitlab.com/rpatterson/feed-archiver
 .. _`a mirror on GitHub`:
    https://github.com/rpatterson/feed-archiver
 .. _`the ./CONTRIBUTING.rst file`:
    https://gitlab.com/rpatterson/feed-archiver/blob/main/CONTRIBUTING.rst
```

### Comparing `feed-archiver-1.0.0b11/README.rst` & `feed-archiver-2.0.0b0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -424,15 +424,15 @@
 .. _Sonarr: https://sonarr.tv
 .. _connect to the Sonarr API: https://github.com/Sonarr/Sonarr/wiki/API#url
 .. _look up the TV show/series: https://github.com/Sonarr/Sonarr/wiki/Series#getid
 .. _lookup the episode file: https://github.com/Sonarr/Sonarr/wiki/Episode#get
 
 .. _the Docker image: https://hub.docker.com/r/merpatterson/feed-archiver
 .. _`the example ./docker-compose.yml file`:
-   https://gitlab.com/rpatterson/feed-archiver/blob/master/docker-compose.yml
+   https://gitlab.com/rpatterson/feed-archiver/blob/main/docker-compose.yml
 
 .. _`This project is hosted on GitLab`:
    https://gitlab.com/rpatterson/feed-archiver
 .. _`a mirror on GitHub`:
    https://github.com/rpatterson/feed-archiver
 .. _`the ./CONTRIBUTING.rst file`:
    https://gitlab.com/rpatterson/feed-archiver/blob/main/CONTRIBUTING.rst
```

### Comparing `feed-archiver-1.0.0b11/TODO.rst` & `feed-archiver-2.0.0b0/TODO.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 ########################################################################################
 Seeking Contributions
 ########################################################################################
 
 Known bugs and desirable features for which contributions are most welcome.
 
-TEMPLATE: Remove any of the following TODOs from the template that your project doesn't
-care about and add your own.
-
 
 ****************************************************************************************
 Required
 ****************************************************************************************
 
 
 ****************************************************************************************
```

### Comparing `feed-archiver-1.0.0b11/bin/cz-check-bump` & `feed-archiver-2.0.0b0/bin/cz-check-bump`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/bin/entrypoint` & `feed-archiver-2.0.0b0/bin/entrypoint`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/bin/get-base-version` & `feed-archiver-2.0.0b0/bin/get-base-version`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/build-host/Dockerfile` & `feed-archiver-2.0.0b0/build-host/Dockerfile`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/build-host/Makefile` & `feed-archiver-2.0.0b0/build-host/Makefile`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/build-host/README.rst` & `feed-archiver-2.0.0b0/build-host/README.rst`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/build-host/bin/entrypoint` & `feed-archiver-2.0.0b0/build-host/bin/entrypoint`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/build-host/requirements-py310.txt` & `feed-archiver-2.0.0b0/build-host/requirements-py310.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/build-host/requirements-py311.txt` & `feed-archiver-2.0.0b0/build-host/requirements-py311.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/build-host/requirements-py37.txt` & `feed-archiver-2.0.0b0/build-host/requirements-py37.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/build-host/requirements-py38.txt` & `feed-archiver-2.0.0b0/build-host/requirements-py38.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/build-host/requirements-py39.txt` & `feed-archiver-2.0.0b0/build-host/requirements-py39.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/docker-compose-servarr.yml` & `feed-archiver-2.0.0b0/docker-compose-servarr.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/docker-compose.override.yml` & `feed-archiver-2.0.0b0/docker-compose.override.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/docker-compose.yml` & `feed-archiver-2.0.0b0/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/gitlab-runner/config/config.toml.in` & `feed-archiver-2.0.0b0/gitlab-runner/config/config.toml.in`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/nginx/templates/default.conf.template` & `feed-archiver-2.0.0b0/nginx/templates/default.conf.template`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/pyproject.toml` & `feed-archiver-2.0.0b0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 [tool.commitizen]
 # Parse commit messages according to conventional commits to decide wether the next
 # versin tag should be a major, minor or patch bump and create the VCS tag.  Also
 # provides VCS hooks to enforce that commit messages comply with conventional commits:
 # https://commitizen-tools.github.io/commitizen/
 name = "cz_conventional_commits"
 changelog_start_rev = "v0.0.0"
-version = "1.0.0b11"
+version = "2.0.0b0"
 tag_format = "v$version"
 annotated_tag = true
 gpg_sign = true
 bump_message = """\
 build(release): Version $current_version → $new_version
 
 [actions skip]
```

### Comparing `feed-archiver-1.0.0b11/requirements/build.txt.in` & `feed-archiver-2.0.0b0/requirements/build.txt.in`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/requirements/py310/build.txt` & `feed-archiver-2.0.0b0/requirements/py310/build.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/requirements/py310/devel.txt` & `feed-archiver-2.0.0b0/requirements/py310/devel.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,35 +2,33 @@
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    pip-compile --extra=devel --output-file=requirements/py310/devel.txt --resolver=backtracking pyproject.toml
 #
 anyio==3.6.2
     # via httpcore
-argcomplete==2.1.2
+argcomplete==3.0.5
     # via feed-archiver (pyproject.toml)
 arrapi==1.4.2
     # via feed-archiver (pyproject.toml)
-astroid==2.15.0
+astroid==2.15.2
     # via
     #   pylint
     #   pylint-celery
     #   pylint-flask
     #   requirements-detector
 attrs==22.2.0
-    # via
-    #   pytest
-    #   pytest-subtests
+    # via pytest-subtests
 autoflake==1.7.8
     # via feed-archiver (pyproject.toml)
 autopep8==2.0.2
     # via feed-archiver (pyproject.toml)
 bandit==1.7.5
     # via prospector
-black==23.1.0
+black==23.3.0
     # via feed-archiver (pyproject.toml)
 build==0.10.0
     # via
     #   feed-archiver (pyproject.toml)
     #   pip-tools
     #   pyroma
 certifi==2022.12.7
@@ -53,15 +51,15 @@
     # via towncrier
 colorama==0.4.6
     # via
     #   radon
     #   typer
 commonmark==0.9.1
     # via rich
-coverage==7.2.2
+coverage==7.2.3
     # via feed-archiver (pyproject.toml)
 dill==0.3.6
     # via pylint
 distlib==0.3.6
     # via virtualenv
 docutils==0.19
     # via
@@ -69,15 +67,15 @@
     #   rstcheck-core
 dodgy==0.2.1
     # via prospector
 exceptiongroup==1.1.1
     # via pytest
 feedparser==6.0.10
     # via feed-archiver (pyproject.toml)
-filelock==3.10.0
+filelock==3.11.0
     # via virtualenv
 flake8==2.3.0
     # via
     #   flake8-polyfill
     #   prospector
 flake8-polyfill==1.0.2
     # via pep8-naming
@@ -87,27 +85,27 @@
     # via gitpython
 gitpython==3.1.31
     # via
     #   bandit
     #   prospector
 h11==0.14.0
     # via httpcore
-httpcore==0.16.3
+httpcore==0.17.0
     # via httpx
-httpx==0.23.3
+httpx==0.24.0
     # via
     #   feed-archiver (pyproject.toml)
     #   respx
-identify==2.5.21
+identify==2.5.22
     # via pre-commit
 idna==3.4
     # via
     #   anyio
+    #   httpx
     #   requests
-    #   rfc3986
 incremental==22.10.0
     # via towncrier
 iniconfig==2.0.0
     # via pytest
 isort==5.12.0
     # via pylint
 jinja2==3.1.2
@@ -123,23 +121,23 @@
 markupsafe==2.1.2
     # via jinja2
 mccabe==0.7.0
     # via
     #   flake8
     #   prospector
     #   pylint
-mypy==1.1.1
+mypy==1.2.0
     # via prospector
 mypy-extensions==1.0.0
     # via
     #   black
     #   mypy
 nodeenv==1.7.0
     # via pre-commit
-packaging==23.0
+packaging==23.1
     # via
     #   black
     #   build
     #   prospector
     #   pyroma
     #   pytest
     #   requirements-detector
@@ -148,47 +146,47 @@
     # via black
 pbr==5.11.1
     # via stevedore
 pep8==1.7.1
     # via flake8
 pep8-naming==0.10.0
     # via prospector
-pip-tools==6.12.3
+pip-tools==6.13.0
     # via feed-archiver (pyproject.toml)
-platformdirs==3.1.1
+platformdirs==3.2.0
     # via
     #   black
     #   pylint
     #   virtualenv
 pluggy==1.0.0
     # via pytest
 poetry-semver==0.1.0
     # via requirements-detector
-pre-commit==3.2.0
+pre-commit==3.2.2
     # via feed-archiver (pyproject.toml)
 prospector[with_everything]==1.9.0
     # via feed-archiver (pyproject.toml)
 pycodestyle==2.10.0
     # via
     #   autopep8
     #   prospector
-pydantic==1.10.6
+pydantic==1.10.7
     # via rstcheck-core
 pydocstyle==6.3.0
     # via prospector
 pyflakes==2.5.0
     # via
     #   autoflake
     #   flake8
     #   prospector
-pygments==2.14.0
+pygments==2.15.0
     # via
     #   pyroma
     #   rich
-pylint==2.17.0
+pylint==2.17.2
     # via
     #   prospector
     #   pylint-celery
     #   pylint-django
     #   pylint-flask
     #   pylint-plugin-utils
 pylint-celery==0.3
@@ -203,15 +201,15 @@
     #   pylint-celery
     #   pylint-django
     #   pylint-flask
 pyproject-hooks==1.0.0
     # via build
 pyroma==4.2
     # via prospector
-pytest==7.2.2
+pytest==7.3.1
     # via
     #   feed-archiver (pyproject.toml)
     #   pytest-subtests
 pytest-subtests==0.10.0
     # via feed-archiver (pyproject.toml)
 pyyaml==6.0
     # via
@@ -230,16 +228,14 @@
     #   xenon
 requests-mock==1.10.0
     # via feed-archiver (pyproject.toml)
 requirements-detector==1.1.0
     # via prospector
 respx==0.20.1
     # via feed-archiver (pyproject.toml)
-rfc3986[idna2008]==1.5.0
-    # via httpx
 rich==12.6.0
     # via
     #   bandit
     #   typer
 rstcheck==6.1.2
     # via feed-archiver (pyproject.toml)
 rstcheck-core==1.0.3
@@ -283,26 +279,30 @@
     #   build
     #   mypy
     #   pylint
     #   pyproject-hooks
     #   pytest
     #   setuptools-scm
     #   towncrier
-tomlkit==0.11.6
+tomlkit==0.11.7
     # via pylint
 towncrier==22.12.0
     # via feed-archiver (pyproject.toml)
 trove-classifiers==2023.3.9
     # via pyroma
 typer[all]==0.7.0
     # via rstcheck
-types-docutils==0.19.1.6
+types-docutils==0.19.1.7
     # via rstcheck-core
-types-pyyaml==6.0.12.8
+types-pyyaml==6.0.12.9
+    # via feed-archiver (pyproject.toml)
+types-requests==2.28.11.17
     # via feed-archiver (pyproject.toml)
+types-urllib3==1.26.25.10
+    # via types-requests
 typing-extensions==4.5.0
     # via
     #   astroid
     #   mypy
     #   pydantic
     #   setuptools-scm
 urllib3==1.26.15
```

### Comparing `feed-archiver-1.0.0b11/requirements/py310/user.txt` & `feed-archiver-2.0.0b0/requirements/py39/user.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,45 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --output-file=requirements/py310/user.txt --resolver=backtracking pyproject.toml
+#    pip-compile --output-file=requirements/py39/user.txt --resolver=backtracking pyproject.toml
 #
 anyio==3.6.2
     # via httpcore
-argcomplete==2.1.2
+argcomplete==3.0.5
     # via feed-archiver (pyproject.toml)
 arrapi==1.4.2
     # via feed-archiver (pyproject.toml)
 certifi==2022.12.7
     # via
     #   httpcore
     #   httpx
     #   requests
 charset-normalizer==3.1.0
     # via requests
 feedparser==6.0.10
     # via feed-archiver (pyproject.toml)
 h11==0.14.0
     # via httpcore
-httpcore==0.16.3
+httpcore==0.17.0
     # via httpx
-httpx==0.23.3
+httpx==0.24.0
     # via feed-archiver (pyproject.toml)
 idna==3.4
     # via
     #   anyio
+    #   httpx
     #   requests
-    #   rfc3986
 lxml==4.9.2
     # via feed-archiver (pyproject.toml)
 pyyaml==6.0
     # via feed-archiver (pyproject.toml)
 requests==2.28.2
     # via arrapi
-rfc3986[idna2008]==1.5.0
-    # via httpx
 sgmllib3k==1.0.0
     # via feedparser
 six==1.16.0
     # via user-agent
 sniffio==1.3.0
     # via
     #   anyio
```

### Comparing `feed-archiver-1.0.0b11/requirements/py311/build.txt` & `feed-archiver-2.0.0b0/requirements/py311/build.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/requirements/py311/devel.txt` & `feed-archiver-2.0.0b0/requirements/py39/devel.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --extra=devel --output-file=requirements/py311/devel.txt --resolver=backtracking pyproject.toml
+#    pip-compile --extra=devel --output-file=requirements/py39/devel.txt --resolver=backtracking pyproject.toml
 #
 anyio==3.6.2
     # via httpcore
-argcomplete==2.1.2
+argcomplete==3.0.5
     # via feed-archiver (pyproject.toml)
 arrapi==1.4.2
     # via feed-archiver (pyproject.toml)
-astroid==2.15.0
+astroid==2.15.2
     # via
     #   pylint
     #   pylint-celery
     #   pylint-flask
     #   requirements-detector
 attrs==22.2.0
-    # via
-    #   pytest
-    #   pytest-subtests
+    # via pytest-subtests
 autoflake==1.7.8
     # via feed-archiver (pyproject.toml)
 autopep8==2.0.2
     # via feed-archiver (pyproject.toml)
 bandit==1.7.5
     # via prospector
-black==23.1.0
+black==23.3.0
     # via feed-archiver (pyproject.toml)
 build==0.10.0
     # via
     #   feed-archiver (pyproject.toml)
     #   pip-tools
     #   pyroma
 certifi==2022.12.7
@@ -53,29 +51,31 @@
     # via towncrier
 colorama==0.4.6
     # via
     #   radon
     #   typer
 commonmark==0.9.1
     # via rich
-coverage==7.2.2
+coverage==7.2.3
     # via feed-archiver (pyproject.toml)
 dill==0.3.6
     # via pylint
 distlib==0.3.6
     # via virtualenv
 docutils==0.19
     # via
     #   pyroma
     #   rstcheck-core
 dodgy==0.2.1
     # via prospector
+exceptiongroup==1.1.1
+    # via pytest
 feedparser==6.0.10
     # via feed-archiver (pyproject.toml)
-filelock==3.10.0
+filelock==3.11.0
     # via virtualenv
 flake8==2.3.0
     # via
     #   flake8-polyfill
     #   prospector
 flake8-polyfill==1.0.2
     # via pep8-naming
@@ -85,27 +85,27 @@
     # via gitpython
 gitpython==3.1.31
     # via
     #   bandit
     #   prospector
 h11==0.14.0
     # via httpcore
-httpcore==0.16.3
+httpcore==0.17.0
     # via httpx
-httpx==0.23.3
+httpx==0.24.0
     # via
     #   feed-archiver (pyproject.toml)
     #   respx
-identify==2.5.21
+identify==2.5.22
     # via pre-commit
 idna==3.4
     # via
     #   anyio
+    #   httpx
     #   requests
-    #   rfc3986
 incremental==22.10.0
     # via towncrier
 iniconfig==2.0.0
     # via pytest
 isort==5.12.0
     # via pylint
 jinja2==3.1.2
@@ -121,23 +121,23 @@
 markupsafe==2.1.2
     # via jinja2
 mccabe==0.7.0
     # via
     #   flake8
     #   prospector
     #   pylint
-mypy==1.1.1
+mypy==1.2.0
     # via prospector
 mypy-extensions==1.0.0
     # via
     #   black
     #   mypy
 nodeenv==1.7.0
     # via pre-commit
-packaging==23.0
+packaging==23.1
     # via
     #   black
     #   build
     #   prospector
     #   pyroma
     #   pytest
     #   requirements-detector
@@ -146,47 +146,47 @@
     # via black
 pbr==5.11.1
     # via stevedore
 pep8==1.7.1
     # via flake8
 pep8-naming==0.10.0
     # via prospector
-pip-tools==6.12.3
+pip-tools==6.13.0
     # via feed-archiver (pyproject.toml)
-platformdirs==3.1.1
+platformdirs==3.2.0
     # via
     #   black
     #   pylint
     #   virtualenv
 pluggy==1.0.0
     # via pytest
 poetry-semver==0.1.0
     # via requirements-detector
-pre-commit==3.2.0
+pre-commit==3.2.2
     # via feed-archiver (pyproject.toml)
 prospector[with_everything]==1.9.0
     # via feed-archiver (pyproject.toml)
 pycodestyle==2.10.0
     # via
     #   autopep8
     #   prospector
-pydantic==1.10.6
+pydantic==1.10.7
     # via rstcheck-core
 pydocstyle==6.3.0
     # via prospector
 pyflakes==2.5.0
     # via
     #   autoflake
     #   flake8
     #   prospector
-pygments==2.14.0
+pygments==2.15.0
     # via
     #   pyroma
     #   rich
-pylint==2.17.0
+pylint==2.17.2
     # via
     #   prospector
     #   pylint-celery
     #   pylint-django
     #   pylint-flask
     #   pylint-plugin-utils
 pylint-celery==0.3
@@ -201,15 +201,15 @@
     #   pylint-celery
     #   pylint-django
     #   pylint-flask
 pyproject-hooks==1.0.0
     # via build
 pyroma==4.2
     # via prospector
-pytest==7.2.2
+pytest==7.3.1
     # via
     #   feed-archiver (pyproject.toml)
     #   pytest-subtests
 pytest-subtests==0.10.0
     # via feed-archiver (pyproject.toml)
 pyyaml==6.0
     # via
@@ -228,16 +228,14 @@
     #   xenon
 requests-mock==1.10.0
     # via feed-archiver (pyproject.toml)
 requirements-detector==1.1.0
     # via prospector
 respx==0.20.1
     # via feed-archiver (pyproject.toml)
-rfc3986[idna2008]==1.5.0
-    # via httpx
 rich==12.6.0
     # via
     #   bandit
     #   typer
 rstcheck==6.1.2
     # via feed-archiver (pyproject.toml)
 rstcheck-core==1.0.3
@@ -269,30 +267,49 @@
 tenacity==8.2.2
     # via feed-archiver (pyproject.toml)
 toml==0.10.2
     # via
     #   prospector
     #   requirements-detector
     #   vulture
-tomlkit==0.11.6
+tomli==2.0.1
+    # via
+    #   autoflake
+    #   autopep8
+    #   black
+    #   build
+    #   mypy
+    #   pylint
+    #   pyproject-hooks
+    #   pytest
+    #   setuptools-scm
+    #   towncrier
+tomlkit==0.11.7
     # via pylint
 towncrier==22.12.0
     # via feed-archiver (pyproject.toml)
 trove-classifiers==2023.3.9
     # via pyroma
 typer[all]==0.7.0
     # via rstcheck
-types-docutils==0.19.1.6
+types-docutils==0.19.1.7
     # via rstcheck-core
-types-pyyaml==6.0.12.8
+types-pyyaml==6.0.12.9
+    # via feed-archiver (pyproject.toml)
+types-requests==2.28.11.17
     # via feed-archiver (pyproject.toml)
+types-urllib3==1.26.25.10
+    # via types-requests
 typing-extensions==4.5.0
     # via
+    #   astroid
+    #   black
     #   mypy
     #   pydantic
+    #   pylint
     #   setuptools-scm
 urllib3==1.26.15
     # via requests
 user-agent==0.1.10
     # via feed-archiver (pyproject.toml)
 virtualenv==20.21.0
     # via pre-commit
```

### Comparing `feed-archiver-1.0.0b11/requirements/py311/user.txt` & `feed-archiver-2.0.0b0/requirements/py38/user.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,45 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --output-file=requirements/py311/user.txt --resolver=backtracking pyproject.toml
+#    pip-compile --output-file=requirements/py38/user.txt --resolver=backtracking pyproject.toml
 #
 anyio==3.6.2
     # via httpcore
-argcomplete==2.1.2
+argcomplete==3.0.5
     # via feed-archiver (pyproject.toml)
 arrapi==1.4.2
     # via feed-archiver (pyproject.toml)
 certifi==2022.12.7
     # via
     #   httpcore
     #   httpx
     #   requests
 charset-normalizer==3.1.0
     # via requests
 feedparser==6.0.10
     # via feed-archiver (pyproject.toml)
 h11==0.14.0
     # via httpcore
-httpcore==0.16.3
+httpcore==0.17.0
     # via httpx
-httpx==0.23.3
+httpx==0.24.0
     # via feed-archiver (pyproject.toml)
 idna==3.4
     # via
     #   anyio
+    #   httpx
     #   requests
-    #   rfc3986
 lxml==4.9.2
     # via feed-archiver (pyproject.toml)
 pyyaml==6.0
     # via feed-archiver (pyproject.toml)
 requests==2.28.2
     # via arrapi
-rfc3986[idna2008]==1.5.0
-    # via httpx
 sgmllib3k==1.0.0
     # via feedparser
 six==1.16.0
     # via user-agent
 sniffio==1.3.0
     # via
     #   anyio
```

### Comparing `feed-archiver-1.0.0b11/requirements/py37/build.txt` & `feed-archiver-2.0.0b0/requirements/py37/build.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/requirements/py37/devel.txt` & `feed-archiver-2.0.0b0/requirements/py37/devel.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,37 +2,35 @@
 # This file is autogenerated by pip-compile with Python 3.7
 # by the following command:
 #
 #    pip-compile --extra=devel --output-file=requirements/py37/devel.txt --resolver=backtracking pyproject.toml
 #
 anyio==3.6.2
     # via httpcore
-argcomplete==2.1.2
+argcomplete==3.0.5
     # via feed-archiver (pyproject.toml)
 arrapi==1.4.2
     # via feed-archiver (pyproject.toml)
-astroid==2.15.0
+astroid==2.15.2
     # via
     #   pylint
     #   pylint-celery
     #   pylint-flask
     #   requirements-detector
 attrs==22.2.0
-    # via
-    #   pytest
-    #   pytest-subtests
+    # via pytest-subtests
 autoflake==1.7.8
     # via feed-archiver (pyproject.toml)
 autopep8==2.0.2
     # via feed-archiver (pyproject.toml)
 backports-cached-property==1.0.2 ; python_version < "3.8"
     # via feed-archiver (pyproject.toml)
 bandit==1.7.5
     # via prospector
-black==23.1.0
+black==23.3.0
     # via feed-archiver (pyproject.toml)
 build==0.10.0
     # via
     #   feed-archiver (pyproject.toml)
     #   pip-tools
     #   pyroma
 certifi==2022.12.7
@@ -55,15 +53,15 @@
     # via towncrier
 colorama==0.4.6
     # via
     #   radon
     #   typer
 commonmark==0.9.1
     # via rich
-coverage==7.2.2
+coverage==7.2.3
     # via feed-archiver (pyproject.toml)
 dill==0.3.6
     # via pylint
 distlib==0.3.6
     # via virtualenv
 docutils==0.19
     # via
@@ -71,15 +69,15 @@
     #   rstcheck-core
 dodgy==0.2.1
     # via prospector
 exceptiongroup==1.1.1
     # via pytest
 feedparser==6.0.10
     # via feed-archiver (pyproject.toml)
-filelock==3.10.0
+filelock==3.11.0
     # via virtualenv
 flake8==2.3.0
     # via
     #   flake8-polyfill
     #   prospector
 flake8-polyfill==1.0.2
     # via pep8-naming
@@ -89,27 +87,27 @@
     # via gitpython
 gitpython==3.1.31
     # via
     #   bandit
     #   prospector
 h11==0.14.0
     # via httpcore
-httpcore==0.16.3
+httpcore==0.17.0
     # via httpx
-httpx==0.23.3
+httpx==0.24.0
     # via
     #   feed-archiver (pyproject.toml)
     #   respx
-identify==2.5.21
+identify==2.5.22
     # via pre-commit
 idna==3.4
     # via
     #   anyio
+    #   httpx
     #   requests
-    #   rfc3986
 importlib-metadata==4.13.0 ; python_version < "3.8"
     # via
     #   argcomplete
     #   build
     #   click
     #   feed-archiver (pyproject.toml)
     #   pluggy
@@ -140,23 +138,23 @@
 markupsafe==2.1.2
     # via jinja2
 mccabe==0.7.0
     # via
     #   flake8
     #   prospector
     #   pylint
-mypy==1.1.1
+mypy==1.2.0
     # via prospector
 mypy-extensions==1.0.0
     # via
     #   black
     #   mypy
 nodeenv==1.7.0
     # via pre-commit
-packaging==23.0
+packaging==23.1
     # via
     #   black
     #   build
     #   prospector
     #   pyroma
     #   pytest
     #   requirements-detector
@@ -165,17 +163,17 @@
     # via black
 pbr==5.11.1
     # via stevedore
 pep8==1.7.1
     # via flake8
 pep8-naming==0.10.0
     # via prospector
-pip-tools==6.12.3
+pip-tools==6.13.0
     # via feed-archiver (pyproject.toml)
-platformdirs==3.1.1
+platformdirs==3.2.0
     # via
     #   black
     #   pylint
     #   virtualenv
 pluggy==1.0.0
     # via pytest
 poetry-semver==0.1.0
@@ -184,28 +182,28 @@
     # via feed-archiver (pyproject.toml)
 prospector[with_everything]==1.9.0
     # via feed-archiver (pyproject.toml)
 pycodestyle==2.10.0
     # via
     #   autopep8
     #   prospector
-pydantic==1.10.6
+pydantic==1.10.7
     # via rstcheck-core
 pydocstyle==6.3.0
     # via prospector
 pyflakes==2.5.0
     # via
     #   autoflake
     #   flake8
     #   prospector
-pygments==2.14.0
+pygments==2.15.0
     # via
     #   pyroma
     #   rich
-pylint==2.17.0
+pylint==2.17.2
     # via
     #   prospector
     #   pylint-celery
     #   pylint-django
     #   pylint-flask
     #   pylint-plugin-utils
 pylint-celery==0.3
@@ -220,15 +218,15 @@
     #   pylint-celery
     #   pylint-django
     #   pylint-flask
 pyproject-hooks==1.0.0
     # via build
 pyroma==4.2
     # via prospector
-pytest==7.2.2
+pytest==7.3.1
     # via
     #   feed-archiver (pyproject.toml)
     #   pytest-subtests
 pytest-subtests==0.10.0
     # via feed-archiver (pyproject.toml)
 pyyaml==6.0
     # via
@@ -247,16 +245,14 @@
     #   xenon
 requests-mock==1.10.0
     # via feed-archiver (pyproject.toml)
 requirements-detector==1.1.0
     # via prospector
 respx==0.20.1
     # via feed-archiver (pyproject.toml)
-rfc3986[idna2008]==1.5.0
-    # via httpx
 rich==12.6.0
     # via
     #   bandit
     #   typer
 rstcheck==6.1.2
     # via feed-archiver (pyproject.toml)
 rstcheck-core==1.0.3
@@ -300,31 +296,35 @@
     #   build
     #   mypy
     #   pylint
     #   pyproject-hooks
     #   pytest
     #   setuptools-scm
     #   towncrier
-tomlkit==0.11.6
+tomlkit==0.11.7
     # via pylint
 towncrier==22.12.0
     # via feed-archiver (pyproject.toml)
 trove-classifiers==2023.3.9
     # via pyroma
 typed-ast==1.5.4
     # via
     #   astroid
     #   black
     #   mypy
 typer[all]==0.7.0
     # via rstcheck
-types-docutils==0.19.1.6
+types-docutils==0.19.1.7
     # via rstcheck-core
-types-pyyaml==6.0.12.8
+types-pyyaml==6.0.12.9
+    # via feed-archiver (pyproject.toml)
+types-requests==2.28.11.17
     # via feed-archiver (pyproject.toml)
+types-urllib3==1.26.25.10
+    # via types-requests
 typing-extensions==4.5.0
     # via
     #   anyio
     #   astroid
     #   black
     #   gitpython
     #   h11
```

### Comparing `feed-archiver-1.0.0b11/requirements/py37/user.txt` & `feed-archiver-2.0.0b0/requirements/py37/user.txt`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This file is autogenerated by pip-compile with Python 3.7
 # by the following command:
 #
 #    pip-compile --output-file=requirements/py37/user.txt --resolver=backtracking pyproject.toml
 #
 anyio==3.6.2
     # via httpcore
-argcomplete==2.1.2
+argcomplete==3.0.5
     # via feed-archiver (pyproject.toml)
 arrapi==1.4.2
     # via feed-archiver (pyproject.toml)
 backports-cached-property==1.0.2 ; python_version < "3.8"
     # via feed-archiver (pyproject.toml)
 certifi==2022.12.7
     # via
@@ -19,35 +19,33 @@
     #   requests
 charset-normalizer==3.1.0
     # via requests
 feedparser==6.0.10
     # via feed-archiver (pyproject.toml)
 h11==0.14.0
     # via httpcore
-httpcore==0.16.3
+httpcore==0.17.0
     # via httpx
-httpx==0.23.3
+httpx==0.24.0
     # via feed-archiver (pyproject.toml)
 idna==3.4
     # via
     #   anyio
+    #   httpx
     #   requests
-    #   rfc3986
 importlib-metadata==5.2.0 ; python_version < "3.8"
     # via
     #   argcomplete
     #   feed-archiver (pyproject.toml)
 lxml==4.9.2
     # via feed-archiver (pyproject.toml)
 pyyaml==6.0
     # via feed-archiver (pyproject.toml)
 requests==2.28.2
     # via arrapi
-rfc3986[idna2008]==1.5.0
-    # via httpx
 sgmllib3k==1.0.0
     # via feedparser
 six==1.16.0
     # via user-agent
 sniffio==1.3.0
     # via
     #   anyio
```

### Comparing `feed-archiver-1.0.0b11/requirements/py38/build.txt` & `feed-archiver-2.0.0b0/requirements/py38/build.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/requirements/py38/devel.txt` & `feed-archiver-2.0.0b0/requirements/py38/devel.txt`

 * *Files 5% similar despite different names*

```diff
@@ -2,35 +2,33 @@
 # This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
 #    pip-compile --extra=devel --output-file=requirements/py38/devel.txt --resolver=backtracking pyproject.toml
 #
 anyio==3.6.2
     # via httpcore
-argcomplete==2.1.2
+argcomplete==3.0.5
     # via feed-archiver (pyproject.toml)
 arrapi==1.4.2
     # via feed-archiver (pyproject.toml)
-astroid==2.15.0
+astroid==2.15.2
     # via
     #   pylint
     #   pylint-celery
     #   pylint-flask
     #   requirements-detector
 attrs==22.2.0
-    # via
-    #   pytest
-    #   pytest-subtests
+    # via pytest-subtests
 autoflake==1.7.8
     # via feed-archiver (pyproject.toml)
 autopep8==2.0.2
     # via feed-archiver (pyproject.toml)
 bandit==1.7.5
     # via prospector
-black==23.1.0
+black==23.3.0
     # via feed-archiver (pyproject.toml)
 build==0.10.0
     # via
     #   feed-archiver (pyproject.toml)
     #   pip-tools
     #   pyroma
 certifi==2022.12.7
@@ -53,15 +51,15 @@
     # via towncrier
 colorama==0.4.6
     # via
     #   radon
     #   typer
 commonmark==0.9.1
     # via rich
-coverage==7.2.2
+coverage==7.2.3
     # via feed-archiver (pyproject.toml)
 dill==0.3.6
     # via pylint
 distlib==0.3.6
     # via virtualenv
 docutils==0.19
     # via
@@ -69,15 +67,15 @@
     #   rstcheck-core
 dodgy==0.2.1
     # via prospector
 exceptiongroup==1.1.1
     # via pytest
 feedparser==6.0.10
     # via feed-archiver (pyproject.toml)
-filelock==3.10.0
+filelock==3.11.0
     # via virtualenv
 flake8==2.3.0
     # via
     #   flake8-polyfill
     #   prospector
 flake8-polyfill==1.0.2
     # via pep8-naming
@@ -87,27 +85,27 @@
     # via gitpython
 gitpython==3.1.31
     # via
     #   bandit
     #   prospector
 h11==0.14.0
     # via httpcore
-httpcore==0.16.3
+httpcore==0.17.0
     # via httpx
-httpx==0.23.3
+httpx==0.24.0
     # via
     #   feed-archiver (pyproject.toml)
     #   respx
-identify==2.5.21
+identify==2.5.22
     # via pre-commit
 idna==3.4
     # via
     #   anyio
+    #   httpx
     #   requests
-    #   rfc3986
 incremental==22.10.0
     # via towncrier
 iniconfig==2.0.0
     # via pytest
 isort==5.12.0
     # via pylint
 jinja2==3.1.2
@@ -123,23 +121,23 @@
 markupsafe==2.1.2
     # via jinja2
 mccabe==0.7.0
     # via
     #   flake8
     #   prospector
     #   pylint
-mypy==1.1.1
+mypy==1.2.0
     # via prospector
 mypy-extensions==1.0.0
     # via
     #   black
     #   mypy
 nodeenv==1.7.0
     # via pre-commit
-packaging==23.0
+packaging==23.1
     # via
     #   black
     #   build
     #   prospector
     #   pyroma
     #   pytest
     #   requirements-detector
@@ -148,47 +146,47 @@
     # via black
 pbr==5.11.1
     # via stevedore
 pep8==1.7.1
     # via flake8
 pep8-naming==0.10.0
     # via prospector
-pip-tools==6.12.3
+pip-tools==6.13.0
     # via feed-archiver (pyproject.toml)
-platformdirs==3.1.1
+platformdirs==3.2.0
     # via
     #   black
     #   pylint
     #   virtualenv
 pluggy==1.0.0
     # via pytest
 poetry-semver==0.1.0
     # via requirements-detector
-pre-commit==3.2.0
+pre-commit==3.2.2
     # via feed-archiver (pyproject.toml)
 prospector[with_everything]==1.9.0
     # via feed-archiver (pyproject.toml)
 pycodestyle==2.10.0
     # via
     #   autopep8
     #   prospector
-pydantic==1.10.6
+pydantic==1.10.7
     # via rstcheck-core
 pydocstyle==6.3.0
     # via prospector
 pyflakes==2.5.0
     # via
     #   autoflake
     #   flake8
     #   prospector
-pygments==2.14.0
+pygments==2.15.0
     # via
     #   pyroma
     #   rich
-pylint==2.17.0
+pylint==2.17.2
     # via
     #   prospector
     #   pylint-celery
     #   pylint-django
     #   pylint-flask
     #   pylint-plugin-utils
 pylint-celery==0.3
@@ -203,15 +201,15 @@
     #   pylint-celery
     #   pylint-django
     #   pylint-flask
 pyproject-hooks==1.0.0
     # via build
 pyroma==4.2
     # via prospector
-pytest==7.2.2
+pytest==7.3.1
     # via
     #   feed-archiver (pyproject.toml)
     #   pytest-subtests
 pytest-subtests==0.10.0
     # via feed-archiver (pyproject.toml)
 pyyaml==6.0
     # via
@@ -230,16 +228,14 @@
     #   xenon
 requests-mock==1.10.0
     # via feed-archiver (pyproject.toml)
 requirements-detector==1.1.0
     # via prospector
 respx==0.20.1
     # via feed-archiver (pyproject.toml)
-rfc3986[idna2008]==1.5.0
-    # via httpx
 rich==12.6.0
     # via
     #   bandit
     #   typer
 rstcheck==6.1.2
     # via feed-archiver (pyproject.toml)
 rstcheck-core==1.0.3
@@ -283,26 +279,30 @@
     #   build
     #   mypy
     #   pylint
     #   pyproject-hooks
     #   pytest
     #   setuptools-scm
     #   towncrier
-tomlkit==0.11.6
+tomlkit==0.11.7
     # via pylint
 towncrier==22.12.0
     # via feed-archiver (pyproject.toml)
 trove-classifiers==2023.3.9
     # via pyroma
 typer[all]==0.7.0
     # via rstcheck
-types-docutils==0.19.1.6
+types-docutils==0.19.1.7
     # via rstcheck-core
-types-pyyaml==6.0.12.8
+types-pyyaml==6.0.12.9
+    # via feed-archiver (pyproject.toml)
+types-requests==2.28.11.17
     # via feed-archiver (pyproject.toml)
+types-urllib3==1.26.25.10
+    # via types-requests
 typing-extensions==4.5.0
     # via
     #   astroid
     #   black
     #   mypy
     #   pydantic
     #   pylint
```

### Comparing `feed-archiver-1.0.0b11/requirements/py38/user.txt` & `feed-archiver-2.0.0b0/requirements/py310/user.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,47 +1,45 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --output-file=requirements/py38/user.txt --resolver=backtracking pyproject.toml
+#    pip-compile --output-file=requirements/py310/user.txt --resolver=backtracking pyproject.toml
 #
 anyio==3.6.2
     # via httpcore
-argcomplete==2.1.2
+argcomplete==3.0.5
     # via feed-archiver (pyproject.toml)
 arrapi==1.4.2
     # via feed-archiver (pyproject.toml)
 certifi==2022.12.7
     # via
     #   httpcore
     #   httpx
     #   requests
 charset-normalizer==3.1.0
     # via requests
 feedparser==6.0.10
     # via feed-archiver (pyproject.toml)
 h11==0.14.0
     # via httpcore
-httpcore==0.16.3
+httpcore==0.17.0
     # via httpx
-httpx==0.23.3
+httpx==0.24.0
     # via feed-archiver (pyproject.toml)
 idna==3.4
     # via
     #   anyio
+    #   httpx
     #   requests
-    #   rfc3986
 lxml==4.9.2
     # via feed-archiver (pyproject.toml)
 pyyaml==6.0
     # via feed-archiver (pyproject.toml)
 requests==2.28.2
     # via arrapi
-rfc3986[idna2008]==1.5.0
-    # via httpx
 sgmllib3k==1.0.0
     # via feedparser
 six==1.16.0
     # via user-agent
 sniffio==1.3.0
     # via
     #   anyio
```

### Comparing `feed-archiver-1.0.0b11/requirements/py39/build.txt` & `feed-archiver-2.0.0b0/requirements/py39/build.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/requirements/py39/devel.txt` & `feed-archiver-2.0.0b0/requirements/py311/devel.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile --extra=devel --output-file=requirements/py39/devel.txt --resolver=backtracking pyproject.toml
+#    pip-compile --extra=devel --output-file=requirements/py311/devel.txt --resolver=backtracking pyproject.toml
 #
 anyio==3.6.2
     # via httpcore
-argcomplete==2.1.2
+argcomplete==3.0.5
     # via feed-archiver (pyproject.toml)
 arrapi==1.4.2
     # via feed-archiver (pyproject.toml)
-astroid==2.15.0
+astroid==2.15.2
     # via
     #   pylint
     #   pylint-celery
     #   pylint-flask
     #   requirements-detector
 attrs==22.2.0
-    # via
-    #   pytest
-    #   pytest-subtests
+    # via pytest-subtests
 autoflake==1.7.8
     # via feed-archiver (pyproject.toml)
 autopep8==2.0.2
     # via feed-archiver (pyproject.toml)
 bandit==1.7.5
     # via prospector
-black==23.1.0
+black==23.3.0
     # via feed-archiver (pyproject.toml)
 build==0.10.0
     # via
     #   feed-archiver (pyproject.toml)
     #   pip-tools
     #   pyroma
 certifi==2022.12.7
@@ -53,31 +51,29 @@
     # via towncrier
 colorama==0.4.6
     # via
     #   radon
     #   typer
 commonmark==0.9.1
     # via rich
-coverage==7.2.2
+coverage==7.2.3
     # via feed-archiver (pyproject.toml)
 dill==0.3.6
     # via pylint
 distlib==0.3.6
     # via virtualenv
 docutils==0.19
     # via
     #   pyroma
     #   rstcheck-core
 dodgy==0.2.1
     # via prospector
-exceptiongroup==1.1.1
-    # via pytest
 feedparser==6.0.10
     # via feed-archiver (pyproject.toml)
-filelock==3.10.0
+filelock==3.11.0
     # via virtualenv
 flake8==2.3.0
     # via
     #   flake8-polyfill
     #   prospector
 flake8-polyfill==1.0.2
     # via pep8-naming
@@ -87,27 +83,27 @@
     # via gitpython
 gitpython==3.1.31
     # via
     #   bandit
     #   prospector
 h11==0.14.0
     # via httpcore
-httpcore==0.16.3
+httpcore==0.17.0
     # via httpx
-httpx==0.23.3
+httpx==0.24.0
     # via
     #   feed-archiver (pyproject.toml)
     #   respx
-identify==2.5.21
+identify==2.5.22
     # via pre-commit
 idna==3.4
     # via
     #   anyio
+    #   httpx
     #   requests
-    #   rfc3986
 incremental==22.10.0
     # via towncrier
 iniconfig==2.0.0
     # via pytest
 isort==5.12.0
     # via pylint
 jinja2==3.1.2
@@ -123,23 +119,23 @@
 markupsafe==2.1.2
     # via jinja2
 mccabe==0.7.0
     # via
     #   flake8
     #   prospector
     #   pylint
-mypy==1.1.1
+mypy==1.2.0
     # via prospector
 mypy-extensions==1.0.0
     # via
     #   black
     #   mypy
 nodeenv==1.7.0
     # via pre-commit
-packaging==23.0
+packaging==23.1
     # via
     #   black
     #   build
     #   prospector
     #   pyroma
     #   pytest
     #   requirements-detector
@@ -148,47 +144,47 @@
     # via black
 pbr==5.11.1
     # via stevedore
 pep8==1.7.1
     # via flake8
 pep8-naming==0.10.0
     # via prospector
-pip-tools==6.12.3
+pip-tools==6.13.0
     # via feed-archiver (pyproject.toml)
-platformdirs==3.1.1
+platformdirs==3.2.0
     # via
     #   black
     #   pylint
     #   virtualenv
 pluggy==1.0.0
     # via pytest
 poetry-semver==0.1.0
     # via requirements-detector
-pre-commit==3.2.0
+pre-commit==3.2.2
     # via feed-archiver (pyproject.toml)
 prospector[with_everything]==1.9.0
     # via feed-archiver (pyproject.toml)
 pycodestyle==2.10.0
     # via
     #   autopep8
     #   prospector
-pydantic==1.10.6
+pydantic==1.10.7
     # via rstcheck-core
 pydocstyle==6.3.0
     # via prospector
 pyflakes==2.5.0
     # via
     #   autoflake
     #   flake8
     #   prospector
-pygments==2.14.0
+pygments==2.15.0
     # via
     #   pyroma
     #   rich
-pylint==2.17.0
+pylint==2.17.2
     # via
     #   prospector
     #   pylint-celery
     #   pylint-django
     #   pylint-flask
     #   pylint-plugin-utils
 pylint-celery==0.3
@@ -203,15 +199,15 @@
     #   pylint-celery
     #   pylint-django
     #   pylint-flask
 pyproject-hooks==1.0.0
     # via build
 pyroma==4.2
     # via prospector
-pytest==7.2.2
+pytest==7.3.1
     # via
     #   feed-archiver (pyproject.toml)
     #   pytest-subtests
 pytest-subtests==0.10.0
     # via feed-archiver (pyproject.toml)
 pyyaml==6.0
     # via
@@ -230,16 +226,14 @@
     #   xenon
 requests-mock==1.10.0
     # via feed-archiver (pyproject.toml)
 requirements-detector==1.1.0
     # via prospector
 respx==0.20.1
     # via feed-archiver (pyproject.toml)
-rfc3986[idna2008]==1.5.0
-    # via httpx
 rich==12.6.0
     # via
     #   bandit
     #   typer
 rstcheck==6.1.2
     # via feed-archiver (pyproject.toml)
 rstcheck-core==1.0.3
@@ -271,45 +265,34 @@
 tenacity==8.2.2
     # via feed-archiver (pyproject.toml)
 toml==0.10.2
     # via
     #   prospector
     #   requirements-detector
     #   vulture
-tomli==2.0.1
-    # via
-    #   autoflake
-    #   autopep8
-    #   black
-    #   build
-    #   mypy
-    #   pylint
-    #   pyproject-hooks
-    #   pytest
-    #   setuptools-scm
-    #   towncrier
-tomlkit==0.11.6
+tomlkit==0.11.7
     # via pylint
 towncrier==22.12.0
     # via feed-archiver (pyproject.toml)
 trove-classifiers==2023.3.9
     # via pyroma
 typer[all]==0.7.0
     # via rstcheck
-types-docutils==0.19.1.6
+types-docutils==0.19.1.7
     # via rstcheck-core
-types-pyyaml==6.0.12.8
+types-pyyaml==6.0.12.9
+    # via feed-archiver (pyproject.toml)
+types-requests==2.28.11.17
     # via feed-archiver (pyproject.toml)
+types-urllib3==1.26.25.10
+    # via types-requests
 typing-extensions==4.5.0
     # via
-    #   astroid
-    #   black
     #   mypy
     #   pydantic
-    #   pylint
     #   setuptools-scm
 urllib3==1.26.15
     # via requests
 user-agent==0.1.10
     # via feed-archiver (pyproject.toml)
 virtualenv==20.21.0
     # via pre-commit
```

### Comparing `feed-archiver-1.0.0b11/requirements/py39/user.txt` & `feed-archiver-2.0.0b0/requirements/py311/user.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,47 +1,45 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile --output-file=requirements/py39/user.txt --resolver=backtracking pyproject.toml
+#    pip-compile --output-file=requirements/py311/user.txt --resolver=backtracking pyproject.toml
 #
 anyio==3.6.2
     # via httpcore
-argcomplete==2.1.2
+argcomplete==3.0.5
     # via feed-archiver (pyproject.toml)
 arrapi==1.4.2
     # via feed-archiver (pyproject.toml)
 certifi==2022.12.7
     # via
     #   httpcore
     #   httpx
     #   requests
 charset-normalizer==3.1.0
     # via requests
 feedparser==6.0.10
     # via feed-archiver (pyproject.toml)
 h11==0.14.0
     # via httpcore
-httpcore==0.16.3
+httpcore==0.17.0
     # via httpx
-httpx==0.23.3
+httpx==0.24.0
     # via feed-archiver (pyproject.toml)
 idna==3.4
     # via
     #   anyio
+    #   httpx
     #   requests
-    #   rfc3986
 lxml==4.9.2
     # via feed-archiver (pyproject.toml)
 pyyaml==6.0
     # via feed-archiver (pyproject.toml)
 requests==2.28.2
     # via arrapi
-rfc3986[idna2008]==1.5.0
-    # via httpx
 sgmllib3k==1.0.0
     # via feedparser
 six==1.16.0
     # via user-agent
 sniffio==1.3.0
     # via
     #   anyio
```

### Comparing `feed-archiver-1.0.0b11/server/docker-compose.yml` & `feed-archiver-2.0.0b0/server/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/setup.cfg` & `feed-archiver-2.0.0b0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -63,20 +63,21 @@
 	coverage
 	prospector[with_everything]
 	xenon
 	rstcheck
 	black
 	autoflake
 	autopep8
-	lxml-stubs
-	types-PyYAML
 	pip-tools
 	setuptools_scm
 	towncrier
 	build
+	lxml-stubs
+	types-requests
+	types-PyYAML
 
 [tool:pytest]
 testpaths = src/feedarchiver
 
 [coverage:run]
 command_line = -m pytest --junit-xml=pytest-junit.xml
 branch = True
```

### Comparing `feed-archiver-1.0.0b11/src/feed_archiver.egg-info/PKG-INFO` & `feed-archiver-2.0.0b0/src/feed_archiver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feed-archiver
-Version: 1.0.0b11
+Version: 2.0.0b0
 Summary: Archive the full contents of RSS/Atom syndication feeds including enclosures and assets.
 Home-page: https://gitlab.com/rpatterson/feed-archiver
 Author: Ross Patterson
 Author-email: me@rpatterson.net
 License: MIT
 Keywords: template,structure
 Classifier: Development Status :: 4 - Beta
@@ -452,15 +452,15 @@
 .. _Sonarr: https://sonarr.tv
 .. _connect to the Sonarr API: https://github.com/Sonarr/Sonarr/wiki/API#url
 .. _look up the TV show/series: https://github.com/Sonarr/Sonarr/wiki/Series#getid
 .. _lookup the episode file: https://github.com/Sonarr/Sonarr/wiki/Episode#get
 
 .. _the Docker image: https://hub.docker.com/r/merpatterson/feed-archiver
 .. _`the example ./docker-compose.yml file`:
-   https://gitlab.com/rpatterson/feed-archiver/blob/master/docker-compose.yml
+   https://gitlab.com/rpatterson/feed-archiver/blob/main/docker-compose.yml
 
 .. _`This project is hosted on GitLab`:
    https://gitlab.com/rpatterson/feed-archiver
 .. _`a mirror on GitHub`:
    https://github.com/rpatterson/feed-archiver
 .. _`the ./CONTRIBUTING.rst file`:
    https://gitlab.com/rpatterson/feed-archiver/blob/main/CONTRIBUTING.rst
```

### Comparing `feed-archiver-1.0.0b11/src/feed_archiver.egg-info/SOURCES.txt` & `feed-archiver-2.0.0b0/src/feed_archiver.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,14 @@
 src/feedarchiver/formats.py
 src/feedarchiver/utils.py
 src/feedarchiver/version.py
 src/feedarchiver/enclosures/__init__.py
 src/feedarchiver/enclosures/servarr.py
 src/feedarchiver/enclosures/template.py
 src/feedarchiver/newsfragments/.gitignore
-src/feedarchiver/newsfragments/request-timeouts.fix.rst
 src/feedarchiver/tests/__init__.py
 src/feedarchiver/tests/test_archive.py
 src/feedarchiver/tests/test_cli.py
 src/feedarchiver/tests/test_download.py
 src/feedarchiver/tests/test_feed.py
 src/feedarchiver/tests/test_linking.py
 src/feedarchiver/tests/test_urls.py
```

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/__init__.py` & `feed-archiver-2.0.0b0/src/feedarchiver/__init__.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/archive.py` & `feed-archiver-2.0.0b0/src/feedarchiver/archive.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/enclosures/__init__.py` & `feed-archiver-2.0.0b0/src/feedarchiver/enclosures/__init__.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/enclosures/servarr.py` & `feed-archiver-2.0.0b0/src/feedarchiver/enclosures/servarr.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/enclosures/template.py` & `feed-archiver-2.0.0b0/src/feedarchiver/enclosures/template.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/feed.py` & `feed-archiver-2.0.0b0/src/feedarchiver/feed.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/formats.py` & `feed-archiver-2.0.0b0/src/feedarchiver/formats.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/tests/__init__.py` & `feed-archiver-2.0.0b0/src/feedarchiver/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/tests/archives/downloads/.feed-archiver.yml` & `feed-archiver-2.0.0b0/src/feedarchiver/tests/archives/downloads/.feed-archiver.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/tests/archives/end-to-end/.feed-archiver.yml.in` & `feed-archiver-2.0.0b0/src/feedarchiver/tests/archives/end-to-end/.feed-archiver.yml.in`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/tests/archives/relink/.feed-archiver.yml` & `feed-archiver-2.0.0b0/src/feedarchiver/tests/archives/relink/.feed-archiver.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/tests/archives/relink-wo-suffix/.feed-archiver.yml` & `feed-archiver-2.0.0b0/src/feedarchiver/tests/archives/relink-wo-suffix/.feed-archiver.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/common-id.mp3` & `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/common-id.mp3`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/el-ni%25C3%25B1o.mp3` & `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/el-ni%25C3%25B1o.mp3`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/common-id.mp3` & `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/common-id.mp3`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/download.mp3` & `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/download.mp3`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/index.html` & `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/index.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/download` & `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/download`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/el-ni%25C3%25B1o.png` & `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/el-ni%25C3%25B1o.png`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/index.html` & `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/index.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/fred-episode-title/download` & `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/fred-episode-title/download`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/garply-bonus-episode/download.mp3` & `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/garply-bonus-episode/download.mp3`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/feed.rss` & `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/feed.rss`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/image.png` & `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/image.png`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/index.html` & `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/index.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/1` & `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/1`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/2` & `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/2`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/3` & `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/3`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/main.html` & `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/main.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss` & `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/feeds/waldo` & `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/feeds/waldo`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/1` & `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/1`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/2` & `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/2`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/3` & `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/3`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/main.html` & `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/main.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/feeds/waldo` & `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/feeds/waldo`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/1` & `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/1`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/2` & `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/2`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/3` & `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/3`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/main.html` & `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/main.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss` & `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/feeds/waldo` & `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/feeds/waldo`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/1` & `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/1`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/2` & `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/2`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/3` & `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/3`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/main.html` & `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/main.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss` & `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/feeds/waldo` & `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/feeds/waldo`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/1` & `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/1`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/2` & `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/2`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/3` & `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/3`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/main.html` & `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/main.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss` & `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/waldo` & `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/waldo`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/tests/test_archive.py` & `feed-archiver-2.0.0b0/src/feedarchiver/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/tests/test_cli.py` & `feed-archiver-2.0.0b0/src/feedarchiver/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/tests/test_download.py` & `feed-archiver-2.0.0b0/src/feedarchiver/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/tests/test_feed.py` & `feed-archiver-2.0.0b0/src/feedarchiver/tests/test_feed.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/tests/test_linking.py` & `feed-archiver-2.0.0b0/src/feedarchiver/tests/test_linking.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/tests/test_urls.py` & `feed-archiver-2.0.0b0/src/feedarchiver/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/src/feedarchiver/utils.py` & `feed-archiver-2.0.0b0/src/feedarchiver/utils.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-1.0.0b11/tox.ini` & `feed-archiver-2.0.0b0/tox.ini`

 * *Files identical despite different names*

