# Comparing `tmp/pyds-cli-0.1.4.tar.gz` & `tmp/pyds-cli-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyds-cli-0.1.4.tar", last modified: Wed Apr  5 22:39:32 2023, max compression
+gzip compressed data, was "pyds-cli-0.1.5.tar", last modified: Sun Apr 16 18:13:14 2023, max compression
```

## Comparing `pyds-cli-0.1.4.tar` & `pyds-cli-0.1.5.tar`

### file list

```diff
@@ -1,51 +1,62 @@
-drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-05 22:39:32.186950 pyds-cli-0.1.4/
--rw-r--r--   0 ericmjl    (501) staff       (20)       28 2021-12-12 03:24:31.000000 pyds-cli-0.1.4/MANIFEST.in
--rw-r--r--   0 ericmjl    (501) staff       (20)       52 2023-04-05 22:39:32.186788 pyds-cli-0.1.4/PKG-INFO
--rw-r--r--   0 ericmjl    (501) staff       (20)     2814 2021-12-12 03:24:31.000000 pyds-cli-0.1.4/README.md
-drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-05 22:39:32.178965 pyds-cli-0.1.4/pyds/
-drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-05 22:39:32.178503 pyds-cli-0.1.4/pyds/cli/
-drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-05 22:39:32.182242 pyds-cli-0.1.4/pyds/cli/templates/
--rw-r--r--   0 ericmjl    (501) staff       (20)       98 2023-04-03 18:56:44.000000 pyds-cli-0.1.4/pyds/cli/templates/.bumpversion.cfg.j2
--rw-r--r--   0 ericmjl    (501) staff       (20)       34 2021-11-05 23:29:52.000000 pyds-cli-0.1.4/pyds/cli/templates/.darglint.j2
-drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-05 22:39:32.182866 pyds-cli-0.1.4/pyds/cli/templates/.devcontainer/
--rw-r--r--   0 ericmjl    (501) staff       (20)     2587 2021-11-15 12:34:35.000000 pyds-cli-0.1.4/pyds/cli/templates/.devcontainer/Dockerfile.j2
--rw-r--r--   0 ericmjl    (501) staff       (20)      645 2021-11-15 12:35:38.000000 pyds-cli-0.1.4/pyds/cli/templates/.devcontainer/devcontainer.json.j2
--rw-r--r--   0 ericmjl    (501) staff       (20)      229 2023-04-03 18:58:17.000000 pyds-cli-0.1.4/pyds/cli/templates/.env.j2
--rw-r--r--   0 ericmjl    (501) staff       (20)       29 2021-12-12 03:24:31.000000 pyds-cli-0.1.4/pyds/cli/templates/.flake8.j2
-drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-05 22:39:32.178702 pyds-cli-0.1.4/pyds/cli/templates/.github/
-drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-05 22:39:32.183530 pyds-cli-0.1.4/pyds/cli/templates/.github/workflows/
--rw-r--r--   0 ericmjl    (501) staff       (20)      257 2021-11-15 12:34:35.000000 pyds-cli-0.1.4/pyds/cli/templates/.github/workflows/code-style.yaml.j2
--rw-r--r--   0 ericmjl    (501) staff       (20)     1546 2023-04-03 18:58:17.000000 pyds-cli-0.1.4/pyds/cli/templates/.github/workflows/docs.yaml.j2
--rw-r--r--   0 ericmjl    (501) staff       (20)     1113 2023-04-03 18:58:17.000000 pyds-cli-0.1.4/pyds/cli/templates/.github/workflows/pr-tests.yaml.j2
--rw-r--r--   0 ericmjl    (501) staff       (20)     2312 2023-04-03 18:58:17.000000 pyds-cli-0.1.4/pyds/cli/templates/.gitignore.j2
--rw-r--r--   0 ericmjl    (501) staff       (20)      923 2021-12-12 03:24:31.000000 pyds-cli-0.1.4/pyds/cli/templates/.pre-commit-config.yaml.j2
--rw-r--r--   0 ericmjl    (501) staff       (20)      124 2021-12-12 03:24:31.000000 pyds-cli-0.1.4/pyds/cli/templates/MANIFEST.in.j2
-drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-05 22:39:32.184223 pyds-cli-0.1.4/pyds/cli/templates/docs/
--rw-r--r--   0 ericmjl    (501) staff       (20)       63 2021-12-12 03:24:31.000000 pyds-cli-0.1.4/pyds/cli/templates/docs/api.md.j2
--rw-r--r--   0 ericmjl    (501) staff       (20)      607 2021-12-12 03:24:31.000000 pyds-cli-0.1.4/pyds/cli/templates/docs/apidocs.css.j2
--rw-r--r--   0 ericmjl    (501) staff       (20)       21 2021-12-12 03:24:31.000000 pyds-cli-0.1.4/pyds/cli/templates/docs/config.js.j2
--rw-r--r--   0 ericmjl    (501) staff       (20)      488 2021-12-12 03:24:31.000000 pyds-cli-0.1.4/pyds/cli/templates/docs/index.md.j2
--rw-r--r--   0 ericmjl    (501) staff       (20)      664 2023-04-03 18:58:17.000000 pyds-cli-0.1.4/pyds/cli/templates/environment.yml.j2
--rw-r--r--   0 ericmjl    (501) staff       (20)     1833 2021-12-12 03:24:31.000000 pyds-cli-0.1.4/pyds/cli/templates/mkdocs.yaml.j2
--rw-r--r--   0 ericmjl    (501) staff       (20)     1594 2023-04-05 17:48:28.000000 pyds-cli-0.1.4/pyds/cli/templates/pyproject.toml.j2
--rw-r--r--   0 ericmjl    (501) staff       (20)      212 2023-04-03 18:58:17.000000 pyds-cli-0.1.4/pyds/cli/templates/setup.cfg.j2
-drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-05 22:39:32.185114 pyds-cli-0.1.4/pyds/cli/templates/src/
--rw-r--r--   0 ericmjl    (501) staff       (20)      221 2023-04-03 18:58:17.000000 pyds-cli-0.1.4/pyds/cli/templates/src/__init__.py.j2
--rw-r--r--   0 ericmjl    (501) staff       (20)      659 2021-12-12 03:24:31.000000 pyds-cli-0.1.4/pyds/cli/templates/src/cli.py.j2
--rw-r--r--   0 ericmjl    (501) staff       (20)       48 2021-12-12 03:24:31.000000 pyds-cli-0.1.4/pyds/cli/templates/src/models.py.j2
--rw-r--r--   0 ericmjl    (501) staff       (20)       35 2021-12-12 03:24:31.000000 pyds-cli-0.1.4/pyds/cli/templates/src/preprocessing.py.j2
--rw-r--r--   0 ericmjl    (501) staff       (20)      192 2021-12-12 03:24:31.000000 pyds-cli-0.1.4/pyds/cli/templates/src/schemas.py.j2
--rw-r--r--   0 ericmjl    (501) staff       (20)       40 2021-11-05 23:30:25.000000 pyds-cli-0.1.4/pyds/cli/templates/src/utils.py.j2
-drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-05 22:39:32.185743 pyds-cli-0.1.4/pyds/cli/templates/tests/
--rw-r--r--   0 ericmjl    (501) staff       (20)       36 2021-12-12 03:24:31.000000 pyds-cli-0.1.4/pyds/cli/templates/tests/test___init__.py.j2
--rw-r--r--   0 ericmjl    (501) staff       (20)       40 2021-12-12 03:24:31.000000 pyds-cli-0.1.4/pyds/cli/templates/tests/test_cli.py.j2
--rw-r--r--   0 ericmjl    (501) staff       (20)       62 2021-12-12 03:24:31.000000 pyds-cli-0.1.4/pyds/cli/templates/tests/test_models.py.j2
-drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-05 22:39:32.186588 pyds-cli-0.1.4/pyds/pyds_cli.egg-info/
--rw-r--r--   0 ericmjl    (501) staff       (20)       52 2023-04-05 22:39:32.000000 pyds-cli-0.1.4/pyds/pyds_cli.egg-info/PKG-INFO
--rw-r--r--   0 ericmjl    (501) staff       (20)     1399 2023-04-05 22:39:32.000000 pyds-cli-0.1.4/pyds/pyds_cli.egg-info/SOURCES.txt
--rw-r--r--   0 ericmjl    (501) staff       (20)        1 2023-04-05 22:39:32.000000 pyds-cli-0.1.4/pyds/pyds_cli.egg-info/dependency_links.txt
--rw-r--r--   0 ericmjl    (501) staff       (20)       38 2023-04-05 22:39:32.000000 pyds-cli-0.1.4/pyds/pyds_cli.egg-info/entry_points.txt
--rw-r--r--   0 ericmjl    (501) staff       (20)      172 2023-04-05 22:39:32.000000 pyds-cli-0.1.4/pyds/pyds_cli.egg-info/requires.txt
--rw-r--r--   0 ericmjl    (501) staff       (20)        1 2023-04-05 22:39:32.000000 pyds-cli-0.1.4/pyds/pyds_cli.egg-info/top_level.txt
--rw-r--r--   0 ericmjl    (501) staff       (20)     1654 2023-04-05 22:39:28.000000 pyds-cli-0.1.4/pyproject.toml
--rw-r--r--   0 ericmjl    (501) staff       (20)       38 2023-04-05 22:39:32.186990 pyds-cli-0.1.4/setup.cfg
+drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-16 18:13:14.958077 pyds-cli-0.1.5/
+-rw-r--r--   0 ericmjl    (501) staff       (20)       28 2021-12-12 03:24:31.000000 pyds-cli-0.1.5/MANIFEST.in
+-rw-r--r--   0 ericmjl    (501) staff       (20)       52 2023-04-16 18:13:14.957934 pyds-cli-0.1.5/PKG-INFO
+-rw-r--r--   0 ericmjl    (501) staff       (20)     2814 2021-12-12 03:24:31.000000 pyds-cli-0.1.5/README.md
+drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-16 18:13:14.948399 pyds-cli-0.1.5/pyds/
+drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-16 18:13:14.950232 pyds-cli-0.1.5/pyds/cli/
+-rw-r--r--   0 ericmjl    (501) staff       (20)     1910 2023-04-05 22:38:40.000000 pyds-cli-0.1.5/pyds/cli/__init__.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)      933 2021-12-12 03:24:31.000000 pyds-cli-0.1.5/pyds/cli/conda.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)      398 2021-12-12 03:24:31.000000 pyds-cli-0.1.5/pyds/cli/docs.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)     2858 2021-12-12 03:24:31.000000 pyds-cli-0.1.5/pyds/cli/environment.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)     2516 2023-04-03 18:58:17.000000 pyds-cli-0.1.5/pyds/cli/package.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)     4535 2021-12-12 03:24:31.000000 pyds-cli-0.1.5/pyds/cli/project.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)     2693 2023-04-03 18:58:17.000000 pyds-cli-0.1.5/pyds/cli/system.py
+drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-16 18:13:14.952797 pyds-cli-0.1.5/pyds/cli/templates/
+-rw-r--r--   0 ericmjl    (501) staff       (20)       98 2023-04-03 18:56:44.000000 pyds-cli-0.1.5/pyds/cli/templates/.bumpversion.cfg.j2
+-rw-r--r--   0 ericmjl    (501) staff       (20)       34 2021-11-05 23:29:52.000000 pyds-cli-0.1.5/pyds/cli/templates/.darglint.j2
+drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-16 18:13:14.953365 pyds-cli-0.1.5/pyds/cli/templates/.devcontainer/
+-rw-r--r--   0 ericmjl    (501) staff       (20)     2587 2021-11-15 12:34:35.000000 pyds-cli-0.1.5/pyds/cli/templates/.devcontainer/Dockerfile.j2
+-rw-r--r--   0 ericmjl    (501) staff       (20)      645 2021-11-15 12:35:38.000000 pyds-cli-0.1.5/pyds/cli/templates/.devcontainer/devcontainer.json.j2
+-rw-r--r--   0 ericmjl    (501) staff       (20)      229 2023-04-03 18:58:17.000000 pyds-cli-0.1.5/pyds/cli/templates/.env.j2
+-rw-r--r--   0 ericmjl    (501) staff       (20)       29 2021-12-12 03:24:31.000000 pyds-cli-0.1.5/pyds/cli/templates/.flake8.j2
+drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-16 18:13:14.948066 pyds-cli-0.1.5/pyds/cli/templates/.github/
+drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-16 18:13:14.954081 pyds-cli-0.1.5/pyds/cli/templates/.github/workflows/
+-rw-r--r--   0 ericmjl    (501) staff       (20)      257 2021-11-15 12:34:35.000000 pyds-cli-0.1.5/pyds/cli/templates/.github/workflows/code-style.yaml.j2
+-rw-r--r--   0 ericmjl    (501) staff       (20)     1546 2023-04-03 18:58:17.000000 pyds-cli-0.1.5/pyds/cli/templates/.github/workflows/docs.yaml.j2
+-rw-r--r--   0 ericmjl    (501) staff       (20)     1113 2023-04-03 18:58:17.000000 pyds-cli-0.1.5/pyds/cli/templates/.github/workflows/pr-tests.yaml.j2
+-rw-r--r--   0 ericmjl    (501) staff       (20)     2312 2023-04-03 18:58:17.000000 pyds-cli-0.1.5/pyds/cli/templates/.gitignore.j2
+-rw-r--r--   0 ericmjl    (501) staff       (20)      923 2021-12-12 03:24:31.000000 pyds-cli-0.1.5/pyds/cli/templates/.pre-commit-config.yaml.j2
+-rw-r--r--   0 ericmjl    (501) staff       (20)      124 2021-12-12 03:24:31.000000 pyds-cli-0.1.5/pyds/cli/templates/MANIFEST.in.j2
+drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-16 18:13:14.954824 pyds-cli-0.1.5/pyds/cli/templates/docs/
+-rw-r--r--   0 ericmjl    (501) staff       (20)       63 2021-12-12 03:24:31.000000 pyds-cli-0.1.5/pyds/cli/templates/docs/api.md.j2
+-rw-r--r--   0 ericmjl    (501) staff       (20)      607 2021-12-12 03:24:31.000000 pyds-cli-0.1.5/pyds/cli/templates/docs/apidocs.css.j2
+-rw-r--r--   0 ericmjl    (501) staff       (20)       21 2021-12-12 03:24:31.000000 pyds-cli-0.1.5/pyds/cli/templates/docs/config.js.j2
+-rw-r--r--   0 ericmjl    (501) staff       (20)      488 2021-12-12 03:24:31.000000 pyds-cli-0.1.5/pyds/cli/templates/docs/index.md.j2
+-rw-r--r--   0 ericmjl    (501) staff       (20)      664 2023-04-03 18:58:17.000000 pyds-cli-0.1.5/pyds/cli/templates/environment.yml.j2
+-rw-r--r--   0 ericmjl    (501) staff       (20)     1833 2021-12-12 03:24:31.000000 pyds-cli-0.1.5/pyds/cli/templates/mkdocs.yaml.j2
+-rw-r--r--   0 ericmjl    (501) staff       (20)     1594 2023-04-05 17:48:28.000000 pyds-cli-0.1.5/pyds/cli/templates/pyproject.toml.j2
+-rw-r--r--   0 ericmjl    (501) staff       (20)      212 2023-04-03 18:58:17.000000 pyds-cli-0.1.5/pyds/cli/templates/setup.cfg.j2
+drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-16 18:13:14.955846 pyds-cli-0.1.5/pyds/cli/templates/src/
+-rw-r--r--   0 ericmjl    (501) staff       (20)      221 2023-04-03 18:58:17.000000 pyds-cli-0.1.5/pyds/cli/templates/src/__init__.py.j2
+-rw-r--r--   0 ericmjl    (501) staff       (20)      659 2021-12-12 03:24:31.000000 pyds-cli-0.1.5/pyds/cli/templates/src/cli.py.j2
+-rw-r--r--   0 ericmjl    (501) staff       (20)       48 2021-12-12 03:24:31.000000 pyds-cli-0.1.5/pyds/cli/templates/src/models.py.j2
+-rw-r--r--   0 ericmjl    (501) staff       (20)       35 2021-12-12 03:24:31.000000 pyds-cli-0.1.5/pyds/cli/templates/src/preprocessing.py.j2
+-rw-r--r--   0 ericmjl    (501) staff       (20)      192 2021-12-12 03:24:31.000000 pyds-cli-0.1.5/pyds/cli/templates/src/schemas.py.j2
+-rw-r--r--   0 ericmjl    (501) staff       (20)       40 2021-11-05 23:30:25.000000 pyds-cli-0.1.5/pyds/cli/templates/src/utils.py.j2
+drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-16 18:13:14.956576 pyds-cli-0.1.5/pyds/cli/templates/tests/
+-rw-r--r--   0 ericmjl    (501) staff       (20)       36 2021-12-12 03:24:31.000000 pyds-cli-0.1.5/pyds/cli/templates/tests/test___init__.py.j2
+-rw-r--r--   0 ericmjl    (501) staff       (20)       40 2021-12-12 03:24:31.000000 pyds-cli-0.1.5/pyds/cli/templates/tests/test_cli.py.j2
+-rw-r--r--   0 ericmjl    (501) staff       (20)       62 2021-12-12 03:24:31.000000 pyds-cli-0.1.5/pyds/cli/templates/tests/test_models.py.j2
+drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-16 18:13:14.957364 pyds-cli-0.1.5/pyds/pyds_cli.egg-info/
+-rw-r--r--   0 ericmjl    (501) staff       (20)       52 2023-04-16 18:13:14.000000 pyds-cli-0.1.5/pyds/pyds_cli.egg-info/PKG-INFO
+-rw-r--r--   0 ericmjl    (501) staff       (20)     1603 2023-04-16 18:13:14.000000 pyds-cli-0.1.5/pyds/pyds_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 ericmjl    (501) staff       (20)        1 2023-04-16 18:13:14.000000 pyds-cli-0.1.5/pyds/pyds_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 ericmjl    (501) staff       (20)       38 2023-04-16 18:13:14.000000 pyds-cli-0.1.5/pyds/pyds_cli.egg-info/entry_points.txt
+-rw-r--r--   0 ericmjl    (501) staff       (20)      172 2023-04-16 18:13:14.000000 pyds-cli-0.1.5/pyds/pyds_cli.egg-info/requires.txt
+-rw-r--r--   0 ericmjl    (501) staff       (20)       10 2023-04-16 18:13:14.000000 pyds-cli-0.1.5/pyds/pyds_cli.egg-info/top_level.txt
+drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-16 18:13:14.957765 pyds-cli-0.1.5/pyds/utils/
+-rw-r--r--   0 ericmjl    (501) staff       (20)     6846 2023-04-03 18:58:17.000000 pyds-cli-0.1.5/pyds/utils/__init__.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)      123 2023-04-03 18:58:17.000000 pyds-cli-0.1.5/pyds/utils/paths.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)     8512 2023-04-05 17:42:03.000000 pyds-cli-0.1.5/pyds/utils/project.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)     1605 2023-04-16 18:13:10.000000 pyds-cli-0.1.5/pyproject.toml
+-rw-r--r--   0 ericmjl    (501) staff       (20)       38 2023-04-16 18:13:14.958116 pyds-cli-0.1.5/setup.cfg
```

### Comparing `pyds-cli-0.1.4/README.md` & `pyds-cli-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.1.4/pyds/cli/templates/.devcontainer/Dockerfile.j2` & `pyds-cli-0.1.5/pyds/cli/templates/.devcontainer/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.1.4/pyds/cli/templates/.devcontainer/devcontainer.json.j2` & `pyds-cli-0.1.5/pyds/cli/templates/.devcontainer/devcontainer.json.j2`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.1.4/pyds/cli/templates/.github/workflows/docs.yaml.j2` & `pyds-cli-0.1.5/pyds/cli/templates/.github/workflows/docs.yaml.j2`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.1.4/pyds/cli/templates/.github/workflows/pr-tests.yaml.j2` & `pyds-cli-0.1.5/pyds/cli/templates/.github/workflows/pr-tests.yaml.j2`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.1.4/pyds/cli/templates/.gitignore.j2` & `pyds-cli-0.1.5/pyds/cli/templates/.gitignore.j2`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.1.4/pyds/cli/templates/.pre-commit-config.yaml.j2` & `pyds-cli-0.1.5/pyds/cli/templates/.pre-commit-config.yaml.j2`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.1.4/pyds/cli/templates/docs/apidocs.css.j2` & `pyds-cli-0.1.5/pyds/cli/templates/docs/apidocs.css.j2`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.1.4/pyds/cli/templates/environment.yml.j2` & `pyds-cli-0.1.5/pyds/cli/templates/environment.yml.j2`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.1.4/pyds/cli/templates/mkdocs.yaml.j2` & `pyds-cli-0.1.5/pyds/cli/templates/mkdocs.yaml.j2`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.1.4/pyds/cli/templates/pyproject.toml.j2` & `pyds-cli-0.1.5/pyds/cli/templates/pyproject.toml.j2`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.1.4/pyds/cli/templates/src/cli.py.j2` & `pyds-cli-0.1.5/pyds/cli/templates/src/cli.py.j2`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.1.4/pyds/pyds_cli.egg-info/SOURCES.txt` & `pyds-cli-0.1.5/pyds/pyds_cli.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 MANIFEST.in
 README.md
 pyproject.toml
+pyds/cli/__init__.py
+pyds/cli/conda.py
+pyds/cli/docs.py
+pyds/cli/environment.py
+pyds/cli/package.py
+pyds/cli/project.py
+pyds/cli/system.py
 pyds/cli/templates/.bumpversion.cfg.j2
 pyds/cli/templates/.darglint.j2
 pyds/cli/templates/.env.j2
 pyds/cli/templates/.flake8.j2
 pyds/cli/templates/.gitignore.j2
 pyds/cli/templates/.pre-commit-config.yaml.j2
 pyds/cli/templates/MANIFEST.in.j2
@@ -31,8 +38,11 @@
 pyds/cli/templates/tests/test_cli.py.j2
 pyds/cli/templates/tests/test_models.py.j2
 pyds/pyds_cli.egg-info/PKG-INFO
 pyds/pyds_cli.egg-info/SOURCES.txt
 pyds/pyds_cli.egg-info/dependency_links.txt
 pyds/pyds_cli.egg-info/entry_points.txt
 pyds/pyds_cli.egg-info/requires.txt
-pyds/pyds_cli.egg-info/top_level.txt
+pyds/pyds_cli.egg-info/top_level.txt
+pyds/utils/__init__.py
+pyds/utils/paths.py
+pyds/utils/project.py
```

### Comparing `pyds-cli-0.1.4/pyproject.toml` & `pyds-cli-0.1.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -54,20 +54,20 @@
 profile = "black"
 
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.packages.find]
 where = ["pyds"]
-include = ["pkg*"]  # alternatively: `exclude = ["additional*"]`
+include = ["*"]
 namespaces = false
 
 [project]
 name = "pyds-cli"
-version = "0.1.4"
+version = "0.1.5"
 dependencies = [
     "typer >=0.3.2",
     "pyyaml >=6.0",
     "jinja2 >=3.0.2",
     "loguru >=0.5.3",
     "pyprojroot >=0.2.0",
     "python-dotenv >=0.19.1",
```

