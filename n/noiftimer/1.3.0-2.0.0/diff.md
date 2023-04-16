# Comparing `tmp/noiftimer-1.3.0.tar.gz` & `tmp/noiftimer-2.0.0.tar.gz`

## Comparing `noiftimer-1.3.0.tar` & `noiftimer-2.0.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 noiftimer-1.3.0/CHANGELOG.md
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 noiftimer-1.3.0/docs/index.html
--rw-r--r--   0        0        0    34120 2020-02-02 00:00:00.000000 noiftimer-1.3.0/docs/noiftimer.html
--rw-r--r--   0        0        0    26382 2020-02-02 00:00:00.000000 noiftimer-1.3.0/docs/search.js
--rw-r--r--   0        0        0   145130 2020-02-02 00:00:00.000000 noiftimer-1.3.0/docs/noiftimer/noiftimer.html
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 noiftimer-1.3.0/src/noiftimer/__init__.py
--rw-r--r--   0        0        0     6014 2020-02-02 00:00:00.000000 noiftimer-1.3.0/src/noiftimer/noiftimer.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 noiftimer-1.3.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 noiftimer-1.3.0/LICENSE.txt
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 noiftimer-1.3.0/README.md
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 noiftimer-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 noiftimer-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 noiftimer-2.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 noiftimer-2.0.0/docs/index.html
+-rw-r--r--   0        0        0    34120 2020-02-02 00:00:00.000000 noiftimer-2.0.0/docs/noiftimer.html
+-rw-r--r--   0        0        0    24774 2020-02-02 00:00:00.000000 noiftimer-2.0.0/docs/search.js
+-rw-r--r--   0        0        0   130100 2020-02-02 00:00:00.000000 noiftimer-2.0.0/docs/noiftimer/noiftimer.html
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 noiftimer-2.0.0/src/noiftimer/__init__.py
+-rw-r--r--   0        0        0     5353 2020-02-02 00:00:00.000000 noiftimer-2.0.0/src/noiftimer/noiftimer.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 noiftimer-2.0.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 noiftimer-2.0.0/LICENSE.txt
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 noiftimer-2.0.0/README.md
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 noiftimer-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 noiftimer-2.0.0/PKG-INFO
```

### Comparing `noiftimer-1.3.0/docs/noiftimer.html` & `noiftimer-2.0.0/docs/noiftimer.html`

 * *Files identical despite different names*

### Comparing `noiftimer-1.3.0/docs/search.js` & `noiftimer-2.0.0/docs/search.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -710,14 +710,21 @@
         "fullname": "noiftimer.noiftimer.Timer.__init__",
         "modulename": "noiftimer.noiftimer",
         "qualname": "Timer.__init__",
         "kind": "function",
         "doc": "<h6 id=\"parameters\">Parameters</h6>\n\n<ul>\n<li><p><strong>averaging_window_length</strong>:  Number of start/stop cycles\nto calculate the average elapsed time with.</p></li>\n<li><p><strong>subsecond_resolution</strong>:  Whether to print formatted time\nstrings with subsecond resolution or not.</p></li>\n</ul>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">averaging_window_length</span><span class=\"p\">:</span> <span class=\"nb\">int</span> <span class=\"o\">=</span> <span class=\"mi\">10</span>, </span><span class=\"param\"><span class=\"n\">subsecond_resolution</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">True</span></span>)</span>"
     }, {
+        "fullname": "noiftimer.noiftimer.Timer.started",
+        "modulename": "noiftimer.noiftimer",
+        "qualname": "Timer.started",
+        "kind": "variable",
+        "doc": "<p>Returns whether the timer has\nbeen started and is currently running.</p>\n",
+        "annotation": ": bool"
+    }, {
         "fullname": "noiftimer.noiftimer.Timer.elapsed",
         "modulename": "noiftimer.noiftimer",
         "qualname": "Timer.elapsed",
         "kind": "variable",
         "doc": "<p>Return the currently elapsed time.</p>\n",
         "annotation": ": float"
     }, {
@@ -729,48 +736,39 @@
         "annotation": ": str"
     }, {
         "fullname": "noiftimer.noiftimer.Timer.start",
         "modulename": "noiftimer.noiftimer",
         "qualname": "Timer.start",
         "kind": "function",
         "doc": "<p>Start timer.\nReturns this Timer instance so\ntimer start can be chained to\nTimer creation.</p>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"gp\">&gt;&gt;&gt; </span><span class=\"n\">timer</span> <span class=\"o\">=</span> <span class=\"n\">Timer</span><span class=\"p\">()</span><span class=\"o\">.</span><span class=\"n\">start</span><span class=\"p\">()</span>\n</code></pre>\n</div>\n",
-        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span></span><span class=\"return-annotation\">) -> <span class=\"n\">Self</span>:</span></span>",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span><span class=\"p\">:</span> <span class=\"n\">Self</span></span><span class=\"return-annotation\">) -> <span class=\"n\">Self</span>:</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "noiftimer.noiftimer.Timer.stop",
         "modulename": "noiftimer.noiftimer",
         "qualname": "Timer.stop",
         "kind": "function",
         "doc": "<p>Stop timer.</p>\n\n<p>Calculates elapsed time and average elapsed time.</p>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
     }, {
-        "fullname": "noiftimer.noiftimer.Timer.current_elapsed_time",
-        "modulename": "noiftimer.noiftimer",
-        "qualname": "Timer.current_elapsed_time",
-        "kind": "function",
-        "doc": "<p>Returns current elapsed without stopping the timer.</p>\n\n<h6 id=\"parameters\">Parameters</h6>\n\n<ul>\n<li><strong>format</strong>:  If True, elapsed time is returned as a string.\nIf False, elapsed time is returned as a float.</li>\n</ul>\n",
-        "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"bp\">self</span>,</span><span class=\"param\">\t<span class=\"nb\">format</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">True</span>,</span><span class=\"param\">\t<span class=\"n\">subsecond_resolution</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">False</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">float</span> <span class=\"o\">|</span> <span class=\"nb\">str</span>:</span></span>",
-        "funcdef": "def"
-    }, {
         "fullname": "noiftimer.noiftimer.Timer.format_time",
         "modulename": "noiftimer.noiftimer",
         "qualname": "Timer.format_time",
         "kind": "function",
         "doc": "<p>Returns num_seconds as a string with units.</p>\n\n<h6 id=\"parameters\">Parameters</h6>\n\n<ul>\n<li><strong>subsecond_resolution</strong>:  Include milliseconds\nand microseconds with the output.</li>\n</ul>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">num_seconds</span><span class=\"p\">:</span> <span class=\"nb\">float</span>, </span><span class=\"param\"><span class=\"n\">subsecond_resolution</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">False</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">str</span>:</span></span>",
         "funcdef": "def"
     }, {
-        "fullname": "noiftimer.noiftimer.Timer.get_stats",
+        "fullname": "noiftimer.noiftimer.Timer.stats",
         "modulename": "noiftimer.noiftimer",
-        "qualname": "Timer.get_stats",
-        "kind": "function",
-        "doc": "<p>Returns string for elapsed time and average elapsed time.</p>\n\n<h6 id=\"parameters\">Parameters</h6>\n\n<ul>\n<li><p><strong>format</strong>:  Times are returned as strings if True,\notherwise they're raw floats.</p></li>\n<li><p><strong>subsecond_resolution</strong>:  Include milliseconds\nand microseconds with the output.</p></li>\n</ul>\n",
-        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"nb\">format</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">True</span>, </span><span class=\"param\"><span class=\"n\">subsecond_resolution</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">False</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">str</span>:</span></span>",
-        "funcdef": "def"
+        "qualname": "Timer.stats",
+        "kind": "variable",
+        "doc": "<p>Returns a string stating the currently elapsed time\nand the average elapsed time.</p>\n",
+        "annotation": ": str"
     }];
 
     // mirrored in build-search-index.js (part 1)
     // Also split on html tags. this is a cheap heuristic, but good enough.
     elasticlunr.tokenizer.setSeperator(/[\s\-.;&_'"=,()]+|<[^>]*>/);
 
     let searchIndex;
```

### Comparing `noiftimer-1.3.0/docs/noiftimer/noiftimer.html` & `noiftimer-2.0.0/docs/noiftimer/noiftimer.html`

 * *Files 2% similar despite different names*

```diff
@@ -36,33 +36,33 @@
             <li>
                     <a class="class" href="#Timer">Timer</a>
                             <ul class="memberlist">
                         <li>
                                 <a class="function" href="#Timer.__init__">Timer</a>
                         </li>
                         <li>
+                                <a class="variable" href="#Timer.started">started</a>
+                        </li>
+                        <li>
                                 <a class="variable" href="#Timer.elapsed">elapsed</a>
                         </li>
                         <li>
                                 <a class="variable" href="#Timer.elapsed_str">elapsed_str</a>
                         </li>
                         <li>
                                 <a class="function" href="#Timer.start">start</a>
                         </li>
                         <li>
                                 <a class="function" href="#Timer.stop">stop</a>
                         </li>
                         <li>
-                                <a class="function" href="#Timer.current_elapsed_time">current_elapsed_time</a>
-                        </li>
-                        <li>
                                 <a class="function" href="#Timer.format_time">format_time</a>
                         </li>
                         <li>
-                                <a class="function" href="#Timer.get_stats">get_stats</a>
+                                <a class="variable" href="#Timer.stats">stats</a>
                         </li>
                 </ul>
 
             </li>
     </ul>
 
 
@@ -80,174 +80,177 @@
 <a href="./../noiftimer.html">noiftimer</a><wbr>.noiftimer    </h1>
 
                 
                         <input id="mod-noiftimer-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 
                         <label class="view-source-button" for="mod-noiftimer-view-source"><span>View Source</span></label>
 
-                        <div class="pdoc-code codehilite"><pre><span></span><span id="L-1"><a href="#L-1"><span class="linenos">  1</span></a><span class="kn">import</span> <span class="nn">warnings</span>
-</span><span id="L-2"><a href="#L-2"><span class="linenos">  2</span></a><span class="kn">from</span> <span class="nn">datetime</span> <span class="kn">import</span> <span class="n">datetime</span>
-</span><span id="L-3"><a href="#L-3"><span class="linenos">  3</span></a><span class="kn">from</span> <span class="nn">typing</span> <span class="kn">import</span> <span class="n">Any</span><span class="p">,</span> <span class="n">Callable</span><span class="p">,</span> <span class="n">Self</span>
-</span><span id="L-4"><a href="#L-4"><span class="linenos">  4</span></a>
+                        <div class="pdoc-code codehilite"><pre><span></span><span id="L-1"><a href="#L-1"><span class="linenos">  1</span></a><span class="kn">import</span> <span class="nn">time</span>
+</span><span id="L-2"><a href="#L-2"><span class="linenos">  2</span></a><span class="kn">from</span> <span class="nn">typing</span> <span class="kn">import</span> <span class="n">Any</span><span class="p">,</span> <span class="n">Callable</span>
+</span><span id="L-3"><a href="#L-3"><span class="linenos">  3</span></a>
+</span><span id="L-4"><a href="#L-4"><span class="linenos">  4</span></a><span class="kn">from</span> <span class="nn">typing_extensions</span> <span class="kn">import</span> <span class="n">Self</span>
 </span><span id="L-5"><a href="#L-5"><span class="linenos">  5</span></a>
-</span><span id="L-6"><a href="#L-6"><span class="linenos">  6</span></a><span class="k">def</span> <span class="nf">time_it</span><span class="p">(</span><span class="n">loops</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">1</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Callable</span><span class="p">[</span><span class="o">...</span><span class="p">,</span> <span class="n">Any</span><span class="p">]:</span>
-</span><span id="L-7"><a href="#L-7"><span class="linenos">  7</span></a>    <span class="sd">&quot;&quot;&quot;Decorator to time function execution time</span>
-</span><span id="L-8"><a href="#L-8"><span class="linenos">  8</span></a><span class="sd">    and print the results.</span>
-</span><span id="L-9"><a href="#L-9"><span class="linenos">  9</span></a>
-</span><span id="L-10"><a href="#L-10"><span class="linenos"> 10</span></a><span class="sd">    :param loops: How many times to loop the function,</span>
-</span><span id="L-11"><a href="#L-11"><span class="linenos"> 11</span></a><span class="sd">    starting and stopping the timer before and after</span>
-</span><span id="L-12"><a href="#L-12"><span class="linenos"> 12</span></a><span class="sd">    each loop.&quot;&quot;&quot;</span>
-</span><span id="L-13"><a href="#L-13"><span class="linenos"> 13</span></a>
-</span><span id="L-14"><a href="#L-14"><span class="linenos"> 14</span></a>    <span class="k">def</span> <span class="nf">decorator</span><span class="p">(</span><span class="n">func</span><span class="p">:</span> <span class="n">Callable</span><span class="p">[</span><span class="o">...</span><span class="p">,</span> <span class="n">Any</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="n">Callable</span><span class="p">[</span><span class="o">...</span><span class="p">,</span> <span class="n">Any</span><span class="p">]:</span>
-</span><span id="L-15"><a href="#L-15"><span class="linenos"> 15</span></a>        <span class="k">def</span> <span class="nf">wrapper</span><span class="p">(</span><span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
-</span><span id="L-16"><a href="#L-16"><span class="linenos"> 16</span></a>            <span class="n">timer</span> <span class="o">=</span> <span class="n">Timer</span><span class="p">(</span><span class="n">loops</span><span class="p">)</span>
-</span><span id="L-17"><a href="#L-17"><span class="linenos"> 17</span></a>            <span class="k">for</span> <span class="n">_</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="n">loops</span><span class="p">):</span>
-</span><span id="L-18"><a href="#L-18"><span class="linenos"> 18</span></a>                <span class="n">timer</span><span class="o">.</span><span class="n">start</span><span class="p">()</span>
-</span><span id="L-19"><a href="#L-19"><span class="linenos"> 19</span></a>                <span class="n">result</span> <span class="o">=</span> <span class="n">func</span><span class="p">(</span><span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">)</span>
-</span><span id="L-20"><a href="#L-20"><span class="linenos"> 20</span></a>                <span class="n">timer</span><span class="o">.</span><span class="n">stop</span><span class="p">()</span>
-</span><span id="L-21"><a href="#L-21"><span class="linenos"> 21</span></a>            <span class="n">execution_time</span> <span class="o">=</span> <span class="n">timer</span><span class="o">.</span><span class="n">format_time</span><span class="p">(</span><span class="n">timer</span><span class="o">.</span><span class="n">average_elapsed_time</span><span class="p">,</span> <span class="kc">True</span><span class="p">)</span>
-</span><span id="L-22"><a href="#L-22"><span class="linenos"> 22</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">func</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2"> average execution time: </span><span class="si">{</span><span class="n">execution_time</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-23"><a href="#L-23"><span class="linenos"> 23</span></a>            <span class="k">return</span> <span class="n">result</span>
-</span><span id="L-24"><a href="#L-24"><span class="linenos"> 24</span></a>
-</span><span id="L-25"><a href="#L-25"><span class="linenos"> 25</span></a>        <span class="k">return</span> <span class="n">wrapper</span>
-</span><span id="L-26"><a href="#L-26"><span class="linenos"> 26</span></a>
-</span><span id="L-27"><a href="#L-27"><span class="linenos"> 27</span></a>    <span class="k">return</span> <span class="n">decorator</span>
-</span><span id="L-28"><a href="#L-28"><span class="linenos"> 28</span></a>
+</span><span id="L-6"><a href="#L-6"><span class="linenos">  6</span></a>
+</span><span id="L-7"><a href="#L-7"><span class="linenos">  7</span></a><span class="k">def</span> <span class="nf">time_it</span><span class="p">(</span><span class="n">loops</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">1</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Callable</span><span class="p">[</span><span class="o">...</span><span class="p">,</span> <span class="n">Any</span><span class="p">]:</span>
+</span><span id="L-8"><a href="#L-8"><span class="linenos">  8</span></a>    <span class="sd">&quot;&quot;&quot;Decorator to time function execution time</span>
+</span><span id="L-9"><a href="#L-9"><span class="linenos">  9</span></a><span class="sd">    and print the results.</span>
+</span><span id="L-10"><a href="#L-10"><span class="linenos"> 10</span></a>
+</span><span id="L-11"><a href="#L-11"><span class="linenos"> 11</span></a><span class="sd">    :param loops: How many times to loop the function,</span>
+</span><span id="L-12"><a href="#L-12"><span class="linenos"> 12</span></a><span class="sd">    starting and stopping the timer before and after</span>
+</span><span id="L-13"><a href="#L-13"><span class="linenos"> 13</span></a><span class="sd">    each loop.&quot;&quot;&quot;</span>
+</span><span id="L-14"><a href="#L-14"><span class="linenos"> 14</span></a>
+</span><span id="L-15"><a href="#L-15"><span class="linenos"> 15</span></a>    <span class="k">def</span> <span class="nf">decorator</span><span class="p">(</span><span class="n">func</span><span class="p">:</span> <span class="n">Callable</span><span class="p">[</span><span class="o">...</span><span class="p">,</span> <span class="n">Any</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="n">Callable</span><span class="p">[</span><span class="o">...</span><span class="p">,</span> <span class="n">Any</span><span class="p">]:</span>
+</span><span id="L-16"><a href="#L-16"><span class="linenos"> 16</span></a>        <span class="k">def</span> <span class="nf">wrapper</span><span class="p">(</span><span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
+</span><span id="L-17"><a href="#L-17"><span class="linenos"> 17</span></a>            <span class="n">timer</span> <span class="o">=</span> <span class="n">Timer</span><span class="p">(</span><span class="n">loops</span><span class="p">)</span>
+</span><span id="L-18"><a href="#L-18"><span class="linenos"> 18</span></a>            <span class="n">result</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="L-19"><a href="#L-19"><span class="linenos"> 19</span></a>            <span class="k">for</span> <span class="n">_</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="n">loops</span><span class="p">):</span>
+</span><span id="L-20"><a href="#L-20"><span class="linenos"> 20</span></a>                <span class="n">timer</span><span class="o">.</span><span class="n">start</span><span class="p">()</span>
+</span><span id="L-21"><a href="#L-21"><span class="linenos"> 21</span></a>                <span class="n">result</span> <span class="o">=</span> <span class="n">func</span><span class="p">(</span><span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">)</span>
+</span><span id="L-22"><a href="#L-22"><span class="linenos"> 22</span></a>                <span class="n">timer</span><span class="o">.</span><span class="n">stop</span><span class="p">()</span>
+</span><span id="L-23"><a href="#L-23"><span class="linenos"> 23</span></a>            <span class="nb">print</span><span class="p">(</span>
+</span><span id="L-24"><a href="#L-24"><span class="linenos"> 24</span></a>                <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">func</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2"> average execution time: </span><span class="si">{</span><span class="n">timer</span><span class="o">.</span><span class="n">average_elapsed_str</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-25"><a href="#L-25"><span class="linenos"> 25</span></a>            <span class="p">)</span>
+</span><span id="L-26"><a href="#L-26"><span class="linenos"> 26</span></a>            <span class="k">return</span> <span class="n">result</span>
+</span><span id="L-27"><a href="#L-27"><span class="linenos"> 27</span></a>
+</span><span id="L-28"><a href="#L-28"><span class="linenos"> 28</span></a>        <span class="k">return</span> <span class="n">wrapper</span>
 </span><span id="L-29"><a href="#L-29"><span class="linenos"> 29</span></a>
-</span><span id="L-30"><a href="#L-30"><span class="linenos"> 30</span></a><span class="k">class</span> <span class="nc">Timer</span><span class="p">:</span>
-</span><span id="L-31"><a href="#L-31"><span class="linenos"> 31</span></a>    <span class="sd">&quot;&quot;&quot;Simple timer class that tracks total elapsed time</span>
-</span><span id="L-32"><a href="#L-32"><span class="linenos"> 32</span></a><span class="sd">    and average time between calls to &#39;start&#39; and &#39;stop&#39;.&quot;&quot;&quot;</span>
-</span><span id="L-33"><a href="#L-33"><span class="linenos"> 33</span></a>
-</span><span id="L-34"><a href="#L-34"><span class="linenos"> 34</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
-</span><span id="L-35"><a href="#L-35"><span class="linenos"> 35</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">averaging_window_length</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">10</span><span class="p">,</span> <span class="n">subsecond_resolution</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a>    <span class="p">):</span>
-</span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a>        <span class="sd">&quot;&quot;&quot;:param averaging_window_length: Number of start/stop cycles</span>
-</span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a><span class="sd">        to calculate the average elapsed time with.</span>
-</span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a>
-</span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a><span class="sd">        :param subsecond_resolution: Whether to print formatted time</span>
-</span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a><span class="sd">        strings with subsecond resolution or not.&quot;&quot;&quot;</span>
-</span><span id="L-42"><a href="#L-42"><span class="linenos"> 42</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">start_time</span><span class="p">:</span> <span class="n">datetime</span> <span class="o">=</span> <span class="n">datetime</span><span class="o">.</span><span class="n">now</span><span class="p">()</span>
-</span><span id="L-43"><a href="#L-43"><span class="linenos"> 43</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">stop_time</span><span class="p">:</span> <span class="n">datetime</span> <span class="o">=</span> <span class="n">datetime</span><span class="o">.</span><span class="n">now</span><span class="p">()</span>
-</span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">average_elapsed_time</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="mi">0</span>
-</span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">history</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">float</span><span class="p">]</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">elapsed_time</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="mi">0</span>
-</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">averaging_window_length</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="n">averaging_window_length</span>
-</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">started</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">subsecond_resolution</span> <span class="o">=</span> <span class="n">subsecond_resolution</span>
-</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a>
-</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a>    <span class="nd">@property</span>
-</span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a>    <span class="k">def</span> <span class="nf">elapsed</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span><span class="p">:</span>
-</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a>        <span class="sd">&quot;&quot;&quot;Return the currently elapsed time.&quot;&quot;&quot;</span>
-</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">started</span><span class="p">:</span>
-</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a>            <span class="k">return</span> <span class="p">(</span><span class="n">datetime</span><span class="o">.</span><span class="n">now</span><span class="p">()</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">start_time</span><span class="p">)</span><span class="o">.</span><span class="n">total_seconds</span><span class="p">()</span>
-</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a>            <span class="k">return</span> <span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">stop_time</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">start_time</span><span class="p">)</span><span class="o">.</span><span class="n">total_seconds</span><span class="p">()</span>
-</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a>
-</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a>    <span class="nd">@property</span>
-</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a>    <span class="k">def</span> <span class="nf">elapsed_str</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a>        <span class="sd">&quot;&quot;&quot;Return the currently elapsed time</span>
-</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a><span class="sd">        as a formatted string.&quot;&quot;&quot;</span>
-</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">format_time</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">elapsed</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">subsecond_resolution</span><span class="p">)</span>
-</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a>
-</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a>    <span class="k">def</span> <span class="nf">start</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
-</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a>        <span class="sd">&quot;&quot;&quot;Start timer.</span>
-</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a><span class="sd">        Returns this Timer instance so</span>
-</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a><span class="sd">        timer start can be chained to</span>
-</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a><span class="sd">        Timer creation.</span>
-</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a>
-</span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a><span class="sd">        &gt;&gt;&gt; timer = Timer().start()&quot;&quot;&quot;</span>
-</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">start_time</span> <span class="o">=</span> <span class="n">datetime</span><span class="o">.</span><span class="n">now</span><span class="p">()</span>
-</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">started</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a>        <span class="k">return</span> <span class="bp">self</span>
-</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a>
-</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a>    <span class="k">def</span> <span class="nf">stop</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a>        <span class="sd">&quot;&quot;&quot;Stop timer.</span>
-</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a>
-</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a><span class="sd">        Calculates elapsed time and average elapsed time.&quot;&quot;&quot;</span>
-</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">stop_time</span> <span class="o">=</span> <span class="n">datetime</span><span class="o">.</span><span class="n">now</span><span class="p">()</span>
-</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">started</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">elapsed_time</span> <span class="o">=</span> <span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">stop_time</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">start_time</span><span class="p">)</span><span class="o">.</span><span class="n">total_seconds</span><span class="p">()</span>
-</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_save_elapsed_time</span><span class="p">()</span>
-</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">average_elapsed_time</span> <span class="o">=</span> <span class="nb">sum</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">history</span><span class="p">)</span> <span class="o">/</span> <span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">history</span><span class="p">))</span>
+</span><span id="L-30"><a href="#L-30"><span class="linenos"> 30</span></a>    <span class="k">return</span> <span class="n">decorator</span>
+</span><span id="L-31"><a href="#L-31"><span class="linenos"> 31</span></a>
+</span><span id="L-32"><a href="#L-32"><span class="linenos"> 32</span></a>
+</span><span id="L-33"><a href="#L-33"><span class="linenos"> 33</span></a><span class="k">class</span> <span class="nc">Timer</span><span class="p">:</span>
+</span><span id="L-34"><a href="#L-34"><span class="linenos"> 34</span></a>    <span class="sd">&quot;&quot;&quot;Simple timer class that tracks total elapsed time</span>
+</span><span id="L-35"><a href="#L-35"><span class="linenos"> 35</span></a><span class="sd">    and average time between calls to &#39;start&#39; and &#39;stop&#39;.&quot;&quot;&quot;</span>
+</span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a>
+</span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
+</span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">averaging_window_length</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">10</span><span class="p">,</span> <span class="n">subsecond_resolution</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a>    <span class="p">):</span>
+</span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a>        <span class="sd">&quot;&quot;&quot;:param averaging_window_length: Number of start/stop cycles</span>
+</span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a><span class="sd">        to calculate the average elapsed time with.</span>
+</span><span id="L-42"><a href="#L-42"><span class="linenos"> 42</span></a>
+</span><span id="L-43"><a href="#L-43"><span class="linenos"> 43</span></a><span class="sd">        :param subsecond_resolution: Whether to print formatted time</span>
+</span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a><span class="sd">        strings with subsecond resolution or not.&quot;&quot;&quot;</span>
+</span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_start_time</span> <span class="o">=</span> <span class="n">time</span><span class="o">.</span><span class="n">time</span><span class="p">()</span>
+</span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_stop_time</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">start_time</span>
+</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_elapsed</span> <span class="o">=</span> <span class="mi">0</span>
+</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_average_elapsed</span> <span class="o">=</span> <span class="mi">0</span>
+</span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_history</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">float</span><span class="p">]</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_started</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">averaging_window_length</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="n">averaging_window_length</span>
+</span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">subsecond_resolution</span> <span class="o">=</span> <span class="n">subsecond_resolution</span>
+</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a>
+</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a>    <span class="nd">@property</span>
+</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a>    <span class="k">def</span> <span class="nf">started</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a>        <span class="sd">&quot;&quot;&quot;Returns whether the timer has</span>
+</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a><span class="sd">        been started and is currently running.&quot;&quot;&quot;</span>
+</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_started</span>
+</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a>
+</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a>    <span class="nd">@property</span>
+</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a>    <span class="k">def</span> <span class="nf">elapsed</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span><span class="p">:</span>
+</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a>        <span class="sd">&quot;&quot;&quot;Return the currently elapsed time.&quot;&quot;&quot;</span>
+</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_started</span><span class="p">:</span>
+</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a>            <span class="k">return</span> <span class="n">time</span><span class="o">.</span><span class="n">time</span><span class="p">()</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">_start_time</span>
+</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a>            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_elapsed</span>
+</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a>
+</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a>    <span class="nd">@property</span>
+</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a>    <span class="k">def</span> <span class="nf">elapsed_str</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a>        <span class="sd">&quot;&quot;&quot;Return the currently elapsed time</span>
+</span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a><span class="sd">        as a formatted string.&quot;&quot;&quot;</span>
+</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">format_time</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">elapsed</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">subsecond_resolution</span><span class="p">)</span>
+</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a>
+</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a>    <span class="nd">@property</span>
+</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a>    <span class="k">def</span> <span class="nf">average_elapsed</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span><span class="p">:</span>
+</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_average_elapsed</span>
+</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a>
+</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a>    <span class="nd">@property</span>
+</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a>    <span class="k">def</span> <span class="nf">average_elapsed_str</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">format_time</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_average_elapsed</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">subsecond_resolution</span><span class="p">)</span>
+</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a>
+</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a>    <span class="nd">@property</span>
+</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a>    <span class="k">def</span> <span class="nf">start_time</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span><span class="p">:</span>
+</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_start_time</span>
 </span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a>
-</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>    <span class="k">def</span> <span class="nf">_save_elapsed_time</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>        <span class="sd">&quot;&quot;&quot;Saves current elapsed time to the history buffer</span>
-</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a><span class="sd">        in a FIFO manner.&quot;&quot;&quot;</span>
-</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">history</span><span class="p">)</span> <span class="o">&gt;=</span> <span class="bp">self</span><span class="o">.</span><span class="n">averaging_window_length</span><span class="p">:</span>
-</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">history</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
-</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">history</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">elapsed_time</span><span class="p">)</span>
-</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a>
-</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a>    <span class="k">def</span> <span class="nf">current_elapsed_time</span><span class="p">(</span>
-</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="nb">format</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span> <span class="n">subsecond_resolution</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span> <span class="o">|</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a>        <span class="sd">&quot;&quot;&quot;Returns current elapsed without stopping the timer.</span>
-</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a>
-</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a><span class="sd">        :param format: If True, elapsed time is returned as a string.</span>
-</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a><span class="sd">        If False, elapsed time is returned as a float.&quot;&quot;&quot;</span>
-</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>        <span class="n">warnings</span><span class="o">.</span><span class="n">warn</span><span class="p">(</span>
-</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>            <span class="s2">&quot;current_elapsed_time is depreciated. Use &#39;elapsed&#39; and &#39;elapsed_str&#39; properties instead.&quot;</span><span class="p">,</span>
-</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>            <span class="ne">FutureWarning</span><span class="p">,</span>
-</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>            <span class="mi">2</span><span class="p">,</span>
-</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>        <span class="p">)</span>
-</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">elapsed_time</span> <span class="o">=</span> <span class="p">(</span><span class="n">datetime</span><span class="o">.</span><span class="n">now</span><span class="p">()</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">start_time</span><span class="p">)</span><span class="o">.</span><span class="n">total_seconds</span><span class="p">()</span>
-</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>        <span class="k">return</span> <span class="p">(</span>
-</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">format_time</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">elapsed_time</span><span class="p">,</span> <span class="n">subsecond_resolution</span><span class="p">)</span>
-</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>            <span class="k">if</span> <span class="nb">format</span>
-</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>            <span class="k">else</span> <span class="bp">self</span><span class="o">.</span><span class="n">elapsed_time</span>
-</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>        <span class="p">)</span>
-</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>
-</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>    <span class="nd">@staticmethod</span>
-</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>    <span class="k">def</span> <span class="nf">format_time</span><span class="p">(</span><span class="n">num_seconds</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">subsecond_resolution</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>        <span class="sd">&quot;&quot;&quot;Returns num_seconds as a string with units.</span>
-</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>
-</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a><span class="sd">        :param subsecond_resolution: Include milliseconds</span>
-</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a><span class="sd">        and microseconds with the output.&quot;&quot;&quot;</span>
-</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>        <span class="n">microsecond</span> <span class="o">=</span> <span class="mf">0.000001</span>
-</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>        <span class="n">millisecond</span> <span class="o">=</span> <span class="mf">0.001</span>
-</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>        <span class="n">second</span> <span class="o">=</span> <span class="mi">1</span>
-</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>        <span class="n">seconds_per_minute</span> <span class="o">=</span> <span class="mi">60</span>
-</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>        <span class="n">seconds_per_hour</span> <span class="o">=</span> <span class="mi">3600</span>
-</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>        <span class="n">seconds_per_day</span> <span class="o">=</span> <span class="mi">86400</span>
-</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>        <span class="n">seconds_per_week</span> <span class="o">=</span> <span class="mi">604800</span>
-</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>        <span class="n">seconds_per_month</span> <span class="o">=</span> <span class="mi">2419200</span>
-</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>        <span class="n">seconds_per_year</span> <span class="o">=</span> <span class="mi">29030400</span>
-</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a>        <span class="n">time_units</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>            <span class="p">(</span><span class="n">seconds_per_year</span><span class="p">,</span> <span class="s2">&quot;y&quot;</span><span class="p">),</span>
-</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a>            <span class="p">(</span><span class="n">seconds_per_month</span><span class="p">,</span> <span class="s2">&quot;mn&quot;</span><span class="p">),</span>
-</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a>            <span class="p">(</span><span class="n">seconds_per_week</span><span class="p">,</span> <span class="s2">&quot;w&quot;</span><span class="p">),</span>
-</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a>            <span class="p">(</span><span class="n">seconds_per_day</span><span class="p">,</span> <span class="s2">&quot;d&quot;</span><span class="p">),</span>
-</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a>            <span class="p">(</span><span class="n">seconds_per_hour</span><span class="p">,</span> <span class="s2">&quot;h&quot;</span><span class="p">),</span>
-</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a>            <span class="p">(</span><span class="n">seconds_per_minute</span><span class="p">,</span> <span class="s2">&quot;m&quot;</span><span class="p">),</span>
-</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a>            <span class="p">(</span><span class="n">second</span><span class="p">,</span> <span class="s2">&quot;s&quot;</span><span class="p">),</span>
-</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a>            <span class="p">(</span><span class="n">millisecond</span><span class="p">,</span> <span class="s2">&quot;ms&quot;</span><span class="p">),</span>
-</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>            <span class="p">(</span><span class="n">microsecond</span><span class="p">,</span> <span class="s2">&quot;us&quot;</span><span class="p">),</span>
-</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>        <span class="p">]</span>
-</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">subsecond_resolution</span><span class="p">:</span>
-</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>            <span class="n">time_units</span> <span class="o">=</span> <span class="n">time_units</span><span class="p">[:</span><span class="o">-</span><span class="mi">2</span><span class="p">]</span>
-</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a>        <span class="n">time_string</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>        <span class="k">for</span> <span class="n">time_unit</span> <span class="ow">in</span> <span class="n">time_units</span><span class="p">:</span>
-</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>            <span class="n">unit_amount</span><span class="p">,</span> <span class="n">num_seconds</span> <span class="o">=</span> <span class="nb">divmod</span><span class="p">(</span><span class="n">num_seconds</span><span class="p">,</span> <span class="n">time_unit</span><span class="p">[</span><span class="mi">0</span><span class="p">])</span>
-</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>            <span class="k">if</span> <span class="n">unit_amount</span> <span class="o">&gt;</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a>                <span class="n">time_string</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">int</span><span class="p">(</span><span class="n">unit_amount</span><span class="p">)</span><span class="si">}{</span><span class="n">time_unit</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2"> &quot;</span>
-</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>        <span class="k">if</span> <span class="n">time_string</span> <span class="o">==</span> <span class="s2">&quot;&quot;</span><span class="p">:</span>
-</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a>            <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;&lt;1</span><span class="si">{</span><span class="n">time_units</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">][</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a>        <span class="k">return</span> <span class="n">time_string</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
-</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>
-</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>    <span class="k">def</span> <span class="nf">get_stats</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="nb">format</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span> <span class="n">subsecond_resolution</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a>        <span class="sd">&quot;&quot;&quot;Returns string for elapsed time and average elapsed time.</span>
-</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>
-</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a><span class="sd">        :param format: Times are returned as strings if True,</span>
-</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a><span class="sd">        otherwise they&#39;re raw floats.</span>
-</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a>
-</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a><span class="sd">        :param subsecond_resolution: Include milliseconds</span>
-</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a><span class="sd">        and microseconds with the output.&quot;&quot;&quot;</span>
-</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a>        <span class="k">if</span> <span class="nb">format</span><span class="p">:</span>
-</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a>            <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;elapsed time: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">format_time</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">elapsed_time</span><span class="p">,</span> <span class="n">subsecond_resolution</span><span class="p">)</span><span class="si">}</span><span class="se">\n</span><span class="s2">average elapsed time: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">format_time</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">average_elapsed_time</span><span class="p">,</span> <span class="n">subsecond_resolution</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a>            <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;elapsed time: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">elapsed_time</span><span class="si">}</span><span class="s2">s</span><span class="se">\n</span><span class="s2">average elapsed time: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">average_elapsed_time</span><span class="si">}</span><span class="s2">s&quot;</span>
+</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>    <span class="nd">@property</span>
+</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>    <span class="k">def</span> <span class="nf">stop_time</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span><span class="p">:</span>
+</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_stop_time</span>
+</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>
+</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>    <span class="nd">@property</span>
+</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>    <span class="k">def</span> <span class="nf">history</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">float</span><span class="p">]:</span>
+</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_history</span>
+</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a>
+</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a>    <span class="k">def</span> <span class="nf">start</span><span class="p">(</span><span class="bp">self</span><span class="p">:</span> <span class="n">Self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
+</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>        <span class="sd">&quot;&quot;&quot;Start timer.</span>
+</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a><span class="sd">        Returns this Timer instance so</span>
+</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a><span class="sd">        timer start can be chained to</span>
+</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a><span class="sd">        Timer creation.</span>
+</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a>
+</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a><span class="sd">        &gt;&gt;&gt; timer = Timer().start()&quot;&quot;&quot;</span>
+</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_start_time</span> <span class="o">=</span> <span class="n">time</span><span class="o">.</span><span class="n">time</span><span class="p">()</span>
+</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_started</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>        <span class="k">return</span> <span class="bp">self</span>
+</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>
+</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>    <span class="k">def</span> <span class="nf">stop</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>        <span class="sd">&quot;&quot;&quot;Stop timer.</span>
+</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a>
+</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a><span class="sd">        Calculates elapsed time and average elapsed time.&quot;&quot;&quot;</span>
+</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_stop_time</span> <span class="o">=</span> <span class="n">time</span><span class="o">.</span><span class="n">time</span><span class="p">()</span>
+</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_started</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_elapsed</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_stop_time</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">_start_time</span>
+</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_save_elapsed_time</span><span class="p">()</span>
+</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_average_elapsed</span> <span class="o">=</span> <span class="nb">sum</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_history</span><span class="p">)</span> <span class="o">/</span> <span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_history</span><span class="p">))</span>
+</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>
+</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>    <span class="k">def</span> <span class="nf">_save_elapsed_time</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>        <span class="sd">&quot;&quot;&quot;Saves current elapsed time to the history buffer</span>
+</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a><span class="sd">        in a FIFO manner.&quot;&quot;&quot;</span>
+</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_history</span><span class="p">)</span> <span class="o">&gt;=</span> <span class="bp">self</span><span class="o">.</span><span class="n">averaging_window_length</span><span class="p">:</span>
+</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_history</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
+</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_history</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_elapsed</span><span class="p">)</span>
+</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>
+</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>    <span class="nd">@staticmethod</span>
+</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>    <span class="k">def</span> <span class="nf">format_time</span><span class="p">(</span><span class="n">num_seconds</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">subsecond_resolution</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>        <span class="sd">&quot;&quot;&quot;Returns num_seconds as a string with units.</span>
+</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>
+</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a><span class="sd">        :param subsecond_resolution: Include milliseconds</span>
+</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a><span class="sd">        and microseconds with the output.&quot;&quot;&quot;</span>
+</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>        <span class="n">microsecond</span> <span class="o">=</span> <span class="mf">0.000001</span>
+</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a>        <span class="n">millisecond</span> <span class="o">=</span> <span class="mf">0.001</span>
+</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a>        <span class="n">second</span> <span class="o">=</span> <span class="mi">1</span>
+</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a>        <span class="n">seconds_per_minute</span> <span class="o">=</span> <span class="mi">60</span>
+</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a>        <span class="n">seconds_per_hour</span> <span class="o">=</span> <span class="mi">3600</span>
+</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a>        <span class="n">seconds_per_day</span> <span class="o">=</span> <span class="mi">86400</span>
+</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a>        <span class="n">seconds_per_week</span> <span class="o">=</span> <span class="mi">604800</span>
+</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a>        <span class="n">seconds_per_month</span> <span class="o">=</span> <span class="mi">2419200</span>
+</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>        <span class="n">seconds_per_year</span> <span class="o">=</span> <span class="mi">29030400</span>
+</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>        <span class="n">time_units</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>            <span class="p">(</span><span class="n">seconds_per_year</span><span class="p">,</span> <span class="s2">&quot;y&quot;</span><span class="p">),</span>
+</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>            <span class="p">(</span><span class="n">seconds_per_month</span><span class="p">,</span> <span class="s2">&quot;mn&quot;</span><span class="p">),</span>
+</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a>            <span class="p">(</span><span class="n">seconds_per_week</span><span class="p">,</span> <span class="s2">&quot;w&quot;</span><span class="p">),</span>
+</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>            <span class="p">(</span><span class="n">seconds_per_day</span><span class="p">,</span> <span class="s2">&quot;d&quot;</span><span class="p">),</span>
+</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>            <span class="p">(</span><span class="n">seconds_per_hour</span><span class="p">,</span> <span class="s2">&quot;h&quot;</span><span class="p">),</span>
+</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>            <span class="p">(</span><span class="n">seconds_per_minute</span><span class="p">,</span> <span class="s2">&quot;m&quot;</span><span class="p">),</span>
+</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a>            <span class="p">(</span><span class="n">second</span><span class="p">,</span> <span class="s2">&quot;s&quot;</span><span class="p">),</span>
+</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>            <span class="p">(</span><span class="n">millisecond</span><span class="p">,</span> <span class="s2">&quot;ms&quot;</span><span class="p">),</span>
+</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a>            <span class="p">(</span><span class="n">microsecond</span><span class="p">,</span> <span class="s2">&quot;us&quot;</span><span class="p">),</span>
+</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a>        <span class="p">]</span>
+</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">subsecond_resolution</span><span class="p">:</span>
+</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>            <span class="n">time_units</span> <span class="o">=</span> <span class="n">time_units</span><span class="p">[:</span><span class="o">-</span><span class="mi">2</span><span class="p">]</span>
+</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a>        <span class="n">time_string</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>        <span class="k">for</span> <span class="n">time_unit</span> <span class="ow">in</span> <span class="n">time_units</span><span class="p">:</span>
+</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a>            <span class="n">unit_amount</span><span class="p">,</span> <span class="n">num_seconds</span> <span class="o">=</span> <span class="nb">divmod</span><span class="p">(</span><span class="n">num_seconds</span><span class="p">,</span> <span class="n">time_unit</span><span class="p">[</span><span class="mi">0</span><span class="p">])</span>
+</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a>            <span class="k">if</span> <span class="n">unit_amount</span> <span class="o">&gt;</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a>                <span class="n">time_string</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">int</span><span class="p">(</span><span class="n">unit_amount</span><span class="p">)</span><span class="si">}{</span><span class="n">time_unit</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2"> &quot;</span>
+</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>        <span class="k">if</span> <span class="n">time_string</span> <span class="o">==</span> <span class="s2">&quot;&quot;</span><span class="p">:</span>
+</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a>            <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;&lt;1</span><span class="si">{</span><span class="n">time_units</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">][</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a>        <span class="k">return</span> <span class="n">time_string</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
+</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a>
+</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a>    <span class="nd">@property</span>
+</span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a>    <span class="k">def</span> <span class="nf">stats</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a>        <span class="sd">&quot;&quot;&quot;Returns a string stating the currently elapsed time</span>
+</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a><span class="sd">        and the average elapsed time.&quot;&quot;&quot;</span>
+</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;elapsed time: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">elapsed_str</span><span class="si">}</span><span class="se">\n</span><span class="s2">average elapsed time: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">average_elapsed_str</span><span class="si">}</span><span class="s2">&quot;</span>
 </span></pre></div>
 
 
             </section>
                 <section id="time_it">
                             <input id="time_it-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -255,36 +258,38 @@
         <span class="def">def</span>
         <span class="name">time_it</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">loops</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">1</span></span><span class="return-annotation">) -> <span class="n">Callable</span><span class="p">[</span><span class="o">...</span><span class="p">,</span> <span class="n">Any</span><span class="p">]</span>:</span></span>
 
                 <label class="view-source-button" for="time_it-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#time_it"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="time_it-7"><a href="#time_it-7"><span class="linenos"> 7</span></a><span class="k">def</span> <span class="nf">time_it</span><span class="p">(</span><span class="n">loops</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">1</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Callable</span><span class="p">[</span><span class="o">...</span><span class="p">,</span> <span class="n">Any</span><span class="p">]:</span>
-</span><span id="time_it-8"><a href="#time_it-8"><span class="linenos"> 8</span></a>    <span class="sd">&quot;&quot;&quot;Decorator to time function execution time</span>
-</span><span id="time_it-9"><a href="#time_it-9"><span class="linenos"> 9</span></a><span class="sd">    and print the results.</span>
-</span><span id="time_it-10"><a href="#time_it-10"><span class="linenos">10</span></a>
-</span><span id="time_it-11"><a href="#time_it-11"><span class="linenos">11</span></a><span class="sd">    :param loops: How many times to loop the function,</span>
-</span><span id="time_it-12"><a href="#time_it-12"><span class="linenos">12</span></a><span class="sd">    starting and stopping the timer before and after</span>
-</span><span id="time_it-13"><a href="#time_it-13"><span class="linenos">13</span></a><span class="sd">    each loop.&quot;&quot;&quot;</span>
-</span><span id="time_it-14"><a href="#time_it-14"><span class="linenos">14</span></a>
-</span><span id="time_it-15"><a href="#time_it-15"><span class="linenos">15</span></a>    <span class="k">def</span> <span class="nf">decorator</span><span class="p">(</span><span class="n">func</span><span class="p">:</span> <span class="n">Callable</span><span class="p">[</span><span class="o">...</span><span class="p">,</span> <span class="n">Any</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="n">Callable</span><span class="p">[</span><span class="o">...</span><span class="p">,</span> <span class="n">Any</span><span class="p">]:</span>
-</span><span id="time_it-16"><a href="#time_it-16"><span class="linenos">16</span></a>        <span class="k">def</span> <span class="nf">wrapper</span><span class="p">(</span><span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
-</span><span id="time_it-17"><a href="#time_it-17"><span class="linenos">17</span></a>            <span class="n">timer</span> <span class="o">=</span> <span class="n">Timer</span><span class="p">(</span><span class="n">loops</span><span class="p">)</span>
-</span><span id="time_it-18"><a href="#time_it-18"><span class="linenos">18</span></a>            <span class="k">for</span> <span class="n">_</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="n">loops</span><span class="p">):</span>
-</span><span id="time_it-19"><a href="#time_it-19"><span class="linenos">19</span></a>                <span class="n">timer</span><span class="o">.</span><span class="n">start</span><span class="p">()</span>
-</span><span id="time_it-20"><a href="#time_it-20"><span class="linenos">20</span></a>                <span class="n">result</span> <span class="o">=</span> <span class="n">func</span><span class="p">(</span><span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">)</span>
-</span><span id="time_it-21"><a href="#time_it-21"><span class="linenos">21</span></a>                <span class="n">timer</span><span class="o">.</span><span class="n">stop</span><span class="p">()</span>
-</span><span id="time_it-22"><a href="#time_it-22"><span class="linenos">22</span></a>            <span class="n">execution_time</span> <span class="o">=</span> <span class="n">timer</span><span class="o">.</span><span class="n">format_time</span><span class="p">(</span><span class="n">timer</span><span class="o">.</span><span class="n">average_elapsed_time</span><span class="p">,</span> <span class="kc">True</span><span class="p">)</span>
-</span><span id="time_it-23"><a href="#time_it-23"><span class="linenos">23</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">func</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2"> average execution time: </span><span class="si">{</span><span class="n">execution_time</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="time_it-24"><a href="#time_it-24"><span class="linenos">24</span></a>            <span class="k">return</span> <span class="n">result</span>
-</span><span id="time_it-25"><a href="#time_it-25"><span class="linenos">25</span></a>
-</span><span id="time_it-26"><a href="#time_it-26"><span class="linenos">26</span></a>        <span class="k">return</span> <span class="n">wrapper</span>
-</span><span id="time_it-27"><a href="#time_it-27"><span class="linenos">27</span></a>
-</span><span id="time_it-28"><a href="#time_it-28"><span class="linenos">28</span></a>    <span class="k">return</span> <span class="n">decorator</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="time_it-8"><a href="#time_it-8"><span class="linenos"> 8</span></a><span class="k">def</span> <span class="nf">time_it</span><span class="p">(</span><span class="n">loops</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">1</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Callable</span><span class="p">[</span><span class="o">...</span><span class="p">,</span> <span class="n">Any</span><span class="p">]:</span>
+</span><span id="time_it-9"><a href="#time_it-9"><span class="linenos"> 9</span></a>    <span class="sd">&quot;&quot;&quot;Decorator to time function execution time</span>
+</span><span id="time_it-10"><a href="#time_it-10"><span class="linenos">10</span></a><span class="sd">    and print the results.</span>
+</span><span id="time_it-11"><a href="#time_it-11"><span class="linenos">11</span></a>
+</span><span id="time_it-12"><a href="#time_it-12"><span class="linenos">12</span></a><span class="sd">    :param loops: How many times to loop the function,</span>
+</span><span id="time_it-13"><a href="#time_it-13"><span class="linenos">13</span></a><span class="sd">    starting and stopping the timer before and after</span>
+</span><span id="time_it-14"><a href="#time_it-14"><span class="linenos">14</span></a><span class="sd">    each loop.&quot;&quot;&quot;</span>
+</span><span id="time_it-15"><a href="#time_it-15"><span class="linenos">15</span></a>
+</span><span id="time_it-16"><a href="#time_it-16"><span class="linenos">16</span></a>    <span class="k">def</span> <span class="nf">decorator</span><span class="p">(</span><span class="n">func</span><span class="p">:</span> <span class="n">Callable</span><span class="p">[</span><span class="o">...</span><span class="p">,</span> <span class="n">Any</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="n">Callable</span><span class="p">[</span><span class="o">...</span><span class="p">,</span> <span class="n">Any</span><span class="p">]:</span>
+</span><span id="time_it-17"><a href="#time_it-17"><span class="linenos">17</span></a>        <span class="k">def</span> <span class="nf">wrapper</span><span class="p">(</span><span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
+</span><span id="time_it-18"><a href="#time_it-18"><span class="linenos">18</span></a>            <span class="n">timer</span> <span class="o">=</span> <span class="n">Timer</span><span class="p">(</span><span class="n">loops</span><span class="p">)</span>
+</span><span id="time_it-19"><a href="#time_it-19"><span class="linenos">19</span></a>            <span class="n">result</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="time_it-20"><a href="#time_it-20"><span class="linenos">20</span></a>            <span class="k">for</span> <span class="n">_</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="n">loops</span><span class="p">):</span>
+</span><span id="time_it-21"><a href="#time_it-21"><span class="linenos">21</span></a>                <span class="n">timer</span><span class="o">.</span><span class="n">start</span><span class="p">()</span>
+</span><span id="time_it-22"><a href="#time_it-22"><span class="linenos">22</span></a>                <span class="n">result</span> <span class="o">=</span> <span class="n">func</span><span class="p">(</span><span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">)</span>
+</span><span id="time_it-23"><a href="#time_it-23"><span class="linenos">23</span></a>                <span class="n">timer</span><span class="o">.</span><span class="n">stop</span><span class="p">()</span>
+</span><span id="time_it-24"><a href="#time_it-24"><span class="linenos">24</span></a>            <span class="nb">print</span><span class="p">(</span>
+</span><span id="time_it-25"><a href="#time_it-25"><span class="linenos">25</span></a>                <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">func</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2"> average execution time: </span><span class="si">{</span><span class="n">timer</span><span class="o">.</span><span class="n">average_elapsed_str</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="time_it-26"><a href="#time_it-26"><span class="linenos">26</span></a>            <span class="p">)</span>
+</span><span id="time_it-27"><a href="#time_it-27"><span class="linenos">27</span></a>            <span class="k">return</span> <span class="n">result</span>
+</span><span id="time_it-28"><a href="#time_it-28"><span class="linenos">28</span></a>
+</span><span id="time_it-29"><a href="#time_it-29"><span class="linenos">29</span></a>        <span class="k">return</span> <span class="n">wrapper</span>
+</span><span id="time_it-30"><a href="#time_it-30"><span class="linenos">30</span></a>
+</span><span id="time_it-31"><a href="#time_it-31"><span class="linenos">31</span></a>    <span class="k">return</span> <span class="n">decorator</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Decorator to time function execution time
 and print the results.</p>
 
 <h6 id="parameters">Parameters</h6>
@@ -305,145 +310,145 @@
     <span class="def">class</span>
     <span class="name">Timer</span>:
 
                 <label class="view-source-button" for="Timer-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Timer"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Timer-31"><a href="#Timer-31"><span class="linenos"> 31</span></a><span class="k">class</span> <span class="nc">Timer</span><span class="p">:</span>
-</span><span id="Timer-32"><a href="#Timer-32"><span class="linenos"> 32</span></a>    <span class="sd">&quot;&quot;&quot;Simple timer class that tracks total elapsed time</span>
-</span><span id="Timer-33"><a href="#Timer-33"><span class="linenos"> 33</span></a><span class="sd">    and average time between calls to &#39;start&#39; and &#39;stop&#39;.&quot;&quot;&quot;</span>
-</span><span id="Timer-34"><a href="#Timer-34"><span class="linenos"> 34</span></a>
-</span><span id="Timer-35"><a href="#Timer-35"><span class="linenos"> 35</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
-</span><span id="Timer-36"><a href="#Timer-36"><span class="linenos"> 36</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">averaging_window_length</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">10</span><span class="p">,</span> <span class="n">subsecond_resolution</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="Timer-37"><a href="#Timer-37"><span class="linenos"> 37</span></a>    <span class="p">):</span>
-</span><span id="Timer-38"><a href="#Timer-38"><span class="linenos"> 38</span></a>        <span class="sd">&quot;&quot;&quot;:param averaging_window_length: Number of start/stop cycles</span>
-</span><span id="Timer-39"><a href="#Timer-39"><span class="linenos"> 39</span></a><span class="sd">        to calculate the average elapsed time with.</span>
-</span><span id="Timer-40"><a href="#Timer-40"><span class="linenos"> 40</span></a>
-</span><span id="Timer-41"><a href="#Timer-41"><span class="linenos"> 41</span></a><span class="sd">        :param subsecond_resolution: Whether to print formatted time</span>
-</span><span id="Timer-42"><a href="#Timer-42"><span class="linenos"> 42</span></a><span class="sd">        strings with subsecond resolution or not.&quot;&quot;&quot;</span>
-</span><span id="Timer-43"><a href="#Timer-43"><span class="linenos"> 43</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">start_time</span><span class="p">:</span> <span class="n">datetime</span> <span class="o">=</span> <span class="n">datetime</span><span class="o">.</span><span class="n">now</span><span class="p">()</span>
-</span><span id="Timer-44"><a href="#Timer-44"><span class="linenos"> 44</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">stop_time</span><span class="p">:</span> <span class="n">datetime</span> <span class="o">=</span> <span class="n">datetime</span><span class="o">.</span><span class="n">now</span><span class="p">()</span>
-</span><span id="Timer-45"><a href="#Timer-45"><span class="linenos"> 45</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">average_elapsed_time</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="mi">0</span>
-</span><span id="Timer-46"><a href="#Timer-46"><span class="linenos"> 46</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">history</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">float</span><span class="p">]</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="Timer-47"><a href="#Timer-47"><span class="linenos"> 47</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">elapsed_time</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="mi">0</span>
-</span><span id="Timer-48"><a href="#Timer-48"><span class="linenos"> 48</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">averaging_window_length</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="n">averaging_window_length</span>
-</span><span id="Timer-49"><a href="#Timer-49"><span class="linenos"> 49</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">started</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="Timer-50"><a href="#Timer-50"><span class="linenos"> 50</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">subsecond_resolution</span> <span class="o">=</span> <span class="n">subsecond_resolution</span>
-</span><span id="Timer-51"><a href="#Timer-51"><span class="linenos"> 51</span></a>
-</span><span id="Timer-52"><a href="#Timer-52"><span class="linenos"> 52</span></a>    <span class="nd">@property</span>
-</span><span id="Timer-53"><a href="#Timer-53"><span class="linenos"> 53</span></a>    <span class="k">def</span> <span class="nf">elapsed</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span><span class="p">:</span>
-</span><span id="Timer-54"><a href="#Timer-54"><span class="linenos"> 54</span></a>        <span class="sd">&quot;&quot;&quot;Return the currently elapsed time.&quot;&quot;&quot;</span>
-</span><span id="Timer-55"><a href="#Timer-55"><span class="linenos"> 55</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">started</span><span class="p">:</span>
-</span><span id="Timer-56"><a href="#Timer-56"><span class="linenos"> 56</span></a>            <span class="k">return</span> <span class="p">(</span><span class="n">datetime</span><span class="o">.</span><span class="n">now</span><span class="p">()</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">start_time</span><span class="p">)</span><span class="o">.</span><span class="n">total_seconds</span><span class="p">()</span>
-</span><span id="Timer-57"><a href="#Timer-57"><span class="linenos"> 57</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="Timer-58"><a href="#Timer-58"><span class="linenos"> 58</span></a>            <span class="k">return</span> <span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">stop_time</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">start_time</span><span class="p">)</span><span class="o">.</span><span class="n">total_seconds</span><span class="p">()</span>
-</span><span id="Timer-59"><a href="#Timer-59"><span class="linenos"> 59</span></a>
-</span><span id="Timer-60"><a href="#Timer-60"><span class="linenos"> 60</span></a>    <span class="nd">@property</span>
-</span><span id="Timer-61"><a href="#Timer-61"><span class="linenos"> 61</span></a>    <span class="k">def</span> <span class="nf">elapsed_str</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="Timer-62"><a href="#Timer-62"><span class="linenos"> 62</span></a>        <span class="sd">&quot;&quot;&quot;Return the currently elapsed time</span>
-</span><span id="Timer-63"><a href="#Timer-63"><span class="linenos"> 63</span></a><span class="sd">        as a formatted string.&quot;&quot;&quot;</span>
-</span><span id="Timer-64"><a href="#Timer-64"><span class="linenos"> 64</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">format_time</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">elapsed</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">subsecond_resolution</span><span class="p">)</span>
-</span><span id="Timer-65"><a href="#Timer-65"><span class="linenos"> 65</span></a>
-</span><span id="Timer-66"><a href="#Timer-66"><span class="linenos"> 66</span></a>    <span class="k">def</span> <span class="nf">start</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
-</span><span id="Timer-67"><a href="#Timer-67"><span class="linenos"> 67</span></a>        <span class="sd">&quot;&quot;&quot;Start timer.</span>
-</span><span id="Timer-68"><a href="#Timer-68"><span class="linenos"> 68</span></a><span class="sd">        Returns this Timer instance so</span>
-</span><span id="Timer-69"><a href="#Timer-69"><span class="linenos"> 69</span></a><span class="sd">        timer start can be chained to</span>
-</span><span id="Timer-70"><a href="#Timer-70"><span class="linenos"> 70</span></a><span class="sd">        Timer creation.</span>
-</span><span id="Timer-71"><a href="#Timer-71"><span class="linenos"> 71</span></a>
-</span><span id="Timer-72"><a href="#Timer-72"><span class="linenos"> 72</span></a><span class="sd">        &gt;&gt;&gt; timer = Timer().start()&quot;&quot;&quot;</span>
-</span><span id="Timer-73"><a href="#Timer-73"><span class="linenos"> 73</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">start_time</span> <span class="o">=</span> <span class="n">datetime</span><span class="o">.</span><span class="n">now</span><span class="p">()</span>
-</span><span id="Timer-74"><a href="#Timer-74"><span class="linenos"> 74</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">started</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="Timer-75"><a href="#Timer-75"><span class="linenos"> 75</span></a>        <span class="k">return</span> <span class="bp">self</span>
-</span><span id="Timer-76"><a href="#Timer-76"><span class="linenos"> 76</span></a>
-</span><span id="Timer-77"><a href="#Timer-77"><span class="linenos"> 77</span></a>    <span class="k">def</span> <span class="nf">stop</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Timer-78"><a href="#Timer-78"><span class="linenos"> 78</span></a>        <span class="sd">&quot;&quot;&quot;Stop timer.</span>
-</span><span id="Timer-79"><a href="#Timer-79"><span class="linenos"> 79</span></a>
-</span><span id="Timer-80"><a href="#Timer-80"><span class="linenos"> 80</span></a><span class="sd">        Calculates elapsed time and average elapsed time.&quot;&quot;&quot;</span>
-</span><span id="Timer-81"><a href="#Timer-81"><span class="linenos"> 81</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">stop_time</span> <span class="o">=</span> <span class="n">datetime</span><span class="o">.</span><span class="n">now</span><span class="p">()</span>
-</span><span id="Timer-82"><a href="#Timer-82"><span class="linenos"> 82</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">started</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="Timer-83"><a href="#Timer-83"><span class="linenos"> 83</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">elapsed_time</span> <span class="o">=</span> <span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">stop_time</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">start_time</span><span class="p">)</span><span class="o">.</span><span class="n">total_seconds</span><span class="p">()</span>
-</span><span id="Timer-84"><a href="#Timer-84"><span class="linenos"> 84</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_save_elapsed_time</span><span class="p">()</span>
-</span><span id="Timer-85"><a href="#Timer-85"><span class="linenos"> 85</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">average_elapsed_time</span> <span class="o">=</span> <span class="nb">sum</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">history</span><span class="p">)</span> <span class="o">/</span> <span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">history</span><span class="p">))</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Timer-34"><a href="#Timer-34"><span class="linenos"> 34</span></a><span class="k">class</span> <span class="nc">Timer</span><span class="p">:</span>
+</span><span id="Timer-35"><a href="#Timer-35"><span class="linenos"> 35</span></a>    <span class="sd">&quot;&quot;&quot;Simple timer class that tracks total elapsed time</span>
+</span><span id="Timer-36"><a href="#Timer-36"><span class="linenos"> 36</span></a><span class="sd">    and average time between calls to &#39;start&#39; and &#39;stop&#39;.&quot;&quot;&quot;</span>
+</span><span id="Timer-37"><a href="#Timer-37"><span class="linenos"> 37</span></a>
+</span><span id="Timer-38"><a href="#Timer-38"><span class="linenos"> 38</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
+</span><span id="Timer-39"><a href="#Timer-39"><span class="linenos"> 39</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">averaging_window_length</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">10</span><span class="p">,</span> <span class="n">subsecond_resolution</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="Timer-40"><a href="#Timer-40"><span class="linenos"> 40</span></a>    <span class="p">):</span>
+</span><span id="Timer-41"><a href="#Timer-41"><span class="linenos"> 41</span></a>        <span class="sd">&quot;&quot;&quot;:param averaging_window_length: Number of start/stop cycles</span>
+</span><span id="Timer-42"><a href="#Timer-42"><span class="linenos"> 42</span></a><span class="sd">        to calculate the average elapsed time with.</span>
+</span><span id="Timer-43"><a href="#Timer-43"><span class="linenos"> 43</span></a>
+</span><span id="Timer-44"><a href="#Timer-44"><span class="linenos"> 44</span></a><span class="sd">        :param subsecond_resolution: Whether to print formatted time</span>
+</span><span id="Timer-45"><a href="#Timer-45"><span class="linenos"> 45</span></a><span class="sd">        strings with subsecond resolution or not.&quot;&quot;&quot;</span>
+</span><span id="Timer-46"><a href="#Timer-46"><span class="linenos"> 46</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_start_time</span> <span class="o">=</span> <span class="n">time</span><span class="o">.</span><span class="n">time</span><span class="p">()</span>
+</span><span id="Timer-47"><a href="#Timer-47"><span class="linenos"> 47</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_stop_time</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">start_time</span>
+</span><span id="Timer-48"><a href="#Timer-48"><span class="linenos"> 48</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_elapsed</span> <span class="o">=</span> <span class="mi">0</span>
+</span><span id="Timer-49"><a href="#Timer-49"><span class="linenos"> 49</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_average_elapsed</span> <span class="o">=</span> <span class="mi">0</span>
+</span><span id="Timer-50"><a href="#Timer-50"><span class="linenos"> 50</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_history</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">float</span><span class="p">]</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="Timer-51"><a href="#Timer-51"><span class="linenos"> 51</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_started</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="Timer-52"><a href="#Timer-52"><span class="linenos"> 52</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">averaging_window_length</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="n">averaging_window_length</span>
+</span><span id="Timer-53"><a href="#Timer-53"><span class="linenos"> 53</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">subsecond_resolution</span> <span class="o">=</span> <span class="n">subsecond_resolution</span>
+</span><span id="Timer-54"><a href="#Timer-54"><span class="linenos"> 54</span></a>
+</span><span id="Timer-55"><a href="#Timer-55"><span class="linenos"> 55</span></a>    <span class="nd">@property</span>
+</span><span id="Timer-56"><a href="#Timer-56"><span class="linenos"> 56</span></a>    <span class="k">def</span> <span class="nf">started</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="Timer-57"><a href="#Timer-57"><span class="linenos"> 57</span></a>        <span class="sd">&quot;&quot;&quot;Returns whether the timer has</span>
+</span><span id="Timer-58"><a href="#Timer-58"><span class="linenos"> 58</span></a><span class="sd">        been started and is currently running.&quot;&quot;&quot;</span>
+</span><span id="Timer-59"><a href="#Timer-59"><span class="linenos"> 59</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_started</span>
+</span><span id="Timer-60"><a href="#Timer-60"><span class="linenos"> 60</span></a>
+</span><span id="Timer-61"><a href="#Timer-61"><span class="linenos"> 61</span></a>    <span class="nd">@property</span>
+</span><span id="Timer-62"><a href="#Timer-62"><span class="linenos"> 62</span></a>    <span class="k">def</span> <span class="nf">elapsed</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span><span class="p">:</span>
+</span><span id="Timer-63"><a href="#Timer-63"><span class="linenos"> 63</span></a>        <span class="sd">&quot;&quot;&quot;Return the currently elapsed time.&quot;&quot;&quot;</span>
+</span><span id="Timer-64"><a href="#Timer-64"><span class="linenos"> 64</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_started</span><span class="p">:</span>
+</span><span id="Timer-65"><a href="#Timer-65"><span class="linenos"> 65</span></a>            <span class="k">return</span> <span class="n">time</span><span class="o">.</span><span class="n">time</span><span class="p">()</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">_start_time</span>
+</span><span id="Timer-66"><a href="#Timer-66"><span class="linenos"> 66</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="Timer-67"><a href="#Timer-67"><span class="linenos"> 67</span></a>            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_elapsed</span>
+</span><span id="Timer-68"><a href="#Timer-68"><span class="linenos"> 68</span></a>
+</span><span id="Timer-69"><a href="#Timer-69"><span class="linenos"> 69</span></a>    <span class="nd">@property</span>
+</span><span id="Timer-70"><a href="#Timer-70"><span class="linenos"> 70</span></a>    <span class="k">def</span> <span class="nf">elapsed_str</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="Timer-71"><a href="#Timer-71"><span class="linenos"> 71</span></a>        <span class="sd">&quot;&quot;&quot;Return the currently elapsed time</span>
+</span><span id="Timer-72"><a href="#Timer-72"><span class="linenos"> 72</span></a><span class="sd">        as a formatted string.&quot;&quot;&quot;</span>
+</span><span id="Timer-73"><a href="#Timer-73"><span class="linenos"> 73</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">format_time</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">elapsed</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">subsecond_resolution</span><span class="p">)</span>
+</span><span id="Timer-74"><a href="#Timer-74"><span class="linenos"> 74</span></a>
+</span><span id="Timer-75"><a href="#Timer-75"><span class="linenos"> 75</span></a>    <span class="nd">@property</span>
+</span><span id="Timer-76"><a href="#Timer-76"><span class="linenos"> 76</span></a>    <span class="k">def</span> <span class="nf">average_elapsed</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span><span class="p">:</span>
+</span><span id="Timer-77"><a href="#Timer-77"><span class="linenos"> 77</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_average_elapsed</span>
+</span><span id="Timer-78"><a href="#Timer-78"><span class="linenos"> 78</span></a>
+</span><span id="Timer-79"><a href="#Timer-79"><span class="linenos"> 79</span></a>    <span class="nd">@property</span>
+</span><span id="Timer-80"><a href="#Timer-80"><span class="linenos"> 80</span></a>    <span class="k">def</span> <span class="nf">average_elapsed_str</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="Timer-81"><a href="#Timer-81"><span class="linenos"> 81</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">format_time</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_average_elapsed</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">subsecond_resolution</span><span class="p">)</span>
+</span><span id="Timer-82"><a href="#Timer-82"><span class="linenos"> 82</span></a>
+</span><span id="Timer-83"><a href="#Timer-83"><span class="linenos"> 83</span></a>    <span class="nd">@property</span>
+</span><span id="Timer-84"><a href="#Timer-84"><span class="linenos"> 84</span></a>    <span class="k">def</span> <span class="nf">start_time</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span><span class="p">:</span>
+</span><span id="Timer-85"><a href="#Timer-85"><span class="linenos"> 85</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_start_time</span>
 </span><span id="Timer-86"><a href="#Timer-86"><span class="linenos"> 86</span></a>
-</span><span id="Timer-87"><a href="#Timer-87"><span class="linenos"> 87</span></a>    <span class="k">def</span> <span class="nf">_save_elapsed_time</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Timer-88"><a href="#Timer-88"><span class="linenos"> 88</span></a>        <span class="sd">&quot;&quot;&quot;Saves current elapsed time to the history buffer</span>
-</span><span id="Timer-89"><a href="#Timer-89"><span class="linenos"> 89</span></a><span class="sd">        in a FIFO manner.&quot;&quot;&quot;</span>
-</span><span id="Timer-90"><a href="#Timer-90"><span class="linenos"> 90</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">history</span><span class="p">)</span> <span class="o">&gt;=</span> <span class="bp">self</span><span class="o">.</span><span class="n">averaging_window_length</span><span class="p">:</span>
-</span><span id="Timer-91"><a href="#Timer-91"><span class="linenos"> 91</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">history</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
-</span><span id="Timer-92"><a href="#Timer-92"><span class="linenos"> 92</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">history</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">elapsed_time</span><span class="p">)</span>
-</span><span id="Timer-93"><a href="#Timer-93"><span class="linenos"> 93</span></a>
-</span><span id="Timer-94"><a href="#Timer-94"><span class="linenos"> 94</span></a>    <span class="k">def</span> <span class="nf">current_elapsed_time</span><span class="p">(</span>
-</span><span id="Timer-95"><a href="#Timer-95"><span class="linenos"> 95</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="nb">format</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span> <span class="n">subsecond_resolution</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="Timer-96"><a href="#Timer-96"><span class="linenos"> 96</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span> <span class="o">|</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="Timer-97"><a href="#Timer-97"><span class="linenos"> 97</span></a>        <span class="sd">&quot;&quot;&quot;Returns current elapsed without stopping the timer.</span>
-</span><span id="Timer-98"><a href="#Timer-98"><span class="linenos"> 98</span></a>
-</span><span id="Timer-99"><a href="#Timer-99"><span class="linenos"> 99</span></a><span class="sd">        :param format: If True, elapsed time is returned as a string.</span>
-</span><span id="Timer-100"><a href="#Timer-100"><span class="linenos">100</span></a><span class="sd">        If False, elapsed time is returned as a float.&quot;&quot;&quot;</span>
-</span><span id="Timer-101"><a href="#Timer-101"><span class="linenos">101</span></a>        <span class="n">warnings</span><span class="o">.</span><span class="n">warn</span><span class="p">(</span>
-</span><span id="Timer-102"><a href="#Timer-102"><span class="linenos">102</span></a>            <span class="s2">&quot;current_elapsed_time is depreciated. Use &#39;elapsed&#39; and &#39;elapsed_str&#39; properties instead.&quot;</span><span class="p">,</span>
-</span><span id="Timer-103"><a href="#Timer-103"><span class="linenos">103</span></a>            <span class="ne">FutureWarning</span><span class="p">,</span>
-</span><span id="Timer-104"><a href="#Timer-104"><span class="linenos">104</span></a>            <span class="mi">2</span><span class="p">,</span>
-</span><span id="Timer-105"><a href="#Timer-105"><span class="linenos">105</span></a>        <span class="p">)</span>
-</span><span id="Timer-106"><a href="#Timer-106"><span class="linenos">106</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">elapsed_time</span> <span class="o">=</span> <span class="p">(</span><span class="n">datetime</span><span class="o">.</span><span class="n">now</span><span class="p">()</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">start_time</span><span class="p">)</span><span class="o">.</span><span class="n">total_seconds</span><span class="p">()</span>
-</span><span id="Timer-107"><a href="#Timer-107"><span class="linenos">107</span></a>        <span class="k">return</span> <span class="p">(</span>
-</span><span id="Timer-108"><a href="#Timer-108"><span class="linenos">108</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">format_time</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">elapsed_time</span><span class="p">,</span> <span class="n">subsecond_resolution</span><span class="p">)</span>
-</span><span id="Timer-109"><a href="#Timer-109"><span class="linenos">109</span></a>            <span class="k">if</span> <span class="nb">format</span>
-</span><span id="Timer-110"><a href="#Timer-110"><span class="linenos">110</span></a>            <span class="k">else</span> <span class="bp">self</span><span class="o">.</span><span class="n">elapsed_time</span>
-</span><span id="Timer-111"><a href="#Timer-111"><span class="linenos">111</span></a>        <span class="p">)</span>
-</span><span id="Timer-112"><a href="#Timer-112"><span class="linenos">112</span></a>
-</span><span id="Timer-113"><a href="#Timer-113"><span class="linenos">113</span></a>    <span class="nd">@staticmethod</span>
-</span><span id="Timer-114"><a href="#Timer-114"><span class="linenos">114</span></a>    <span class="k">def</span> <span class="nf">format_time</span><span class="p">(</span><span class="n">num_seconds</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">subsecond_resolution</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="Timer-115"><a href="#Timer-115"><span class="linenos">115</span></a>        <span class="sd">&quot;&quot;&quot;Returns num_seconds as a string with units.</span>
-</span><span id="Timer-116"><a href="#Timer-116"><span class="linenos">116</span></a>
-</span><span id="Timer-117"><a href="#Timer-117"><span class="linenos">117</span></a><span class="sd">        :param subsecond_resolution: Include milliseconds</span>
-</span><span id="Timer-118"><a href="#Timer-118"><span class="linenos">118</span></a><span class="sd">        and microseconds with the output.&quot;&quot;&quot;</span>
-</span><span id="Timer-119"><a href="#Timer-119"><span class="linenos">119</span></a>        <span class="n">microsecond</span> <span class="o">=</span> <span class="mf">0.000001</span>
-</span><span id="Timer-120"><a href="#Timer-120"><span class="linenos">120</span></a>        <span class="n">millisecond</span> <span class="o">=</span> <span class="mf">0.001</span>
-</span><span id="Timer-121"><a href="#Timer-121"><span class="linenos">121</span></a>        <span class="n">second</span> <span class="o">=</span> <span class="mi">1</span>
-</span><span id="Timer-122"><a href="#Timer-122"><span class="linenos">122</span></a>        <span class="n">seconds_per_minute</span> <span class="o">=</span> <span class="mi">60</span>
-</span><span id="Timer-123"><a href="#Timer-123"><span class="linenos">123</span></a>        <span class="n">seconds_per_hour</span> <span class="o">=</span> <span class="mi">3600</span>
-</span><span id="Timer-124"><a href="#Timer-124"><span class="linenos">124</span></a>        <span class="n">seconds_per_day</span> <span class="o">=</span> <span class="mi">86400</span>
-</span><span id="Timer-125"><a href="#Timer-125"><span class="linenos">125</span></a>        <span class="n">seconds_per_week</span> <span class="o">=</span> <span class="mi">604800</span>
-</span><span id="Timer-126"><a href="#Timer-126"><span class="linenos">126</span></a>        <span class="n">seconds_per_month</span> <span class="o">=</span> <span class="mi">2419200</span>
-</span><span id="Timer-127"><a href="#Timer-127"><span class="linenos">127</span></a>        <span class="n">seconds_per_year</span> <span class="o">=</span> <span class="mi">29030400</span>
-</span><span id="Timer-128"><a href="#Timer-128"><span class="linenos">128</span></a>        <span class="n">time_units</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="Timer-129"><a href="#Timer-129"><span class="linenos">129</span></a>            <span class="p">(</span><span class="n">seconds_per_year</span><span class="p">,</span> <span class="s2">&quot;y&quot;</span><span class="p">),</span>
-</span><span id="Timer-130"><a href="#Timer-130"><span class="linenos">130</span></a>            <span class="p">(</span><span class="n">seconds_per_month</span><span class="p">,</span> <span class="s2">&quot;mn&quot;</span><span class="p">),</span>
-</span><span id="Timer-131"><a href="#Timer-131"><span class="linenos">131</span></a>            <span class="p">(</span><span class="n">seconds_per_week</span><span class="p">,</span> <span class="s2">&quot;w&quot;</span><span class="p">),</span>
-</span><span id="Timer-132"><a href="#Timer-132"><span class="linenos">132</span></a>            <span class="p">(</span><span class="n">seconds_per_day</span><span class="p">,</span> <span class="s2">&quot;d&quot;</span><span class="p">),</span>
-</span><span id="Timer-133"><a href="#Timer-133"><span class="linenos">133</span></a>            <span class="p">(</span><span class="n">seconds_per_hour</span><span class="p">,</span> <span class="s2">&quot;h&quot;</span><span class="p">),</span>
-</span><span id="Timer-134"><a href="#Timer-134"><span class="linenos">134</span></a>            <span class="p">(</span><span class="n">seconds_per_minute</span><span class="p">,</span> <span class="s2">&quot;m&quot;</span><span class="p">),</span>
-</span><span id="Timer-135"><a href="#Timer-135"><span class="linenos">135</span></a>            <span class="p">(</span><span class="n">second</span><span class="p">,</span> <span class="s2">&quot;s&quot;</span><span class="p">),</span>
-</span><span id="Timer-136"><a href="#Timer-136"><span class="linenos">136</span></a>            <span class="p">(</span><span class="n">millisecond</span><span class="p">,</span> <span class="s2">&quot;ms&quot;</span><span class="p">),</span>
-</span><span id="Timer-137"><a href="#Timer-137"><span class="linenos">137</span></a>            <span class="p">(</span><span class="n">microsecond</span><span class="p">,</span> <span class="s2">&quot;us&quot;</span><span class="p">),</span>
-</span><span id="Timer-138"><a href="#Timer-138"><span class="linenos">138</span></a>        <span class="p">]</span>
-</span><span id="Timer-139"><a href="#Timer-139"><span class="linenos">139</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">subsecond_resolution</span><span class="p">:</span>
-</span><span id="Timer-140"><a href="#Timer-140"><span class="linenos">140</span></a>            <span class="n">time_units</span> <span class="o">=</span> <span class="n">time_units</span><span class="p">[:</span><span class="o">-</span><span class="mi">2</span><span class="p">]</span>
-</span><span id="Timer-141"><a href="#Timer-141"><span class="linenos">141</span></a>        <span class="n">time_string</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="Timer-142"><a href="#Timer-142"><span class="linenos">142</span></a>        <span class="k">for</span> <span class="n">time_unit</span> <span class="ow">in</span> <span class="n">time_units</span><span class="p">:</span>
-</span><span id="Timer-143"><a href="#Timer-143"><span class="linenos">143</span></a>            <span class="n">unit_amount</span><span class="p">,</span> <span class="n">num_seconds</span> <span class="o">=</span> <span class="nb">divmod</span><span class="p">(</span><span class="n">num_seconds</span><span class="p">,</span> <span class="n">time_unit</span><span class="p">[</span><span class="mi">0</span><span class="p">])</span>
-</span><span id="Timer-144"><a href="#Timer-144"><span class="linenos">144</span></a>            <span class="k">if</span> <span class="n">unit_amount</span> <span class="o">&gt;</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="Timer-145"><a href="#Timer-145"><span class="linenos">145</span></a>                <span class="n">time_string</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">int</span><span class="p">(</span><span class="n">unit_amount</span><span class="p">)</span><span class="si">}{</span><span class="n">time_unit</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2"> &quot;</span>
-</span><span id="Timer-146"><a href="#Timer-146"><span class="linenos">146</span></a>        <span class="k">if</span> <span class="n">time_string</span> <span class="o">==</span> <span class="s2">&quot;&quot;</span><span class="p">:</span>
-</span><span id="Timer-147"><a href="#Timer-147"><span class="linenos">147</span></a>            <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;&lt;1</span><span class="si">{</span><span class="n">time_units</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">][</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="Timer-148"><a href="#Timer-148"><span class="linenos">148</span></a>        <span class="k">return</span> <span class="n">time_string</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
-</span><span id="Timer-149"><a href="#Timer-149"><span class="linenos">149</span></a>
-</span><span id="Timer-150"><a href="#Timer-150"><span class="linenos">150</span></a>    <span class="k">def</span> <span class="nf">get_stats</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="nb">format</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span> <span class="n">subsecond_resolution</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="Timer-151"><a href="#Timer-151"><span class="linenos">151</span></a>        <span class="sd">&quot;&quot;&quot;Returns string for elapsed time and average elapsed time.</span>
-</span><span id="Timer-152"><a href="#Timer-152"><span class="linenos">152</span></a>
-</span><span id="Timer-153"><a href="#Timer-153"><span class="linenos">153</span></a><span class="sd">        :param format: Times are returned as strings if True,</span>
-</span><span id="Timer-154"><a href="#Timer-154"><span class="linenos">154</span></a><span class="sd">        otherwise they&#39;re raw floats.</span>
-</span><span id="Timer-155"><a href="#Timer-155"><span class="linenos">155</span></a>
-</span><span id="Timer-156"><a href="#Timer-156"><span class="linenos">156</span></a><span class="sd">        :param subsecond_resolution: Include milliseconds</span>
-</span><span id="Timer-157"><a href="#Timer-157"><span class="linenos">157</span></a><span class="sd">        and microseconds with the output.&quot;&quot;&quot;</span>
-</span><span id="Timer-158"><a href="#Timer-158"><span class="linenos">158</span></a>        <span class="k">if</span> <span class="nb">format</span><span class="p">:</span>
-</span><span id="Timer-159"><a href="#Timer-159"><span class="linenos">159</span></a>            <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;elapsed time: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">format_time</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">elapsed_time</span><span class="p">,</span> <span class="n">subsecond_resolution</span><span class="p">)</span><span class="si">}</span><span class="se">\n</span><span class="s2">average elapsed time: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">format_time</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">average_elapsed_time</span><span class="p">,</span> <span class="n">subsecond_resolution</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="Timer-160"><a href="#Timer-160"><span class="linenos">160</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="Timer-161"><a href="#Timer-161"><span class="linenos">161</span></a>            <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;elapsed time: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">elapsed_time</span><span class="si">}</span><span class="s2">s</span><span class="se">\n</span><span class="s2">average elapsed time: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">average_elapsed_time</span><span class="si">}</span><span class="s2">s&quot;</span>
+</span><span id="Timer-87"><a href="#Timer-87"><span class="linenos"> 87</span></a>    <span class="nd">@property</span>
+</span><span id="Timer-88"><a href="#Timer-88"><span class="linenos"> 88</span></a>    <span class="k">def</span> <span class="nf">stop_time</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span><span class="p">:</span>
+</span><span id="Timer-89"><a href="#Timer-89"><span class="linenos"> 89</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_stop_time</span>
+</span><span id="Timer-90"><a href="#Timer-90"><span class="linenos"> 90</span></a>
+</span><span id="Timer-91"><a href="#Timer-91"><span class="linenos"> 91</span></a>    <span class="nd">@property</span>
+</span><span id="Timer-92"><a href="#Timer-92"><span class="linenos"> 92</span></a>    <span class="k">def</span> <span class="nf">history</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">float</span><span class="p">]:</span>
+</span><span id="Timer-93"><a href="#Timer-93"><span class="linenos"> 93</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_history</span>
+</span><span id="Timer-94"><a href="#Timer-94"><span class="linenos"> 94</span></a>
+</span><span id="Timer-95"><a href="#Timer-95"><span class="linenos"> 95</span></a>    <span class="k">def</span> <span class="nf">start</span><span class="p">(</span><span class="bp">self</span><span class="p">:</span> <span class="n">Self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
+</span><span id="Timer-96"><a href="#Timer-96"><span class="linenos"> 96</span></a>        <span class="sd">&quot;&quot;&quot;Start timer.</span>
+</span><span id="Timer-97"><a href="#Timer-97"><span class="linenos"> 97</span></a><span class="sd">        Returns this Timer instance so</span>
+</span><span id="Timer-98"><a href="#Timer-98"><span class="linenos"> 98</span></a><span class="sd">        timer start can be chained to</span>
+</span><span id="Timer-99"><a href="#Timer-99"><span class="linenos"> 99</span></a><span class="sd">        Timer creation.</span>
+</span><span id="Timer-100"><a href="#Timer-100"><span class="linenos">100</span></a>
+</span><span id="Timer-101"><a href="#Timer-101"><span class="linenos">101</span></a><span class="sd">        &gt;&gt;&gt; timer = Timer().start()&quot;&quot;&quot;</span>
+</span><span id="Timer-102"><a href="#Timer-102"><span class="linenos">102</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_start_time</span> <span class="o">=</span> <span class="n">time</span><span class="o">.</span><span class="n">time</span><span class="p">()</span>
+</span><span id="Timer-103"><a href="#Timer-103"><span class="linenos">103</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_started</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="Timer-104"><a href="#Timer-104"><span class="linenos">104</span></a>        <span class="k">return</span> <span class="bp">self</span>
+</span><span id="Timer-105"><a href="#Timer-105"><span class="linenos">105</span></a>
+</span><span id="Timer-106"><a href="#Timer-106"><span class="linenos">106</span></a>    <span class="k">def</span> <span class="nf">stop</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Timer-107"><a href="#Timer-107"><span class="linenos">107</span></a>        <span class="sd">&quot;&quot;&quot;Stop timer.</span>
+</span><span id="Timer-108"><a href="#Timer-108"><span class="linenos">108</span></a>
+</span><span id="Timer-109"><a href="#Timer-109"><span class="linenos">109</span></a><span class="sd">        Calculates elapsed time and average elapsed time.&quot;&quot;&quot;</span>
+</span><span id="Timer-110"><a href="#Timer-110"><span class="linenos">110</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_stop_time</span> <span class="o">=</span> <span class="n">time</span><span class="o">.</span><span class="n">time</span><span class="p">()</span>
+</span><span id="Timer-111"><a href="#Timer-111"><span class="linenos">111</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_started</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="Timer-112"><a href="#Timer-112"><span class="linenos">112</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_elapsed</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_stop_time</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">_start_time</span>
+</span><span id="Timer-113"><a href="#Timer-113"><span class="linenos">113</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_save_elapsed_time</span><span class="p">()</span>
+</span><span id="Timer-114"><a href="#Timer-114"><span class="linenos">114</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_average_elapsed</span> <span class="o">=</span> <span class="nb">sum</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_history</span><span class="p">)</span> <span class="o">/</span> <span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_history</span><span class="p">))</span>
+</span><span id="Timer-115"><a href="#Timer-115"><span class="linenos">115</span></a>
+</span><span id="Timer-116"><a href="#Timer-116"><span class="linenos">116</span></a>    <span class="k">def</span> <span class="nf">_save_elapsed_time</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Timer-117"><a href="#Timer-117"><span class="linenos">117</span></a>        <span class="sd">&quot;&quot;&quot;Saves current elapsed time to the history buffer</span>
+</span><span id="Timer-118"><a href="#Timer-118"><span class="linenos">118</span></a><span class="sd">        in a FIFO manner.&quot;&quot;&quot;</span>
+</span><span id="Timer-119"><a href="#Timer-119"><span class="linenos">119</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_history</span><span class="p">)</span> <span class="o">&gt;=</span> <span class="bp">self</span><span class="o">.</span><span class="n">averaging_window_length</span><span class="p">:</span>
+</span><span id="Timer-120"><a href="#Timer-120"><span class="linenos">120</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_history</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
+</span><span id="Timer-121"><a href="#Timer-121"><span class="linenos">121</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_history</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_elapsed</span><span class="p">)</span>
+</span><span id="Timer-122"><a href="#Timer-122"><span class="linenos">122</span></a>
+</span><span id="Timer-123"><a href="#Timer-123"><span class="linenos">123</span></a>    <span class="nd">@staticmethod</span>
+</span><span id="Timer-124"><a href="#Timer-124"><span class="linenos">124</span></a>    <span class="k">def</span> <span class="nf">format_time</span><span class="p">(</span><span class="n">num_seconds</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">subsecond_resolution</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="Timer-125"><a href="#Timer-125"><span class="linenos">125</span></a>        <span class="sd">&quot;&quot;&quot;Returns num_seconds as a string with units.</span>
+</span><span id="Timer-126"><a href="#Timer-126"><span class="linenos">126</span></a>
+</span><span id="Timer-127"><a href="#Timer-127"><span class="linenos">127</span></a><span class="sd">        :param subsecond_resolution: Include milliseconds</span>
+</span><span id="Timer-128"><a href="#Timer-128"><span class="linenos">128</span></a><span class="sd">        and microseconds with the output.&quot;&quot;&quot;</span>
+</span><span id="Timer-129"><a href="#Timer-129"><span class="linenos">129</span></a>        <span class="n">microsecond</span> <span class="o">=</span> <span class="mf">0.000001</span>
+</span><span id="Timer-130"><a href="#Timer-130"><span class="linenos">130</span></a>        <span class="n">millisecond</span> <span class="o">=</span> <span class="mf">0.001</span>
+</span><span id="Timer-131"><a href="#Timer-131"><span class="linenos">131</span></a>        <span class="n">second</span> <span class="o">=</span> <span class="mi">1</span>
+</span><span id="Timer-132"><a href="#Timer-132"><span class="linenos">132</span></a>        <span class="n">seconds_per_minute</span> <span class="o">=</span> <span class="mi">60</span>
+</span><span id="Timer-133"><a href="#Timer-133"><span class="linenos">133</span></a>        <span class="n">seconds_per_hour</span> <span class="o">=</span> <span class="mi">3600</span>
+</span><span id="Timer-134"><a href="#Timer-134"><span class="linenos">134</span></a>        <span class="n">seconds_per_day</span> <span class="o">=</span> <span class="mi">86400</span>
+</span><span id="Timer-135"><a href="#Timer-135"><span class="linenos">135</span></a>        <span class="n">seconds_per_week</span> <span class="o">=</span> <span class="mi">604800</span>
+</span><span id="Timer-136"><a href="#Timer-136"><span class="linenos">136</span></a>        <span class="n">seconds_per_month</span> <span class="o">=</span> <span class="mi">2419200</span>
+</span><span id="Timer-137"><a href="#Timer-137"><span class="linenos">137</span></a>        <span class="n">seconds_per_year</span> <span class="o">=</span> <span class="mi">29030400</span>
+</span><span id="Timer-138"><a href="#Timer-138"><span class="linenos">138</span></a>        <span class="n">time_units</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="Timer-139"><a href="#Timer-139"><span class="linenos">139</span></a>            <span class="p">(</span><span class="n">seconds_per_year</span><span class="p">,</span> <span class="s2">&quot;y&quot;</span><span class="p">),</span>
+</span><span id="Timer-140"><a href="#Timer-140"><span class="linenos">140</span></a>            <span class="p">(</span><span class="n">seconds_per_month</span><span class="p">,</span> <span class="s2">&quot;mn&quot;</span><span class="p">),</span>
+</span><span id="Timer-141"><a href="#Timer-141"><span class="linenos">141</span></a>            <span class="p">(</span><span class="n">seconds_per_week</span><span class="p">,</span> <span class="s2">&quot;w&quot;</span><span class="p">),</span>
+</span><span id="Timer-142"><a href="#Timer-142"><span class="linenos">142</span></a>            <span class="p">(</span><span class="n">seconds_per_day</span><span class="p">,</span> <span class="s2">&quot;d&quot;</span><span class="p">),</span>
+</span><span id="Timer-143"><a href="#Timer-143"><span class="linenos">143</span></a>            <span class="p">(</span><span class="n">seconds_per_hour</span><span class="p">,</span> <span class="s2">&quot;h&quot;</span><span class="p">),</span>
+</span><span id="Timer-144"><a href="#Timer-144"><span class="linenos">144</span></a>            <span class="p">(</span><span class="n">seconds_per_minute</span><span class="p">,</span> <span class="s2">&quot;m&quot;</span><span class="p">),</span>
+</span><span id="Timer-145"><a href="#Timer-145"><span class="linenos">145</span></a>            <span class="p">(</span><span class="n">second</span><span class="p">,</span> <span class="s2">&quot;s&quot;</span><span class="p">),</span>
+</span><span id="Timer-146"><a href="#Timer-146"><span class="linenos">146</span></a>            <span class="p">(</span><span class="n">millisecond</span><span class="p">,</span> <span class="s2">&quot;ms&quot;</span><span class="p">),</span>
+</span><span id="Timer-147"><a href="#Timer-147"><span class="linenos">147</span></a>            <span class="p">(</span><span class="n">microsecond</span><span class="p">,</span> <span class="s2">&quot;us&quot;</span><span class="p">),</span>
+</span><span id="Timer-148"><a href="#Timer-148"><span class="linenos">148</span></a>        <span class="p">]</span>
+</span><span id="Timer-149"><a href="#Timer-149"><span class="linenos">149</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">subsecond_resolution</span><span class="p">:</span>
+</span><span id="Timer-150"><a href="#Timer-150"><span class="linenos">150</span></a>            <span class="n">time_units</span> <span class="o">=</span> <span class="n">time_units</span><span class="p">[:</span><span class="o">-</span><span class="mi">2</span><span class="p">]</span>
+</span><span id="Timer-151"><a href="#Timer-151"><span class="linenos">151</span></a>        <span class="n">time_string</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="Timer-152"><a href="#Timer-152"><span class="linenos">152</span></a>        <span class="k">for</span> <span class="n">time_unit</span> <span class="ow">in</span> <span class="n">time_units</span><span class="p">:</span>
+</span><span id="Timer-153"><a href="#Timer-153"><span class="linenos">153</span></a>            <span class="n">unit_amount</span><span class="p">,</span> <span class="n">num_seconds</span> <span class="o">=</span> <span class="nb">divmod</span><span class="p">(</span><span class="n">num_seconds</span><span class="p">,</span> <span class="n">time_unit</span><span class="p">[</span><span class="mi">0</span><span class="p">])</span>
+</span><span id="Timer-154"><a href="#Timer-154"><span class="linenos">154</span></a>            <span class="k">if</span> <span class="n">unit_amount</span> <span class="o">&gt;</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="Timer-155"><a href="#Timer-155"><span class="linenos">155</span></a>                <span class="n">time_string</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">int</span><span class="p">(</span><span class="n">unit_amount</span><span class="p">)</span><span class="si">}{</span><span class="n">time_unit</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2"> &quot;</span>
+</span><span id="Timer-156"><a href="#Timer-156"><span class="linenos">156</span></a>        <span class="k">if</span> <span class="n">time_string</span> <span class="o">==</span> <span class="s2">&quot;&quot;</span><span class="p">:</span>
+</span><span id="Timer-157"><a href="#Timer-157"><span class="linenos">157</span></a>            <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;&lt;1</span><span class="si">{</span><span class="n">time_units</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">][</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="Timer-158"><a href="#Timer-158"><span class="linenos">158</span></a>        <span class="k">return</span> <span class="n">time_string</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
+</span><span id="Timer-159"><a href="#Timer-159"><span class="linenos">159</span></a>
+</span><span id="Timer-160"><a href="#Timer-160"><span class="linenos">160</span></a>    <span class="nd">@property</span>
+</span><span id="Timer-161"><a href="#Timer-161"><span class="linenos">161</span></a>    <span class="k">def</span> <span class="nf">stats</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="Timer-162"><a href="#Timer-162"><span class="linenos">162</span></a>        <span class="sd">&quot;&quot;&quot;Returns a string stating the currently elapsed time</span>
+</span><span id="Timer-163"><a href="#Timer-163"><span class="linenos">163</span></a><span class="sd">        and the average elapsed time.&quot;&quot;&quot;</span>
+</span><span id="Timer-164"><a href="#Timer-164"><span class="linenos">164</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;elapsed time: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">elapsed_str</span><span class="si">}</span><span class="se">\n</span><span class="s2">average elapsed time: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">average_elapsed_str</span><span class="si">}</span><span class="s2">&quot;</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Simple timer class that tracks total elapsed time
 and average time between calls to 'start' and 'stop'.</p>
 </div>
 
@@ -454,30 +459,30 @@
             
         <span class="name">Timer</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">averaging_window_length</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">10</span>, </span><span class="param"><span class="n">subsecond_resolution</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span></span>)</span>
 
                 <label class="view-source-button" for="Timer.__init__-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Timer.__init__"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Timer.__init__-35"><a href="#Timer.__init__-35"><span class="linenos">35</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
-</span><span id="Timer.__init__-36"><a href="#Timer.__init__-36"><span class="linenos">36</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">averaging_window_length</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">10</span><span class="p">,</span> <span class="n">subsecond_resolution</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="Timer.__init__-37"><a href="#Timer.__init__-37"><span class="linenos">37</span></a>    <span class="p">):</span>
-</span><span id="Timer.__init__-38"><a href="#Timer.__init__-38"><span class="linenos">38</span></a>        <span class="sd">&quot;&quot;&quot;:param averaging_window_length: Number of start/stop cycles</span>
-</span><span id="Timer.__init__-39"><a href="#Timer.__init__-39"><span class="linenos">39</span></a><span class="sd">        to calculate the average elapsed time with.</span>
-</span><span id="Timer.__init__-40"><a href="#Timer.__init__-40"><span class="linenos">40</span></a>
-</span><span id="Timer.__init__-41"><a href="#Timer.__init__-41"><span class="linenos">41</span></a><span class="sd">        :param subsecond_resolution: Whether to print formatted time</span>
-</span><span id="Timer.__init__-42"><a href="#Timer.__init__-42"><span class="linenos">42</span></a><span class="sd">        strings with subsecond resolution or not.&quot;&quot;&quot;</span>
-</span><span id="Timer.__init__-43"><a href="#Timer.__init__-43"><span class="linenos">43</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">start_time</span><span class="p">:</span> <span class="n">datetime</span> <span class="o">=</span> <span class="n">datetime</span><span class="o">.</span><span class="n">now</span><span class="p">()</span>
-</span><span id="Timer.__init__-44"><a href="#Timer.__init__-44"><span class="linenos">44</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">stop_time</span><span class="p">:</span> <span class="n">datetime</span> <span class="o">=</span> <span class="n">datetime</span><span class="o">.</span><span class="n">now</span><span class="p">()</span>
-</span><span id="Timer.__init__-45"><a href="#Timer.__init__-45"><span class="linenos">45</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">average_elapsed_time</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="mi">0</span>
-</span><span id="Timer.__init__-46"><a href="#Timer.__init__-46"><span class="linenos">46</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">history</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">float</span><span class="p">]</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="Timer.__init__-47"><a href="#Timer.__init__-47"><span class="linenos">47</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">elapsed_time</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="mi">0</span>
-</span><span id="Timer.__init__-48"><a href="#Timer.__init__-48"><span class="linenos">48</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">averaging_window_length</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="n">averaging_window_length</span>
-</span><span id="Timer.__init__-49"><a href="#Timer.__init__-49"><span class="linenos">49</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">started</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="Timer.__init__-50"><a href="#Timer.__init__-50"><span class="linenos">50</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">subsecond_resolution</span> <span class="o">=</span> <span class="n">subsecond_resolution</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Timer.__init__-38"><a href="#Timer.__init__-38"><span class="linenos">38</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
+</span><span id="Timer.__init__-39"><a href="#Timer.__init__-39"><span class="linenos">39</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">averaging_window_length</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">10</span><span class="p">,</span> <span class="n">subsecond_resolution</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="Timer.__init__-40"><a href="#Timer.__init__-40"><span class="linenos">40</span></a>    <span class="p">):</span>
+</span><span id="Timer.__init__-41"><a href="#Timer.__init__-41"><span class="linenos">41</span></a>        <span class="sd">&quot;&quot;&quot;:param averaging_window_length: Number of start/stop cycles</span>
+</span><span id="Timer.__init__-42"><a href="#Timer.__init__-42"><span class="linenos">42</span></a><span class="sd">        to calculate the average elapsed time with.</span>
+</span><span id="Timer.__init__-43"><a href="#Timer.__init__-43"><span class="linenos">43</span></a>
+</span><span id="Timer.__init__-44"><a href="#Timer.__init__-44"><span class="linenos">44</span></a><span class="sd">        :param subsecond_resolution: Whether to print formatted time</span>
+</span><span id="Timer.__init__-45"><a href="#Timer.__init__-45"><span class="linenos">45</span></a><span class="sd">        strings with subsecond resolution or not.&quot;&quot;&quot;</span>
+</span><span id="Timer.__init__-46"><a href="#Timer.__init__-46"><span class="linenos">46</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_start_time</span> <span class="o">=</span> <span class="n">time</span><span class="o">.</span><span class="n">time</span><span class="p">()</span>
+</span><span id="Timer.__init__-47"><a href="#Timer.__init__-47"><span class="linenos">47</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_stop_time</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">start_time</span>
+</span><span id="Timer.__init__-48"><a href="#Timer.__init__-48"><span class="linenos">48</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_elapsed</span> <span class="o">=</span> <span class="mi">0</span>
+</span><span id="Timer.__init__-49"><a href="#Timer.__init__-49"><span class="linenos">49</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_average_elapsed</span> <span class="o">=</span> <span class="mi">0</span>
+</span><span id="Timer.__init__-50"><a href="#Timer.__init__-50"><span class="linenos">50</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_history</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">float</span><span class="p">]</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="Timer.__init__-51"><a href="#Timer.__init__-51"><span class="linenos">51</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_started</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="Timer.__init__-52"><a href="#Timer.__init__-52"><span class="linenos">52</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">averaging_window_length</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="n">averaging_window_length</span>
+</span><span id="Timer.__init__-53"><a href="#Timer.__init__-53"><span class="linenos">53</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">subsecond_resolution</span> <span class="o">=</span> <span class="n">subsecond_resolution</span>
 </span></pre></div>
 
 
             <div class="docstring"><h6 id="parameters">Parameters</h6>
 
 <ul>
 <li><p><strong>averaging_window_length</strong>:  Number of start/stop cycles
@@ -485,14 +490,28 @@
 <li><p><strong>subsecond_resolution</strong>:  Whether to print formatted time
 strings with subsecond resolution or not.</p></li>
 </ul>
 </div>
 
 
                             </div>
+                            <div id="Timer.started" class="classattr">
+                                <div class="attr variable">
+            <span class="name">started</span><span class="annotation">: bool</span>
+
+        
+    </div>
+    <a class="headerlink" href="#Timer.started"></a>
+    
+            <div class="docstring"><p>Returns whether the timer has
+been started and is currently running.</p>
+</div>
+
+
+                            </div>
                             <div id="Timer.elapsed" class="classattr">
                                 <div class="attr variable">
             <span class="name">elapsed</span><span class="annotation">: float</span>
 
         
     </div>
     <a class="headerlink" href="#Timer.elapsed"></a>
@@ -517,30 +536,30 @@
 
                             </div>
                             <div id="Timer.start" class="classattr">
                                         <input id="Timer.start-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
-        <span class="name">start</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">) -> <span class="n">Self</span>:</span></span>
+        <span class="name">start</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span><span class="p">:</span> <span class="n">Self</span></span><span class="return-annotation">) -> <span class="n">Self</span>:</span></span>
 
                 <label class="view-source-button" for="Timer.start-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Timer.start"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Timer.start-66"><a href="#Timer.start-66"><span class="linenos">66</span></a>    <span class="k">def</span> <span class="nf">start</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
-</span><span id="Timer.start-67"><a href="#Timer.start-67"><span class="linenos">67</span></a>        <span class="sd">&quot;&quot;&quot;Start timer.</span>
-</span><span id="Timer.start-68"><a href="#Timer.start-68"><span class="linenos">68</span></a><span class="sd">        Returns this Timer instance so</span>
-</span><span id="Timer.start-69"><a href="#Timer.start-69"><span class="linenos">69</span></a><span class="sd">        timer start can be chained to</span>
-</span><span id="Timer.start-70"><a href="#Timer.start-70"><span class="linenos">70</span></a><span class="sd">        Timer creation.</span>
-</span><span id="Timer.start-71"><a href="#Timer.start-71"><span class="linenos">71</span></a>
-</span><span id="Timer.start-72"><a href="#Timer.start-72"><span class="linenos">72</span></a><span class="sd">        &gt;&gt;&gt; timer = Timer().start()&quot;&quot;&quot;</span>
-</span><span id="Timer.start-73"><a href="#Timer.start-73"><span class="linenos">73</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">start_time</span> <span class="o">=</span> <span class="n">datetime</span><span class="o">.</span><span class="n">now</span><span class="p">()</span>
-</span><span id="Timer.start-74"><a href="#Timer.start-74"><span class="linenos">74</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">started</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="Timer.start-75"><a href="#Timer.start-75"><span class="linenos">75</span></a>        <span class="k">return</span> <span class="bp">self</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Timer.start-95"><a href="#Timer.start-95"><span class="linenos"> 95</span></a>    <span class="k">def</span> <span class="nf">start</span><span class="p">(</span><span class="bp">self</span><span class="p">:</span> <span class="n">Self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
+</span><span id="Timer.start-96"><a href="#Timer.start-96"><span class="linenos"> 96</span></a>        <span class="sd">&quot;&quot;&quot;Start timer.</span>
+</span><span id="Timer.start-97"><a href="#Timer.start-97"><span class="linenos"> 97</span></a><span class="sd">        Returns this Timer instance so</span>
+</span><span id="Timer.start-98"><a href="#Timer.start-98"><span class="linenos"> 98</span></a><span class="sd">        timer start can be chained to</span>
+</span><span id="Timer.start-99"><a href="#Timer.start-99"><span class="linenos"> 99</span></a><span class="sd">        Timer creation.</span>
+</span><span id="Timer.start-100"><a href="#Timer.start-100"><span class="linenos">100</span></a>
+</span><span id="Timer.start-101"><a href="#Timer.start-101"><span class="linenos">101</span></a><span class="sd">        &gt;&gt;&gt; timer = Timer().start()&quot;&quot;&quot;</span>
+</span><span id="Timer.start-102"><a href="#Timer.start-102"><span class="linenos">102</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_start_time</span> <span class="o">=</span> <span class="n">time</span><span class="o">.</span><span class="n">time</span><span class="p">()</span>
+</span><span id="Timer.start-103"><a href="#Timer.start-103"><span class="linenos">103</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_started</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="Timer.start-104"><a href="#Timer.start-104"><span class="linenos">104</span></a>        <span class="k">return</span> <span class="bp">self</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Start timer.
 Returns this Timer instance so
 timer start can be chained to
 Timer creation.</p>
@@ -560,125 +579,81 @@
         <span class="def">def</span>
         <span class="name">stop</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="Timer.stop-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Timer.stop"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Timer.stop-77"><a href="#Timer.stop-77"><span class="linenos">77</span></a>    <span class="k">def</span> <span class="nf">stop</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Timer.stop-78"><a href="#Timer.stop-78"><span class="linenos">78</span></a>        <span class="sd">&quot;&quot;&quot;Stop timer.</span>
-</span><span id="Timer.stop-79"><a href="#Timer.stop-79"><span class="linenos">79</span></a>
-</span><span id="Timer.stop-80"><a href="#Timer.stop-80"><span class="linenos">80</span></a><span class="sd">        Calculates elapsed time and average elapsed time.&quot;&quot;&quot;</span>
-</span><span id="Timer.stop-81"><a href="#Timer.stop-81"><span class="linenos">81</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">stop_time</span> <span class="o">=</span> <span class="n">datetime</span><span class="o">.</span><span class="n">now</span><span class="p">()</span>
-</span><span id="Timer.stop-82"><a href="#Timer.stop-82"><span class="linenos">82</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">started</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="Timer.stop-83"><a href="#Timer.stop-83"><span class="linenos">83</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">elapsed_time</span> <span class="o">=</span> <span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">stop_time</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">start_time</span><span class="p">)</span><span class="o">.</span><span class="n">total_seconds</span><span class="p">()</span>
-</span><span id="Timer.stop-84"><a href="#Timer.stop-84"><span class="linenos">84</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_save_elapsed_time</span><span class="p">()</span>
-</span><span id="Timer.stop-85"><a href="#Timer.stop-85"><span class="linenos">85</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">average_elapsed_time</span> <span class="o">=</span> <span class="nb">sum</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">history</span><span class="p">)</span> <span class="o">/</span> <span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">history</span><span class="p">))</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Timer.stop-106"><a href="#Timer.stop-106"><span class="linenos">106</span></a>    <span class="k">def</span> <span class="nf">stop</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Timer.stop-107"><a href="#Timer.stop-107"><span class="linenos">107</span></a>        <span class="sd">&quot;&quot;&quot;Stop timer.</span>
+</span><span id="Timer.stop-108"><a href="#Timer.stop-108"><span class="linenos">108</span></a>
+</span><span id="Timer.stop-109"><a href="#Timer.stop-109"><span class="linenos">109</span></a><span class="sd">        Calculates elapsed time and average elapsed time.&quot;&quot;&quot;</span>
+</span><span id="Timer.stop-110"><a href="#Timer.stop-110"><span class="linenos">110</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_stop_time</span> <span class="o">=</span> <span class="n">time</span><span class="o">.</span><span class="n">time</span><span class="p">()</span>
+</span><span id="Timer.stop-111"><a href="#Timer.stop-111"><span class="linenos">111</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_started</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="Timer.stop-112"><a href="#Timer.stop-112"><span class="linenos">112</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_elapsed</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_stop_time</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">_start_time</span>
+</span><span id="Timer.stop-113"><a href="#Timer.stop-113"><span class="linenos">113</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_save_elapsed_time</span><span class="p">()</span>
+</span><span id="Timer.stop-114"><a href="#Timer.stop-114"><span class="linenos">114</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_average_elapsed</span> <span class="o">=</span> <span class="nb">sum</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_history</span><span class="p">)</span> <span class="o">/</span> <span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_history</span><span class="p">))</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Stop timer.</p>
 
 <p>Calculates elapsed time and average elapsed time.</p>
 </div>
 
 
                             </div>
-                            <div id="Timer.current_elapsed_time" class="classattr">
-                                        <input id="Timer.current_elapsed_time-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
-<div class="attr function">
-            
-        <span class="def">def</span>
-        <span class="name">current_elapsed_time</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="nb">format</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>,</span><span class="param">	<span class="n">subsecond_resolution</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span></span><span class="return-annotation">) -> <span class="nb">float</span> <span class="o">|</span> <span class="nb">str</span>:</span></span>
-
-                <label class="view-source-button" for="Timer.current_elapsed_time-view-source"><span>View Source</span></label>
-
-    </div>
-    <a class="headerlink" href="#Timer.current_elapsed_time"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Timer.current_elapsed_time-94"><a href="#Timer.current_elapsed_time-94"><span class="linenos"> 94</span></a>    <span class="k">def</span> <span class="nf">current_elapsed_time</span><span class="p">(</span>
-</span><span id="Timer.current_elapsed_time-95"><a href="#Timer.current_elapsed_time-95"><span class="linenos"> 95</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="nb">format</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span> <span class="n">subsecond_resolution</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="Timer.current_elapsed_time-96"><a href="#Timer.current_elapsed_time-96"><span class="linenos"> 96</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span> <span class="o">|</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="Timer.current_elapsed_time-97"><a href="#Timer.current_elapsed_time-97"><span class="linenos"> 97</span></a>        <span class="sd">&quot;&quot;&quot;Returns current elapsed without stopping the timer.</span>
-</span><span id="Timer.current_elapsed_time-98"><a href="#Timer.current_elapsed_time-98"><span class="linenos"> 98</span></a>
-</span><span id="Timer.current_elapsed_time-99"><a href="#Timer.current_elapsed_time-99"><span class="linenos"> 99</span></a><span class="sd">        :param format: If True, elapsed time is returned as a string.</span>
-</span><span id="Timer.current_elapsed_time-100"><a href="#Timer.current_elapsed_time-100"><span class="linenos">100</span></a><span class="sd">        If False, elapsed time is returned as a float.&quot;&quot;&quot;</span>
-</span><span id="Timer.current_elapsed_time-101"><a href="#Timer.current_elapsed_time-101"><span class="linenos">101</span></a>        <span class="n">warnings</span><span class="o">.</span><span class="n">warn</span><span class="p">(</span>
-</span><span id="Timer.current_elapsed_time-102"><a href="#Timer.current_elapsed_time-102"><span class="linenos">102</span></a>            <span class="s2">&quot;current_elapsed_time is depreciated. Use &#39;elapsed&#39; and &#39;elapsed_str&#39; properties instead.&quot;</span><span class="p">,</span>
-</span><span id="Timer.current_elapsed_time-103"><a href="#Timer.current_elapsed_time-103"><span class="linenos">103</span></a>            <span class="ne">FutureWarning</span><span class="p">,</span>
-</span><span id="Timer.current_elapsed_time-104"><a href="#Timer.current_elapsed_time-104"><span class="linenos">104</span></a>            <span class="mi">2</span><span class="p">,</span>
-</span><span id="Timer.current_elapsed_time-105"><a href="#Timer.current_elapsed_time-105"><span class="linenos">105</span></a>        <span class="p">)</span>
-</span><span id="Timer.current_elapsed_time-106"><a href="#Timer.current_elapsed_time-106"><span class="linenos">106</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">elapsed_time</span> <span class="o">=</span> <span class="p">(</span><span class="n">datetime</span><span class="o">.</span><span class="n">now</span><span class="p">()</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">start_time</span><span class="p">)</span><span class="o">.</span><span class="n">total_seconds</span><span class="p">()</span>
-</span><span id="Timer.current_elapsed_time-107"><a href="#Timer.current_elapsed_time-107"><span class="linenos">107</span></a>        <span class="k">return</span> <span class="p">(</span>
-</span><span id="Timer.current_elapsed_time-108"><a href="#Timer.current_elapsed_time-108"><span class="linenos">108</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">format_time</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">elapsed_time</span><span class="p">,</span> <span class="n">subsecond_resolution</span><span class="p">)</span>
-</span><span id="Timer.current_elapsed_time-109"><a href="#Timer.current_elapsed_time-109"><span class="linenos">109</span></a>            <span class="k">if</span> <span class="nb">format</span>
-</span><span id="Timer.current_elapsed_time-110"><a href="#Timer.current_elapsed_time-110"><span class="linenos">110</span></a>            <span class="k">else</span> <span class="bp">self</span><span class="o">.</span><span class="n">elapsed_time</span>
-</span><span id="Timer.current_elapsed_time-111"><a href="#Timer.current_elapsed_time-111"><span class="linenos">111</span></a>        <span class="p">)</span>
-</span></pre></div>
-
-
-            <div class="docstring"><p>Returns current elapsed without stopping the timer.</p>
-
-<h6 id="parameters">Parameters</h6>
-
-<ul>
-<li><strong>format</strong>:  If True, elapsed time is returned as a string.
-If False, elapsed time is returned as a float.</li>
-</ul>
-</div>
-
-
-                            </div>
                             <div id="Timer.format_time" class="classattr">
                                         <input id="Timer.format_time-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
                     <div class="decorator">@staticmethod</div>
 
         <span class="def">def</span>
         <span class="name">format_time</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">num_seconds</span><span class="p">:</span> <span class="nb">float</span>, </span><span class="param"><span class="n">subsecond_resolution</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span></span><span class="return-annotation">) -> <span class="nb">str</span>:</span></span>
 
                 <label class="view-source-button" for="Timer.format_time-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Timer.format_time"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Timer.format_time-113"><a href="#Timer.format_time-113"><span class="linenos">113</span></a>    <span class="nd">@staticmethod</span>
-</span><span id="Timer.format_time-114"><a href="#Timer.format_time-114"><span class="linenos">114</span></a>    <span class="k">def</span> <span class="nf">format_time</span><span class="p">(</span><span class="n">num_seconds</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">subsecond_resolution</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="Timer.format_time-115"><a href="#Timer.format_time-115"><span class="linenos">115</span></a>        <span class="sd">&quot;&quot;&quot;Returns num_seconds as a string with units.</span>
-</span><span id="Timer.format_time-116"><a href="#Timer.format_time-116"><span class="linenos">116</span></a>
-</span><span id="Timer.format_time-117"><a href="#Timer.format_time-117"><span class="linenos">117</span></a><span class="sd">        :param subsecond_resolution: Include milliseconds</span>
-</span><span id="Timer.format_time-118"><a href="#Timer.format_time-118"><span class="linenos">118</span></a><span class="sd">        and microseconds with the output.&quot;&quot;&quot;</span>
-</span><span id="Timer.format_time-119"><a href="#Timer.format_time-119"><span class="linenos">119</span></a>        <span class="n">microsecond</span> <span class="o">=</span> <span class="mf">0.000001</span>
-</span><span id="Timer.format_time-120"><a href="#Timer.format_time-120"><span class="linenos">120</span></a>        <span class="n">millisecond</span> <span class="o">=</span> <span class="mf">0.001</span>
-</span><span id="Timer.format_time-121"><a href="#Timer.format_time-121"><span class="linenos">121</span></a>        <span class="n">second</span> <span class="o">=</span> <span class="mi">1</span>
-</span><span id="Timer.format_time-122"><a href="#Timer.format_time-122"><span class="linenos">122</span></a>        <span class="n">seconds_per_minute</span> <span class="o">=</span> <span class="mi">60</span>
-</span><span id="Timer.format_time-123"><a href="#Timer.format_time-123"><span class="linenos">123</span></a>        <span class="n">seconds_per_hour</span> <span class="o">=</span> <span class="mi">3600</span>
-</span><span id="Timer.format_time-124"><a href="#Timer.format_time-124"><span class="linenos">124</span></a>        <span class="n">seconds_per_day</span> <span class="o">=</span> <span class="mi">86400</span>
-</span><span id="Timer.format_time-125"><a href="#Timer.format_time-125"><span class="linenos">125</span></a>        <span class="n">seconds_per_week</span> <span class="o">=</span> <span class="mi">604800</span>
-</span><span id="Timer.format_time-126"><a href="#Timer.format_time-126"><span class="linenos">126</span></a>        <span class="n">seconds_per_month</span> <span class="o">=</span> <span class="mi">2419200</span>
-</span><span id="Timer.format_time-127"><a href="#Timer.format_time-127"><span class="linenos">127</span></a>        <span class="n">seconds_per_year</span> <span class="o">=</span> <span class="mi">29030400</span>
-</span><span id="Timer.format_time-128"><a href="#Timer.format_time-128"><span class="linenos">128</span></a>        <span class="n">time_units</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="Timer.format_time-129"><a href="#Timer.format_time-129"><span class="linenos">129</span></a>            <span class="p">(</span><span class="n">seconds_per_year</span><span class="p">,</span> <span class="s2">&quot;y&quot;</span><span class="p">),</span>
-</span><span id="Timer.format_time-130"><a href="#Timer.format_time-130"><span class="linenos">130</span></a>            <span class="p">(</span><span class="n">seconds_per_month</span><span class="p">,</span> <span class="s2">&quot;mn&quot;</span><span class="p">),</span>
-</span><span id="Timer.format_time-131"><a href="#Timer.format_time-131"><span class="linenos">131</span></a>            <span class="p">(</span><span class="n">seconds_per_week</span><span class="p">,</span> <span class="s2">&quot;w&quot;</span><span class="p">),</span>
-</span><span id="Timer.format_time-132"><a href="#Timer.format_time-132"><span class="linenos">132</span></a>            <span class="p">(</span><span class="n">seconds_per_day</span><span class="p">,</span> <span class="s2">&quot;d&quot;</span><span class="p">),</span>
-</span><span id="Timer.format_time-133"><a href="#Timer.format_time-133"><span class="linenos">133</span></a>            <span class="p">(</span><span class="n">seconds_per_hour</span><span class="p">,</span> <span class="s2">&quot;h&quot;</span><span class="p">),</span>
-</span><span id="Timer.format_time-134"><a href="#Timer.format_time-134"><span class="linenos">134</span></a>            <span class="p">(</span><span class="n">seconds_per_minute</span><span class="p">,</span> <span class="s2">&quot;m&quot;</span><span class="p">),</span>
-</span><span id="Timer.format_time-135"><a href="#Timer.format_time-135"><span class="linenos">135</span></a>            <span class="p">(</span><span class="n">second</span><span class="p">,</span> <span class="s2">&quot;s&quot;</span><span class="p">),</span>
-</span><span id="Timer.format_time-136"><a href="#Timer.format_time-136"><span class="linenos">136</span></a>            <span class="p">(</span><span class="n">millisecond</span><span class="p">,</span> <span class="s2">&quot;ms&quot;</span><span class="p">),</span>
-</span><span id="Timer.format_time-137"><a href="#Timer.format_time-137"><span class="linenos">137</span></a>            <span class="p">(</span><span class="n">microsecond</span><span class="p">,</span> <span class="s2">&quot;us&quot;</span><span class="p">),</span>
-</span><span id="Timer.format_time-138"><a href="#Timer.format_time-138"><span class="linenos">138</span></a>        <span class="p">]</span>
-</span><span id="Timer.format_time-139"><a href="#Timer.format_time-139"><span class="linenos">139</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">subsecond_resolution</span><span class="p">:</span>
-</span><span id="Timer.format_time-140"><a href="#Timer.format_time-140"><span class="linenos">140</span></a>            <span class="n">time_units</span> <span class="o">=</span> <span class="n">time_units</span><span class="p">[:</span><span class="o">-</span><span class="mi">2</span><span class="p">]</span>
-</span><span id="Timer.format_time-141"><a href="#Timer.format_time-141"><span class="linenos">141</span></a>        <span class="n">time_string</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="Timer.format_time-142"><a href="#Timer.format_time-142"><span class="linenos">142</span></a>        <span class="k">for</span> <span class="n">time_unit</span> <span class="ow">in</span> <span class="n">time_units</span><span class="p">:</span>
-</span><span id="Timer.format_time-143"><a href="#Timer.format_time-143"><span class="linenos">143</span></a>            <span class="n">unit_amount</span><span class="p">,</span> <span class="n">num_seconds</span> <span class="o">=</span> <span class="nb">divmod</span><span class="p">(</span><span class="n">num_seconds</span><span class="p">,</span> <span class="n">time_unit</span><span class="p">[</span><span class="mi">0</span><span class="p">])</span>
-</span><span id="Timer.format_time-144"><a href="#Timer.format_time-144"><span class="linenos">144</span></a>            <span class="k">if</span> <span class="n">unit_amount</span> <span class="o">&gt;</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="Timer.format_time-145"><a href="#Timer.format_time-145"><span class="linenos">145</span></a>                <span class="n">time_string</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">int</span><span class="p">(</span><span class="n">unit_amount</span><span class="p">)</span><span class="si">}{</span><span class="n">time_unit</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2"> &quot;</span>
-</span><span id="Timer.format_time-146"><a href="#Timer.format_time-146"><span class="linenos">146</span></a>        <span class="k">if</span> <span class="n">time_string</span> <span class="o">==</span> <span class="s2">&quot;&quot;</span><span class="p">:</span>
-</span><span id="Timer.format_time-147"><a href="#Timer.format_time-147"><span class="linenos">147</span></a>            <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;&lt;1</span><span class="si">{</span><span class="n">time_units</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">][</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="Timer.format_time-148"><a href="#Timer.format_time-148"><span class="linenos">148</span></a>        <span class="k">return</span> <span class="n">time_string</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Timer.format_time-123"><a href="#Timer.format_time-123"><span class="linenos">123</span></a>    <span class="nd">@staticmethod</span>
+</span><span id="Timer.format_time-124"><a href="#Timer.format_time-124"><span class="linenos">124</span></a>    <span class="k">def</span> <span class="nf">format_time</span><span class="p">(</span><span class="n">num_seconds</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">subsecond_resolution</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="Timer.format_time-125"><a href="#Timer.format_time-125"><span class="linenos">125</span></a>        <span class="sd">&quot;&quot;&quot;Returns num_seconds as a string with units.</span>
+</span><span id="Timer.format_time-126"><a href="#Timer.format_time-126"><span class="linenos">126</span></a>
+</span><span id="Timer.format_time-127"><a href="#Timer.format_time-127"><span class="linenos">127</span></a><span class="sd">        :param subsecond_resolution: Include milliseconds</span>
+</span><span id="Timer.format_time-128"><a href="#Timer.format_time-128"><span class="linenos">128</span></a><span class="sd">        and microseconds with the output.&quot;&quot;&quot;</span>
+</span><span id="Timer.format_time-129"><a href="#Timer.format_time-129"><span class="linenos">129</span></a>        <span class="n">microsecond</span> <span class="o">=</span> <span class="mf">0.000001</span>
+</span><span id="Timer.format_time-130"><a href="#Timer.format_time-130"><span class="linenos">130</span></a>        <span class="n">millisecond</span> <span class="o">=</span> <span class="mf">0.001</span>
+</span><span id="Timer.format_time-131"><a href="#Timer.format_time-131"><span class="linenos">131</span></a>        <span class="n">second</span> <span class="o">=</span> <span class="mi">1</span>
+</span><span id="Timer.format_time-132"><a href="#Timer.format_time-132"><span class="linenos">132</span></a>        <span class="n">seconds_per_minute</span> <span class="o">=</span> <span class="mi">60</span>
+</span><span id="Timer.format_time-133"><a href="#Timer.format_time-133"><span class="linenos">133</span></a>        <span class="n">seconds_per_hour</span> <span class="o">=</span> <span class="mi">3600</span>
+</span><span id="Timer.format_time-134"><a href="#Timer.format_time-134"><span class="linenos">134</span></a>        <span class="n">seconds_per_day</span> <span class="o">=</span> <span class="mi">86400</span>
+</span><span id="Timer.format_time-135"><a href="#Timer.format_time-135"><span class="linenos">135</span></a>        <span class="n">seconds_per_week</span> <span class="o">=</span> <span class="mi">604800</span>
+</span><span id="Timer.format_time-136"><a href="#Timer.format_time-136"><span class="linenos">136</span></a>        <span class="n">seconds_per_month</span> <span class="o">=</span> <span class="mi">2419200</span>
+</span><span id="Timer.format_time-137"><a href="#Timer.format_time-137"><span class="linenos">137</span></a>        <span class="n">seconds_per_year</span> <span class="o">=</span> <span class="mi">29030400</span>
+</span><span id="Timer.format_time-138"><a href="#Timer.format_time-138"><span class="linenos">138</span></a>        <span class="n">time_units</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="Timer.format_time-139"><a href="#Timer.format_time-139"><span class="linenos">139</span></a>            <span class="p">(</span><span class="n">seconds_per_year</span><span class="p">,</span> <span class="s2">&quot;y&quot;</span><span class="p">),</span>
+</span><span id="Timer.format_time-140"><a href="#Timer.format_time-140"><span class="linenos">140</span></a>            <span class="p">(</span><span class="n">seconds_per_month</span><span class="p">,</span> <span class="s2">&quot;mn&quot;</span><span class="p">),</span>
+</span><span id="Timer.format_time-141"><a href="#Timer.format_time-141"><span class="linenos">141</span></a>            <span class="p">(</span><span class="n">seconds_per_week</span><span class="p">,</span> <span class="s2">&quot;w&quot;</span><span class="p">),</span>
+</span><span id="Timer.format_time-142"><a href="#Timer.format_time-142"><span class="linenos">142</span></a>            <span class="p">(</span><span class="n">seconds_per_day</span><span class="p">,</span> <span class="s2">&quot;d&quot;</span><span class="p">),</span>
+</span><span id="Timer.format_time-143"><a href="#Timer.format_time-143"><span class="linenos">143</span></a>            <span class="p">(</span><span class="n">seconds_per_hour</span><span class="p">,</span> <span class="s2">&quot;h&quot;</span><span class="p">),</span>
+</span><span id="Timer.format_time-144"><a href="#Timer.format_time-144"><span class="linenos">144</span></a>            <span class="p">(</span><span class="n">seconds_per_minute</span><span class="p">,</span> <span class="s2">&quot;m&quot;</span><span class="p">),</span>
+</span><span id="Timer.format_time-145"><a href="#Timer.format_time-145"><span class="linenos">145</span></a>            <span class="p">(</span><span class="n">second</span><span class="p">,</span> <span class="s2">&quot;s&quot;</span><span class="p">),</span>
+</span><span id="Timer.format_time-146"><a href="#Timer.format_time-146"><span class="linenos">146</span></a>            <span class="p">(</span><span class="n">millisecond</span><span class="p">,</span> <span class="s2">&quot;ms&quot;</span><span class="p">),</span>
+</span><span id="Timer.format_time-147"><a href="#Timer.format_time-147"><span class="linenos">147</span></a>            <span class="p">(</span><span class="n">microsecond</span><span class="p">,</span> <span class="s2">&quot;us&quot;</span><span class="p">),</span>
+</span><span id="Timer.format_time-148"><a href="#Timer.format_time-148"><span class="linenos">148</span></a>        <span class="p">]</span>
+</span><span id="Timer.format_time-149"><a href="#Timer.format_time-149"><span class="linenos">149</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">subsecond_resolution</span><span class="p">:</span>
+</span><span id="Timer.format_time-150"><a href="#Timer.format_time-150"><span class="linenos">150</span></a>            <span class="n">time_units</span> <span class="o">=</span> <span class="n">time_units</span><span class="p">[:</span><span class="o">-</span><span class="mi">2</span><span class="p">]</span>
+</span><span id="Timer.format_time-151"><a href="#Timer.format_time-151"><span class="linenos">151</span></a>        <span class="n">time_string</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="Timer.format_time-152"><a href="#Timer.format_time-152"><span class="linenos">152</span></a>        <span class="k">for</span> <span class="n">time_unit</span> <span class="ow">in</span> <span class="n">time_units</span><span class="p">:</span>
+</span><span id="Timer.format_time-153"><a href="#Timer.format_time-153"><span class="linenos">153</span></a>            <span class="n">unit_amount</span><span class="p">,</span> <span class="n">num_seconds</span> <span class="o">=</span> <span class="nb">divmod</span><span class="p">(</span><span class="n">num_seconds</span><span class="p">,</span> <span class="n">time_unit</span><span class="p">[</span><span class="mi">0</span><span class="p">])</span>
+</span><span id="Timer.format_time-154"><a href="#Timer.format_time-154"><span class="linenos">154</span></a>            <span class="k">if</span> <span class="n">unit_amount</span> <span class="o">&gt;</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="Timer.format_time-155"><a href="#Timer.format_time-155"><span class="linenos">155</span></a>                <span class="n">time_string</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">int</span><span class="p">(</span><span class="n">unit_amount</span><span class="p">)</span><span class="si">}{</span><span class="n">time_unit</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2"> &quot;</span>
+</span><span id="Timer.format_time-156"><a href="#Timer.format_time-156"><span class="linenos">156</span></a>        <span class="k">if</span> <span class="n">time_string</span> <span class="o">==</span> <span class="s2">&quot;&quot;</span><span class="p">:</span>
+</span><span id="Timer.format_time-157"><a href="#Timer.format_time-157"><span class="linenos">157</span></a>            <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;&lt;1</span><span class="si">{</span><span class="n">time_units</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">][</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="Timer.format_time-158"><a href="#Timer.format_time-158"><span class="linenos">158</span></a>        <span class="k">return</span> <span class="n">time_string</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Returns num_seconds as a string with units.</p>
 
 <h6 id="parameters">Parameters</h6>
 
@@ -686,50 +661,24 @@
 <li><strong>subsecond_resolution</strong>:  Include milliseconds
 and microseconds with the output.</li>
 </ul>
 </div>
 
 
                             </div>
-                            <div id="Timer.get_stats" class="classattr">
-                                        <input id="Timer.get_stats-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
-<div class="attr function">
-            
-        <span class="def">def</span>
-        <span class="name">get_stats</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="nb">format</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>, </span><span class="param"><span class="n">subsecond_resolution</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span></span><span class="return-annotation">) -> <span class="nb">str</span>:</span></span>
-
-                <label class="view-source-button" for="Timer.get_stats-view-source"><span>View Source</span></label>
+                            <div id="Timer.stats" class="classattr">
+                                <div class="attr variable">
+            <span class="name">stats</span><span class="annotation">: str</span>
 
+        
     </div>
-    <a class="headerlink" href="#Timer.get_stats"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Timer.get_stats-150"><a href="#Timer.get_stats-150"><span class="linenos">150</span></a>    <span class="k">def</span> <span class="nf">get_stats</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="nb">format</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span> <span class="n">subsecond_resolution</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="Timer.get_stats-151"><a href="#Timer.get_stats-151"><span class="linenos">151</span></a>        <span class="sd">&quot;&quot;&quot;Returns string for elapsed time and average elapsed time.</span>
-</span><span id="Timer.get_stats-152"><a href="#Timer.get_stats-152"><span class="linenos">152</span></a>
-</span><span id="Timer.get_stats-153"><a href="#Timer.get_stats-153"><span class="linenos">153</span></a><span class="sd">        :param format: Times are returned as strings if True,</span>
-</span><span id="Timer.get_stats-154"><a href="#Timer.get_stats-154"><span class="linenos">154</span></a><span class="sd">        otherwise they&#39;re raw floats.</span>
-</span><span id="Timer.get_stats-155"><a href="#Timer.get_stats-155"><span class="linenos">155</span></a>
-</span><span id="Timer.get_stats-156"><a href="#Timer.get_stats-156"><span class="linenos">156</span></a><span class="sd">        :param subsecond_resolution: Include milliseconds</span>
-</span><span id="Timer.get_stats-157"><a href="#Timer.get_stats-157"><span class="linenos">157</span></a><span class="sd">        and microseconds with the output.&quot;&quot;&quot;</span>
-</span><span id="Timer.get_stats-158"><a href="#Timer.get_stats-158"><span class="linenos">158</span></a>        <span class="k">if</span> <span class="nb">format</span><span class="p">:</span>
-</span><span id="Timer.get_stats-159"><a href="#Timer.get_stats-159"><span class="linenos">159</span></a>            <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;elapsed time: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">format_time</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">elapsed_time</span><span class="p">,</span> <span class="n">subsecond_resolution</span><span class="p">)</span><span class="si">}</span><span class="se">\n</span><span class="s2">average elapsed time: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">format_time</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">average_elapsed_time</span><span class="p">,</span> <span class="n">subsecond_resolution</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="Timer.get_stats-160"><a href="#Timer.get_stats-160"><span class="linenos">160</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="Timer.get_stats-161"><a href="#Timer.get_stats-161"><span class="linenos">161</span></a>            <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;elapsed time: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">elapsed_time</span><span class="si">}</span><span class="s2">s</span><span class="se">\n</span><span class="s2">average elapsed time: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">average_elapsed_time</span><span class="si">}</span><span class="s2">s&quot;</span>
-</span></pre></div>
-
-
-            <div class="docstring"><p>Returns string for elapsed time and average elapsed time.</p>
-
-<h6 id="parameters">Parameters</h6>
-
-<ul>
-<li><p><strong>format</strong>:  Times are returned as strings if True,
-otherwise they're raw floats.</p></li>
-<li><p><strong>subsecond_resolution</strong>:  Include milliseconds
-and microseconds with the output.</p></li>
-</ul>
+    <a class="headerlink" href="#Timer.stats"></a>
+    
+            <div class="docstring"><p>Returns a string stating the currently elapsed time
+and the average elapsed time.</p>
 </div>
 
 
                             </div>
                 </section>
     </main>
 <script>
```

#### html2text {}

```diff
@@ -2,521 +2,464 @@
 
   ⁰
 ____ noiftimer [Unknown INPUT type]
 ***** API Documentation *****
     * time_it
     * Timer
           o Timer
+          o started
           o elapsed
           o elapsed_str
           o start
           o stop
-          o current_elapsed_time
           o format_time
-          o get_stats
+          o stats
 built_with_pdoc[pdoc_logo]
 
 ****** noiftimer.noiftimer ******
 ⁰ View Source
-__1import warnings
-__2from datetime import datetime
-__3from typing import Any, Callable, Self
-__4
+__1import time
+__2from typing import Any, Callable
+__3
+__4from typing_extensions import Self
 __5
-__6def time_it(loops: int = 1) -> Callable[..., Any]:
-__7    """Decorator to time function execution time
-__8    and print the results.
-__9
-_10    :param loops: How many times to loop the function,
-_11    starting and stopping the timer before and after
-_12    each loop."""
-_13
-_14    def decorator(func: Callable[..., Any]) -> Callable[..., Any]:
-_15        def wrapper(*args, **kwargs) -> Any:
-_16            timer = Timer(loops)
-_17            for _ in range(loops):
-_18                timer.start()
-_19                result = func(*args, **kwargs)
-_20                timer.stop()
-_21            execution_time = timer.format_time(timer.average_elapsed_time,
-True)
-_22            print(f"{func.__name__} average execution time:
-{execution_time}")
-_23            return result
-_24
-_25        return wrapper
-_26
-_27    return decorator
-_28
+__6
+__7def time_it(loops: int = 1) -> Callable[..., Any]:
+__8    """Decorator to time function execution time
+__9    and print the results.
+_10
+_11    :param loops: How many times to loop the function,
+_12    starting and stopping the timer before and after
+_13    each loop."""
+_14
+_15    def decorator(func: Callable[..., Any]) -> Callable[..., Any]:
+_16        def wrapper(*args, **kwargs) -> Any:
+_17            timer = Timer(loops)
+_18            result = None
+_19            for _ in range(loops):
+_20                timer.start()
+_21                result = func(*args, **kwargs)
+_22                timer.stop()
+_23            print(
+_24                f"{func.__name__} average execution time:
+{timer.average_elapsed_str}"
+_25            )
+_26            return result
+_27
+_28        return wrapper
 _29
-_30class Timer:
-_31    """Simple timer class that tracks total elapsed time
-_32    and average time between calls to 'start' and 'stop'."""
-_33
-_34    def __init__(
-_35        self, averaging_window_length: int = 10, subsecond_resolution: bool
+_30    return decorator
+_31
+_32
+_33class Timer:
+_34    """Simple timer class that tracks total elapsed time
+_35    and average time between calls to 'start' and 'stop'."""
+_36
+_37    def __init__(
+_38        self, averaging_window_length: int = 10, subsecond_resolution: bool
 = True
-_36    ):
-_37        """:param averaging_window_length: Number of start/stop cycles
-_38        to calculate the average elapsed time with.
-_39
-_40        :param subsecond_resolution: Whether to print formatted time
-_41        strings with subsecond resolution or not."""
-_42        self.start_time: datetime = datetime.now()
-_43        self.stop_time: datetime = datetime.now()
-_44        self.average_elapsed_time: float = 0
-_45        self.history: list[float] = []
-_46        self.elapsed_time: float = 0
-_47        self.averaging_window_length: int = averaging_window_length
-_48        self.started: bool = False
-_49        self.subsecond_resolution = subsecond_resolution
-_50
-_51    @property
-_52    def elapsed(self) -> float:
-_53        """Return the currently elapsed time."""
-_54        if self.started:
-_55            return (datetime.now() - self.start_time).total_seconds()
-_56        else:
-_57            return (self.stop_time - self.start_time).total_seconds()
-_58
-_59    @property
-_60    def elapsed_str(self) -> str:
-_61        """Return the currently elapsed time
-_62        as a formatted string."""
-_63        return self.format_time(self.elapsed, self.subsecond_resolution)
-_64
-_65    def start(self) -> Self:
-_66        """Start timer.
-_67        Returns this Timer instance so
-_68        timer start can be chained to
-_69        Timer creation.
-_70
-_71        >>> timer = Timer().start()"""
-_72        self.start_time = datetime.now()
-_73        self.started = True
-_74        return self
-_75
-_76    def stop(self):
-_77        """Stop timer.
-_78
-_79        Calculates elapsed time and average elapsed time."""
-_80        self.stop_time = datetime.now()
-_81        self.started = False
-_82        self.elapsed_time = (self.stop_time - self.start_time).total_seconds
-()
-_83        self._save_elapsed_time()
-_84        self.average_elapsed_time = sum(self.history) / (len(self.history))
+_39    ):
+_40        """:param averaging_window_length: Number of start/stop cycles
+_41        to calculate the average elapsed time with.
+_42
+_43        :param subsecond_resolution: Whether to print formatted time
+_44        strings with subsecond resolution or not."""
+_45        self._start_time = time.time()
+_46        self._stop_time = self.start_time
+_47        self._elapsed = 0
+_48        self._average_elapsed = 0
+_49        self._history: list[float] = []
+_50        self._started: bool = False
+_51        self.averaging_window_length: int = averaging_window_length
+_52        self.subsecond_resolution = subsecond_resolution
+_53
+_54    @property
+_55    def started(self) -> bool:
+_56        """Returns whether the timer has
+_57        been started and is currently running."""
+_58        return self._started
+_59
+_60    @property
+_61    def elapsed(self) -> float:
+_62        """Return the currently elapsed time."""
+_63        if self._started:
+_64            return time.time() - self._start_time
+_65        else:
+_66            return self._elapsed
+_67
+_68    @property
+_69    def elapsed_str(self) -> str:
+_70        """Return the currently elapsed time
+_71        as a formatted string."""
+_72        return self.format_time(self.elapsed, self.subsecond_resolution)
+_73
+_74    @property
+_75    def average_elapsed(self) -> float:
+_76        return self._average_elapsed
+_77
+_78    @property
+_79    def average_elapsed_str(self) -> str:
+_80        return self.format_time(self._average_elapsed,
+self.subsecond_resolution)
+_81
+_82    @property
+_83    def start_time(self) -> float:
+_84        return self._start_time
 _85
-_86    def _save_elapsed_time(self):
-_87        """Saves current elapsed time to the history buffer
-_88        in a FIFO manner."""
-_89        if len(self.history) >= self.averaging_window_length:
-_90            self.history.pop(0)
-_91        self.history.append(self.elapsed_time)
-_92
-_93    def current_elapsed_time(
-_94        self, format: bool = True, subsecond_resolution: bool = False
-_95    ) -> float | str:
-_96        """Returns current elapsed without stopping the timer.
-_97
-_98        :param format: If True, elapsed time is returned as a string.
-_99        If False, elapsed time is returned as a float."""
-100        warnings.warn(
-101            "current_elapsed_time is depreciated. Use 'elapsed' and
-'elapsed_str' properties instead.",
-102            FutureWarning,
-103            2,
-104        )
-105        self.elapsed_time = (datetime.now() - self.start_time).total_seconds
-()
-106        return (
-107            self.format_time(self.elapsed_time, subsecond_resolution)
-108            if format
-109            else self.elapsed_time
-110        )
-111
-112    @staticmethod
-113    def format_time(num_seconds: float, subsecond_resolution: bool = False)
+_86    @property
+_87    def stop_time(self) -> float:
+_88        return self._stop_time
+_89
+_90    @property
+_91    def history(self) -> list[float]:
+_92        return self._history
+_93
+_94    def start(self: Self) -> Self:
+_95        """Start timer.
+_96        Returns this Timer instance so
+_97        timer start can be chained to
+_98        Timer creation.
+_99
+100        >>> timer = Timer().start()"""
+101        self._start_time = time.time()
+102        self._started = True
+103        return self
+104
+105    def stop(self):
+106        """Stop timer.
+107
+108        Calculates elapsed time and average elapsed time."""
+109        self._stop_time = time.time()
+110        self._started = False
+111        self._elapsed = self._stop_time - self._start_time
+112        self._save_elapsed_time()
+113        self._average_elapsed = sum(self._history) / (len(self._history))
+114
+115    def _save_elapsed_time(self):
+116        """Saves current elapsed time to the history buffer
+117        in a FIFO manner."""
+118        if len(self._history) >= self.averaging_window_length:
+119            self._history.pop(0)
+120        self._history.append(self._elapsed)
+121
+122    @staticmethod
+123    def format_time(num_seconds: float, subsecond_resolution: bool = False)
 -> str:
-114        """Returns num_seconds as a string with units.
-115
-116        :param subsecond_resolution: Include milliseconds
-117        and microseconds with the output."""
-118        microsecond = 0.000001
-119        millisecond = 0.001
-120        second = 1
-121        seconds_per_minute = 60
-122        seconds_per_hour = 3600
-123        seconds_per_day = 86400
-124        seconds_per_week = 604800
-125        seconds_per_month = 2419200
-126        seconds_per_year = 29030400
-127        time_units = [
-128            (seconds_per_year, "y"),
-129            (seconds_per_month, "mn"),
-130            (seconds_per_week, "w"),
-131            (seconds_per_day, "d"),
-132            (seconds_per_hour, "h"),
-133            (seconds_per_minute, "m"),
-134            (second, "s"),
-135            (millisecond, "ms"),
-136            (microsecond, "us"),
-137        ]
-138        if not subsecond_resolution:
-139            time_units = time_units[:-2]
-140        time_string = ""
-141        for time_unit in time_units:
-142            unit_amount, num_seconds = divmod(num_seconds, time_unit[0])
-143            if unit_amount > 0:
-144                time_string += f"{int(unit_amount)}{time_unit[1]} "
-145        if time_string == "":
-146            return f"<1{time_units[-1][1]}"
-147        return time_string.strip()
-148
-149    def get_stats(self, format: bool = True, subsecond_resolution: bool =
-False) -> str:
-150        """Returns string for elapsed time and average elapsed time.
-151
-152        :param format: Times are returned as strings if True,
-153        otherwise they're raw floats.
-154
-155        :param subsecond_resolution: Include milliseconds
-156        and microseconds with the output."""
-157        if format:
-158            return f"elapsed time: {self.format_time(self.elapsed_time,
-subsecond_resolution)}\naverage elapsed time: {self.format_time
-(self.average_elapsed_time, subsecond_resolution)}"
-159        else:
-160            return f"elapsed time: {self.elapsed_time}s\naverage elapsed
-time: {self.average_elapsed_time}s"
+124        """Returns num_seconds as a string with units.
+125
+126        :param subsecond_resolution: Include milliseconds
+127        and microseconds with the output."""
+128        microsecond = 0.000001
+129        millisecond = 0.001
+130        second = 1
+131        seconds_per_minute = 60
+132        seconds_per_hour = 3600
+133        seconds_per_day = 86400
+134        seconds_per_week = 604800
+135        seconds_per_month = 2419200
+136        seconds_per_year = 29030400
+137        time_units = [
+138            (seconds_per_year, "y"),
+139            (seconds_per_month, "mn"),
+140            (seconds_per_week, "w"),
+141            (seconds_per_day, "d"),
+142            (seconds_per_hour, "h"),
+143            (seconds_per_minute, "m"),
+144            (second, "s"),
+145            (millisecond, "ms"),
+146            (microsecond, "us"),
+147        ]
+148        if not subsecond_resolution:
+149            time_units = time_units[:-2]
+150        time_string = ""
+151        for time_unit in time_units:
+152            unit_amount, num_seconds = divmod(num_seconds, time_unit[0])
+153            if unit_amount > 0:
+154                time_string += f"{int(unit_amount)}{time_unit[1]} "
+155        if time_string == "":
+156            return f"<1{time_units[-1][1]}"
+157        return time_string.strip()
+158
+159    @property
+160    def stats(self) -> str:
+161        """Returns a string stating the currently elapsed time
+162        and the average elapsed time."""
+163        return f"elapsed time: {self.elapsed_str}\naverage elapsed time:
+{self.average_elapsed_str}"
   ⁰
 def time_it(loops: int = 1) -> Callable[..., Any]: View Source
-_7def time_it(loops: int = 1) -> Callable[..., Any]:
-_8    """Decorator to time function execution time
-_9    and print the results.
-10
-11    :param loops: How many times to loop the function,
-12    starting and stopping the timer before and after
-13    each loop."""
-14
-15    def decorator(func: Callable[..., Any]) -> Callable[..., Any]:
-16        def wrapper(*args, **kwargs) -> Any:
-17            timer = Timer(loops)
-18            for _ in range(loops):
-19                timer.start()
-20                result = func(*args, **kwargs)
-21                timer.stop()
-22            execution_time = timer.format_time(timer.average_elapsed_time,
-True)
-23            print(f"{func.__name__} average execution time:
-{execution_time}")
-24            return result
-25
-26        return wrapper
-27
-28    return decorator
+_8def time_it(loops: int = 1) -> Callable[..., Any]:
+_9    """Decorator to time function execution time
+10    and print the results.
+11
+12    :param loops: How many times to loop the function,
+13    starting and stopping the timer before and after
+14    each loop."""
+15
+16    def decorator(func: Callable[..., Any]) -> Callable[..., Any]:
+17        def wrapper(*args, **kwargs) -> Any:
+18            timer = Timer(loops)
+19            result = None
+20            for _ in range(loops):
+21                timer.start()
+22                result = func(*args, **kwargs)
+23                timer.stop()
+24            print(
+25                f"{func.__name__} average execution time:
+{timer.average_elapsed_str}"
+26            )
+27            return result
+28
+29        return wrapper
+30
+31    return decorator
 Decorator to time function execution time and print the results.
 * Parameters *
     * loops: How many times to loop the function, starting and stopping the
       timer before and after each loop.
   ⁰
 class Timer: View Source
-_31class Timer:
-_32    """Simple timer class that tracks total elapsed time
-_33    and average time between calls to 'start' and 'stop'."""
-_34
-_35    def __init__(
-_36        self, averaging_window_length: int = 10, subsecond_resolution: bool
+_34class Timer:
+_35    """Simple timer class that tracks total elapsed time
+_36    and average time between calls to 'start' and 'stop'."""
+_37
+_38    def __init__(
+_39        self, averaging_window_length: int = 10, subsecond_resolution: bool
 = True
-_37    ):
-_38        """:param averaging_window_length: Number of start/stop cycles
-_39        to calculate the average elapsed time with.
-_40
-_41        :param subsecond_resolution: Whether to print formatted time
-_42        strings with subsecond resolution or not."""
-_43        self.start_time: datetime = datetime.now()
-_44        self.stop_time: datetime = datetime.now()
-_45        self.average_elapsed_time: float = 0
-_46        self.history: list[float] = []
-_47        self.elapsed_time: float = 0
-_48        self.averaging_window_length: int = averaging_window_length
-_49        self.started: bool = False
-_50        self.subsecond_resolution = subsecond_resolution
-_51
-_52    @property
-_53    def elapsed(self) -> float:
-_54        """Return the currently elapsed time."""
-_55        if self.started:
-_56            return (datetime.now() - self.start_time).total_seconds()
-_57        else:
-_58            return (self.stop_time - self.start_time).total_seconds()
-_59
-_60    @property
-_61    def elapsed_str(self) -> str:
-_62        """Return the currently elapsed time
-_63        as a formatted string."""
-_64        return self.format_time(self.elapsed, self.subsecond_resolution)
-_65
-_66    def start(self) -> Self:
-_67        """Start timer.
-_68        Returns this Timer instance so
-_69        timer start can be chained to
-_70        Timer creation.
-_71
-_72        >>> timer = Timer().start()"""
-_73        self.start_time = datetime.now()
-_74        self.started = True
-_75        return self
-_76
-_77    def stop(self):
-_78        """Stop timer.
-_79
-_80        Calculates elapsed time and average elapsed time."""
-_81        self.stop_time = datetime.now()
-_82        self.started = False
-_83        self.elapsed_time = (self.stop_time - self.start_time).total_seconds
-()
-_84        self._save_elapsed_time()
-_85        self.average_elapsed_time = sum(self.history) / (len(self.history))
+_40    ):
+_41        """:param averaging_window_length: Number of start/stop cycles
+_42        to calculate the average elapsed time with.
+_43
+_44        :param subsecond_resolution: Whether to print formatted time
+_45        strings with subsecond resolution or not."""
+_46        self._start_time = time.time()
+_47        self._stop_time = self.start_time
+_48        self._elapsed = 0
+_49        self._average_elapsed = 0
+_50        self._history: list[float] = []
+_51        self._started: bool = False
+_52        self.averaging_window_length: int = averaging_window_length
+_53        self.subsecond_resolution = subsecond_resolution
+_54
+_55    @property
+_56    def started(self) -> bool:
+_57        """Returns whether the timer has
+_58        been started and is currently running."""
+_59        return self._started
+_60
+_61    @property
+_62    def elapsed(self) -> float:
+_63        """Return the currently elapsed time."""
+_64        if self._started:
+_65            return time.time() - self._start_time
+_66        else:
+_67            return self._elapsed
+_68
+_69    @property
+_70    def elapsed_str(self) -> str:
+_71        """Return the currently elapsed time
+_72        as a formatted string."""
+_73        return self.format_time(self.elapsed, self.subsecond_resolution)
+_74
+_75    @property
+_76    def average_elapsed(self) -> float:
+_77        return self._average_elapsed
+_78
+_79    @property
+_80    def average_elapsed_str(self) -> str:
+_81        return self.format_time(self._average_elapsed,
+self.subsecond_resolution)
+_82
+_83    @property
+_84    def start_time(self) -> float:
+_85        return self._start_time
 _86
-_87    def _save_elapsed_time(self):
-_88        """Saves current elapsed time to the history buffer
-_89        in a FIFO manner."""
-_90        if len(self.history) >= self.averaging_window_length:
-_91            self.history.pop(0)
-_92        self.history.append(self.elapsed_time)
-_93
-_94    def current_elapsed_time(
-_95        self, format: bool = True, subsecond_resolution: bool = False
-_96    ) -> float | str:
-_97        """Returns current elapsed without stopping the timer.
-_98
-_99        :param format: If True, elapsed time is returned as a string.
-100        If False, elapsed time is returned as a float."""
-101        warnings.warn(
-102            "current_elapsed_time is depreciated. Use 'elapsed' and
-'elapsed_str' properties instead.",
-103            FutureWarning,
-104            2,
-105        )
-106        self.elapsed_time = (datetime.now() - self.start_time).total_seconds
-()
-107        return (
-108            self.format_time(self.elapsed_time, subsecond_resolution)
-109            if format
-110            else self.elapsed_time
-111        )
-112
-113    @staticmethod
-114    def format_time(num_seconds: float, subsecond_resolution: bool = False)
+_87    @property
+_88    def stop_time(self) -> float:
+_89        return self._stop_time
+_90
+_91    @property
+_92    def history(self) -> list[float]:
+_93        return self._history
+_94
+_95    def start(self: Self) -> Self:
+_96        """Start timer.
+_97        Returns this Timer instance so
+_98        timer start can be chained to
+_99        Timer creation.
+100
+101        >>> timer = Timer().start()"""
+102        self._start_time = time.time()
+103        self._started = True
+104        return self
+105
+106    def stop(self):
+107        """Stop timer.
+108
+109        Calculates elapsed time and average elapsed time."""
+110        self._stop_time = time.time()
+111        self._started = False
+112        self._elapsed = self._stop_time - self._start_time
+113        self._save_elapsed_time()
+114        self._average_elapsed = sum(self._history) / (len(self._history))
+115
+116    def _save_elapsed_time(self):
+117        """Saves current elapsed time to the history buffer
+118        in a FIFO manner."""
+119        if len(self._history) >= self.averaging_window_length:
+120            self._history.pop(0)
+121        self._history.append(self._elapsed)
+122
+123    @staticmethod
+124    def format_time(num_seconds: float, subsecond_resolution: bool = False)
 -> str:
-115        """Returns num_seconds as a string with units.
-116
-117        :param subsecond_resolution: Include milliseconds
-118        and microseconds with the output."""
-119        microsecond = 0.000001
-120        millisecond = 0.001
-121        second = 1
-122        seconds_per_minute = 60
-123        seconds_per_hour = 3600
-124        seconds_per_day = 86400
-125        seconds_per_week = 604800
-126        seconds_per_month = 2419200
-127        seconds_per_year = 29030400
-128        time_units = [
-129            (seconds_per_year, "y"),
-130            (seconds_per_month, "mn"),
-131            (seconds_per_week, "w"),
-132            (seconds_per_day, "d"),
-133            (seconds_per_hour, "h"),
-134            (seconds_per_minute, "m"),
-135            (second, "s"),
-136            (millisecond, "ms"),
-137            (microsecond, "us"),
-138        ]
-139        if not subsecond_resolution:
-140            time_units = time_units[:-2]
-141        time_string = ""
-142        for time_unit in time_units:
-143            unit_amount, num_seconds = divmod(num_seconds, time_unit[0])
-144            if unit_amount > 0:
-145                time_string += f"{int(unit_amount)}{time_unit[1]} "
-146        if time_string == "":
-147            return f"<1{time_units[-1][1]}"
-148        return time_string.strip()
-149
-150    def get_stats(self, format: bool = True, subsecond_resolution: bool =
-False) -> str:
-151        """Returns string for elapsed time and average elapsed time.
-152
-153        :param format: Times are returned as strings if True,
-154        otherwise they're raw floats.
-155
-156        :param subsecond_resolution: Include milliseconds
-157        and microseconds with the output."""
-158        if format:
-159            return f"elapsed time: {self.format_time(self.elapsed_time,
-subsecond_resolution)}\naverage elapsed time: {self.format_time
-(self.average_elapsed_time, subsecond_resolution)}"
-160        else:
-161            return f"elapsed time: {self.elapsed_time}s\naverage elapsed
-time: {self.average_elapsed_time}s"
+125        """Returns num_seconds as a string with units.
+126
+127        :param subsecond_resolution: Include milliseconds
+128        and microseconds with the output."""
+129        microsecond = 0.000001
+130        millisecond = 0.001
+131        second = 1
+132        seconds_per_minute = 60
+133        seconds_per_hour = 3600
+134        seconds_per_day = 86400
+135        seconds_per_week = 604800
+136        seconds_per_month = 2419200
+137        seconds_per_year = 29030400
+138        time_units = [
+139            (seconds_per_year, "y"),
+140            (seconds_per_month, "mn"),
+141            (seconds_per_week, "w"),
+142            (seconds_per_day, "d"),
+143            (seconds_per_hour, "h"),
+144            (seconds_per_minute, "m"),
+145            (second, "s"),
+146            (millisecond, "ms"),
+147            (microsecond, "us"),
+148        ]
+149        if not subsecond_resolution:
+150            time_units = time_units[:-2]
+151        time_string = ""
+152        for time_unit in time_units:
+153            unit_amount, num_seconds = divmod(num_seconds, time_unit[0])
+154            if unit_amount > 0:
+155                time_string += f"{int(unit_amount)}{time_unit[1]} "
+156        if time_string == "":
+157            return f"<1{time_units[-1][1]}"
+158        return time_string.strip()
+159
+160    @property
+161    def stats(self) -> str:
+162        """Returns a string stating the currently elapsed time
+163        and the average elapsed time."""
+164        return f"elapsed time: {self.elapsed_str}\naverage elapsed time:
+{self.average_elapsed_str}"
 Simple timer class that tracks total elapsed time and average time between
 calls to 'start' and 'stop'.
 ⁰
 Timer(averaging_window_length: int = 10, subsecond_resolution: bool = True)
 View Source
-35    def __init__(
-36        self, averaging_window_length: int = 10, subsecond_resolution: bool =
+38    def __init__(
+39        self, averaging_window_length: int = 10, subsecond_resolution: bool =
 True
-37    ):
-38        """:param averaging_window_length: Number of start/stop cycles
-39        to calculate the average elapsed time with.
-40
-41        :param subsecond_resolution: Whether to print formatted time
-42        strings with subsecond resolution or not."""
-43        self.start_time: datetime = datetime.now()
-44        self.stop_time: datetime = datetime.now()
-45        self.average_elapsed_time: float = 0
-46        self.history: list[float] = []
-47        self.elapsed_time: float = 0
-48        self.averaging_window_length: int = averaging_window_length
-49        self.started: bool = False
-50        self.subsecond_resolution = subsecond_resolution
+40    ):
+41        """:param averaging_window_length: Number of start/stop cycles
+42        to calculate the average elapsed time with.
+43
+44        :param subsecond_resolution: Whether to print formatted time
+45        strings with subsecond resolution or not."""
+46        self._start_time = time.time()
+47        self._stop_time = self.start_time
+48        self._elapsed = 0
+49        self._average_elapsed = 0
+50        self._history: list[float] = []
+51        self._started: bool = False
+52        self.averaging_window_length: int = averaging_window_length
+53        self.subsecond_resolution = subsecond_resolution
 * Parameters *
     * averaging_window_length: Number of start/stop cycles to calculate the
       average elapsed time with.
     * subsecond_resolution: Whether to print formatted time strings with
       subsecond resolution or not.
+started: bool
+Returns whether the timer has been started and is currently running.
 elapsed: float
 Return the currently elapsed time.
 elapsed_str: str
 Return the currently elapsed time as a formatted string.
 ⁰
-def start(self) -> Self: View Source
-66    def start(self) -> Self:
-67        """Start timer.
-68        Returns this Timer instance so
-69        timer start can be chained to
-70        Timer creation.
-71
-72        >>> timer = Timer().start()"""
-73        self.start_time = datetime.now()
-74        self.started = True
-75        return self
+def start(self: Self) -> Self: View Source
+_95    def start(self: Self) -> Self:
+_96        """Start timer.
+_97        Returns this Timer instance so
+_98        timer start can be chained to
+_99        Timer creation.
+100
+101        >>> timer = Timer().start()"""
+102        self._start_time = time.time()
+103        self._started = True
+104        return self
 Start timer. Returns this Timer instance so timer start can be chained to Timer
 creation.
 >>> timer = Timer().start()
 ⁰
 def stop(self): View Source
-77    def stop(self):
-78        """Stop timer.
-79
-80        Calculates elapsed time and average elapsed time."""
-81        self.stop_time = datetime.now()
-82        self.started = False
-83        self.elapsed_time = (self.stop_time - self.start_time).total_seconds
-()
-84        self._save_elapsed_time()
-85        self.average_elapsed_time = sum(self.history) / (len(self.history))
+106    def stop(self):
+107        """Stop timer.
+108
+109        Calculates elapsed time and average elapsed time."""
+110        self._stop_time = time.time()
+111        self._started = False
+112        self._elapsed = self._stop_time - self._start_time
+113        self._save_elapsed_time()
+114        self._average_elapsed = sum(self._history) / (len(self._history))
 Stop timer.
 Calculates elapsed time and average elapsed time.
 ⁰
-def current_elapsed_time(
-self,
-format: bool = True,
-subsecond_resolution: bool = False) -> float | str: View Source
-_94    def current_elapsed_time(
-_95        self, format: bool = True, subsecond_resolution: bool = False
-_96    ) -> float | str:
-_97        """Returns current elapsed without stopping the timer.
-_98
-_99        :param format: If True, elapsed time is returned as a string.
-100        If False, elapsed time is returned as a float."""
-101        warnings.warn(
-102            "current_elapsed_time is depreciated. Use 'elapsed' and
-'elapsed_str' properties instead.",
-103            FutureWarning,
-104            2,
-105        )
-106        self.elapsed_time = (datetime.now() - self.start_time).total_seconds
-()
-107        return (
-108            self.format_time(self.elapsed_time, subsecond_resolution)
-109            if format
-110            else self.elapsed_time
-111        )
-Returns current elapsed without stopping the timer.
-* Parameters *
-    * format: If True, elapsed time is returned as a string. If False, elapsed
-      time is returned as a float.
-⁰
 @staticmethod
 def format_time(num_seconds: float, subsecond_resolution: bool = False) -> str:
 View Source
-113    @staticmethod
-114    def format_time(num_seconds: float, subsecond_resolution: bool = False)
+123    @staticmethod
+124    def format_time(num_seconds: float, subsecond_resolution: bool = False)
 -> str:
-115        """Returns num_seconds as a string with units.
-116
-117        :param subsecond_resolution: Include milliseconds
-118        and microseconds with the output."""
-119        microsecond = 0.000001
-120        millisecond = 0.001
-121        second = 1
-122        seconds_per_minute = 60
-123        seconds_per_hour = 3600
-124        seconds_per_day = 86400
-125        seconds_per_week = 604800
-126        seconds_per_month = 2419200
-127        seconds_per_year = 29030400
-128        time_units = [
-129            (seconds_per_year, "y"),
-130            (seconds_per_month, "mn"),
-131            (seconds_per_week, "w"),
-132            (seconds_per_day, "d"),
-133            (seconds_per_hour, "h"),
-134            (seconds_per_minute, "m"),
-135            (second, "s"),
-136            (millisecond, "ms"),
-137            (microsecond, "us"),
-138        ]
-139        if not subsecond_resolution:
-140            time_units = time_units[:-2]
-141        time_string = ""
-142        for time_unit in time_units:
-143            unit_amount, num_seconds = divmod(num_seconds, time_unit[0])
-144            if unit_amount > 0:
-145                time_string += f"{int(unit_amount)}{time_unit[1]} "
-146        if time_string == "":
-147            return f"<1{time_units[-1][1]}"
-148        return time_string.strip()
+125        """Returns num_seconds as a string with units.
+126
+127        :param subsecond_resolution: Include milliseconds
+128        and microseconds with the output."""
+129        microsecond = 0.000001
+130        millisecond = 0.001
+131        second = 1
+132        seconds_per_minute = 60
+133        seconds_per_hour = 3600
+134        seconds_per_day = 86400
+135        seconds_per_week = 604800
+136        seconds_per_month = 2419200
+137        seconds_per_year = 29030400
+138        time_units = [
+139            (seconds_per_year, "y"),
+140            (seconds_per_month, "mn"),
+141            (seconds_per_week, "w"),
+142            (seconds_per_day, "d"),
+143            (seconds_per_hour, "h"),
+144            (seconds_per_minute, "m"),
+145            (second, "s"),
+146            (millisecond, "ms"),
+147            (microsecond, "us"),
+148        ]
+149        if not subsecond_resolution:
+150            time_units = time_units[:-2]
+151        time_string = ""
+152        for time_unit in time_units:
+153            unit_amount, num_seconds = divmod(num_seconds, time_unit[0])
+154            if unit_amount > 0:
+155                time_string += f"{int(unit_amount)}{time_unit[1]} "
+156        if time_string == "":
+157            return f"<1{time_units[-1][1]}"
+158        return time_string.strip()
 Returns num_seconds as a string with units.
 * Parameters *
     * subsecond_resolution: Include milliseconds and microseconds with the
       output.
-⁰
-def get_stats(self, format: bool = True, subsecond_resolution: bool = False) -
-> str: View Source
-150    def get_stats(self, format: bool = True, subsecond_resolution: bool =
-False) -> str:
-151        """Returns string for elapsed time and average elapsed time.
-152
-153        :param format: Times are returned as strings if True,
-154        otherwise they're raw floats.
-155
-156        :param subsecond_resolution: Include milliseconds
-157        and microseconds with the output."""
-158        if format:
-159            return f"elapsed time: {self.format_time(self.elapsed_time,
-subsecond_resolution)}\naverage elapsed time: {self.format_time
-(self.average_elapsed_time, subsecond_resolution)}"
-160        else:
-161            return f"elapsed time: {self.elapsed_time}s\naverage elapsed
-time: {self.average_elapsed_time}s"
-Returns string for elapsed time and average elapsed time.
-* Parameters *
-    * format: Times are returned as strings if True, otherwise they're raw
-      floats.
-    * subsecond_resolution: Include milliseconds and microseconds with the
-      output.
+stats: str
+Returns a string stating the currently elapsed time and the average elapsed
+time.
```

### Comparing `noiftimer-1.3.0/src/noiftimer/noiftimer.py` & `noiftimer-2.0.0/src/noiftimer/noiftimer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,32 @@
-import warnings
-from datetime import datetime
-from typing import Any, Callable, Self
+import time
+from typing import Any, Callable
+
+from typing_extensions import Self
 
 
 def time_it(loops: int = 1) -> Callable[..., Any]:
     """Decorator to time function execution time
     and print the results.
 
     :param loops: How many times to loop the function,
     starting and stopping the timer before and after
     each loop."""
 
     def decorator(func: Callable[..., Any]) -> Callable[..., Any]:
         def wrapper(*args, **kwargs) -> Any:
             timer = Timer(loops)
+            result = None
             for _ in range(loops):
                 timer.start()
                 result = func(*args, **kwargs)
                 timer.stop()
-            execution_time = timer.format_time(timer.average_elapsed_time, True)
-            print(f"{func.__name__} average execution time: {execution_time}")
+            print(
+                f"{func.__name__} average execution time: {timer.average_elapsed_str}"
+            )
             return result
 
         return wrapper
 
     return decorator
 
 
@@ -35,83 +38,90 @@
         self, averaging_window_length: int = 10, subsecond_resolution: bool = True
     ):
         """:param averaging_window_length: Number of start/stop cycles
         to calculate the average elapsed time with.
 
         :param subsecond_resolution: Whether to print formatted time
         strings with subsecond resolution or not."""
-        self.start_time: datetime = datetime.now()
-        self.stop_time: datetime = datetime.now()
-        self.average_elapsed_time: float = 0
-        self.history: list[float] = []
-        self.elapsed_time: float = 0
+        self._start_time = time.time()
+        self._stop_time = self.start_time
+        self._elapsed = 0
+        self._average_elapsed = 0
+        self._history: list[float] = []
+        self._started: bool = False
         self.averaging_window_length: int = averaging_window_length
-        self.started: bool = False
         self.subsecond_resolution = subsecond_resolution
 
     @property
+    def started(self) -> bool:
+        """Returns whether the timer has
+        been started and is currently running."""
+        return self._started
+
+    @property
     def elapsed(self) -> float:
         """Return the currently elapsed time."""
-        if self.started:
-            return (datetime.now() - self.start_time).total_seconds()
+        if self._started:
+            return time.time() - self._start_time
         else:
-            return (self.stop_time - self.start_time).total_seconds()
+            return self._elapsed
 
     @property
     def elapsed_str(self) -> str:
         """Return the currently elapsed time
         as a formatted string."""
         return self.format_time(self.elapsed, self.subsecond_resolution)
 
-    def start(self) -> Self:
+    @property
+    def average_elapsed(self) -> float:
+        return self._average_elapsed
+
+    @property
+    def average_elapsed_str(self) -> str:
+        return self.format_time(self._average_elapsed, self.subsecond_resolution)
+
+    @property
+    def start_time(self) -> float:
+        return self._start_time
+
+    @property
+    def stop_time(self) -> float:
+        return self._stop_time
+
+    @property
+    def history(self) -> list[float]:
+        return self._history
+
+    def start(self: Self) -> Self:
         """Start timer.
         Returns this Timer instance so
         timer start can be chained to
         Timer creation.
 
         >>> timer = Timer().start()"""
-        self.start_time = datetime.now()
-        self.started = True
+        self._start_time = time.time()
+        self._started = True
         return self
 
     def stop(self):
         """Stop timer.
 
         Calculates elapsed time and average elapsed time."""
-        self.stop_time = datetime.now()
-        self.started = False
-        self.elapsed_time = (self.stop_time - self.start_time).total_seconds()
+        self._stop_time = time.time()
+        self._started = False
+        self._elapsed = self._stop_time - self._start_time
         self._save_elapsed_time()
-        self.average_elapsed_time = sum(self.history) / (len(self.history))
+        self._average_elapsed = sum(self._history) / (len(self._history))
 
     def _save_elapsed_time(self):
         """Saves current elapsed time to the history buffer
         in a FIFO manner."""
-        if len(self.history) >= self.averaging_window_length:
-            self.history.pop(0)
-        self.history.append(self.elapsed_time)
-
-    def current_elapsed_time(
-        self, format: bool = True, subsecond_resolution: bool = False
-    ) -> float | str:
-        """Returns current elapsed without stopping the timer.
-
-        :param format: If True, elapsed time is returned as a string.
-        If False, elapsed time is returned as a float."""
-        warnings.warn(
-            "current_elapsed_time is depreciated. Use 'elapsed' and 'elapsed_str' properties instead.",
-            FutureWarning,
-            2,
-        )
-        self.elapsed_time = (datetime.now() - self.start_time).total_seconds()
-        return (
-            self.format_time(self.elapsed_time, subsecond_resolution)
-            if format
-            else self.elapsed_time
-        )
+        if len(self._history) >= self.averaging_window_length:
+            self._history.pop(0)
+        self._history.append(self._elapsed)
 
     @staticmethod
     def format_time(num_seconds: float, subsecond_resolution: bool = False) -> str:
         """Returns num_seconds as a string with units.
 
         :param subsecond_resolution: Include milliseconds
         and microseconds with the output."""
@@ -142,19 +152,12 @@
             unit_amount, num_seconds = divmod(num_seconds, time_unit[0])
             if unit_amount > 0:
                 time_string += f"{int(unit_amount)}{time_unit[1]} "
         if time_string == "":
             return f"<1{time_units[-1][1]}"
         return time_string.strip()
 
-    def get_stats(self, format: bool = True, subsecond_resolution: bool = False) -> str:
-        """Returns string for elapsed time and average elapsed time.
-
-        :param format: Times are returned as strings if True,
-        otherwise they're raw floats.
-
-        :param subsecond_resolution: Include milliseconds
-        and microseconds with the output."""
-        if format:
-            return f"elapsed time: {self.format_time(self.elapsed_time, subsecond_resolution)}\naverage elapsed time: {self.format_time(self.average_elapsed_time, subsecond_resolution)}"
-        else:
-            return f"elapsed time: {self.elapsed_time}s\naverage elapsed time: {self.average_elapsed_time}s"
+    @property
+    def stats(self) -> str:
+        """Returns a string stating the currently elapsed time
+        and the average elapsed time."""
+        return f"elapsed time: {self.elapsed_str}\naverage elapsed time: {self.average_elapsed_str}"
```

### Comparing `noiftimer-1.3.0/LICENSE.txt` & `noiftimer-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `noiftimer-1.3.0/README.md` & `noiftimer-2.0.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,42 @@
 # noiftimer
-Simple timer class to track average elapsed time with optional sub-second precision.<br>
+Simple timer class to track elapsed time.<br>
 Install with:
 <pre>pip install noiftimer</pre>
 
 Usage:
 <pre>
-from noiftimer import Timer
-import time
-
-def very_complicated_function():
-    time.sleep(1)
-
-timer = Timer()
-for _ in range(10):
-    timer.start()
-    very_complicated_function()
-    timer.stop()
-print(f'{timer.average_elapsed_time=}')
-print(timer.get_stats(subsecond_resolution=True))
+>>> from noiftimer import Timer, time_it
+>>> import time
+</pre>
+Timer object
+<pre>
+>>> def very_complicated_function():
+...     time.sleep(1)
+...
+>>> timer = Timer()
+>>> for _ in range(10):
+...     timer.start()
+...     very_complicated_function()
+...     timer.stop()
+...
+>>> print(timer.stats)
+elapsed time: 1s 1ms 173us
+average elapsed time: 1s 912us
+>>> timer.elapsed
+1.001173496246338
+>>> timer.elapsed_str
+'1s 1ms 173us'
+>>> timer.average_elapsed
+1.0009121656417848
+>>> timer.average_elapsed_str
+'1s 912us'
 </pre>
-produces
+time_it decorator (executes the decorated function 10 times)
 <pre>
-timer.average_elapsed_time=1.0006019
-elapsed time: 1s 836us
-average elapsed time: 1s 601us
+>>> @time_it(10)
+... def very_complicated_function():
+...     time.sleep(1)
+...
+>>> very_complicated_function()
+very_complicated_function average execution time: 1s 469us
 </pre>
```

### Comparing `noiftimer-1.3.0/pyproject.toml` & `noiftimer-2.0.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "noiftimer"
 authors = [{name="Matt Manes"}]
 description = "Timing class for measuring elapsed time and average elapsed time."
-version = "1.3.0"
-requires-python = ">=3.11"
-dependencies = ["pytest"]
+version = "2.0.0"
+requires-python = ">=3.9"
+dependencies = ["pytest", "typing_extensions"]
 readme = "README.md"
 keywords = [
     "timer",
     "timing"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `noiftimer-1.3.0/PKG-INFO` & `noiftimer-2.0.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,44 +1,60 @@
 Metadata-Version: 2.1
 Name: noiftimer
-Version: 1.3.0
+Version: 2.0.0
 Summary: Timing class for measuring elapsed time and average elapsed time.
 Project-URL: Homepage, https://github.com/matt-manes/noiftimer
 Project-URL: Documentation, https://github.com/matt-manes/noiftimer/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/noiftimer/tree/main/src/noiftimer
 Author: Matt Manes
 License-File: LICENSE.txt
 Keywords: timer,timing
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.11
+Requires-Python: >=3.9
 Requires-Dist: pytest
+Requires-Dist: typing-extensions
 Description-Content-Type: text/markdown
 
 # noiftimer
-Simple timer class to track average elapsed time with optional sub-second precision.<br>
+Simple timer class to track elapsed time.<br>
 Install with:
 <pre>pip install noiftimer</pre>
 
 Usage:
 <pre>
-from noiftimer import Timer
-import time
-
-def very_complicated_function():
-    time.sleep(1)
-
-timer = Timer()
-for _ in range(10):
-    timer.start()
-    very_complicated_function()
-    timer.stop()
-print(f'{timer.average_elapsed_time=}')
-print(timer.get_stats(subsecond_resolution=True))
+>>> from noiftimer import Timer, time_it
+>>> import time
+</pre>
+Timer object
+<pre>
+>>> def very_complicated_function():
+...     time.sleep(1)
+...
+>>> timer = Timer()
+>>> for _ in range(10):
+...     timer.start()
+...     very_complicated_function()
+...     timer.stop()
+...
+>>> print(timer.stats)
+elapsed time: 1s 1ms 173us
+average elapsed time: 1s 912us
+>>> timer.elapsed
+1.001173496246338
+>>> timer.elapsed_str
+'1s 1ms 173us'
+>>> timer.average_elapsed
+1.0009121656417848
+>>> timer.average_elapsed_str
+'1s 912us'
 </pre>
-produces
+time_it decorator (executes the decorated function 10 times)
 <pre>
-timer.average_elapsed_time=1.0006019
-elapsed time: 1s 836us
-average elapsed time: 1s 601us
+>>> @time_it(10)
+... def very_complicated_function():
+...     time.sleep(1)
+...
+>>> very_complicated_function()
+very_complicated_function average execution time: 1s 469us
 </pre>
```

