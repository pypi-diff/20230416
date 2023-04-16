# Comparing `tmp/hassle-2.5.0.tar.gz` & `tmp/hassle-2.6.0.tar.gz`

## Comparing `hassle-2.5.0.tar` & `hassle-2.6.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 hassle-2.5.0/CHANGELOG.md
--rw-r--r--   0        0        0    33936 2020-02-02 00:00:00.000000 hassle-2.5.0/docs/hassle.html
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 hassle-2.5.0/docs/index.html
--rw-r--r--   0        0        0    41427 2020-02-02 00:00:00.000000 hassle-2.5.0/docs/search.js
--rw-r--r--   0        0        0    93051 2020-02-02 00:00:00.000000 hassle-2.5.0/docs/hassle/generate_tests.html
--rw-r--r--   0        0        0   121512 2020-02-02 00:00:00.000000 hassle-2.5.0/docs/hassle/hassle.html
--rw-r--r--   0        0        0   107599 2020-02-02 00:00:00.000000 hassle-2.5.0/docs/hassle/hassle_config.html
--rw-r--r--   0        0        0   103640 2020-02-02 00:00:00.000000 hassle-2.5.0/docs/hassle/hassle_utilities.html
--rw-r--r--   0        0        0   165766 2020-02-02 00:00:00.000000 hassle-2.5.0/docs/hassle/new_project.html
--rw-r--r--   0        0        0    52052 2020-02-02 00:00:00.000000 hassle-2.5.0/docs/hassle/run_tests.html
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 hassle-2.5.0/src/hassle/.gitignore_template
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 hassle-2.5.0/src/hassle/.vscode_template
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 hassle-2.5.0/src/hassle/README_template.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hassle-2.5.0/src/hassle/__init__.py
--rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 hassle-2.5.0/src/hassle/generate_tests.py
--rw-r--r--   0        0        0     6737 2020-02-02 00:00:00.000000 hassle-2.5.0/src/hassle/hassle.py
--rw-r--r--   0        0        0     5456 2020-02-02 00:00:00.000000 hassle-2.5.0/src/hassle/hassle_config.py
--rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 hassle-2.5.0/src/hassle/hassle_utilities.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 hassle-2.5.0/src/hassle/license_template.txt
--rw-r--r--   0        0        0     9173 2020-02-02 00:00:00.000000 hassle-2.5.0/src/hassle/new_project.py
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 hassle-2.5.0/src/hassle/pyproject_template.toml
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 hassle-2.5.0/src/hassle/run_tests.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 hassle-2.5.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 hassle-2.5.0/LICENSE.txt
--rw-r--r--   0        0        0    22059 2020-02-02 00:00:00.000000 hassle-2.5.0/README.md
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 hassle-2.5.0/pyproject.toml
--rw-r--r--   0        0        0    22508 2020-02-02 00:00:00.000000 hassle-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 hassle-2.6.0/CHANGELOG.md
+-rw-r--r--   0        0        0    33936 2020-02-02 00:00:00.000000 hassle-2.6.0/docs/hassle.html
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 hassle-2.6.0/docs/index.html
+-rw-r--r--   0        0        0    42579 2020-02-02 00:00:00.000000 hassle-2.6.0/docs/search.js
+-rw-r--r--   0        0        0    93051 2020-02-02 00:00:00.000000 hassle-2.6.0/docs/hassle/generate_tests.html
+-rw-r--r--   0        0        0   121512 2020-02-02 00:00:00.000000 hassle-2.6.0/docs/hassle/hassle.html
+-rw-r--r--   0        0        0   107599 2020-02-02 00:00:00.000000 hassle-2.6.0/docs/hassle/hassle_config.html
+-rw-r--r--   0        0        0   112334 2020-02-02 00:00:00.000000 hassle-2.6.0/docs/hassle/hassle_utilities.html
+-rw-r--r--   0        0        0   165766 2020-02-02 00:00:00.000000 hassle-2.6.0/docs/hassle/new_project.html
+-rw-r--r--   0        0        0    52052 2020-02-02 00:00:00.000000 hassle-2.6.0/docs/hassle/run_tests.html
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 hassle-2.6.0/src/hassle/.gitignore_template
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 hassle-2.6.0/src/hassle/.vscode_template
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 hassle-2.6.0/src/hassle/README_template.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hassle-2.6.0/src/hassle/__init__.py
+-rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 hassle-2.6.0/src/hassle/generate_tests.py
+-rw-r--r--   0        0        0     6737 2020-02-02 00:00:00.000000 hassle-2.6.0/src/hassle/hassle.py
+-rw-r--r--   0        0        0     5456 2020-02-02 00:00:00.000000 hassle-2.6.0/src/hassle/hassle_config.py
+-rw-r--r--   0        0        0     5055 2020-02-02 00:00:00.000000 hassle-2.6.0/src/hassle/hassle_utilities.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 hassle-2.6.0/src/hassle/license_template.txt
+-rw-r--r--   0        0        0     9173 2020-02-02 00:00:00.000000 hassle-2.6.0/src/hassle/new_project.py
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 hassle-2.6.0/src/hassle/pyproject_template.toml
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 hassle-2.6.0/src/hassle/run_tests.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 hassle-2.6.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 hassle-2.6.0/LICENSE.txt
+-rw-r--r--   0        0        0    22059 2020-02-02 00:00:00.000000 hassle-2.6.0/README.md
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 hassle-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0    22508 2020-02-02 00:00:00.000000 hassle-2.6.0/PKG-INFO
```

### Comparing `hassle-2.5.0/CHANGELOG.md` & `hassle-2.6.0/CHANGELOG.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,39 @@
 # Changelog
 
-## 2.4.0 (2023-04-07)
+## 2.5.0 (2023-04-15)
+
+#### Fixes
+
+* fix already exist error by switching pathlib to pathier
+#### Refactorings
+
+* replace pathlib, os.chdir, and shutil calls with pathier
+#### Others
+
+* prune dependencies
+
+
+## v2.4.0 (2023-04-07)
 
 #### New Features
 
 * implement manual override for 'tests' location
 * generate_tests cli accepts individual files instead of only directories
 #### Fixes
 
 * add tests_dir.mkdir() to write_placeholders to keep pytest from throwing a fit
 * fix not passing args.tests_dir param to test file generators
 #### Refactorings
 
 * generated test functions will have the form 'test_{function_name}'
+#### Others
+
+* build v2.4.0
+* update changelog
 
 
 ## v2.3.2 (2023-04-02)
 
 #### Refactorings
 
 * install command will always isntall local copy b/c pypi doesn't update fast enough
```

### Comparing `hassle-2.5.0/docs/hassle.html` & `hassle-2.6.0/docs/hassle.html`

 * *Files identical despite different names*

### Comparing `hassle-2.5.0/docs/search.js` & `hassle-2.6.0/docs/search.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -824,14 +824,30 @@
         "modulename": "hassle.hassle_utilities",
         "qualname": "increment_version",
         "kind": "function",
         "doc": "<p>Increment the project.version field in pyproject.toml.</p>\n\n<h6 id=\"parameters\">Parameters</h6>\n\n<ul>\n<li><p><strong>package_path</strong>:  Path to the package/project directory.</p></li>\n<li><p><strong>increment_type</strong>:  One from 'major', 'minor', or 'patch'.</p></li>\n</ul>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">pyproject_path</span><span class=\"p\">:</span> <span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">Pathier</span>, </span><span class=\"param\"><span class=\"n\">increment_type</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
     }, {
+        "fullname": "hassle.hassle_utilities.get_minimum_py_version",
+        "modulename": "hassle.hassle_utilities",
+        "qualname": "get_minimum_py_version",
+        "kind": "function",
+        "doc": "<p>Scan src with vermin and return minimum\npython version.</p>\n",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">src</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">str</span>:</span></span>",
+        "funcdef": "def"
+    }, {
+        "fullname": "hassle.hassle_utilities.get_project_code",
+        "modulename": "hassle.hassle_utilities",
+        "qualname": "get_project_code",
+        "kind": "function",
+        "doc": "<p>Read and return all code from project_path\nas one string.</p>\n",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">project_path</span><span class=\"p\">:</span> <span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">Pathier</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">str</span>:</span></span>",
+        "funcdef": "def"
+    }, {
         "fullname": "hassle.hassle_utilities.update_minimum_python_version",
         "modulename": "hassle.hassle_utilities",
         "qualname": "update_minimum_python_version",
         "kind": "function",
         "doc": "<p>Use vermin to determine the minimum compatible\nPython version and update the corresponding field\nin pyproject.toml.</p>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">pyproject_path</span><span class=\"p\">:</span> <span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">Pathier</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
```

### Comparing `hassle-2.5.0/docs/hassle/generate_tests.html` & `hassle-2.6.0/docs/hassle/generate_tests.html`

 * *Files identical despite different names*

### Comparing `hassle-2.5.0/docs/hassle/hassle.html` & `hassle-2.6.0/docs/hassle/hassle.html`

 * *Files identical despite different names*

### Comparing `hassle-2.5.0/docs/hassle/hassle_config.html` & `hassle-2.6.0/docs/hassle/hassle_config.html`

 * *Files identical despite different names*

### Comparing `hassle-2.5.0/docs/hassle/hassle_utilities.html` & `hassle-2.6.0/docs/hassle/hassle_utilities.html`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,20 @@
 
         <h2>API Documentation</h2>
             <ul class="memberlist">
             <li>
                     <a class="function" href="#increment_version">increment_version</a>
             </li>
             <li>
+                    <a class="function" href="#get_minimum_py_version">get_minimum_py_version</a>
+            </li>
+            <li>
+                    <a class="function" href="#get_project_code">get_project_code</a>
+            </li>
+            <li>
                     <a class="function" href="#update_minimum_python_version">update_minimum_python_version</a>
             </li>
             <li>
                     <a class="function" href="#generate_docs">generate_docs</a>
             </li>
             <li>
                     <a class="function" href="#update_dependencies">update_dependencies</a>
@@ -98,109 +104,124 @@
 </span><span id="L-27"><a href="#L-27"><span class="linenos"> 27</span></a>    <span class="k">elif</span> <span class="n">increment_type</span> <span class="o">==</span> <span class="s2">&quot;patch&quot;</span><span class="p">:</span>
 </span><span id="L-28"><a href="#L-28"><span class="linenos"> 28</span></a>        <span class="n">patch</span> <span class="o">+=</span> <span class="mi">1</span>
 </span><span id="L-29"><a href="#L-29"><span class="linenos"> 29</span></a>    <span class="n">incremented_version</span> <span class="o">=</span> <span class="s2">&quot;.&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">num</span><span class="p">)</span> <span class="k">for</span> <span class="n">num</span> <span class="ow">in</span> <span class="p">[</span><span class="n">major</span><span class="p">,</span> <span class="n">minor</span><span class="p">,</span> <span class="n">patch</span><span class="p">])</span>
 </span><span id="L-30"><a href="#L-30"><span class="linenos"> 30</span></a>    <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">incremented_version</span>
 </span><span id="L-31"><a href="#L-31"><span class="linenos"> 31</span></a>    <span class="n">pyproject_path</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">meta</span><span class="p">)</span>
 </span><span id="L-32"><a href="#L-32"><span class="linenos"> 32</span></a>
 </span><span id="L-33"><a href="#L-33"><span class="linenos"> 33</span></a>
-</span><span id="L-34"><a href="#L-34"><span class="linenos"> 34</span></a><span class="k">def</span> <span class="nf">update_minimum_python_version</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
-</span><span id="L-35"><a href="#L-35"><span class="linenos"> 35</span></a>    <span class="sd">&quot;&quot;&quot;Use vermin to determine the minimum compatible</span>
-</span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a><span class="sd">    Python version and update the corresponding field</span>
-</span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a><span class="sd">    in pyproject.toml.&quot;&quot;&quot;</span>
-</span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a>    <span class="n">project_code</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
-</span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a>        <span class="n">file</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="p">(</span><span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span> <span class="o">/</span> <span class="s2">&quot;src&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.py&quot;</span><span class="p">)</span>
-</span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a>    <span class="p">)</span>
-</span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a>    <span class="n">meta</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">loads</span><span class="p">()</span>
-</span><span id="L-42"><a href="#L-42"><span class="linenos"> 42</span></a>    <span class="n">minimum_version</span> <span class="o">=</span> <span class="n">vermin</span><span class="o">.</span><span class="n">visit</span><span class="p">(</span><span class="n">project_code</span><span class="p">,</span> <span class="n">vermin</span><span class="o">.</span><span class="n">Config</span><span class="p">())</span><span class="o">.</span><span class="n">minimum_versions</span><span class="p">()[</span><span class="mi">1</span><span class="p">]</span>
-</span><span id="L-43"><a href="#L-43"><span class="linenos"> 43</span></a>    <span class="n">minimum_version</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;&gt;=</span><span class="si">{</span><span class="n">minimum_version</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s2">.</span><span class="si">{</span><span class="n">minimum_version</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a>    <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;requires-python&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">minimum_version</span>
-</span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a>    <span class="n">pyproject_path</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">meta</span><span class="p">)</span>
-</span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a>
-</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a>
-</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a><span class="k">def</span> <span class="nf">generate_docs</span><span class="p">(</span><span class="n">package_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
-</span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a>    <span class="sd">&quot;&quot;&quot;Generate project documentation using pdoc.&quot;&quot;&quot;</span>
-</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a>    <span class="k">try</span><span class="p">:</span>
-</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a>        <span class="p">(</span><span class="n">package_path</span> <span class="o">/</span> <span class="s2">&quot;docs&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span>
-</span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a>    <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a>        <span class="k">pass</span>
-</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span>
-</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a>        <span class="sa">f</span><span class="s2">&quot;pdoc -o </span><span class="si">{</span><span class="n">package_path</span> <span class="o">/</span> <span class="s1">&#39;docs&#39;</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">package_path</span> <span class="o">/</span> <span class="s1">&#39;src&#39;</span> <span class="o">/</span> <span class="n">package_path</span><span class="o">.</span><span class="n">stem</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a>    <span class="p">)</span>
-</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a>
-</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a>
-</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a><span class="k">def</span> <span class="nf">update_dependencies</span><span class="p">(</span>
-</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a>    <span class="n">pyproject_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">overwrite</span><span class="p">:</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">include_versions</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a><span class="p">):</span>
-</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a>    <span class="sd">&quot;&quot;&quot;Update dependencies list in pyproject.toml.</span>
-</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a>
-</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a><span class="sd">    :param overwrite: If True, replace the dependencies in pyproject.toml</span>
-</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a><span class="sd">    with the results of packagelister.scan() .</span>
-</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a><span class="sd">    If False, packages returned by packagelister are appended to</span>
-</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a><span class="sd">    the current dependencies in pyproject.toml if they don&#39;t already</span>
-</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a><span class="sd">    exist in the field.&quot;&quot;&quot;</span>
-</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="n">packagelister</span><span class="o">.</span><span class="n">scan</span><span class="p">(</span><span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span><span class="p">)</span>
-</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a>
-</span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a>        <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}</span><span class="s2">~=</span><span class="si">{</span><span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s1">&#39;version&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a>        <span class="k">if</span> <span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span> <span class="ow">and</span> <span class="n">include_versions</span>
-</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a>        <span class="k">else</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a>        <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span>
-</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a>        <span class="k">if</span> <span class="n">package</span> <span class="o">!=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">stem</span>
-</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a>    <span class="p">]</span>
-</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a>        <span class="n">package</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;speech_recognition&quot;</span><span class="p">,</span> <span class="s2">&quot;speechRecognition&quot;</span><span class="p">)</span>
-</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a>        <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span>
-</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a>    <span class="p">]</span>
-</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a>    <span class="n">meta</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">loads</span><span class="p">()</span>
-</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a>    <span class="k">if</span> <span class="n">overwrite</span><span class="p">:</span>
-</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a>        <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;dependencies&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">packages</span>
-</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a>    <span class="k">else</span><span class="p">:</span>
-</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>        <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span><span class="p">:</span>
-</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>            <span class="k">if</span> <span class="s2">&quot;~&quot;</span> <span class="ow">in</span> <span class="n">package</span><span class="p">:</span>
-</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>                <span class="n">name</span> <span class="o">=</span> <span class="n">package</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;~&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>            <span class="k">elif</span> <span class="s2">&quot;=&quot;</span> <span class="ow">in</span> <span class="n">package</span><span class="p">:</span>
-</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>                <span class="n">name</span> <span class="o">=</span> <span class="n">package</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;=&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a>                <span class="n">name</span> <span class="o">=</span> <span class="n">package</span>
-</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a>            <span class="k">if</span> <span class="nb">all</span><span class="p">(</span>
-</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a>                <span class="n">name</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">dependency</span> <span class="k">for</span> <span class="n">dependency</span> <span class="ow">in</span> <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;dependencies&quot;</span><span class="p">]</span>
-</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>            <span class="p">):</span>
-</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a>                <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;dependencies&quot;</span><span class="p">]</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">package</span><span class="p">)</span>
-</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a>    <span class="n">pyproject_path</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">meta</span><span class="p">)</span>
-</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>
-</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a>
-</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a><span class="k">def</span> <span class="nf">update_changelog</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
-</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>    <span class="sd">&quot;&quot;&quot;Update project changelog.&quot;&quot;&quot;</span>
-</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>    <span class="n">meta</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">loads</span><span class="p">()</span>
-</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>    <span class="k">if</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">config_exists</span><span class="p">():</span>
-</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>        <span class="n">config</span> <span class="o">=</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">load_config</span><span class="p">()</span>
-</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>    <span class="k">else</span><span class="p">:</span>
-</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>        <span class="n">hassle_config</span><span class="o">.</span><span class="n">warn</span><span class="p">()</span>
-</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Creating blank hassle_config.toml...&quot;</span><span class="p">)</span>
-</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>        <span class="n">config</span> <span class="o">=</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">load_config</span><span class="p">()</span>
-</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>    <span class="n">changelog_path</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span> <span class="o">/</span> <span class="s2">&quot;CHANGELOG.md&quot;</span>
-</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span>
-</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>        <span class="sa">f</span><span class="s2">&quot;auto-changelog -p </span><span class="si">{</span><span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span><span class="si">}</span><span class="s2"> --tag-prefix </span><span class="si">{</span><span class="n">config</span><span class="p">[</span><span class="s1">&#39;git&#39;</span><span class="p">][</span><span class="s1">&#39;tag_prefix&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2"> --unreleased -v </span><span class="si">{</span><span class="n">meta</span><span class="p">[</span><span class="s1">&#39;project&#39;</span><span class="p">][</span><span class="s1">&#39;version&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2"> -o </span><span class="si">{</span><span class="n">changelog_path</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>    <span class="p">)</span>
-</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>    <span class="n">changelog</span> <span class="o">=</span> <span class="n">changelog_path</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span><span class="o">.</span><span class="n">splitlines</span><span class="p">()</span>
-</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>    <span class="n">changelog</span> <span class="o">=</span> <span class="p">[</span><span class="n">line</span> <span class="k">for</span> <span class="n">line</span> <span class="ow">in</span> <span class="n">changelog</span> <span class="k">if</span> <span class="s2">&quot;Full set of changes:&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">line</span><span class="p">]</span>
-</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>    <span class="n">changelog_path</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">changelog</span><span class="p">))</span>
-</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>
-</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>
-</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a><span class="k">def</span> <span class="nf">tag_version</span><span class="p">(</span><span class="n">package_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
-</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>    <span class="sd">&quot;&quot;&quot;Add a git tag corresponding</span>
-</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a><span class="sd">    to the version number in pyproject.toml.&quot;&quot;&quot;</span>
-</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>    <span class="k">if</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">config_exists</span><span class="p">():</span>
-</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>        <span class="n">tag_prefix</span> <span class="o">=</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">load_config</span><span class="p">()[</span><span class="s2">&quot;git&quot;</span><span class="p">][</span><span class="s2">&quot;tag_prefix&quot;</span><span class="p">]</span>
-</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>    <span class="k">else</span><span class="p">:</span>
-</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>        <span class="n">hassle_config</span><span class="o">.</span><span class="n">warn</span><span class="p">()</span>
-</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>        <span class="n">tag_prefix</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>    <span class="n">version</span> <span class="o">=</span> <span class="p">(</span><span class="n">package_path</span> <span class="o">/</span> <span class="s2">&quot;pyproject.toml&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">loads</span><span class="p">()[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span>
-</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">package_path</span><span class="p">)</span>
-</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;git tag </span><span class="si">{</span><span class="n">tag_prefix</span><span class="si">}{</span><span class="n">version</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-34"><a href="#L-34"><span class="linenos"> 34</span></a><span class="k">def</span> <span class="nf">get_minimum_py_version</span><span class="p">(</span><span class="n">src</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="L-35"><a href="#L-35"><span class="linenos"> 35</span></a>    <span class="sd">&quot;&quot;&quot;Scan src with vermin and return minimum</span>
+</span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a><span class="sd">    python version.&quot;&quot;&quot;</span>
+</span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a>    <span class="n">config</span> <span class="o">=</span> <span class="n">vermin</span><span class="o">.</span><span class="n">Config</span><span class="p">()</span>
+</span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a>    <span class="n">config</span><span class="o">.</span><span class="n">add_backport</span><span class="p">(</span><span class="s2">&quot;typing&quot;</span><span class="p">)</span>
+</span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a>    <span class="n">config</span><span class="o">.</span><span class="n">add_backport</span><span class="p">(</span><span class="s2">&quot;typing_extensions&quot;</span><span class="p">)</span>
+</span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a>    <span class="n">config</span><span class="o">.</span><span class="n">set_eval_annotations</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span>
+</span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a>    <span class="n">result</span> <span class="o">=</span> <span class="n">vermin</span><span class="o">.</span><span class="n">visit</span><span class="p">(</span><span class="n">src</span><span class="p">,</span> <span class="n">config</span><span class="p">)</span><span class="o">.</span><span class="n">minimum_versions</span><span class="p">()[</span><span class="mi">1</span><span class="p">]</span>
+</span><span id="L-42"><a href="#L-42"><span class="linenos"> 42</span></a>    <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">result</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s2">.</span><span class="si">{</span><span class="n">result</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-43"><a href="#L-43"><span class="linenos"> 43</span></a>
+</span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a>
+</span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a><span class="k">def</span> <span class="nf">get_project_code</span><span class="p">(</span><span class="n">project_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a>    <span class="sd">&quot;&quot;&quot;Read and return all code from project_path</span>
+</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a><span class="sd">    as one string.&quot;&quot;&quot;</span>
+</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a>    <span class="k">return</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">file</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">project_path</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.py&quot;</span><span class="p">))</span>
+</span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a>
+</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a>
+</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a><span class="k">def</span> <span class="nf">update_minimum_python_version</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
+</span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a>    <span class="sd">&quot;&quot;&quot;Use vermin to determine the minimum compatible</span>
+</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a><span class="sd">    Python version and update the corresponding field</span>
+</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a><span class="sd">    in pyproject.toml.&quot;&quot;&quot;</span>
+</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a>    <span class="n">project_code</span> <span class="o">=</span> <span class="n">get_project_code</span><span class="p">(</span><span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span> <span class="o">/</span> <span class="s2">&quot;src&quot;</span><span class="p">)</span>
+</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a>    <span class="n">meta</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">loads</span><span class="p">()</span>
+</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a>    <span class="n">minimum_version</span> <span class="o">=</span> <span class="n">get_minimum_py_version</span><span class="p">(</span><span class="n">project_code</span><span class="p">)</span>
+</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a>    <span class="n">minimum_version</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;&gt;=</span><span class="si">{</span><span class="n">minimum_version</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a>    <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;requires-python&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">minimum_version</span>
+</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a>    <span class="n">pyproject_path</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">meta</span><span class="p">)</span>
+</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a>
+</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a>
+</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a><span class="k">def</span> <span class="nf">generate_docs</span><span class="p">(</span><span class="n">package_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
+</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a>    <span class="sd">&quot;&quot;&quot;Generate project documentation using pdoc.&quot;&quot;&quot;</span>
+</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a>    <span class="k">try</span><span class="p">:</span>
+</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a>        <span class="p">(</span><span class="n">package_path</span> <span class="o">/</span> <span class="s2">&quot;docs&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span>
+</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a>    <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a>        <span class="k">pass</span>
+</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span>
+</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a>        <span class="sa">f</span><span class="s2">&quot;pdoc -o </span><span class="si">{</span><span class="n">package_path</span> <span class="o">/</span> <span class="s1">&#39;docs&#39;</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">package_path</span> <span class="o">/</span> <span class="s1">&#39;src&#39;</span> <span class="o">/</span> <span class="n">package_path</span><span class="o">.</span><span class="n">stem</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a>    <span class="p">)</span>
+</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a>
+</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a>
+</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a><span class="k">def</span> <span class="nf">update_dependencies</span><span class="p">(</span>
+</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a>    <span class="n">pyproject_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">overwrite</span><span class="p">:</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">include_versions</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a><span class="p">):</span>
+</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a>    <span class="sd">&quot;&quot;&quot;Update dependencies list in pyproject.toml.</span>
+</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a>
+</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a><span class="sd">    :param overwrite: If True, replace the dependencies in pyproject.toml</span>
+</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a><span class="sd">    with the results of packagelister.scan() .</span>
+</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a><span class="sd">    If False, packages returned by packagelister are appended to</span>
+</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a><span class="sd">    the current dependencies in pyproject.toml if they don&#39;t already</span>
+</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a><span class="sd">    exist in the field.&quot;&quot;&quot;</span>
+</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="n">packagelister</span><span class="o">.</span><span class="n">scan</span><span class="p">(</span><span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span><span class="p">)</span>
+</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a>
+</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>        <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}</span><span class="s2">~=</span><span class="si">{</span><span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s1">&#39;version&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>        <span class="k">if</span> <span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span> <span class="ow">and</span> <span class="n">include_versions</span>
+</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>        <span class="k">else</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>        <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span>
+</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>        <span class="k">if</span> <span class="n">package</span> <span class="o">!=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">stem</span>
+</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a>    <span class="p">]</span>
+</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a>        <span class="n">package</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;speech_recognition&quot;</span><span class="p">,</span> <span class="s2">&quot;speechRecognition&quot;</span><span class="p">)</span>
+</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>        <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span>
+</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a>    <span class="p">]</span>
+</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a>    <span class="n">meta</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">loads</span><span class="p">()</span>
+</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>    <span class="k">if</span> <span class="n">overwrite</span><span class="p">:</span>
+</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a>        <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;dependencies&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">packages</span>
+</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>    <span class="k">else</span><span class="p">:</span>
+</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>        <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span><span class="p">:</span>
+</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>            <span class="k">if</span> <span class="s2">&quot;~&quot;</span> <span class="ow">in</span> <span class="n">package</span><span class="p">:</span>
+</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>                <span class="n">name</span> <span class="o">=</span> <span class="n">package</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;~&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>            <span class="k">elif</span> <span class="s2">&quot;=&quot;</span> <span class="ow">in</span> <span class="n">package</span><span class="p">:</span>
+</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>                <span class="n">name</span> <span class="o">=</span> <span class="n">package</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;=&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a>                <span class="n">name</span> <span class="o">=</span> <span class="n">package</span>
+</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>            <span class="k">if</span> <span class="nb">all</span><span class="p">(</span>
+</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>                <span class="n">name</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">dependency</span> <span class="k">for</span> <span class="n">dependency</span> <span class="ow">in</span> <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;dependencies&quot;</span><span class="p">]</span>
+</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>            <span class="p">):</span>
+</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>                <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;dependencies&quot;</span><span class="p">]</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">package</span><span class="p">)</span>
+</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>    <span class="n">pyproject_path</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">meta</span><span class="p">)</span>
+</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>
+</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>
+</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a><span class="k">def</span> <span class="nf">update_changelog</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
+</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>    <span class="sd">&quot;&quot;&quot;Update project changelog.&quot;&quot;&quot;</span>
+</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>    <span class="n">meta</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">loads</span><span class="p">()</span>
+</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>    <span class="k">if</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">config_exists</span><span class="p">():</span>
+</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>        <span class="n">config</span> <span class="o">=</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">load_config</span><span class="p">()</span>
+</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>    <span class="k">else</span><span class="p">:</span>
+</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>        <span class="n">hassle_config</span><span class="o">.</span><span class="n">warn</span><span class="p">()</span>
+</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Creating blank hassle_config.toml...&quot;</span><span class="p">)</span>
+</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>        <span class="n">config</span> <span class="o">=</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">load_config</span><span class="p">()</span>
+</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>    <span class="n">changelog_path</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span> <span class="o">/</span> <span class="s2">&quot;CHANGELOG.md&quot;</span>
+</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span>
+</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>        <span class="sa">f</span><span class="s2">&quot;auto-changelog -p </span><span class="si">{</span><span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span><span class="si">}</span><span class="s2"> --tag-prefix </span><span class="si">{</span><span class="n">config</span><span class="p">[</span><span class="s1">&#39;git&#39;</span><span class="p">][</span><span class="s1">&#39;tag_prefix&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2"> --unreleased -v </span><span class="si">{</span><span class="n">meta</span><span class="p">[</span><span class="s1">&#39;project&#39;</span><span class="p">][</span><span class="s1">&#39;version&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2"> -o </span><span class="si">{</span><span class="n">changelog_path</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a>    <span class="p">)</span>
+</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>    <span class="n">changelog</span> <span class="o">=</span> <span class="n">changelog_path</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span><span class="o">.</span><span class="n">splitlines</span><span class="p">()</span>
+</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a>    <span class="n">changelog</span> <span class="o">=</span> <span class="p">[</span><span class="n">line</span> <span class="k">for</span> <span class="n">line</span> <span class="ow">in</span> <span class="n">changelog</span> <span class="k">if</span> <span class="s2">&quot;Full set of changes:&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">line</span><span class="p">]</span>
+</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a>    <span class="n">changelog_path</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">changelog</span><span class="p">))</span>
+</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a>
+</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a>
+</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a><span class="k">def</span> <span class="nf">tag_version</span><span class="p">(</span><span class="n">package_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
+</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a>    <span class="sd">&quot;&quot;&quot;Add a git tag corresponding</span>
+</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a><span class="sd">    to the version number in pyproject.toml.&quot;&quot;&quot;</span>
+</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>    <span class="k">if</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">config_exists</span><span class="p">():</span>
+</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>        <span class="n">tag_prefix</span> <span class="o">=</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">load_config</span><span class="p">()[</span><span class="s2">&quot;git&quot;</span><span class="p">][</span><span class="s2">&quot;tag_prefix&quot;</span><span class="p">]</span>
+</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>    <span class="k">else</span><span class="p">:</span>
+</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>        <span class="n">hassle_config</span><span class="o">.</span><span class="n">warn</span><span class="p">()</span>
+</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a>        <span class="n">tag_prefix</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>    <span class="n">version</span> <span class="o">=</span> <span class="p">(</span><span class="n">package_path</span> <span class="o">/</span> <span class="s2">&quot;pyproject.toml&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">loads</span><span class="p">()[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span>
+</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">package_path</span><span class="p">)</span>
+</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;git tag </span><span class="si">{</span><span class="n">tag_prefix</span><span class="si">}{</span><span class="n">version</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             </section>
                 <section id="increment_version">
                             <input id="increment_version-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -243,37 +264,88 @@
 <li><p><strong>package_path</strong>:  Path to the package/project directory.</p></li>
 <li><p><strong>increment_type</strong>:  One from 'major', 'minor', or 'patch'.</p></li>
 </ul>
 </div>
 
 
                 </section>
+                <section id="get_minimum_py_version">
+                            <input id="get_minimum_py_version-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+<div class="attr function">
+            
+        <span class="def">def</span>
+        <span class="name">get_minimum_py_version</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">src</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="nb">str</span>:</span></span>
+
+                <label class="view-source-button" for="get_minimum_py_version-view-source"><span>View Source</span></label>
+
+    </div>
+    <a class="headerlink" href="#get_minimum_py_version"></a>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="get_minimum_py_version-35"><a href="#get_minimum_py_version-35"><span class="linenos">35</span></a><span class="k">def</span> <span class="nf">get_minimum_py_version</span><span class="p">(</span><span class="n">src</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="get_minimum_py_version-36"><a href="#get_minimum_py_version-36"><span class="linenos">36</span></a>    <span class="sd">&quot;&quot;&quot;Scan src with vermin and return minimum</span>
+</span><span id="get_minimum_py_version-37"><a href="#get_minimum_py_version-37"><span class="linenos">37</span></a><span class="sd">    python version.&quot;&quot;&quot;</span>
+</span><span id="get_minimum_py_version-38"><a href="#get_minimum_py_version-38"><span class="linenos">38</span></a>    <span class="n">config</span> <span class="o">=</span> <span class="n">vermin</span><span class="o">.</span><span class="n">Config</span><span class="p">()</span>
+</span><span id="get_minimum_py_version-39"><a href="#get_minimum_py_version-39"><span class="linenos">39</span></a>    <span class="n">config</span><span class="o">.</span><span class="n">add_backport</span><span class="p">(</span><span class="s2">&quot;typing&quot;</span><span class="p">)</span>
+</span><span id="get_minimum_py_version-40"><a href="#get_minimum_py_version-40"><span class="linenos">40</span></a>    <span class="n">config</span><span class="o">.</span><span class="n">add_backport</span><span class="p">(</span><span class="s2">&quot;typing_extensions&quot;</span><span class="p">)</span>
+</span><span id="get_minimum_py_version-41"><a href="#get_minimum_py_version-41"><span class="linenos">41</span></a>    <span class="n">config</span><span class="o">.</span><span class="n">set_eval_annotations</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span>
+</span><span id="get_minimum_py_version-42"><a href="#get_minimum_py_version-42"><span class="linenos">42</span></a>    <span class="n">result</span> <span class="o">=</span> <span class="n">vermin</span><span class="o">.</span><span class="n">visit</span><span class="p">(</span><span class="n">src</span><span class="p">,</span> <span class="n">config</span><span class="p">)</span><span class="o">.</span><span class="n">minimum_versions</span><span class="p">()[</span><span class="mi">1</span><span class="p">]</span>
+</span><span id="get_minimum_py_version-43"><a href="#get_minimum_py_version-43"><span class="linenos">43</span></a>    <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">result</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s2">.</span><span class="si">{</span><span class="n">result</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span>
+</span></pre></div>
+
+
+            <div class="docstring"><p>Scan src with vermin and return minimum
+python version.</p>
+</div>
+
+
+                </section>
+                <section id="get_project_code">
+                            <input id="get_project_code-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+<div class="attr function">
+            
+        <span class="def">def</span>
+        <span class="name">get_project_code</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">project_path</span><span class="p">:</span> <span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span></span><span class="return-annotation">) -> <span class="nb">str</span>:</span></span>
+
+                <label class="view-source-button" for="get_project_code-view-source"><span>View Source</span></label>
+
+    </div>
+    <a class="headerlink" href="#get_project_code"></a>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="get_project_code-46"><a href="#get_project_code-46"><span class="linenos">46</span></a><span class="k">def</span> <span class="nf">get_project_code</span><span class="p">(</span><span class="n">project_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="get_project_code-47"><a href="#get_project_code-47"><span class="linenos">47</span></a>    <span class="sd">&quot;&quot;&quot;Read and return all code from project_path</span>
+</span><span id="get_project_code-48"><a href="#get_project_code-48"><span class="linenos">48</span></a><span class="sd">    as one string.&quot;&quot;&quot;</span>
+</span><span id="get_project_code-49"><a href="#get_project_code-49"><span class="linenos">49</span></a>    <span class="k">return</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">file</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">project_path</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.py&quot;</span><span class="p">))</span>
+</span></pre></div>
+
+
+            <div class="docstring"><p>Read and return all code from project_path
+as one string.</p>
+</div>
+
+
+                </section>
                 <section id="update_minimum_python_version">
                             <input id="update_minimum_python_version-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
         <span class="name">update_minimum_python_version</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">pyproject_path</span><span class="p">:</span> <span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="update_minimum_python_version-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#update_minimum_python_version"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="update_minimum_python_version-35"><a href="#update_minimum_python_version-35"><span class="linenos">35</span></a><span class="k">def</span> <span class="nf">update_minimum_python_version</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
-</span><span id="update_minimum_python_version-36"><a href="#update_minimum_python_version-36"><span class="linenos">36</span></a>    <span class="sd">&quot;&quot;&quot;Use vermin to determine the minimum compatible</span>
-</span><span id="update_minimum_python_version-37"><a href="#update_minimum_python_version-37"><span class="linenos">37</span></a><span class="sd">    Python version and update the corresponding field</span>
-</span><span id="update_minimum_python_version-38"><a href="#update_minimum_python_version-38"><span class="linenos">38</span></a><span class="sd">    in pyproject.toml.&quot;&quot;&quot;</span>
-</span><span id="update_minimum_python_version-39"><a href="#update_minimum_python_version-39"><span class="linenos">39</span></a>    <span class="n">project_code</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
-</span><span id="update_minimum_python_version-40"><a href="#update_minimum_python_version-40"><span class="linenos">40</span></a>        <span class="n">file</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="p">(</span><span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span> <span class="o">/</span> <span class="s2">&quot;src&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.py&quot;</span><span class="p">)</span>
-</span><span id="update_minimum_python_version-41"><a href="#update_minimum_python_version-41"><span class="linenos">41</span></a>    <span class="p">)</span>
-</span><span id="update_minimum_python_version-42"><a href="#update_minimum_python_version-42"><span class="linenos">42</span></a>    <span class="n">meta</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">loads</span><span class="p">()</span>
-</span><span id="update_minimum_python_version-43"><a href="#update_minimum_python_version-43"><span class="linenos">43</span></a>    <span class="n">minimum_version</span> <span class="o">=</span> <span class="n">vermin</span><span class="o">.</span><span class="n">visit</span><span class="p">(</span><span class="n">project_code</span><span class="p">,</span> <span class="n">vermin</span><span class="o">.</span><span class="n">Config</span><span class="p">())</span><span class="o">.</span><span class="n">minimum_versions</span><span class="p">()[</span><span class="mi">1</span><span class="p">]</span>
-</span><span id="update_minimum_python_version-44"><a href="#update_minimum_python_version-44"><span class="linenos">44</span></a>    <span class="n">minimum_version</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;&gt;=</span><span class="si">{</span><span class="n">minimum_version</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s2">.</span><span class="si">{</span><span class="n">minimum_version</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="update_minimum_python_version-45"><a href="#update_minimum_python_version-45"><span class="linenos">45</span></a>    <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;requires-python&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">minimum_version</span>
-</span><span id="update_minimum_python_version-46"><a href="#update_minimum_python_version-46"><span class="linenos">46</span></a>    <span class="n">pyproject_path</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">meta</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="update_minimum_python_version-52"><a href="#update_minimum_python_version-52"><span class="linenos">52</span></a><span class="k">def</span> <span class="nf">update_minimum_python_version</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
+</span><span id="update_minimum_python_version-53"><a href="#update_minimum_python_version-53"><span class="linenos">53</span></a>    <span class="sd">&quot;&quot;&quot;Use vermin to determine the minimum compatible</span>
+</span><span id="update_minimum_python_version-54"><a href="#update_minimum_python_version-54"><span class="linenos">54</span></a><span class="sd">    Python version and update the corresponding field</span>
+</span><span id="update_minimum_python_version-55"><a href="#update_minimum_python_version-55"><span class="linenos">55</span></a><span class="sd">    in pyproject.toml.&quot;&quot;&quot;</span>
+</span><span id="update_minimum_python_version-56"><a href="#update_minimum_python_version-56"><span class="linenos">56</span></a>    <span class="n">project_code</span> <span class="o">=</span> <span class="n">get_project_code</span><span class="p">(</span><span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span> <span class="o">/</span> <span class="s2">&quot;src&quot;</span><span class="p">)</span>
+</span><span id="update_minimum_python_version-57"><a href="#update_minimum_python_version-57"><span class="linenos">57</span></a>    <span class="n">meta</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">loads</span><span class="p">()</span>
+</span><span id="update_minimum_python_version-58"><a href="#update_minimum_python_version-58"><span class="linenos">58</span></a>    <span class="n">minimum_version</span> <span class="o">=</span> <span class="n">get_minimum_py_version</span><span class="p">(</span><span class="n">project_code</span><span class="p">)</span>
+</span><span id="update_minimum_python_version-59"><a href="#update_minimum_python_version-59"><span class="linenos">59</span></a>    <span class="n">minimum_version</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;&gt;=</span><span class="si">{</span><span class="n">minimum_version</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="update_minimum_python_version-60"><a href="#update_minimum_python_version-60"><span class="linenos">60</span></a>    <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;requires-python&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">minimum_version</span>
+</span><span id="update_minimum_python_version-61"><a href="#update_minimum_python_version-61"><span class="linenos">61</span></a>    <span class="n">pyproject_path</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">meta</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Use vermin to determine the minimum compatible
 Python version and update the corresponding field
 in pyproject.toml.</p>
 </div>
@@ -287,23 +359,23 @@
         <span class="def">def</span>
         <span class="name">generate_docs</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">package_path</span><span class="p">:</span> <span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="generate_docs-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#generate_docs"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="generate_docs-49"><a href="#generate_docs-49"><span class="linenos">49</span></a><span class="k">def</span> <span class="nf">generate_docs</span><span class="p">(</span><span class="n">package_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
-</span><span id="generate_docs-50"><a href="#generate_docs-50"><span class="linenos">50</span></a>    <span class="sd">&quot;&quot;&quot;Generate project documentation using pdoc.&quot;&quot;&quot;</span>
-</span><span id="generate_docs-51"><a href="#generate_docs-51"><span class="linenos">51</span></a>    <span class="k">try</span><span class="p">:</span>
-</span><span id="generate_docs-52"><a href="#generate_docs-52"><span class="linenos">52</span></a>        <span class="p">(</span><span class="n">package_path</span> <span class="o">/</span> <span class="s2">&quot;docs&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span>
-</span><span id="generate_docs-53"><a href="#generate_docs-53"><span class="linenos">53</span></a>    <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="generate_docs-54"><a href="#generate_docs-54"><span class="linenos">54</span></a>        <span class="k">pass</span>
-</span><span id="generate_docs-55"><a href="#generate_docs-55"><span class="linenos">55</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span>
-</span><span id="generate_docs-56"><a href="#generate_docs-56"><span class="linenos">56</span></a>        <span class="sa">f</span><span class="s2">&quot;pdoc -o </span><span class="si">{</span><span class="n">package_path</span> <span class="o">/</span> <span class="s1">&#39;docs&#39;</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">package_path</span> <span class="o">/</span> <span class="s1">&#39;src&#39;</span> <span class="o">/</span> <span class="n">package_path</span><span class="o">.</span><span class="n">stem</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="generate_docs-57"><a href="#generate_docs-57"><span class="linenos">57</span></a>    <span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="generate_docs-64"><a href="#generate_docs-64"><span class="linenos">64</span></a><span class="k">def</span> <span class="nf">generate_docs</span><span class="p">(</span><span class="n">package_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
+</span><span id="generate_docs-65"><a href="#generate_docs-65"><span class="linenos">65</span></a>    <span class="sd">&quot;&quot;&quot;Generate project documentation using pdoc.&quot;&quot;&quot;</span>
+</span><span id="generate_docs-66"><a href="#generate_docs-66"><span class="linenos">66</span></a>    <span class="k">try</span><span class="p">:</span>
+</span><span id="generate_docs-67"><a href="#generate_docs-67"><span class="linenos">67</span></a>        <span class="p">(</span><span class="n">package_path</span> <span class="o">/</span> <span class="s2">&quot;docs&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span>
+</span><span id="generate_docs-68"><a href="#generate_docs-68"><span class="linenos">68</span></a>    <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="generate_docs-69"><a href="#generate_docs-69"><span class="linenos">69</span></a>        <span class="k">pass</span>
+</span><span id="generate_docs-70"><a href="#generate_docs-70"><span class="linenos">70</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span>
+</span><span id="generate_docs-71"><a href="#generate_docs-71"><span class="linenos">71</span></a>        <span class="sa">f</span><span class="s2">&quot;pdoc -o </span><span class="si">{</span><span class="n">package_path</span> <span class="o">/</span> <span class="s1">&#39;docs&#39;</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">package_path</span> <span class="o">/</span> <span class="s1">&#39;src&#39;</span> <span class="o">/</span> <span class="n">package_path</span><span class="o">.</span><span class="n">stem</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="generate_docs-72"><a href="#generate_docs-72"><span class="linenos">72</span></a>    <span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Generate project documentation using pdoc.</p>
 </div>
 
 
@@ -315,53 +387,53 @@
         <span class="def">def</span>
         <span class="name">update_dependencies</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="n">pyproject_path</span><span class="p">:</span> <span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span>,</span><span class="param">	<span class="n">overwrite</span><span class="p">:</span> <span class="nb">bool</span>,</span><span class="param">	<span class="n">include_versions</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="update_dependencies-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#update_dependencies"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="update_dependencies-60"><a href="#update_dependencies-60"><span class="linenos">60</span></a><span class="k">def</span> <span class="nf">update_dependencies</span><span class="p">(</span>
-</span><span id="update_dependencies-61"><a href="#update_dependencies-61"><span class="linenos">61</span></a>    <span class="n">pyproject_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">overwrite</span><span class="p">:</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">include_versions</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="update_dependencies-62"><a href="#update_dependencies-62"><span class="linenos">62</span></a><span class="p">):</span>
-</span><span id="update_dependencies-63"><a href="#update_dependencies-63"><span class="linenos">63</span></a>    <span class="sd">&quot;&quot;&quot;Update dependencies list in pyproject.toml.</span>
-</span><span id="update_dependencies-64"><a href="#update_dependencies-64"><span class="linenos">64</span></a>
-</span><span id="update_dependencies-65"><a href="#update_dependencies-65"><span class="linenos">65</span></a><span class="sd">    :param overwrite: If True, replace the dependencies in pyproject.toml</span>
-</span><span id="update_dependencies-66"><a href="#update_dependencies-66"><span class="linenos">66</span></a><span class="sd">    with the results of packagelister.scan() .</span>
-</span><span id="update_dependencies-67"><a href="#update_dependencies-67"><span class="linenos">67</span></a><span class="sd">    If False, packages returned by packagelister are appended to</span>
-</span><span id="update_dependencies-68"><a href="#update_dependencies-68"><span class="linenos">68</span></a><span class="sd">    the current dependencies in pyproject.toml if they don&#39;t already</span>
-</span><span id="update_dependencies-69"><a href="#update_dependencies-69"><span class="linenos">69</span></a><span class="sd">    exist in the field.&quot;&quot;&quot;</span>
-</span><span id="update_dependencies-70"><a href="#update_dependencies-70"><span class="linenos">70</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="n">packagelister</span><span class="o">.</span><span class="n">scan</span><span class="p">(</span><span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span><span class="p">)</span>
-</span><span id="update_dependencies-71"><a href="#update_dependencies-71"><span class="linenos">71</span></a>
-</span><span id="update_dependencies-72"><a href="#update_dependencies-72"><span class="linenos">72</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="update_dependencies-73"><a href="#update_dependencies-73"><span class="linenos">73</span></a>        <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}</span><span class="s2">~=</span><span class="si">{</span><span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s1">&#39;version&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="update_dependencies-74"><a href="#update_dependencies-74"><span class="linenos">74</span></a>        <span class="k">if</span> <span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span> <span class="ow">and</span> <span class="n">include_versions</span>
-</span><span id="update_dependencies-75"><a href="#update_dependencies-75"><span class="linenos">75</span></a>        <span class="k">else</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="update_dependencies-76"><a href="#update_dependencies-76"><span class="linenos">76</span></a>        <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span>
-</span><span id="update_dependencies-77"><a href="#update_dependencies-77"><span class="linenos">77</span></a>        <span class="k">if</span> <span class="n">package</span> <span class="o">!=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">stem</span>
-</span><span id="update_dependencies-78"><a href="#update_dependencies-78"><span class="linenos">78</span></a>    <span class="p">]</span>
-</span><span id="update_dependencies-79"><a href="#update_dependencies-79"><span class="linenos">79</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="update_dependencies-80"><a href="#update_dependencies-80"><span class="linenos">80</span></a>        <span class="n">package</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;speech_recognition&quot;</span><span class="p">,</span> <span class="s2">&quot;speechRecognition&quot;</span><span class="p">)</span>
-</span><span id="update_dependencies-81"><a href="#update_dependencies-81"><span class="linenos">81</span></a>        <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span>
-</span><span id="update_dependencies-82"><a href="#update_dependencies-82"><span class="linenos">82</span></a>    <span class="p">]</span>
-</span><span id="update_dependencies-83"><a href="#update_dependencies-83"><span class="linenos">83</span></a>    <span class="n">meta</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">loads</span><span class="p">()</span>
-</span><span id="update_dependencies-84"><a href="#update_dependencies-84"><span class="linenos">84</span></a>    <span class="k">if</span> <span class="n">overwrite</span><span class="p">:</span>
-</span><span id="update_dependencies-85"><a href="#update_dependencies-85"><span class="linenos">85</span></a>        <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;dependencies&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">packages</span>
-</span><span id="update_dependencies-86"><a href="#update_dependencies-86"><span class="linenos">86</span></a>    <span class="k">else</span><span class="p">:</span>
-</span><span id="update_dependencies-87"><a href="#update_dependencies-87"><span class="linenos">87</span></a>        <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span><span class="p">:</span>
-</span><span id="update_dependencies-88"><a href="#update_dependencies-88"><span class="linenos">88</span></a>            <span class="k">if</span> <span class="s2">&quot;~&quot;</span> <span class="ow">in</span> <span class="n">package</span><span class="p">:</span>
-</span><span id="update_dependencies-89"><a href="#update_dependencies-89"><span class="linenos">89</span></a>                <span class="n">name</span> <span class="o">=</span> <span class="n">package</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;~&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="update_dependencies-90"><a href="#update_dependencies-90"><span class="linenos">90</span></a>            <span class="k">elif</span> <span class="s2">&quot;=&quot;</span> <span class="ow">in</span> <span class="n">package</span><span class="p">:</span>
-</span><span id="update_dependencies-91"><a href="#update_dependencies-91"><span class="linenos">91</span></a>                <span class="n">name</span> <span class="o">=</span> <span class="n">package</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;=&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="update_dependencies-92"><a href="#update_dependencies-92"><span class="linenos">92</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="update_dependencies-93"><a href="#update_dependencies-93"><span class="linenos">93</span></a>                <span class="n">name</span> <span class="o">=</span> <span class="n">package</span>
-</span><span id="update_dependencies-94"><a href="#update_dependencies-94"><span class="linenos">94</span></a>            <span class="k">if</span> <span class="nb">all</span><span class="p">(</span>
-</span><span id="update_dependencies-95"><a href="#update_dependencies-95"><span class="linenos">95</span></a>                <span class="n">name</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">dependency</span> <span class="k">for</span> <span class="n">dependency</span> <span class="ow">in</span> <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;dependencies&quot;</span><span class="p">]</span>
-</span><span id="update_dependencies-96"><a href="#update_dependencies-96"><span class="linenos">96</span></a>            <span class="p">):</span>
-</span><span id="update_dependencies-97"><a href="#update_dependencies-97"><span class="linenos">97</span></a>                <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;dependencies&quot;</span><span class="p">]</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">package</span><span class="p">)</span>
-</span><span id="update_dependencies-98"><a href="#update_dependencies-98"><span class="linenos">98</span></a>    <span class="n">pyproject_path</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">meta</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="update_dependencies-75"><a href="#update_dependencies-75"><span class="linenos"> 75</span></a><span class="k">def</span> <span class="nf">update_dependencies</span><span class="p">(</span>
+</span><span id="update_dependencies-76"><a href="#update_dependencies-76"><span class="linenos"> 76</span></a>    <span class="n">pyproject_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">overwrite</span><span class="p">:</span> <span class="nb">bool</span><span class="p">,</span> <span class="n">include_versions</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="update_dependencies-77"><a href="#update_dependencies-77"><span class="linenos"> 77</span></a><span class="p">):</span>
+</span><span id="update_dependencies-78"><a href="#update_dependencies-78"><span class="linenos"> 78</span></a>    <span class="sd">&quot;&quot;&quot;Update dependencies list in pyproject.toml.</span>
+</span><span id="update_dependencies-79"><a href="#update_dependencies-79"><span class="linenos"> 79</span></a>
+</span><span id="update_dependencies-80"><a href="#update_dependencies-80"><span class="linenos"> 80</span></a><span class="sd">    :param overwrite: If True, replace the dependencies in pyproject.toml</span>
+</span><span id="update_dependencies-81"><a href="#update_dependencies-81"><span class="linenos"> 81</span></a><span class="sd">    with the results of packagelister.scan() .</span>
+</span><span id="update_dependencies-82"><a href="#update_dependencies-82"><span class="linenos"> 82</span></a><span class="sd">    If False, packages returned by packagelister are appended to</span>
+</span><span id="update_dependencies-83"><a href="#update_dependencies-83"><span class="linenos"> 83</span></a><span class="sd">    the current dependencies in pyproject.toml if they don&#39;t already</span>
+</span><span id="update_dependencies-84"><a href="#update_dependencies-84"><span class="linenos"> 84</span></a><span class="sd">    exist in the field.&quot;&quot;&quot;</span>
+</span><span id="update_dependencies-85"><a href="#update_dependencies-85"><span class="linenos"> 85</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="n">packagelister</span><span class="o">.</span><span class="n">scan</span><span class="p">(</span><span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span><span class="p">)</span>
+</span><span id="update_dependencies-86"><a href="#update_dependencies-86"><span class="linenos"> 86</span></a>
+</span><span id="update_dependencies-87"><a href="#update_dependencies-87"><span class="linenos"> 87</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="update_dependencies-88"><a href="#update_dependencies-88"><span class="linenos"> 88</span></a>        <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}</span><span class="s2">~=</span><span class="si">{</span><span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s1">&#39;version&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="update_dependencies-89"><a href="#update_dependencies-89"><span class="linenos"> 89</span></a>        <span class="k">if</span> <span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span> <span class="ow">and</span> <span class="n">include_versions</span>
+</span><span id="update_dependencies-90"><a href="#update_dependencies-90"><span class="linenos"> 90</span></a>        <span class="k">else</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="update_dependencies-91"><a href="#update_dependencies-91"><span class="linenos"> 91</span></a>        <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span>
+</span><span id="update_dependencies-92"><a href="#update_dependencies-92"><span class="linenos"> 92</span></a>        <span class="k">if</span> <span class="n">package</span> <span class="o">!=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">stem</span>
+</span><span id="update_dependencies-93"><a href="#update_dependencies-93"><span class="linenos"> 93</span></a>    <span class="p">]</span>
+</span><span id="update_dependencies-94"><a href="#update_dependencies-94"><span class="linenos"> 94</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="update_dependencies-95"><a href="#update_dependencies-95"><span class="linenos"> 95</span></a>        <span class="n">package</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;speech_recognition&quot;</span><span class="p">,</span> <span class="s2">&quot;speechRecognition&quot;</span><span class="p">)</span>
+</span><span id="update_dependencies-96"><a href="#update_dependencies-96"><span class="linenos"> 96</span></a>        <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span>
+</span><span id="update_dependencies-97"><a href="#update_dependencies-97"><span class="linenos"> 97</span></a>    <span class="p">]</span>
+</span><span id="update_dependencies-98"><a href="#update_dependencies-98"><span class="linenos"> 98</span></a>    <span class="n">meta</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">loads</span><span class="p">()</span>
+</span><span id="update_dependencies-99"><a href="#update_dependencies-99"><span class="linenos"> 99</span></a>    <span class="k">if</span> <span class="n">overwrite</span><span class="p">:</span>
+</span><span id="update_dependencies-100"><a href="#update_dependencies-100"><span class="linenos">100</span></a>        <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;dependencies&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">packages</span>
+</span><span id="update_dependencies-101"><a href="#update_dependencies-101"><span class="linenos">101</span></a>    <span class="k">else</span><span class="p">:</span>
+</span><span id="update_dependencies-102"><a href="#update_dependencies-102"><span class="linenos">102</span></a>        <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span><span class="p">:</span>
+</span><span id="update_dependencies-103"><a href="#update_dependencies-103"><span class="linenos">103</span></a>            <span class="k">if</span> <span class="s2">&quot;~&quot;</span> <span class="ow">in</span> <span class="n">package</span><span class="p">:</span>
+</span><span id="update_dependencies-104"><a href="#update_dependencies-104"><span class="linenos">104</span></a>                <span class="n">name</span> <span class="o">=</span> <span class="n">package</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;~&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="update_dependencies-105"><a href="#update_dependencies-105"><span class="linenos">105</span></a>            <span class="k">elif</span> <span class="s2">&quot;=&quot;</span> <span class="ow">in</span> <span class="n">package</span><span class="p">:</span>
+</span><span id="update_dependencies-106"><a href="#update_dependencies-106"><span class="linenos">106</span></a>                <span class="n">name</span> <span class="o">=</span> <span class="n">package</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;=&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="update_dependencies-107"><a href="#update_dependencies-107"><span class="linenos">107</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="update_dependencies-108"><a href="#update_dependencies-108"><span class="linenos">108</span></a>                <span class="n">name</span> <span class="o">=</span> <span class="n">package</span>
+</span><span id="update_dependencies-109"><a href="#update_dependencies-109"><span class="linenos">109</span></a>            <span class="k">if</span> <span class="nb">all</span><span class="p">(</span>
+</span><span id="update_dependencies-110"><a href="#update_dependencies-110"><span class="linenos">110</span></a>                <span class="n">name</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">dependency</span> <span class="k">for</span> <span class="n">dependency</span> <span class="ow">in</span> <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;dependencies&quot;</span><span class="p">]</span>
+</span><span id="update_dependencies-111"><a href="#update_dependencies-111"><span class="linenos">111</span></a>            <span class="p">):</span>
+</span><span id="update_dependencies-112"><a href="#update_dependencies-112"><span class="linenos">112</span></a>                <span class="n">meta</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;dependencies&quot;</span><span class="p">]</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">package</span><span class="p">)</span>
+</span><span id="update_dependencies-113"><a href="#update_dependencies-113"><span class="linenos">113</span></a>    <span class="n">pyproject_path</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">meta</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Update dependencies list in pyproject.toml.</p>
 
 <h6 id="parameters">Parameters</h6>
 
@@ -383,30 +455,30 @@
         <span class="def">def</span>
         <span class="name">update_changelog</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">pyproject_path</span><span class="p">:</span> <span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="update_changelog-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#update_changelog"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="update_changelog-101"><a href="#update_changelog-101"><span class="linenos">101</span></a><span class="k">def</span> <span class="nf">update_changelog</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
-</span><span id="update_changelog-102"><a href="#update_changelog-102"><span class="linenos">102</span></a>    <span class="sd">&quot;&quot;&quot;Update project changelog.&quot;&quot;&quot;</span>
-</span><span id="update_changelog-103"><a href="#update_changelog-103"><span class="linenos">103</span></a>    <span class="n">meta</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">loads</span><span class="p">()</span>
-</span><span id="update_changelog-104"><a href="#update_changelog-104"><span class="linenos">104</span></a>    <span class="k">if</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">config_exists</span><span class="p">():</span>
-</span><span id="update_changelog-105"><a href="#update_changelog-105"><span class="linenos">105</span></a>        <span class="n">config</span> <span class="o">=</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">load_config</span><span class="p">()</span>
-</span><span id="update_changelog-106"><a href="#update_changelog-106"><span class="linenos">106</span></a>    <span class="k">else</span><span class="p">:</span>
-</span><span id="update_changelog-107"><a href="#update_changelog-107"><span class="linenos">107</span></a>        <span class="n">hassle_config</span><span class="o">.</span><span class="n">warn</span><span class="p">()</span>
-</span><span id="update_changelog-108"><a href="#update_changelog-108"><span class="linenos">108</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Creating blank hassle_config.toml...&quot;</span><span class="p">)</span>
-</span><span id="update_changelog-109"><a href="#update_changelog-109"><span class="linenos">109</span></a>        <span class="n">config</span> <span class="o">=</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">load_config</span><span class="p">()</span>
-</span><span id="update_changelog-110"><a href="#update_changelog-110"><span class="linenos">110</span></a>    <span class="n">changelog_path</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span> <span class="o">/</span> <span class="s2">&quot;CHANGELOG.md&quot;</span>
-</span><span id="update_changelog-111"><a href="#update_changelog-111"><span class="linenos">111</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span>
-</span><span id="update_changelog-112"><a href="#update_changelog-112"><span class="linenos">112</span></a>        <span class="sa">f</span><span class="s2">&quot;auto-changelog -p </span><span class="si">{</span><span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span><span class="si">}</span><span class="s2"> --tag-prefix </span><span class="si">{</span><span class="n">config</span><span class="p">[</span><span class="s1">&#39;git&#39;</span><span class="p">][</span><span class="s1">&#39;tag_prefix&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2"> --unreleased -v </span><span class="si">{</span><span class="n">meta</span><span class="p">[</span><span class="s1">&#39;project&#39;</span><span class="p">][</span><span class="s1">&#39;version&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2"> -o </span><span class="si">{</span><span class="n">changelog_path</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="update_changelog-113"><a href="#update_changelog-113"><span class="linenos">113</span></a>    <span class="p">)</span>
-</span><span id="update_changelog-114"><a href="#update_changelog-114"><span class="linenos">114</span></a>    <span class="n">changelog</span> <span class="o">=</span> <span class="n">changelog_path</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span><span class="o">.</span><span class="n">splitlines</span><span class="p">()</span>
-</span><span id="update_changelog-115"><a href="#update_changelog-115"><span class="linenos">115</span></a>    <span class="n">changelog</span> <span class="o">=</span> <span class="p">[</span><span class="n">line</span> <span class="k">for</span> <span class="n">line</span> <span class="ow">in</span> <span class="n">changelog</span> <span class="k">if</span> <span class="s2">&quot;Full set of changes:&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">line</span><span class="p">]</span>
-</span><span id="update_changelog-116"><a href="#update_changelog-116"><span class="linenos">116</span></a>    <span class="n">changelog_path</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">changelog</span><span class="p">))</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="update_changelog-116"><a href="#update_changelog-116"><span class="linenos">116</span></a><span class="k">def</span> <span class="nf">update_changelog</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
+</span><span id="update_changelog-117"><a href="#update_changelog-117"><span class="linenos">117</span></a>    <span class="sd">&quot;&quot;&quot;Update project changelog.&quot;&quot;&quot;</span>
+</span><span id="update_changelog-118"><a href="#update_changelog-118"><span class="linenos">118</span></a>    <span class="n">meta</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">loads</span><span class="p">()</span>
+</span><span id="update_changelog-119"><a href="#update_changelog-119"><span class="linenos">119</span></a>    <span class="k">if</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">config_exists</span><span class="p">():</span>
+</span><span id="update_changelog-120"><a href="#update_changelog-120"><span class="linenos">120</span></a>        <span class="n">config</span> <span class="o">=</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">load_config</span><span class="p">()</span>
+</span><span id="update_changelog-121"><a href="#update_changelog-121"><span class="linenos">121</span></a>    <span class="k">else</span><span class="p">:</span>
+</span><span id="update_changelog-122"><a href="#update_changelog-122"><span class="linenos">122</span></a>        <span class="n">hassle_config</span><span class="o">.</span><span class="n">warn</span><span class="p">()</span>
+</span><span id="update_changelog-123"><a href="#update_changelog-123"><span class="linenos">123</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Creating blank hassle_config.toml...&quot;</span><span class="p">)</span>
+</span><span id="update_changelog-124"><a href="#update_changelog-124"><span class="linenos">124</span></a>        <span class="n">config</span> <span class="o">=</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">load_config</span><span class="p">()</span>
+</span><span id="update_changelog-125"><a href="#update_changelog-125"><span class="linenos">125</span></a>    <span class="n">changelog_path</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span> <span class="o">/</span> <span class="s2">&quot;CHANGELOG.md&quot;</span>
+</span><span id="update_changelog-126"><a href="#update_changelog-126"><span class="linenos">126</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span>
+</span><span id="update_changelog-127"><a href="#update_changelog-127"><span class="linenos">127</span></a>        <span class="sa">f</span><span class="s2">&quot;auto-changelog -p </span><span class="si">{</span><span class="n">pyproject_path</span><span class="o">.</span><span class="n">parent</span><span class="si">}</span><span class="s2"> --tag-prefix </span><span class="si">{</span><span class="n">config</span><span class="p">[</span><span class="s1">&#39;git&#39;</span><span class="p">][</span><span class="s1">&#39;tag_prefix&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2"> --unreleased -v </span><span class="si">{</span><span class="n">meta</span><span class="p">[</span><span class="s1">&#39;project&#39;</span><span class="p">][</span><span class="s1">&#39;version&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2"> -o </span><span class="si">{</span><span class="n">changelog_path</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="update_changelog-128"><a href="#update_changelog-128"><span class="linenos">128</span></a>    <span class="p">)</span>
+</span><span id="update_changelog-129"><a href="#update_changelog-129"><span class="linenos">129</span></a>    <span class="n">changelog</span> <span class="o">=</span> <span class="n">changelog_path</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span><span class="o">.</span><span class="n">splitlines</span><span class="p">()</span>
+</span><span id="update_changelog-130"><a href="#update_changelog-130"><span class="linenos">130</span></a>    <span class="n">changelog</span> <span class="o">=</span> <span class="p">[</span><span class="n">line</span> <span class="k">for</span> <span class="n">line</span> <span class="ow">in</span> <span class="n">changelog</span> <span class="k">if</span> <span class="s2">&quot;Full set of changes:&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">line</span><span class="p">]</span>
+</span><span id="update_changelog-131"><a href="#update_changelog-131"><span class="linenos">131</span></a>    <span class="n">changelog_path</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">changelog</span><span class="p">))</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Update project changelog.</p>
 </div>
 
 
@@ -418,25 +490,25 @@
         <span class="def">def</span>
         <span class="name">tag_version</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">package_path</span><span class="p">:</span> <span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="tag_version-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#tag_version"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="tag_version-119"><a href="#tag_version-119"><span class="linenos">119</span></a><span class="k">def</span> <span class="nf">tag_version</span><span class="p">(</span><span class="n">package_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
-</span><span id="tag_version-120"><a href="#tag_version-120"><span class="linenos">120</span></a>    <span class="sd">&quot;&quot;&quot;Add a git tag corresponding</span>
-</span><span id="tag_version-121"><a href="#tag_version-121"><span class="linenos">121</span></a><span class="sd">    to the version number in pyproject.toml.&quot;&quot;&quot;</span>
-</span><span id="tag_version-122"><a href="#tag_version-122"><span class="linenos">122</span></a>    <span class="k">if</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">config_exists</span><span class="p">():</span>
-</span><span id="tag_version-123"><a href="#tag_version-123"><span class="linenos">123</span></a>        <span class="n">tag_prefix</span> <span class="o">=</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">load_config</span><span class="p">()[</span><span class="s2">&quot;git&quot;</span><span class="p">][</span><span class="s2">&quot;tag_prefix&quot;</span><span class="p">]</span>
-</span><span id="tag_version-124"><a href="#tag_version-124"><span class="linenos">124</span></a>    <span class="k">else</span><span class="p">:</span>
-</span><span id="tag_version-125"><a href="#tag_version-125"><span class="linenos">125</span></a>        <span class="n">hassle_config</span><span class="o">.</span><span class="n">warn</span><span class="p">()</span>
-</span><span id="tag_version-126"><a href="#tag_version-126"><span class="linenos">126</span></a>        <span class="n">tag_prefix</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="tag_version-127"><a href="#tag_version-127"><span class="linenos">127</span></a>    <span class="n">version</span> <span class="o">=</span> <span class="p">(</span><span class="n">package_path</span> <span class="o">/</span> <span class="s2">&quot;pyproject.toml&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">loads</span><span class="p">()[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span>
-</span><span id="tag_version-128"><a href="#tag_version-128"><span class="linenos">128</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">package_path</span><span class="p">)</span>
-</span><span id="tag_version-129"><a href="#tag_version-129"><span class="linenos">129</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;git tag </span><span class="si">{</span><span class="n">tag_prefix</span><span class="si">}{</span><span class="n">version</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="tag_version-134"><a href="#tag_version-134"><span class="linenos">134</span></a><span class="k">def</span> <span class="nf">tag_version</span><span class="p">(</span><span class="n">package_path</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
+</span><span id="tag_version-135"><a href="#tag_version-135"><span class="linenos">135</span></a>    <span class="sd">&quot;&quot;&quot;Add a git tag corresponding</span>
+</span><span id="tag_version-136"><a href="#tag_version-136"><span class="linenos">136</span></a><span class="sd">    to the version number in pyproject.toml.&quot;&quot;&quot;</span>
+</span><span id="tag_version-137"><a href="#tag_version-137"><span class="linenos">137</span></a>    <span class="k">if</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">config_exists</span><span class="p">():</span>
+</span><span id="tag_version-138"><a href="#tag_version-138"><span class="linenos">138</span></a>        <span class="n">tag_prefix</span> <span class="o">=</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">load_config</span><span class="p">()[</span><span class="s2">&quot;git&quot;</span><span class="p">][</span><span class="s2">&quot;tag_prefix&quot;</span><span class="p">]</span>
+</span><span id="tag_version-139"><a href="#tag_version-139"><span class="linenos">139</span></a>    <span class="k">else</span><span class="p">:</span>
+</span><span id="tag_version-140"><a href="#tag_version-140"><span class="linenos">140</span></a>        <span class="n">hassle_config</span><span class="o">.</span><span class="n">warn</span><span class="p">()</span>
+</span><span id="tag_version-141"><a href="#tag_version-141"><span class="linenos">141</span></a>        <span class="n">tag_prefix</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="tag_version-142"><a href="#tag_version-142"><span class="linenos">142</span></a>    <span class="n">version</span> <span class="o">=</span> <span class="p">(</span><span class="n">package_path</span> <span class="o">/</span> <span class="s2">&quot;pyproject.toml&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">loads</span><span class="p">()[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span>
+</span><span id="tag_version-143"><a href="#tag_version-143"><span class="linenos">143</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">package_path</span><span class="p">)</span>
+</span><span id="tag_version-144"><a href="#tag_version-144"><span class="linenos">144</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;git tag </span><span class="si">{</span><span class="n">tag_prefix</span><span class="si">}{</span><span class="n">version</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Add a git tag corresponding
 to the version number in pyproject.toml.</p>
 </div>
```

#### html2text {}

```diff
@@ -1,13 +1,15 @@
 
 
   ⁰
 ____ hassle [Unknown INPUT type]
 ***** API Documentation *****
     * increment_version
+    * get_minimum_py_version
+    * get_project_code
     * update_minimum_python_version
     * generate_docs
     * update_dependencies
     * update_changelog
     * tag_version
 built_with_pdoc[pdoc_logo]
 
@@ -44,117 +46,131 @@
 _28        patch += 1
 _29    incremented_version = ".".join(str(num) for num in [major, minor,
 patch])
 _30    meta["project"]["version"] = incremented_version
 _31    pyproject_path.dumps(meta)
 _32
 _33
-_34def update_minimum_python_version(pyproject_path: Pathier):
-_35    """Use vermin to determine the minimum compatible
-_36    Python version and update the corresponding field
-_37    in pyproject.toml."""
-_38    project_code = "\n".join(
-_39        file.read_text() for file in (pyproject_path.parent / "src").rglob
-("*.py")
-_40    )
-_41    meta = pyproject_path.loads()
-_42    minimum_version = vermin.visit(project_code, vermin.Config
-()).minimum_versions()[1]
-_43    minimum_version = f">={minimum_version[0]}.{minimum_version[1]}"
-_44    meta["project"]["requires-python"] = minimum_version
-_45    pyproject_path.dumps(meta)
-_46
-_47
-_48def generate_docs(package_path: Pathier):
-_49    """Generate project documentation using pdoc."""
-_50    try:
-_51        (package_path / "docs").delete()
-_52    except Exception as e:
-_53        pass
-_54    os.system(
-_55        f"pdoc -o {package_path / 'docs'} {package_path / 'src' /
+_34def get_minimum_py_version(src: str) -> str:
+_35    """Scan src with vermin and return minimum
+_36    python version."""
+_37    config = vermin.Config()
+_38    config.add_backport("typing")
+_39    config.add_backport("typing_extensions")
+_40    config.set_eval_annotations(True)
+_41    result = vermin.visit(src, config).minimum_versions()[1]
+_42    return f"{result[0]}.{result[1]}"
+_43
+_44
+_45def get_project_code(project_path: Pathier) -> str:
+_46    """Read and return all code from project_path
+_47    as one string."""
+_48    return "\n".join(file.read_text() for file in project_path.rglob
+("*.py"))
+_49
+_50
+_51def update_minimum_python_version(pyproject_path: Pathier):
+_52    """Use vermin to determine the minimum compatible
+_53    Python version and update the corresponding field
+_54    in pyproject.toml."""
+_55    project_code = get_project_code(pyproject_path.parent / "src")
+_56    meta = pyproject_path.loads()
+_57    minimum_version = get_minimum_py_version(project_code)
+_58    minimum_version = f">={minimum_version}"
+_59    meta["project"]["requires-python"] = minimum_version
+_60    pyproject_path.dumps(meta)
+_61
+_62
+_63def generate_docs(package_path: Pathier):
+_64    """Generate project documentation using pdoc."""
+_65    try:
+_66        (package_path / "docs").delete()
+_67    except Exception as e:
+_68        pass
+_69    os.system(
+_70        f"pdoc -o {package_path / 'docs'} {package_path / 'src' /
 package_path.stem}"
-_56    )
-_57
-_58
-_59def update_dependencies(
-_60    pyproject_path: Pathier, overwrite: bool, include_versions: bool = False
-_61):
-_62    """Update dependencies list in pyproject.toml.
-_63
-_64    :param overwrite: If True, replace the dependencies in pyproject.toml
-_65    with the results of packagelister.scan() .
-_66    If False, packages returned by packagelister are appended to
-_67    the current dependencies in pyproject.toml if they don't already
-_68    exist in the field."""
-_69    packages = packagelister.scan(pyproject_path.parent)
-_70
-_71    packages = [
-_72        f"{package}~={packages[package]['version']}"
-_73        if packages[package]["version"] and include_versions
-_74        else f"{package}"
-_75        for package in packages
-_76        if package != pyproject_path.parent.stem
-_77    ]
-_78    packages = [
-_79        package.replace("speech_recognition", "speechRecognition")
-_80        for package in packages
-_81    ]
-_82    meta = pyproject_path.loads()
-_83    if overwrite:
-_84        meta["project"]["dependencies"] = packages
-_85    else:
-_86        for package in packages:
-_87            if "~" in package:
-_88                name = package.split("~")[0]
-_89            elif "=" in package:
-_90                name = package.split("=")[0]
-_91            else:
-_92                name = package
-_93            if all(
-_94                name not in dependency for dependency in meta["project"]
+_71    )
+_72
+_73
+_74def update_dependencies(
+_75    pyproject_path: Pathier, overwrite: bool, include_versions: bool = False
+_76):
+_77    """Update dependencies list in pyproject.toml.
+_78
+_79    :param overwrite: If True, replace the dependencies in pyproject.toml
+_80    with the results of packagelister.scan() .
+_81    If False, packages returned by packagelister are appended to
+_82    the current dependencies in pyproject.toml if they don't already
+_83    exist in the field."""
+_84    packages = packagelister.scan(pyproject_path.parent)
+_85
+_86    packages = [
+_87        f"{package}~={packages[package]['version']}"
+_88        if packages[package]["version"] and include_versions
+_89        else f"{package}"
+_90        for package in packages
+_91        if package != pyproject_path.parent.stem
+_92    ]
+_93    packages = [
+_94        package.replace("speech_recognition", "speechRecognition")
+_95        for package in packages
+_96    ]
+_97    meta = pyproject_path.loads()
+_98    if overwrite:
+_99        meta["project"]["dependencies"] = packages
+100    else:
+101        for package in packages:
+102            if "~" in package:
+103                name = package.split("~")[0]
+104            elif "=" in package:
+105                name = package.split("=")[0]
+106            else:
+107                name = package
+108            if all(
+109                name not in dependency for dependency in meta["project"]
 ["dependencies"]
-_95            ):
-_96                meta["project"]["dependencies"].append(package)
-_97    pyproject_path.dumps(meta)
-_98
-_99
-100def update_changelog(pyproject_path: Pathier):
-101    """Update project changelog."""
-102    meta = pyproject_path.loads()
-103    if hassle_config.config_exists():
-104        config = hassle_config.load_config()
-105    else:
-106        hassle_config.warn()
-107        print("Creating blank hassle_config.toml...")
-108        config = hassle_config.load_config()
-109    changelog_path = pyproject_path.parent / "CHANGELOG.md"
-110    os.system(
-111        f"auto-changelog -p {pyproject_path.parent} --tag-prefix {config
+110            ):
+111                meta["project"]["dependencies"].append(package)
+112    pyproject_path.dumps(meta)
+113
+114
+115def update_changelog(pyproject_path: Pathier):
+116    """Update project changelog."""
+117    meta = pyproject_path.loads()
+118    if hassle_config.config_exists():
+119        config = hassle_config.load_config()
+120    else:
+121        hassle_config.warn()
+122        print("Creating blank hassle_config.toml...")
+123        config = hassle_config.load_config()
+124    changelog_path = pyproject_path.parent / "CHANGELOG.md"
+125    os.system(
+126        f"auto-changelog -p {pyproject_path.parent} --tag-prefix {config
 ['git']['tag_prefix']} --unreleased -v {meta['project']['version']} -o
 {changelog_path}"
-112    )
-113    changelog = changelog_path.read_text().splitlines()
-114    changelog = [line for line in changelog if "Full set of changes:" not in
+127    )
+128    changelog = changelog_path.read_text().splitlines()
+129    changelog = [line for line in changelog if "Full set of changes:" not in
 line]
-115    changelog_path.write_text("\n".join(changelog))
-116
-117
-118def tag_version(package_path: Pathier):
-119    """Add a git tag corresponding
-120    to the version number in pyproject.toml."""
-121    if hassle_config.config_exists():
-122        tag_prefix = hassle_config.load_config()["git"]["tag_prefix"]
-123    else:
-124        hassle_config.warn()
-125        tag_prefix = ""
-126    version = (package_path / "pyproject.toml").loads()["project"]
+130    changelog_path.write_text("\n".join(changelog))
+131
+132
+133def tag_version(package_path: Pathier):
+134    """Add a git tag corresponding
+135    to the version number in pyproject.toml."""
+136    if hassle_config.config_exists():
+137        tag_prefix = hassle_config.load_config()["git"]["tag_prefix"]
+138    else:
+139        hassle_config.warn()
+140        tag_prefix = ""
+141    version = (package_path / "pyproject.toml").loads()["project"]
 ["version"]
-127    os.chdir(package_path)
-128    os.system(f"git tag {tag_prefix}{version}")
+142    os.chdir(package_path)
+143    os.system(f"git tag {tag_prefix}{version}")
   ⁰
 def increment_version(pyproject_path: pathier.pathier.Pathier, increment_type:
 str): View Source
 13def increment_version(pyproject_path: Pathier, increment_type: str):
 14    """Increment the project.version field in pyproject.toml.
 15
 16    :param package_path: Path to the package/project directory.
@@ -176,127 +192,142 @@
 31    meta["project"]["version"] = incremented_version
 32    pyproject_path.dumps(meta)
 Increment the project.version field in pyproject.toml.
 * Parameters *
     * package_path: Path to the package/project directory.
     * increment_type: One from 'major', 'minor', or 'patch'.
   ⁰
+def get_minimum_py_version(src: str) -> str: View Source
+35def get_minimum_py_version(src: str) -> str:
+36    """Scan src with vermin and return minimum
+37    python version."""
+38    config = vermin.Config()
+39    config.add_backport("typing")
+40    config.add_backport("typing_extensions")
+41    config.set_eval_annotations(True)
+42    result = vermin.visit(src, config).minimum_versions()[1]
+43    return f"{result[0]}.{result[1]}"
+Scan src with vermin and return minimum python version.
+  ⁰
+def get_project_code(project_path: pathier.pathier.Pathier) -> str: View Source
+46def get_project_code(project_path: Pathier) -> str:
+47    """Read and return all code from project_path
+48    as one string."""
+49    return "\n".join(file.read_text() for file in project_path.rglob("*.py"))
+Read and return all code from project_path as one string.
+  ⁰
 def update_minimum_python_version(pyproject_path: pathier.pathier.Pathier):
 View Source
-35def update_minimum_python_version(pyproject_path: Pathier):
-36    """Use vermin to determine the minimum compatible
-37    Python version and update the corresponding field
-38    in pyproject.toml."""
-39    project_code = "\n".join(
-40        file.read_text() for file in (pyproject_path.parent / "src").rglob
-("*.py")
-41    )
-42    meta = pyproject_path.loads()
-43    minimum_version = vermin.visit(project_code, vermin.Config
-()).minimum_versions()[1]
-44    minimum_version = f">={minimum_version[0]}.{minimum_version[1]}"
-45    meta["project"]["requires-python"] = minimum_version
-46    pyproject_path.dumps(meta)
+52def update_minimum_python_version(pyproject_path: Pathier):
+53    """Use vermin to determine the minimum compatible
+54    Python version and update the corresponding field
+55    in pyproject.toml."""
+56    project_code = get_project_code(pyproject_path.parent / "src")
+57    meta = pyproject_path.loads()
+58    minimum_version = get_minimum_py_version(project_code)
+59    minimum_version = f">={minimum_version}"
+60    meta["project"]["requires-python"] = minimum_version
+61    pyproject_path.dumps(meta)
 Use vermin to determine the minimum compatible Python version and update the
 corresponding field in pyproject.toml.
   ⁰
 def generate_docs(package_path: pathier.pathier.Pathier): View Source
-49def generate_docs(package_path: Pathier):
-50    """Generate project documentation using pdoc."""
-51    try:
-52        (package_path / "docs").delete()
-53    except Exception as e:
-54        pass
-55    os.system(
-56        f"pdoc -o {package_path / 'docs'} {package_path / 'src' /
+64def generate_docs(package_path: Pathier):
+65    """Generate project documentation using pdoc."""
+66    try:
+67        (package_path / "docs").delete()
+68    except Exception as e:
+69        pass
+70    os.system(
+71        f"pdoc -o {package_path / 'docs'} {package_path / 'src' /
 package_path.stem}"
-57    )
+72    )
 Generate project documentation using pdoc.
   ⁰
 def update_dependencies(
 pyproject_path: pathier.pathier.Pathier,
 overwrite: bool,
 include_versions: bool = False): View Source
-60def update_dependencies(
-61    pyproject_path: Pathier, overwrite: bool, include_versions: bool = False
-62):
-63    """Update dependencies list in pyproject.toml.
-64
-65    :param overwrite: If True, replace the dependencies in pyproject.toml
-66    with the results of packagelister.scan() .
-67    If False, packages returned by packagelister are appended to
-68    the current dependencies in pyproject.toml if they don't already
-69    exist in the field."""
-70    packages = packagelister.scan(pyproject_path.parent)
-71
-72    packages = [
-73        f"{package}~={packages[package]['version']}"
-74        if packages[package]["version"] and include_versions
-75        else f"{package}"
-76        for package in packages
-77        if package != pyproject_path.parent.stem
-78    ]
-79    packages = [
-80        package.replace("speech_recognition", "speechRecognition")
-81        for package in packages
-82    ]
-83    meta = pyproject_path.loads()
-84    if overwrite:
-85        meta["project"]["dependencies"] = packages
-86    else:
-87        for package in packages:
-88            if "~" in package:
-89                name = package.split("~")[0]
-90            elif "=" in package:
-91                name = package.split("=")[0]
-92            else:
-93                name = package
-94            if all(
-95                name not in dependency for dependency in meta["project"]
+_75def update_dependencies(
+_76    pyproject_path: Pathier, overwrite: bool, include_versions: bool = False
+_77):
+_78    """Update dependencies list in pyproject.toml.
+_79
+_80    :param overwrite: If True, replace the dependencies in pyproject.toml
+_81    with the results of packagelister.scan() .
+_82    If False, packages returned by packagelister are appended to
+_83    the current dependencies in pyproject.toml if they don't already
+_84    exist in the field."""
+_85    packages = packagelister.scan(pyproject_path.parent)
+_86
+_87    packages = [
+_88        f"{package}~={packages[package]['version']}"
+_89        if packages[package]["version"] and include_versions
+_90        else f"{package}"
+_91        for package in packages
+_92        if package != pyproject_path.parent.stem
+_93    ]
+_94    packages = [
+_95        package.replace("speech_recognition", "speechRecognition")
+_96        for package in packages
+_97    ]
+_98    meta = pyproject_path.loads()
+_99    if overwrite:
+100        meta["project"]["dependencies"] = packages
+101    else:
+102        for package in packages:
+103            if "~" in package:
+104                name = package.split("~")[0]
+105            elif "=" in package:
+106                name = package.split("=")[0]
+107            else:
+108                name = package
+109            if all(
+110                name not in dependency for dependency in meta["project"]
 ["dependencies"]
-96            ):
-97                meta["project"]["dependencies"].append(package)
-98    pyproject_path.dumps(meta)
+111            ):
+112                meta["project"]["dependencies"].append(package)
+113    pyproject_path.dumps(meta)
 Update dependencies list in pyproject.toml.
 * Parameters *
     * overwrite: If True, replace the dependencies in pyproject.toml with the
       results of packagelister.scan() . If False, packages returned by
       packagelister are appended to the current dependencies in pyproject.toml
       if they don't already exist in the field.
   ⁰
 def update_changelog(pyproject_path: pathier.pathier.Pathier): View Source
-101def update_changelog(pyproject_path: Pathier):
-102    """Update project changelog."""
-103    meta = pyproject_path.loads()
-104    if hassle_config.config_exists():
-105        config = hassle_config.load_config()
-106    else:
-107        hassle_config.warn()
-108        print("Creating blank hassle_config.toml...")
-109        config = hassle_config.load_config()
-110    changelog_path = pyproject_path.parent / "CHANGELOG.md"
-111    os.system(
-112        f"auto-changelog -p {pyproject_path.parent} --tag-prefix {config
+116def update_changelog(pyproject_path: Pathier):
+117    """Update project changelog."""
+118    meta = pyproject_path.loads()
+119    if hassle_config.config_exists():
+120        config = hassle_config.load_config()
+121    else:
+122        hassle_config.warn()
+123        print("Creating blank hassle_config.toml...")
+124        config = hassle_config.load_config()
+125    changelog_path = pyproject_path.parent / "CHANGELOG.md"
+126    os.system(
+127        f"auto-changelog -p {pyproject_path.parent} --tag-prefix {config
 ['git']['tag_prefix']} --unreleased -v {meta['project']['version']} -o
 {changelog_path}"
-113    )
-114    changelog = changelog_path.read_text().splitlines()
-115    changelog = [line for line in changelog if "Full set of changes:" not in
+128    )
+129    changelog = changelog_path.read_text().splitlines()
+130    changelog = [line for line in changelog if "Full set of changes:" not in
 line]
-116    changelog_path.write_text("\n".join(changelog))
+131    changelog_path.write_text("\n".join(changelog))
 Update project changelog.
   ⁰
 def tag_version(package_path: pathier.pathier.Pathier): View Source
-119def tag_version(package_path: Pathier):
-120    """Add a git tag corresponding
-121    to the version number in pyproject.toml."""
-122    if hassle_config.config_exists():
-123        tag_prefix = hassle_config.load_config()["git"]["tag_prefix"]
-124    else:
-125        hassle_config.warn()
-126        tag_prefix = ""
-127    version = (package_path / "pyproject.toml").loads()["project"]
+134def tag_version(package_path: Pathier):
+135    """Add a git tag corresponding
+136    to the version number in pyproject.toml."""
+137    if hassle_config.config_exists():
+138        tag_prefix = hassle_config.load_config()["git"]["tag_prefix"]
+139    else:
+140        hassle_config.warn()
+141        tag_prefix = ""
+142    version = (package_path / "pyproject.toml").loads()["project"]
 ["version"]
-128    os.chdir(package_path)
-129    os.system(f"git tag {tag_prefix}{version}")
+143    os.chdir(package_path)
+144    os.system(f"git tag {tag_prefix}{version}")
 Add a git tag corresponding to the version number in pyproject.toml.
```

### Comparing `hassle-2.5.0/docs/hassle/new_project.html` & `hassle-2.6.0/docs/hassle/new_project.html`

 * *Files identical despite different names*

### Comparing `hassle-2.5.0/docs/hassle/run_tests.html` & `hassle-2.6.0/docs/hassle/run_tests.html`

 * *Files identical despite different names*

### Comparing `hassle-2.5.0/src/hassle/generate_tests.py` & `hassle-2.6.0/src/hassle/generate_tests.py`

 * *Files identical despite different names*

### Comparing `hassle-2.5.0/src/hassle/hassle.py` & `hassle-2.6.0/src/hassle/hassle.py`

 * *Files identical despite different names*

### Comparing `hassle-2.5.0/src/hassle/hassle_config.py` & `hassle-2.6.0/src/hassle/hassle_config.py`

 * *Files identical despite different names*

### Comparing `hassle-2.5.0/src/hassle/hassle_utilities.py` & `hassle-2.6.0/src/hassle/hassle_utilities.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,24 +27,39 @@
     elif increment_type == "patch":
         patch += 1
     incremented_version = ".".join(str(num) for num in [major, minor, patch])
     meta["project"]["version"] = incremented_version
     pyproject_path.dumps(meta)
 
 
+def get_minimum_py_version(src: str) -> str:
+    """Scan src with vermin and return minimum
+    python version."""
+    config = vermin.Config()
+    config.add_backport("typing")
+    config.add_backport("typing_extensions")
+    config.set_eval_annotations(True)
+    result = vermin.visit(src, config).minimum_versions()[1]
+    return f"{result[0]}.{result[1]}"
+
+
+def get_project_code(project_path: Pathier) -> str:
+    """Read and return all code from project_path
+    as one string."""
+    return "\n".join(file.read_text() for file in project_path.rglob("*.py"))
+
+
 def update_minimum_python_version(pyproject_path: Pathier):
     """Use vermin to determine the minimum compatible
     Python version and update the corresponding field
     in pyproject.toml."""
-    project_code = "\n".join(
-        file.read_text() for file in (pyproject_path.parent / "src").rglob("*.py")
-    )
+    project_code = get_project_code(pyproject_path.parent / "src")
     meta = pyproject_path.loads()
-    minimum_version = vermin.visit(project_code, vermin.Config()).minimum_versions()[1]
-    minimum_version = f">={minimum_version[0]}.{minimum_version[1]}"
+    minimum_version = get_minimum_py_version(project_code)
+    minimum_version = f">={minimum_version}"
     meta["project"]["requires-python"] = minimum_version
     pyproject_path.dumps(meta)
 
 
 def generate_docs(package_path: Pathier):
     """Generate project documentation using pdoc."""
     try:
```

### Comparing `hassle-2.5.0/src/hassle/license_template.txt` & `hassle-2.6.0/src/hassle/license_template.txt`

 * *Files identical despite different names*

### Comparing `hassle-2.5.0/src/hassle/new_project.py` & `hassle-2.6.0/src/hassle/new_project.py`

 * *Files identical despite different names*

### Comparing `hassle-2.5.0/src/hassle/pyproject_template.toml` & `hassle-2.6.0/src/hassle/pyproject_template.toml`

 * *Files identical despite different names*

### Comparing `hassle-2.5.0/src/hassle/run_tests.py` & `hassle-2.6.0/src/hassle/run_tests.py`

 * *Files identical despite different names*

### Comparing `hassle-2.5.0/LICENSE.txt` & `hassle-2.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hassle-2.5.0/README.md` & `hassle-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `hassle-2.5.0/pyproject.toml` & `hassle-2.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 00000090: 226d 6174 746d 616e 6573 4070 6d2e 6d65  "mattmanes@pm.me
 000000a0: 227d 5d0d 0a64 6573 6372 6970 7469 6f6e  "}]..description
 000000b0: 203d 2022 4372 6561 7465 2c20 6275 696c   = "Create, buil
 000000c0: 642c 2074 6573 742c 2061 6e64 2070 7562  d, test, and pub
 000000d0: 6c69 7368 2050 7974 686f 6e20 7072 6f6a  lish Python proj
 000000e0: 6563 7473 2061 6e64 2070 6163 6b61 6765  ects and package
 000000f0: 732e 220d 0a76 6572 7369 6f6e 203d 2022  s."..version = "
-00000100: 322e 352e 3022 0d0a 7265 7175 6972 6573  2.5.0"..requires
+00000100: 322e 362e 3022 0d0a 7265 7175 6972 6573  2.6.0"..requires
 00000110: 2d70 7974 686f 6e20 3d20 223e 3d33 2e31  -python = ">=3.1
 00000120: 3022 0d0a 6465 7065 6e64 656e 6369 6573  0"..dependencies
 00000130: 203d 205b 0d0a 2020 2020 2262 6c61 636b   = [..    "black
 00000140: 222c 200d 0a20 2020 2022 6973 6f72 7422  ", ..    "isort"
 00000150: 2c20 0d0a 2020 2020 2270 7974 6573 747e  , ..    "pytest~
 00000160: 3d37 2e32 2e31 222c 200d 0a20 2020 2022  =7.2.1", ..    "
 00000170: 636f 7665 7261 6765 222c 0d0a 2020 2020  coverage",..
```

### Comparing `hassle-2.5.0/PKG-INFO` & `hassle-2.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hassle
-Version: 2.5.0
+Version: 2.6.0
 Summary: Create, build, test, and publish Python projects and packages.
 Project-URL: Homepage, https://github.com/matt-manes/hassle
 Project-URL: Documentation, https://github.com/matt-manes/hassle/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/hassle/tree/main/src/hassle
 Author-email: Matt Manes <mattmanes@pm.me>
 License-File: LICENSE.txt
 Keywords: automation,build,devops,packaging,test
```

