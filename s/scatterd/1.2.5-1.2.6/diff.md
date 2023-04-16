# Comparing `tmp/scatterd-1.2.5.tar.gz` & `tmp/scatterd-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scatterd-1.2.5.tar", last modified: Wed Jan 11 19:16:52 2023, max compression
+gzip compressed data, was "scatterd-1.2.6.tar", last modified: Sun Apr 16 18:57:57 2023, max compression
```

## Comparing `scatterd-1.2.5.tar` & `scatterd-1.2.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-01-11 19:16:52.300923 scatterd-1.2.5/
--rw-rw-rw-   0        0        0     1121 2021-11-13 12:45:24.000000 scatterd-1.2.5/LICENSE
--rw-rw-rw-   0        0        0      115 2021-11-13 12:45:24.000000 scatterd-1.2.5/MANIFEST.in
--rw-rw-rw-   0        0        0     5035 2023-01-11 19:16:52.300923 scatterd-1.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     4451 2022-12-19 19:17:15.000000 scatterd-1.2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-01-11 19:16:52.266017 scatterd-1.2.5/scatterd/
--rw-rw-rw-   0        0        0     1473 2023-01-11 19:14:34.000000 scatterd-1.2.5/scatterd/__init__.py
--rw-rw-rw-   0        0        0     2194 2023-01-09 21:37:10.000000 scatterd-1.2.5/scatterd/examples.py
--rw-rw-rw-   0        0        0    14804 2023-01-11 19:12:34.000000 scatterd-1.2.5/scatterd/scatterd.py
-drwxrwxrwx   0        0        0        0 2023-01-11 19:16:52.299927 scatterd-1.2.5/scatterd.egg-info/
--rw-rw-rw-   0        0        0     5035 2023-01-11 19:16:51.000000 scatterd-1.2.5/scatterd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-01-11 19:16:52.000000 scatterd-1.2.5/scatterd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-11 19:16:51.000000 scatterd-1.2.5/scatterd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-01-11 19:16:51.000000 scatterd-1.2.5/scatterd.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-01-11 19:16:51.000000 scatterd-1.2.5/scatterd.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      259 2023-01-11 19:16:52.304920 scatterd-1.2.5/setup.cfg
--rw-rw-rw-   0        0        0     1411 2022-11-01 20:52:58.000000 scatterd-1.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 18:57:57.455701 scatterd-1.2.6/
+-rw-rw-rw-   0        0        0     1121 2021-11-13 12:45:24.000000 scatterd-1.2.6/LICENSE
+-rw-rw-rw-   0        0        0      115 2021-11-13 12:45:24.000000 scatterd-1.2.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     4994 2023-04-16 18:57:57.455701 scatterd-1.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4451 2022-12-19 19:17:15.000000 scatterd-1.2.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-16 18:57:57.414851 scatterd-1.2.6/scatterd/
+-rw-rw-rw-   0        0        0     1473 2023-04-16 18:57:13.000000 scatterd-1.2.6/scatterd/__init__.py
+-rw-rw-rw-   0        0        0     2194 2023-01-09 21:37:10.000000 scatterd-1.2.6/scatterd/examples.py
+-rw-rw-rw-   0        0        0    15201 2023-04-16 18:10:29.000000 scatterd-1.2.6/scatterd/scatterd.py
+drwxrwxrwx   0        0        0        0 2023-04-16 18:57:57.454735 scatterd-1.2.6/scatterd.egg-info/
+-rw-rw-rw-   0        0        0     4994 2023-04-16 18:57:57.000000 scatterd-1.2.6/scatterd.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-04-16 18:57:57.000000 scatterd-1.2.6/scatterd.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 18:57:57.000000 scatterd-1.2.6/scatterd.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-04-16 18:57:57.000000 scatterd-1.2.6/scatterd.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-16 18:57:57.000000 scatterd-1.2.6/scatterd.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      259 2023-04-16 18:57:57.461685 scatterd-1.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     1411 2022-11-01 20:52:58.000000 scatterd-1.2.6/setup.py
```

### Comparing `scatterd-1.2.5/LICENSE` & `scatterd-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `scatterd-1.2.5/PKG-INFO` & `scatterd-1.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: scatterd
-Version: 1.2.5
+Version: 1.2.6
 Summary: scatterd is an easy and fast way of creating scatter plots.
 Home-page: https://erdogant.github.io/scatterd
-Download-URL: https://github.com/erdogant/scatterd/archive/1.2.5.tar.gz
+Download-URL: https://github.com/erdogant/scatterd/archive/1.2.6.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -112,9 +110,7 @@
 
 	* Become a Sponsor!
 	* Star this repo at the github page.
 	* Other contributions can be in the form of feature requests, idea discussions, reporting bugs, opening pull requests.
 	* Read more why becoming an sponsor is important on the Sponsor Github Page.
 	
 	Cheers Mate.
-
-
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: scatterd Version: 1.2.5 Summary: scatterd is an
+Metadata-Version: 2.1 Name: scatterd Version: 1.2.6 Summary: scatterd is an
 easy and fast way of creating scatter plots. Home-page: https://
 erdogant.github.io/scatterd Download-URL: https://github.com/erdogant/scatterd/
-archive/1.2.5.tar.gz Author: Erdogan Taskesen Author-email: erdogant@gmail.com
-License: UNKNOWN Platform: UNKNOWN Classifier: Programming Language :: Python
-:: 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
-System :: OS Independent Requires-Python: >=3 Description-Content-Type: text/
-markdown License-File: LICENSE # scatterd [![Python](https://img.shields.io/
-pypi/pyversions/scatterd)](https://img.shields.io/pypi/pyversions/scatterd) [!
-[Pypi](https://img.shields.io/pypi/v/scatterd)](https://pypi.org/project/
-scatterd/) [![Docs](https://img.shields.io/badge/Sphinx-Docs-Green)](https://
-erdogant.github.io/scatterd/) [![LOC](https://sloc.xyz/github/erdogant/
-scatterd/?category=code)](https://github.com/erdogant/scatterd/) [![Downloads]
-(https://static.pepy.tech/personalized-badge/
+archive/1.2.6.tar.gz Author: Erdogan Taskesen Author-email: erdogant@gmail.com
+Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
+Approved :: MIT License Classifier: Operating System :: OS Independent
+Requires-Python: >=3 Description-Content-Type: text/markdown License-File:
+LICENSE # scatterd [![Python](https://img.shields.io/pypi/pyversions/scatterd)]
+(https://img.shields.io/pypi/pyversions/scatterd) [![Pypi](https://
+img.shields.io/pypi/v/scatterd)](https://pypi.org/project/scatterd/) [![Docs]
+(https://img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/
+scatterd/) [![LOC](https://sloc.xyz/github/erdogant/scatterd/?category=code)]
+(https://github.com/erdogant/scatterd/) [![Downloads](https://static.pepy.tech/
+personalized-badge/
 scatterd?period=month&units=international_system&left_color=grey&right_color=brightgreen&left_text=PyPI%20downloads/
 month)](https://pepy.tech/project/scatterd) [![Downloads](https://
 static.pepy.tech/personalized-badge/
 scatterd?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)]
 (https://pepy.tech/project/scatterd) [![License](https://img.shields.io/badge/
 license-MIT-green.svg)](https://github.com/erdogant/scatterd/blob/master/
 LICENSE) [![Forks](https://img.shields.io/github/forks/erdogant/scatterd.svg)]
```

### Comparing `scatterd-1.2.5/README.md` & `scatterd-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `scatterd-1.2.5/scatterd/__init__.py` & `scatterd-1.2.6/scatterd/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from scatterd.scatterd import scatterd,import_example, set_colors, _preprocessing, gradient_on_density_color
 
 __author__ = 'Erdogan Tasksen'
 __email__ = 'erdogant@gmail.com'
-__version__ = '1.2.5'
+__version__ = '1.2.6'
 
 # module level doc-string
 __doc__ = """
 scatterd
 =====================================================================
 
 Description
```

### Comparing `scatterd-1.2.5/scatterd/examples.py` & `scatterd-1.2.6/scatterd/examples.py`

 * *Files identical despite different names*

### Comparing `scatterd-1.2.5/scatterd/scatterd.py` & `scatterd-1.2.6/scatterd/scatterd.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
              gradient=None,
              density=False,
              norm=False,
              cmap='Set1',
              figsize=(25, 15),
              legend=True,
              ax=None,
+             jitter=None,
              xlabel='x-axis', ylabel='y-axis', title='', fontsize=24, fontcolor=None, axiscolor='#dddddd',
              args_density = {'cmap': 'Reds', 'shade': True, 'thresh': 0.05, 'bw_adjust': .6, 'alpha': 0.66, 'legend': False, 'cbar': False, 'fill': True}):
     """Make scaterplot.
 
     Parameters
     ----------
     x : numpy array
@@ -65,14 +66,18 @@
     fontsize : String, optional
         The fontsize of the y labels that are plotted in the graph. The default is 16.
     fontcolor: list/array of RGB colors with same size as X (default : None)
         None : Use same colorscheme as for c
         [0,0,0] : If the input is a single color, all fonts will get this color.
     norm : Bool, optional
         Normalize datapoints. The default is False.
+    legend : bool, (default: False)
+        Plot the legend.
+    jitter : float, default: None
+        Add jitter to data points as random normal data. Values of 0.01 is usually good for one-hot data seperation.
     cmap : String, optional
         'Set1'       (default)
         'Set2'
         'rainbow'
         'bwr'        Blue-white-red
         'binary' or 'binary_r'
         'seismic'    Blue-white-red
@@ -132,14 +137,19 @@
     if not isinstance(s, int) and len(s)!=len(x): raise Exception('[scatterd] >Error: input parameter s(ize) should be of same size of X.')
     if (z is not None) and len(x)!=len(z): raise Exception('[scatterd] >Error: input parameter z should be the same size of x and y.')
 
     # Defaults
     defaults_kde = {'cmap': 'Reds', 'shade': True, 'thresh': 0.05, 'bw_adjust': .6, 'alpha': 0.66, 'legend': False, 'cbar': False, 'fill': True}
     args_density = {**defaults_kde, **args_density}
 
+    # Add jitter
+    if jitter is not None:
+        x = x + np.random.normal(0, jitter, size=1)
+        y = y + np.random.normal(0, jitter, size=1)
+
     # Preprocessing
     X, labels = _preprocessing(x, y, z, labels, norm)
 
     # Figure properties
     c_rgb, fontcolor = set_colors(X, labels, fontcolor, c, cmap, gradient=gradient)
 
     if s is None:
```

### Comparing `scatterd-1.2.5/scatterd.egg-info/PKG-INFO` & `scatterd-1.2.6/scatterd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: scatterd
-Version: 1.2.5
+Version: 1.2.6
 Summary: scatterd is an easy and fast way of creating scatter plots.
 Home-page: https://erdogant.github.io/scatterd
-Download-URL: https://github.com/erdogant/scatterd/archive/1.2.5.tar.gz
+Download-URL: https://github.com/erdogant/scatterd/archive/1.2.6.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -112,9 +110,7 @@
 
 	* Become a Sponsor!
 	* Star this repo at the github page.
 	* Other contributions can be in the form of feature requests, idea discussions, reporting bugs, opening pull requests.
 	* Read more why becoming an sponsor is important on the Sponsor Github Page.
 	
 	Cheers Mate.
-
-
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: scatterd Version: 1.2.5 Summary: scatterd is an
+Metadata-Version: 2.1 Name: scatterd Version: 1.2.6 Summary: scatterd is an
 easy and fast way of creating scatter plots. Home-page: https://
 erdogant.github.io/scatterd Download-URL: https://github.com/erdogant/scatterd/
-archive/1.2.5.tar.gz Author: Erdogan Taskesen Author-email: erdogant@gmail.com
-License: UNKNOWN Platform: UNKNOWN Classifier: Programming Language :: Python
-:: 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
-System :: OS Independent Requires-Python: >=3 Description-Content-Type: text/
-markdown License-File: LICENSE # scatterd [![Python](https://img.shields.io/
-pypi/pyversions/scatterd)](https://img.shields.io/pypi/pyversions/scatterd) [!
-[Pypi](https://img.shields.io/pypi/v/scatterd)](https://pypi.org/project/
-scatterd/) [![Docs](https://img.shields.io/badge/Sphinx-Docs-Green)](https://
-erdogant.github.io/scatterd/) [![LOC](https://sloc.xyz/github/erdogant/
-scatterd/?category=code)](https://github.com/erdogant/scatterd/) [![Downloads]
-(https://static.pepy.tech/personalized-badge/
+archive/1.2.6.tar.gz Author: Erdogan Taskesen Author-email: erdogant@gmail.com
+Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
+Approved :: MIT License Classifier: Operating System :: OS Independent
+Requires-Python: >=3 Description-Content-Type: text/markdown License-File:
+LICENSE # scatterd [![Python](https://img.shields.io/pypi/pyversions/scatterd)]
+(https://img.shields.io/pypi/pyversions/scatterd) [![Pypi](https://
+img.shields.io/pypi/v/scatterd)](https://pypi.org/project/scatterd/) [![Docs]
+(https://img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/
+scatterd/) [![LOC](https://sloc.xyz/github/erdogant/scatterd/?category=code)]
+(https://github.com/erdogant/scatterd/) [![Downloads](https://static.pepy.tech/
+personalized-badge/
 scatterd?period=month&units=international_system&left_color=grey&right_color=brightgreen&left_text=PyPI%20downloads/
 month)](https://pepy.tech/project/scatterd) [![Downloads](https://
 static.pepy.tech/personalized-badge/
 scatterd?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)]
 (https://pepy.tech/project/scatterd) [![License](https://img.shields.io/badge/
 license-MIT-green.svg)](https://github.com/erdogant/scatterd/blob/master/
 LICENSE) [![Forks](https://img.shields.io/github/forks/erdogant/scatterd.svg)]
```

### Comparing `scatterd-1.2.5/setup.py` & `scatterd-1.2.6/setup.py`

 * *Files identical despite different names*

