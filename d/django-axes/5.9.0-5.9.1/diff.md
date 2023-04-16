# Comparing `tmp/django-axes-5.9.0.tar.gz` & `tmp/django-axes-5.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-axes-5.9.0.tar", last modified: Thu Nov  5 22:52:48 2020, max compression
+gzip compressed data, was "dist/django-axes-5.9.1.tar", last modified: Wed Dec  2 16:01:47 2020, max compression
```

## Comparing `django-axes-5.9.0.tar` & `django-axes-5.9.1.tar`

### file list

```diff
@@ -1,118 +1,121 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-11-05 22:52:48.000000 django-axes-5.9.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)      136 2020-11-05 22:52:19.000000 django-axes-5.9.0/MANIFEST.in
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-11-05 22:52:48.000000 django-axes-5.9.0/docs/
--rw-rw-r--   0 travis    (2000) travis    (2000)     9545 2020-11-05 22:52:19.000000 django-axes-5.9.0/docs/6_integration.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       43 2020-11-05 22:52:19.000000 django-axes-5.9.0/docs/10_changelog.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1392 2020-11-05 22:52:19.000000 django-axes-5.9.0/docs/9_development.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     5199 2020-11-05 22:52:19.000000 django-axes-5.9.0/docs/5_customization.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     7425 2020-11-05 22:52:19.000000 django-axes-5.9.0/docs/Makefile
--rw-rw-r--   0 travis    (2000) travis    (2000)     4011 2020-11-05 22:52:19.000000 django-axes-5.9.0/docs/conf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      648 2020-11-05 22:52:19.000000 django-axes-5.9.0/docs/1_requirements.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-11-05 22:52:48.000000 django-axes-5.9.0/docs/images/
--rw-rw-r--   0 travis    (2000) travis    (2000)   133029 2020-11-05 22:52:19.000000 django-axes-5.9.0/docs/images/flow.png
--rw-rw-r--   0 travis    (2000) travis    (2000)     5518 2020-11-05 22:52:19.000000 django-axes-5.9.0/docs/2_installation.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     4307 2020-11-05 22:52:19.000000 django-axes-5.9.0/docs/3_usage.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     3596 2020-11-05 22:52:19.000000 django-axes-5.9.0/docs/7_architecture.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      355 2020-11-05 22:52:19.000000 django-axes-5.9.0/docs/index.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      406 2020-11-05 22:52:19.000000 django-axes-5.9.0/docs/8_reference.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)    12450 2020-11-05 22:52:19.000000 django-axes-5.9.0/docs/4_configuration.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       89 2020-11-05 22:52:19.000000 django-axes-5.9.0/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    24149 2020-11-05 22:52:19.000000 django-axes-5.9.0/CHANGES.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)    38779 2020-11-05 22:52:48.000000 django-axes-5.9.0/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-11-05 22:52:48.000000 django-axes-5.9.0/axes/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4551 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/checks.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1782 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/signals.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-11-05 22:52:48.000000 django-axes-5.9.0/axes/handlers/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4529 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/handlers/cache.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      677 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/handlers/dummy.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      644 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/handlers/test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4382 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/handlers/proxy.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6752 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/handlers/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/handlers/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10177 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/handlers/database.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      611 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/decorators.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4901 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/conf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2807 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/backends.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-11-05 22:52:48.000000 django-axes-5.9.0/axes/locale/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-11-05 22:52:48.000000 django-axes-5.9.0/axes/locale/tr/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-11-05 22:52:48.000000 django-axes-5.9.0/axes/locale/tr/LC_MESSAGES/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1450 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/locale/tr/LC_MESSAGES/django.mo
--rw-rw-r--   0 travis    (2000) travis    (2000)     2072 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/locale/tr/LC_MESSAGES/django.po
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-11-05 22:52:48.000000 django-axes-5.9.0/axes/locale/de/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-11-05 22:52:48.000000 django-axes-5.9.0/axes/locale/de/LC_MESSAGES/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1549 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/locale/de/LC_MESSAGES/django.mo
--rw-rw-r--   0 travis    (2000) travis    (2000)     2122 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/locale/de/LC_MESSAGES/django.po
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-11-05 22:52:48.000000 django-axes-5.9.0/axes/locale/ru/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-11-05 22:52:48.000000 django-axes-5.9.0/axes/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1950 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/locale/ru/LC_MESSAGES/django.mo
--rw-rw-r--   0 travis    (2000) travis    (2000)     2494 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/locale/ru/LC_MESSAGES/django.po
--rw-rw-r--   0 travis    (2000) travis    (2000)      380 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/exceptions.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-11-05 22:52:48.000000 django-axes-5.9.0/axes/migrations/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1723 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/migrations/0002_auto_20151217_2044.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1948 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/migrations/0003_auto_20160322_0929.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2831 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/migrations/0001_initial.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      219 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/migrations/0005_remove_accessattempt_trusted.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2197 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/migrations/0004_auto_20181024_1538.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      274 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/migrations/0006_remove_accesslog_trusted.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/migrations/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1656 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1404 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/models.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2098 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/middleware.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2008 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/admin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1531 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/apps.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      142 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3041 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/attempts.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16042 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/helpers.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-11-05 22:52:48.000000 django-axes-5.9.0/axes/management/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-11-05 22:52:48.000000 django-axes-5.9.0/axes/management/commands/
--rw-rw-r--   0 travis    (2000) travis    (2000)      579 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/management/commands/axes_reset_user.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      404 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/management/commands/axes_list_attempts.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      409 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/management/commands/axes_reset.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      552 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/management/commands/axes_reset_ip.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      643 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/management/commands/axes_reset_logs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      579 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/management/commands/axes_reset_username.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/management/commands/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/management/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-11-05 22:52:48.000000 django-axes-5.9.0/axes/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)      494 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/tests/test_signals.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3765 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/tests/test_management.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3329 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/tests/test_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1149 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/tests/test_models.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4376 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/tests/test_logging.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27443 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/tests/test_login.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4341 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/tests/test_middleware.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      112 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/tests/urls.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3600 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/tests/test_checks.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15136 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/tests/test_handlers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      752 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/tests/test_backends.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5851 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/tests/test_attempts.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5717 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/tests/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       23 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/tests/urls_empty.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      940 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/tests/test_admin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2002 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/tests/settings.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22266 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/tests/test_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1944 2020-11-05 22:52:19.000000 django-axes-5.9.0/axes/tests/test_decorators.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      212 2020-11-05 22:52:19.000000 django-axes-5.9.0/codecov.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)      702 2020-11-05 22:52:19.000000 django-axes-5.9.0/tox.ini
--rw-rw-r--   0 travis    (2000) travis    (2000)      228 2020-11-05 22:52:19.000000 django-axes-5.9.0/pytest.ini
--rw-rw-r--   0 travis    (2000) travis    (2000)      164 2020-11-05 22:52:19.000000 django-axes-5.9.0/.gitignore
--rw-rw-r--   0 travis    (2000) travis    (2000)       86 2020-11-05 22:52:19.000000 django-axes-5.9.0/.prospector.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2020-11-05 22:52:48.000000 django-axes-5.9.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      105 2020-11-05 22:52:19.000000 django-axes-5.9.0/mypy.ini
--rw-rw-r--   0 travis    (2000) travis    (2000)      254 2020-11-05 22:52:19.000000 django-axes-5.9.0/manage.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      919 2020-11-05 22:52:19.000000 django-axes-5.9.0/.travis.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)     1184 2020-11-05 22:52:19.000000 django-axes-5.9.0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)       34 2020-11-05 22:52:19.000000 django-axes-5.9.0/.coveragerc
--rw-rw-r--   0 travis    (2000) travis    (2000)     3103 2020-11-05 22:52:19.000000 django-axes-5.9.0/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       76 2020-11-05 22:52:19.000000 django-axes-5.9.0/pyproject.toml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-11-05 22:52:48.000000 django-axes-5.9.0/django_axes.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)    38779 2020-11-05 22:52:48.000000 django-axes-5.9.0/django_axes.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-11-05 22:52:48.000000 django-axes-5.9.0/django_axes.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        5 2020-11-05 22:52:48.000000 django-axes-5.9.0/django_axes.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-11-05 22:52:48.000000 django-axes-5.9.0/django_axes.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)     2448 2020-11-05 22:52:48.000000 django-axes-5.9.0/django_axes.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       32 2020-11-05 22:52:48.000000 django-axes-5.9.0/django_axes.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       44 2020-11-05 22:52:19.000000 django-axes-5.9.0/requirements-qa.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     2332 2020-11-05 22:52:19.000000 django-axes-5.9.0/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       96 2020-11-05 22:52:19.000000 django-axes-5.9.0/requirements-test.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-02 16:01:47.139804 django-axes-5.9.1/
+-rw-r--r--   0 runner    (1001) docker     (116)       34 2020-12-02 16:01:29.000000 django-axes-5.9.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-02 16:01:47.127803 django-axes-5.9.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-02 16:01:47.131804 django-axes-5.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (116)     1340 2020-12-02 16:01:29.000000 django-axes-5.9.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (116)     1128 2020-12-02 16:01:29.000000 django-axes-5.9.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      177 2020-12-02 16:01:29.000000 django-axes-5.9.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (116)       86 2020-12-02 16:01:29.000000 django-axes-5.9.1/.prospector.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)    24332 2020-12-02 16:01:29.000000 django-axes-5.9.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     1184 2020-12-02 16:01:29.000000 django-axes-5.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)      136 2020-12-02 16:01:29.000000 django-axes-5.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)    39046 2020-12-02 16:01:47.139804 django-axes-5.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     3115 2020-12-02 16:01:29.000000 django-axes-5.9.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-02 16:01:47.131804 django-axes-5.9.1/axes/
+-rw-r--r--   0 runner    (1001) docker     (116)      142 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2008 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/admin.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1531 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/apps.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3041 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/attempts.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2807 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/backends.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4551 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/checks.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4901 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/conf.py
+-rw-r--r--   0 runner    (1001) docker     (116)      611 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (116)      380 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-02 16:01:47.131804 django-axes-5.9.1/axes/handlers/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6752 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4529 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/handlers/cache.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10177 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/handlers/database.py
+-rw-r--r--   0 runner    (1001) docker     (116)      677 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/handlers/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4382 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/handlers/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (116)      644 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/handlers/test.py
+-rw-r--r--   0 runner    (1001) docker     (116)    16042 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-02 16:01:47.127803 django-axes-5.9.1/axes/locale/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-02 16:01:47.127803 django-axes-5.9.1/axes/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-02 16:01:47.131804 django-axes-5.9.1/axes/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (116)     1549 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (116)     2122 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-02 16:01:47.127803 django-axes-5.9.1/axes/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-02 16:01:47.131804 django-axes-5.9.1/axes/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (116)     1950 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (116)     2494 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-02 16:01:47.127803 django-axes-5.9.1/axes/locale/tr/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-02 16:01:47.135804 django-axes-5.9.1/axes/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (116)     1450 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (116)     2072 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-02 16:01:47.135804 django-axes-5.9.1/axes/management/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-02 16:01:47.135804 django-axes-5.9.1/axes/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      404 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/management/commands/axes_list_attempts.py
+-rw-r--r--   0 runner    (1001) docker     (116)      409 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/management/commands/axes_reset.py
+-rw-r--r--   0 runner    (1001) docker     (116)      552 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/management/commands/axes_reset_ip.py
+-rw-r--r--   0 runner    (1001) docker     (116)      643 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/management/commands/axes_reset_logs.py
+-rw-r--r--   0 runner    (1001) docker     (116)      579 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/management/commands/axes_reset_user.py
+-rw-r--r--   0 runner    (1001) docker     (116)      579 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/management/commands/axes_reset_username.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2218 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-02 16:01:47.135804 django-axes-5.9.1/axes/migrations/
+-rw-r--r--   0 runner    (1001) docker     (116)     2831 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1723 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/migrations/0002_auto_20151217_2044.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1948 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/migrations/0003_auto_20160322_0929.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2197 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/migrations/0004_auto_20181024_1538.py
+-rw-r--r--   0 runner    (1001) docker     (116)      219 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/migrations/0005_remove_accessattempt_trusted.py
+-rw-r--r--   0 runner    (1001) docker     (116)      274 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/migrations/0006_remove_accesslog_trusted.py
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1404 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/models.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1782 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-02 16:01:47.135804 django-axes-5.9.1/axes/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5717 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2002 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (116)      940 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5851 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/tests/test_attempts.py
+-rw-r--r--   0 runner    (1001) docker     (116)      752 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3600 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1944 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (116)    15136 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/tests/test_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3329 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4376 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (116)    27443 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/tests/test_login.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3765 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/tests/test_management.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4672 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/tests/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1149 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (116)      494 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/tests/test_signals.py
+-rw-r--r--   0 runner    (1001) docker     (116)    22266 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)      112 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (116)       23 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/tests/urls_empty.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1656 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)      212 2020-12-02 16:01:29.000000 django-axes-5.9.1/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-02 16:01:47.139804 django-axes-5.9.1/django_axes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)    39046 2020-12-02 16:01:46.000000 django-axes-5.9.1/django_axes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     2493 2020-12-02 16:01:47.000000 django-axes-5.9.1/django_axes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-02 16:01:46.000000 django-axes-5.9.1/django_axes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-02 16:01:46.000000 django-axes-5.9.1/django_axes.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (116)       32 2020-12-02 16:01:46.000000 django-axes-5.9.1/django_axes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        5 2020-12-02 16:01:46.000000 django-axes-5.9.1/django_axes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-02 16:01:47.139804 django-axes-5.9.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (116)       43 2020-12-02 16:01:29.000000 django-axes-5.9.1/docs/10_changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      648 2020-12-02 16:01:29.000000 django-axes-5.9.1/docs/1_requirements.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     5518 2020-12-02 16:01:29.000000 django-axes-5.9.1/docs/2_installation.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     4307 2020-12-02 16:01:29.000000 django-axes-5.9.1/docs/3_usage.rst
+-rw-r--r--   0 runner    (1001) docker     (116)    12450 2020-12-02 16:01:29.000000 django-axes-5.9.1/docs/4_configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     5199 2020-12-02 16:01:29.000000 django-axes-5.9.1/docs/5_customization.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     9545 2020-12-02 16:01:29.000000 django-axes-5.9.1/docs/6_integration.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     3596 2020-12-02 16:01:29.000000 django-axes-5.9.1/docs/7_architecture.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      406 2020-12-02 16:01:29.000000 django-axes-5.9.1/docs/8_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     1400 2020-12-02 16:01:29.000000 django-axes-5.9.1/docs/9_development.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     7425 2020-12-02 16:01:29.000000 django-axes-5.9.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (116)     4011 2020-12-02 16:01:29.000000 django-axes-5.9.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-02 16:01:47.139804 django-axes-5.9.1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (116)   133029 2020-12-02 16:01:29.000000 django-axes-5.9.1/docs/images/flow.png
+-rw-r--r--   0 runner    (1001) docker     (116)      355 2020-12-02 16:01:29.000000 django-axes-5.9.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      254 2020-12-02 16:01:29.000000 django-axes-5.9.1/manage.py
+-rw-r--r--   0 runner    (1001) docker     (116)      105 2020-12-02 16:01:29.000000 django-axes-5.9.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (116)       76 2020-12-02 16:01:29.000000 django-axes-5.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (116)      245 2020-12-02 16:01:29.000000 django-axes-5.9.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (116)       44 2020-12-02 16:01:29.000000 django-axes-5.9.1/requirements-qa.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       96 2020-12-02 16:01:29.000000 django-axes-5.9.1/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       89 2020-12-02 16:01:29.000000 django-axes-5.9.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2020-12-02 16:01:47.139804 django-axes-5.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     2332 2020-12-02 16:01:29.000000 django-axes-5.9.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (116)      655 2020-12-02 16:01:29.000000 django-axes-5.9.1/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-axes-5.9.0/docs/6_integration.rst` & `django-axes-5.9.1/docs/6_integration.rst`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.0/docs/9_development.rst` & `django-axes-5.9.1/docs/9_development.rst`

 * *Files 8% similar despite different names*

```diff
@@ -33,14 +33,14 @@
 
     $ mypy .
 
 Before committing, you can run all the above tests against all supported Python and Django versions with tox::
 
     $ tox
 
-Tox runs the same test set that is run by Travis, and your code should be good to go if it passes.
+Tox runs the same test set that is run by GitHub Actions, and your code should be good to go if it passes.
 
 If you wish to limit the testing to specific environment(s), you can parametrize the tox run::
 
     $ tox -e py37-django21
 
 After you have pushed your changes, open a pull request on GitHub for getting your code upstreamed.
```

### Comparing `django-axes-5.9.0/docs/5_customization.rst` & `django-axes-5.9.1/docs/5_customization.rst`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.0/docs/Makefile` & `django-axes-5.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.0/docs/conf.py` & `django-axes-5.9.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.0/docs/1_requirements.rst` & `django-axes-5.9.1/docs/1_requirements.rst`

 * *Files 8% similar despite different names*

```diff
@@ -3,13 +3,13 @@
 Requirements
 ============
 
 Axes requires a supported Django version and runs on Python versions 3.6 and above.
 
 Refer to the project source code repository in
 `GitHub <https://github.com/jazzband/django-axes/>`_ and see the
-`Travis CI configuration <https://github.com/jazzband/django-axes/blob/master/.travis.yml>`_ and
+`Tox configuration <https://github.com/jazzband/django-axes/blob/master/tox.ini>`_ and
 `Python package definition <https://github.com/jazzband/django-axes/blob/master/setup.py>`_
 to check if your Django and Python version are supported.
 
-The `Travis CI builds <https://travis-ci.org/jazzband/django-axes>`_
+The `GitHub Actions builds <https://github.com/jazzband/django-axes/actions>`_
 test Axes compatibility with the Django master branch for future compatibility as well.
```

### Comparing `django-axes-5.9.0/docs/images/flow.png` & `django-axes-5.9.1/docs/images/flow.png`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.0/docs/2_installation.rst` & `django-axes-5.9.1/docs/2_installation.rst`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.0/docs/3_usage.rst` & `django-axes-5.9.1/docs/3_usage.rst`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.0/docs/7_architecture.rst` & `django-axes-5.9.1/docs/7_architecture.rst`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.0/docs/4_configuration.rst` & `django-axes-5.9.1/docs/4_configuration.rst`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.0/CHANGES.rst` & `django-axes-5.9.1/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 
 Changes
 =======
 
 
+5.9.1 (2020-12-02)
+------------------
+
+- Move tests to GitHub Actions
+  [jezdez]
+- Fix running Axes code in middleware when ``AXES_ENABLED`` is ``False``.
+  [ashokdelphia]
+
+
 5.9.0 (2020-11-05)
 ------------------
 
 - Add Python 3.9 support.
   [hramezani]
 - Prevent ``AccessAttempt`` creation with database handler 
   when username is not set
   and ``AXES_ONLY_USER_FAILURES`` setting is not set.
-  
-  
+  [hramezani]
+
 
 5.8.0 (2020-10-16)
 ------------------
 
 - Improve Django REST Framework (DRF) integration.
   [Anatoly]
```

### Comparing `django-axes-5.9.0/PKG-INFO` & `django-axes-5.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: django-axes
-Version: 5.9.0
+Version: 5.9.1
 Summary: Keep track of failed login attempts in Django-powered sites.
 Home-page: https://github.com/jazzband/django-axes
 Author: Josh VanderLinden, Philip Neustrom, Michael Blume, Alex Clark, Camilo Nova, Aleksi Hakli
 Author-email: security@jazzband.co
 Maintainer: Jazzband
 Maintainer-email: security@jazzband.co
 License: MIT
@@ -27,17 +27,17 @@
            :target: https://pypi.org/project/django-axes/
            :alt: PyPI release
         
         .. image:: https://img.shields.io/readthedocs/django-axes.svg
            :target: https://django-axes.readthedocs.io/
            :alt: Documentation
         
-        .. image:: https://secure.travis-ci.org/jazzband/django-axes.svg?branch=master
-           :target: http://travis-ci.org/jazzband/django-axes
-           :alt: Build Status
+        .. image:: https://github.com/jazzband/django-axes/workflows/Test/badge.svg
+           :target: https://github.com/jazzband/django-axes/actions
+           :alt: GitHub Actions
         
         .. image:: https://codecov.io/gh/jazzband/django-axes/branch/master/graph/badge.svg
            :target: https://codecov.io/gh/jazzband/django-axes
            :alt: Coverage
         
         
         Axes is a Django plugin for keeping track of suspicious
@@ -98,37 +98,46 @@
         * documentation improvements, or
         * tooling and CI improvements.
         
         Merging contributions requires passing the checks configured
         with the CI. This includes running tests and linters successfully
         on the currently officially supported Python and Django versions.
         
-        The test automation is run automatically by Travis CI, but you can
+        The test automation is run automatically with GitHub Actions, but you can
         run it locally with the ``tox`` command before pushing commits.
         
         Please note that this is a `Jazzband <https://jazzband.co>`_ project.
         By contributing you agree to abide by the
         `Contributor Code of Conduct <https://jazzband.co/about/conduct>`_
         and follow the `guidelines <https://jazzband.co/about/guidelines>`_.
         
         
         Changes
         =======
         
         
+        5.9.1 (2020-12-02)
+        ------------------
+        
+        - Move tests to GitHub Actions
+          [jezdez]
+        - Fix running Axes code in middleware when ``AXES_ENABLED`` is ``False``.
+          [ashokdelphia]
+        
+        
         5.9.0 (2020-11-05)
         ------------------
         
         - Add Python 3.9 support.
           [hramezani]
         - Prevent ``AccessAttempt`` creation with database handler 
           when username is not set
           and ``AXES_ONLY_USER_FAILURES`` setting is not set.
-          
-          
+          [hramezani]
+        
         
         5.8.0 (2020-10-16)
         ------------------
         
         - Improve Django REST Framework (DRF) integration.
           [Anatoly]
```

### Comparing `django-axes-5.9.0/axes/checks.py` & `django-axes-5.9.1/axes/checks.py`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.0/axes/signals.py` & `django-axes-5.9.1/axes/signals.py`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.0/axes/handlers/cache.py` & `django-axes-5.9.1/axes/handlers/cache.py`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.0/axes/handlers/dummy.py` & `django-axes-5.9.1/axes/handlers/dummy.py`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.0/axes/handlers/test.py` & `django-axes-5.9.1/axes/handlers/test.py`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.0/axes/handlers/proxy.py` & `django-axes-5.9.1/axes/handlers/proxy.py`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.0/axes/handlers/base.py` & `django-axes-5.9.1/axes/handlers/base.py`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.0/axes/handlers/database.py` & `django-axes-5.9.1/axes/handlers/database.py`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.0/axes/decorators.py` & `django-axes-5.9.1/axes/decorators.py`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.0/axes/conf.py` & `django-axes-5.9.1/axes/conf.py`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.0/axes/backends.py` & `django-axes-5.9.1/axes/backends.py`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.0/axes/locale/tr/LC_MESSAGES/django.mo` & `django-axes-5.9.1/axes/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.0/axes/locale/tr/LC_MESSAGES/django.po` & `django-axes-5.9.1/axes/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.0/axes/locale/de/LC_MESSAGES/django.mo` & `django-axes-5.9.1/axes/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.0/axes/locale/de/LC_MESSAGES/django.po` & `django-axes-5.9.1/axes/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.0/axes/locale/ru/LC_MESSAGES/django.mo` & `django-axes-5.9.1/axes/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.0/axes/locale/ru/LC_MESSAGES/django.po` & `django-axes-5.9.1/axes/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.0/axes/migrations/0002_auto_20151217_2044.py` & `django-axes-5.9.1/axes/migrations/0002_auto_20151217_2044.py`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.0/axes/migrations/0003_auto_20160322_0929.py` & `django-axes-5.9.1/axes/migrations/0003_auto_20160322_0929.py`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.0/axes/migrations/0001_initial.py` & `django-axes-5.9.1/axes/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.0/axes/migrations/0004_auto_20181024_1538.py` & `django-axes-5.9.1/axes/migrations/0004_auto_20181024_1538.py`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.0/axes/utils.py` & `django-axes-5.9.1/axes/utils.py`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.0/axes/models.py` & `django-axes-5.9.1/axes/models.py`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.0/axes/middleware.py` & `django-axes-5.9.1/axes/middleware.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,23 +38,26 @@
 
     def __init__(self, get_response: Callable):
         self.get_response = get_response
 
     def __call__(self, request):
         response = self.get_response(request)
 
-        if "rest_framework" in settings.INSTALLED_APPS:
-            AxesProxyHandler.update_request(request)
-            username = get_client_username(request)
-            credentials = get_credentials(username)
-            failures_since_start = AxesProxyHandler.get_failures(request, credentials)
-            if (
-                settings.AXES_LOCK_OUT_AT_FAILURE
-                and failures_since_start >= get_failure_limit(request, credentials)
-            ):
+        if settings.AXES_ENABLED:
+            if "rest_framework" in settings.INSTALLED_APPS:
+                AxesProxyHandler.update_request(request)
+                username = get_client_username(request)
+                credentials = get_credentials(username)
+                failures_since_start = AxesProxyHandler.get_failures(
+                    request, credentials
+                )
+                if (
+                    settings.AXES_LOCK_OUT_AT_FAILURE
+                    and failures_since_start >= get_failure_limit(request, credentials)
+                ):
 
-                request.axes_locked_out = True
+                    request.axes_locked_out = True
 
-        if getattr(request, "axes_locked_out", None):
-            response = get_lockout_response(request)  # type: ignore
+            if getattr(request, "axes_locked_out", None):
+                response = get_lockout_response(request)  # type: ignore
 
         return response
```

### Comparing `django-axes-5.9.0/axes/admin.py` & `django-axes-5.9.1/axes/admin.py`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.0/axes/apps.py` & `django-axes-5.9.1/axes/apps.py`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.0/axes/attempts.py` & `django-axes-5.9.1/axes/attempts.py`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.0/axes/helpers.py` & `django-axes-5.9.1/axes/helpers.py`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.0/axes/management/commands/axes_reset_user.py` & `django-axes-5.9.1/axes/management/commands/axes_reset_user.py`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.0/axes/management/commands/axes_reset_ip.py` & `django-axes-5.9.1/axes/management/commands/axes_reset_ip.py`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.0/axes/management/commands/axes_reset_logs.py` & `django-axes-5.9.1/axes/management/commands/axes_reset_logs.py`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.0/axes/management/commands/axes_reset_username.py` & `django-axes-5.9.1/axes/management/commands/axes_reset_username.py`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.0/axes/tests/test_management.py` & `django-axes-5.9.1/axes/tests/test_management.py`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.0/axes/tests/test_helpers.py` & `django-axes-5.9.1/axes/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.0/axes/tests/test_models.py` & `django-axes-5.9.1/axes/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.0/axes/tests/test_logging.py` & `django-axes-5.9.1/axes/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.0/axes/tests/test_login.py` & `django-axes-5.9.1/axes/tests/test_login.py`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.0/axes/tests/test_middleware.py` & `django-axes-5.9.1/axes/tests/test_middleware.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,23 @@
         def get_response(request):
             request.axes_locked_out = True
             return HttpResponse()
 
         response = AxesMiddleware(get_response)(self.request)
         self.assertEqual(response.status_code, self.STATUS_LOCKOUT)
 
+    @override_settings(AXES_ENABLED=False)
+    def test_respects_enabled_switch(self):
+        def get_response(request):
+            request.axes_locked_out = True
+            return HttpResponse()
+
+        response = AxesMiddleware(get_response)(self.request)
+        self.assertEqual(response.status_code, self.STATUS_SUCCESS)
+
     @mock.patch("django.conf.settings.INSTALLED_APPS", ["rest_framework"])
     def test_response_contains_required_attrs_with_drf_integration(self):
         def get_response(request):
             return HttpResponse()
 
         self.assertFalse(hasattr(self.request, "axes_locked_out"))
         self.assertFalse(hasattr(self.request, "axes_attempt_time"))
```

### Comparing `django-axes-5.9.0/axes/tests/test_checks.py` & `django-axes-5.9.1/axes/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.0/axes/tests/test_handlers.py` & `django-axes-5.9.1/axes/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.0/axes/tests/test_backends.py` & `django-axes-5.9.1/axes/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.0/axes/tests/test_attempts.py` & `django-axes-5.9.1/axes/tests/test_attempts.py`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.0/axes/tests/base.py` & `django-axes-5.9.1/axes/tests/base.py`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.0/axes/tests/test_admin.py` & `django-axes-5.9.1/axes/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.0/axes/tests/settings.py` & `django-axes-5.9.1/axes/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.0/axes/tests/test_utils.py` & `django-axes-5.9.1/axes/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.0/axes/tests/test_decorators.py` & `django-axes-5.9.1/axes/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.0/LICENSE` & `django-axes-5.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.0/README.rst` & `django-axes-5.9.1/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -14,17 +14,17 @@
    :target: https://pypi.org/project/django-axes/
    :alt: PyPI release
 
 .. image:: https://img.shields.io/readthedocs/django-axes.svg
    :target: https://django-axes.readthedocs.io/
    :alt: Documentation
 
-.. image:: https://secure.travis-ci.org/jazzband/django-axes.svg?branch=master
-   :target: http://travis-ci.org/jazzband/django-axes
-   :alt: Build Status
+.. image:: https://github.com/jazzband/django-axes/workflows/Test/badge.svg
+   :target: https://github.com/jazzband/django-axes/actions
+   :alt: GitHub Actions
 
 .. image:: https://codecov.io/gh/jazzband/django-axes/branch/master/graph/badge.svg
    :target: https://codecov.io/gh/jazzband/django-axes
    :alt: Coverage
 
 
 Axes is a Django plugin for keeping track of suspicious
@@ -85,14 +85,14 @@
 * documentation improvements, or
 * tooling and CI improvements.
 
 Merging contributions requires passing the checks configured
 with the CI. This includes running tests and linters successfully
 on the currently officially supported Python and Django versions.
 
-The test automation is run automatically by Travis CI, but you can
+The test automation is run automatically with GitHub Actions, but you can
 run it locally with the ``tox`` command before pushing commits.
 
 Please note that this is a `Jazzband <https://jazzband.co>`_ project.
 By contributing you agree to abide by the
 `Contributor Code of Conduct <https://jazzband.co/about/conduct>`_
 and follow the `guidelines <https://jazzband.co/about/guidelines>`_.
```

### Comparing `django-axes-5.9.0/django_axes.egg-info/PKG-INFO` & `django-axes-5.9.1/django_axes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: django-axes
-Version: 5.9.0
+Version: 5.9.1
 Summary: Keep track of failed login attempts in Django-powered sites.
 Home-page: https://github.com/jazzband/django-axes
 Author: Josh VanderLinden, Philip Neustrom, Michael Blume, Alex Clark, Camilo Nova, Aleksi Hakli
 Author-email: security@jazzband.co
 Maintainer: Jazzband
 Maintainer-email: security@jazzband.co
 License: MIT
@@ -27,17 +27,17 @@
            :target: https://pypi.org/project/django-axes/
            :alt: PyPI release
         
         .. image:: https://img.shields.io/readthedocs/django-axes.svg
            :target: https://django-axes.readthedocs.io/
            :alt: Documentation
         
-        .. image:: https://secure.travis-ci.org/jazzband/django-axes.svg?branch=master
-           :target: http://travis-ci.org/jazzband/django-axes
-           :alt: Build Status
+        .. image:: https://github.com/jazzband/django-axes/workflows/Test/badge.svg
+           :target: https://github.com/jazzband/django-axes/actions
+           :alt: GitHub Actions
         
         .. image:: https://codecov.io/gh/jazzband/django-axes/branch/master/graph/badge.svg
            :target: https://codecov.io/gh/jazzband/django-axes
            :alt: Coverage
         
         
         Axes is a Django plugin for keeping track of suspicious
@@ -98,37 +98,46 @@
         * documentation improvements, or
         * tooling and CI improvements.
         
         Merging contributions requires passing the checks configured
         with the CI. This includes running tests and linters successfully
         on the currently officially supported Python and Django versions.
         
-        The test automation is run automatically by Travis CI, but you can
+        The test automation is run automatically with GitHub Actions, but you can
         run it locally with the ``tox`` command before pushing commits.
         
         Please note that this is a `Jazzband <https://jazzband.co>`_ project.
         By contributing you agree to abide by the
         `Contributor Code of Conduct <https://jazzband.co/about/conduct>`_
         and follow the `guidelines <https://jazzband.co/about/guidelines>`_.
         
         
         Changes
         =======
         
         
+        5.9.1 (2020-12-02)
+        ------------------
+        
+        - Move tests to GitHub Actions
+          [jezdez]
+        - Fix running Axes code in middleware when ``AXES_ENABLED`` is ``False``.
+          [ashokdelphia]
+        
+        
         5.9.0 (2020-11-05)
         ------------------
         
         - Add Python 3.9 support.
           [hramezani]
         - Prevent ``AccessAttempt`` creation with database handler 
           when username is not set
           and ``AXES_ONLY_USER_FAILURES`` setting is not set.
-          
-          
+          [hramezani]
+        
         
         5.8.0 (2020-10-16)
         ------------------
         
         - Improve Django REST Framework (DRF) integration.
           [Anatoly]
```

### Comparing `django-axes-5.9.0/django_axes.egg-info/SOURCES.txt` & `django-axes-5.9.1/django_axes.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 .coveragerc
 .gitignore
 .prospector.yaml
-.travis.yml
 CHANGES.rst
 LICENSE
 MANIFEST.in
 README.rst
 codecov.yml
 manage.py
 mypy.ini
 pyproject.toml
 pytest.ini
 requirements-qa.txt
 requirements-test.txt
 requirements.txt
 setup.py
 tox.ini
+.github/workflows/release.yml
+.github/workflows/test.yml
 axes/__init__.py
 axes/admin.py
 axes/apps.py
 axes/attempts.py
 axes/backends.py
 axes/checks.py
 axes/conf.py
```

### Comparing `django-axes-5.9.0/setup.py` & `django-axes-5.9.1/setup.py`

 * *Files identical despite different names*

