# Comparing `tmp/jinja2_inflection-0.1.0.tar.gz` & `tmp/jinja2_inflection-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jinja2_inflection-0.1.0.tar", last modified: Sun Apr 16 08:38:34 2023, max compression
+gzip compressed data, was "jinja2_inflection-0.1.1.tar", last modified: Sun Apr 16 08:54:32 2023, max compression
```

## Comparing `jinja2_inflection-0.1.0.tar` & `jinja2_inflection-0.1.1.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-r--r--   0        0        0       56 2023-04-16 08:32:09.839714 jinja2_inflection-0.1.0/README.md
--rw-r--r--   0        0        0      349 2023-04-16 08:38:34.237207 jinja2_inflection-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      255 1970-01-01 00:00:00.000000 jinja2_inflection-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       56 2023-04-16 08:32:09.839714 jinja2_inflection-0.1.1/README.md
+-rw-r--r--   0        0        0      349 2023-04-16 08:54:32.950410 jinja2_inflection-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      255 1970-01-01 00:00:00.000000 jinja2_inflection-0.1.1/PKG-INFO
```

