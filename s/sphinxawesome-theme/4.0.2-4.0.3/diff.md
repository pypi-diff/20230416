# Comparing `tmp/sphinxawesome_theme-4.0.2.tar.gz` & `tmp/sphinxawesome_theme-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxawesome_theme-4.0.2.tar", max compression
+gzip compressed data, was "sphinxawesome_theme-4.0.3.tar", max compression
```

## Comparing `sphinxawesome_theme-4.0.2.tar` & `sphinxawesome_theme-4.0.3.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0     1066 2023-03-05 14:58:35.320068 sphinxawesome_theme-4.0.2/LICENSE
--rw-r--r--   0        0        0     2857 2023-03-05 14:58:35.320068 sphinxawesome_theme-4.0.2/README.md
--rw-r--r--   0        0        0     2155 2023-03-05 14:58:35.320068 sphinxawesome_theme-4.0.2/pyproject.toml
--rw-r--r--   0        0        0      172 2023-03-05 14:58:35.320068 sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/README.rst
--rw-r--r--   0        0        0     2733 2023-03-05 14:58:35.320068 sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/__init__.py
--rw-r--r--   0        0        0      671 2023-03-05 14:58:35.324068 sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/breadcrumbs.html
--rw-r--r--   0        0        0     2255 2023-03-05 14:58:35.324068 sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/docsearch.py
--rw-r--r--   0        0        0      875 2023-03-05 14:58:35.324068 sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/footer.html
--rw-r--r--   0        0        0     2726 2023-03-05 14:58:35.324068 sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/header.html
--rw-r--r--   0        0        0    12023 2023-03-05 14:58:35.324068 sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/highlighting.py
--rw-r--r--   0        0        0    11203 2023-03-05 14:58:35.324068 sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/html_translator.py
--rw-r--r--   0        0        0     1668 2023-03-05 14:58:35.324068 sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/icons.py
--rw-r--r--   0        0        0     2744 2023-03-05 14:58:35.324068 sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/jinja_functions.py
--rw-r--r--   0        0        0     1239 2023-03-05 14:58:35.324068 sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/jsonimpl.py
--rw-r--r--   0        0        0     2892 2023-03-05 14:58:35.324068 sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/layout.html
--rw-r--r--   0        0        0     1396 2023-03-05 14:58:35.324068 sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/menu.html
--rw-r--r--   0        0        0      622 2023-03-05 14:58:35.324068 sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/modals.html
--rw-r--r--   0        0        0      311 2023-03-05 14:58:35.324068 sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/page.html
--rw-r--r--   0        0        0     5817 2023-03-05 14:58:35.324068 sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/postprocess.py
--rw-r--r--   0        0        0      836 2023-03-05 14:58:35.324068 sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/prev_next.html
--rw-r--r--   0        0        0      692 2023-03-05 14:58:35.324068 sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/scrolltop.html
--rw-r--r--   0        0        0      808 2023-03-05 14:58:35.324068 sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/search.html
--rw-r--r--   0        0        0     1344 2023-03-05 14:58:35.324068 sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/searchbox.html
--rw-r--r--   0        0        0     1055 2023-03-05 14:58:35.324068 sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/sidebar.html
--rw-r--r--   0        0        0      432 2023-03-05 14:58:35.324068 sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/skip.html
--rw-r--r--   0        0        0    28348 2023-03-05 14:58:35.324068 sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/static/09be83022f2ac2ce16b0.woff
--rw-r--r--   0        0        0    22192 2023-03-05 14:58:35.324068 sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/static/31f64b9c465158bd6066.woff2
--rw-r--r--   0        0        0    17336 2023-03-05 14:58:35.324068 sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/static/3a43b67e5bbdfb3ab0a6.woff2
--rw-r--r--   0        0        0    26732 2023-03-05 14:58:35.324068 sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/static/42ba3027499c19034257.woff
--rw-r--r--   0        0        0    26680 2023-03-05 14:58:35.324068 sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/static/46830c334f8112fa510a.woff
--rw-r--r--   0        0        0    20544 2023-03-05 14:58:35.324068 sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/static/48af7707fe9e6494d6a5.woff
--rw-r--r--   0        0        0    25940 2023-03-05 14:58:35.324068 sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/static/6f04107ce68d524ebe69.woff
--rw-r--r--   0        0        0    22092 2023-03-05 14:58:35.324068 sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/static/9ac5da2442b734abc516.woff
--rw-r--r--   0        0        0    21184 2023-03-05 14:58:35.324068 sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/static/a49e53c029ef019e7422.woff2
--rw-r--r--   0        0        0    27532 2023-03-05 14:58:35.324068 sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/static/ad463ea60cc8b68792f4.woff
--rw-r--r--   0        0        0    15744 2023-03-05 14:58:35.324068 sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/static/b009a76ad6afe4ebd301.woff2
--rw-r--r--   0        0        0    22048 2023-03-05 14:58:35.324068 sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/static/d037cb4792991826de7d.woff
--rw-r--r--   0        0        0    20388 2023-03-05 14:58:35.324068 sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/static/d0b41bd1d599bc0a52b7.woff2
--rw-r--r--   0        0        0    15435 2023-03-05 14:58:35.324068 sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/static/docsearch.70ebcfe862b41f7a90b7.css
--rw-r--r--   0        0        0   106915 2023-03-05 14:58:35.324068 sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/static/docsearch.e95232a0fe67eecc8db0.js
--rw-r--r--   0        0        0      109 2023-03-05 14:58:35.324068 sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/static/docsearch.e95232a0fe67eecc8db0.js.LICENSE.txt
--rw-r--r--   0        0        0      263 2023-03-05 14:58:35.324068 sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/static/docsearch_config.js_t
--rw-r--r--   0        0        0    17368 2023-03-05 14:58:35.324068 sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/static/e10742dbb1d4a0864ba8.woff2
--rw-r--r--   0        0        0    20932 2023-03-05 14:58:35.324068 sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/static/ec416b97881f4a422686.woff2
--rw-r--r--   0        0        0    20344 2023-03-05 14:58:35.324068 sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/static/f1e2a76794cb86b2aa8e.woff
--rw-r--r--   0        0        0    15920 2023-03-05 14:58:35.324068 sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/static/f25d774ecfe0996f8eb5.woff2
--rw-r--r--   0        0        0    21412 2023-03-05 14:58:35.324068 sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/static/ff058b7e238adc5cba09.woff2
--rw-r--r--   0        0        0     1862 2023-03-05 14:58:35.324068 sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/static/manifest.json
--rw-r--r--   0        0        0    43143 2023-03-05 14:58:35.324068 sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/static/theme.39dcd091ff2d4f33bf46.css
--rw-r--r--   0        0        0    57350 2023-03-05 14:58:35.324068 sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/static/theme.b62e1ded0c8c099a2d47.js
--rw-r--r--   0        0        0       93 2023-03-05 14:58:35.324068 sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/static/theme.b62e1ded0c8c099a2d47.js.LICENSE.txt
--rw-r--r--   0        0        0      275 2023-03-05 14:58:35.324068 sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/theme.conf
--rw-r--r--   0        0        0     1269 2023-03-05 14:58:35.324068 sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/with-sidebar.html
--rw-r--r--   0        0        0     1101 2023-03-05 14:58:35.324068 sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/without-sidebar.html
--rw-r--r--   0        0        0     4168 1970-01-01 00:00:00.000000 sphinxawesome_theme-4.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-16 05:34:13.172649 sphinxawesome_theme-4.0.3/LICENSE
+-rw-r--r--   0        0        0     2857 2023-04-16 05:34:13.172649 sphinxawesome_theme-4.0.3/README.md
+-rw-r--r--   0        0        0     2189 2023-04-16 05:34:13.172649 sphinxawesome_theme-4.0.3/pyproject.toml
+-rw-r--r--   0        0        0      172 2023-04-16 05:34:13.172649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/README.rst
+-rw-r--r--   0        0        0     2733 2023-04-16 05:34:13.172649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/__init__.py
+-rw-r--r--   0        0        0      671 2023-04-16 05:34:13.172649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/breadcrumbs.html
+-rw-r--r--   0        0        0     2255 2023-04-16 05:34:13.172649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/docsearch.py
+-rw-r--r--   0        0        0      875 2023-04-16 05:34:13.172649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/footer.html
+-rw-r--r--   0        0        0     2726 2023-04-16 05:34:13.172649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/header.html
+-rw-r--r--   0        0        0    12023 2023-04-16 05:34:13.172649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/highlighting.py
+-rw-r--r--   0        0        0    11203 2023-04-16 05:34:13.172649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/html_translator.py
+-rw-r--r--   0        0        0     1668 2023-04-16 05:34:13.172649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/icons.py
+-rw-r--r--   0        0        0     3085 2023-04-16 05:34:13.172649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/jinja_functions.py
+-rw-r--r--   0        0        0     1239 2023-04-16 05:34:13.172649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/jsonimpl.py
+-rw-r--r--   0        0        0     2770 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/layout.html
+-rw-r--r--   0        0        0     1396 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/menu.html
+-rw-r--r--   0        0        0      622 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/modals.html
+-rw-r--r--   0        0        0      311 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/page.html
+-rw-r--r--   0        0        0     5817 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/postprocess.py
+-rw-r--r--   0        0        0      836 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/prev_next.html
+-rw-r--r--   0        0        0      692 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/scrolltop.html
+-rw-r--r--   0        0        0      808 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/search.html
+-rw-r--r--   0        0        0     1344 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/searchbox.html
+-rw-r--r--   0        0        0     1055 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/sidebar.html
+-rw-r--r--   0        0        0      432 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/skip.html
+-rw-r--r--   0        0        0    28348 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/09be83022f2ac2ce16b0.woff
+-rw-r--r--   0        0        0    22192 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/31f64b9c465158bd6066.woff2
+-rw-r--r--   0        0        0    17336 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/3a43b67e5bbdfb3ab0a6.woff2
+-rw-r--r--   0        0        0    26732 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/42ba3027499c19034257.woff
+-rw-r--r--   0        0        0    26680 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/46830c334f8112fa510a.woff
+-rw-r--r--   0        0        0    20544 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/48af7707fe9e6494d6a5.woff
+-rw-r--r--   0        0        0    25940 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/6f04107ce68d524ebe69.woff
+-rw-r--r--   0        0        0    22092 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/9ac5da2442b734abc516.woff
+-rw-r--r--   0        0        0    21184 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/a49e53c029ef019e7422.woff2
+-rw-r--r--   0        0        0    27532 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/ad463ea60cc8b68792f4.woff
+-rw-r--r--   0        0        0    15744 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/b009a76ad6afe4ebd301.woff2
+-rw-r--r--   0        0        0    22048 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/d037cb4792991826de7d.woff
+-rw-r--r--   0        0        0    20388 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/d0b41bd1d599bc0a52b7.woff2
+-rw-r--r--   0        0        0   106899 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/docsearch.53303c497cdefb581f6f.js
+-rw-r--r--   0        0        0      109 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/docsearch.53303c497cdefb581f6f.js.LICENSE.txt
+-rw-r--r--   0        0        0    15435 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/docsearch.70ebcfe862b41f7a90b7.css
+-rw-r--r--   0        0        0      263 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/docsearch_config.js_t
+-rw-r--r--   0        0        0    17368 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/e10742dbb1d4a0864ba8.woff2
+-rw-r--r--   0        0        0    20932 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/ec416b97881f4a422686.woff2
+-rw-r--r--   0        0        0    20344 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/f1e2a76794cb86b2aa8e.woff
+-rw-r--r--   0        0        0    15920 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/f25d774ecfe0996f8eb5.woff2
+-rw-r--r--   0        0        0    21412 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/ff058b7e238adc5cba09.woff2
+-rw-r--r--   0        0        0     1862 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/manifest.json
+-rw-r--r--   0        0        0    43174 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/theme.2e8060a090e1247124e3.css
+-rw-r--r--   0        0        0    57350 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/theme.b62e1ded0c8c099a2d47.js
+-rw-r--r--   0        0        0       93 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/theme.b62e1ded0c8c099a2d47.js.LICENSE.txt
+-rw-r--r--   0        0        0      275 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/theme.conf
+-rw-r--r--   0        0        0     1269 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/with-sidebar.html
+-rw-r--r--   0        0        0     1101 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/without-sidebar.html
+-rw-r--r--   0        0        0     4167 1970-01-01 00:00:00.000000 sphinxawesome_theme-4.0.3/PKG-INFO
```

### Comparing `sphinxawesome_theme-4.0.2/LICENSE` & `sphinxawesome_theme-4.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.2/README.md` & `sphinxawesome_theme-4.0.3/README.md`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.2/pyproject.toml` & `sphinxawesome_theme-4.0.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sphinxawesome-theme"
-version = "4.0.2"
+version = "4.0.3"
 description = "An awesome theme for the Sphinx documentation generator"
 readme = "README.md"
 authors = ["Kai Welke <kai687@pm.me>"]
 homepage = "https://sphinxawesome.xyz"
 documentation = "https://sphinxawesome.xyz"
 repository = "https://github.com/kai687/sphinxawesome-theme"
 license = "MIT"
@@ -21,27 +21,27 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 sphinx = ">4"
 beautifulsoup4 = "^4.9.1"
 python-dotenv = ">=0.19,<1.1"
-myst-parser = {version = ">=0.19,<0.20", optional = true}
+myst-parser = {version = ">=0.19,<1.1", optional = true}
 sphinx-autobuild = {version = "^2021.3.14", optional = true}
 sphinx-sitemap = { version = "^2.2.0", optional = true}
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1"
 pre-commit = "^3.1.1"
 pytest = "^7.2"
 pytest-cov = "^4.0"
 mypy = "^1.0"
 coverage = { extras = ["toml"], version = "^7.2" }
-isort = "^5.11.5"
-ruff = "^0.0.254"
+ruff = ">=0.0.254,<0.0.262"
+types-docutils = "^0.19.1.6"
 
 [tool.poetry.extras]
 docs = ["myst-parser", "sphinx-autobuild", "sphinx-sitemap"]
 
 [tool.coverage.paths]
 source = ["src"]
 
@@ -67,15 +67,15 @@
 pretty = true
 strict = true
 show_column_numbers = true
 warn_unreachable = true
 warn_unused_ignores = true
 
 [[tool.mypy.overrides]]
-module = ["pygments.*", "bs4", "dotenv", "sphinxcontrib.serializinghtml"]
+module = ["pygments.*", "bs4", "dotenv", "sphinxcontrib.serializinghtml", "nox_poetry"]
 ignore_missing_imports = true
 
 [tool.poetry.plugins."sphinx.html_themes"]
 "sphinxawesome_theme" = "sphinxawesome_theme"
 
 [build-system]
 requires = ["poetry_core"]
```

### Comparing `sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/__init__.py` & `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/breadcrumbs.html` & `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/docsearch.py` & `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/docsearch.py`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/footer.html` & `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/footer.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/header.html` & `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/header.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/highlighting.py` & `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/highlighting.py`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/html_translator.py` & `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/html_translator.py`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/icons.py` & `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/icons.py`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/jinja_functions.py` & `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/jinja_functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,42 +40,51 @@
     if app.builder and app.builder.theme:  # type: ignore[attr-defined]
         # find the first 'manifest.json' file in the theme's directories
         for entry in app.builder.theme.get_theme_dirs()[::-1]:  # type: ignore[attr-defined] # noqa: E501,B950
             manifest = path.join(entry, "static", "manifest.json")
             if path.isfile(manifest):
                 with open(manifest) as m:
                     return json.load(m)
-        else:
-            return {}
     else:
         return {}
 
 
 def _make_asset_url(app: Sphinx, asset: str) -> Any:
     """Turn a *clean* asset file name to a hashed one."""
     manifest = _get_manifest_json(app)
 
     # return the asset itself if it is not in the manifest
     return manifest.get(asset, asset)
 
 
+def _make_canonical(app: Sphinx, pagename: str) -> str:
+    """Turn a filepath into the correct canonical link.
+
+    Upstream Sphinx builds the wrong canonical links for the ``dirhtml`` builder.
+    """
+    canonical = posixpath.join(app.config.html_baseurl, pagename.replace("index", ""))
+    if not canonical.endswith("/"):
+        canonical += "/"
+    return canonical
+
+
 def setup_jinja(
     app: Sphinx,
     pagename: str,
     templatename: str,
     context: Dict[str, Any],
     doctree: Node,
 ) -> None:
     """Register a function as a Jinja2 filter."""
     if app.builder is not None:
         app.builder.templates.environment.filters["sanitize"] = _make_id_from_title
         context["asset"] = partial(_make_asset_url, app)
         # must override `pageurl` for directory builder
-        if app.builder.name == "dirhtml":
-            context["pageurl"] = posixpath.join(app.config.html_baseurl, pagename + "/")
+        if app.builder.name == "dirhtml" and app.config.html_baseurl:
+            context["pageurl"] = _make_canonical(app, pagename)
 
 
 def setup(app: Sphinx) -> Dict[str, Any]:
     """Register this jinja filter as extension."""
     app.connect("html-page-context", setup_jinja)
 
     return {
```

### Comparing `sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/jsonimpl.py` & `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/jsonimpl.py`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/menu.html` & `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/menu.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/modals.html` & `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/modals.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/postprocess.py` & `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/postprocess.py`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/prev_next.html` & `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/prev_next.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/scrolltop.html` & `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/scrolltop.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/search.html` & `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/search.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/searchbox.html` & `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/searchbox.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/sidebar.html` & `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/sidebar.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/static/09be83022f2ac2ce16b0.woff` & `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/09be83022f2ac2ce16b0.woff`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/static/31f64b9c465158bd6066.woff2` & `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/31f64b9c465158bd6066.woff2`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/static/3a43b67e5bbdfb3ab0a6.woff2` & `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/3a43b67e5bbdfb3ab0a6.woff2`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/static/42ba3027499c19034257.woff` & `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/42ba3027499c19034257.woff`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/static/46830c334f8112fa510a.woff` & `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/46830c334f8112fa510a.woff`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/static/48af7707fe9e6494d6a5.woff` & `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/48af7707fe9e6494d6a5.woff`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/static/6f04107ce68d524ebe69.woff` & `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/6f04107ce68d524ebe69.woff`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/static/9ac5da2442b734abc516.woff` & `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/9ac5da2442b734abc516.woff`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/static/a49e53c029ef019e7422.woff2` & `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/a49e53c029ef019e7422.woff2`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/static/ad463ea60cc8b68792f4.woff` & `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/ad463ea60cc8b68792f4.woff`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/static/b009a76ad6afe4ebd301.woff2` & `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/b009a76ad6afe4ebd301.woff2`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/static/d037cb4792991826de7d.woff` & `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/d037cb4792991826de7d.woff`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/static/d0b41bd1d599bc0a52b7.woff2` & `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/d0b41bd1d599bc0a52b7.woff2`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/static/docsearch.70ebcfe862b41f7a90b7.css` & `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/docsearch.70ebcfe862b41f7a90b7.css`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/static/docsearch.e95232a0fe67eecc8db0.js` & `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/docsearch.53303c497cdefb581f6f.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see docsearch.e95232a0fe67eecc8db0.js.LICENSE.txt */ ! function() {
+/*! For license information please see docsearch.53303c497cdefb581f6f.js.LICENSE.txt */ ! function() {
     "use strict";
 
     function e(e, t) {
         var n = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var r = Object.getOwnPropertySymbols(e);
             t && (r = r.filter((function(t) {
@@ -3690,74 +3690,71 @@
         }
     }
     var hr = {
             Read: 1,
             Write: 2,
             Any: 3
         },
-        vr = 1,
-        yr = 2,
-        _r = 3;
+        vr = 1;
 
-    function br(e) {
+    function yr(e) {
         var n = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : vr;
         return t(t({}, e), {}, {
             status: n,
             lastUpdate: Date.now()
         })
     }
 
-    function gr(e) {
+    function _r(e) {
         return "string" == typeof e ? {
             protocol: "https",
             url: e,
             accept: hr.Any
         } : {
             protocol: e.protocol || "https",
             url: e.url,
             accept: e.accept || hr.Any
         }
     }
-    var Or = "GET",
-        Sr = "POST";
+    var br = "POST";
 
-    function Er(e, n, r, o) {
+    function gr(e, n, r, o) {
         var c = [],
             a = function(e, n) {
-                if (e.method !== Or && (void 0 !== e.data || void 0 !== n.data)) {
+                if ("GET" !== e.method && (void 0 !== e.data || void 0 !== n.data)) {
                     var r = Array.isArray(e.data) ? e.data : t(t({}, e.data), n.data);
                     return JSON.stringify(r)
                 }
             }(r, o),
             u = function(e, n) {
                 var r = t(t({}, e.headers), n.headers),
                     o = {};
                 return Object.keys(r).forEach((function(e) {
                     var t = r[e];
                     o[e.toLowerCase()] = t
                 })), o
             }(e, o),
             l = r.method,
-            s = r.method !== Or ? {} : t(t({}, r.data), o.data),
+            s = "GET" !== r.method ? {} : t(t({}, r.data), o.data),
             f = t(t(t({
                 "x-algolia-agent": e.userAgent.value
             }, e.queryParameters), s), o.queryParameters),
             p = 0,
             m = function t(n, i) {
                 var s = n.pop();
                 if (void 0 === s) throw {
                     name: "RetryError",
                     message: "Unreachable hosts - your application id may be incorrect. If the error persists, contact support@algolia.com.",
-                    transporterStackTrace: Ir(c)
+                    transporterStackTrace: wr(c)
                 };
                 var m = {
                         data: a,
                         headers: u,
                         method: l,
-                        url: jr(s, r.path, f),
+                        url: Sr(s, r.path, f),
                         connectTimeout: i(p, e.timeouts.connect),
                         responseTimeout: i(p, o.timeout)
                     },
                     d = function(e) {
                         var t = {
                             request: m,
                             response: e,
@@ -3780,15 +3777,15 @@
                                         }
                                     }(t.message, e)
                                 }
                             }(e)
                         },
                         onRetry: function(r) {
                             var o = d(r);
-                            return r.isTimedOut && p++, Promise.all([e.logger.info("Retryable failure", kr(o)), e.hostsCache.set(s, br(s, r.isTimedOut ? _r : yr))]).then((function() {
+                            return r.isTimedOut && p++, Promise.all([e.logger.info("Retryable failure", jr(o)), e.hostsCache.set(s, yr(s, r.isTimedOut ? 3 : 2))]).then((function() {
                                 return t(n, i)
                             }))
                         },
                         onFail: function(e) {
                             throw d(e),
                                 function(e, t) {
                                     var n = e.content,
@@ -3801,15 +3798,15 @@
                                         return {
                                             name: "ApiError",
                                             message: e,
                                             status: t,
                                             transporterStackTrace: n
                                         }
                                     }(o, r, t)
-                                }(e, Ir(c))
+                                }(e, wr(c))
                         }
                     };
                 return e.requester.send(m).then((function(e) {
                     return function(e, t) {
                         return function(e) {
                             var t = e.status;
                             return e.isTimedOut || function(e) {
@@ -3820,83 +3817,83 @@
                         }(e) ? t.onRetry(e) : 2 == ~~(e.status / 100) ? t.onSucess(e) : t.onFail(e)
                     }(e, h)
                 }))
             };
         return function(e, t) {
             return Promise.all(t.map((function(t) {
                 return e.get(t, (function() {
-                    return Promise.resolve(br(t))
+                    return Promise.resolve(yr(t))
                 }))
             }))).then((function(e) {
                 var n = e.filter((function(e) {
                         return function(e) {
                             return e.status === vr || Date.now() - e.lastUpdate > 12e4
                         }(e)
                     })),
                     r = e.filter((function(e) {
                         return function(e) {
-                            return e.status === _r && Date.now() - e.lastUpdate <= 12e4
+                            return 3 === e.status && Date.now() - e.lastUpdate <= 12e4
                         }(e)
                     })),
                     o = [].concat(i(n), i(r));
                 return {
                     getTimeout: function(e, t) {
                         return (0 === r.length && 0 === e ? 1 : r.length + 3 + e) * t
                     },
                     statelessHosts: o.length > 0 ? o.map((function(e) {
-                        return gr(e)
+                        return _r(e)
                     })) : t
                 }
             }))
         }(e.hostsCache, n).then((function(e) {
             return m(i(e.statelessHosts).reverse(), e.getTimeout)
         }))
     }
 
-    function wr(e) {
+    function Or(e) {
         var t = {
             value: "Algolia for JavaScript (".concat(e, ")"),
             add: function(e) {
                 var n = "; ".concat(e.segment).concat(void 0 !== e.version ? " (".concat(e.version, ")") : "");
                 return -1 === t.value.indexOf(n) && (t.value = "".concat(t.value).concat(n)), t
             }
         };
         return t
     }
 
-    function jr(e, t, n) {
-        var r = Pr(n),
+    function Sr(e, t, n) {
+        var r = Er(n),
             o = "".concat(e.protocol, "://").concat(e.url, "/").concat("/" === t.charAt(0) ? t.substr(1) : t);
         return r.length && (o += "?".concat(r)), o
     }
 
-    function Pr(e) {
+    function Er(e) {
         return Object.keys(e).map((function(t) {
             return pr("%s=%s", t, (n = e[t], "[object Object]" === Object.prototype.toString.call(n) || "[object Array]" === Object.prototype.toString.call(n) ? JSON.stringify(e[t]) : e[t]));
             var n
         })).join("&")
     }
 
-    function Ir(e) {
+    function wr(e) {
         return e.map((function(e) {
-            return kr(e)
+            return jr(e)
         }))
     }
 
-    function kr(e) {
+    function jr(e) {
         var n = e.request.headers["x-algolia-api-key"] ? {
             "x-algolia-api-key": "*****"
         } : {};
         return t(t({}, e), {}, {
             request: t(t({}, e.request), {}, {
                 headers: t(t({}, e.request.headers), n)
             })
         })
     }
-    var Dr = function(e) {
+    var Pr = function(e) {
             var n = e.appId,
                 r = function(e, t, n) {
                     var r = {
                         "x-algolia-api-key": n,
                         "x-algolia-application-id": t
                     };
                     return {
@@ -3925,20 +3922,20 @@
                             requestsCache: o,
                             responsesCache: i,
                             timeouts: a,
                             userAgent: u,
                             headers: e.headers,
                             queryParameters: s,
                             hosts: l.map((function(e) {
-                                return gr(e)
+                                return _r(e)
                             })),
                             read: function(e, t) {
                                 var n = dr(t, f.timeouts.read),
                                     r = function() {
-                                        return Er(f, f.hosts.filter((function(e) {
+                                        return gr(f, f.hosts.filter((function(e) {
                                             return 0 != (e.accept & hr.Read)
                                         })), e, n)
                                     };
                                 if (!0 !== (void 0 !== n.cacheable ? n.cacheable : e.cacheable)) return r();
                                 var o = {
                                     request: e,
                                     mappedRequestOptions: n,
@@ -3961,15 +3958,15 @@
                                 }), {
                                     miss: function(e) {
                                         return f.responsesCache.set(o, e)
                                     }
                                 })
                             },
                             write: function(e, t) {
-                                return Er(f, f.hosts.filter((function(e) {
+                                return gr(f, f.hosts.filter((function(e) {
                                     return 0 != (e.accept & hr.Write)
                                 })), e, dr(t, f.timeouts.write))
                             }
                         };
                     return f
                 }(t(t({
                     hosts: [{
@@ -4002,42 +3999,42 @@
                     },
                     clearCache: function() {
                         return Promise.all([o.requestsCache.clear(), o.responsesCache.clear()]).then((function() {}))
                     }
                 };
             return fr(i, e.methods)
         },
-        Cr = function(e) {
+        Ir = function(e) {
             return function(t) {
                 var n = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
                 return fr({
                     transporter: e.transporter,
                     appId: e.appId,
                     indexName: t
                 }, n.methods)
             }
         },
-        Ar = function(e) {
+        kr = function(e) {
             return function(n, r) {
                 var o = n.map((function(e) {
                     return t(t({}, e), {}, {
-                        params: Pr(e.params || {})
+                        params: Er(e.params || {})
                     })
                 }));
                 return e.transporter.read({
-                    method: Sr,
+                    method: br,
                     path: "1/indexes/*/queries",
                     data: {
                         requests: o
                     },
                     cacheable: !0
                 }, r)
             }
         },
-        xr = function(e) {
+        Dr = function(e) {
             return function(n, r) {
                 return Promise.all(n.map((function(n) {
                     var o = n.params,
                         c = o.facetName,
                         i = o.facetQuery,
                         a = function(e, t) {
                             if (null == e) return {};
@@ -4050,64 +4047,64 @@
                             }(e, t);
                             if (Object.getOwnPropertySymbols) {
                                 var c = Object.getOwnPropertySymbols(e);
                                 for (r = 0; r < c.length; r++) n = c[r], t.indexOf(n) >= 0 || Object.prototype.propertyIsEnumerable.call(e, n) && (o[n] = e[n])
                             }
                             return o
                         }(o, ir);
-                    return Cr(e)(n.indexName, {
+                    return Ir(e)(n.indexName, {
                         methods: {
-                            searchForFacetValues: Tr
+                            searchForFacetValues: xr
                         }
                     }).searchForFacetValues(c, i, t(t({}, r), a))
                 })))
             }
         },
-        Nr = function(e) {
+        Cr = function(e) {
             return function(t, n, r) {
                 return e.transporter.read({
-                    method: Sr,
+                    method: br,
                     path: pr("1/answers/%s/prediction", e.indexName),
                     data: {
                         query: t,
                         queryLanguages: n
                     },
                     cacheable: !0
                 }, r)
             }
         },
-        Rr = function(e) {
+        Ar = function(e) {
             return function(t, n) {
                 return e.transporter.read({
-                    method: Sr,
+                    method: br,
                     path: pr("1/indexes/%s/query", e.indexName),
                     data: {
                         query: t
                     },
                     cacheable: !0
                 }, n)
             }
         },
-        Tr = function(e) {
+        xr = function(e) {
             return function(t, n, r) {
                 return e.transporter.read({
-                    method: Sr,
+                    method: br,
                     path: pr("1/indexes/%s/facets/%s/query", e.indexName, t),
                     data: {
                         facetQuery: n
                     },
                     cacheable: !0
                 }, r)
             }
         },
-        Lr = 1,
-        qr = 2,
-        Mr = 3;
+        Nr = 1,
+        Rr = 2,
+        Tr = 3;
 
-    function Hr(e, n, r) {
+    function Lr(e, n, r) {
         var o, c = {
             appId: e,
             apiKey: n,
             timeouts: {
                 connect: 1,
                 read: 2,
                 write: 30
@@ -4143,112 +4140,112 @@
                                 status: n.status,
                                 isTimedOut: !1
                             })
                         }, n.send(e.data)
                     }))
                 }
             },
-            logger: (o = Mr, {
+            logger: (o = Tr, {
                 debug: function(e, t) {
-                    return Lr >= o && console.debug(e, t), Promise.resolve()
+                    return Nr >= o && console.debug(e, t), Promise.resolve()
                 },
                 info: function(e, t) {
-                    return qr >= o && console.info(e, t), Promise.resolve()
+                    return Rr >= o && console.info(e, t), Promise.resolve()
                 },
                 error: function(e, t) {
                     return console.error(e, t), Promise.resolve()
                 }
             }),
             responsesCache: lr(),
             requestsCache: lr({
                 serializable: !1
             }),
             hostsCache: ur({
                 caches: [ar({
                     key: "".concat("4.8.5", "-").concat(e)
                 }), lr()]
             }),
-            userAgent: wr("4.8.5").add({
+            userAgent: Or("4.8.5").add({
                 segment: "Browser",
                 version: "lite"
             }),
             authMode: mr.WithinQueryParameters
         };
-        return Dr(t(t(t({}, c), r), {}, {
+        return Pr(t(t(t({}, c), r), {}, {
             methods: {
-                search: Ar,
-                searchForFacetValues: xr,
-                multipleQueries: Ar,
-                multipleSearchForFacetValues: xr,
+                search: kr,
+                searchForFacetValues: Dr,
+                multipleQueries: kr,
+                multipleSearchForFacetValues: Dr,
                 initIndex: function(e) {
                     return function(t) {
-                        return Cr(e)(t, {
+                        return Ir(e)(t, {
                             methods: {
-                                search: Rr,
-                                searchForFacetValues: Tr,
-                                findAnswers: Nr
+                                search: Ar,
+                                searchForFacetValues: xr,
+                                findAnswers: Cr
                             }
                         })
                     }
                 }
             }
         }))
     }
-    Hr.version = "4.8.5";
-    var Ur = ["footer", "searchBox"];
+    Lr.version = "4.8.5";
+    var qr = ["footer", "searchBox"];
 
-    function Fr() {
-        return Fr = Object.assign || function(e) {
+    function Mr() {
+        return Mr = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = arguments[t];
                 for (var r in n) Object.prototype.hasOwnProperty.call(n, r) && (e[r] = n[r])
             }
             return e
-        }, Fr.apply(this, arguments)
+        }, Mr.apply(this, arguments)
     }
 
-    function Br(e, t) {
+    function Hr(e, t) {
         var n = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var r = Object.getOwnPropertySymbols(e);
             t && (r = r.filter((function(t) {
                 return Object.getOwnPropertyDescriptor(e, t).enumerable
             }))), n.push.apply(n, r)
         }
         return n
     }
 
-    function Vr(e) {
+    function Ur(e) {
         for (var t = 1; t < arguments.length; t++) {
             var n = null != arguments[t] ? arguments[t] : {};
-            t % 2 ? Br(Object(n), !0).forEach((function(t) {
-                Wr(e, t, n[t])
-            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Br(Object(n)).forEach((function(t) {
+            t % 2 ? Hr(Object(n), !0).forEach((function(t) {
+                Fr(e, t, n[t])
+            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Hr(Object(n)).forEach((function(t) {
                 Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
             }))
         }
         return e
     }
 
-    function Wr(e, t, n) {
+    function Fr(e, t, n) {
         return t in e ? Object.defineProperty(e, t, {
             value: n,
             enumerable: !0,
             configurable: !0,
             writable: !0
         }) : e[t] = n, e
     }
 
-    function Kr(e, t) {
+    function Br(e, t) {
         (null == t || t > e.length) && (t = e.length);
         for (var n = 0, r = new Array(t); n < t; n++) r[n] = e[n];
         return r
     }
 
-    function zr(e) {
+    function Vr(e) {
         var t = e.appId,
             n = e.apiKey,
             r = e.indexName,
             o = e.placeholder,
             c = void 0 === o ? "Search docs" : o,
             i = e.searchParameters,
             a = e.onClose,
@@ -4285,15 +4282,15 @@
                     return o
                 }(e, t);
                 if (Object.getOwnPropertySymbols) {
                     var c = Object.getOwnPropertySymbols(e);
                     for (r = 0; r < c.length; r++) n = c[r], t.indexOf(n) >= 0 || Object.prototype.propertyIsEnumerable.call(e, n) && (o[n] = e[n])
                 }
                 return o
-            }(j, Ur),
+            }(j, qr),
             C = function(e, t) {
                 return function(e) {
                     if (Array.isArray(e)) return e
                 }(e) || function(e, t) {
                     var n = null == e ? null : "undefined" != typeof Symbol && e[Symbol.iterator] || e["@@iterator"];
                     if (null != n) {
                         var r, o, c = [],
@@ -4310,17 +4307,17 @@
                                 if (a) throw o
                             }
                         }
                         return c
                     }
                 }(e) || function(e, t) {
                     if (e) {
-                        if ("string" == typeof e) return Kr(e, 2);
+                        if ("string" == typeof e) return Br(e, 2);
                         var n = Object.prototype.toString.call(e).slice(8, -1);
-                        return "Object" === n && e.constructor && (n = e.constructor.name), "Map" === n || "Set" === n ? Array.from(e) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? Kr(e, 2) : void 0
+                        return "Object" === n && e.constructor && (n = e.constructor.name), "Map" === n || "Set" === n ? Array.from(e) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? Br(e, 2) : void 0
                     }
                 }(e) || function() {
                     throw new TypeError("Invalid attempt to destructure non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
                 }()
             }(Fe.useState({
                 query: "",
                 collections: [],
@@ -4338,15 +4335,15 @@
             L = Fe.useRef(null),
             q = Fe.useRef(null),
             M = Fe.useRef(10),
             H = Fe.useRef("undefined" != typeof window ? window.getSelection().toString().slice(0, 64) : "").current,
             U = Fe.useRef(E || H).current,
             F = function(e, t, n) {
                 return Fe.useMemo((function() {
-                    var r = Hr(e, t);
+                    var r = Lr(e, t);
                     return r.addAlgoliaAgent("docsearch", "3.3.3"), !1 === /docsearch.js \(.*\)/.test(r.transporter.userAgent.value) && r.addAlgoliaAgent("docsearch-react", "3.3.3"), n(r)
                 }), [e, t, n])
             }(t, n, b),
             B = Fe.useRef(cr({
                 key: "__DOCSEARCH_FAVORITE_SEARCHES__".concat(r),
                 limit: 10
             })).current,
@@ -4382,15 +4379,15 @@
                         var t = e.query,
                             n = e.state,
                             o = e.setContext,
                             c = e.setStatus;
                         return t ? F.search([{
                             query: t,
                             indexName: r,
-                            params: Vr({
+                            params: Ur({
                                 attributesToRetrieve: ["hierarchy.lvl0", "hierarchy.lvl1", "hierarchy.lvl2", "hierarchy.lvl3", "hierarchy.lvl4", "hierarchy.lvl5", "hierarchy.lvl6", "content", "type", "url"],
                                 attributesToSnippet: ["hierarchy.lvl1:".concat(M.current), "hierarchy.lvl2:".concat(M.current), "hierarchy.lvl3:".concat(M.current), "hierarchy.lvl4:".concat(M.current), "hierarchy.lvl5:".concat(M.current), "hierarchy.lvl6:".concat(M.current), "content:".concat(M.current)],
                                 snippetEllipsisText: "…",
                                 highlightPreTag: "<mark>",
                                 highlightPostTag: "</mark>",
                                 hitsPerPage: 20
                             }, i)
@@ -4419,15 +4416,15 @@
                                         return e.item.url
                                     },
                                     getItems: function() {
                                         return Object.values(Fn(e, (function(e) {
                                             return e.hierarchy.lvl1
                                         }))).map(s).map((function(e) {
                                             return e.map((function(t) {
-                                                return Vr(Vr({}, t), {}, {
+                                                return Ur(Ur({}, t), {}, {
                                                     __docsearch_parent: "lvl1" !== t.type && e.find((function(e) {
                                                         return "lvl1" === e.type && e.hierarchy.lvl1 === t.hierarchy.lvl1
                                                     }))
                                                 })
                                             }))
                                         })).flat()
                                     }
@@ -4530,15 +4527,15 @@
                         R.current.style.setProperty("--docsearch-vh", "".concat(e, "px"))
                     }
                 }
                 return e(), window.addEventListener("resize", e),
                     function() {
                         window.removeEventListener("resize", e)
                     }
-            }), []), Fe.createElement("div", Fr({
+            }), []), Fe.createElement("div", Mr({
                 ref: N
             }, J({
                 "aria-expanded": !0
             }), {
                 className: ["DocSearch", "DocSearch-Container", "stalled" === A.status && "DocSearch-Container--Stalled", "error" === A.status && "DocSearch-Container--Errored"].filter(Boolean).join(" "),
                 role: "button",
                 tabIndex: 0,
@@ -4547,25 +4544,25 @@
                 }
             }), Fe.createElement("div", {
                 className: "DocSearch-Modal",
                 ref: R
             }, Fe.createElement("header", {
                 className: "DocSearch-SearchBar",
                 ref: T
-            }, Fe.createElement(rr, Fr({}, K, {
+            }, Fe.createElement(rr, Mr({}, K, {
                 state: A,
                 autoFocus: 0 === U.length,
                 inputRef: q,
                 isFromSelection: Boolean(U) && U === H,
                 translations: k,
                 onClose: u
             }))), Fe.createElement("div", {
                 className: "DocSearch-Dropdown",
                 ref: L
-            }, Fe.createElement(er, Fr({}, K, {
+            }, Fe.createElement(er, Mr({}, K, {
                 indexName: r,
                 state: A,
                 hitComponent: p,
                 resultsFooterComponent: d,
                 disableUserPersonalization: O,
                 recentSearches: V,
                 favoriteSearches: B,
@@ -4578,25 +4575,25 @@
             }))), Fe.createElement("footer", {
                 className: "DocSearch-Footer"
             }, Fe.createElement(mn, {
                 translations: I
             }))))
     }
 
-    function Jr() {
-        return Jr = Object.assign || function(e) {
+    function Wr() {
+        return Wr = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = arguments[t];
                 for (var r in n) Object.prototype.hasOwnProperty.call(n, r) && (e[r] = n[r])
             }
             return e
-        }, Jr.apply(this, arguments)
+        }, Wr.apply(this, arguments)
     }
 
-    function $r(e, t) {
+    function Kr(e, t) {
         return function(e) {
             if (Array.isArray(e)) return e
         }(e) || function(e, t) {
             var n = null == e ? null : "undefined" != typeof Symbol && e[Symbol.iterator] || e["@@iterator"];
             if (null != n) {
                 var r, o, c = [],
                     i = !0,
@@ -4612,35 +4609,35 @@
                         if (a) throw o
                     }
                 }
                 return c
             }
         }(e, t) || function(e, t) {
             if (e) {
-                if ("string" == typeof e) return Qr(e, t);
+                if ("string" == typeof e) return zr(e, t);
                 var n = Object.prototype.toString.call(e).slice(8, -1);
-                return "Object" === n && e.constructor && (n = e.constructor.name), "Map" === n || "Set" === n ? Array.from(e) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? Qr(e, t) : void 0
+                return "Object" === n && e.constructor && (n = e.constructor.name), "Map" === n || "Set" === n ? Array.from(e) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? zr(e, t) : void 0
             }
         }(e, t) || function() {
             throw new TypeError("Invalid attempt to destructure non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
         }()
     }
 
-    function Qr(e, t) {
+    function zr(e, t) {
         (null == t || t > e.length) && (t = e.length);
         for (var n = 0, r = new Array(t); n < t; n++) r[n] = e[n];
         return r
     }
 
-    function Zr(e) {
+    function Jr(e) {
         var t, n, r = Fe.useRef(null),
-            o = $r(Fe.useState(!1), 2),
+            o = Kr(Fe.useState(!1), 2),
             c = o[0],
             i = o[1],
-            a = $r(Fe.useState((null == e ? void 0 : e.initialQuery) || void 0), 2),
+            a = Kr(Fe.useState((null == e ? void 0 : e.initialQuery) || void 0), 2),
             u = a[0],
             l = a[1],
             s = Fe.useCallback((function() {
                 i(!0)
             }), [i]),
             f = Fe.useCallback((function() {
                 i(!1)
@@ -4672,23 +4669,23 @@
                 i(!0), l(e.key)
             }), [i, l]),
             searchButtonRef: r
         }), Fe.createElement(Fe.Fragment, null, Fe.createElement(Je, {
             ref: r,
             translations: null == e || null === (t = e.translations) || void 0 === t ? void 0 : t.button,
             onClick: s
-        }), c && Pe(Fe.createElement(zr, Jr({}, e, {
+        }), c && Pe(Fe.createElement(Vr, Wr({}, e, {
             initialScrollY: window.scrollY,
             initialQuery: u,
             translations: null == e || null === (n = e.translations) || void 0 === n ? void 0 : n.modal,
             onClose: f
         })), document.body))
     }
     window.docsearch = function(e) {
-        Ce(Fe.createElement(Zr, o({}, e, {
+        Ce(Fe.createElement(Jr, o({}, e, {
             transformSearchClient: function(t) {
                 return t.addAlgoliaAgent("docsearch.js", "3.3.3"), e.transformSearchClient ? e.transformSearchClient(t) : t
             }
         })), function(e) {
             var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : window;
             return "string" == typeof e ? t.document.querySelector(e) : e
         }(e.container, e.environment))
```

### Comparing `sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/static/e10742dbb1d4a0864ba8.woff2` & `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/e10742dbb1d4a0864ba8.woff2`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/static/ec416b97881f4a422686.woff2` & `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/ec416b97881f4a422686.woff2`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/static/f1e2a76794cb86b2aa8e.woff` & `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/f1e2a76794cb86b2aa8e.woff`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/static/f25d774ecfe0996f8eb5.woff2` & `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/f25d774ecfe0996f8eb5.woff2`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/static/ff058b7e238adc5cba09.woff2` & `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/ff058b7e238adc5cba09.woff2`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/static/manifest.json` & `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/manifest.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9565217391304348%*

 * *Differences: {"'_static/docsearch.js'": "'_static/docsearch.53303c497cdefb581f6f.js'",*

 * * "'_static/theme.css'": "'_static/theme.2e8060a090e1247124e3.css'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "_static/docsearch.css": "_static/docsearch.70ebcfe862b41f7a90b7.css",
-    "_static/docsearch.js": "_static/docsearch.e95232a0fe67eecc8db0.js",
+    "_static/docsearch.js": "_static/docsearch.53303c497cdefb581f6f.js",
     "_static/docsearch_config.js_t": "_static/docsearch_config.js_t",
     "_static/jetbrains-mono-latin-400-italic.woff": "_static/ad463ea60cc8b68792f4.woff",
     "_static/jetbrains-mono-latin-400-italic.woff2": "_static/ff058b7e238adc5cba09.woff2",
     "_static/jetbrains-mono-latin-400-normal.woff": "_static/6f04107ce68d524ebe69.woff",
     "_static/jetbrains-mono-latin-400-normal.woff2": "_static/d0b41bd1d599bc0a52b7.woff2",
     "_static/jetbrains-mono-latin-500-italic.woff": "_static/09be83022f2ac2ce16b0.woff",
     "_static/jetbrains-mono-latin-500-italic.woff2": "_static/31f64b9c465158bd6066.woff2",
@@ -16,10 +16,10 @@
     "_static/roboto-latin-400-italic.woff2": "_static/e10742dbb1d4a0864ba8.woff2",
     "_static/roboto-latin-400-normal.woff": "_static/f1e2a76794cb86b2aa8e.woff",
     "_static/roboto-latin-400-normal.woff2": "_static/b009a76ad6afe4ebd301.woff2",
     "_static/roboto-latin-500-italic.woff": "_static/9ac5da2442b734abc516.woff",
     "_static/roboto-latin-500-italic.woff2": "_static/3a43b67e5bbdfb3ab0a6.woff2",
     "_static/roboto-latin-500-normal.woff": "_static/48af7707fe9e6494d6a5.woff",
     "_static/roboto-latin-500-normal.woff2": "_static/f25d774ecfe0996f8eb5.woff2",
-    "_static/theme.css": "_static/theme.39dcd091ff2d4f33bf46.css",
+    "_static/theme.css": "_static/theme.2e8060a090e1247124e3.css",
     "_static/theme.js": "_static/theme.b62e1ded0c8c099a2d47.js"
 }
```

### Comparing `sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/static/theme.39dcd091ff2d4f33bf46.css` & `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/theme.2e8060a090e1247124e3.css`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/*! tailwindcss v3.2.7 | MIT License | https://tailwindcss.com*/*,:after,:before{border:0 solid #e5e7eb;box-sizing:border-box}:after,:before{--tw-content:""}html{-webkit-text-size-adjust:100%;font-feature-settings:normal;font-family:Roboto,sans-serif;line-height:1.5;-moz-tab-size:4;-o-tab-size:4;tab-size:4}body{line-height:inherit;margin:0}hr{border-top-width:1px;color:inherit;height:0}abbr:where([title]){text-decoration:underline;-webkit-text-decoration:underline dotted;text-decoration:underline dotted}h1,h2,h3,h4,h5,h6{font-size:inherit;font-weight:inherit}a{color:inherit;text-decoration:inherit}b,strong{font-weight:bolder}code,kbd,pre,samp{font-family:JetBrains\ Mono,monospace;font-size:1em}small{font-size:80%}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline}sub{bottom:-.25em}sup{top:-.5em}table{border-collapse:collapse;border-color:inherit;text-indent:0}button,input,optgroup,select,textarea{color:inherit;font-family:inherit;font-size:100%;font-weight:inherit;line-height:inherit;margin:0;padding:0}button,select{text-transform:none}[type=button],[type=reset],[type=submit],button{-webkit-appearance:button;background-color:transparent;background-image:none}:-moz-focusring{outline:auto}:-moz-ui-invalid{box-shadow:none}progress{vertical-align:baseline}::-webkit-inner-spin-button,::-webkit-outer-spin-button{height:auto}[type=search]{-webkit-appearance:textfield;outline-offset:-2px}::-webkit-search-decoration{-webkit-appearance:none}::-webkit-file-upload-button{-webkit-appearance:button;font:inherit}summary{display:list-item}blockquote,dd,dl,figure,h1,h2,h3,h4,h5,h6,hr,p,pre{margin:0}fieldset{margin:0}fieldset,legend{padding:0}menu,ol,ul{list-style:none;margin:0;padding:0}textarea{resize:vertical}input::-moz-placeholder,textarea::-moz-placeholder{color:#9ca3af;opacity:1}input::placeholder,textarea::placeholder{color:#9ca3af;opacity:1}[role=button],button{cursor:pointer}:disabled{cursor:default}audio,canvas,embed,iframe,img,object,svg,video{display:block;vertical-align:middle}img,video{height:auto;max-width:100%}[hidden]{display:none}button,input{-webkit-appearance:none;-moz-appearance:none;appearance:none;border-radius:0}main footer,main section{max-width:760px}section>section{padding-bottom:1.5rem;padding-top:1.5rem}@media print{section>section{padding-bottom:0;padding-top:0}}section>p{margin-bottom:1.5rem;margin-top:1.5rem}hr{border-top-width:1px;margin-bottom:3rem}strong{font-weight:500}svg{display:inline}h1{--tw-text-opacity:1;color:#212121;color:rgb(33 33 33/var(--tw-text-opacity));font-size:2.5rem;letter-spacing:-.025em;line-height:1.2;margin-top:5rem}@media print{h1{margin-top:0}}h2{--tw-text-opacity:1;color:#212121;color:rgb(33 33 33/var(--tw-text-opacity));font-size:1.5rem;letter-spacing:-.025em;line-height:1.2;line-height:1.5rem;margin-bottom:2rem}@media (min-width:640px){h2{font-size:1.75rem;line-height:1.2}}h3{font-size:1.375rem;line-height:1.2}h3,h4{--tw-text-opacity:1;color:#212121;color:rgb(33 33 33/var(--tw-text-opacity))}h4{font-weight:500}article ol{list-style-type:decimal}article ol,article ol ol{margin-bottom:1rem;margin-top:1rem;padding-left:1.25rem}article ol ol{list-style-type:lower-latin}article ol li{margin-bottom:1rem;margin-top:1rem;padding-left:.25rem}article ol li::marker{--tw-text-opacity:1;color:#212121;color:rgb(33 33 33/var(--tw-text-opacity));font-weight:500}article ol li p{margin-bottom:.5rem;margin-top:.5rem}article ul{list-style-type:disc;padding-left:1.25rem}article ul,article ul li{margin-bottom:1rem;margin-top:1rem}article ul li{padding-left:.25rem}@media print{article ul li{margin-bottom:0;margin-top:0}}article ul li::marker{--tw-text-opacity:1;color:#616161;color:rgb(97 97 97/var(--tw-text-opacity))}article ul li p{margin-bottom:.5rem;margin-top:.5rem}article dt{font-weight:500;margin-bottom:1rem;margin-top:1rem}article dd{padding-left:1.25rem}article dd p{margin-bottom:1rem;margin-top:1rem}*,:after,:before{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:rgba(14,165,233,.5);--tw-ring-offset-shadow:0 0 transparent;--tw-ring-shadow:0 0 transparent;--tw-shadow:0 0 transparent;--tw-shadow-colored:0 0 transparent;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: }::backdrop{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:rgba(14,165,233,.5);--tw-ring-offset-shadow:0 0 transparent;--tw-ring-shadow:0 0 transparent;--tw-shadow:0 0 transparent;--tw-shadow-colored:0 0 transparent;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: }.container{width:100%}@media (min-width:400px){.container{max-width:400px}}@media (min-width:640px){.container{max-width:640px}}@media (min-width:768px){.container{max-width:768px}}@media (min-width:1024px){.container{max-width:1024px}}@media (min-width:1280px){.container{max-width:1280px}}@media (min-width:1536px){.container{max-width:1536px}}:root{--sidebar-width:300px;--fluid-margin:7.5vw;--color-brand:#0ea5e9;--color-link:#0369a1}.contents.local{border-bottom-width:1px;display:block;margin-top:3rem;padding-bottom:3rem}@media print{.contents.local{display:none}}.contents.local .topic-title{--tw-text-opacity:1;color:#616161;color:rgb(97 97 97/var(--tw-text-opacity));font-family:JetBrains\ Mono,monospace;font-size:.875rem;font-weight:500;line-height:1.5;margin-bottom:.5rem;margin-top:0;text-transform:uppercase}.contents.local ul{list-style-type:none;margin-bottom:0;margin-top:0;padding-left:0;padding-top:.5rem}.contents.local ul ul{margin-left:1rem}.contents.local li{padding-bottom:.5rem;padding-left:0;padding-top:.5rem}.contents.local li,.contents.local li p{margin-bottom:0;margin-top:0}.contents.local a{--tw-text-opacity:1;color:#616161;color:rgb(97 97 97/var(--tw-text-opacity));display:block}.contents.local a:focus,.contents.local a:hover{--tw-text-opacity:1;color:#212121;color:rgb(33 33 33/var(--tw-text-opacity))}.nav-toc .caption{--tw-text-opacity:1;color:#424242;color:rgb(66 66 66/var(--tw-text-opacity));font-size:1.125rem;font-weight:500;letter-spacing:.025em;line-height:1.5;padding-bottom:.75rem;padding-top:2.5rem}.nav-toc p:first-of-type,.nav-toc>ul:first-child{padding-top:1rem}.nav-toc .expand{fill:currentColor;cursor:pointer;display:inline;height:1.2rem;margin-left:-.4rem;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transition-duration:.15s;transition-property:transform;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-timing-function:cubic-bezier(0,0,.2,1);-webkit-user-select:none;-moz-user-select:none;user-select:none}.nav-toc .expand:focus,.nav-toc .expand:hover{color:#0ea5e9;color:var(--color-brand)}.nav-toc li>ul{max-height:0;overflow-y:hidden;padding-left:1rem}.nav-toc .expanded>div>.expand{--tw-rotate:90deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(90deg) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.nav-toc .expanded>ul{max-height:100%}.nav-toc .expanded>ul a.current{color:#0ea5e9;color:var(--color-brand)}.nav-toc a{--tw-text-opacity:1;color:#616161;color:rgb(97 97 97/var(--tw-text-opacity));display:inline-block;padding-bottom:.25rem;padding-top:.25rem}.nav-toc a:focus,.nav-toc a:hover{color:#0ea5e9;color:var(--color-brand)}.nav-toc a.current{--tw-text-opacity:1;color:#212121;color:rgb(33 33 33/var(--tw-text-opacity));font-weight:500}.nav-toc ul+ul{margin-top:2rem}.toctree-wrapper .caption{--tw-text-opacity:1;color:#616161;color:rgb(97 97 97/var(--tw-text-opacity));font-family:JetBrains\ Mono,monospace;font-size:.875rem;font-weight:500;line-height:1.5;padding-bottom:1.5rem;text-transform:uppercase}.toctree-wrapper{border-top-width:1px;margin-bottom:3rem;margin-top:3rem;padding-top:3rem}.toctree-wrapper li li{padding-left:1rem}.toctree-wrapper a{color:#0369a1;color:var(--color-link);display:block;padding-bottom:.25rem;padding-top:.25rem}.toctree-wrapper a:focus,.toctree-wrapper a:hover{color:#0ea5e9;color:var(--color-brand)}.nav-link{font-size:.95rem;letter-spacing:.2px}.headerlink{font-size:1em;line-height:1.2em;margin-left:.25rem;vertical-align:middle}.headerlink:focus,.headerlink:hover{color:#0ea5e9;color:var(--color-brand)}.headerlink>*{fill:currentColor;height:1em;visibility:hidden}.headerlink:focus>*{visibility:visible}h1 .headerlink,h2 .headerlink,h3 .headerlink{--tw-text-opacity:1;color:#9ca3af;color:rgb(156 163 175/var(--tw-text-opacity))}h1 .headerlink:focus,h1 .headerlink:hover,h2 .headerlink:focus,h2 .headerlink:hover,h3 .headerlink:focus,h3 .headerlink:hover{color:#0ea5e9;color:var(--color-brand)}h1 .headerlink{font-size:.65em;line-height:1.2}h2 .headerlink{font-size:.75em;line-height:1.2}.code-header .headerlink{margin-right:.5rem}.admonition-title:hover .headerlink,.admonition-title:hover .headerlink>*,.code-header:hover .headerlink,.code-header:hover .headerlink>*,dt:not(.does-not-exist):hover .headerlink,dt:not(.does-not-exist):hover .headerlink>*,figure:not(.does-not-exist):hover .headerlink,figure:not(.does-not-exist):hover .headerlink>*,h1:not(.does-not-exist):hover .headerlink,h1:not(.does-not-exist):hover .headerlink>*,h2:not(.does-not-exist):hover .headerlink,h2:not(.does-not-exist):hover .headerlink>*,h3:not(.does-not-exist):hover .headerlink,h3:not(.does-not-exist):hover .headerlink>*,h4:not(.does-not-exist):hover .headerlink,h4:not(.does-not-exist):hover .headerlink>*,table:not(.does-not-exist):hover .headerlink,table:not(.does-not-exist):hover .headerlink>*{visibility:visible}.search a,p:not(.admonition-title) a{color:#0369a1;color:var(--color-link)}.search a:focus,.search a:hover,p:not(.admonition-title) a:focus,p:not(.admonition-title) a:hover{color:#0ea5e9;color:var(--color-brand)}ul.search{list-style-type:none;padding-left:0}.search li{border-top-width:1px;margin-bottom:1rem;margin-top:1rem;padding-bottom:1rem;padding-left:0;padding-top:1rem}.search li a{font-size:1.375rem;line-height:1.2}.search .context{--tw-text-opacity:1;color:#1f2937;color:rgb(31 41 55/var(--tw-text-opacity));font-size:.875rem;line-height:1.5}.highlighted{--tw-bg-opacity:1;background-color:#fef9c3;background-color:rgb(254 249 195/var(--tw-bg-opacity));font-weight:500;padding-bottom:1px;padding-top:1px}.highlight-link{display:none}article p a:focus,article p a:hover{text-decoration-line:underline}.footnote-reference{font-size:.75rem;line-height:1.5;vertical-align:super}.external-link-icon{fill:currentColor;height:.875rem;margin-bottom:2px;margin-left:1px}.viewcode-link{color:#0369a1;color:var(--color-link);margin-left:1rem}.viewcode-link:focus,.viewcode-link:hover{color:#0ea5e9;color:var(--color-brand)}.viewcode-back{color:#0369a1;color:var(--color-link);position:absolute;right:1rem}.viewcode-back:focus,.viewcode-back:hover{color:#0ea5e9;color:var(--color-brand)}:not(pre)>code{--tw-bg-opacity:1;background-color:#f9fafb;background-color:rgb(249 250 251/var(--tw-bg-opacity));border-width:1px;font-weight:500;padding-left:.25rem;padding-right:.25rem}@media (min-width:640px){:not(pre)>code{font-size:.9375em;line-height:1.5}}:not(pre)>code.highlight{--tw-bg-opacity:1;background-color:#f9fafb;background-color:rgb(249 250 251/var(--tw-bg-opacity))}main kbd:not(.compound){--tw-border-opacity:1;border-color:#212121;border-color:rgb(33 33 33/var(--tw-border-opacity));border-radius:.125rem;border-width:1px;display:inline-block;font-size:.75rem;font-weight:500;line-height:1.5;padding:.25rem}pre{border-radius:.125rem;border-width:1px;line-height:1.5;margin-bottom:1.5rem;overflow-x:hidden;position:relative}pre code,pre.literal-block{overflow-x:auto;padding-bottom:1rem;padding-left:1rem;padding-top:1rem}pre code{display:block}pre .copy{--tw-bg-opacity:1;--tw-text-opacity:1;background-color:#fff;background-color:rgb(255 255 255/var(--tw-bg-opacity));border-radius:.125rem;border-width:1px;color:#374151;color:rgb(55 65 81/var(--tw-text-opacity));font-size:.75rem;letter-spacing:.025em;line-height:1.5;opacity:0;padding:.25rem;position:absolute;right:.375rem;text-transform:uppercase;top:.75rem;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transition-duration:.5s;transition-property:all;transition-timing-function:cubic-bezier(.4,0,.2,1);-webkit-user-select:none;-moz-user-select:none;user-select:none}pre .copy:focus{opacity:1}pre .copy:active{--tw-translate-x:0.125rem;--tw-translate-y:0.125rem;transform:translate(.125rem,.125rem) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}pre:hover .copy{opacity:1}.code-wrapper{margin-bottom:1.5rem;margin-top:1.5rem}.code-wrapper .caption-text{--tw-text-opacity:1;color:#616161;color:rgb(97 97 97/var(--tw-text-opacity));letter-spacing:.025em}.code-wrapper pre{border-top-left-radius:0;border-top-right-radius:0}.code-wrapper del,.code-wrapper ins,.code-wrapper mark{display:block;margin-left:-1rem;padding-bottom:1px;padding-left:1rem;padding-top:1px;position:relative}.code-wrapper mark{background-color:rgba(186,230,253,.7)}.code-wrapper ins{background-color:rgba(187,247,208,.7);text-decoration-line:none}.code-wrapper ins:before{--tw-text-opacity:1;color:#14532d;color:rgb(20 83 45/var(--tw-text-opacity));content:"\002b";left:2px;position:absolute}.code-wrapper del{background-color:hsla(0,96%,89%,.7);text-decoration-line:none}.code-wrapper del:before{--tw-text-opacity:1;color:#7f1d1d;color:rgb(127 29 29/var(--tw-text-opacity));content:"\2212";left:2px;position:absolute}.code-wrapper .linenos{--tw-text-opacity:1;background-color:transparent;color:#374151;color:rgb(55 65 81/var(--tw-text-opacity));padding:0 1.5rem 0 0;-webkit-user-select:none;-moz-user-select:none;user-select:none}.code-wrapper .code-line{display:block}span.gd{background-color:#fecaca;background-color:rgb(254 202 202/var(--tw-bg-opacity))}span.gd,span.gi{--tw-bg-opacity:1;display:inline-block;padding-bottom:1px;padding-top:1px;width:100%}span.gi{background-color:#bbf7d0;background-color:rgb(187 247 208/var(--tw-bg-opacity))}.code-header{--tw-bg-opacity:1;align-items:center;background-color:#f9fafb;background-color:rgb(249 250 251/var(--tw-bg-opacity));border-left-width:1px;border-right-width:1px;border-top-left-radius:.125rem;border-top-right-radius:.125rem;border-top-width:1px;display:flex;font-size:.875rem;justify-content:space-between;line-height:1.5;padding-bottom:.25rem;padding-top:.25rem}.code-lang{--tw-text-opacity:1;color:#212121;color:rgb(33 33 33/var(--tw-text-opacity));display:inline-block;font-family:JetBrains\ Mono,monospace;letter-spacing:.05em;margin-left:.5rem;margin-right:auto;text-transform:uppercase}.gp{font-weight:500;pointer-events:none;-webkit-user-select:none;-moz-user-select:none;user-select:none}var{--tw-text-opacity:1;color:#6b21a8;color:rgb(107 33 168/var(--tw-text-opacity));font-style:italic}.guilabel,.menuselection{--tw-text-opacity:1;color:#212121;color:rgb(33 33 33/var(--tw-text-opacity));font-weight:500;letter-spacing:.025em}dl.code-definition,dl.option-list{border-top-width:1px;margin-bottom:3rem;margin-top:1.5rem;padding-top:1.5rem}dl.code-definition dt,dl.option-list dt{font-weight:400}dl.code-definition dt>code,dl.code-definition dt>kbd,dl.option-list dt>code,dl.option-list dt>kbd{--tw-text-opacity:1;background-color:transparent;border-style:none;color:#212121;color:rgb(33 33 33/var(--tw-text-opacity));font-size:16px;font-weight:600;line-height:1.5;padding-left:0;padding-right:0}dl.code-definition .property,dl.option-list .property{--tw-text-opacity:1;color:#616161;color:rgb(97 97 97/var(--tw-text-opacity));font-family:JetBrains\ Mono,monospace;font-weight:500}dl.code-definition .sig-param,dl.option-list .sig-param{--tw-text-opacity:1;color:#0c4a6e;color:rgb(12 74 110/var(--tw-text-opacity));font-family:JetBrains\ Mono,monospace}dl.code-definition .sig-paren,dl.option-list .sig-paren{margin-left:.25rem;margin-right:.25rem}dl.footnote{display:grid;font-size:.875rem;grid-template-columns:max-content auto;line-height:1.5}dl.footnote dt{color:#0369a1;color:var(--color-link)}dl.footnote span.brackets:before{content:"["}dl.footnote span.brackets:after{content:"]"}table caption{--tw-text-opacity:1;color:#616161;color:rgb(97 97 97/var(--tw-text-opacity));font-size:.875rem;letter-spacing:.025em;line-height:1.5;margin-bottom:1rem;text-align:left}table:not(.highlighttable){font-size:.875rem;line-height:1.5;margin-bottom:3rem;margin-top:3rem}table:not(.highlighttable) p+p{margin-top:1rem}table:not(.highlighttable) tbody tr{border-top-width:1px}table:not(.highlighttable) th{font-weight:500;letter-spacing:.025em;padding-bottom:.75rem;padding-top:.75rem;text-align:left;vertical-align:top}table:not(.highlighttable) td{padding-bottom:.5rem;padding-top:.5rem;text-align:left;vertical-align:top}.caption-number{--tw-text-opacity:1;color:#616161;color:rgb(97 97 97/var(--tw-text-opacity));font-size:.875rem;font-weight:500;line-height:1.5}figure{margin-bottom:3rem;margin-top:3rem}figure .legend{--tw-text-opacity:1;border-bottom-width:1px;color:#616161;color:rgb(97 97 97/var(--tw-text-opacity));font-size:.875rem;line-height:1.5;padding-bottom:2rem}figure .legend p{margin-bottom:1rem;margin-top:1rem}figure img{display:inline-block}main :not(figure)>img{margin-bottom:3rem;margin-top:3rem}figcaption{--tw-text-opacity:1;color:#616161;color:rgb(97 97 97/var(--tw-text-opacity));font-size:.875rem;letter-spacing:.025em;line-height:1.25;margin-top:1rem}.align-center{margin-left:auto;margin-right:auto;text-align:center}.align-right{margin-left:auto;text-align:right}blockquote{--tw-shadow:0 1px 3px 0 rgba(0,0,0,.1),0 1px 2px -1px rgba(0,0,0,.1);--tw-shadow-colored:0 1px 3px 0 var(--tw-shadow-color),0 1px 2px -1px var(--tw-shadow-color);background-color:rgba(249,250,251,.3);border-left-width:4px;border-radius:.125rem;box-shadow:0 0 transparent,0 0 transparent,0 1px 3px 0 rgba(0,0,0,.1),0 1px 2px -1px rgba(0,0,0,.1);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow);font-size:.875rem;line-height:1.5;margin-bottom:1.5rem;margin-top:1.5rem;padding:1rem}blockquote .attribution{font-style:italic}.admonition{--tw-border-opacity:1;--tw-bg-opacity:0.02;--tw-text-opacity:1;--tw-shadow:0 1px 3px 0 rgba(0,0,0,.1),0 1px 2px -1px rgba(0,0,0,.1);--tw-shadow-colored:0 1px 3px 0 var(--tw-shadow-color),0 1px 2px -1px var(--tw-shadow-color);background-color:rgba(56,189,248,.02);background-color:rgb(56 189 248/var(--tw-bg-opacity));border-color:#38bdf8;border-color:rgb(56 189 248/var(--tw-border-opacity));border-left-width:4px;border-radius:.125rem;box-shadow:0 0 transparent,0 0 transparent,0 1px 3px 0 rgba(0,0,0,.1),0 1px 2px -1px rgba(0,0,0,.1);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow);color:#0c4a6e;color:rgb(12 74 110/var(--tw-text-opacity));font-size:.875rem;line-height:1.5;margin-bottom:1.5rem;margin-top:1.5rem;padding:1rem}.admonition p:not(.admonition-title){margin-bottom:1rem;margin-top:1rem}.admonition p:last-child{margin-bottom:0}.admonition .headerlink{color:currentColor}.seealso{--tw-text-opacity:1;background-color:transparent;border-style:none;color:#616161;color:rgb(97 97 97/var(--tw-text-opacity));padding:.5rem}.seealso .admonition-title{padding-left:.5rem;padding-right:.5rem}.seealso a{background-color:rgba(249,250,251,.4);display:inline-block;padding:.5rem;transition-duration:.15s;transition-property:all;transition-timing-function:cubic-bezier(.4,0,.2,1)}.seealso a.internal:after{content:"\2192";margin-left:.5rem;opacity:0;transition-duration:.15s}.seealso a:hover{background-color:#0ea5e9;background-color:var(--color-brand);color:#fff!important;-webkit-text-decoration:none!important;text-decoration:none!important}.seealso a:hover:after{opacity:1}.seealso a code{background-color:transparent;border-style:none}.hint,.tip{background-color:rgba(74,222,128,.02);background-color:rgb(74 222 128/var(--tw-bg-opacity));border-color:#4ade80;border-color:rgb(74 222 128/var(--tw-border-opacity));color:#14532d;color:rgb(20 83 45/var(--tw-text-opacity))}.danger,.error,.hint,.tip,.warning{--tw-border-opacity:1;--tw-bg-opacity:0.02;--tw-text-opacity:1}.danger,.error,.warning{background-color:hsla(0,91%,71%,.02);background-color:rgb(248 113 113/var(--tw-bg-opacity));border-color:#f87171;border-color:rgb(248 113 113/var(--tw-border-opacity));color:#7f1d1d;color:rgb(127 29 29/var(--tw-text-opacity))}.caution,.important{--tw-border-opacity:1;--tw-bg-opacity:0.02;--tw-text-opacity:1;background-color:rgba(250,204,21,.02);background-color:rgb(250 204 21/var(--tw-bg-opacity));border-color:#facc15;border-color:rgb(250 204 21/var(--tw-border-opacity));color:#713f12;color:rgb(113 63 18/var(--tw-text-opacity))}.admonition-title{font-weight:500;letter-spacing:.025em;margin-bottom:1rem;margin-top:0}@media print{p{orphans:2;widows:2}h2,h3,h4{-moz-column-break-after:avoid;break-after:avoid;page-break-after:avoid}a,h2,h3,h4{-moz-column-break-inside:avoid;break-inside:avoid;page-break-inside:avoid}section[role=contentinfo]{-moz-column-break-before:avoid;break-before:avoid;page-break-before:avoid}table{-moz-column-break-inside:avoid;break-inside:avoid;page-break-inside:avoid}code,pre{white-space:pre-wrap!important}.seealso a.internal:after,main a:after{content:" (" attr(href) ")"}}.tooltipped{position:relative}.tooltipped:after{-webkit-font-smoothing:subpixel-antialiased;word-wrap:break-word;--tw-bg-opacity:0.75;--tw-text-opacity:1;background-color:rgba(31,41,55,.75);background-color:rgb(31 41 55/var(--tw-bg-opacity));border-radius:.125rem;color:#fff;color:rgb(255 255 255/var(--tw-text-opacity));content:attr(aria-label);display:none;font-size:.75rem;font-weight:400;letter-spacing:normal;letter-spacing:.025em;line-height:1.5;opacity:0;padding:.25rem .5rem;pointer-events:none;position:absolute;text-align:center;text-decoration-line:none;text-shadow:none;text-transform:none;white-space:pre;z-index:1000000}@keyframes tooltip-appear{0%{opacity:0}to{opacity:1}}.tooltipped:focus:after,.tooltipped:focus:before,.tooltipped:hover:after,.tooltipped:hover:before{animation-delay:.2s;animation-duration:.4s;animation-fill-mode:forwards;animation-name:tooltip-appear;animation-timing-function:ease-in;display:inline-block;-webkit-text-decoration:none;text-decoration:none}.tooltipped-no-delay:focus:after,.tooltipped-no-delay:focus:before,.tooltipped-no-delay:hover:after,.tooltipped-no-delay:hover:before{animation-delay:0s}.tooltipped-multiline:focus:after,.tooltipped-multiline:hover:after{display:table-cell}.tooltipped-s:after,.tooltipped-se:after,.tooltipped-sw:after{margin-top:6px;right:50%;top:100%}.tooltipped-s:before,.tooltipped-se:before,.tooltipped-sw:before{border-bottom-color:#1a202c;bottom:-7px;margin-right:-6px;right:50%;top:auto}.tooltipped-se:after{left:50%;margin-left:-16px;right:auto}.tooltipped-sw:after{margin-right:-16px}.tooltipped-n:after,.tooltipped-ne:after,.tooltipped-nw:after{bottom:100%;margin-bottom:6px;right:50%}.tooltipped-n:before,.tooltipped-ne:before,.tooltipped-nw:before{border-top-color:#1a202c;bottom:auto;margin-right:-6px;right:50%;top:-7px}.tooltipped-ne:after{left:50%;margin-left:-16px;right:auto}.tooltipped-nw:after{margin-right:-16px}.tooltipped-n:after,.tooltipped-s:after{transform:translateX(50%)}.tooltipped-w:after{bottom:50%;margin-right:6px;right:100%;transform:translateY(50%)}.tooltipped-w:before{border-left-color:#1a202c;bottom:50%;left:-7px;margin-top:-6px;top:50%}.tooltipped-e:after{bottom:50%;left:100%;margin-left:6px;transform:translateY(50%)}.tooltipped-e:before{border-right-color:#1a202c;bottom:50%;margin-top:-6px;right:-7px;top:50%}.tooltipped-align-right-1:after,.tooltipped-align-right-2:after{margin-right:0;right:0}.tooltipped-align-right-1:before{right:10px}.tooltipped-align-right-2:before{right:15px}.tooltipped-align-left-1:after,.tooltipped-align-left-2:after{left:0;margin-left:0}.tooltipped-align-left-1:before{left:5px}.tooltipped-align-left-2:before{left:10px}.tooltipped-multiline:after{word-wrap:break-word;border-collapse:separate;max-width:250px;white-space:pre-line;width:-moz-max-content;width:max-content}.tooltipped-multiline.tooltipped-n:after,.tooltipped-multiline.tooltipped-s:after{left:50%;right:auto;transform:translateX(-50%)}.tooltipped-multiline.tooltipped-e:after,.tooltipped-multiline.tooltipped-w:after{right:100%}@media screen and (min-width:0\0){.tooltipped-multiline:after{width:250px}}.tooltipped-sticky:after,.tooltipped-sticky:before{display:inline-block}.tooltipped-sticky.tooltipped-multiline:after{display:table-cell}button.expand-more{--tw-text-opacity:1;color:#4b5563;color:rgb(75 85 99/var(--tw-text-opacity));float:right;margin-left:.5rem}button.expand-more:focus,button.expand-more:hover{color:#0ea5e9;color:var(--color-brand)}button.expand-more>svg{--tw-rotate:0deg;fill:currentColor;height:1.5rem;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(0deg) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transition-duration:.1s;transition-property:transform;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-timing-function:cubic-bezier(0,0,.2,1);width:1.5rem}.accordion:hover .expand-more{color:#0ea5e9;color:var(--color-brand)}.active .expand-more>svg{--tw-rotate:180deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(180deg) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.panel{max-height:0;opacity:0;overflow-y:hidden;transition-duration:.5s;transition-property:opacity;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-timing-function:cubic-bezier(0,0,.2,1);visibility:hidden}.active+.panel{max-height:-moz-fit-content;max-height:fit-content;opacity:1;overflow-y:visible;visibility:visible}:root{--docsearch-searchbox-background:transparent;--docsearch-searchbox-shadow:inset 0 0 0 2px var(--color-brand);--docsearch-key-gradient:transparent;--docsearch-primary-color:#1c75b0;--docsearch-modal-width:960px}.DocSearch-Button{border-radius:0;height:3.5rem;line-height:3.5rem;padding-right:1rem}.DocSearch-Button-Key{font-family:Roboto,sans-serif;font-size:.875rem;height:1.25rem;line-height:1.5;padding:1rem}.DocSearch-Button:hover .DocSearch-Button-Key{--tw-border-opacity:1;--tw-text-opacity:1;border-color:#212121;border-color:rgb(33 33 33/var(--tw-border-opacity));color:#212121;color:rgb(33 33 33/var(--tw-text-opacity))}.DocSearch-Button .DocSearch-Search-Icon{--tw-text-opacity:1;stroke-width:2.5;color:#f3f4f6;color:rgb(243 244 246/var(--tw-text-opacity))}.DocSearch-Button:hover .DocSearch-Search-Icon{color:var(--docsearch-text-color)}.DocSearch-Button-Placeholder{padding-left:.75rem}.sr-only{clip:rect(0,0,0,0);border-width:0;height:1px;margin:-1px;overflow:hidden;padding:0;position:absolute;white-space:nowrap;width:1px}.pointer-events-none{pointer-events:none}.visible{visibility:visible}.collapse{visibility:collapse}.static{position:static}.fixed{position:fixed}.absolute{position:absolute}.relative{position:relative}.sticky{position:sticky}.inset-0{left:0;right:0}.inset-0,.inset-y-0{bottom:0;top:0}.bottom-0{bottom:0}.left-0{left:0}.right-0{right:0}.top-0{top:0}.z-10{z-index:10}.z-20{z-index:20}.col-span-full{grid-column:1/-1}.m-4{margin:1rem}.mx-0{margin-left:0;margin-right:0}.mx-5{margin-left:1.25rem;margin-right:1.25rem}.mx-auto{margin-left:auto;margin-right:auto}.my-8{margin-bottom:2rem;margin-top:2rem}.mb-2{margin-bottom:.5rem}.mb-4{margin-bottom:1rem}.ml-auto{margin-left:auto}.mr-1{margin-right:.25rem}.mr-auto{margin-right:auto}.mt-12{margin-top:3rem}.mt-16{margin-top:4rem}.mt-20{margin-top:5rem}.block{display:block}.inline-block{display:inline-block}.flex{display:flex}.hidden{display:none}.h-14{height:3.5rem}.h-6{height:1.5rem}.h-8{height:2rem}.h-full{height:100%}.min-h-screen{min-height:100vh}.w-0{width:0}.w-14{width:3.5rem}.w-6{width:1.5rem}.w-8{width:2rem}.w-full{width:100%}.max-w-prose{max-width:760px}.flex-1{flex:1 1 0%}.shrink-0{flex-shrink:0}.-translate-x-full{--tw-translate-x:-100%;transform:translate(-100%,var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.translate-y-full{--tw-translate-y:100%;transform:translate(var(--tw-translate-x),100%) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.transform,.translate-y-full{transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.transform-gpu{transform:translate3d(var(--tw-translate-x),var(--tw-translate-y),0) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.flex-col{flex-direction:column}.items-center{align-items:center}.justify-end{justify-content:flex-end}.justify-center{justify-content:center}.justify-between{justify-content:space-between}.self-center{align-self:center}.overflow-y-auto{overflow-y:auto}.scroll-smooth{scroll-behavior:smooth}.rounded-full{border-radius:9999px}.border-b-4{border-bottom-width:4px}.border-brand{border-color:#0ea5e9;border-color:var(--color-brand)}.bg-black{--tw-bg-opacity:1;background-color:#000;background-color:rgb(0 0 0/var(--tw-bg-opacity))}.bg-gray-700{--tw-bg-opacity:1;background-color:#374151;background-color:rgb(55 65 81/var(--tw-bg-opacity))}.bg-gray-900{--tw-bg-opacity:1;background-color:#111827;background-color:rgb(17 24 39/var(--tw-bg-opacity))}.bg-gray-dark{--tw-bg-opacity:1;background-color:#212121;background-color:rgb(33 33 33/var(--tw-bg-opacity))}.bg-transparent{background-color:transparent}.bg-white{--tw-bg-opacity:1;background-color:#fff;background-color:rgb(255 255 255/var(--tw-bg-opacity))}.bg-opacity-50{--tw-bg-opacity:0.5}.fill-current{fill:currentColor}.stroke-current{stroke:currentColor}.p-2{padding:.5rem}.p-3{padding:.75rem}.p-4{padding:1rem}.px-2{padding-left:.5rem;padding-right:.5rem}.px-4{padding-left:1rem;padding-right:1rem}.pl-2{padding-left:.5rem}.pl-6{padding-left:1.5rem}.pr-2{padding-right:.5rem}.pr-4{padding-right:1rem}.pt-14{padding-top:3.5rem}.pt-4{padding-top:1rem}.pt-8{padding-top:2rem}.text-right{text-align:right}.text-3xl{font-size:2.5rem;line-height:1.2}.text-4xl{font-size:3rem;line-height:1.2}.text-sm{font-size:.875rem;line-height:1.5}.text-xl{font-size:1.5rem;line-height:1.2}.text-xs{font-size:.75rem;line-height:1.5}.font-medium{font-weight:500}.uppercase{text-transform:uppercase}.leading-14{line-height:3.5rem}.tracking-wide{letter-spacing:.025em}.tracking-wider{letter-spacing:.05em}.text-gray{--tw-text-opacity:1;color:#424242;color:rgb(66 66 66/var(--tw-text-opacity))}.text-gray-100{--tw-text-opacity:1;color:#f3f4f6;color:rgb(243 244 246/var(--tw-text-opacity))}.text-gray-300{--tw-text-opacity:1;color:#d1d5db;color:rgb(209 213 219/var(--tw-text-opacity))}.text-gray-600{--tw-text-opacity:1;color:#4b5563;color:rgb(75 85 99/var(--tw-text-opacity))}.text-gray-700{--tw-text-opacity:1;color:#374151;color:rgb(55 65 81/var(--tw-text-opacity))}.text-gray-800{--tw-text-opacity:1;color:#1f2937;color:rgb(31 41 55/var(--tw-text-opacity))}.text-gray-light{--tw-text-opacity:1;color:#616161;color:rgb(97 97 97/var(--tw-text-opacity))}.text-inherit{color:inherit}.text-link{color:#0369a1;color:var(--color-link)}.text-red-700{--tw-text-opacity:1;color:#b91c1c;color:rgb(185 28 28/var(--tw-text-opacity))}.text-white{--tw-text-opacity:1;color:#fff;color:rgb(255 255 255/var(--tw-text-opacity))}.antialiased{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale}.opacity-0{opacity:0}.shadow-md{--tw-shadow:0 4px 6px -1px rgba(0,0,0,.1),0 2px 4px -2px rgba(0,0,0,.1);--tw-shadow-colored:0 4px 6px -1px var(--tw-shadow-color),0 2px 4px -2px var(--tw-shadow-color);box-shadow:0 0 transparent,0 0 transparent,0 4px 6px -1px rgba(0,0,0,.1),0 2px 4px -2px rgba(0,0,0,.1);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow)}.blur{--tw-blur:blur(8px);filter:blur(8px) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) var(--tw-invert) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow);filter:var(--tw-blur) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) var(--tw-invert) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow)}.transition{transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,-webkit-backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter,-webkit-backdrop-filter;transition-timing-function:cubic-bezier(.4,0,.2,1)}.transition-all{transition-duration:.15s;transition-property:all;transition-timing-function:cubic-bezier(.4,0,.2,1)}.transition-opacity{transition-duration:.15s;transition-property:opacity;transition-timing-function:cubic-bezier(.4,0,.2,1)}.duration-100{transition-duration:.1s}.duration-1000{transition-duration:1s}.duration-300{transition-duration:.3s}.duration-500{transition-duration:.5s}.lead{--tw-text-opacity:1;color:#212121;color:rgb(33 33 33/var(--tw-text-opacity));font-size:1.125rem;line-height:1.5;margin-bottom:4rem;margin-top:1rem}.centered{text-align:center}p.rubric{--tw-text-opacity:1;color:#212121;color:rgb(33 33 33/var(--tw-text-opacity));font-weight:500;margin-bottom:0;margin-top:3rem}.grid-area-header{grid-area:header}.grid-area-sidebar{grid-area:sidebar}.grid-area-main{grid-area:main}#page.isShown{overflow:hidden}[data-sidebar-target=sidebar].isShown{--tw-translate-x:0px;max-width:90%;opacity:1;transform:translateY(var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));width:100%}[data-scroll-target=scrollToTop].isShown{opacity:1;pointer-events:auto}[data-sidebar-target=screen].isShown{display:block}[data-search-target=snackbar].isShown{--tw-translate-y:0px;opacity:1;transform:translate(var(--tw-translate-x)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transition-duration:.5s;transition-timing-function:cubic-bezier(0,0,.2,1)}.focus-within\:absolute:focus-within{position:absolute}.focus-within\:inset-x-0:focus-within{left:0;right:0}.focus-within\:top-0:focus-within{top:0}.focus-within\:bg-gray-50:focus-within{--tw-bg-opacity:1;background-color:#f9fafb;background-color:rgb(249 250 251/var(--tw-bg-opacity))}.focus-within\:text-gray-800:focus-within{--tw-text-opacity:1;color:#1f2937;color:rgb(31 41 55/var(--tw-text-opacity))}.hover\:bg-gray-300:hover{--tw-bg-opacity:1;background-color:#d1d5db;background-color:rgb(209 213 219/var(--tw-bg-opacity))}.hover\:bg-gray-700:hover{--tw-bg-opacity:1;background-color:#374151;background-color:rgb(55 65 81/var(--tw-bg-opacity))}.hover\:text-brand:hover{color:#0ea5e9;color:var(--color-brand)}.hover\:text-gray-dark:hover{--tw-text-opacity:1;color:#212121;color:rgb(33 33 33/var(--tw-text-opacity))}.hover\:text-link:hover{color:#0369a1;color:var(--color-link)}.hover\:underline:hover{text-decoration-line:underline}.hover\:no-underline:hover{text-decoration-line:none}.focus\:w-full:focus{width:100%}.focus\:translate-x-0:focus{--tw-translate-x:0px;transform:translateY(var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.focus\:bg-gray-200:focus{--tw-bg-opacity:1;background-color:#e5e7eb;background-color:rgb(229 231 235/var(--tw-bg-opacity))}.focus\:bg-gray-700:focus{--tw-bg-opacity:1;background-color:#374151;background-color:rgb(55 65 81/var(--tw-bg-opacity))}.focus\:text-brand:focus{color:#0ea5e9;color:var(--color-brand)}.focus\:text-gray-dark:focus{--tw-text-opacity:1;color:#212121;color:rgb(33 33 33/var(--tw-text-opacity))}.focus\:text-link:focus{color:#0369a1;color:var(--color-link)}.focus\:underline:focus{text-decoration-line:underline}.focus\:opacity-100:focus{opacity:1}.focus\:outline-none:focus{outline:2px solid transparent;outline-offset:2px}.focus\:ring-2:focus{--tw-ring-offset-shadow:var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow:var(--tw-ring-inset) 0 0 0 calc(2px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color),var(--tw-ring-inset) 0 0 0 calc(2px + var(--tw-ring-offset-width)) var(--tw-ring-color),0 0 transparent;box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow,0 0 #0000)}.focus\:ring-blue-600:focus{--tw-ring-opacity:1;--tw-ring-color:rgba(2,132,199,var(--tw-ring-opacity))}@media (min-width:640px){.sm\:px-4{padding-left:1rem;padding-right:1rem}}@media (min-width:768px){.md\:mx-auto{margin-left:auto;margin-right:auto}.md\:ml-4{margin-left:1rem}.md\:w-auto{width:auto}.md\:focus-within\:static:focus-within{position:static}.md\:focus-within\:w-full:focus-within{width:100%}}@media (min-width:1024px){.lg\:inline-block{display:inline-block}}@media (min-width:1280px){.xl\:relative{position:relative}.xl\:z-0{z-index:0}.xl\:ml-fluid{margin-left:7.5vw;margin-left:var(--fluid-margin)}.xl\:mr-0{margin-right:0}.xl\:grid{display:grid}.xl\:hidden{display:none}.xl\:h-screen{height:100vh}.xl\:translate-x-0{--tw-translate-x:0px;transform:translateY(var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.xl\:px-2{padding-left:.5rem;padding-right:.5rem}.xl\:opacity-100{opacity:1}.xl\:grid-layout{grid-template-areas:"header header" "sidebar main";grid-template-columns:max(300px,17%) 1fr;grid-template-columns:max(var(--sidebar-width),17%) 1fr;grid-template-rows:min-content 1fr}}@media print{.print\:mt-4{margin-top:1rem}.print\:block{display:block}.print\:hidden{display:none}.print\:h-auto{height:auto}}
+/*! tailwindcss v3.3.1 | MIT License | https://tailwindcss.com*/*,:after,:before{border:0 solid #e5e7eb;box-sizing:border-box}:after,:before{--tw-content:""}html{-webkit-text-size-adjust:100%;font-feature-settings:normal;font-family:Roboto,sans-serif;font-variation-settings:normal;line-height:1.5;-moz-tab-size:4;-o-tab-size:4;tab-size:4}body{line-height:inherit;margin:0}hr{border-top-width:1px;color:inherit;height:0}abbr:where([title]){text-decoration:underline;-webkit-text-decoration:underline dotted;text-decoration:underline dotted}h1,h2,h3,h4,h5,h6{font-size:inherit;font-weight:inherit}a{color:inherit;text-decoration:inherit}b,strong{font-weight:bolder}code,kbd,pre,samp{font-family:JetBrains\ Mono,monospace;font-size:1em}small{font-size:80%}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline}sub{bottom:-.25em}sup{top:-.5em}table{border-collapse:collapse;border-color:inherit;text-indent:0}button,input,optgroup,select,textarea{color:inherit;font-family:inherit;font-size:100%;font-weight:inherit;line-height:inherit;margin:0;padding:0}button,select{text-transform:none}[type=button],[type=reset],[type=submit],button{-webkit-appearance:button;background-color:transparent;background-image:none}:-moz-focusring{outline:auto}:-moz-ui-invalid{box-shadow:none}progress{vertical-align:baseline}::-webkit-inner-spin-button,::-webkit-outer-spin-button{height:auto}[type=search]{-webkit-appearance:textfield;outline-offset:-2px}::-webkit-search-decoration{-webkit-appearance:none}::-webkit-file-upload-button{-webkit-appearance:button;font:inherit}summary{display:list-item}blockquote,dd,dl,figure,h1,h2,h3,h4,h5,h6,hr,p,pre{margin:0}fieldset{margin:0}fieldset,legend{padding:0}menu,ol,ul{list-style:none;margin:0;padding:0}textarea{resize:vertical}input::-moz-placeholder,textarea::-moz-placeholder{color:#9ca3af;opacity:1}input::placeholder,textarea::placeholder{color:#9ca3af;opacity:1}[role=button],button{cursor:pointer}:disabled{cursor:default}audio,canvas,embed,iframe,img,object,svg,video{display:block;vertical-align:middle}img,video{height:auto;max-width:100%}[hidden]{display:none}button,input{-webkit-appearance:none;-moz-appearance:none;appearance:none;border-radius:0}main footer,main section{max-width:760px}section>section{padding-bottom:1.5rem;padding-top:1.5rem}@media print{section>section{padding-bottom:0;padding-top:0}}section>p{margin-bottom:1.5rem;margin-top:1.5rem}hr{border-top-width:1px;margin-bottom:3rem}strong{font-weight:500}svg{display:inline}h1{--tw-text-opacity:1;color:#212121;color:rgb(33 33 33/var(--tw-text-opacity));font-size:2.5rem;letter-spacing:-.025em;line-height:1.2;margin-top:5rem}@media print{h1{margin-top:0}}h2{--tw-text-opacity:1;color:#212121;color:rgb(33 33 33/var(--tw-text-opacity));font-size:1.5rem;letter-spacing:-.025em;line-height:1.2;line-height:1.5rem;margin-bottom:2rem}@media (min-width:640px){h2{font-size:1.75rem;line-height:1.2}}h3{font-size:1.375rem;line-height:1.2}h3,h4{--tw-text-opacity:1;color:#212121;color:rgb(33 33 33/var(--tw-text-opacity))}h4{font-weight:500}article ol{list-style-type:decimal}article ol,article ol ol{margin-bottom:1rem;margin-top:1rem;padding-left:1.25rem}article ol ol{list-style-type:lower-latin}article ol li{margin-bottom:1rem;margin-top:1rem;padding-left:.25rem}article ol li::marker{--tw-text-opacity:1;color:#212121;color:rgb(33 33 33/var(--tw-text-opacity));font-weight:500}article ol li p{margin-bottom:.5rem;margin-top:.5rem}article ul{list-style-type:disc;padding-left:1.25rem}article ul,article ul li{margin-bottom:1rem;margin-top:1rem}article ul li{padding-left:.25rem}@media print{article ul li{margin-bottom:0;margin-top:0}}article ul li::marker{--tw-text-opacity:1;color:#616161;color:rgb(97 97 97/var(--tw-text-opacity))}article ul li p{margin-bottom:.5rem;margin-top:.5rem}article dt{font-weight:500;margin-bottom:1rem;margin-top:1rem}article dd{padding-left:1.25rem}article dd p{margin-bottom:1rem;margin-top:1rem}*,:after,:before{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:rgba(14,165,233,.5);--tw-ring-offset-shadow:0 0 transparent;--tw-ring-shadow:0 0 transparent;--tw-shadow:0 0 transparent;--tw-shadow-colored:0 0 transparent;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: }::backdrop{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:rgba(14,165,233,.5);--tw-ring-offset-shadow:0 0 transparent;--tw-ring-shadow:0 0 transparent;--tw-shadow:0 0 transparent;--tw-shadow-colored:0 0 transparent;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: }.container{width:100%}@media (min-width:400px){.container{max-width:400px}}@media (min-width:640px){.container{max-width:640px}}@media (min-width:768px){.container{max-width:768px}}@media (min-width:1024px){.container{max-width:1024px}}@media (min-width:1280px){.container{max-width:1280px}}@media (min-width:1536px){.container{max-width:1536px}}:root{--sidebar-width:300px;--fluid-margin:7.5vw;--color-brand:#0ea5e9;--color-link:#0369a1}.contents.local{border-bottom-width:1px;display:block;margin-top:3rem;padding-bottom:3rem}@media print{.contents.local{display:none}}.contents.local .topic-title{--tw-text-opacity:1;color:#616161;color:rgb(97 97 97/var(--tw-text-opacity));font-family:JetBrains\ Mono,monospace;font-size:.875rem;font-weight:500;line-height:1.5;margin-bottom:.5rem;margin-top:0;text-transform:uppercase}.contents.local ul{list-style-type:none;margin-bottom:0;margin-top:0;padding-left:0;padding-top:.5rem}.contents.local ul ul{margin-left:1rem}.contents.local li{padding-bottom:.5rem;padding-left:0;padding-top:.5rem}.contents.local li,.contents.local li p{margin-bottom:0;margin-top:0}.contents.local a{--tw-text-opacity:1;color:#616161;color:rgb(97 97 97/var(--tw-text-opacity));display:block}.contents.local a:focus,.contents.local a:hover{--tw-text-opacity:1;color:#212121;color:rgb(33 33 33/var(--tw-text-opacity))}.nav-toc .caption{--tw-text-opacity:1;color:#424242;color:rgb(66 66 66/var(--tw-text-opacity));font-size:1.125rem;font-weight:500;letter-spacing:.025em;line-height:1.5;padding-bottom:.75rem;padding-top:2.5rem}.nav-toc p:first-of-type,.nav-toc>ul:first-child{padding-top:1rem}.nav-toc .expand{fill:currentColor;cursor:pointer;display:inline;height:1.2rem;margin-left:-.4rem;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transition-duration:.15s;transition-property:transform;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-timing-function:cubic-bezier(0,0,.2,1);-webkit-user-select:none;-moz-user-select:none;user-select:none}.nav-toc .expand:focus,.nav-toc .expand:hover{color:#0ea5e9;color:var(--color-brand)}.nav-toc li>ul{max-height:0;overflow-y:hidden;padding-left:1rem}.nav-toc .expanded>div>.expand{--tw-rotate:90deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(90deg) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.nav-toc .expanded>ul{max-height:100%}.nav-toc .expanded>ul a.current{color:#0ea5e9;color:var(--color-brand)}.nav-toc a{--tw-text-opacity:1;color:#616161;color:rgb(97 97 97/var(--tw-text-opacity));display:inline-block;padding-bottom:.25rem;padding-top:.25rem}.nav-toc a:focus,.nav-toc a:hover{color:#0ea5e9;color:var(--color-brand)}.nav-toc a.current{--tw-text-opacity:1;color:#212121;color:rgb(33 33 33/var(--tw-text-opacity));font-weight:500}.nav-toc ul+ul{margin-top:2rem}.toctree-wrapper .caption{--tw-text-opacity:1;color:#616161;color:rgb(97 97 97/var(--tw-text-opacity));font-family:JetBrains\ Mono,monospace;font-size:.875rem;font-weight:500;line-height:1.5;padding-bottom:1.5rem;text-transform:uppercase}.toctree-wrapper{border-top-width:1px;margin-bottom:3rem;margin-top:3rem;padding-top:3rem}.toctree-wrapper li li{padding-left:1rem}.toctree-wrapper a{color:#0369a1;color:var(--color-link);display:block;padding-bottom:.25rem;padding-top:.25rem}.toctree-wrapper a:focus,.toctree-wrapper a:hover{color:#0ea5e9;color:var(--color-brand)}.nav-link{font-size:.95rem;letter-spacing:.2px}.headerlink{font-size:1em;line-height:1.2em;margin-left:.25rem;vertical-align:middle}.headerlink:focus,.headerlink:hover{color:#0ea5e9;color:var(--color-brand)}.headerlink>*{fill:currentColor;height:1em;visibility:hidden}.headerlink:focus>*{visibility:visible}h1 .headerlink,h2 .headerlink,h3 .headerlink{--tw-text-opacity:1;color:#9ca3af;color:rgb(156 163 175/var(--tw-text-opacity))}h1 .headerlink:focus,h1 .headerlink:hover,h2 .headerlink:focus,h2 .headerlink:hover,h3 .headerlink:focus,h3 .headerlink:hover{color:#0ea5e9;color:var(--color-brand)}h1 .headerlink{font-size:.65em;line-height:1.2}h2 .headerlink{font-size:.75em;line-height:1.2}.code-header .headerlink{margin-right:.5rem}.admonition-title:hover .headerlink,.admonition-title:hover .headerlink>*,.code-header:hover .headerlink,.code-header:hover .headerlink>*,dt:not(.does-not-exist):hover .headerlink,dt:not(.does-not-exist):hover .headerlink>*,figure:not(.does-not-exist):hover .headerlink,figure:not(.does-not-exist):hover .headerlink>*,h1:not(.does-not-exist):hover .headerlink,h1:not(.does-not-exist):hover .headerlink>*,h2:not(.does-not-exist):hover .headerlink,h2:not(.does-not-exist):hover .headerlink>*,h3:not(.does-not-exist):hover .headerlink,h3:not(.does-not-exist):hover .headerlink>*,h4:not(.does-not-exist):hover .headerlink,h4:not(.does-not-exist):hover .headerlink>*,table:not(.does-not-exist):hover .headerlink,table:not(.does-not-exist):hover .headerlink>*{visibility:visible}.search a,p:not(.admonition-title) a{color:#0369a1;color:var(--color-link)}.search a:focus,.search a:hover,p:not(.admonition-title) a:focus,p:not(.admonition-title) a:hover{color:#0ea5e9;color:var(--color-brand)}ul.search{list-style-type:none;padding-left:0}.search li{border-top-width:1px;margin-bottom:1rem;margin-top:1rem;padding-bottom:1rem;padding-left:0;padding-top:1rem}.search li a{font-size:1.375rem;line-height:1.2}.search .context{--tw-text-opacity:1;color:#1f2937;color:rgb(31 41 55/var(--tw-text-opacity));font-size:.875rem;line-height:1.5}.highlighted{--tw-bg-opacity:1;background-color:#fef9c3;background-color:rgb(254 249 195/var(--tw-bg-opacity));font-weight:500;padding-bottom:1px;padding-top:1px}.highlight-link{display:none}article p a:focus,article p a:hover{text-decoration-line:underline}.footnote-reference{font-size:.75rem;line-height:1.5;vertical-align:super}.external-link-icon{fill:currentColor;height:.875rem;margin-bottom:2px;margin-left:1px}.viewcode-link{color:#0369a1;color:var(--color-link);margin-left:1rem}.viewcode-link:focus,.viewcode-link:hover{color:#0ea5e9;color:var(--color-brand)}.viewcode-back{color:#0369a1;color:var(--color-link);position:absolute;right:1rem}.viewcode-back:focus,.viewcode-back:hover{color:#0ea5e9;color:var(--color-brand)}:not(pre)>code{--tw-bg-opacity:1;background-color:#f9fafb;background-color:rgb(249 250 251/var(--tw-bg-opacity));border-width:1px;font-weight:500;padding-left:.25rem;padding-right:.25rem}@media (min-width:640px){:not(pre)>code{font-size:.9375em;line-height:1.5}}:not(pre)>code.highlight{--tw-bg-opacity:1;background-color:#f9fafb;background-color:rgb(249 250 251/var(--tw-bg-opacity))}main kbd:not(.compound){--tw-border-opacity:1;border-color:#212121;border-color:rgb(33 33 33/var(--tw-border-opacity));border-radius:.125rem;border-width:1px;display:inline-block;font-size:.75rem;font-weight:500;line-height:1.5;padding:.25rem}pre{border-radius:.125rem;border-width:1px;line-height:1.5;margin-bottom:1.5rem;overflow-x:hidden;position:relative}pre code,pre.literal-block{overflow-x:auto;padding-bottom:1rem;padding-left:1rem;padding-top:1rem}pre code{display:block}pre .copy{--tw-bg-opacity:1;--tw-text-opacity:1;background-color:#fff;background-color:rgb(255 255 255/var(--tw-bg-opacity));border-radius:.125rem;border-width:1px;color:#374151;color:rgb(55 65 81/var(--tw-text-opacity));font-size:.75rem;letter-spacing:.025em;line-height:1.5;opacity:0;padding:.25rem;position:absolute;right:.375rem;text-transform:uppercase;top:.75rem;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transition-duration:.5s;transition-property:all;transition-timing-function:cubic-bezier(.4,0,.2,1);-webkit-user-select:none;-moz-user-select:none;user-select:none}pre .copy:focus{opacity:1}pre .copy:active{--tw-translate-x:0.125rem;--tw-translate-y:0.125rem;transform:translate(.125rem,.125rem) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}pre:hover .copy{opacity:1}.code-wrapper{margin-bottom:1.5rem;margin-top:1.5rem}.code-wrapper .caption-text{--tw-text-opacity:1;color:#616161;color:rgb(97 97 97/var(--tw-text-opacity));letter-spacing:.025em}.code-wrapper pre{border-top-left-radius:0;border-top-right-radius:0}.code-wrapper del,.code-wrapper ins,.code-wrapper mark{display:block;margin-left:-1rem;padding-bottom:1px;padding-left:1rem;padding-top:1px;position:relative}.code-wrapper mark{background-color:rgba(186,230,253,.7)}.code-wrapper ins{background-color:rgba(187,247,208,.7);text-decoration-line:none}.code-wrapper ins:before{--tw-text-opacity:1;color:#14532d;color:rgb(20 83 45/var(--tw-text-opacity));content:"\002b";left:2px;position:absolute}.code-wrapper del{background-color:hsla(0,96%,89%,.7);text-decoration-line:none}.code-wrapper del:before{--tw-text-opacity:1;color:#7f1d1d;color:rgb(127 29 29/var(--tw-text-opacity));content:"\2212";left:2px;position:absolute}.code-wrapper .linenos{--tw-text-opacity:1;background-color:transparent;color:#374151;color:rgb(55 65 81/var(--tw-text-opacity));padding:0 1.5rem 0 0;-webkit-user-select:none;-moz-user-select:none;user-select:none}.code-wrapper .code-line{display:block}span.gd{background-color:#fecaca;background-color:rgb(254 202 202/var(--tw-bg-opacity))}span.gd,span.gi{--tw-bg-opacity:1;display:inline-block;padding-bottom:1px;padding-top:1px;width:100%}span.gi{background-color:#bbf7d0;background-color:rgb(187 247 208/var(--tw-bg-opacity))}.code-header{--tw-bg-opacity:1;align-items:center;background-color:#f9fafb;background-color:rgb(249 250 251/var(--tw-bg-opacity));border-left-width:1px;border-right-width:1px;border-top-left-radius:.125rem;border-top-right-radius:.125rem;border-top-width:1px;display:flex;font-size:.875rem;justify-content:space-between;line-height:1.5;padding-bottom:.25rem;padding-top:.25rem}.code-lang{--tw-text-opacity:1;color:#212121;color:rgb(33 33 33/var(--tw-text-opacity));display:inline-block;font-family:JetBrains\ Mono,monospace;letter-spacing:.05em;margin-left:.5rem;margin-right:auto;text-transform:uppercase}.gp{font-weight:500;pointer-events:none;-webkit-user-select:none;-moz-user-select:none;user-select:none}var{--tw-text-opacity:1;color:#6b21a8;color:rgb(107 33 168/var(--tw-text-opacity));font-style:italic}.guilabel,.menuselection{--tw-text-opacity:1;color:#212121;color:rgb(33 33 33/var(--tw-text-opacity));font-weight:500;letter-spacing:.025em}dl.code-definition,dl.option-list{border-top-width:1px;margin-bottom:3rem;margin-top:1.5rem;padding-top:1.5rem}dl.code-definition dt,dl.option-list dt{font-weight:400}dl.code-definition dt>code,dl.code-definition dt>kbd,dl.option-list dt>code,dl.option-list dt>kbd{--tw-text-opacity:1;background-color:transparent;border-style:none;color:#212121;color:rgb(33 33 33/var(--tw-text-opacity));font-size:16px;font-weight:600;line-height:1.5;padding-left:0;padding-right:0}dl.code-definition .property,dl.option-list .property{--tw-text-opacity:1;color:#616161;color:rgb(97 97 97/var(--tw-text-opacity));font-family:JetBrains\ Mono,monospace;font-weight:500}dl.code-definition .sig-param,dl.option-list .sig-param{--tw-text-opacity:1;color:#0c4a6e;color:rgb(12 74 110/var(--tw-text-opacity));font-family:JetBrains\ Mono,monospace}dl.code-definition .sig-paren,dl.option-list .sig-paren{margin-left:.25rem;margin-right:.25rem}dl.footnote{display:grid;font-size:.875rem;grid-template-columns:max-content auto;line-height:1.5}dl.footnote dt{color:#0369a1;color:var(--color-link)}dl.footnote span.brackets:before{content:"["}dl.footnote span.brackets:after{content:"]"}table caption{--tw-text-opacity:1;color:#616161;color:rgb(97 97 97/var(--tw-text-opacity));font-size:.875rem;letter-spacing:.025em;line-height:1.5;margin-bottom:1rem;text-align:left}table:not(.highlighttable){font-size:.875rem;line-height:1.5;margin-bottom:3rem;margin-top:3rem}table:not(.highlighttable) p+p{margin-top:1rem}table:not(.highlighttable) tbody tr{border-top-width:1px}table:not(.highlighttable) th{font-weight:500;letter-spacing:.025em;padding-bottom:.75rem;padding-top:.75rem;text-align:left;vertical-align:top}table:not(.highlighttable) td{padding-bottom:.5rem;padding-top:.5rem;text-align:left;vertical-align:top}.caption-number{--tw-text-opacity:1;color:#616161;color:rgb(97 97 97/var(--tw-text-opacity));font-size:.875rem;font-weight:500;line-height:1.5}figure{margin-bottom:3rem;margin-top:3rem}figure .legend{--tw-text-opacity:1;border-bottom-width:1px;color:#616161;color:rgb(97 97 97/var(--tw-text-opacity));font-size:.875rem;line-height:1.5;padding-bottom:2rem}figure .legend p{margin-bottom:1rem;margin-top:1rem}figure img{display:inline-block}main :not(figure)>img{margin-bottom:3rem;margin-top:3rem}figcaption{--tw-text-opacity:1;color:#616161;color:rgb(97 97 97/var(--tw-text-opacity));font-size:.875rem;letter-spacing:.025em;line-height:1.25;margin-top:1rem}.align-center{margin-left:auto;margin-right:auto;text-align:center}.align-right{margin-left:auto;text-align:right}blockquote{--tw-shadow:0 1px 3px 0 rgba(0,0,0,.1),0 1px 2px -1px rgba(0,0,0,.1);--tw-shadow-colored:0 1px 3px 0 var(--tw-shadow-color),0 1px 2px -1px var(--tw-shadow-color);background-color:rgba(249,250,251,.3);border-left-width:4px;border-radius:.125rem;box-shadow:0 0 transparent,0 0 transparent,0 1px 3px 0 rgba(0,0,0,.1),0 1px 2px -1px rgba(0,0,0,.1);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow);font-size:.875rem;line-height:1.5;margin-bottom:1.5rem;margin-top:1.5rem;padding:1rem}blockquote .attribution{font-style:italic}.admonition{--tw-border-opacity:1;--tw-bg-opacity:0.02;--tw-text-opacity:1;--tw-shadow:0 1px 3px 0 rgba(0,0,0,.1),0 1px 2px -1px rgba(0,0,0,.1);--tw-shadow-colored:0 1px 3px 0 var(--tw-shadow-color),0 1px 2px -1px var(--tw-shadow-color);background-color:rgba(56,189,248,.02);background-color:rgb(56 189 248/var(--tw-bg-opacity));border-color:#38bdf8;border-color:rgb(56 189 248/var(--tw-border-opacity));border-left-width:4px;border-radius:.125rem;box-shadow:0 0 transparent,0 0 transparent,0 1px 3px 0 rgba(0,0,0,.1),0 1px 2px -1px rgba(0,0,0,.1);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow);color:#0c4a6e;color:rgb(12 74 110/var(--tw-text-opacity));font-size:.875rem;line-height:1.5;margin-bottom:1.5rem;margin-top:1.5rem;padding:1rem}.admonition p:not(.admonition-title){margin-bottom:1rem;margin-top:1rem}.admonition p:last-child{margin-bottom:0}.admonition .headerlink{color:currentColor}.seealso{--tw-text-opacity:1;background-color:transparent;border-style:none;color:#616161;color:rgb(97 97 97/var(--tw-text-opacity));padding:.5rem}.seealso .admonition-title{padding-left:.5rem;padding-right:.5rem}.seealso a{background-color:rgba(249,250,251,.4);display:inline-block;padding:.5rem;transition-duration:.15s;transition-property:all;transition-timing-function:cubic-bezier(.4,0,.2,1)}.seealso a.internal:after{content:"\2192";margin-left:.5rem;opacity:0;transition-duration:.15s}.seealso a:hover{background-color:#0ea5e9;background-color:var(--color-brand);color:#fff!important;-webkit-text-decoration:none!important;text-decoration:none!important}.seealso a:hover:after{opacity:1}.seealso a code{background-color:transparent;border-style:none}.hint,.tip{background-color:rgba(74,222,128,.02);background-color:rgb(74 222 128/var(--tw-bg-opacity));border-color:#4ade80;border-color:rgb(74 222 128/var(--tw-border-opacity));color:#14532d;color:rgb(20 83 45/var(--tw-text-opacity))}.danger,.error,.hint,.tip,.warning{--tw-border-opacity:1;--tw-bg-opacity:0.02;--tw-text-opacity:1}.danger,.error,.warning{background-color:hsla(0,91%,71%,.02);background-color:rgb(248 113 113/var(--tw-bg-opacity));border-color:#f87171;border-color:rgb(248 113 113/var(--tw-border-opacity));color:#7f1d1d;color:rgb(127 29 29/var(--tw-text-opacity))}.caution,.important{--tw-border-opacity:1;--tw-bg-opacity:0.02;--tw-text-opacity:1;background-color:rgba(250,204,21,.02);background-color:rgb(250 204 21/var(--tw-bg-opacity));border-color:#facc15;border-color:rgb(250 204 21/var(--tw-border-opacity));color:#713f12;color:rgb(113 63 18/var(--tw-text-opacity))}.admonition-title{font-weight:500;letter-spacing:.025em;margin-bottom:1rem;margin-top:0}@media print{p{orphans:2;widows:2}h2,h3,h4{-moz-column-break-after:avoid;break-after:avoid;page-break-after:avoid}a,h2,h3,h4{-moz-column-break-inside:avoid;break-inside:avoid;page-break-inside:avoid}section[role=contentinfo]{-moz-column-break-before:avoid;break-before:avoid;page-break-before:avoid}table{-moz-column-break-inside:avoid;break-inside:avoid;page-break-inside:avoid}code,pre{white-space:pre-wrap!important}.seealso a.internal:after,main a:after{content:" (" attr(href) ")"}}.tooltipped{position:relative}.tooltipped:after{-webkit-font-smoothing:subpixel-antialiased;word-wrap:break-word;--tw-bg-opacity:0.75;--tw-text-opacity:1;background-color:rgba(31,41,55,.75);background-color:rgb(31 41 55/var(--tw-bg-opacity));border-radius:.125rem;color:#fff;color:rgb(255 255 255/var(--tw-text-opacity));content:attr(aria-label);display:none;font-size:.75rem;font-weight:400;letter-spacing:normal;letter-spacing:.025em;line-height:1.5;opacity:0;padding:.25rem .5rem;pointer-events:none;position:absolute;text-align:center;text-decoration-line:none;text-shadow:none;text-transform:none;white-space:pre;z-index:1000000}@keyframes tooltip-appear{0%{opacity:0}to{opacity:1}}.tooltipped:focus:after,.tooltipped:focus:before,.tooltipped:hover:after,.tooltipped:hover:before{animation-delay:.2s;animation-duration:.4s;animation-fill-mode:forwards;animation-name:tooltip-appear;animation-timing-function:ease-in;display:inline-block;-webkit-text-decoration:none;text-decoration:none}.tooltipped-no-delay:focus:after,.tooltipped-no-delay:focus:before,.tooltipped-no-delay:hover:after,.tooltipped-no-delay:hover:before{animation-delay:0s}.tooltipped-multiline:focus:after,.tooltipped-multiline:hover:after{display:table-cell}.tooltipped-s:after,.tooltipped-se:after,.tooltipped-sw:after{margin-top:6px;right:50%;top:100%}.tooltipped-s:before,.tooltipped-se:before,.tooltipped-sw:before{border-bottom-color:#1a202c;bottom:-7px;margin-right:-6px;right:50%;top:auto}.tooltipped-se:after{left:50%;margin-left:-16px;right:auto}.tooltipped-sw:after{margin-right:-16px}.tooltipped-n:after,.tooltipped-ne:after,.tooltipped-nw:after{bottom:100%;margin-bottom:6px;right:50%}.tooltipped-n:before,.tooltipped-ne:before,.tooltipped-nw:before{border-top-color:#1a202c;bottom:auto;margin-right:-6px;right:50%;top:-7px}.tooltipped-ne:after{left:50%;margin-left:-16px;right:auto}.tooltipped-nw:after{margin-right:-16px}.tooltipped-n:after,.tooltipped-s:after{transform:translateX(50%)}.tooltipped-w:after{bottom:50%;margin-right:6px;right:100%;transform:translateY(50%)}.tooltipped-w:before{border-left-color:#1a202c;bottom:50%;left:-7px;margin-top:-6px;top:50%}.tooltipped-e:after{bottom:50%;left:100%;margin-left:6px;transform:translateY(50%)}.tooltipped-e:before{border-right-color:#1a202c;bottom:50%;margin-top:-6px;right:-7px;top:50%}.tooltipped-align-right-1:after,.tooltipped-align-right-2:after{margin-right:0;right:0}.tooltipped-align-right-1:before{right:10px}.tooltipped-align-right-2:before{right:15px}.tooltipped-align-left-1:after,.tooltipped-align-left-2:after{left:0;margin-left:0}.tooltipped-align-left-1:before{left:5px}.tooltipped-align-left-2:before{left:10px}.tooltipped-multiline:after{word-wrap:break-word;border-collapse:separate;max-width:250px;white-space:pre-line;width:-moz-max-content;width:max-content}.tooltipped-multiline.tooltipped-n:after,.tooltipped-multiline.tooltipped-s:after{left:50%;right:auto;transform:translateX(-50%)}.tooltipped-multiline.tooltipped-e:after,.tooltipped-multiline.tooltipped-w:after{right:100%}@media screen and (min-width:0\0){.tooltipped-multiline:after{width:250px}}.tooltipped-sticky:after,.tooltipped-sticky:before{display:inline-block}.tooltipped-sticky.tooltipped-multiline:after{display:table-cell}button.expand-more{--tw-text-opacity:1;color:#4b5563;color:rgb(75 85 99/var(--tw-text-opacity));float:right;margin-left:.5rem}button.expand-more:focus,button.expand-more:hover{color:#0ea5e9;color:var(--color-brand)}button.expand-more>svg{--tw-rotate:0deg;fill:currentColor;height:1.5rem;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(0deg) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transition-duration:.1s;transition-property:transform;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-timing-function:cubic-bezier(0,0,.2,1);width:1.5rem}.accordion:hover .expand-more{color:#0ea5e9;color:var(--color-brand)}.active .expand-more>svg{--tw-rotate:180deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(180deg) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.panel{max-height:0;opacity:0;overflow-y:hidden;transition-duration:.5s;transition-property:opacity;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-timing-function:cubic-bezier(0,0,.2,1);visibility:hidden}.active+.panel{max-height:-moz-fit-content;max-height:fit-content;opacity:1;overflow-y:visible;visibility:visible}:root{--docsearch-searchbox-background:transparent;--docsearch-searchbox-shadow:inset 0 0 0 2px var(--color-brand);--docsearch-key-gradient:transparent;--docsearch-primary-color:#1c75b0;--docsearch-modal-width:960px}.DocSearch-Button{border-radius:0;height:3.5rem;line-height:3.5rem;padding-right:1rem}.DocSearch-Button-Key{font-family:Roboto,sans-serif;font-size:.875rem;height:1.25rem;line-height:1.5;padding:1rem}.DocSearch-Button:hover .DocSearch-Button-Key{--tw-border-opacity:1;--tw-text-opacity:1;border-color:#212121;border-color:rgb(33 33 33/var(--tw-border-opacity));color:#212121;color:rgb(33 33 33/var(--tw-text-opacity))}.DocSearch-Button .DocSearch-Search-Icon{--tw-text-opacity:1;stroke-width:2.5;color:#f3f4f6;color:rgb(243 244 246/var(--tw-text-opacity))}.DocSearch-Button:hover .DocSearch-Search-Icon{color:var(--docsearch-text-color)}.DocSearch-Button-Placeholder{padding-left:.75rem}.sr-only{clip:rect(0,0,0,0);border-width:0;height:1px;margin:-1px;overflow:hidden;padding:0;position:absolute;white-space:nowrap;width:1px}.pointer-events-none{pointer-events:none}.visible{visibility:visible}.collapse{visibility:collapse}.static{position:static}.fixed{position:fixed}.absolute{position:absolute}.relative{position:relative}.sticky{position:sticky}.inset-0{left:0;right:0}.inset-0,.inset-y-0{bottom:0;top:0}.bottom-0{bottom:0}.left-0{left:0}.right-0{right:0}.top-0{top:0}.z-10{z-index:10}.z-20{z-index:20}.col-span-full{grid-column:1/-1}.m-4{margin:1rem}.mx-0{margin-left:0;margin-right:0}.mx-5{margin-left:1.25rem;margin-right:1.25rem}.mx-auto{margin-left:auto;margin-right:auto}.my-8{margin-bottom:2rem;margin-top:2rem}.mb-2{margin-bottom:.5rem}.mb-4{margin-bottom:1rem}.ml-auto{margin-left:auto}.mr-1{margin-right:.25rem}.mr-auto{margin-right:auto}.mt-12{margin-top:3rem}.mt-16{margin-top:4rem}.mt-20{margin-top:5rem}.block{display:block}.inline-block{display:inline-block}.flex{display:flex}.hidden{display:none}.h-14{height:3.5rem}.h-6{height:1.5rem}.h-8{height:2rem}.h-full{height:100%}.min-h-screen{min-height:100vh}.w-0{width:0}.w-14{width:3.5rem}.w-6{width:1.5rem}.w-8{width:2rem}.w-full{width:100%}.max-w-prose{max-width:760px}.flex-1{flex:1 1 0%}.shrink-0{flex-shrink:0}.-translate-x-full{--tw-translate-x:-100%;transform:translate(-100%,var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.translate-y-full{--tw-translate-y:100%;transform:translate(var(--tw-translate-x),100%) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.transform,.translate-y-full{transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.transform-gpu{transform:translate3d(var(--tw-translate-x),var(--tw-translate-y),0) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.flex-col{flex-direction:column}.items-center{align-items:center}.justify-end{justify-content:flex-end}.justify-center{justify-content:center}.justify-between{justify-content:space-between}.self-center{align-self:center}.overflow-y-auto{overflow-y:auto}.scroll-smooth{scroll-behavior:smooth}.rounded-full{border-radius:9999px}.border-b-4{border-bottom-width:4px}.border-brand{border-color:#0ea5e9;border-color:var(--color-brand)}.bg-black{--tw-bg-opacity:1;background-color:#000;background-color:rgb(0 0 0/var(--tw-bg-opacity))}.bg-gray-700{--tw-bg-opacity:1;background-color:#374151;background-color:rgb(55 65 81/var(--tw-bg-opacity))}.bg-gray-900{--tw-bg-opacity:1;background-color:#111827;background-color:rgb(17 24 39/var(--tw-bg-opacity))}.bg-gray-dark{--tw-bg-opacity:1;background-color:#212121;background-color:rgb(33 33 33/var(--tw-bg-opacity))}.bg-transparent{background-color:transparent}.bg-white{--tw-bg-opacity:1;background-color:#fff;background-color:rgb(255 255 255/var(--tw-bg-opacity))}.bg-opacity-50{--tw-bg-opacity:0.5}.fill-current{fill:currentColor}.stroke-current{stroke:currentColor}.p-2{padding:.5rem}.p-3{padding:.75rem}.p-4{padding:1rem}.px-2{padding-left:.5rem;padding-right:.5rem}.px-4{padding-left:1rem;padding-right:1rem}.pl-2{padding-left:.5rem}.pl-6{padding-left:1.5rem}.pr-2{padding-right:.5rem}.pr-4{padding-right:1rem}.pt-14{padding-top:3.5rem}.pt-4{padding-top:1rem}.pt-8{padding-top:2rem}.text-right{text-align:right}.text-3xl{font-size:2.5rem;line-height:1.2}.text-4xl{font-size:3rem;line-height:1.2}.text-sm{font-size:.875rem;line-height:1.5}.text-xl{font-size:1.5rem;line-height:1.2}.text-xs{font-size:.75rem;line-height:1.5}.font-medium{font-weight:500}.uppercase{text-transform:uppercase}.leading-14{line-height:3.5rem}.tracking-wide{letter-spacing:.025em}.tracking-wider{letter-spacing:.05em}.text-gray{--tw-text-opacity:1;color:#424242;color:rgb(66 66 66/var(--tw-text-opacity))}.text-gray-100{--tw-text-opacity:1;color:#f3f4f6;color:rgb(243 244 246/var(--tw-text-opacity))}.text-gray-300{--tw-text-opacity:1;color:#d1d5db;color:rgb(209 213 219/var(--tw-text-opacity))}.text-gray-600{--tw-text-opacity:1;color:#4b5563;color:rgb(75 85 99/var(--tw-text-opacity))}.text-gray-700{--tw-text-opacity:1;color:#374151;color:rgb(55 65 81/var(--tw-text-opacity))}.text-gray-800{--tw-text-opacity:1;color:#1f2937;color:rgb(31 41 55/var(--tw-text-opacity))}.text-gray-light{--tw-text-opacity:1;color:#616161;color:rgb(97 97 97/var(--tw-text-opacity))}.text-inherit{color:inherit}.text-link{color:#0369a1;color:var(--color-link)}.text-red-700{--tw-text-opacity:1;color:#b91c1c;color:rgb(185 28 28/var(--tw-text-opacity))}.text-white{--tw-text-opacity:1;color:#fff;color:rgb(255 255 255/var(--tw-text-opacity))}.antialiased{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale}.opacity-0{opacity:0}.shadow-md{--tw-shadow:0 4px 6px -1px rgba(0,0,0,.1),0 2px 4px -2px rgba(0,0,0,.1);--tw-shadow-colored:0 4px 6px -1px var(--tw-shadow-color),0 2px 4px -2px var(--tw-shadow-color);box-shadow:0 0 transparent,0 0 transparent,0 4px 6px -1px rgba(0,0,0,.1),0 2px 4px -2px rgba(0,0,0,.1);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow)}.blur{--tw-blur:blur(8px);filter:blur(8px) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) var(--tw-invert) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow);filter:var(--tw-blur) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) var(--tw-invert) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow)}.transition{transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,-webkit-backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter,-webkit-backdrop-filter;transition-timing-function:cubic-bezier(.4,0,.2,1)}.transition-all{transition-duration:.15s;transition-property:all;transition-timing-function:cubic-bezier(.4,0,.2,1)}.transition-opacity{transition-duration:.15s;transition-property:opacity;transition-timing-function:cubic-bezier(.4,0,.2,1)}.duration-100{transition-duration:.1s}.duration-1000{transition-duration:1s}.duration-300{transition-duration:.3s}.duration-500{transition-duration:.5s}.lead{--tw-text-opacity:1;color:#212121;color:rgb(33 33 33/var(--tw-text-opacity));font-size:1.125rem;line-height:1.5;margin-bottom:4rem;margin-top:1rem}.centered{text-align:center}p.rubric{--tw-text-opacity:1;color:#212121;color:rgb(33 33 33/var(--tw-text-opacity));font-weight:500;margin-bottom:0;margin-top:3rem}.grid-area-header{grid-area:header}.grid-area-sidebar{grid-area:sidebar}.grid-area-main{grid-area:main}#page.isShown{overflow:hidden}[data-sidebar-target=sidebar].isShown{--tw-translate-x:0px;max-width:90%;opacity:1;transform:translateY(var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));width:100%}[data-scroll-target=scrollToTop].isShown{opacity:1;pointer-events:auto}[data-sidebar-target=screen].isShown{display:block}[data-search-target=snackbar].isShown{--tw-translate-y:0px;opacity:1;transform:translate(var(--tw-translate-x)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transition-duration:.5s;transition-timing-function:cubic-bezier(0,0,.2,1)}.focus-within\:absolute:focus-within{position:absolute}.focus-within\:inset-x-0:focus-within{left:0;right:0}.focus-within\:top-0:focus-within{top:0}.focus-within\:bg-gray-50:focus-within{--tw-bg-opacity:1;background-color:#f9fafb;background-color:rgb(249 250 251/var(--tw-bg-opacity))}.focus-within\:text-gray-800:focus-within{--tw-text-opacity:1;color:#1f2937;color:rgb(31 41 55/var(--tw-text-opacity))}.hover\:bg-gray-300:hover{--tw-bg-opacity:1;background-color:#d1d5db;background-color:rgb(209 213 219/var(--tw-bg-opacity))}.hover\:bg-gray-700:hover{--tw-bg-opacity:1;background-color:#374151;background-color:rgb(55 65 81/var(--tw-bg-opacity))}.hover\:text-brand:hover{color:#0ea5e9;color:var(--color-brand)}.hover\:text-gray-dark:hover{--tw-text-opacity:1;color:#212121;color:rgb(33 33 33/var(--tw-text-opacity))}.hover\:text-link:hover{color:#0369a1;color:var(--color-link)}.hover\:underline:hover{text-decoration-line:underline}.hover\:no-underline:hover{text-decoration-line:none}.focus\:w-full:focus{width:100%}.focus\:translate-x-0:focus{--tw-translate-x:0px;transform:translateY(var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.focus\:bg-gray-200:focus{--tw-bg-opacity:1;background-color:#e5e7eb;background-color:rgb(229 231 235/var(--tw-bg-opacity))}.focus\:bg-gray-700:focus{--tw-bg-opacity:1;background-color:#374151;background-color:rgb(55 65 81/var(--tw-bg-opacity))}.focus\:text-brand:focus{color:#0ea5e9;color:var(--color-brand)}.focus\:text-gray-dark:focus{--tw-text-opacity:1;color:#212121;color:rgb(33 33 33/var(--tw-text-opacity))}.focus\:text-link:focus{color:#0369a1;color:var(--color-link)}.focus\:underline:focus{text-decoration-line:underline}.focus\:opacity-100:focus{opacity:1}.focus\:outline-none:focus{outline:2px solid transparent;outline-offset:2px}.focus\:ring-2:focus{--tw-ring-offset-shadow:var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow:var(--tw-ring-inset) 0 0 0 calc(2px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color),var(--tw-ring-inset) 0 0 0 calc(2px + var(--tw-ring-offset-width)) var(--tw-ring-color),0 0 transparent;box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow,0 0 #0000)}.focus\:ring-blue-600:focus{--tw-ring-opacity:1;--tw-ring-color:rgba(2,132,199,var(--tw-ring-opacity))}@media (min-width:640px){.sm\:px-4{padding-left:1rem;padding-right:1rem}}@media (min-width:768px){.md\:mx-auto{margin-left:auto;margin-right:auto}.md\:ml-4{margin-left:1rem}.md\:w-auto{width:auto}.md\:focus-within\:static:focus-within{position:static}.md\:focus-within\:w-full:focus-within{width:100%}}@media (min-width:1024px){.lg\:inline-block{display:inline-block}}@media (min-width:1280px){.xl\:relative{position:relative}.xl\:z-0{z-index:0}.xl\:ml-fluid{margin-left:7.5vw;margin-left:var(--fluid-margin)}.xl\:mr-0{margin-right:0}.xl\:grid{display:grid}.xl\:hidden{display:none}.xl\:h-screen{height:100vh}.xl\:translate-x-0{--tw-translate-x:0px;transform:translateY(var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.xl\:px-2{padding-left:.5rem;padding-right:.5rem}.xl\:opacity-100{opacity:1}.xl\:grid-layout{grid-template-areas:"header header" "sidebar main";grid-template-columns:max(300px,17%) 1fr;grid-template-columns:max(var(--sidebar-width),17%) 1fr;grid-template-rows:min-content 1fr}}@media print{.print\:mt-4{margin-top:1rem}.print\:block{display:block}.print\:hidden{display:none}.print\:h-auto{height:auto}}
 @font-face{font-display:swap;font-family:Roboto;font-style:normal;font-weight:400;src:url(b009a76ad6afe4ebd301.woff2) format("woff2"),url(f1e2a76794cb86b2aa8e.woff) format("woff")}
 @font-face{font-display:swap;font-family:Roboto;font-style:italic;font-weight:400;src:url(e10742dbb1d4a0864ba8.woff2) format("woff2"),url(d037cb4792991826de7d.woff) format("woff")}
 @font-face{font-display:swap;font-family:Roboto;font-style:normal;font-weight:500;src:url(f25d774ecfe0996f8eb5.woff2) format("woff2"),url(48af7707fe9e6494d6a5.woff) format("woff")}
 @font-face{font-display:swap;font-family:Roboto;font-style:italic;font-weight:500;src:url(3a43b67e5bbdfb3ab0a6.woff2) format("woff2"),url(9ac5da2442b734abc516.woff) format("woff")}
 @font-face{font-display:swap;font-family:JetBrains Mono;font-style:normal;font-weight:400;src:url(d0b41bd1d599bc0a52b7.woff2) format("woff2"),url(6f04107ce68d524ebe69.woff) format("woff")}
 @font-face{font-display:swap;font-family:JetBrains Mono;font-style:italic;font-weight:400;src:url(ff058b7e238adc5cba09.woff2) format("woff2"),url(ad463ea60cc8b68792f4.woff) format("woff")}
 @font-face{font-display:swap;font-family:JetBrains Mono;font-style:normal;font-weight:500;src:url(ec416b97881f4a422686.woff2) format("woff2"),url(46830c334f8112fa510a.woff) format("woff")}
```

### Comparing `sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/static/theme.b62e1ded0c8c099a2d47.js` & `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/theme.b62e1ded0c8c099a2d47.js`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/with-sidebar.html` & `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/with-sidebar.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.2/src/sphinxawesome_theme/without-sidebar.html` & `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/without-sidebar.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.2/PKG-INFO` & `sphinxawesome_theme-4.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinxawesome-theme
-Version: 4.0.2
+Version: 4.0.3
 Summary: An awesome theme for the Sphinx documentation generator
 Home-page: https://sphinxawesome.xyz
 License: MIT
 Author: Kai Welke
 Author-email: kai687@pm.me
 Requires-Python: >=3.8,<4.0
 Classifier: Framework :: Sphinx
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Documentation
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development :: Documentation
 Provides-Extra: docs
 Requires-Dist: beautifulsoup4 (>=4.9.1,<5.0.0)
-Requires-Dist: myst-parser (>=0.19,<0.20) ; extra == "docs"
+Requires-Dist: myst-parser (>=0.19,<1.1) ; extra == "docs"
 Requires-Dist: python-dotenv (>=0.19,<1.1)
 Requires-Dist: sphinx (>4)
 Requires-Dist: sphinx-autobuild (>=2021.3.14,<2022.0.0) ; extra == "docs"
 Requires-Dist: sphinx-sitemap (>=2.2.0,<3.0.0) ; extra == "docs"
 Project-URL: Documentation, https://sphinxawesome.xyz
 Project-URL: Repository, https://github.com/kai687/sphinxawesome-theme
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: sphinxawesome-theme Version: 4.0.2 Summary: An
+Metadata-Version: 2.1 Name: sphinxawesome-theme Version: 4.0.3 Summary: An
 awesome theme for the Sphinx documentation generator Home-page: https://
 sphinxawesome.xyz License: MIT Author: Kai Welke Author-email: kai687@pm.me
 Requires-Python: >=3.8,<4.0 Classifier: Framework :: Sphinx Classifier:
 Framework :: Sphinx :: Theme Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Topic :: Documentation Classifier: Topic :: Documentation :: Sphinx Classifier:
 Topic :: Software Development :: Documentation Provides-Extra: docs Requires-
-Dist: beautifulsoup4 (>=4.9.1,<5.0.0) Requires-Dist: myst-parser (>=0.19,<0.20)
+Dist: beautifulsoup4 (>=4.9.1,<5.0.0) Requires-Dist: myst-parser (>=0.19,<1.1)
 ; extra == "docs" Requires-Dist: python-dotenv (>=0.19,<1.1) Requires-Dist:
 sphinx (>4) Requires-Dist: sphinx-autobuild (>=2021.3.14,<2022.0.0) ; extra ==
 "docs" Requires-Dist: sphinx-sitemap (>=2.2.0,<3.0.0) ; extra == "docs"
 Project-URL: Documentation, https://sphinxawesome.xyz Project-URL: Repository,
 https://github.com/kai687/sphinxawesome-theme Description-Content-Type: text/
 markdown
                       ****** Sphinx awesome theme ******
```

