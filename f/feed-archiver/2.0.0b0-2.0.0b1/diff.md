# Comparing `tmp/feed-archiver-2.0.0b0.tar.gz` & `tmp/feed-archiver-2.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feed-archiver-2.0.0b0.tar", last modified: Sat Apr 15 22:29:47 2023, max compression
+gzip compressed data, was "feed-archiver-2.0.0b1.tar", last modified: Sun Apr 16 17:35:48 2023, max compression
```

## Comparing `feed-archiver-2.0.0b0.tar` & `feed-archiver-2.0.0b1.tar`

### file list

```diff
@@ -1,250 +1,250 @@
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.214660 feed-archiver-2.0.0b0/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      543 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/.dir-locals.el.in
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1661 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/.dockerignore
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1115 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/.env.in
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.202660 feed-archiver-2.0.0b0/.github/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/.github/workflows/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3944 2023-04-15 21:45:16.000000 feed-archiver-2.0.0b0/.github/workflows/build-test.yml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1661 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/.gitignore
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4472 2023-04-15 21:45:16.000000 feed-archiver-2.0.0b0/.gitlab-ci.yml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      779 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/.pre-commit-config.yaml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2442 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/.prospector.yaml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4121 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/CONTRIBUTING.rst
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2482 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/Dockerfile
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2747 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/Dockerfile.devel
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1081 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/LICENSE
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    61264 2023-04-15 22:18:59.000000 feed-archiver-2.0.0b0/Makefile
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      205 2023-04-15 22:20:07.000000 feed-archiver-2.0.0b0/NEWS-VERSION.rst
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3823 2023-04-15 22:20:08.000000 feed-archiver-2.0.0b0/NEWS.rst
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)    22909 2023-04-15 22:29:47.214660 feed-archiver-2.0.0b0/PKG-INFO
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    21849 2023-04-15 21:45:16.000000 feed-archiver-2.0.0b0/README.rst
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3758 2023-04-15 21:45:16.000000 feed-archiver-2.0.0b0/TODO.rst
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/bin/
--rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)     2792 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/bin/cz-check-bump
--rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)      936 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/bin/entrypoint
--rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)     1101 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/bin/get-base-version
--rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)      321 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/bin/hadolint
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/build-host/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2002 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/build-host/Dockerfile
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1476 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/build-host/Makefile
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      746 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/build-host/README.rst
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/build-host/bin/
--rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)     2047 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/build-host/bin/entrypoint
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      731 2023-04-15 22:20:35.000000 feed-archiver-2.0.0b0/build-host/requirements-py310.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      674 2023-04-15 22:20:35.000000 feed-archiver-2.0.0b0/build-host/requirements-py311.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      948 2023-04-15 22:20:35.000000 feed-archiver-2.0.0b0/build-host/requirements-py37.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      729 2023-04-15 22:20:35.000000 feed-archiver-2.0.0b0/build-host/requirements-py38.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      729 2023-04-15 22:20:35.000000 feed-archiver-2.0.0b0/build-host/requirements-py39.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)        4 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/build-host/requirements.txt.in
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/dist/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      122 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/dist/.gitignore
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      954 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/docker-compose-servarr.yml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5675 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/docker-compose.override.yml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      927 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/docker-compose.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/gitlab-runner/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       46 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/gitlab-runner/.gitignore
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/gitlab-runner/config/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1323 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/gitlab-runner/config/config.toml.in
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/home/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       64 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/home/.gitignore
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      327 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/home/.pypirc.in
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      111 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/link-fallbacks.feature.rst
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/nginx/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/nginx/templates/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1086 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/nginx/templates/default.conf.template
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2940 2023-04-15 22:20:09.000000 feed-archiver-2.0.0b0/pyproject.toml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/requirements/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      578 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/requirements/build.txt.in
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/requirements/py310/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2414 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/requirements/py310/build.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     6384 2023-04-15 22:20:35.000000 feed-archiver-2.0.0b0/requirements/py310/devel.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1140 2023-04-15 22:20:35.000000 feed-archiver-2.0.0b0/requirements/py310/user.txt
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/requirements/py311/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2414 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/requirements/py311/build.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     6135 2023-04-15 22:20:35.000000 feed-archiver-2.0.0b0/requirements/py311/devel.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1140 2023-04-15 22:20:35.000000 feed-archiver-2.0.0b0/requirements/py311/user.txt
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/requirements/py37/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2645 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/requirements/py37/build.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     7083 2023-04-15 22:20:35.000000 feed-archiver-2.0.0b0/requirements/py37/devel.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1487 2023-04-15 22:20:35.000000 feed-archiver-2.0.0b0/requirements/py37/user.txt
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/requirements/py38/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2515 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/requirements/py38/build.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     6424 2023-04-15 22:20:35.000000 feed-archiver-2.0.0b0/requirements/py38/devel.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1138 2023-04-15 22:20:35.000000 feed-archiver-2.0.0b0/requirements/py38/user.txt
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/requirements/py39/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2412 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/requirements/py39/build.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     6411 2023-04-15 22:20:35.000000 feed-archiver-2.0.0b0/requirements/py39/devel.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1138 2023-04-15 22:20:35.000000 feed-archiver-2.0.0b0/requirements/py39/user.txt
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/server/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4397 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/server/docker-compose.yml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2136 2023-04-15 22:29:47.214660 feed-archiver-2.0.0b0/setup.cfg
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/src/feed_archiver.egg-info/
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)    22909 2023-04-15 22:29:47.000000 feed-archiver-2.0.0b0/src/feed_archiver.egg-info/PKG-INFO
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     7309 2023-04-15 22:29:47.000000 feed-archiver-2.0.0b0/src/feed_archiver.egg-info/SOURCES.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)        1 2023-04-15 22:29:47.000000 feed-archiver-2.0.0b0/src/feed_archiver.egg-info/dependency_links.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      277 2023-04-15 22:29:47.000000 feed-archiver-2.0.0b0/src/feed_archiver.egg-info/entry_points.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      360 2023-04-15 22:29:47.000000 feed-archiver-2.0.0b0/src/feed_archiver.egg-info/requires.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)       13 2023-04-15 22:29:47.000000 feed-archiver-2.0.0b0/src/feed_archiver.egg-info/top_level.txt
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/src/feedarchiver/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5287 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/src/feedarchiver/__init__.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      201 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/__main__.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    11802 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/src/feedarchiver/archive.py
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/src/feedarchiver/enclosures/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3371 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/src/feedarchiver/enclosures/__init__.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     8155 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/src/feedarchiver/enclosures/servarr.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1968 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/src/feedarchiver/enclosures/template.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    34925 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/src/feedarchiver/feed.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     7074 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/src/feedarchiver/formats.py
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/src/feedarchiver/newsfragments/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       91 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/newsfragments/.gitignore
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/src/feedarchiver/tests/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     9888 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/__init__.py
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/archives/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/src/feedarchiver/tests/archives/downloads/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1349 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/archives/downloads/.feed-archiver.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/src/feedarchiver/tests/archives/empty/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       32 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/archives/empty/.gitignore
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/src/feedarchiver/tests/archives/empty-feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       60 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/archives/empty-feeds/.feed-archiver.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/src/feedarchiver/tests/archives/empty-items/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      337 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/archives/empty-items/.feed-archiver.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/src/feedarchiver/tests/archives/end-to-end/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      962 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/archives/end-to-end/.feed-archiver.yml.in
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/src/feedarchiver/tests/archives/relink/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      936 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/archives/relink/.feed-archiver.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/src/feedarchiver/tests/archives/relink-wo-suffix/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      932 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/archives/relink-wo-suffix/.feed-archiver.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/src/feedarchiver/tests/archives/simple/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      228 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/archives/simple/.feed-archiver.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/http/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      243 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/episode%3Fapikey=secret%26seriesId=7
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      224 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/episodeFile%3Fapikey=secret%26seriesId=7
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/series/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       91 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/series/7%3Fapikey=secret
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      105 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/series%3Fapikey=secret
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/common-id.mp3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/el-ni%25C3%25B1o.mp3
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/common-id.mp3
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/download.mp3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/index.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/download
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3435 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/el-ni%25C3%25B1o.png
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/index.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/fred-episode-title/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/fred-episode-title/download
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/garply-bonus-episode/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/garply-bonus-episode/download.mp3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5617 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/feed.rss
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3435 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/image.png
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/index.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/empty-items/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/empty-items/orig/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/empty-items/orig/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/empty-items/orig/https/foo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.210660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/empty-items/orig/https/foo.example.com/podcast/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      405 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/empty-items/orig/https/foo.example.com/podcast/empty.rss
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/added-item/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/added-item/http/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.214660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.214660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/1
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/2
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/main.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/added-item/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.214660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1186 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.214660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/feeds/waldo
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/empty/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/empty/http/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.214660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.214660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/1
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/2
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/main.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/empty/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/empty/https/foo-username%3Asecret@grault.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.214660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/empty/https/foo-username%3Asecret@grault.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       92 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/empty/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.214660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/feeds/waldo
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/orig/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/orig/http/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.214660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.214660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/1
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/2
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/main.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/orig/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.214660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      831 1980-11-25 08:31:00.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.214660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/feeds/waldo
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/removed-item/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/removed-item/http/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.214660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.214660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/1
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/2
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/main.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/removed-item/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.214660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      841 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.214660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/feeds/waldo
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/reordered-item/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.214660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.214660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/1
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/2
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/main.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/reordered-item/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.214660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1550 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.206660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-15 22:29:47.214660 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-15 21:28:30.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/waldo
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3286 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/test_archive.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4257 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/test_cli.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    10833 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/test_download.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    15051 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/test_feed.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     7436 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/test_linking.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2165 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/src/feedarchiver/tests/test_urls.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     8147 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/src/feedarchiver/utils.py
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      162 2023-04-15 22:29:47.000000 feed-archiver-2.0.0b0/src/feedarchiver/version.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3362 2023-04-15 21:32:20.000000 feed-archiver-2.0.0b0/tox.ini
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      543 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/.dir-locals.el.in
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1661 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/.dockerignore
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1115 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/.env.in
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.059723 feed-archiver-2.0.0b1/.github/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/.github/workflows/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3944 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/.github/workflows/build-test.yml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1661 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/.gitignore
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4472 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/.gitlab-ci.yml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      779 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/.pre-commit-config.yaml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2442 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/.prospector.yaml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4121 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/CONTRIBUTING.rst
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2482 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/Dockerfile
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2747 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/Dockerfile.devel
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1081 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/LICENSE
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    61244 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/Makefile
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      180 2023-04-16 17:24:44.000000 feed-archiver-2.0.0b1/NEWS-VERSION.rst
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3567 2023-04-16 17:24:46.000000 feed-archiver-2.0.0b1/NEWS.rst
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)    22909 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/PKG-INFO
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    21849 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/README.rst
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3758 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/TODO.rst
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/bin/
+-rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)     2792 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/bin/cz-check-bump
+-rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)      936 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/bin/entrypoint
+-rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)     1101 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/bin/get-base-version
+-rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)      321 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/bin/hadolint
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/build-host/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2002 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/build-host/Dockerfile
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1476 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/build-host/Makefile
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      746 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/build-host/README.rst
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/build-host/bin/
+-rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)     2047 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/build-host/bin/entrypoint
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      731 2023-04-16 17:25:05.000000 feed-archiver-2.0.0b1/build-host/requirements-py310.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      674 2023-04-16 17:25:05.000000 feed-archiver-2.0.0b1/build-host/requirements-py311.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      948 2023-04-16 17:25:05.000000 feed-archiver-2.0.0b1/build-host/requirements-py37.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      729 2023-04-16 17:25:05.000000 feed-archiver-2.0.0b1/build-host/requirements-py38.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      729 2023-04-16 17:25:05.000000 feed-archiver-2.0.0b1/build-host/requirements-py39.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)        4 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/build-host/requirements.txt.in
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/dist/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      122 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/dist/.gitignore
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      954 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/docker-compose-servarr.yml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5687 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/docker-compose.override.yml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      927 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/docker-compose.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/gitlab-runner/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       46 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/gitlab-runner/.gitignore
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/gitlab-runner/config/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1323 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/gitlab-runner/config/config.toml.in
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/home/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       64 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/home/.gitignore
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      327 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/home/.pypirc.in
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      111 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/link-fallbacks.feature.rst
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.059723 feed-archiver-2.0.0b1/nginx/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/nginx/templates/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1086 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/nginx/templates/default.conf.template
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2940 2023-04-16 17:24:46.000000 feed-archiver-2.0.0b1/pyproject.toml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/requirements/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      578 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/requirements/build.txt.in
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/requirements/py310/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2414 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/requirements/py310/build.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     6384 2023-04-16 17:25:05.000000 feed-archiver-2.0.0b1/requirements/py310/devel.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1140 2023-04-16 17:25:05.000000 feed-archiver-2.0.0b1/requirements/py310/user.txt
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/requirements/py311/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2414 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/requirements/py311/build.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     6135 2023-04-16 17:25:05.000000 feed-archiver-2.0.0b1/requirements/py311/devel.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1140 2023-04-16 17:25:05.000000 feed-archiver-2.0.0b1/requirements/py311/user.txt
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/requirements/py37/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2645 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/requirements/py37/build.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     7097 2023-04-16 17:25:05.000000 feed-archiver-2.0.0b1/requirements/py37/devel.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1487 2023-04-16 17:25:05.000000 feed-archiver-2.0.0b1/requirements/py37/user.txt
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/requirements/py38/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2515 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/requirements/py38/build.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     6424 2023-04-16 17:25:05.000000 feed-archiver-2.0.0b1/requirements/py38/devel.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1138 2023-04-16 17:25:05.000000 feed-archiver-2.0.0b1/requirements/py38/user.txt
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/requirements/py39/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2412 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/requirements/py39/build.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     6411 2023-04-16 17:25:05.000000 feed-archiver-2.0.0b1/requirements/py39/devel.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1138 2023-04-16 17:25:05.000000 feed-archiver-2.0.0b1/requirements/py39/user.txt
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/server/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4397 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/server/docker-compose.yml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2136 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/setup.cfg
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.059723 feed-archiver-2.0.0b1/src/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/src/feed_archiver.egg-info/
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)    22909 2023-04-16 17:35:48.000000 feed-archiver-2.0.0b1/src/feed_archiver.egg-info/PKG-INFO
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     7309 2023-04-16 17:35:48.000000 feed-archiver-2.0.0b1/src/feed_archiver.egg-info/SOURCES.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)        1 2023-04-16 17:35:48.000000 feed-archiver-2.0.0b1/src/feed_archiver.egg-info/dependency_links.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      277 2023-04-16 17:35:48.000000 feed-archiver-2.0.0b1/src/feed_archiver.egg-info/entry_points.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      360 2023-04-16 17:35:48.000000 feed-archiver-2.0.0b1/src/feed_archiver.egg-info/requires.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)       13 2023-04-16 17:35:48.000000 feed-archiver-2.0.0b1/src/feed_archiver.egg-info/top_level.txt
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5287 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/__init__.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      201 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/__main__.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    11802 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/archive.py
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/enclosures/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3371 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/enclosures/__init__.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     8155 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/enclosures/servarr.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1968 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/enclosures/template.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    34925 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/feed.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     7074 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/formats.py
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/newsfragments/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       91 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/newsfragments/.gitignore
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     9888 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/__init__.py
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.059723 feed-archiver-2.0.0b1/src/feedarchiver/tests/archives/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/archives/downloads/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1349 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/archives/downloads/.feed-archiver.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/archives/empty/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       32 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/archives/empty/.gitignore
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/archives/empty-feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       60 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/archives/empty-feeds/.feed-archiver.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/archives/empty-items/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      337 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/archives/empty-items/.feed-archiver.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/archives/end-to-end/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      962 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/archives/end-to-end/.feed-archiver.yml.in
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/archives/relink/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      936 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/archives/relink/.feed-archiver.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/archives/relink-wo-suffix/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      932 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/archives/relink-wo-suffix/.feed-archiver.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/archives/simple/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      228 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/archives/simple/.feed-archiver.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.059723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.059723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.059723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.059723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/http/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.059723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.059723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      243 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/episode%3Fapikey=secret%26seriesId=7
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      224 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/episodeFile%3Fapikey=secret%26seriesId=7
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/series/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       91 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/series/7%3Fapikey=secret
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      105 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/series%3Fapikey=secret
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.059723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.059723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/common-id.mp3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/el-ni%25C3%25B1o.mp3
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.059723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/common-id.mp3
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.059723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/download.mp3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/index.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/download
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3435 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/el-ni%25C3%25B1o.png
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/index.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/fred-episode-title/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/fred-episode-title/download
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/garply-bonus-episode/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/garply-bonus-episode/download.mp3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5617 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/feed.rss
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3435 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/image.png
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/index.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.059723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/empty-items/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.059723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/empty-items/orig/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.059723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/empty-items/orig/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.059723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/empty-items/orig/https/foo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/empty-items/orig/https/foo.example.com/podcast/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      405 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/empty-items/orig/https/foo.example.com/podcast/empty.rss
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.059723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/added-item/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.059723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/added-item/http/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.059723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/1
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/2
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/main.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.059723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/added-item/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.059723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1186 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.059723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/feeds/waldo
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.059723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/empty/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.059723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/empty/http/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.059723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/1
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/2
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/main.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/empty/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/empty/https/foo-username%3Asecret@grault.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/empty/https/foo-username%3Asecret@grault.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       92 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/empty/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/feeds/waldo
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/orig/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/orig/http/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/1
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/2
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/main.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/orig/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      831 1980-11-25 08:31:00.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/feeds/waldo
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/removed-item/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/removed-item/http/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/1
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/2
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/main.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/removed-item/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      841 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/feeds/waldo
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/reordered-item/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/reordered-item/http/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/1
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/2
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/main.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/reordered-item/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1550 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.063723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-16 17:35:48.067723 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/waldo
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3286 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/test_archive.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4257 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/test_cli.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    10833 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/test_download.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    15051 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/test_feed.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     7436 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/test_linking.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2165 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/tests/test_urls.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     8147 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/src/feedarchiver/utils.py
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      162 2023-04-16 17:35:48.000000 feed-archiver-2.0.0b1/src/feedarchiver/version.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3362 2023-04-16 17:23:28.000000 feed-archiver-2.0.0b1/tox.ini
```

### Comparing `feed-archiver-2.0.0b0/.dir-locals.el.in` & `feed-archiver-2.0.0b1/.dir-locals.el.in`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/.dockerignore` & `feed-archiver-2.0.0b1/.dockerignore`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/.env.in` & `feed-archiver-2.0.0b1/.env.in`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/.github/workflows/build-test.yml` & `feed-archiver-2.0.0b1/.github/workflows/build-test.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/.gitignore` & `feed-archiver-2.0.0b1/.gitignore`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/.gitlab-ci.yml` & `feed-archiver-2.0.0b1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/.pre-commit-config.yaml` & `feed-archiver-2.0.0b1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/.prospector.yaml` & `feed-archiver-2.0.0b1/.prospector.yaml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/CONTRIBUTING.rst` & `feed-archiver-2.0.0b1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/Dockerfile` & `feed-archiver-2.0.0b1/Dockerfile`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/Dockerfile.devel` & `feed-archiver-2.0.0b1/Dockerfile.devel`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/LICENSE` & `feed-archiver-2.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/Makefile` & `feed-archiver-2.0.0b1/Makefile`

 * *Files 0% similar despite different names*

```diff
@@ -889,29 +889,28 @@
 		./var/git/refs/remotes/$(VCS_REMOTE)/$(VCS_BRANCH) \
 		./var/log/git-remotes.log
 	remote_branch_exists=false
 	if git fetch "$(VCS_REMOTE)" "$(VCS_BRANCH)-upgrade"
 	then
 	    remote_branch_exists=true
 	fi
-	git switch -C "$(VCS_BRANCH)-upgrade" --track "$(VCS_REMOTE)/$(VCS_BRANCH)" --
+	git switch -C "$(VCS_BRANCH)-upgrade" --track "$(VCS_BRANCH)" --
 	now=$$(date -u)
 	$(MAKE) -e devel-upgrade
 	if $(MAKE) -e "test-clean"
 	then
 # No changes from upgrade, exit successfully but push nothing
 	    exit
 	fi
 # Commit the upgrade changes
 	echo "Upgrade all requirements to the latest versions as of $${now}." \
-	    >"./src/feedarchiver/newsfragments/upgrade-requirements.bugfix.rst"
+	    >"./src/feedarchiver/newsfragments/+upgrade-requirements.bugfix.rst"
 	git add --update './build-host/requirements-*.txt' './requirements/*/*.txt' \
 	    "./.pre-commit-config.yaml"
-	git add \
-	    "./src/feedarchiver/newsfragments/upgrade-requirements.bugfix.rst"
+	git add "./src/feedarchiver/newsfragments/+upgrade-requirements.bugfix.rst"
 	git_commit_args="--all --gpg-sign"
 ifeq ($(CI),true)
 # Don't duplicate the CI run from the push below:
 	git_push_args+=" --no-verify"
 endif
 	git commit $${git_commit_args} -m \
 	    "fix(deps): Upgrade requirements latest versions"
@@ -1052,15 +1051,15 @@
 	    touch "$(@)" "./var/docker/$(PYTHON_ENV)/log/rebuild.log"
 # Ensure the virtualenv in the volume is also current:
 	    docker compose run $(DOCKER_COMPOSE_RUN_ARGS) \
 	        feed-archiver-devel make -e PYTHON_MINORS="$(PYTHON_MINOR)" \
 	        "./var/log/tox/$(PYTHON_ENV)/build.log"
 	    exit
 	fi
-else
+endif
 # https://github.com/moby/moby/issues/39003#issuecomment-879441675
 	docker_build_args="$(DOCKER_BUILD_ARGS) \
 	    --build-arg BUILDKIT_INLINE_CACHE=1 \
 	    --build-arg PYTHON_MINOR=$(PYTHON_MINOR) \
 	    --build-arg PYTHON_ENV=$(PYTHON_ENV) \
 	    --build-arg VERSION=$${VERSION}"
 	docker_build_devel_tags=""
@@ -1117,15 +1116,14 @@
 ifeq ($(CI),true)
 # On CI, any changes from compiling requirements is a failure so no need to waste time
 # rebuilding images:
 	touch "$(@)"
 else
 	$(MAKE) -e "$(@)"
 endif
-endif
 
 # Build the end-user image:
 ./var/docker/$(PYTHON_ENV)/log/build-user.log: \
 		./var/docker/$(PYTHON_ENV)/log/build-devel.log ./Dockerfile \
 		./var/docker/$(PYTHON_ENV)/log/rebuild.log
 	true DEBUG Updated prereqs: $(?)
 	$(MAKE) -e "./var/git/refs/remotes/$(VCS_REMOTE)/$(VCS_BRANCH)" \
@@ -1493,15 +1491,15 @@
 	echo "ERROR: GPG_SIGNING_PRIVATE_KEY or GPG_PASSPHRASE " \
 	    "missing from ./.env or CI secrets"
 	false
 endif
 	date | tee -a "$(@)"
 endif
 
-./gitlab-runner/config/config.toml: ./gitlab-runner/config/config.toml.in
+./var/gitlab-runner/config/config.toml: ./gitlab-runner/config/config.toml.in
 	docker compose run --rm gitlab-runner register \
 	    --url "https://gitlab.com/" --docker-image "docker" --executor "docker"
 
 
 ## Utility Targets:
 #
 # Recipes used to make similar changes across targets where using Make's basic syntax
```

### Comparing `feed-archiver-2.0.0b0/NEWS.rst` & `feed-archiver-2.0.0b1/NEWS.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,128 +1,137 @@
+feed-archiver 2.0.0b1 (2023-04-16)
+==================================
+
+Bugfixes
+--------
+
+- Upgrade all requirements to the latest versions as of Sun Apr 16 03:54:21 PM UTC 2023.
+
+
 feed-archiver 2.0.0b0 (2023-04-15)
 ==================================
 
 Bugfixes
 --------
 
 - Restore correct versions going forward.  Versions from here to v1.0.0 below are
-  incorrect. (correct-versions)
+  incorrect.
 
 
 feed-archiver 1.0.0b11 (2023-04-15)
 ===================================
 
 Bugfixes
 --------
 
-- Upgrade all requirements to the latest versions as of Sat Apr 15 06:11:17 PM UTC 2023. (upgrade-requirements)
+- Upgrade all requirements to the latest versions as of Sat Apr 15 06:11:17 PM UTC 2023.
 
 
 Feedarchiver 1.0.0b10 (2023-03-15)
 ==================================
 
 Features
 --------
 
-- Address a Bandit warning about requests without timeouts. (request-timeouts)
-- Write an ``./index.html`` file listing links to archived feeds. (archive-index)
+- Address a Bandit warning about requests without timeouts.
+- Write an ``./index.html`` file listing links to archived feeds.
 - Rename the ``link-paths`` plugin system to a more accurate name, ``enclosures``.  Note
   that this requires an update to existing archive configurations using ``link-paths``
-  plugins. (enclosure-plugin-rename)
+  plugins.
 - Replace ``content`` term with more correct ``enclosure`` term.  Requires running the ``$
-  feed-archiver relink`` sub-command to update existing archives. (enclosure-term)
+  feed-archiver relink`` sub-command to update existing archives.
 - Avoid unintended sub-directories in link path plugin template paths, add support for
-  quoting path separators in plugin configuration. (link-quote-path-sep)
+  quoting path separators in plugin configuration.
 - Make a parsed version of the feed and item with richer data available to link path
-  plugin configurations, e.g. dates and times. (link-rich-parser)
+  plugin configurations, e.g. dates and times.
 - Provide access to regular expression symbolic group names in the ``template`` plugins
-  format strings. (re-group-names)
+  format strings.
 - Improve link plugin template usability by providing the ``basename`` via a
-  ``pathlib.Path`` object and use that to improve the default enclosure link basename. (template-url-path)
+  ``pathlib.Path`` object and use that to improve the default enclosure link basename.
 
 
 Bugfixes
 --------
 
-- Fix an error when backup feed XML is present in the archive. (feed-backups)
-- Filter out duplicate link paths returned from plugins. (link-duplicates)
+- Fix an error when backup feed XML is present in the archive.
+- Filter out duplicate link paths returned from plugins.
 
 
 Feedarchiver 1.0.0b9 (2023-02-22)
 =================================
 
 Features
 --------
 
-- Support all currently maintained versions of Python. (python-versions)
+- Support all currently maintained versions of Python.
 
 
 Feedarchiver 1.0.0b5 (2022-12-22)
 =================================
 
 Features
 --------
 
 - Add the ``$ feed-archiver relink`` sub-command to re-link existing archived feed item
   enclosures as they would be if they had been newly archived by the ``$ feed-archiver
-  update`` sub-command. (relink-item-content)
+  update`` sub-command.
 
 
 Bugfixes
 --------
 
-- Fix the check that the remote feed format (RSS vs Atom) matches the archived feed. (wrong-archive-feed-format-check)
+- Fix the check that the remote feed format (RSS vs Atom) matches the archived feed.
 
 
 Feedarchiver 1.0.0b1 (2022-12-17)
 =================================
 
 Bugfixes
 --------
 
-- Don't report results from the ``update`` sub-command when there are none. (empty-results)
+- Don't report results from the ``update`` sub-command when there are none.
 
 
 Feedarchiver 1.0.0 (2022-12-16)
 ===============================
 
 No significant changes.
 
 
 Feedarchiver 1.0.0b0 (2022-12-16)
 =================================
 
 Features
 --------
 
-- First stable release. (initial-release)
+- First stable release.
 
 
 Feedarchiver 0.1.2b1 (2022-12-16)
 =================================
 
 Deprecations and Removals
 -------------------------
 
-- Remove the archive migration code and sub-command now that the format is stable. (migrate-sub-command)
+- Remove the archive migration code and sub-command now that the format is stable.
 
 
 Feedarchiver 0.1.2b0 (2022-12-16)
 =================================
 
 Bugfixes
 --------
 
 - Tolerate errors when parsing the local archive copy of the feed.  Try to parse the local
   archive version of the feed if possible.  If there are errors parsing it, then treat it
-  as if it's the first time archiving this feed. (archive-feed-parse-errors)
-- Cleanup ``pathlib.Path(...)`` objects in ``$ feed-archiver update`` output. (download-path-output)
+  as if it's the first time archiving this feed.
+- Cleanup ``pathlib.Path(...)`` objects in ``$ feed-archiver update`` output.
 
 
 Feedarchiver 0.1.1b0 (2022-12-14)
 =================================
 
 Bugfixes
 --------
 
 - Add CI/CD pipeline/workflow that also publishes releases.  Force a patch version bump
-  and release to ensure the latest published release artifacts are all the same. (ci-cd-publish-releases)
+  and release to ensure the latest published release artifacts are all the same.
```

### Comparing `feed-archiver-2.0.0b0/PKG-INFO` & `feed-archiver-2.0.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feed-archiver
-Version: 2.0.0b0
+Version: 2.0.0b1
 Summary: Archive the full contents of RSS/Atom syndication feeds including enclosures and assets.
 Home-page: https://gitlab.com/rpatterson/feed-archiver
 Author: Ross Patterson
 Author-email: me@rpatterson.net
 License: MIT
 Keywords: template,structure
 Classifier: Development Status :: 4 - Beta
```

### Comparing `feed-archiver-2.0.0b0/README.rst` & `feed-archiver-2.0.0b1/README.rst`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/TODO.rst` & `feed-archiver-2.0.0b1/TODO.rst`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/bin/cz-check-bump` & `feed-archiver-2.0.0b1/bin/cz-check-bump`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/bin/entrypoint` & `feed-archiver-2.0.0b1/bin/entrypoint`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/bin/get-base-version` & `feed-archiver-2.0.0b1/bin/get-base-version`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/build-host/Dockerfile` & `feed-archiver-2.0.0b1/build-host/Dockerfile`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/build-host/Makefile` & `feed-archiver-2.0.0b1/build-host/Makefile`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/build-host/README.rst` & `feed-archiver-2.0.0b1/build-host/README.rst`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/build-host/bin/entrypoint` & `feed-archiver-2.0.0b1/build-host/bin/entrypoint`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/build-host/requirements-py310.txt` & `feed-archiver-2.0.0b1/build-host/requirements-py310.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/build-host/requirements-py311.txt` & `feed-archiver-2.0.0b1/build-host/requirements-py311.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/build-host/requirements-py37.txt` & `feed-archiver-2.0.0b1/build-host/requirements-py37.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/build-host/requirements-py38.txt` & `feed-archiver-2.0.0b1/build-host/requirements-py38.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/build-host/requirements-py39.txt` & `feed-archiver-2.0.0b1/build-host/requirements-py39.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/docker-compose-servarr.yml` & `feed-archiver-2.0.0b1/docker-compose-servarr.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/docker-compose.override.yml` & `feed-archiver-2.0.0b1/docker-compose.override.yml`

 * *Files 2% similar despite different names*

```diff
@@ -155,13 +155,13 @@
 
   # Conserve shared runner minutes, run GitLab CI/CD jobs locally:
   gitlab-runner:
     image: "gitlab/gitlab-runner"
     profiles:
       - "ci"
     volumes:
-      - "./gitlab-runner/config:/etc/gitlab-runner"
+      - "./var/gitlab-runner/config:/etc/gitlab-runner"
       - "/var/run/docker.sock:/var/run/docker.sock"
-      - "./gitlab-runner/cache:/cache"
-      - "./gitlab-runner/certs:/certs"
+      - "./var/gitlab-runner/cache:/cache"
+      - "./var/gitlab-runner/certs:/certs"
     ports:
       - "8093:8093"
```

### Comparing `feed-archiver-2.0.0b0/docker-compose.yml` & `feed-archiver-2.0.0b1/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/gitlab-runner/config/config.toml.in` & `feed-archiver-2.0.0b1/gitlab-runner/config/config.toml.in`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/nginx/templates/default.conf.template` & `feed-archiver-2.0.0b1/nginx/templates/default.conf.template`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/pyproject.toml` & `feed-archiver-2.0.0b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 [tool.commitizen]
 # Parse commit messages according to conventional commits to decide wether the next
 # versin tag should be a major, minor or patch bump and create the VCS tag.  Also
 # provides VCS hooks to enforce that commit messages comply with conventional commits:
 # https://commitizen-tools.github.io/commitizen/
 name = "cz_conventional_commits"
 changelog_start_rev = "v0.0.0"
-version = "2.0.0b0"
+version = "2.0.0b1"
 tag_format = "v$version"
 annotated_tag = true
 gpg_sign = true
 bump_message = """\
 build(release): Version $current_version → $new_version
 
 [actions skip]
```

### Comparing `feed-archiver-2.0.0b0/requirements/build.txt.in` & `feed-archiver-2.0.0b1/requirements/build.txt.in`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/requirements/py310/build.txt` & `feed-archiver-2.0.0b1/requirements/py310/build.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/requirements/py310/devel.txt` & `feed-archiver-2.0.0b1/requirements/py310/devel.txt`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     # via feed-archiver (pyproject.toml)
 astroid==2.15.2
     # via
     #   pylint
     #   pylint-celery
     #   pylint-flask
     #   requirements-detector
-attrs==22.2.0
+attrs==23.1.0
     # via pytest-subtests
 autoflake==1.7.8
     # via feed-archiver (pyproject.toml)
 autopep8==2.0.2
     # via feed-archiver (pyproject.toml)
 bandit==1.7.5
     # via prospector
```

### Comparing `feed-archiver-2.0.0b0/requirements/py310/user.txt` & `feed-archiver-2.0.0b1/requirements/py310/user.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/requirements/py311/build.txt` & `feed-archiver-2.0.0b1/requirements/py311/build.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/requirements/py311/devel.txt` & `feed-archiver-2.0.0b1/requirements/py311/devel.txt`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     # via feed-archiver (pyproject.toml)
 astroid==2.15.2
     # via
     #   pylint
     #   pylint-celery
     #   pylint-flask
     #   requirements-detector
-attrs==22.2.0
+attrs==23.1.0
     # via pytest-subtests
 autoflake==1.7.8
     # via feed-archiver (pyproject.toml)
 autopep8==2.0.2
     # via feed-archiver (pyproject.toml)
 bandit==1.7.5
     # via prospector
```

### Comparing `feed-archiver-2.0.0b0/requirements/py311/user.txt` & `feed-archiver-2.0.0b1/requirements/py311/user.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/requirements/py37/build.txt` & `feed-archiver-2.0.0b1/requirements/py37/build.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/requirements/py37/devel.txt` & `feed-archiver-2.0.0b1/requirements/py37/devel.txt`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     # via feed-archiver (pyproject.toml)
 astroid==2.15.2
     # via
     #   pylint
     #   pylint-celery
     #   pylint-flask
     #   requirements-detector
-attrs==22.2.0
+attrs==23.1.0
     # via pytest-subtests
 autoflake==1.7.8
     # via feed-archiver (pyproject.toml)
 autopep8==2.0.2
     # via feed-archiver (pyproject.toml)
 backports-cached-property==1.0.2 ; python_version < "3.8"
     # via feed-archiver (pyproject.toml)
@@ -103,14 +103,15 @@
     # via
     #   anyio
     #   httpx
     #   requests
 importlib-metadata==4.13.0 ; python_version < "3.8"
     # via
     #   argcomplete
+    #   attrs
     #   build
     #   click
     #   feed-archiver (pyproject.toml)
     #   pluggy
     #   pre-commit
     #   pydocstyle
     #   pytest
```

### Comparing `feed-archiver-2.0.0b0/requirements/py37/user.txt` & `feed-archiver-2.0.0b1/requirements/py37/user.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/requirements/py38/build.txt` & `feed-archiver-2.0.0b1/requirements/py38/build.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/requirements/py38/devel.txt` & `feed-archiver-2.0.0b1/requirements/py38/devel.txt`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     # via feed-archiver (pyproject.toml)
 astroid==2.15.2
     # via
     #   pylint
     #   pylint-celery
     #   pylint-flask
     #   requirements-detector
-attrs==22.2.0
+attrs==23.1.0
     # via pytest-subtests
 autoflake==1.7.8
     # via feed-archiver (pyproject.toml)
 autopep8==2.0.2
     # via feed-archiver (pyproject.toml)
 bandit==1.7.5
     # via prospector
```

### Comparing `feed-archiver-2.0.0b0/requirements/py38/user.txt` & `feed-archiver-2.0.0b1/requirements/py38/user.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/requirements/py39/build.txt` & `feed-archiver-2.0.0b1/requirements/py39/build.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/requirements/py39/devel.txt` & `feed-archiver-2.0.0b1/requirements/py39/devel.txt`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     # via feed-archiver (pyproject.toml)
 astroid==2.15.2
     # via
     #   pylint
     #   pylint-celery
     #   pylint-flask
     #   requirements-detector
-attrs==22.2.0
+attrs==23.1.0
     # via pytest-subtests
 autoflake==1.7.8
     # via feed-archiver (pyproject.toml)
 autopep8==2.0.2
     # via feed-archiver (pyproject.toml)
 bandit==1.7.5
     # via prospector
```

### Comparing `feed-archiver-2.0.0b0/requirements/py39/user.txt` & `feed-archiver-2.0.0b1/requirements/py39/user.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/server/docker-compose.yml` & `feed-archiver-2.0.0b1/server/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/setup.cfg` & `feed-archiver-2.0.0b1/setup.cfg`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feed_archiver.egg-info/PKG-INFO` & `feed-archiver-2.0.0b1/src/feed_archiver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feed-archiver
-Version: 2.0.0b0
+Version: 2.0.0b1
 Summary: Archive the full contents of RSS/Atom syndication feeds including enclosures and assets.
 Home-page: https://gitlab.com/rpatterson/feed-archiver
 Author: Ross Patterson
 Author-email: me@rpatterson.net
 License: MIT
 Keywords: template,structure
 Classifier: Development Status :: 4 - Beta
```

### Comparing `feed-archiver-2.0.0b0/src/feed_archiver.egg-info/SOURCES.txt` & `feed-archiver-2.0.0b1/src/feed_archiver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/__init__.py` & `feed-archiver-2.0.0b1/src/feedarchiver/__init__.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/archive.py` & `feed-archiver-2.0.0b1/src/feedarchiver/archive.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/enclosures/__init__.py` & `feed-archiver-2.0.0b1/src/feedarchiver/enclosures/__init__.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/enclosures/servarr.py` & `feed-archiver-2.0.0b1/src/feedarchiver/enclosures/servarr.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/enclosures/template.py` & `feed-archiver-2.0.0b1/src/feedarchiver/enclosures/template.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/feed.py` & `feed-archiver-2.0.0b1/src/feedarchiver/feed.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/formats.py` & `feed-archiver-2.0.0b1/src/feedarchiver/formats.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/tests/__init__.py` & `feed-archiver-2.0.0b1/src/feedarchiver/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/tests/archives/downloads/.feed-archiver.yml` & `feed-archiver-2.0.0b1/src/feedarchiver/tests/archives/downloads/.feed-archiver.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/tests/archives/end-to-end/.feed-archiver.yml.in` & `feed-archiver-2.0.0b1/src/feedarchiver/tests/archives/end-to-end/.feed-archiver.yml.in`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/tests/archives/relink/.feed-archiver.yml` & `feed-archiver-2.0.0b1/src/feedarchiver/tests/archives/relink/.feed-archiver.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/tests/archives/relink-wo-suffix/.feed-archiver.yml` & `feed-archiver-2.0.0b1/src/feedarchiver/tests/archives/relink-wo-suffix/.feed-archiver.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/common-id.mp3` & `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/common-id.mp3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/el-ni%25C3%25B1o.mp3` & `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/el-ni%25C3%25B1o.mp3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/common-id.mp3` & `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/common-id.mp3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/download.mp3` & `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/download.mp3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/index.html` & `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/index.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/download` & `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/download`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/el-ni%25C3%25B1o.png` & `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/el-ni%25C3%25B1o.png`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/index.html` & `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/index.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/fred-episode-title/download` & `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/fred-episode-title/download`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/garply-bonus-episode/download.mp3` & `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/garply-bonus-episode/download.mp3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/feed.rss` & `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/feed.rss`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/image.png` & `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/image.png`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/index.html` & `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/index.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/1` & `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/1`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/2` & `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/2`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/3` & `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/main.html` & `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/main.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss` & `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/feeds/waldo` & `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/feeds/waldo`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/1` & `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/1`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/2` & `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/2`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/3` & `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/main.html` & `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/main.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/feeds/waldo` & `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/feeds/waldo`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/1` & `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/1`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/2` & `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/2`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/3` & `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/main.html` & `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/main.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss` & `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/feeds/waldo` & `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/feeds/waldo`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/1` & `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/1`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/2` & `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/2`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/3` & `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/main.html` & `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/main.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss` & `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/feeds/waldo` & `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/feeds/waldo`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/1` & `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/1`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/2` & `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/2`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/3` & `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/main.html` & `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/main.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss` & `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/waldo` & `feed-archiver-2.0.0b1/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/waldo`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/tests/test_archive.py` & `feed-archiver-2.0.0b1/src/feedarchiver/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/tests/test_cli.py` & `feed-archiver-2.0.0b1/src/feedarchiver/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/tests/test_download.py` & `feed-archiver-2.0.0b1/src/feedarchiver/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/tests/test_feed.py` & `feed-archiver-2.0.0b1/src/feedarchiver/tests/test_feed.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/tests/test_linking.py` & `feed-archiver-2.0.0b1/src/feedarchiver/tests/test_linking.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/tests/test_urls.py` & `feed-archiver-2.0.0b1/src/feedarchiver/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/src/feedarchiver/utils.py` & `feed-archiver-2.0.0b1/src/feedarchiver/utils.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.0b0/tox.ini` & `feed-archiver-2.0.0b1/tox.ini`

 * *Files identical despite different names*

