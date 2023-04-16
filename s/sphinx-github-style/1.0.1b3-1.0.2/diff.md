# Comparing `tmp/sphinx-github-style-1.0.1b3.tar.gz` & `tmp/sphinx-github-style-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-github-style-1.0.1b3.tar", last modified: Sat Feb 25 07:24:20 2023, max compression
+gzip compressed data, was "sphinx-github-style-1.0.2.tar", last modified: Sun Apr 16 21:47:00 2023, max compression
```

## Comparing `sphinx-github-style-1.0.1b3.tar` & `sphinx-github-style-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-02-25 07:24:20.738140 sphinx-github-style-1.0.1b3/
--rw-rw-rw-   0        0        0     1087 2023-02-19 05:31:28.000000 sphinx-github-style-1.0.1b3/LICENSE
--rw-rw-rw-   0        0        0     7182 2023-02-25 07:24:20.738140 sphinx-github-style-1.0.1b3/PKG-INFO
--rw-rw-rw-   0        0        0     6409 2023-02-25 06:57:43.000000 sphinx-github-style-1.0.1b3/README.rst
--rw-rw-rw-   0        0        0       42 2023-02-25 07:24:20.738140 sphinx-github-style-1.0.1b3/setup.cfg
--rw-rw-rw-   0        0        0     1513 2023-02-24 03:09:40.000000 sphinx-github-style-1.0.1b3/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-25 07:24:20.722519 sphinx-github-style-1.0.1b3/sphinx_github_style/
--rw-rw-rw-   0        0        0     8632 2023-02-25 07:22:38.000000 sphinx-github-style-1.0.1b3/sphinx_github_style/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-25 07:24:20.722519 sphinx-github-style-1.0.1b3/sphinx_github_style/_static/
--rw-rw-rw-   0        0        0     1128 2023-02-24 03:09:40.000000 sphinx-github-style-1.0.1b3/sphinx_github_style/_static/github_style.css
--rw-rw-rw-   0        0        0     1218 2023-02-24 03:09:40.000000 sphinx-github-style-1.0.1b3/sphinx_github_style/add_linkcode_class.py
--rw-rw-rw-   0        0        0     5556 2023-02-24 03:09:40.000000 sphinx-github-style-1.0.1b3/sphinx_github_style/github_style.py
--rw-rw-rw-   0        0        0     1462 2023-02-25 06:13:35.000000 sphinx-github-style-1.0.1b3/sphinx_github_style/meth_lexer.py
-drwxrwxrwx   0        0        0        0 2023-02-25 07:24:20.722519 sphinx-github-style-1.0.1b3/sphinx_github_style.egg-info/
--rw-rw-rw-   0        0        0     7182 2023-02-25 07:24:20.000000 sphinx-github-style-1.0.1b3/sphinx_github_style.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      430 2023-02-25 07:24:20.000000 sphinx-github-style-1.0.1b3/sphinx_github_style.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-25 07:24:20.000000 sphinx-github-style-1.0.1b3/sphinx_github_style.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-02-25 07:24:20.000000 sphinx-github-style-1.0.1b3/sphinx_github_style.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-02-25 07:24:20.000000 sphinx-github-style-1.0.1b3/sphinx_github_style.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 21:47:00.737181 sphinx-github-style-1.0.2/
+-rw-rw-rw-   0        0        0     1087 2023-02-19 05:31:28.000000 sphinx-github-style-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     7180 2023-04-16 21:47:00.737181 sphinx-github-style-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6409 2023-04-16 21:44:56.000000 sphinx-github-style-1.0.2/README.rst
+-rw-rw-rw-   0        0        0       42 2023-04-16 21:47:00.737181 sphinx-github-style-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1513 2023-02-26 08:01:56.000000 sphinx-github-style-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 21:47:00.721562 sphinx-github-style-1.0.2/sphinx_github_style/
+-rw-rw-rw-   0        0        0     8881 2023-04-16 21:42:53.000000 sphinx-github-style-1.0.2/sphinx_github_style/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 21:47:00.737181 sphinx-github-style-1.0.2/sphinx_github_style/_static/
+-rw-rw-rw-   0        0        0     1128 2023-02-24 03:09:40.000000 sphinx-github-style-1.0.2/sphinx_github_style/_static/github_style.css
+-rw-rw-rw-   0        0        0     1218 2023-02-24 03:09:40.000000 sphinx-github-style-1.0.2/sphinx_github_style/add_linkcode_class.py
+-rw-rw-rw-   0        0        0     5556 2023-02-24 03:09:40.000000 sphinx-github-style-1.0.2/sphinx_github_style/github_style.py
+-rw-rw-rw-   0        0        0     1462 2023-04-16 20:26:22.000000 sphinx-github-style-1.0.2/sphinx_github_style/meth_lexer.py
+drwxrwxrwx   0        0        0        0 2023-04-16 21:47:00.737181 sphinx-github-style-1.0.2/sphinx_github_style.egg-info/
+-rw-rw-rw-   0        0        0     7180 2023-04-16 21:47:00.000000 sphinx-github-style-1.0.2/sphinx_github_style.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      430 2023-04-16 21:47:00.000000 sphinx-github-style-1.0.2/sphinx_github_style.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 21:47:00.000000 sphinx-github-style-1.0.2/sphinx_github_style.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-16 21:47:00.000000 sphinx-github-style-1.0.2/sphinx_github_style.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-04-16 21:47:00.000000 sphinx-github-style-1.0.2/sphinx_github_style.egg-info/top_level.txt
```

### Comparing `sphinx-github-style-1.0.1b3/LICENSE` & `sphinx-github-style-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx-github-style-1.0.1b3/PKG-INFO` & `sphinx-github-style-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-github-style
-Version: 1.0.1b3
+Version: 1.0.2
 Summary: Sphinx Github Integration and Github Dark Theme Pygments Style
 Home-page: https://github.com/tdkorn/sphinx-github-style
 Author: Adam Korn
 Author-email: hello@dailykitten.net
 License: MIT License
 Download-URL: https://github.com/TDKorn/sphinx-github-style/tarball/master
 Keywords: sphinx,sphinx-extension,sphinx-theme,pygments,pygments-style,github,linkcode
@@ -17,23 +17,23 @@
 License-File: LICENSE
 
 ..  Title: Sphinx Github Style
 ..  Description: A Sphinx extension to add GitHub source code links and syntax highlighting
 ..  Author: TDKorn (Adam Korn)
 
 .. |.get_linkcode_resolve| replace:: get_linkcode_resolve()
-.. _.get_linkcode_resolve: https://github.com/TDKorn/sphinx-github-style/blob/v1.0.0/sphinx_github_style/__init__.py#L153-L210
+.. _.get_linkcode_resolve: https://github.com/TDKorn/sphinx-github-style/blob/v1.0.2/sphinx_github_style/__init__.py#L142-L203
 .. |.add_linkcode_node_class| replace:: add_linkcode_node_class()
-.. _.add_linkcode_node_class: https://github.com/TDKorn/sphinx-github-style/blob/v1.0.0/sphinx_github_style/add_linkcode_class.py#L9-L24
+.. _.add_linkcode_node_class: https://github.com/TDKorn/sphinx-github-style/blob/v1.0.2/sphinx_github_style/add_linkcode_class.py#L9-L24
 .. |.TDKStyle| replace:: TDKStyle
-.. _.TDKStyle: https://github.com/TDKorn/sphinx-github-style/blob/v1.0.0/sphinx_github_style/github_style.py#L44-L139
-.. |.TDKMethLexor| replace:: TDKMethLexor
-.. _.TDKMethLexor: https://github.com/TDKorn/sphinx-github-style/blob/v1.0.0/sphinx_github_style/meth_lexer.py#L28-L43
+.. _.TDKStyle: https://github.com/TDKorn/sphinx-github-style/blob/v1.0.2/sphinx_github_style/github_style.py#L44-L139
+.. |.TDKMethLexer| replace:: TDKMethLexer
+.. _.TDKMethLexer: https://github.com/TDKorn/sphinx-github-style/blob/v1.0.2/sphinx_github_style/meth_lexer.py#L27-L42
 .. |.github_style| replace:: github_style.css
-.. _.github_style: https://github.com/tdkorn/sphinx-github-style/blob/v1.0.0/sphinx_github_style/_static/github_style.css
+.. _.github_style: https://github.com/tdkorn/sphinx-github-style/blob/v1.0.2/sphinx_github_style/_static/github_style.css
 .. |RTD| replace:: ReadTheDocs
 .. _RTD: https://sphinx-github-style.readthedocs.io/en/latest/
 .. |Note| replace:: 📝 **Note**
 .. |docs| replace:: **Explore the docs »**
 .. _docs: https://sphinx-github-style.readthedocs.io/en/latest/
 
 
@@ -217,15 +217,15 @@
 
 |
 
 Noteworthy Components
 ~~~~~~~~~~~~~~~~~~~~~
 
 * |.TDKStyle|_ - Pygments Style for syntax highlighting similar to Github Pretty Lights Dark Theme
-* |.TDKMethLexor|_ - Pygments Lexor to add syntax highlighting to methods
+* |.TDKMethLexer|_ - Pygments Lexor to add syntax highlighting to methods
 * |.get_linkcode_resolve|_ - to link to GitHub source code using ``sphinx.ext.linkcode``
 * |.add_linkcode_node_class|_ - adds a new ``linkcode-link`` class, allowing for CSS styling separately from ``viewcode`` links
 * |.github_style|_ - CSS styling for linkcode links (icon + text)
 
 |
 
 Documentation
```

### Comparing `sphinx-github-style-1.0.1b3/README.rst` & `sphinx-github-style-1.0.2/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ..  Title: Sphinx Github Style
 ..  Description: A Sphinx extension to add GitHub source code links and syntax highlighting
 ..  Author: TDKorn (Adam Korn)
 
 .. |.get_linkcode_resolve| replace:: ``get_linkcode_resolve()``
-.. _.get_linkcode_resolve: https://github.com/TDKorn/sphinx-github-style/blob/v1.0.0/sphinx_github_style/__init__.py#L153-L210
+.. _.get_linkcode_resolve: https://github.com/TDKorn/sphinx-github-style/blob/v1.0.2/sphinx_github_style/__init__.py#L142-L203
 .. |.add_linkcode_node_class| replace:: ``add_linkcode_node_class()``
-.. _.add_linkcode_node_class: https://github.com/TDKorn/sphinx-github-style/blob/v1.0.0/sphinx_github_style/add_linkcode_class.py#L9-L24
+.. _.add_linkcode_node_class: https://github.com/TDKorn/sphinx-github-style/blob/v1.0.2/sphinx_github_style/add_linkcode_class.py#L9-L24
 .. |.TDKStyle| replace:: ``TDKStyle``
-.. _.TDKStyle: https://github.com/TDKorn/sphinx-github-style/blob/v1.0.0/sphinx_github_style/github_style.py#L44-L139
-.. |.TDKMethLexor| replace:: ``TDKMethLexor``
-.. _.TDKMethLexor: https://github.com/TDKorn/sphinx-github-style/blob/v1.0.0/sphinx_github_style/meth_lexer.py#L28-L43
+.. _.TDKStyle: https://github.com/TDKorn/sphinx-github-style/blob/v1.0.2/sphinx_github_style/github_style.py#L44-L139
+.. |.TDKMethLexer| replace:: ``TDKMethLexer``
+.. _.TDKMethLexer: https://github.com/TDKorn/sphinx-github-style/blob/v1.0.2/sphinx_github_style/meth_lexer.py#L27-L42
 .. |.github_style| replace:: ``github_style.css``
-.. _.github_style: https://github.com/tdkorn/sphinx-github-style/blob/v1.0.0/sphinx_github_style/_static/github_style.css
+.. _.github_style: https://github.com/tdkorn/sphinx-github-style/blob/v1.0.2/sphinx_github_style/_static/github_style.css
 .. |RTD| replace:: ReadTheDocs
 .. _RTD: https://sphinx-github-style.readthedocs.io/en/latest/
 .. |docs| replace:: **Explore the docs »**
 .. _docs: https://sphinx-github-style.readthedocs.io/en/latest/
 
 
 .. raw:: html
@@ -209,15 +209,15 @@
 
 |
 
 Noteworthy Components
 ~~~~~~~~~~~~~~~~~~~~~
 
 * |.TDKStyle|_ - Pygments Style for syntax highlighting similar to Github Pretty Lights Dark Theme
-* |.TDKMethLexor|_ - Pygments Lexor to add syntax highlighting to methods
+* |.TDKMethLexer|_ - Pygments Lexor to add syntax highlighting to methods
 * |.get_linkcode_resolve|_ - to link to GitHub source code using ``sphinx.ext.linkcode``
 * |.add_linkcode_node_class|_ - adds a new ``linkcode-link`` class, allowing for CSS styling separately from ``viewcode`` links
 * |.github_style|_ - CSS styling for linkcode links (icon + text)
 
 |
 
 Documentation
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
 .. Title: Sphinx Github Style .. Description: A Sphinx extension to add GitHub
 source code links and syntax highlighting .. Author: TDKorn (Adam Korn) ..
 |.get_linkcode_resolve| replace:: ``get_linkcode_resolve()`` ..
 _.get_linkcode_resolve: https://github.com/TDKorn/sphinx-github-style/blob/
-v1.0.0/sphinx_github_style/__init__.py#L153-L210 .. |.add_linkcode_node_class|
+v1.0.2/sphinx_github_style/__init__.py#L142-L203 .. |.add_linkcode_node_class|
 replace:: ``add_linkcode_node_class()`` .. _.add_linkcode_node_class: https://
-github.com/TDKorn/sphinx-github-style/blob/v1.0.0/sphinx_github_style/
+github.com/TDKorn/sphinx-github-style/blob/v1.0.2/sphinx_github_style/
 add_linkcode_class.py#L9-L24 .. |.TDKStyle| replace:: ``TDKStyle`` ..
-_.TDKStyle: https://github.com/TDKorn/sphinx-github-style/blob/v1.0.0/
-sphinx_github_style/github_style.py#L44-L139 .. |.TDKMethLexor| replace::
-``TDKMethLexor`` .. _.TDKMethLexor: https://github.com/TDKorn/sphinx-github-
-style/blob/v1.0.0/sphinx_github_style/meth_lexer.py#L28-L43 .. |.github_style|
+_.TDKStyle: https://github.com/TDKorn/sphinx-github-style/blob/v1.0.2/
+sphinx_github_style/github_style.py#L44-L139 .. |.TDKMethLexer| replace::
+``TDKMethLexer`` .. _.TDKMethLexer: https://github.com/TDKorn/sphinx-github-
+style/blob/v1.0.2/sphinx_github_style/meth_lexer.py#L27-L42 .. |.github_style|
 replace:: ``github_style.css`` .. _.github_style: https://github.com/tdkorn/
-sphinx-github-style/blob/v1.0.0/sphinx_github_style/_static/github_style.css ..
+sphinx-github-style/blob/v1.0.2/sphinx_github_style/_static/github_style.css ..
 |RTD| replace:: ReadTheDocs .. _RTD: https://sphinx-github-
 style.readthedocs.io/en/latest/ .. |docs| replace:: **Explore the docs Â»** ..
 _docs: https://sphinx-github-style.readthedocs.io/en/latest/ .. raw:: html
  .. image:: docs/source/_static/logo_square_grey_blue.png :alt: Sphinx GitHub
  Style: GitHub Integration and Pygments Style for Sphinx Documentation :width:
                                25% .. raw:: html
                        ****** sphinx-github-style ******
@@ -72,14 +72,14 @@
 ``linkcode_link_text`` ^^^^^^^^^^^^^^^^^^^^^^ .. code-block:: python
 linkcode_link_text: str = "View on GitHub" The text to use for the linkcode
 link ... ``linkcode_resolve`` ^^^^^^^^^^^^^^^^^^^^^^^^ .. code-block:: python
 linkcode_resolve: types.FunctionType A ``linkcode_resolve()`` function to use
 for resolving the link target * Uses default function from
 |.get_linkcode_resolve|_ if not specified (recommended) | Noteworthy Components
 ~~~~~~~~~~~~~~~~~~~~~ * |.TDKStyle|_ - Pygments Style for syntax highlighting
-similar to Github Pretty Lights Dark Theme * |.TDKMethLexor|_ - Pygments Lexor
+similar to Github Pretty Lights Dark Theme * |.TDKMethLexer|_ - Pygments Lexor
 to add syntax highlighting to methods * |.get_linkcode_resolve|_ - to link to
 GitHub source code using ``sphinx.ext.linkcode`` * |.add_linkcode_node_class|_
 - adds a new ``linkcode-link`` class, allowing for CSS styling separately from
 ``viewcode`` links * |.github_style|_ - CSS styling for linkcode links (icon +
 text) | Documentation ~~~~~~~~~~~~~~~~ Full documentation can be found on
 |RTD|_
```

### Comparing `sphinx-github-style-1.0.1b3/setup.py` & `sphinx-github-style-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `sphinx-github-style-1.0.1b3/sphinx_github_style/__init__.py` & `sphinx-github-style-1.0.2/sphinx_github_style/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,19 +5,17 @@
 import subprocess
 import pkg_resources
 from pathlib import Path
 from sphinx.application import Sphinx
 from sphinx.errors import ExtensionError
 from typing import Dict, Any, Optional, Callable
 
-
-__version__ = "1.0.1b3"
+__version__ = "1.0.2"
 __author__ = 'Adam Korn <hello@dailykitten.net>'
 
-
 from .add_linkcode_class import add_linkcode_node_class
 from .meth_lexer import TDKMethLexer
 from .github_style import TDKStyle
 
 
 def setup(app: Sphinx) -> Dict[str, Any]:
     app.connect("builder-inited", add_static_path)
@@ -26,52 +24,51 @@
     app.add_config_value('top_level', get_top_level(app), '')
 
     app.setup_extension('sphinx_github_style.add_linkcode_class')
     app.setup_extension('sphinx_github_style.github_style')
     app.setup_extension('sphinx_github_style.meth_lexer')
     app.setup_extension('sphinx.ext.linkcode')
 
-    html_context = getattr(app.config, 'html_context', {})
-    html_context['github_version'] = get_linkcode_revision(app)
-    setattr(app.config, 'html_context', html_context)
-
-    linkcode_url = get_linkcode_url(app)
+    linkcode_blob = get_conf_val(app, "linkcode_blob")
+    linkcode_url = get_linkcode_url(
+        blob=get_linkcode_revision(linkcode_blob),
+        url=get_conf_val(app, 'linkcode_url'),
+        context=get_conf_val(app, 'html_context'),
+    )
     linkcode_func = get_conf_val(app, "linkcode_resolve")
 
     if not callable(linkcode_func):
         print(
             "Function `linkcode_resolve` not found in ``conf.py``; "
             "using default function from ``sphinx_github_style``"
         )
         linkcode_func = get_linkcode_resolve(linkcode_url)
 
-    app.config.linkcode_resolve = linkcode_func
+    set_conf_val(app, 'linkcode_resolve', linkcode_func)
     return {'version': sphinx.__display_version__, 'parallel_read_safe': True}
 
 
 def add_static_path(app) -> None:
     """Add the path for the ``_static`` folder"""
     app.config.html_static_path.append(
         str(Path(__file__).parent.joinpath("_static").absolute())
     )
 
 
-def get_linkcode_revision(app: Sphinx) -> str:
+def get_linkcode_revision(blob: str) -> str:
     """Get the blob to link to on GitHub
 
     .. note::
 
-       The generated links depend on  the ``conf.py`` value of ``linkcode_blob``,
-       which can be any of ``"head"``, ``"last_tag"``, or ``"{blob}"``
+       The value of ``blob`` can be any of ``"head"``, ``"last_tag"``, or ``"{blob}"``
 
        * ``head`` (default): links to the most recent commit hash; if this commit is tagged, uses the tag instead
        * ``last_tag``: links to the most recently tagged commit; if no tags exist, uses ``head``
        * ``blob``: links to any blob you want, for example ``"master"`` or ``"v2.0.1"``
     """
-    blob = get_conf_val(app, "linkcode_blob")
     if blob == "head":
         return get_head()
     if blob == 'last_tag':
         return get_last_tag()
     # Link to the branch/tree/blob you provided, ex. "master"
     return blob
 
@@ -111,40 +108,39 @@
         cmd = "git describe --tags --abbrev=0"
         return subprocess.check_output(cmd.split(" ")).strip().decode('utf-8')
 
     except subprocess.CalledProcessError as e:
         raise RuntimeError("No tags exist for the repo...(?)") from e
 
 
-def get_linkcode_url(app: Sphinx) -> str:
+def get_linkcode_url(blob: Optional[str] = None, context: Optional[Dict] = None, url: Optional[str] = None) -> str:
     """Get the template URL for linking to highlighted GitHub source code
 
     Formatted into the final link by ``linkcode_resolve()``
     """
-    context = get_conf_val(app, "html_context")
-    url = get_conf_val(app, "linkcode_url")
-
     if url is None:
         if context is None or not all(context.get(key) for key in ("github_user", "github_repo")):
             raise ExtensionError(
                 "sphinx-github-style: config value ``linkcode_url`` is missing")
         else:
             print(
                 "sphinx-github-style: config value ``linkcode_url`` is missing. "
                 "Creating link from ``html_context`` values..."
             )
-            blob = context['github_version']  # Added by setup() above
-            url = f"https://github.com/{context['github_user']}/{context['github_repo']}/{blob}/"
+            url = f"https://github.com/{context['github_user']}/{context['github_repo']}"
 
+    blob = get_linkcode_revision(blob) if blob else context.get('github_version')
+
+    if blob is not None:
+        url = url.strip("/") + f"/blob/{blob}/"  # URL should be "https://github.com/user/repo"
     else:
-        # URL should be "https://github.com/user/repo"
-        url = url.strip("/") + f"/blob/{get_linkcode_revision(app)}/"
+        raise ExtensionError(
+            "sphinx-github-style: must provide a blob or GitHub version to link to")
 
-    url += "{filepath}#L{linestart}-L{linestop}"
-    return url
+    return url + "{filepath}#L{linestart}-L{linestop}"
 
 
 def get_linkcode_resolve(linkcode_url: str) -> Callable:
     """Defines and returns a ``linkcode_resolve`` function for your package
 
     Used by default if ``linkcode_resolve`` isn't defined in ``conf.py``
     """
@@ -230,23 +226,32 @@
 
                 except pkg_resources.DistributionNotFound:
                     pass
 
         finally:
             if pkg is None:
                 raise ExtensionError(
-                        "sphinx_github_style: Unable to determine top-level package")
+                    "sphinx_github_style: Unable to determine top-level package")
 
         top_level = pkg.get_metadata('top_level.txt').strip()
         app.config._raw_config['top_level'] = top_level
 
     return top_level
 
 
-def get_conf_val(app: Sphinx, attr: str, default: Any = None) -> Any:
-    """Retrieve values from ``conf.py``
+def get_conf_val(app: Sphinx, attr: str, default: Optional[Any] = None) -> Any:
+    """Retrieve the value of a ``conf.py`` config variable
 
-    Currently unclear why non-default ``conf.py`` values aren't being updated in the config attributes (?)
-    So checking for values in the ``_raw_config`` dict first, since they *do* get updated
+    :param attr: the config variable to retrieve
+    :param default: the default value to return if the variable isn't found
     """
     return app.config._raw_config.get(attr, getattr(app.config, attr, default))
 
+
+def set_conf_val(app: Sphinx, attr: str, value: Any) -> None:
+    """Set the value of a ``conf.py`` config variable
+
+    :param attr: the config variable to set
+    :param value: the variable value
+    """
+    app.config._raw_config[attr] = value
+    setattr(app.config, attr, value)
```

### Comparing `sphinx-github-style-1.0.1b3/sphinx_github_style/_static/github_style.css` & `sphinx-github-style-1.0.2/sphinx_github_style/_static/github_style.css`

 * *Files identical despite different names*

### Comparing `sphinx-github-style-1.0.1b3/sphinx_github_style/add_linkcode_class.py` & `sphinx-github-style-1.0.2/sphinx_github_style/add_linkcode_class.py`

 * *Files identical despite different names*

### Comparing `sphinx-github-style-1.0.1b3/sphinx_github_style/github_style.py` & `sphinx-github-style-1.0.2/sphinx_github_style/github_style.py`

 * *Files identical despite different names*

### Comparing `sphinx-github-style-1.0.1b3/sphinx_github_style/meth_lexer.py` & `sphinx-github-style-1.0.2/sphinx_github_style/meth_lexer.py`

 * *Files identical despite different names*

### Comparing `sphinx-github-style-1.0.1b3/sphinx_github_style.egg-info/PKG-INFO` & `sphinx-github-style-1.0.2/sphinx_github_style.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-github-style
-Version: 1.0.1b3
+Version: 1.0.2
 Summary: Sphinx Github Integration and Github Dark Theme Pygments Style
 Home-page: https://github.com/tdkorn/sphinx-github-style
 Author: Adam Korn
 Author-email: hello@dailykitten.net
 License: MIT License
 Download-URL: https://github.com/TDKorn/sphinx-github-style/tarball/master
 Keywords: sphinx,sphinx-extension,sphinx-theme,pygments,pygments-style,github,linkcode
@@ -17,23 +17,23 @@
 License-File: LICENSE
 
 ..  Title: Sphinx Github Style
 ..  Description: A Sphinx extension to add GitHub source code links and syntax highlighting
 ..  Author: TDKorn (Adam Korn)
 
 .. |.get_linkcode_resolve| replace:: get_linkcode_resolve()
-.. _.get_linkcode_resolve: https://github.com/TDKorn/sphinx-github-style/blob/v1.0.0/sphinx_github_style/__init__.py#L153-L210
+.. _.get_linkcode_resolve: https://github.com/TDKorn/sphinx-github-style/blob/v1.0.2/sphinx_github_style/__init__.py#L142-L203
 .. |.add_linkcode_node_class| replace:: add_linkcode_node_class()
-.. _.add_linkcode_node_class: https://github.com/TDKorn/sphinx-github-style/blob/v1.0.0/sphinx_github_style/add_linkcode_class.py#L9-L24
+.. _.add_linkcode_node_class: https://github.com/TDKorn/sphinx-github-style/blob/v1.0.2/sphinx_github_style/add_linkcode_class.py#L9-L24
 .. |.TDKStyle| replace:: TDKStyle
-.. _.TDKStyle: https://github.com/TDKorn/sphinx-github-style/blob/v1.0.0/sphinx_github_style/github_style.py#L44-L139
-.. |.TDKMethLexor| replace:: TDKMethLexor
-.. _.TDKMethLexor: https://github.com/TDKorn/sphinx-github-style/blob/v1.0.0/sphinx_github_style/meth_lexer.py#L28-L43
+.. _.TDKStyle: https://github.com/TDKorn/sphinx-github-style/blob/v1.0.2/sphinx_github_style/github_style.py#L44-L139
+.. |.TDKMethLexer| replace:: TDKMethLexer
+.. _.TDKMethLexer: https://github.com/TDKorn/sphinx-github-style/blob/v1.0.2/sphinx_github_style/meth_lexer.py#L27-L42
 .. |.github_style| replace:: github_style.css
-.. _.github_style: https://github.com/tdkorn/sphinx-github-style/blob/v1.0.0/sphinx_github_style/_static/github_style.css
+.. _.github_style: https://github.com/tdkorn/sphinx-github-style/blob/v1.0.2/sphinx_github_style/_static/github_style.css
 .. |RTD| replace:: ReadTheDocs
 .. _RTD: https://sphinx-github-style.readthedocs.io/en/latest/
 .. |Note| replace:: 📝 **Note**
 .. |docs| replace:: **Explore the docs »**
 .. _docs: https://sphinx-github-style.readthedocs.io/en/latest/
 
 
@@ -217,15 +217,15 @@
 
 |
 
 Noteworthy Components
 ~~~~~~~~~~~~~~~~~~~~~
 
 * |.TDKStyle|_ - Pygments Style for syntax highlighting similar to Github Pretty Lights Dark Theme
-* |.TDKMethLexor|_ - Pygments Lexor to add syntax highlighting to methods
+* |.TDKMethLexer|_ - Pygments Lexor to add syntax highlighting to methods
 * |.get_linkcode_resolve|_ - to link to GitHub source code using ``sphinx.ext.linkcode``
 * |.add_linkcode_node_class|_ - adds a new ``linkcode-link`` class, allowing for CSS styling separately from ``viewcode`` links
 * |.github_style|_ - CSS styling for linkcode links (icon + text)
 
 |
 
 Documentation
```

