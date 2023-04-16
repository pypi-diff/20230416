# Comparing `tmp/mdformat_wikilink-0.1.0.tar.gz` & `tmp/mdformat_wikilink-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdformat_wikilink-0.1.0.tar", max compression
+gzip compressed data, was "mdformat_wikilink-0.1.1.tar", max compression
```

## Comparing `mdformat_wikilink-0.1.0.tar` & `mdformat_wikilink-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1009 2023-04-16 13:32:35.125363 mdformat_wikilink-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      351 2023-04-14 09:20:02.427474 mdformat_wikilink-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-04-13 17:02:35.608055 mdformat_wikilink-0.1.0/src/mdformat_wikilink/__init__.py
--rw-r--r--   0        0        0      505 2023-04-14 10:13:40.293086 mdformat_wikilink-0.1.0/src/mdformat_wikilink/mdformat_plugin.py
--rw-r--r--   0        0        0      566 2023-04-14 10:13:38.660186 mdformat_wikilink-0.1.0/src/mdformat_wikilink/mdit_wikilink_plugin.py
--rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 mdformat_wikilink-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      351 2023-04-16 14:38:56.750524 mdformat_wikilink-0.1.1/README.md
+-rw-r--r--   0        0        0      963 2023-04-16 14:38:56.750524 mdformat_wikilink-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-16 14:38:56.750524 mdformat_wikilink-0.1.1/src/mdformat_wikilink/__init__.py
+-rw-r--r--   0        0        0      487 2023-04-16 14:38:56.750524 mdformat_wikilink-0.1.1/src/mdformat_wikilink/mdformat_plugin.py
+-rw-r--r--   0        0        0      543 2023-04-16 14:38:56.750524 mdformat_wikilink-0.1.1/src/mdformat_wikilink/mdit_wikilink_plugin.py
+-rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 mdformat_wikilink-0.1.1/PKG-INFO
```

### Comparing `mdformat_wikilink-0.1.0/pyproject.toml` & `mdformat_wikilink-0.1.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-[tool.poetry]
-name = "mdformat_wikilink"
-version = "0.1.0"
-description = ""
-authors = ["Tamir Bahar"]
-license = "MIT"
-readme = "README.md"
-
-[tool.poetry.dependencies]
-python = "^3.11"
-markdown-it-py = "^2.2.0"
-mdformat = "^0.7.16"
-
-
-[tool.poetry.group.dev.dependencies]
-ruff = "^0.0.261"
-black = "^23.3.0"
-isort = "^5.12.0"
-nox = "^2022.11.21"
-mypy = "^1.2.0"
-pytest = "^7.3.0"
-pytest-cov = "^4.0.0"
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
-
-
-[tool.poetry.plugins."mdformat.parser_extension"]
-"wikilink" = "mdformat_wikilink.mdformat_plugin"
-
-[tool.isort]
-# Configure isort to work without access to site-packages
-known_first_party = ["mdformat_wikilink", "tests"]
-
-# Settings for Black compatibility
-profile = "black"
-
-[tool.mypy]
-check_untyped_defs = true
-
-[tool.pytest.ini_options]
-xfail_strict = true
-addopts = "-ra -q --cov=mdformat_wikilink --cov-report=xml --cov-report=term-missing"
-testpaths = [
-    "tests",
+[tool.poetry]
+name = "mdformat_wikilink"
+version = "0.1.1"
+description = ""
+authors = ["Tamir Bahar"]
+license = "MIT"
+readme = "README.md"
+
+[tool.poetry.dependencies]
+python = "^3.11"
+markdown-it-py = "^2.2.0"
+mdformat = "^0.7.16"
+
+
+[tool.poetry.group.dev.dependencies]
+ruff = "^0.0.261"
+black = "^23.3.0"
+isort = "^5.12.0"
+nox = "^2022.11.21"
+mypy = "^1.2.0"
+pytest = "^7.3.0"
+pytest-cov = "^4.0.0"
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
+
+
+[tool.poetry.plugins."mdformat.parser_extension"]
+"wikilink" = "mdformat_wikilink.mdformat_plugin"
+
+[tool.isort]
+# Configure isort to work without access to site-packages
+known_first_party = ["mdformat_wikilink", "tests"]
+
+# Settings for Black compatibility
+profile = "black"
+
+[tool.mypy]
+check_untyped_defs = true
+
+[tool.pytest.ini_options]
+xfail_strict = true
+addopts = "-ra -q --cov=mdformat_wikilink --cov-report=xml --cov-report=term-missing"
+testpaths = [
+    "tests",
 ]
```

### Comparing `mdformat_wikilink-0.1.0/src/mdformat_wikilink/mdit_wikilink_plugin.py` & `mdformat_wikilink-0.1.1/src/mdformat_wikilink/mdit_wikilink_plugin.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-import re
-
-from markdown_it import MarkdownIt
-from markdown_it.rules_inline import StateInline
-
-LINK_PATTERN = re.compile(r"\[\[([^[|\]\n])+(\|[^]\n]+)?]]")
-
-
-def _wikilink_inline(state: StateInline, silent: bool) -> bool:
-    match = LINK_PATTERN.match(state.src[state.pos :])
-    if not match:
-        return False
-
-    token = state.push("wikilink", "", 0)
-    token.content = match.group()
-
-    state.pos += match.end()
-
-    return True
-
-
-def wikilink_plugin(md: MarkdownIt) -> None:
-    md.inline.ruler.push("wikilink", _wikilink_inline)
+import re
+
+from markdown_it import MarkdownIt
+from markdown_it.rules_inline import StateInline
+
+LINK_PATTERN = re.compile(r"\[\[([^[|\]\n])+(\|[^]\n]+)?]]")
+
+
+def _wikilink_inline(state: StateInline, silent: bool) -> bool:
+    match = LINK_PATTERN.match(state.src[state.pos :])
+    if not match:
+        return False
+
+    token = state.push("wikilink", "", 0)
+    token.content = match.group()
+
+    state.pos += match.end()
+
+    return True
+
+
+def wikilink_plugin(md: MarkdownIt) -> None:
+    md.inline.ruler.push("wikilink", _wikilink_inline)
```

