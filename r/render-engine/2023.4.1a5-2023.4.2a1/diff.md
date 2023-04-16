# Comparing `tmp/render_engine-2023.4.1a5.tar.gz` & `tmp/render_engine-2023.4.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "render_engine-2023.4.1a5.tar", last modified: Sat Apr  8 02:16:16 2023, max compression
+gzip compressed data, was "render_engine-2023.4.2a1.tar", last modified: Sun Apr 16 16:25:51 2023, max compression
```

## Comparing `render_engine-2023.4.1a5.tar` & `render_engine-2023.4.2a1.tar`

### file list

```diff
@@ -1,113 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:16:16.242204 render_engine-2023.4.1a5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:16:16.230204 render_engine-2023.4.1a5/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/.devcontainer/setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:16:16.234204 render_engine-2023.4.1a5/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/.github/CONTRIBUTION.md
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/.github/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:16:16.234204 render_engine-2023.4.1a5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:16:16.234204 render_engine-2023.4.1a5/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/Contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-04-08 02:16:16.242204 render_engine-2023.4.1a5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:16:16.234204 render_engine-2023.4.1a5/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:16:16.234204 render_engine-2023.4.1a5/docs/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/docs/docs/archive.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:16:16.234204 render_engine-2023.4.1a5/docs/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   273561 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/docs/docs/assets/create-app-help.png
--rw-r--r--   0 runner    (1001) docker     (123)    90538 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/docs/docs/assets/render-engine-init.png
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/docs/docs/collection.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:16:16.234204 render_engine-2023.4.1a5/docs/docs/contributing/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/docs/docs/contributing/pages.md
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/docs/docs/custom_collections.md
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/docs/docs/feeds.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:16:16.234204 render_engine-2023.4.1a5/docs/docs/getting-started/
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/docs/docs/getting-started/create-app.md
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/docs/docs/getting-started/creating-a-collection.md
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/docs/docs/getting-started/creating-a-page.md
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/docs/docs/getting-started/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/docs/docs/getting-started/layout.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/docs/docs/hookspecs.md
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/docs/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/docs/docs/page.md
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/docs/docs/plugins.md
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/docs/docs/site.md
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/docs/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 02:16:16.242204 render_engine-2023.4.1a5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:16:16.234204 render_engine-2023.4.1a5/src/
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/src/.DS_Store
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:16:16.238204 render_engine-2023.4.1a5/src/render_engine/
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/src/render_engine/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/src/render_engine/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/src/render_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/src/render_engine/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/src/render_engine/_base_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/src/render_engine/archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/src/render_engine/blog.py
--rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/src/render_engine/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/src/render_engine/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/src/render_engine/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/src/render_engine/feeds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/src/render_engine/hookspecs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/src/render_engine/links.py
--rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/src/render_engine/page.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:16:16.238204 render_engine-2023.4.1a5/src/render_engine/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/src/render_engine/parsers/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/src/render_engine/parsers/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/src/render_engine/parsers/README_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/src/render_engine/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/src/render_engine/parsers/base_parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:16:16.238204 render_engine-2023.4.1a5/src/render_engine/parsers/markdown/
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/src/render_engine/parsers/markdown/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/src/render_engine/parsers/markdown/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/src/render_engine/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:16:16.238204 render_engine-2023.4.1a5/src/render_engine/render_engine_templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/src/render_engine/render_engine_templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/src/render_engine/render_engine_templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/src/render_engine/render_engine_templates/base_collection_path.md
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/src/render_engine/render_engine_templates/content.html
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/src/render_engine/render_engine_templates/create_app_py.txt
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/src/render_engine/render_engine_templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/src/render_engine/render_engine_templates/rss2.0.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/src/render_engine/render_engine_templates/rss2.0_items.xml
--rwxr-xr-x   0 runner    (1001) docker     (123)      180 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/src/render_engine/render_engine_templates/sitemap.xml
--rwxr-xr-x   0 runner    (1001) docker     (123)      283 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/src/render_engine/render_engine_templates/sitemap_item.xml
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/src/render_engine/site.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:16:16.238204 render_engine-2023.4.1a5/src/render_engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-04-08 02:16:16.000000 render_engine-2023.4.1a5/src/render_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-04-08 02:16:16.000000 render_engine-2023.4.1a5/src/render_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 02:16:16.000000 render_engine-2023.4.1a5/src/render_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-08 02:16:16.000000 render_engine-2023.4.1a5/src/render_engine.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-08 02:16:16.000000 render_engine-2023.4.1a5/src/render_engine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-08 02:16:16.000000 render_engine-2023.4.1a5/src/render_engine.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:16:16.242204 render_engine-2023.4.1a5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/tests/create_app_check_file.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:16:16.242204 render_engine-2023.4.1a5/tests/site_test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:16:16.242204 render_engine-2023.4.1a5/tests/site_test/blog/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/tests/site_test/blog/test_blog_content.md
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/tests/site_test/build.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:16:16.242204 render_engine-2023.4.1a5/tests/site_test/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/tests/site_test/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/tests/test_archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/tests/test_base_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/tests/test_base_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/tests/test_blog.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/tests/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/tests/test_create_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/tests/test_feeds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/tests/test_page.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/tests/test_parser_markdown_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-04-08 02:16:00.000000 render_engine-2023.4.1a5/tests/test_site.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:51.338037 render_engine-2023.4.2a1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:51.330037 render_engine-2023.4.2a1/.chglog/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1142 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/.chglog/CHANGELOG.tpl.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      330 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/.chglog/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:51.330037 render_engine-2023.4.2a1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/.devcontainer/setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:51.330037 render_engine-2023.4.2a1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/.github/CONTRIBUTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/.github/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:51.330037 render_engine-2023.4.2a1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:51.330037 render_engine-2023.4.2a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:51.330037 render_engine-2023.4.2a1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/Contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-04-16 16:25:51.338037 render_engine-2023.4.2a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:51.330037 render_engine-2023.4.2a1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:51.330037 render_engine-2023.4.2a1/docs/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/docs/docs/archive.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:51.334037 render_engine-2023.4.2a1/docs/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   273561 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/docs/docs/assets/create-app-help.png
+-rw-r--r--   0 runner    (1001) docker     (123)    90538 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/docs/docs/assets/render-engine-init.png
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/docs/docs/collection.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:51.334037 render_engine-2023.4.2a1/docs/docs/contributing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/docs/docs/contributing/pages.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/docs/docs/custom_collections.md
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/docs/docs/feeds.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:51.334037 render_engine-2023.4.2a1/docs/docs/getting-started/
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/docs/docs/getting-started/create-app.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/docs/docs/getting-started/creating-a-collection.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/docs/docs/getting-started/creating-a-page.md
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/docs/docs/getting-started/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/docs/docs/getting-started/layout.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/docs/docs/hookspecs.md
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/docs/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/docs/docs/page.md
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/docs/docs/plugins.md
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/docs/docs/site.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/docs/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 16:25:51.338037 render_engine-2023.4.2a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:51.334037 render_engine-2023.4.2a1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/.DS_Store
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:51.334037 render_engine-2023.4.2a1/src/render_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/_base_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/blog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9558 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/feeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/hookspecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/page.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:51.338037 render_engine-2023.4.2a1/src/render_engine/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/parsers/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/parsers/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/parsers/README_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/parsers/base_parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:51.338037 render_engine-2023.4.2a1/src/render_engine/parsers/markdown/
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/parsers/markdown/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/parsers/markdown/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:51.338037 render_engine-2023.4.2a1/src/render_engine/render_engine_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/render_engine_templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/render_engine_templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/render_engine_templates/base_collection_path.md
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/render_engine_templates/content.html
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/render_engine_templates/create_app_py.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/render_engine_templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/render_engine_templates/rss2.0.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/render_engine_templates/rss2.0_items.xml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      180 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/render_engine_templates/sitemap.xml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      283 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/render_engine_templates/sitemap_item.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/src/render_engine/site.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:51.334037 render_engine-2023.4.2a1/src/render_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-04-16 16:25:51.000000 render_engine-2023.4.2a1/src/render_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-04-16 16:25:51.000000 render_engine-2023.4.2a1/src/render_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 16:25:51.000000 render_engine-2023.4.2a1/src/render_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-16 16:25:51.000000 render_engine-2023.4.2a1/src/render_engine.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-16 16:25:51.000000 render_engine-2023.4.2a1/src/render_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-16 16:25:51.000000 render_engine-2023.4.2a1/src/render_engine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:51.338037 render_engine-2023.4.2a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/tests/create_app_check_file.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:51.338037 render_engine-2023.4.2a1/tests/site_test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:51.338037 render_engine-2023.4.2a1/tests/site_test/blog/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/tests/site_test/blog/test_blog_content.md
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/tests/site_test/build.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:51.338037 render_engine-2023.4.2a1/tests/site_test/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/tests/site_test/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/tests/test_archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/tests/test_base_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/tests/test_base_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/tests/test_blog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/tests/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/tests/test_create_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/tests/test_feeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/tests/test_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/tests/test_parser_markdown_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-04-16 16:25:37.000000 render_engine-2023.4.2a1/tests/test_site.py
```

### Comparing `render_engine-2023.4.1a5/.devcontainer/devcontainer.json` & `render_engine-2023.4.2a1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.1a5/.github/CODE_OF_CONDUCT.md` & `render_engine-2023.4.2a1/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.1a5/.github/CONTRIBUTION.md` & `render_engine-2023.4.2a1/.github/CONTRIBUTION.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.1a5/.github/FUNDING.yml` & `render_engine-2023.4.2a1/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.1a5/.github/LICENSE` & `render_engine-2023.4.2a1/.github/LICENSE`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.1a5/.github/workflows/publish.yml` & `render_engine-2023.4.2a1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.1a5/.gitignore` & `render_engine-2023.4.2a1/.gitignore`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.1a5/PKG-INFO` & `render_engine-2023.4.2a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: render_engine
-Version: 2023.4.1a5
+Version: 2023.4.2a1
 Summary: A Flexible Static Site Generator for Python
 Project-URL: homepage, https://github.com/kjaymiller/render_engine/
 Project-URL: repository, https://github.com/kjaymiller/render_engine/
 Project-URL: documentation, https://render-engine.readthedocs.io/en/latest/
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `render_engine-2023.4.1a5/README.md` & `render_engine-2023.4.2a1/README.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.1a5/docs/docs/archive.md` & `render_engine-2023.4.2a1/docs/docs/archive.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.1a5/docs/docs/assets/create-app-help.png` & `render_engine-2023.4.2a1/docs/docs/assets/create-app-help.png`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.1a5/docs/docs/assets/render-engine-init.png` & `render_engine-2023.4.2a1/docs/docs/assets/render-engine-init.png`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.1a5/docs/docs/contributing/pages.md` & `render_engine-2023.4.2a1/docs/docs/contributing/pages.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.1a5/docs/docs/custom_collections.md` & `render_engine-2023.4.2a1/docs/docs/custom_collections.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.1a5/docs/docs/getting-started/create-app.md` & `render_engine-2023.4.2a1/docs/docs/getting-started/create-app.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.1a5/docs/docs/getting-started/creating-a-collection.md` & `render_engine-2023.4.2a1/docs/docs/getting-started/creating-a-collection.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.1a5/docs/docs/getting-started/creating-a-page.md` & `render_engine-2023.4.2a1/docs/docs/getting-started/creating-a-page.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.1a5/docs/docs/getting-started/installation.md` & `render_engine-2023.4.2a1/docs/docs/getting-started/installation.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.1a5/docs/docs/getting-started/layout.md` & `render_engine-2023.4.2a1/docs/docs/getting-started/layout.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.1a5/docs/docs/index.md` & `render_engine-2023.4.2a1/docs/docs/index.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.1a5/docs/docs/page.md` & `render_engine-2023.4.2a1/docs/docs/page.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.1a5/docs/mkdocs.yml` & `render_engine-2023.4.2a1/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.1a5/pyproject.toml` & `render_engine-2023.4.2a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.1a5/requirements.txt` & `render_engine-2023.4.2a1/requirements.txt`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     # via render-engine (pyproject.toml)
 ghp-import==2.1.0
     # via mkdocs
 gitdb==4.0.10
     # via gitpython
 gitpython==3.1.31
     # via render-engine (pyproject.toml)
-griffe==0.25.5
+griffe==0.27.0
     # via mkdocstrings-python
 idna==3.4
     # via requests
 iniconfig==2.0.0
     # via pytest
 jinja2==3.1.2
     # via
@@ -62,29 +62,29 @@
     # via
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
     #   render-engine (pyproject.toml)
 mkdocs-autorefs==0.4.1
     # via mkdocstrings
-mkdocs-material==9.1.4
+mkdocs-material==9.1.6
     # via render-engine (pyproject.toml)
 mkdocs-material-extensions==1.1.1
     # via mkdocs-material
-mkdocstrings[python]==0.20.0
+mkdocstrings[python]==0.21.2
     # via
     #   mkdocstrings-python
     #   render-engine (pyproject.toml)
-mkdocstrings-python==0.8.3
+mkdocstrings-python==0.9.0
     # via mkdocstrings
 more-itertools==9.1.0
     # via render-engine (pyproject.toml)
 mypy-extensions==1.0.0
     # via black
-packaging==23.0
+packaging==23.1
     # via
     #   black
     #   mkdocs
     #   pytest
 pathspec==0.11.1
     # via black
 platformdirs==3.2.0
@@ -98,15 +98,15 @@
     #   mkdocs-material
     #   rich
 pymdown-extensions==9.10
     # via
     #   mkdocs-material
     #   mkdocstrings
     #   render-engine (pyproject.toml)
-pytest==7.2.2
+pytest==7.3.1
     # via
     #   pytest-mock
     #   render-engine (pyproject.toml)
 pytest-mock==3.10.0
     # via render-engine (pyproject.toml)
 python-dateutil==2.8.2
     # via
@@ -124,17 +124,17 @@
     #   pyyaml-env-tag
 pyyaml-env-tag==0.1
     # via mkdocs
 regex==2023.3.23
     # via mkdocs-material
 requests==2.28.2
     # via mkdocs-material
-rich==13.3.3
+rich==13.3.4
     # via render-engine (pyproject.toml)
-ruff==0.0.260
+ruff==0.0.261
     # via render-engine (pyproject.toml)
 six==1.16.0
     # via python-dateutil
 smmap==5.0.0
     # via gitdb
 text-unidecode==1.3
     # via python-slugify
```

### Comparing `render_engine-2023.4.1a5/src/.DS_Store` & `render_engine-2023.4.2a1/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.1a5/src/render_engine/.DS_Store` & `render_engine-2023.4.2a1/src/render_engine/.DS_Store`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.1a5/src/render_engine/_base_object.py` & `render_engine-2023.4.2a1/src/render_engine/_base_object.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.1a5/src/render_engine/archive.py` & `render_engine-2023.4.2a1/src/render_engine/archive.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """
 The Archive is the Page object used by the collection that focuses on presenting Page objects.
 """
 import pathlib
+
 import jinja2
 
-from .page import BasePage 
+from .page import BasePage
 
 
 class Archive(BasePage):
     """
     ???+ Warning "Not Directly Used"
         The Archive object is not meant to be used directly. 
         It is used by the [Collection][src.render_engine.Collection] object. 
         Attributes can be used to customize the 
         [archive_template][src.render_engine.collection.Collection].
 
-    Custom [`Page`][src.render_engine.page.Page] object used to show all the pages in a [Collection][src.render_engine.Collection].
+    Custom [`Page`][src.render_engine.page.Page] used to show the pages in a [Collection][src.render_engine.Collection].
 
     Parameters:
         pages: The list of pages to include in the archive
         title: The title of the archive
         template: The template to use for the archive
         routes: The routes for where the archive page should be generated
         archive_index: The index of the page in the series of archive pages
```

### Comparing `render_engine-2023.4.1a5/src/render_engine/cli.py` & `render_engine-2023.4.2a1/src/render_engine/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# noqa: UP007
+
 import importlib
 import pathlib
 import sys
 import typing
 from http.server import HTTPServer, SimpleHTTPRequestHandler
 
 import dtyper
@@ -258,14 +260,26 @@
     port: int = typer.Option(
         8000,
         "--port",
         "-p",
         help="Port to serve on",
         show_default=False,
     ),
+    attempts: int = typer.Option(
+        10,
+        "--attempts",
+        help="Attempt to bind to port.",
+        show_default=True,
+    ),
+    attempts_wait_time: int = typer.Option(
+        60,
+        "--attempts-timeout",
+        help="Time to wait between attempts to bind to port.",
+        show_default=True,
+    ),
 ):
     """CLI for creating a new site"""
     app = get_app(module_site)
 
     if build:
         app.render()
 
@@ -273,16 +287,27 @@
         directory = app.output_path
 
     class server(SimpleHTTPRequestHandler):
         def __init__(self, *args, **kwargs):
             super().__init__(*args, directory=directory, **kwargs)
 
     server_address = ("localhost", port)
-    httpd = HTTPServer(server_address, server)
     console = Console()
-    console.print(f"Serving [blue]{directory} on http://localhost:{port}")
-    console.print(f"Press [bold red]CTRL+C[/bold red] to stop serving")
-    return httpd.serve_forever()
+    while attempts:
+        try:
+            httpd = HTTPServer(server_address, server)
+        except OSError as e:
+            if 'Address already in use' in str(e):
+                import time
+                attempts -= 1
+                if attempts:
+                    console.print(f"Unable to list to http://{server_address[0]}:{server_address[1]}.")
+                    console.print(f"Address is already in use, sleeping 60 sec. Attempts left {attempts}")
+                    time.sleep(attempts_wait_time)
+        else:
+           console.print(f"Serving [blue]{directory} on http://{server_address[0]}:{server_address[1]}")
+           console.print(f"Press [bold red]CTRL+C[/bold red] to stop serving")
+           return httpd.serve_forever()
 
 
 def cli():
     app()
```

### Comparing `render_engine-2023.4.1a5/src/render_engine/collection.py` & `render_engine-2023.4.2a1/src/render_engine/collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-from enum import Enum
 import pathlib
-from typing import Any, Callable, Generator, Type
+import typing
 
 import git
 from more_itertools import batched, flatten
 from slugify import slugify
 
 from ._base_object import BaseObject
 from .archive import Archive
 from .feeds import RSSFeed
+from .hookspecs import register_plugins
 from .page import Page
 from .parsers import BasePageParser
 from .parsers.markdown import MarkdownPageParser
-from .hookspecs import register_plugins
 
 
 class Collection(BaseObject):
     """
     Collection objects serve as a way to quickly process pages that have a
     portion of content that is similar or file driven.
 
@@ -53,30 +52,30 @@
 
         archive_template str | None: The template to use for the archive pages.
 
     """
 
     archive_template: str | None
     content_path: pathlib.Path | str
-    content_type: Type[Page] = Page
-    Feed: Type[RSSFeed]
+    content_type: Page = Page
+    Feed: RSSFeed
     feed_title: str
     include_suffixes: list[str] = ["*.md", "*.html"]
     items_per_page: int | None
-    PageParser: Type[BasePageParser] = MarkdownPageParser
-    parser_extras: dict[str, Any]
+    PageParser: BasePageParser = MarkdownPageParser
+    parser_extras: dict[str, any]
     routes: list[str] = ["./"]
     sort_by: str = "title"
     sort_reverse: bool = False
     template: str | None
-    plugins: list[Callable] | None
+    plugins: list[typing.Callable] | None
 
     def __init__(
         self,
-        plugins: list[Callable] = [],
+        plugins: list[typing.Callable] = [],
     ) -> None:
 
         self.has_archive = any(
             [
                 hasattr(self, "archive_template"),
                 getattr(self, "items_per_page", None),
             ]
@@ -91,15 +90,15 @@
         return flatten(
             [
                 pathlib.Path(self.content_path).glob(suffix)
                 for suffix in self.include_suffixes
             ]
         )
     
-    def _generate_content_from_modified_pages(self) -> Generator[Page, None, None]:
+    def _generate_content_from_modified_pages(self) -> typing.Generator[Page, None, None]:
         """
         Check git status for newly created and modified files.
         Returns the Page objects for the files in the content path
         """
         
         repo = git.Repo()
         
@@ -135,15 +134,15 @@
         return sorted(
             (page for page in self.__iter__()),
             key=lambda page: getattr(page, self.sort_by, self._title),
             reverse=self.sort_reverse,
         )
 
     @property
-    def archives(self) -> Generator[Archive, None, None]:
+    def archives(self) -> typing.Generator[Archive, None, None]:
         """
         Returns a [Archive][src.render_engine.archive] objects containing the pages from the `content_path` .
 
         Archives are an iterable and the individual pages are built shortly after the collection pages are built. This happens when [Site.render][render_engine.Site.render] is called.
         """
 
         if not self.has_archive:
```

### Comparing `render_engine-2023.4.1a5/src/render_engine/engine.py` & `render_engine-2023.4.2a1/src/render_engine/engine.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from datetime import datetime
 from email import utils
-from typing import Type
+import typing
 
 from jinja2 import (
     ChoiceLoader,
     Environment,
     FileSystemLoader,
     PackageLoader,
+    pass_environment,
     select_autoescape,
 )
 
 render_engine_templates_loader = ChoiceLoader(
     [
         FileSystemLoader("templates"),
         PackageLoader("render_engine", "render_engine_templates"),
@@ -20,14 +21,21 @@
 
 def to_pub_date(value: datetime):
     """
     Parse information from the given class object.
     """
     return utils.format_datetime(value)
 
+@pass_environment
+def format_datetime(env: Environment, value: str) -> datetime:
+    """
+    Parse information from the given class object.
+    """
+    return datetime.strftime(value, env.globals.get("DATETIME_FORMAT", "%d %b %Y %H:%M %Z"))
+
 
 def url_for(value: str, site):
     if value in site.route_list:
         return site.route_list[value].url_for
     else:
         raise ValueError(f"{value} is not a valid route.")
 
@@ -36,7 +44,8 @@
     loader=render_engine_templates_loader,
     autoescape=select_autoescape(["xml"]),
     lstrip_blocks=True,
     trim_blocks=True,
 )
 
 engine.filters["to_pub_date"] = to_pub_date
+engine.filters["format_datetime"] = format_datetime
```

### Comparing `render_engine-2023.4.1a5/src/render_engine/feeds.py` & `render_engine-2023.4.2a1/src/render_engine/feeds.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.1a5/src/render_engine/hookspecs.py` & `render_engine-2023.4.2a1/src/render_engine/hookspecs.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.1a5/src/render_engine/links.py` & `render_engine-2023.4.2a1/src/render_engine/links.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.1a5/src/render_engine/page.py` & `render_engine-2023.4.2a1/src/render_engine/page.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.1a5/src/render_engine/parsers/.DS_Store` & `render_engine-2023.4.2a1/src/render_engine/parsers/.DS_Store`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.1a5/src/render_engine/parsers/README_TEMPLATE.md` & `render_engine-2023.4.2a1/src/render_engine/parsers/README_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.1a5/src/render_engine/parsers/base_parsers.py` & `render_engine-2023.4.2a1/src/render_engine/parsers/base_parsers.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.1a5/src/render_engine/parsers/markdown/README.md` & `render_engine-2023.4.2a1/src/render_engine/parsers/markdown/README.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.1a5/src/render_engine/plugins.py` & `render_engine-2023.4.2a1/src/render_engine/plugins.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.1a5/src/render_engine/render_engine_templates/create_app_py.txt` & `render_engine-2023.4.2a1/src/render_engine/render_engine_templates/create_app_py.txt`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.1a5/src/render_engine/render_engine_templates/index.html` & `render_engine-2023.4.2a1/src/render_engine/render_engine_templates/index.html`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.1a5/src/render_engine/render_engine_templates/rss2.0.xml` & `render_engine-2023.4.2a1/src/render_engine/render_engine_templates/rss2.0.xml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.1a5/src/render_engine/render_engine_templates/rss2.0_items.xml` & `render_engine-2023.4.2a1/src/render_engine/render_engine_templates/rss2.0_items.xml`

 * *Files 10% similar despite different names*

#### Comparing `render_engine-2023.4.1a5/src/render_engine/render_engine_templates/rss2.0_items.xml` & `render_engine-2023.4.2a1/src/render_engine/render_engine_templates/rss2.0_items.xml`

```diff
@@ -16,16 +16,16 @@
   {% if item.category is defined and category['domain'] %}
   <category domain="{{item.category['domain']}}">{{item.category}}</category>
   {% else %}
   <category>{{item.category}}</category>
   {% endif %}
 {% endif %}
   <link>{{SITE_URL}}{{item.url_for()}}</link>
-  {% if item.date_published is defined and date_published %}
-  <pubDate>{{item.date_published | to_pub_date }}</pubDate>
+  {% if item.date is defined %}
+  <pubDate>{{item.date | to_pub_date }}</pubDate>
   {% endif %}
 {% if item.guid is defined and guid %}
   <guid isPermaLink="false">{{item.guid}}</guid>
   {% endif %}
 {% if item.author is defined and author %}{{item.author}}{% endif %}
 {% if item.comments is defined and comments %}{{item.comments}}{% endif %}
 {% if item.source is defined and source %}
```

### Comparing `render_engine-2023.4.1a5/src/render_engine/site.py` & `render_engine-2023.4.2a1/src/render_engine/site.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from jinja2 import Environment
 from rich.progress import Progress
 
 from .collection import Collection
 from .engine import engine, url_for
 from .hookspecs import register_plugins
 from .page import Page
+from datetime import datetime
 
 
 class Site:
     """
     The site stores your pages and collections to be rendered.
 
     Attributes:
@@ -31,17 +32,20 @@
     output_path: str = "output"
     static_path: str = "static"
     partial: bool = False
 
     site_vars: dict = {
         "SITE_TITLE": "Untitled Site",
         "SITE_URL": "http://localhost:8000/",
+        "DATETIME_FORMAT": "%d %b %Y %H:%M %Z"
     }
     plugins: list
 
+
+
     def __init__(
         self,
         plugins: list[str] = [],
     ) -> None:
         self.route_list = dict()
         self.subcollections = defaultdict(lambda: {"pages": []})
         self.engine.filters["url_for"] = partial(url_for, site=self)
```

### Comparing `render_engine-2023.4.1a5/src/render_engine.egg-info/PKG-INFO` & `render_engine-2023.4.2a1/src/render_engine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: render-engine
-Version: 2023.4.1a5
+Version: 2023.4.2a1
 Summary: A Flexible Static Site Generator for Python
 Project-URL: homepage, https://github.com/kjaymiller/render_engine/
 Project-URL: repository, https://github.com/kjaymiller/render_engine/
 Project-URL: documentation, https://render-engine.readthedocs.io/en/latest/
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `render_engine-2023.4.1a5/src/render_engine.egg-info/SOURCES.txt` & `render_engine-2023.4.2a1/src/render_engine.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 .gitignore
 .readthedocs.yml
 Contributing.md
 README.md
+changelog.md
 pyproject.toml
 requirements.txt
+.chglog/CHANGELOG.tpl.md
+.chglog/config.yml
 .devcontainer/Dockerfile
 .devcontainer/devcontainer.json
 .devcontainer/setup.sh
 .github/CODE_OF_CONDUCT.md
 .github/CONTRIBUTION.md
 .github/FUNDING.yml
 .github/LICENSE
 .github/dependabot.yml
+.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
 .github/workflows/publish.yml
 .github/workflows/test.yml
 .vscode/tasks.json
 docs/mkdocs.yml
 docs/requirements.txt
 docs/docs/archive.md
 docs/docs/collection.md
```

### Comparing `render_engine-2023.4.1a5/tests/create_app_check_file.txt` & `render_engine-2023.4.2a1/tests/create_app_check_file.txt`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.1a5/tests/test_base_object.py` & `render_engine-2023.4.2a1/tests/test_base_object.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.1a5/tests/test_base_parser.py` & `render_engine-2023.4.2a1/tests/test_base_parser.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.1a5/tests/test_collections.py` & `render_engine-2023.4.2a1/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.1a5/tests/test_create_app.py` & `render_engine-2023.4.2a1/tests/test_create_app.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.1a5/tests/test_feeds.py` & `render_engine-2023.4.2a1/tests/test_feeds.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-import pluggy
+import datetime
 
+import pluggy
 from jinja2 import StrictUndefined
 
 from render_engine.collection import Collection
+from render_engine.engine import engine, to_pub_date
 from render_engine.feeds import RSSFeed
 from render_engine.page import Page
-from render_engine.engine import engine
 
 pm = pluggy.PluginManager("fake_test")
 
 
 def test_can_manually_set_slug():
     """Test that the feed slug can be set manually"""
 
@@ -86,7 +87,32 @@
         engine=engine,
         SITE_TITLE="Test Site Title",
         SITE_URL="http://localhost:8000",
         title="Test Feed Title",
         description="Test Feed Description",
     )
     assert "http://localhost:8000/page.html" in rendered_content
+
+
+def test_rss_feed_template_parses_date_correctly(engine):
+    """Tests that a feed parses the page date in RFC2822 Format"""
+
+
+    class TestPage(Page):
+        date = datetime.datetime(2023, 4, 15, 0, 0, 0, tzinfo=datetime.timezone.utc)   # noqa: UP017
+    class TestCollection(Collection):
+        Feed = RSSFeed
+        pages = [TestPage()]
+
+    collection = TestCollection()
+
+    engine.filters["to_pub_date"] = to_pub_date
+
+    rendered_content = collection._feed._render_content(
+        engine=engine,
+        SITE_TITLE="Test Site Title",
+        SITE_URL="http://localhost:8000",
+        title="Test Feed Title",
+        description="Test Feed Description",
+    )
+
+    assert "Sat, 15 Apr 2023 00:00:00 +0000" in rendered_content
```

### Comparing `render_engine-2023.4.1a5/tests/test_page.py` & `render_engine-2023.4.2a1/tests/test_page.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.4.1a5/tests/test_site.py` & `render_engine-2023.4.2a1/tests/test_site.py`

 * *Files identical despite different names*

