# Comparing `tmp/bandripper-0.1.4.tar.gz` & `tmp/bandripper-0.1.5.tar.gz`

## Comparing `bandripper-0.1.4.tar` & `bandripper-0.1.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 bandripper-0.1.4/CHANGELOG.md
--rw-r--r--   0        0        0    33565 2020-02-02 00:00:00.000000 bandripper-0.1.4/docs/bandripper.html
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bandripper-0.1.4/docs/index.html
--rw-r--r--   0        0        0    30351 2020-02-02 00:00:00.000000 bandripper-0.1.4/docs/search.js
--rw-r--r--   0        0        0   229819 2020-02-02 00:00:00.000000 bandripper-0.1.4/docs/bandripper/bandripper.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bandripper-0.1.4/src/bandripper/__init__.py
--rw-r--r--   0        0        0     9673 2020-02-02 00:00:00.000000 bandripper-0.1.4/src/bandripper/bandripper.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 bandripper-0.1.4/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 bandripper-0.1.4/LICENSE.txt
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 bandripper-0.1.4/README.md
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 bandripper-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 bandripper-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 bandripper-0.1.5/CHANGELOG.md
+-rw-r--r--   0        0        0    33565 2020-02-02 00:00:00.000000 bandripper-0.1.5/docs/bandripper.html
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bandripper-0.1.5/docs/index.html
+-rw-r--r--   0        0        0    30351 2020-02-02 00:00:00.000000 bandripper-0.1.5/docs/search.js
+-rw-r--r--   0        0        0   228834 2020-02-02 00:00:00.000000 bandripper-0.1.5/docs/bandripper/bandripper.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bandripper-0.1.5/src/bandripper/__init__.py
+-rw-r--r--   0        0        0     9624 2020-02-02 00:00:00.000000 bandripper-0.1.5/src/bandripper/bandripper.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 bandripper-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 bandripper-0.1.5/LICENSE.txt
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 bandripper-0.1.5/README.md
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 bandripper-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 bandripper-0.1.5/PKG-INFO
```

### Comparing `bandripper-0.1.4/docs/bandripper.html` & `bandripper-0.1.5/docs/bandripper.html`

 * *Files identical despite different names*

### Comparing `bandripper-0.1.4/docs/search.js` & `bandripper-0.1.5/docs/search.js`

 * *Files identical despite different names*

### Comparing `bandripper-0.1.4/docs/bandripper/bandripper.html` & `bandripper-0.1.5/docs/bandripper/bandripper.html`

 * *Files 0% similar despite different names*

```diff
@@ -131,284 +131,282 @@
 </span><span id="L-3"><a href="#L-3"><span class="linenos">  3</span></a><span class="kn">import</span> <span class="nn">re</span>
 </span><span id="L-4"><a href="#L-4"><span class="linenos">  4</span></a><span class="kn">import</span> <span class="nn">string</span>
 </span><span id="L-5"><a href="#L-5"><span class="linenos">  5</span></a><span class="kn">from</span> <span class="nn">dataclasses</span> <span class="kn">import</span> <span class="n">dataclass</span>
 </span><span id="L-6"><a href="#L-6"><span class="linenos">  6</span></a><span class="kn">from</span> <span class="nn">pathlib</span> <span class="kn">import</span> <span class="n">Path</span>
 </span><span id="L-7"><a href="#L-7"><span class="linenos">  7</span></a><span class="kn">from</span> <span class="nn">urllib.parse</span> <span class="kn">import</span> <span class="n">urlparse</span>
 </span><span id="L-8"><a href="#L-8"><span class="linenos">  8</span></a>
 </span><span id="L-9"><a href="#L-9"><span class="linenos">  9</span></a><span class="kn">import</span> <span class="nn">requests</span>
-</span><span id="L-10"><a href="#L-10"><span class="linenos"> 10</span></a><span class="kn">from</span> <span class="nn">bs4</span> <span class="kn">import</span> <span class="n">BeautifulSoup</span>
-</span><span id="L-11"><a href="#L-11"><span class="linenos"> 11</span></a>
-</span><span id="L-12"><a href="#L-12"><span class="linenos"> 12</span></a><span class="kn">import</span> <span class="nn">whosyouragent</span>
-</span><span id="L-13"><a href="#L-13"><span class="linenos"> 13</span></a><span class="kn">from</span> <span class="nn">noiftimer</span> <span class="kn">import</span> <span class="n">Timer</span>
-</span><span id="L-14"><a href="#L-14"><span class="linenos"> 14</span></a><span class="kn">from</span> <span class="nn">printbuddies</span> <span class="kn">import</span> <span class="n">ProgBar</span>
-</span><span id="L-15"><a href="#L-15"><span class="linenos"> 15</span></a>
-</span><span id="L-16"><a href="#L-16"><span class="linenos"> 16</span></a><span class="n">root</span> <span class="o">=</span> <span class="n">Path</span><span class="p">(</span><span class="vm">__file__</span><span class="p">)</span><span class="o">.</span><span class="n">parent</span>
+</span><span id="L-10"><a href="#L-10"><span class="linenos"> 10</span></a><span class="kn">import</span> <span class="nn">whosyouragent</span>
+</span><span id="L-11"><a href="#L-11"><span class="linenos"> 11</span></a><span class="kn">from</span> <span class="nn">bs4</span> <span class="kn">import</span> <span class="n">BeautifulSoup</span>
+</span><span id="L-12"><a href="#L-12"><span class="linenos"> 12</span></a><span class="kn">from</span> <span class="nn">noiftimer</span> <span class="kn">import</span> <span class="n">Timer</span>
+</span><span id="L-13"><a href="#L-13"><span class="linenos"> 13</span></a><span class="kn">from</span> <span class="nn">printbuddies</span> <span class="kn">import</span> <span class="n">ProgBar</span>
+</span><span id="L-14"><a href="#L-14"><span class="linenos"> 14</span></a>
+</span><span id="L-15"><a href="#L-15"><span class="linenos"> 15</span></a><span class="n">root</span> <span class="o">=</span> <span class="n">Path</span><span class="p">(</span><span class="vm">__file__</span><span class="p">)</span><span class="o">.</span><span class="n">parent</span>
+</span><span id="L-16"><a href="#L-16"><span class="linenos"> 16</span></a>
 </span><span id="L-17"><a href="#L-17"><span class="linenos"> 17</span></a>
-</span><span id="L-18"><a href="#L-18"><span class="linenos"> 18</span></a>
-</span><span id="L-19"><a href="#L-19"><span class="linenos"> 19</span></a><span class="k">def</span> <span class="nf">clean_string</span><span class="p">(</span><span class="n">text</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="L-20"><a href="#L-20"><span class="linenos"> 20</span></a>    <span class="sd">&quot;&quot;&quot;Remove punctuation and trailing spaces from text.&quot;&quot;&quot;</span>
-</span><span id="L-21"><a href="#L-21"><span class="linenos"> 21</span></a>    <span class="k">return</span> <span class="n">re</span><span class="o">.</span><span class="n">sub</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;[</span><span class="si">{</span><span class="n">re</span><span class="o">.</span><span class="n">escape</span><span class="p">(</span><span class="n">string</span><span class="o">.</span><span class="n">punctuation</span><span class="p">)</span><span class="si">}</span><span class="s2">]&quot;</span><span class="p">,</span> <span class="s2">&quot;&quot;</span><span class="p">,</span> <span class="n">text</span><span class="p">)</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
+</span><span id="L-18"><a href="#L-18"><span class="linenos"> 18</span></a><span class="k">def</span> <span class="nf">clean_string</span><span class="p">(</span><span class="n">text</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="L-19"><a href="#L-19"><span class="linenos"> 19</span></a>    <span class="sd">&quot;&quot;&quot;Remove punctuation and trailing spaces from text.&quot;&quot;&quot;</span>
+</span><span id="L-20"><a href="#L-20"><span class="linenos"> 20</span></a>    <span class="k">return</span> <span class="n">re</span><span class="o">.</span><span class="n">sub</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;[</span><span class="si">{</span><span class="n">re</span><span class="o">.</span><span class="n">escape</span><span class="p">(</span><span class="n">string</span><span class="o">.</span><span class="n">punctuation</span><span class="p">)</span><span class="si">}</span><span class="s2">]&quot;</span><span class="p">,</span> <span class="s2">&quot;&quot;</span><span class="p">,</span> <span class="n">text</span><span class="p">)</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
+</span><span id="L-21"><a href="#L-21"><span class="linenos"> 21</span></a>
 </span><span id="L-22"><a href="#L-22"><span class="linenos"> 22</span></a>
-</span><span id="L-23"><a href="#L-23"><span class="linenos"> 23</span></a>
-</span><span id="L-24"><a href="#L-24"><span class="linenos"> 24</span></a><span class="nd">@dataclass</span>
-</span><span id="L-25"><a href="#L-25"><span class="linenos"> 25</span></a><span class="k">class</span> <span class="nc">Track</span><span class="p">:</span>
-</span><span id="L-26"><a href="#L-26"><span class="linenos"> 26</span></a>    <span class="n">title</span><span class="p">:</span> <span class="nb">str</span>
-</span><span id="L-27"><a href="#L-27"><span class="linenos"> 27</span></a>    <span class="n">number</span><span class="p">:</span> <span class="nb">int</span>
-</span><span id="L-28"><a href="#L-28"><span class="linenos"> 28</span></a>    <span class="n">url</span><span class="p">:</span> <span class="nb">str</span>
-</span><span id="L-29"><a href="#L-29"><span class="linenos"> 29</span></a>
-</span><span id="L-30"><a href="#L-30"><span class="linenos"> 30</span></a>    <span class="k">def</span> <span class="nf">__post_init__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="L-31"><a href="#L-31"><span class="linenos"> 31</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">title</span> <span class="o">=</span> <span class="n">clean_string</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">title</span><span class="p">)</span>
-</span><span id="L-32"><a href="#L-32"><span class="linenos"> 32</span></a>
-</span><span id="L-33"><a href="#L-33"><span class="linenos"> 33</span></a>    <span class="nd">@property</span>
-</span><span id="L-34"><a href="#L-34"><span class="linenos"> 34</span></a>    <span class="k">def</span> <span class="nf">numbered_title</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="L-35"><a href="#L-35"><span class="linenos"> 35</span></a>        <span class="n">num</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">number</span><span class="p">)</span>
-</span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">num</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
-</span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a>            <span class="n">num</span> <span class="o">=</span> <span class="s2">&quot;0&quot;</span> <span class="o">+</span> <span class="n">num</span>
-</span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">num</span><span class="si">}</span><span class="s2"> - </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">title</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-23"><a href="#L-23"><span class="linenos"> 23</span></a><span class="nd">@dataclass</span>
+</span><span id="L-24"><a href="#L-24"><span class="linenos"> 24</span></a><span class="k">class</span> <span class="nc">Track</span><span class="p">:</span>
+</span><span id="L-25"><a href="#L-25"><span class="linenos"> 25</span></a>    <span class="n">title</span><span class="p">:</span> <span class="nb">str</span>
+</span><span id="L-26"><a href="#L-26"><span class="linenos"> 26</span></a>    <span class="n">number</span><span class="p">:</span> <span class="nb">int</span>
+</span><span id="L-27"><a href="#L-27"><span class="linenos"> 27</span></a>    <span class="n">url</span><span class="p">:</span> <span class="nb">str</span>
+</span><span id="L-28"><a href="#L-28"><span class="linenos"> 28</span></a>
+</span><span id="L-29"><a href="#L-29"><span class="linenos"> 29</span></a>    <span class="k">def</span> <span class="nf">__post_init__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-30"><a href="#L-30"><span class="linenos"> 30</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">title</span> <span class="o">=</span> <span class="n">clean_string</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">title</span><span class="p">)</span>
+</span><span id="L-31"><a href="#L-31"><span class="linenos"> 31</span></a>
+</span><span id="L-32"><a href="#L-32"><span class="linenos"> 32</span></a>    <span class="nd">@property</span>
+</span><span id="L-33"><a href="#L-33"><span class="linenos"> 33</span></a>    <span class="k">def</span> <span class="nf">numbered_title</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-34"><a href="#L-34"><span class="linenos"> 34</span></a>        <span class="n">num</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">number</span><span class="p">)</span>
+</span><span id="L-35"><a href="#L-35"><span class="linenos"> 35</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">num</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
+</span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a>            <span class="n">num</span> <span class="o">=</span> <span class="s2">&quot;0&quot;</span> <span class="o">+</span> <span class="n">num</span>
+</span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">num</span><span class="si">}</span><span class="s2"> - </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">title</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a>
 </span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a>
-</span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a>
-</span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a><span class="nd">@dataclass</span>
-</span><span id="L-42"><a href="#L-42"><span class="linenos"> 42</span></a><span class="k">class</span> <span class="nc">Album</span><span class="p">:</span>
-</span><span id="L-43"><a href="#L-43"><span class="linenos"> 43</span></a>    <span class="n">url</span><span class="p">:</span> <span class="nb">str</span>
-</span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a>    <span class="n">artist</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a>    <span class="n">title</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a>    <span class="n">tracks</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Track</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a>    <span class="n">art_url</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a>
-</span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a>    <span class="k">def</span> <span class="fm">__repr__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">title</span><span class="si">}</span><span class="s2"> by </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">artist</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a>
-</span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a>    <span class="k">def</span> <span class="nf">__post_init__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a>        <span class="n">response</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">url</span><span class="p">,</span> <span class="n">headers</span><span class="o">=</span><span class="n">whosyouragent</span><span class="o">.</span><span class="n">get_agent</span><span class="p">(</span><span class="n">as_dict</span><span class="o">=</span><span class="kc">True</span><span class="p">))</span>
-</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a>        <span class="k">if</span> <span class="n">response</span><span class="o">.</span><span class="n">status_code</span> <span class="o">!=</span> <span class="mi">200</span><span class="p">:</span>
-</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a>            <span class="k">raise</span> <span class="ne">RuntimeError</span><span class="p">(</span>
-</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a>                <span class="sa">f</span><span class="s2">&quot;Getting album info failed with code </span><span class="si">{</span><span class="n">response</span><span class="o">.</span><span class="n">status_code</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a>            <span class="p">)</span>
-</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a>        <span class="n">soup</span> <span class="o">=</span> <span class="n">BeautifulSoup</span><span class="p">(</span><span class="n">response</span><span class="o">.</span><span class="n">text</span><span class="p">,</span> <span class="s2">&quot;html.parser&quot;</span><span class="p">)</span>
-</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">art_url</span> <span class="o">=</span> <span class="n">soup</span><span class="o">.</span><span class="n">find</span><span class="p">(</span><span class="s2">&quot;meta&quot;</span><span class="p">,</span> <span class="n">attrs</span><span class="o">=</span><span class="p">{</span><span class="s2">&quot;property&quot;</span><span class="p">:</span> <span class="s2">&quot;og:image&quot;</span><span class="p">})</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;content&quot;</span><span class="p">)</span>
-</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a>        <span class="k">for</span> <span class="n">script</span> <span class="ow">in</span> <span class="n">soup</span><span class="o">.</span><span class="n">find_all</span><span class="p">(</span><span class="s2">&quot;script&quot;</span><span class="p">):</span>
-</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a>            <span class="k">if</span> <span class="n">script</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;data-cart&quot;</span><span class="p">):</span>
-</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a>                <span class="n">data</span> <span class="o">=</span> <span class="n">script</span>
-</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a>                <span class="k">break</span>
-</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a>        <span class="n">data</span> <span class="o">=</span> <span class="n">json</span><span class="o">.</span><span class="n">loads</span><span class="p">(</span><span class="n">data</span><span class="o">.</span><span class="n">attrs</span><span class="p">[</span><span class="s2">&quot;data-tralbum&quot;</span><span class="p">])</span>
-</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">artist</span> <span class="o">=</span> <span class="n">clean_string</span><span class="p">(</span><span class="n">data</span><span class="p">[</span><span class="s2">&quot;artist&quot;</span><span class="p">])</span>
-</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">title</span> <span class="o">=</span> <span class="n">clean_string</span><span class="p">(</span><span class="n">data</span><span class="p">[</span><span class="s2">&quot;current&quot;</span><span class="p">][</span><span class="s2">&quot;title&quot;</span><span class="p">])</span>
-</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">tracks</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a>            <span class="n">Track</span><span class="p">(</span><span class="n">track</span><span class="p">[</span><span class="s2">&quot;title&quot;</span><span class="p">],</span> <span class="n">track</span><span class="p">[</span><span class="s2">&quot;track_num&quot;</span><span class="p">],</span> <span class="n">track</span><span class="p">[</span><span class="s2">&quot;file&quot;</span><span class="p">][</span><span class="s2">&quot;mp3-128&quot;</span><span class="p">])</span>
-</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a>            <span class="k">for</span> <span class="n">track</span> <span class="ow">in</span> <span class="n">data</span><span class="p">[</span><span class="s2">&quot;trackinfo&quot;</span><span class="p">]</span>
-</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a>            <span class="k">if</span> <span class="n">track</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;file&quot;</span><span class="p">)</span>
-</span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a>        <span class="p">]</span>
+</span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a><span class="nd">@dataclass</span>
+</span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a><span class="k">class</span> <span class="nc">Album</span><span class="p">:</span>
+</span><span id="L-42"><a href="#L-42"><span class="linenos"> 42</span></a>    <span class="n">url</span><span class="p">:</span> <span class="nb">str</span>
+</span><span id="L-43"><a href="#L-43"><span class="linenos"> 43</span></a>    <span class="n">artist</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a>    <span class="n">title</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a>    <span class="n">tracks</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Track</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a>    <span class="n">art_url</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a>
+</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a>    <span class="k">def</span> <span class="fm">__repr__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">title</span><span class="si">}</span><span class="s2"> by </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">artist</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a>
+</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a>    <span class="k">def</span> <span class="nf">__post_init__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a>        <span class="n">response</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">url</span><span class="p">,</span> <span class="n">headers</span><span class="o">=</span><span class="n">whosyouragent</span><span class="o">.</span><span class="n">get_agent</span><span class="p">(</span><span class="n">as_dict</span><span class="o">=</span><span class="kc">True</span><span class="p">))</span>
+</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a>        <span class="k">if</span> <span class="n">response</span><span class="o">.</span><span class="n">status_code</span> <span class="o">!=</span> <span class="mi">200</span><span class="p">:</span>
+</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a>            <span class="k">raise</span> <span class="ne">RuntimeError</span><span class="p">(</span>
+</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a>                <span class="sa">f</span><span class="s2">&quot;Getting album info failed with code </span><span class="si">{</span><span class="n">response</span><span class="o">.</span><span class="n">status_code</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a>            <span class="p">)</span>
+</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a>        <span class="n">soup</span> <span class="o">=</span> <span class="n">BeautifulSoup</span><span class="p">(</span><span class="n">response</span><span class="o">.</span><span class="n">text</span><span class="p">,</span> <span class="s2">&quot;html.parser&quot;</span><span class="p">)</span>
+</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">art_url</span> <span class="o">=</span> <span class="n">soup</span><span class="o">.</span><span class="n">find</span><span class="p">(</span><span class="s2">&quot;meta&quot;</span><span class="p">,</span> <span class="n">attrs</span><span class="o">=</span><span class="p">{</span><span class="s2">&quot;property&quot;</span><span class="p">:</span> <span class="s2">&quot;og:image&quot;</span><span class="p">})</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;content&quot;</span><span class="p">)</span>
+</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a>        <span class="k">for</span> <span class="n">script</span> <span class="ow">in</span> <span class="n">soup</span><span class="o">.</span><span class="n">find_all</span><span class="p">(</span><span class="s2">&quot;script&quot;</span><span class="p">):</span>
+</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a>            <span class="k">if</span> <span class="n">script</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;data-cart&quot;</span><span class="p">):</span>
+</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a>                <span class="n">data</span> <span class="o">=</span> <span class="n">script</span>
+</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a>                <span class="k">break</span>
+</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a>        <span class="n">data</span> <span class="o">=</span> <span class="n">json</span><span class="o">.</span><span class="n">loads</span><span class="p">(</span><span class="n">data</span><span class="o">.</span><span class="n">attrs</span><span class="p">[</span><span class="s2">&quot;data-tralbum&quot;</span><span class="p">])</span>
+</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">artist</span> <span class="o">=</span> <span class="n">clean_string</span><span class="p">(</span><span class="n">data</span><span class="p">[</span><span class="s2">&quot;artist&quot;</span><span class="p">])</span>
+</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">title</span> <span class="o">=</span> <span class="n">clean_string</span><span class="p">(</span><span class="n">data</span><span class="p">[</span><span class="s2">&quot;current&quot;</span><span class="p">][</span><span class="s2">&quot;title&quot;</span><span class="p">])</span>
+</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">tracks</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a>            <span class="n">Track</span><span class="p">(</span><span class="n">track</span><span class="p">[</span><span class="s2">&quot;title&quot;</span><span class="p">],</span> <span class="n">track</span><span class="p">[</span><span class="s2">&quot;track_num&quot;</span><span class="p">],</span> <span class="n">track</span><span class="p">[</span><span class="s2">&quot;file&quot;</span><span class="p">][</span><span class="s2">&quot;mp3-128&quot;</span><span class="p">])</span>
+</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a>            <span class="k">for</span> <span class="n">track</span> <span class="ow">in</span> <span class="n">data</span><span class="p">[</span><span class="s2">&quot;trackinfo&quot;</span><span class="p">]</span>
+</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a>            <span class="k">if</span> <span class="n">track</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;file&quot;</span><span class="p">)</span>
+</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a>        <span class="p">]</span>
+</span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a>
 </span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a>
-</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a>
-</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a><span class="k">class</span> <span class="nc">AlbumRipper</span><span class="p">:</span>
-</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
-</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">album_url</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">no_track_number</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span> <span class="n">overwrite</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a>    <span class="p">):</span>
-</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a>        <span class="sd">&quot;&quot;&quot;</span>
-</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a><span class="sd">        :param no_track_number: If True, don&#39;t add the track</span>
-</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a><span class="sd">        number to the front of the track title.&quot;&quot;&quot;</span>
-</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">album</span> <span class="o">=</span> <span class="n">Album</span><span class="p">(</span><span class="n">album_url</span><span class="p">)</span>
-</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">no_track_number</span> <span class="o">=</span> <span class="n">no_track_number</span>
-</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">overwrite</span> <span class="o">=</span> <span class="n">overwrite</span>
-</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a>
-</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a>    <span class="k">def</span> <span class="nf">make_save_path</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">save_path</span> <span class="o">=</span> <span class="n">Path</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span> <span class="o">/</span> <span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">artist</span> <span class="o">/</span> <span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">title</span>
-</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">save_path</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>
-</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>    <span class="nd">@property</span>
-</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>    <span class="k">def</span> <span class="nf">headers</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">dict</span><span class="p">:</span>
-</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>        <span class="sd">&quot;&quot;&quot;Get a headers dict with a random useragent.&quot;&quot;&quot;</span>
-</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a>        <span class="k">return</span> <span class="n">whosyouragent</span><span class="o">.</span><span class="n">get_agent</span><span class="p">(</span><span class="n">as_dict</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a>
-</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a>    <span class="k">def</span> <span class="nf">save_track</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">track_title</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">content</span><span class="p">:</span> <span class="nb">bytes</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Path</span><span class="p">:</span>
-</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>        <span class="sd">&quot;&quot;&quot;Save track to self.save_path/{track_title}.mp3.</span>
-</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a><span class="sd">        Returns the Path object for the save location.</span>
-</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a>
-</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a><span class="sd">        :param content: The binary data of the track.&quot;&quot;&quot;</span>
-</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a>        <span class="n">file_path</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">save_path</span> <span class="o">/</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">track_title</span><span class="si">}</span><span class="s2">.mp3&quot;</span>
-</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>        <span class="n">file_path</span><span class="o">.</span><span class="n">write_bytes</span><span class="p">(</span><span class="n">content</span><span class="p">)</span>
-</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>        <span class="k">return</span> <span class="n">file_path</span>
-</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>
-</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>    <span class="k">def</span> <span class="nf">get_track_content</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">track_url</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bytes</span><span class="p">:</span>
-</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>        <span class="sd">&quot;&quot;&quot;Make a request to track_url and return the content.</span>
-</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a><span class="sd">        Raises a RunTimeError exception if response.status_code != 200.&quot;&quot;&quot;</span>
-</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>        <span class="n">response</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="n">track_url</span><span class="p">,</span> <span class="n">headers</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">headers</span><span class="p">)</span>
-</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a>        <span class="k">if</span> <span class="n">response</span><span class="o">.</span><span class="n">status_code</span> <span class="o">!=</span> <span class="mi">200</span><span class="p">:</span>
-</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>            <span class="k">raise</span> <span class="ne">RuntimeError</span><span class="p">(</span>
-</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>                <span class="sa">f</span><span class="s2">&quot;Downloading track failed with status code </span><span class="si">{</span><span class="n">response</span><span class="o">.</span><span class="n">status_code</span><span class="si">}</span><span class="s2">.&quot;</span>
-</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>            <span class="p">)</span>
-</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>        <span class="k">return</span> <span class="n">response</span><span class="o">.</span><span class="n">content</span>
-</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>
-</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>    <span class="k">def</span> <span class="nf">download_album_art</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>        <span class="sd">&quot;&quot;&quot;Download the album art and save as a .jpg.&quot;&quot;&quot;</span>
-</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>        <span class="n">file_path</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">save_path</span> <span class="o">/</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">title</span><span class="si">}</span><span class="s2">.jpg&quot;</span>
-</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>            <span class="n">response</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">art_url</span><span class="p">,</span> <span class="n">headers</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">headers</span><span class="p">)</span>
-</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>            <span class="n">file_path</span><span class="o">.</span><span class="n">write_bytes</span><span class="p">(</span><span class="n">response</span><span class="o">.</span><span class="n">content</span><span class="p">)</span>
-</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Failed to download art for </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
-</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>
-</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>    <span class="k">def</span> <span class="nf">track_exists</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">track</span><span class="p">:</span> <span class="n">Track</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>        <span class="sd">&quot;&quot;&quot;Return if a track already exists in self.save_path.&quot;&quot;&quot;</span>
-</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">save_path</span> <span class="o">/</span> <span class="p">(</span>
-</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>            <span class="n">track</span><span class="o">.</span><span class="n">title</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">no_track_number</span> <span class="k">else</span> <span class="n">track</span><span class="o">.</span><span class="n">numbered_title</span>
-</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a>        <span class="p">)</span>
-</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>        <span class="k">return</span> <span class="n">path</span><span class="o">.</span><span class="n">with_suffix</span><span class="p">(</span><span class="s2">&quot;.mp3&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">exists</span><span class="p">()</span>
-</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a>
-</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a>    <span class="k">def</span> <span class="nf">rip</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a>        <span class="sd">&quot;&quot;&quot;Download and save the album tracks and album art.&quot;&quot;&quot;</span>
-</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;No public tracks available for </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a>            <span class="k">return</span> <span class="kc">None</span>
-</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">make_save_path</span><span class="p">()</span>
-</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">download_album_art</span><span class="p">()</span>
-</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>        <span class="n">bar</span> <span class="o">=</span> <span class="n">ProgBar</span><span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span><span class="p">)</span> <span class="o">-</span> <span class="mi">1</span><span class="p">,</span> <span class="n">width_ratio</span><span class="o">=</span><span class="mf">0.5</span><span class="p">)</span>
-</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>        <span class="n">bar</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">subsecond_resolution</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>        <span class="n">fails</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">overwrite</span><span class="p">:</span>
-</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>                <span class="n">track</span> <span class="k">for</span> <span class="n">track</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span> <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">track_exists</span><span class="p">(</span><span class="n">track</span><span class="p">)</span>
-</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>            <span class="p">]</span>
-</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a>        <span class="k">for</span> <span class="n">track</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span><span class="p">:</span>
-</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>            <span class="n">bar</span><span class="o">.</span><span class="n">display</span><span class="p">(</span>
-</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a>                <span class="n">suffix</span><span class="o">=</span><span class="sa">f</span><span class="s2">&quot;Downloading </span><span class="si">{</span><span class="n">track</span><span class="o">.</span><span class="n">title</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">,</span>
-</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a>                <span class="n">counter_override</span><span class="o">=</span><span class="mi">1</span> <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span> <span class="k">else</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>            <span class="p">)</span>
-</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>            <span class="k">try</span><span class="p">:</span>
-</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a>                <span class="n">content</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_track_content</span><span class="p">(</span><span class="n">track</span><span class="o">.</span><span class="n">url</span><span class="p">)</span>
-</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">save_track</span><span class="p">(</span>
-</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a>                    <span class="n">track</span><span class="o">.</span><span class="n">title</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">no_track_number</span> <span class="k">else</span> <span class="n">track</span><span class="o">.</span><span class="n">numbered_title</span><span class="p">,</span>
-</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a>                    <span class="n">content</span><span class="p">,</span>
-</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a>                <span class="p">)</span>
-</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a>                <span class="n">fails</span><span class="o">.</span><span class="n">append</span><span class="p">((</span><span class="n">track</span><span class="p">,</span> <span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">)))</span>
-</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Finished downloading </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="si">}</span><span class="s2"> in </span><span class="si">{</span><span class="n">bar</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">elapsed_str</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a>        <span class="k">if</span> <span class="n">fails</span><span class="p">:</span>
-</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;The following tracks failed to download:&quot;</span><span class="p">)</span>
-</span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a>            <span class="k">for</span> <span class="n">fail</span> <span class="ow">in</span> <span class="n">fails</span><span class="p">:</span>
-</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">fail</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">title</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">fail</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a>
-</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a>
-</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a><span class="k">class</span> <span class="nc">BandRipper</span><span class="p">:</span>
-</span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
-</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">band_url</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">no_track_number</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span> <span class="n">overwrite</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a>    <span class="p">):</span>
-</span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">band_url</span> <span class="o">=</span> <span class="n">band_url</span>
-</span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">albums</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a>        <span class="k">for</span> <span class="n">url</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_album_urls</span><span class="p">(</span><span class="n">band_url</span><span class="p">):</span>
-</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a>            <span class="k">try</span><span class="p">:</span>
-</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">AlbumRipper</span><span class="p">(</span><span class="n">url</span><span class="p">,</span> <span class="n">no_track_number</span><span class="p">,</span> <span class="n">overwrite</span><span class="p">))</span>
-</span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a>                <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
-</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a>
-</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a>    <span class="k">def</span> <span class="nf">get_album_urls</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">band_url</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
-</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a>        <span class="sd">&quot;&quot;&quot;Get album urls from the main bandcamp url.&quot;&quot;&quot;</span>
-</span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Fetching discography from </span><span class="si">{</span><span class="n">band_url</span><span class="si">}</span><span class="s2">...&quot;</span><span class="p">)</span>
-</span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a>        <span class="n">response</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="n">band_url</span><span class="p">,</span> <span class="n">headers</span><span class="o">=</span><span class="n">whosyouragent</span><span class="o">.</span><span class="n">get_agent</span><span class="p">(</span><span class="n">as_dict</span><span class="o">=</span><span class="kc">True</span><span class="p">))</span>
-</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a>        <span class="k">if</span> <span class="n">response</span><span class="o">.</span><span class="n">status_code</span> <span class="o">!=</span> <span class="mi">200</span><span class="p">:</span>
-</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a>            <span class="k">raise</span> <span class="ne">RuntimeError</span><span class="p">(</span>
-</span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a>                <span class="sa">f</span><span class="s2">&quot;Getting </span><span class="si">{</span><span class="n">band_url</span><span class="si">}</span><span class="s2"> failed with status code </span><span class="si">{</span><span class="n">response</span><span class="o">.</span><span class="n">status_code</span><span class="si">}</span><span class="s2">.&quot;</span>
-</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a>            <span class="p">)</span>
-</span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a>        <span class="n">soup</span> <span class="o">=</span> <span class="n">BeautifulSoup</span><span class="p">(</span><span class="n">response</span><span class="o">.</span><span class="n">text</span><span class="p">,</span> <span class="s2">&quot;html.parser&quot;</span><span class="p">)</span>
-</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a>        <span class="n">grid</span> <span class="o">=</span> <span class="n">soup</span><span class="o">.</span><span class="n">find</span><span class="p">(</span><span class="s2">&quot;ol&quot;</span><span class="p">,</span> <span class="n">attrs</span><span class="o">=</span><span class="p">{</span><span class="s2">&quot;id&quot;</span><span class="p">:</span> <span class="s2">&quot;music-grid&quot;</span><span class="p">})</span>
-</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a>        <span class="n">parsed_url</span> <span class="o">=</span> <span class="n">urlparse</span><span class="p">(</span><span class="n">band_url</span><span class="p">)</span>
-</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a>        <span class="n">base_url</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;https://</span><span class="si">{</span><span class="n">parsed_url</span><span class="o">.</span><span class="n">netloc</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a>        <span class="k">return</span> <span class="p">[</span><span class="n">base_url</span> <span class="o">+</span> <span class="n">album</span><span class="o">.</span><span class="n">a</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;href&quot;</span><span class="p">)</span> <span class="k">for</span> <span class="n">album</span> <span class="ow">in</span> <span class="n">grid</span><span class="o">.</span><span class="n">find_all</span><span class="p">(</span><span class="s2">&quot;li&quot;</span><span class="p">)]</span>
-</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a>
-</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a>    <span class="k">def</span> <span class="nf">rip</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a>        <span class="nb">print</span><span class="p">(</span>
-</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a>            <span class="sa">f</span><span class="s2">&quot;Downloading </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">)</span><span class="si">}</span><span class="s2"> albums by </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">artist</span><span class="si">}</span><span class="s2">.&quot;</span>
-</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a>        <span class="p">)</span>
-</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a>        <span class="n">timer</span> <span class="o">=</span> <span class="n">Timer</span><span class="p">(</span><span class="n">subsecond_resolution</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a>        <span class="n">timer</span><span class="o">.</span><span class="n">start</span><span class="p">()</span>
-</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a>        <span class="n">fails</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a>        <span class="k">for</span> <span class="n">album</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">:</span>
-</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a>            <span class="k">try</span><span class="p">:</span>
-</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a>                <span class="n">album</span><span class="o">.</span><span class="n">rip</span><span class="p">()</span>
-</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a>                <span class="n">fails</span><span class="o">.</span><span class="n">append</span><span class="p">((</span><span class="n">album</span><span class="p">,</span> <span class="n">e</span><span class="p">))</span>
-</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a>        <span class="n">timer</span><span class="o">.</span><span class="n">stop</span><span class="p">()</span>
-</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a>        <span class="n">artist</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">artist</span>
-</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a>        <span class="nb">print</span><span class="p">(</span>
-</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a>            <span class="sa">f</span><span class="s2">&quot;Finished downloading </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">)</span><span class="si">}</span><span class="s2"> albums by </span><span class="si">{</span><span class="n">artist</span><span class="si">}</span><span class="s2"> in </span><span class="si">{</span><span class="n">timer</span><span class="o">.</span><span class="n">elapsed_str</span><span class="si">}</span><span class="s2">.&quot;</span>
-</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a>        <span class="p">)</span>
-</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a>        <span class="k">if</span> <span class="n">fails</span><span class="p">:</span>
-</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;The following downloads failed:&quot;</span><span class="p">)</span>
-</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a>            <span class="k">for</span> <span class="n">fail</span> <span class="ow">in</span> <span class="n">fails</span><span class="p">:</span>
-</span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">fail</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">fail</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a>
-</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a>
-</span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a><span class="k">def</span> <span class="nf">page_is_discography</span><span class="p">(</span><span class="n">url</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a>    <span class="sd">&quot;&quot;&quot;Returns whether the url is to a discography page or not.&quot;&quot;&quot;</span>
-</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a>    <span class="n">response</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="n">url</span><span class="p">,</span> <span class="n">headers</span><span class="o">=</span><span class="n">whosyouragent</span><span class="o">.</span><span class="n">get_agent</span><span class="p">(</span><span class="n">as_dict</span><span class="o">=</span><span class="kc">True</span><span class="p">))</span>
-</span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a>    <span class="k">if</span> <span class="n">response</span><span class="o">.</span><span class="n">status_code</span> <span class="o">!=</span> <span class="mi">200</span><span class="p">:</span>
-</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a>        <span class="k">raise</span> <span class="ne">RuntimeError</span><span class="p">(</span>
-</span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a>            <span class="sa">f</span><span class="s2">&quot;Getting </span><span class="si">{</span><span class="n">url</span><span class="si">}</span><span class="s2"> failed with status code </span><span class="si">{</span><span class="n">response</span><span class="o">.</span><span class="n">status_code</span><span class="si">}</span><span class="s2">.&quot;</span>
-</span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a>        <span class="p">)</span>
-</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a>    <span class="n">soup</span> <span class="o">=</span> <span class="n">BeautifulSoup</span><span class="p">(</span><span class="n">response</span><span class="o">.</span><span class="n">text</span><span class="p">,</span> <span class="s2">&quot;html.parser&quot;</span><span class="p">)</span>
-</span><span id="L-221"><a href="#L-221"><span class="linenos">221</span></a>    <span class="c1"># Returns None if it doesn&#39;t exist.</span>
-</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a>    <span class="n">grid</span> <span class="o">=</span> <span class="n">soup</span><span class="o">.</span><span class="n">find</span><span class="p">(</span><span class="s2">&quot;ol&quot;</span><span class="p">,</span> <span class="n">attrs</span><span class="o">=</span><span class="p">{</span><span class="s2">&quot;id&quot;</span><span class="p">:</span> <span class="s2">&quot;music-grid&quot;</span><span class="p">})</span>
-</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a>    <span class="k">if</span> <span class="n">grid</span><span class="p">:</span>
-</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a>        <span class="k">return</span> <span class="kc">True</span>
-</span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a>    <span class="k">return</span> <span class="kc">False</span>
-</span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a>
-</span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a>
-</span><span id="L-228"><a href="#L-228"><span class="linenos">228</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
-</span><span id="L-229"><a href="#L-229"><span class="linenos">229</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
-</span><span id="L-230"><a href="#L-230"><span class="linenos">230</span></a>
-</span><span id="L-231"><a href="#L-231"><span class="linenos">231</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-232"><a href="#L-232"><span class="linenos">232</span></a>        <span class="s2">&quot;urls&quot;</span><span class="p">,</span>
-</span><span id="L-233"><a href="#L-233"><span class="linenos">233</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="L-234"><a href="#L-234"><span class="linenos">234</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
-</span><span id="L-235"><a href="#L-235"><span class="linenos">235</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The bandcamp url(s) for the album or artist.</span>
-</span><span id="L-236"><a href="#L-236"><span class="linenos">236</span></a><span class="s2">            If the url is to an artists main page,</span>
-</span><span id="L-237"><a href="#L-237"><span class="linenos">237</span></a><span class="s2">            all albums will be downloaded.</span>
-</span><span id="L-238"><a href="#L-238"><span class="linenos">238</span></a><span class="s2">            The tracks will be saved to a subdirectory of</span>
-</span><span id="L-239"><a href="#L-239"><span class="linenos">239</span></a><span class="s2">            your current directory.</span>
-</span><span id="L-240"><a href="#L-240"><span class="linenos">240</span></a><span class="s2">            If a track can&#39;t be streamed (i.e. private) it</span>
-</span><span id="L-241"><a href="#L-241"><span class="linenos">241</span></a><span class="s2">            won&#39;t be downloaded. Multiple urls can be passed.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-242"><a href="#L-242"><span class="linenos">242</span></a>    <span class="p">)</span>
-</span><span id="L-243"><a href="#L-243"><span class="linenos">243</span></a>
-</span><span id="L-244"><a href="#L-244"><span class="linenos">244</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-245"><a href="#L-245"><span class="linenos">245</span></a>        <span class="s2">&quot;-n&quot;</span><span class="p">,</span>
-</span><span id="L-246"><a href="#L-246"><span class="linenos">246</span></a>        <span class="s2">&quot;--no_track_number&quot;</span><span class="p">,</span>
-</span><span id="L-247"><a href="#L-247"><span class="linenos">247</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="L-248"><a href="#L-248"><span class="linenos">248</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; By default the track number will be added</span>
-</span><span id="L-249"><a href="#L-249"><span class="linenos">249</span></a><span class="s2">        to the front of the track title. Pass this switch</span>
-</span><span id="L-250"><a href="#L-250"><span class="linenos">250</span></a><span class="s2">        to disable the behavior.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a>    <span class="p">)</span>
-</span><span id="L-252"><a href="#L-252"><span class="linenos">252</span></a>
-</span><span id="L-253"><a href="#L-253"><span class="linenos">253</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-254"><a href="#L-254"><span class="linenos">254</span></a>        <span class="s2">&quot;-o&quot;</span><span class="p">,</span>
-</span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a>        <span class="s2">&quot;--overwrite&quot;</span><span class="p">,</span>
-</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="L-257"><a href="#L-257"><span class="linenos">257</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Pass this flag to overwrite existing files.</span>
-</span><span id="L-258"><a href="#L-258"><span class="linenos">258</span></a><span class="s2">        Otherwise don&#39;t download tracks that already exist locally.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-259"><a href="#L-259"><span class="linenos">259</span></a>    <span class="p">)</span>
-</span><span id="L-260"><a href="#L-260"><span class="linenos">260</span></a>
-</span><span id="L-261"><a href="#L-261"><span class="linenos">261</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
-</span><span id="L-262"><a href="#L-262"><span class="linenos">262</span></a>    <span class="n">args</span><span class="o">.</span><span class="n">urls</span> <span class="o">=</span> <span class="p">[</span><span class="n">url</span><span class="o">.</span><span class="n">strip</span><span class="p">(</span><span class="s2">&quot;/&quot;</span><span class="p">)</span> <span class="k">for</span> <span class="n">url</span> <span class="ow">in</span> <span class="n">args</span><span class="o">.</span><span class="n">urls</span><span class="p">]</span>
+</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a><span class="k">class</span> <span class="nc">AlbumRipper</span><span class="p">:</span>
+</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
+</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">album_url</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">no_track_number</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span> <span class="n">overwrite</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a>    <span class="p">):</span>
+</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a>        <span class="sd">&quot;&quot;&quot;</span>
+</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a><span class="sd">        :param no_track_number: If True, don&#39;t add the track</span>
+</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a><span class="sd">        number to the front of the track title.&quot;&quot;&quot;</span>
+</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">album</span> <span class="o">=</span> <span class="n">Album</span><span class="p">(</span><span class="n">album_url</span><span class="p">)</span>
+</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">no_track_number</span> <span class="o">=</span> <span class="n">no_track_number</span>
+</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">overwrite</span> <span class="o">=</span> <span class="n">overwrite</span>
+</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a>
+</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a>    <span class="k">def</span> <span class="nf">make_save_path</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">save_path</span> <span class="o">=</span> <span class="n">Path</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span> <span class="o">/</span> <span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">artist</span> <span class="o">/</span> <span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">title</span>
+</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">save_path</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>
+</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>    <span class="nd">@property</span>
+</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>    <span class="k">def</span> <span class="nf">headers</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">dict</span><span class="p">:</span>
+</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>        <span class="sd">&quot;&quot;&quot;Get a headers dict with a random useragent.&quot;&quot;&quot;</span>
+</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>        <span class="k">return</span> <span class="n">whosyouragent</span><span class="o">.</span><span class="n">get_agent</span><span class="p">(</span><span class="n">as_dict</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a>
+</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a>    <span class="k">def</span> <span class="nf">save_track</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">track_title</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">content</span><span class="p">:</span> <span class="nb">bytes</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Path</span><span class="p">:</span>
+</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a>        <span class="sd">&quot;&quot;&quot;Save track to self.save_path/{track_title}.mp3.</span>
+</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a><span class="sd">        Returns the Path object for the save location.</span>
+</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a>
+</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a><span class="sd">        :param content: The binary data of the track.&quot;&quot;&quot;</span>
+</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>        <span class="n">file_path</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">save_path</span> <span class="o">/</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">track_title</span><span class="si">}</span><span class="s2">.mp3&quot;</span>
+</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a>        <span class="n">file_path</span><span class="o">.</span><span class="n">write_bytes</span><span class="p">(</span><span class="n">content</span><span class="p">)</span>
+</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>        <span class="k">return</span> <span class="n">file_path</span>
+</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>
+</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>    <span class="k">def</span> <span class="nf">get_track_content</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">track_url</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bytes</span><span class="p">:</span>
+</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>        <span class="sd">&quot;&quot;&quot;Make a request to track_url and return the content.</span>
+</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a><span class="sd">        Raises a RunTimeError exception if response.status_code != 200.&quot;&quot;&quot;</span>
+</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>        <span class="n">response</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="n">track_url</span><span class="p">,</span> <span class="n">headers</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">headers</span><span class="p">)</span>
+</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>        <span class="k">if</span> <span class="n">response</span><span class="o">.</span><span class="n">status_code</span> <span class="o">!=</span> <span class="mi">200</span><span class="p">:</span>
+</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a>            <span class="k">raise</span> <span class="ne">RuntimeError</span><span class="p">(</span>
+</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>                <span class="sa">f</span><span class="s2">&quot;Downloading track failed with status code </span><span class="si">{</span><span class="n">response</span><span class="o">.</span><span class="n">status_code</span><span class="si">}</span><span class="s2">.&quot;</span>
+</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>            <span class="p">)</span>
+</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>        <span class="k">return</span> <span class="n">response</span><span class="o">.</span><span class="n">content</span>
+</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>
+</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>    <span class="k">def</span> <span class="nf">download_album_art</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>        <span class="sd">&quot;&quot;&quot;Download the album art and save as a .jpg.&quot;&quot;&quot;</span>
+</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>        <span class="n">file_path</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">save_path</span> <span class="o">/</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">title</span><span class="si">}</span><span class="s2">.jpg&quot;</span>
+</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>            <span class="n">response</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">art_url</span><span class="p">,</span> <span class="n">headers</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">headers</span><span class="p">)</span>
+</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>            <span class="n">file_path</span><span class="o">.</span><span class="n">write_bytes</span><span class="p">(</span><span class="n">response</span><span class="o">.</span><span class="n">content</span><span class="p">)</span>
+</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Failed to download art for </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
+</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>
+</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>    <span class="k">def</span> <span class="nf">track_exists</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">track</span><span class="p">:</span> <span class="n">Track</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>        <span class="sd">&quot;&quot;&quot;Return if a track already exists in self.save_path.&quot;&quot;&quot;</span>
+</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">save_path</span> <span class="o">/</span> <span class="p">(</span>
+</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>            <span class="n">track</span><span class="o">.</span><span class="n">title</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">no_track_number</span> <span class="k">else</span> <span class="n">track</span><span class="o">.</span><span class="n">numbered_title</span>
+</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>        <span class="p">)</span>
+</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a>        <span class="k">return</span> <span class="n">path</span><span class="o">.</span><span class="n">with_suffix</span><span class="p">(</span><span class="s2">&quot;.mp3&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">exists</span><span class="p">()</span>
+</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>
+</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a>    <span class="k">def</span> <span class="nf">rip</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a>        <span class="sd">&quot;&quot;&quot;Download and save the album tracks and album art.&quot;&quot;&quot;</span>
+</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;No public tracks available for </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a>            <span class="k">return</span> <span class="kc">None</span>
+</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">make_save_path</span><span class="p">()</span>
+</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">download_album_art</span><span class="p">()</span>
+</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>        <span class="n">bar</span> <span class="o">=</span> <span class="n">ProgBar</span><span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span><span class="p">)</span> <span class="o">-</span> <span class="mi">1</span><span class="p">,</span> <span class="n">width_ratio</span><span class="o">=</span><span class="mf">0.5</span><span class="p">)</span>
+</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>        <span class="n">fails</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">overwrite</span><span class="p">:</span>
+</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a>                <span class="n">track</span> <span class="k">for</span> <span class="n">track</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span> <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">track_exists</span><span class="p">(</span><span class="n">track</span><span class="p">)</span>
+</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>            <span class="p">]</span>
+</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>        <span class="k">for</span> <span class="n">track</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span><span class="p">:</span>
+</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>            <span class="n">bar</span><span class="o">.</span><span class="n">display</span><span class="p">(</span>
+</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a>                <span class="n">suffix</span><span class="o">=</span><span class="sa">f</span><span class="s2">&quot;Downloading </span><span class="si">{</span><span class="n">track</span><span class="o">.</span><span class="n">title</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">,</span>
+</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>                <span class="n">counter_override</span><span class="o">=</span><span class="mi">1</span> <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span> <span class="k">else</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a>            <span class="p">)</span>
+</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a>            <span class="k">try</span><span class="p">:</span>
+</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>                <span class="n">content</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_track_content</span><span class="p">(</span><span class="n">track</span><span class="o">.</span><span class="n">url</span><span class="p">)</span>
+</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">save_track</span><span class="p">(</span>
+</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a>                    <span class="n">track</span><span class="o">.</span><span class="n">title</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">no_track_number</span> <span class="k">else</span> <span class="n">track</span><span class="o">.</span><span class="n">numbered_title</span><span class="p">,</span>
+</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>                    <span class="n">content</span><span class="p">,</span>
+</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a>                <span class="p">)</span>
+</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a>                <span class="n">fails</span><span class="o">.</span><span class="n">append</span><span class="p">((</span><span class="n">track</span><span class="p">,</span> <span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">)))</span>
+</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Finished downloading </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="si">}</span><span class="s2"> in </span><span class="si">{</span><span class="n">bar</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">elapsed_str</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a>        <span class="k">if</span> <span class="n">fails</span><span class="p">:</span>
+</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;The following tracks failed to download:&quot;</span><span class="p">)</span>
+</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a>            <span class="k">for</span> <span class="n">fail</span> <span class="ow">in</span> <span class="n">fails</span><span class="p">:</span>
+</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">fail</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">title</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">fail</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a>
+</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a>
+</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a><span class="k">class</span> <span class="nc">BandRipper</span><span class="p">:</span>
+</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
+</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">band_url</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">no_track_number</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span> <span class="n">overwrite</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a>    <span class="p">):</span>
+</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">band_url</span> <span class="o">=</span> <span class="n">band_url</span>
+</span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">albums</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a>        <span class="k">for</span> <span class="n">url</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_album_urls</span><span class="p">(</span><span class="n">band_url</span><span class="p">):</span>
+</span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a>            <span class="k">try</span><span class="p">:</span>
+</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">AlbumRipper</span><span class="p">(</span><span class="n">url</span><span class="p">,</span> <span class="n">no_track_number</span><span class="p">,</span> <span class="n">overwrite</span><span class="p">))</span>
+</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a>                <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
+</span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a>
+</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a>    <span class="k">def</span> <span class="nf">get_album_urls</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">band_url</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
+</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a>        <span class="sd">&quot;&quot;&quot;Get album urls from the main bandcamp url.&quot;&quot;&quot;</span>
+</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Fetching discography from </span><span class="si">{</span><span class="n">band_url</span><span class="si">}</span><span class="s2">...&quot;</span><span class="p">)</span>
+</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a>        <span class="n">response</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="n">band_url</span><span class="p">,</span> <span class="n">headers</span><span class="o">=</span><span class="n">whosyouragent</span><span class="o">.</span><span class="n">get_agent</span><span class="p">(</span><span class="n">as_dict</span><span class="o">=</span><span class="kc">True</span><span class="p">))</span>
+</span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a>        <span class="k">if</span> <span class="n">response</span><span class="o">.</span><span class="n">status_code</span> <span class="o">!=</span> <span class="mi">200</span><span class="p">:</span>
+</span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a>            <span class="k">raise</span> <span class="ne">RuntimeError</span><span class="p">(</span>
+</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a>                <span class="sa">f</span><span class="s2">&quot;Getting </span><span class="si">{</span><span class="n">band_url</span><span class="si">}</span><span class="s2"> failed with status code </span><span class="si">{</span><span class="n">response</span><span class="o">.</span><span class="n">status_code</span><span class="si">}</span><span class="s2">.&quot;</span>
+</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a>            <span class="p">)</span>
+</span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a>        <span class="n">soup</span> <span class="o">=</span> <span class="n">BeautifulSoup</span><span class="p">(</span><span class="n">response</span><span class="o">.</span><span class="n">text</span><span class="p">,</span> <span class="s2">&quot;html.parser&quot;</span><span class="p">)</span>
+</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a>        <span class="n">grid</span> <span class="o">=</span> <span class="n">soup</span><span class="o">.</span><span class="n">find</span><span class="p">(</span><span class="s2">&quot;ol&quot;</span><span class="p">,</span> <span class="n">attrs</span><span class="o">=</span><span class="p">{</span><span class="s2">&quot;id&quot;</span><span class="p">:</span> <span class="s2">&quot;music-grid&quot;</span><span class="p">})</span>
+</span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a>        <span class="n">parsed_url</span> <span class="o">=</span> <span class="n">urlparse</span><span class="p">(</span><span class="n">band_url</span><span class="p">)</span>
+</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a>        <span class="n">base_url</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;https://</span><span class="si">{</span><span class="n">parsed_url</span><span class="o">.</span><span class="n">netloc</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a>        <span class="k">return</span> <span class="p">[</span><span class="n">base_url</span> <span class="o">+</span> <span class="n">album</span><span class="o">.</span><span class="n">a</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;href&quot;</span><span class="p">)</span> <span class="k">for</span> <span class="n">album</span> <span class="ow">in</span> <span class="n">grid</span><span class="o">.</span><span class="n">find_all</span><span class="p">(</span><span class="s2">&quot;li&quot;</span><span class="p">)]</span>
+</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a>
+</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a>    <span class="k">def</span> <span class="nf">rip</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a>        <span class="nb">print</span><span class="p">(</span>
+</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a>            <span class="sa">f</span><span class="s2">&quot;Downloading </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">)</span><span class="si">}</span><span class="s2"> albums by </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">artist</span><span class="si">}</span><span class="s2">.&quot;</span>
+</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a>        <span class="p">)</span>
+</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a>        <span class="n">timer</span> <span class="o">=</span> <span class="n">Timer</span><span class="p">(</span><span class="n">subsecond_resolution</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a>        <span class="n">timer</span><span class="o">.</span><span class="n">start</span><span class="p">()</span>
+</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a>        <span class="n">fails</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a>        <span class="k">for</span> <span class="n">album</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">:</span>
+</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a>            <span class="k">try</span><span class="p">:</span>
+</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a>                <span class="n">album</span><span class="o">.</span><span class="n">rip</span><span class="p">()</span>
+</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a>                <span class="n">fails</span><span class="o">.</span><span class="n">append</span><span class="p">((</span><span class="n">album</span><span class="p">,</span> <span class="n">e</span><span class="p">))</span>
+</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a>        <span class="n">timer</span><span class="o">.</span><span class="n">stop</span><span class="p">()</span>
+</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a>        <span class="n">artist</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">artist</span>
+</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a>        <span class="nb">print</span><span class="p">(</span>
+</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a>            <span class="sa">f</span><span class="s2">&quot;Finished downloading </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">)</span><span class="si">}</span><span class="s2"> albums by </span><span class="si">{</span><span class="n">artist</span><span class="si">}</span><span class="s2"> in </span><span class="si">{</span><span class="n">timer</span><span class="o">.</span><span class="n">elapsed_str</span><span class="si">}</span><span class="s2">.&quot;</span>
+</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a>        <span class="p">)</span>
+</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a>        <span class="k">if</span> <span class="n">fails</span><span class="p">:</span>
+</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;The following downloads failed:&quot;</span><span class="p">)</span>
+</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a>            <span class="k">for</span> <span class="n">fail</span> <span class="ow">in</span> <span class="n">fails</span><span class="p">:</span>
+</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">fail</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">fail</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a>
+</span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a>
+</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a><span class="k">def</span> <span class="nf">page_is_discography</span><span class="p">(</span><span class="n">url</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a>    <span class="sd">&quot;&quot;&quot;Returns whether the url is to a discography page or not.&quot;&quot;&quot;</span>
+</span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a>    <span class="n">response</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="n">url</span><span class="p">,</span> <span class="n">headers</span><span class="o">=</span><span class="n">whosyouragent</span><span class="o">.</span><span class="n">get_agent</span><span class="p">(</span><span class="n">as_dict</span><span class="o">=</span><span class="kc">True</span><span class="p">))</span>
+</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a>    <span class="k">if</span> <span class="n">response</span><span class="o">.</span><span class="n">status_code</span> <span class="o">!=</span> <span class="mi">200</span><span class="p">:</span>
+</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a>        <span class="k">raise</span> <span class="ne">RuntimeError</span><span class="p">(</span>
+</span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a>            <span class="sa">f</span><span class="s2">&quot;Getting </span><span class="si">{</span><span class="n">url</span><span class="si">}</span><span class="s2"> failed with status code </span><span class="si">{</span><span class="n">response</span><span class="o">.</span><span class="n">status_code</span><span class="si">}</span><span class="s2">.&quot;</span>
+</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a>        <span class="p">)</span>
+</span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a>    <span class="n">soup</span> <span class="o">=</span> <span class="n">BeautifulSoup</span><span class="p">(</span><span class="n">response</span><span class="o">.</span><span class="n">text</span><span class="p">,</span> <span class="s2">&quot;html.parser&quot;</span><span class="p">)</span>
+</span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a>    <span class="c1"># Returns None if it doesn&#39;t exist.</span>
+</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a>    <span class="n">grid</span> <span class="o">=</span> <span class="n">soup</span><span class="o">.</span><span class="n">find</span><span class="p">(</span><span class="s2">&quot;ol&quot;</span><span class="p">,</span> <span class="n">attrs</span><span class="o">=</span><span class="p">{</span><span class="s2">&quot;id&quot;</span><span class="p">:</span> <span class="s2">&quot;music-grid&quot;</span><span class="p">})</span>
+</span><span id="L-221"><a href="#L-221"><span class="linenos">221</span></a>    <span class="k">if</span> <span class="n">grid</span><span class="p">:</span>
+</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a>        <span class="k">return</span> <span class="kc">True</span>
+</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a>    <span class="k">return</span> <span class="kc">False</span>
+</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a>
+</span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a>
+</span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
+</span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
+</span><span id="L-228"><a href="#L-228"><span class="linenos">228</span></a>
+</span><span id="L-229"><a href="#L-229"><span class="linenos">229</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-230"><a href="#L-230"><span class="linenos">230</span></a>        <span class="s2">&quot;urls&quot;</span><span class="p">,</span>
+</span><span id="L-231"><a href="#L-231"><span class="linenos">231</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="L-232"><a href="#L-232"><span class="linenos">232</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
+</span><span id="L-233"><a href="#L-233"><span class="linenos">233</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The bandcamp url(s) for the album or artist.</span>
+</span><span id="L-234"><a href="#L-234"><span class="linenos">234</span></a><span class="s2">            If the url is to an artists main page,</span>
+</span><span id="L-235"><a href="#L-235"><span class="linenos">235</span></a><span class="s2">            all albums will be downloaded.</span>
+</span><span id="L-236"><a href="#L-236"><span class="linenos">236</span></a><span class="s2">            The tracks will be saved to a subdirectory of</span>
+</span><span id="L-237"><a href="#L-237"><span class="linenos">237</span></a><span class="s2">            your current directory.</span>
+</span><span id="L-238"><a href="#L-238"><span class="linenos">238</span></a><span class="s2">            If a track can&#39;t be streamed (i.e. private) it</span>
+</span><span id="L-239"><a href="#L-239"><span class="linenos">239</span></a><span class="s2">            won&#39;t be downloaded. Multiple urls can be passed.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-240"><a href="#L-240"><span class="linenos">240</span></a>    <span class="p">)</span>
+</span><span id="L-241"><a href="#L-241"><span class="linenos">241</span></a>
+</span><span id="L-242"><a href="#L-242"><span class="linenos">242</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-243"><a href="#L-243"><span class="linenos">243</span></a>        <span class="s2">&quot;-n&quot;</span><span class="p">,</span>
+</span><span id="L-244"><a href="#L-244"><span class="linenos">244</span></a>        <span class="s2">&quot;--no_track_number&quot;</span><span class="p">,</span>
+</span><span id="L-245"><a href="#L-245"><span class="linenos">245</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="L-246"><a href="#L-246"><span class="linenos">246</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; By default the track number will be added</span>
+</span><span id="L-247"><a href="#L-247"><span class="linenos">247</span></a><span class="s2">        to the front of the track title. Pass this switch</span>
+</span><span id="L-248"><a href="#L-248"><span class="linenos">248</span></a><span class="s2">        to disable the behavior.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-249"><a href="#L-249"><span class="linenos">249</span></a>    <span class="p">)</span>
+</span><span id="L-250"><a href="#L-250"><span class="linenos">250</span></a>
+</span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-252"><a href="#L-252"><span class="linenos">252</span></a>        <span class="s2">&quot;-o&quot;</span><span class="p">,</span>
+</span><span id="L-253"><a href="#L-253"><span class="linenos">253</span></a>        <span class="s2">&quot;--overwrite&quot;</span><span class="p">,</span>
+</span><span id="L-254"><a href="#L-254"><span class="linenos">254</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Pass this flag to overwrite existing files.</span>
+</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a><span class="s2">        Otherwise don&#39;t download tracks that already exist locally.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-257"><a href="#L-257"><span class="linenos">257</span></a>    <span class="p">)</span>
+</span><span id="L-258"><a href="#L-258"><span class="linenos">258</span></a>
+</span><span id="L-259"><a href="#L-259"><span class="linenos">259</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
+</span><span id="L-260"><a href="#L-260"><span class="linenos">260</span></a>    <span class="n">args</span><span class="o">.</span><span class="n">urls</span> <span class="o">=</span> <span class="p">[</span><span class="n">url</span><span class="o">.</span><span class="n">strip</span><span class="p">(</span><span class="s2">&quot;/&quot;</span><span class="p">)</span> <span class="k">for</span> <span class="n">url</span> <span class="ow">in</span> <span class="n">args</span><span class="o">.</span><span class="n">urls</span><span class="p">]</span>
+</span><span id="L-261"><a href="#L-261"><span class="linenos">261</span></a>
+</span><span id="L-262"><a href="#L-262"><span class="linenos">262</span></a>    <span class="k">return</span> <span class="n">args</span>
 </span><span id="L-263"><a href="#L-263"><span class="linenos">263</span></a>
-</span><span id="L-264"><a href="#L-264"><span class="linenos">264</span></a>    <span class="k">return</span> <span class="n">args</span>
-</span><span id="L-265"><a href="#L-265"><span class="linenos">265</span></a>
-</span><span id="L-266"><a href="#L-266"><span class="linenos">266</span></a>
-</span><span id="L-267"><a href="#L-267"><span class="linenos">267</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="L-268"><a href="#L-268"><span class="linenos">268</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
-</span><span id="L-269"><a href="#L-269"><span class="linenos">269</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
-</span><span id="L-270"><a href="#L-270"><span class="linenos">270</span></a>    <span class="k">for</span> <span class="n">url</span> <span class="ow">in</span> <span class="n">args</span><span class="o">.</span><span class="n">urls</span><span class="p">:</span>
-</span><span id="L-271"><a href="#L-271"><span class="linenos">271</span></a>        <span class="k">if</span> <span class="n">page_is_discography</span><span class="p">(</span><span class="n">url</span><span class="p">):</span>
-</span><span id="L-272"><a href="#L-272"><span class="linenos">272</span></a>            <span class="n">ripper</span> <span class="o">=</span> <span class="n">BandRipper</span><span class="p">(</span><span class="n">url</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">no_track_number</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">overwrite</span><span class="p">)</span>
-</span><span id="L-273"><a href="#L-273"><span class="linenos">273</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="L-274"><a href="#L-274"><span class="linenos">274</span></a>            <span class="n">ripper</span> <span class="o">=</span> <span class="n">AlbumRipper</span><span class="p">(</span><span class="n">url</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">no_track_number</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">overwrite</span><span class="p">)</span>
-</span><span id="L-275"><a href="#L-275"><span class="linenos">275</span></a>        <span class="n">ripper</span><span class="o">.</span><span class="n">rip</span><span class="p">()</span>
-</span><span id="L-276"><a href="#L-276"><span class="linenos">276</span></a>
-</span><span id="L-277"><a href="#L-277"><span class="linenos">277</span></a>
-</span><span id="L-278"><a href="#L-278"><span class="linenos">278</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
-</span><span id="L-279"><a href="#L-279"><span class="linenos">279</span></a>    <span class="n">main</span><span class="p">(</span><span class="n">get_args</span><span class="p">())</span>
+</span><span id="L-264"><a href="#L-264"><span class="linenos">264</span></a>
+</span><span id="L-265"><a href="#L-265"><span class="linenos">265</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="L-266"><a href="#L-266"><span class="linenos">266</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
+</span><span id="L-267"><a href="#L-267"><span class="linenos">267</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
+</span><span id="L-268"><a href="#L-268"><span class="linenos">268</span></a>    <span class="k">for</span> <span class="n">url</span> <span class="ow">in</span> <span class="n">args</span><span class="o">.</span><span class="n">urls</span><span class="p">:</span>
+</span><span id="L-269"><a href="#L-269"><span class="linenos">269</span></a>        <span class="k">if</span> <span class="n">page_is_discography</span><span class="p">(</span><span class="n">url</span><span class="p">):</span>
+</span><span id="L-270"><a href="#L-270"><span class="linenos">270</span></a>            <span class="n">ripper</span> <span class="o">=</span> <span class="n">BandRipper</span><span class="p">(</span><span class="n">url</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">no_track_number</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">overwrite</span><span class="p">)</span>
+</span><span id="L-271"><a href="#L-271"><span class="linenos">271</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="L-272"><a href="#L-272"><span class="linenos">272</span></a>            <span class="n">ripper</span> <span class="o">=</span> <span class="n">AlbumRipper</span><span class="p">(</span><span class="n">url</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">no_track_number</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">overwrite</span><span class="p">)</span>
+</span><span id="L-273"><a href="#L-273"><span class="linenos">273</span></a>        <span class="n">ripper</span><span class="o">.</span><span class="n">rip</span><span class="p">()</span>
+</span><span id="L-274"><a href="#L-274"><span class="linenos">274</span></a>
+</span><span id="L-275"><a href="#L-275"><span class="linenos">275</span></a>
+</span><span id="L-276"><a href="#L-276"><span class="linenos">276</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
+</span><span id="L-277"><a href="#L-277"><span class="linenos">277</span></a>    <span class="n">main</span><span class="p">(</span><span class="n">get_args</span><span class="p">())</span>
 </span></pre></div>
 
 
             </section>
                 <section id="clean_string">
                             <input id="clean_string-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -416,17 +414,17 @@
         <span class="def">def</span>
         <span class="name">clean_string</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">text</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="nb">str</span>:</span></span>
 
                 <label class="view-source-button" for="clean_string-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#clean_string"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="clean_string-20"><a href="#clean_string-20"><span class="linenos">20</span></a><span class="k">def</span> <span class="nf">clean_string</span><span class="p">(</span><span class="n">text</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="clean_string-21"><a href="#clean_string-21"><span class="linenos">21</span></a>    <span class="sd">&quot;&quot;&quot;Remove punctuation and trailing spaces from text.&quot;&quot;&quot;</span>
-</span><span id="clean_string-22"><a href="#clean_string-22"><span class="linenos">22</span></a>    <span class="k">return</span> <span class="n">re</span><span class="o">.</span><span class="n">sub</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;[</span><span class="si">{</span><span class="n">re</span><span class="o">.</span><span class="n">escape</span><span class="p">(</span><span class="n">string</span><span class="o">.</span><span class="n">punctuation</span><span class="p">)</span><span class="si">}</span><span class="s2">]&quot;</span><span class="p">,</span> <span class="s2">&quot;&quot;</span><span class="p">,</span> <span class="n">text</span><span class="p">)</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="clean_string-19"><a href="#clean_string-19"><span class="linenos">19</span></a><span class="k">def</span> <span class="nf">clean_string</span><span class="p">(</span><span class="n">text</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="clean_string-20"><a href="#clean_string-20"><span class="linenos">20</span></a>    <span class="sd">&quot;&quot;&quot;Remove punctuation and trailing spaces from text.&quot;&quot;&quot;</span>
+</span><span id="clean_string-21"><a href="#clean_string-21"><span class="linenos">21</span></a>    <span class="k">return</span> <span class="n">re</span><span class="o">.</span><span class="n">sub</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;[</span><span class="si">{</span><span class="n">re</span><span class="o">.</span><span class="n">escape</span><span class="p">(</span><span class="n">string</span><span class="o">.</span><span class="n">punctuation</span><span class="p">)</span><span class="si">}</span><span class="s2">]&quot;</span><span class="p">,</span> <span class="s2">&quot;&quot;</span><span class="p">,</span> <span class="n">text</span><span class="p">)</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Remove punctuation and trailing spaces from text.</p>
 </div>
 
 
@@ -439,29 +437,29 @@
     <span class="def">class</span>
     <span class="name">Track</span>:
 
                 <label class="view-source-button" for="Track-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Track"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Track-25"><a href="#Track-25"><span class="linenos">25</span></a><span class="nd">@dataclass</span>
-</span><span id="Track-26"><a href="#Track-26"><span class="linenos">26</span></a><span class="k">class</span> <span class="nc">Track</span><span class="p">:</span>
-</span><span id="Track-27"><a href="#Track-27"><span class="linenos">27</span></a>    <span class="n">title</span><span class="p">:</span> <span class="nb">str</span>
-</span><span id="Track-28"><a href="#Track-28"><span class="linenos">28</span></a>    <span class="n">number</span><span class="p">:</span> <span class="nb">int</span>
-</span><span id="Track-29"><a href="#Track-29"><span class="linenos">29</span></a>    <span class="n">url</span><span class="p">:</span> <span class="nb">str</span>
-</span><span id="Track-30"><a href="#Track-30"><span class="linenos">30</span></a>
-</span><span id="Track-31"><a href="#Track-31"><span class="linenos">31</span></a>    <span class="k">def</span> <span class="nf">__post_init__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Track-32"><a href="#Track-32"><span class="linenos">32</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">title</span> <span class="o">=</span> <span class="n">clean_string</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">title</span><span class="p">)</span>
-</span><span id="Track-33"><a href="#Track-33"><span class="linenos">33</span></a>
-</span><span id="Track-34"><a href="#Track-34"><span class="linenos">34</span></a>    <span class="nd">@property</span>
-</span><span id="Track-35"><a href="#Track-35"><span class="linenos">35</span></a>    <span class="k">def</span> <span class="nf">numbered_title</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Track-36"><a href="#Track-36"><span class="linenos">36</span></a>        <span class="n">num</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">number</span><span class="p">)</span>
-</span><span id="Track-37"><a href="#Track-37"><span class="linenos">37</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">num</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
-</span><span id="Track-38"><a href="#Track-38"><span class="linenos">38</span></a>            <span class="n">num</span> <span class="o">=</span> <span class="s2">&quot;0&quot;</span> <span class="o">+</span> <span class="n">num</span>
-</span><span id="Track-39"><a href="#Track-39"><span class="linenos">39</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">num</span><span class="si">}</span><span class="s2"> - </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">title</span><span class="si">}</span><span class="s2">&quot;</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Track-24"><a href="#Track-24"><span class="linenos">24</span></a><span class="nd">@dataclass</span>
+</span><span id="Track-25"><a href="#Track-25"><span class="linenos">25</span></a><span class="k">class</span> <span class="nc">Track</span><span class="p">:</span>
+</span><span id="Track-26"><a href="#Track-26"><span class="linenos">26</span></a>    <span class="n">title</span><span class="p">:</span> <span class="nb">str</span>
+</span><span id="Track-27"><a href="#Track-27"><span class="linenos">27</span></a>    <span class="n">number</span><span class="p">:</span> <span class="nb">int</span>
+</span><span id="Track-28"><a href="#Track-28"><span class="linenos">28</span></a>    <span class="n">url</span><span class="p">:</span> <span class="nb">str</span>
+</span><span id="Track-29"><a href="#Track-29"><span class="linenos">29</span></a>
+</span><span id="Track-30"><a href="#Track-30"><span class="linenos">30</span></a>    <span class="k">def</span> <span class="nf">__post_init__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Track-31"><a href="#Track-31"><span class="linenos">31</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">title</span> <span class="o">=</span> <span class="n">clean_string</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">title</span><span class="p">)</span>
+</span><span id="Track-32"><a href="#Track-32"><span class="linenos">32</span></a>
+</span><span id="Track-33"><a href="#Track-33"><span class="linenos">33</span></a>    <span class="nd">@property</span>
+</span><span id="Track-34"><a href="#Track-34"><span class="linenos">34</span></a>    <span class="k">def</span> <span class="nf">numbered_title</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Track-35"><a href="#Track-35"><span class="linenos">35</span></a>        <span class="n">num</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">number</span><span class="p">)</span>
+</span><span id="Track-36"><a href="#Track-36"><span class="linenos">36</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">num</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
+</span><span id="Track-37"><a href="#Track-37"><span class="linenos">37</span></a>            <span class="n">num</span> <span class="o">=</span> <span class="s2">&quot;0&quot;</span> <span class="o">+</span> <span class="n">num</span>
+</span><span id="Track-38"><a href="#Track-38"><span class="linenos">38</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">num</span><span class="si">}</span><span class="s2"> - </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">title</span><span class="si">}</span><span class="s2">&quot;</span>
 </span></pre></div>
 
 
     
 
                             <div id="Track.__init__" class="classattr">
                                 <div class="attr function">
@@ -484,45 +482,45 @@
     <span class="def">class</span>
     <span class="name">Album</span>:
 
                 <label class="view-source-button" for="Album-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Album"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Album-42"><a href="#Album-42"><span class="linenos">42</span></a><span class="nd">@dataclass</span>
-</span><span id="Album-43"><a href="#Album-43"><span class="linenos">43</span></a><span class="k">class</span> <span class="nc">Album</span><span class="p">:</span>
-</span><span id="Album-44"><a href="#Album-44"><span class="linenos">44</span></a>    <span class="n">url</span><span class="p">:</span> <span class="nb">str</span>
-</span><span id="Album-45"><a href="#Album-45"><span class="linenos">45</span></a>    <span class="n">artist</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="Album-46"><a href="#Album-46"><span class="linenos">46</span></a>    <span class="n">title</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="Album-47"><a href="#Album-47"><span class="linenos">47</span></a>    <span class="n">tracks</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Track</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="Album-48"><a href="#Album-48"><span class="linenos">48</span></a>    <span class="n">art_url</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="Album-49"><a href="#Album-49"><span class="linenos">49</span></a>
-</span><span id="Album-50"><a href="#Album-50"><span class="linenos">50</span></a>    <span class="k">def</span> <span class="fm">__repr__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Album-51"><a href="#Album-51"><span class="linenos">51</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">title</span><span class="si">}</span><span class="s2"> by </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">artist</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="Album-52"><a href="#Album-52"><span class="linenos">52</span></a>
-</span><span id="Album-53"><a href="#Album-53"><span class="linenos">53</span></a>    <span class="k">def</span> <span class="nf">__post_init__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Album-54"><a href="#Album-54"><span class="linenos">54</span></a>        <span class="n">response</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">url</span><span class="p">,</span> <span class="n">headers</span><span class="o">=</span><span class="n">whosyouragent</span><span class="o">.</span><span class="n">get_agent</span><span class="p">(</span><span class="n">as_dict</span><span class="o">=</span><span class="kc">True</span><span class="p">))</span>
-</span><span id="Album-55"><a href="#Album-55"><span class="linenos">55</span></a>        <span class="k">if</span> <span class="n">response</span><span class="o">.</span><span class="n">status_code</span> <span class="o">!=</span> <span class="mi">200</span><span class="p">:</span>
-</span><span id="Album-56"><a href="#Album-56"><span class="linenos">56</span></a>            <span class="k">raise</span> <span class="ne">RuntimeError</span><span class="p">(</span>
-</span><span id="Album-57"><a href="#Album-57"><span class="linenos">57</span></a>                <span class="sa">f</span><span class="s2">&quot;Getting album info failed with code </span><span class="si">{</span><span class="n">response</span><span class="o">.</span><span class="n">status_code</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="Album-58"><a href="#Album-58"><span class="linenos">58</span></a>            <span class="p">)</span>
-</span><span id="Album-59"><a href="#Album-59"><span class="linenos">59</span></a>        <span class="n">soup</span> <span class="o">=</span> <span class="n">BeautifulSoup</span><span class="p">(</span><span class="n">response</span><span class="o">.</span><span class="n">text</span><span class="p">,</span> <span class="s2">&quot;html.parser&quot;</span><span class="p">)</span>
-</span><span id="Album-60"><a href="#Album-60"><span class="linenos">60</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">art_url</span> <span class="o">=</span> <span class="n">soup</span><span class="o">.</span><span class="n">find</span><span class="p">(</span><span class="s2">&quot;meta&quot;</span><span class="p">,</span> <span class="n">attrs</span><span class="o">=</span><span class="p">{</span><span class="s2">&quot;property&quot;</span><span class="p">:</span> <span class="s2">&quot;og:image&quot;</span><span class="p">})</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;content&quot;</span><span class="p">)</span>
-</span><span id="Album-61"><a href="#Album-61"><span class="linenos">61</span></a>        <span class="k">for</span> <span class="n">script</span> <span class="ow">in</span> <span class="n">soup</span><span class="o">.</span><span class="n">find_all</span><span class="p">(</span><span class="s2">&quot;script&quot;</span><span class="p">):</span>
-</span><span id="Album-62"><a href="#Album-62"><span class="linenos">62</span></a>            <span class="k">if</span> <span class="n">script</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;data-cart&quot;</span><span class="p">):</span>
-</span><span id="Album-63"><a href="#Album-63"><span class="linenos">63</span></a>                <span class="n">data</span> <span class="o">=</span> <span class="n">script</span>
-</span><span id="Album-64"><a href="#Album-64"><span class="linenos">64</span></a>                <span class="k">break</span>
-</span><span id="Album-65"><a href="#Album-65"><span class="linenos">65</span></a>        <span class="n">data</span> <span class="o">=</span> <span class="n">json</span><span class="o">.</span><span class="n">loads</span><span class="p">(</span><span class="n">data</span><span class="o">.</span><span class="n">attrs</span><span class="p">[</span><span class="s2">&quot;data-tralbum&quot;</span><span class="p">])</span>
-</span><span id="Album-66"><a href="#Album-66"><span class="linenos">66</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">artist</span> <span class="o">=</span> <span class="n">clean_string</span><span class="p">(</span><span class="n">data</span><span class="p">[</span><span class="s2">&quot;artist&quot;</span><span class="p">])</span>
-</span><span id="Album-67"><a href="#Album-67"><span class="linenos">67</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">title</span> <span class="o">=</span> <span class="n">clean_string</span><span class="p">(</span><span class="n">data</span><span class="p">[</span><span class="s2">&quot;current&quot;</span><span class="p">][</span><span class="s2">&quot;title&quot;</span><span class="p">])</span>
-</span><span id="Album-68"><a href="#Album-68"><span class="linenos">68</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">tracks</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="Album-69"><a href="#Album-69"><span class="linenos">69</span></a>            <span class="n">Track</span><span class="p">(</span><span class="n">track</span><span class="p">[</span><span class="s2">&quot;title&quot;</span><span class="p">],</span> <span class="n">track</span><span class="p">[</span><span class="s2">&quot;track_num&quot;</span><span class="p">],</span> <span class="n">track</span><span class="p">[</span><span class="s2">&quot;file&quot;</span><span class="p">][</span><span class="s2">&quot;mp3-128&quot;</span><span class="p">])</span>
-</span><span id="Album-70"><a href="#Album-70"><span class="linenos">70</span></a>            <span class="k">for</span> <span class="n">track</span> <span class="ow">in</span> <span class="n">data</span><span class="p">[</span><span class="s2">&quot;trackinfo&quot;</span><span class="p">]</span>
-</span><span id="Album-71"><a href="#Album-71"><span class="linenos">71</span></a>            <span class="k">if</span> <span class="n">track</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;file&quot;</span><span class="p">)</span>
-</span><span id="Album-72"><a href="#Album-72"><span class="linenos">72</span></a>        <span class="p">]</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Album-41"><a href="#Album-41"><span class="linenos">41</span></a><span class="nd">@dataclass</span>
+</span><span id="Album-42"><a href="#Album-42"><span class="linenos">42</span></a><span class="k">class</span> <span class="nc">Album</span><span class="p">:</span>
+</span><span id="Album-43"><a href="#Album-43"><span class="linenos">43</span></a>    <span class="n">url</span><span class="p">:</span> <span class="nb">str</span>
+</span><span id="Album-44"><a href="#Album-44"><span class="linenos">44</span></a>    <span class="n">artist</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="Album-45"><a href="#Album-45"><span class="linenos">45</span></a>    <span class="n">title</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="Album-46"><a href="#Album-46"><span class="linenos">46</span></a>    <span class="n">tracks</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Track</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="Album-47"><a href="#Album-47"><span class="linenos">47</span></a>    <span class="n">art_url</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="Album-48"><a href="#Album-48"><span class="linenos">48</span></a>
+</span><span id="Album-49"><a href="#Album-49"><span class="linenos">49</span></a>    <span class="k">def</span> <span class="fm">__repr__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Album-50"><a href="#Album-50"><span class="linenos">50</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">title</span><span class="si">}</span><span class="s2"> by </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">artist</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="Album-51"><a href="#Album-51"><span class="linenos">51</span></a>
+</span><span id="Album-52"><a href="#Album-52"><span class="linenos">52</span></a>    <span class="k">def</span> <span class="nf">__post_init__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Album-53"><a href="#Album-53"><span class="linenos">53</span></a>        <span class="n">response</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">url</span><span class="p">,</span> <span class="n">headers</span><span class="o">=</span><span class="n">whosyouragent</span><span class="o">.</span><span class="n">get_agent</span><span class="p">(</span><span class="n">as_dict</span><span class="o">=</span><span class="kc">True</span><span class="p">))</span>
+</span><span id="Album-54"><a href="#Album-54"><span class="linenos">54</span></a>        <span class="k">if</span> <span class="n">response</span><span class="o">.</span><span class="n">status_code</span> <span class="o">!=</span> <span class="mi">200</span><span class="p">:</span>
+</span><span id="Album-55"><a href="#Album-55"><span class="linenos">55</span></a>            <span class="k">raise</span> <span class="ne">RuntimeError</span><span class="p">(</span>
+</span><span id="Album-56"><a href="#Album-56"><span class="linenos">56</span></a>                <span class="sa">f</span><span class="s2">&quot;Getting album info failed with code </span><span class="si">{</span><span class="n">response</span><span class="o">.</span><span class="n">status_code</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="Album-57"><a href="#Album-57"><span class="linenos">57</span></a>            <span class="p">)</span>
+</span><span id="Album-58"><a href="#Album-58"><span class="linenos">58</span></a>        <span class="n">soup</span> <span class="o">=</span> <span class="n">BeautifulSoup</span><span class="p">(</span><span class="n">response</span><span class="o">.</span><span class="n">text</span><span class="p">,</span> <span class="s2">&quot;html.parser&quot;</span><span class="p">)</span>
+</span><span id="Album-59"><a href="#Album-59"><span class="linenos">59</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">art_url</span> <span class="o">=</span> <span class="n">soup</span><span class="o">.</span><span class="n">find</span><span class="p">(</span><span class="s2">&quot;meta&quot;</span><span class="p">,</span> <span class="n">attrs</span><span class="o">=</span><span class="p">{</span><span class="s2">&quot;property&quot;</span><span class="p">:</span> <span class="s2">&quot;og:image&quot;</span><span class="p">})</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;content&quot;</span><span class="p">)</span>
+</span><span id="Album-60"><a href="#Album-60"><span class="linenos">60</span></a>        <span class="k">for</span> <span class="n">script</span> <span class="ow">in</span> <span class="n">soup</span><span class="o">.</span><span class="n">find_all</span><span class="p">(</span><span class="s2">&quot;script&quot;</span><span class="p">):</span>
+</span><span id="Album-61"><a href="#Album-61"><span class="linenos">61</span></a>            <span class="k">if</span> <span class="n">script</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;data-cart&quot;</span><span class="p">):</span>
+</span><span id="Album-62"><a href="#Album-62"><span class="linenos">62</span></a>                <span class="n">data</span> <span class="o">=</span> <span class="n">script</span>
+</span><span id="Album-63"><a href="#Album-63"><span class="linenos">63</span></a>                <span class="k">break</span>
+</span><span id="Album-64"><a href="#Album-64"><span class="linenos">64</span></a>        <span class="n">data</span> <span class="o">=</span> <span class="n">json</span><span class="o">.</span><span class="n">loads</span><span class="p">(</span><span class="n">data</span><span class="o">.</span><span class="n">attrs</span><span class="p">[</span><span class="s2">&quot;data-tralbum&quot;</span><span class="p">])</span>
+</span><span id="Album-65"><a href="#Album-65"><span class="linenos">65</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">artist</span> <span class="o">=</span> <span class="n">clean_string</span><span class="p">(</span><span class="n">data</span><span class="p">[</span><span class="s2">&quot;artist&quot;</span><span class="p">])</span>
+</span><span id="Album-66"><a href="#Album-66"><span class="linenos">66</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">title</span> <span class="o">=</span> <span class="n">clean_string</span><span class="p">(</span><span class="n">data</span><span class="p">[</span><span class="s2">&quot;current&quot;</span><span class="p">][</span><span class="s2">&quot;title&quot;</span><span class="p">])</span>
+</span><span id="Album-67"><a href="#Album-67"><span class="linenos">67</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">tracks</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="Album-68"><a href="#Album-68"><span class="linenos">68</span></a>            <span class="n">Track</span><span class="p">(</span><span class="n">track</span><span class="p">[</span><span class="s2">&quot;title&quot;</span><span class="p">],</span> <span class="n">track</span><span class="p">[</span><span class="s2">&quot;track_num&quot;</span><span class="p">],</span> <span class="n">track</span><span class="p">[</span><span class="s2">&quot;file&quot;</span><span class="p">][</span><span class="s2">&quot;mp3-128&quot;</span><span class="p">])</span>
+</span><span id="Album-69"><a href="#Album-69"><span class="linenos">69</span></a>            <span class="k">for</span> <span class="n">track</span> <span class="ow">in</span> <span class="n">data</span><span class="p">[</span><span class="s2">&quot;trackinfo&quot;</span><span class="p">]</span>
+</span><span id="Album-70"><a href="#Album-70"><span class="linenos">70</span></a>            <span class="k">if</span> <span class="n">track</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;file&quot;</span><span class="p">)</span>
+</span><span id="Album-71"><a href="#Album-71"><span class="linenos">71</span></a>        <span class="p">]</span>
 </span></pre></div>
 
 
     
 
                             <div id="Album.__init__" class="classattr">
                                 <div class="attr function">
@@ -544,102 +542,101 @@
     <span class="def">class</span>
     <span class="name">AlbumRipper</span>:
 
                 <label class="view-source-button" for="AlbumRipper-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#AlbumRipper"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="AlbumRipper-75"><a href="#AlbumRipper-75"><span class="linenos"> 75</span></a><span class="k">class</span> <span class="nc">AlbumRipper</span><span class="p">:</span>
-</span><span id="AlbumRipper-76"><a href="#AlbumRipper-76"><span class="linenos"> 76</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
-</span><span id="AlbumRipper-77"><a href="#AlbumRipper-77"><span class="linenos"> 77</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">album_url</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">no_track_number</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span> <span class="n">overwrite</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="AlbumRipper-78"><a href="#AlbumRipper-78"><span class="linenos"> 78</span></a>    <span class="p">):</span>
-</span><span id="AlbumRipper-79"><a href="#AlbumRipper-79"><span class="linenos"> 79</span></a>        <span class="sd">&quot;&quot;&quot;</span>
-</span><span id="AlbumRipper-80"><a href="#AlbumRipper-80"><span class="linenos"> 80</span></a><span class="sd">        :param no_track_number: If True, don&#39;t add the track</span>
-</span><span id="AlbumRipper-81"><a href="#AlbumRipper-81"><span class="linenos"> 81</span></a><span class="sd">        number to the front of the track title.&quot;&quot;&quot;</span>
-</span><span id="AlbumRipper-82"><a href="#AlbumRipper-82"><span class="linenos"> 82</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">album</span> <span class="o">=</span> <span class="n">Album</span><span class="p">(</span><span class="n">album_url</span><span class="p">)</span>
-</span><span id="AlbumRipper-83"><a href="#AlbumRipper-83"><span class="linenos"> 83</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">no_track_number</span> <span class="o">=</span> <span class="n">no_track_number</span>
-</span><span id="AlbumRipper-84"><a href="#AlbumRipper-84"><span class="linenos"> 84</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">overwrite</span> <span class="o">=</span> <span class="n">overwrite</span>
-</span><span id="AlbumRipper-85"><a href="#AlbumRipper-85"><span class="linenos"> 85</span></a>
-</span><span id="AlbumRipper-86"><a href="#AlbumRipper-86"><span class="linenos"> 86</span></a>    <span class="k">def</span> <span class="nf">make_save_path</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="AlbumRipper-87"><a href="#AlbumRipper-87"><span class="linenos"> 87</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">save_path</span> <span class="o">=</span> <span class="n">Path</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span> <span class="o">/</span> <span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">artist</span> <span class="o">/</span> <span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">title</span>
-</span><span id="AlbumRipper-88"><a href="#AlbumRipper-88"><span class="linenos"> 88</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">save_path</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-</span><span id="AlbumRipper-89"><a href="#AlbumRipper-89"><span class="linenos"> 89</span></a>
-</span><span id="AlbumRipper-90"><a href="#AlbumRipper-90"><span class="linenos"> 90</span></a>    <span class="nd">@property</span>
-</span><span id="AlbumRipper-91"><a href="#AlbumRipper-91"><span class="linenos"> 91</span></a>    <span class="k">def</span> <span class="nf">headers</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">dict</span><span class="p">:</span>
-</span><span id="AlbumRipper-92"><a href="#AlbumRipper-92"><span class="linenos"> 92</span></a>        <span class="sd">&quot;&quot;&quot;Get a headers dict with a random useragent.&quot;&quot;&quot;</span>
-</span><span id="AlbumRipper-93"><a href="#AlbumRipper-93"><span class="linenos"> 93</span></a>        <span class="k">return</span> <span class="n">whosyouragent</span><span class="o">.</span><span class="n">get_agent</span><span class="p">(</span><span class="n">as_dict</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-</span><span id="AlbumRipper-94"><a href="#AlbumRipper-94"><span class="linenos"> 94</span></a>
-</span><span id="AlbumRipper-95"><a href="#AlbumRipper-95"><span class="linenos"> 95</span></a>    <span class="k">def</span> <span class="nf">save_track</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">track_title</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">content</span><span class="p">:</span> <span class="nb">bytes</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Path</span><span class="p">:</span>
-</span><span id="AlbumRipper-96"><a href="#AlbumRipper-96"><span class="linenos"> 96</span></a>        <span class="sd">&quot;&quot;&quot;Save track to self.save_path/{track_title}.mp3.</span>
-</span><span id="AlbumRipper-97"><a href="#AlbumRipper-97"><span class="linenos"> 97</span></a><span class="sd">        Returns the Path object for the save location.</span>
-</span><span id="AlbumRipper-98"><a href="#AlbumRipper-98"><span class="linenos"> 98</span></a>
-</span><span id="AlbumRipper-99"><a href="#AlbumRipper-99"><span class="linenos"> 99</span></a><span class="sd">        :param content: The binary data of the track.&quot;&quot;&quot;</span>
-</span><span id="AlbumRipper-100"><a href="#AlbumRipper-100"><span class="linenos">100</span></a>        <span class="n">file_path</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">save_path</span> <span class="o">/</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">track_title</span><span class="si">}</span><span class="s2">.mp3&quot;</span>
-</span><span id="AlbumRipper-101"><a href="#AlbumRipper-101"><span class="linenos">101</span></a>        <span class="n">file_path</span><span class="o">.</span><span class="n">write_bytes</span><span class="p">(</span><span class="n">content</span><span class="p">)</span>
-</span><span id="AlbumRipper-102"><a href="#AlbumRipper-102"><span class="linenos">102</span></a>        <span class="k">return</span> <span class="n">file_path</span>
-</span><span id="AlbumRipper-103"><a href="#AlbumRipper-103"><span class="linenos">103</span></a>
-</span><span id="AlbumRipper-104"><a href="#AlbumRipper-104"><span class="linenos">104</span></a>    <span class="k">def</span> <span class="nf">get_track_content</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">track_url</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bytes</span><span class="p">:</span>
-</span><span id="AlbumRipper-105"><a href="#AlbumRipper-105"><span class="linenos">105</span></a>        <span class="sd">&quot;&quot;&quot;Make a request to track_url and return the content.</span>
-</span><span id="AlbumRipper-106"><a href="#AlbumRipper-106"><span class="linenos">106</span></a><span class="sd">        Raises a RunTimeError exception if response.status_code != 200.&quot;&quot;&quot;</span>
-</span><span id="AlbumRipper-107"><a href="#AlbumRipper-107"><span class="linenos">107</span></a>        <span class="n">response</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="n">track_url</span><span class="p">,</span> <span class="n">headers</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">headers</span><span class="p">)</span>
-</span><span id="AlbumRipper-108"><a href="#AlbumRipper-108"><span class="linenos">108</span></a>        <span class="k">if</span> <span class="n">response</span><span class="o">.</span><span class="n">status_code</span> <span class="o">!=</span> <span class="mi">200</span><span class="p">:</span>
-</span><span id="AlbumRipper-109"><a href="#AlbumRipper-109"><span class="linenos">109</span></a>            <span class="k">raise</span> <span class="ne">RuntimeError</span><span class="p">(</span>
-</span><span id="AlbumRipper-110"><a href="#AlbumRipper-110"><span class="linenos">110</span></a>                <span class="sa">f</span><span class="s2">&quot;Downloading track failed with status code </span><span class="si">{</span><span class="n">response</span><span class="o">.</span><span class="n">status_code</span><span class="si">}</span><span class="s2">.&quot;</span>
-</span><span id="AlbumRipper-111"><a href="#AlbumRipper-111"><span class="linenos">111</span></a>            <span class="p">)</span>
-</span><span id="AlbumRipper-112"><a href="#AlbumRipper-112"><span class="linenos">112</span></a>        <span class="k">return</span> <span class="n">response</span><span class="o">.</span><span class="n">content</span>
-</span><span id="AlbumRipper-113"><a href="#AlbumRipper-113"><span class="linenos">113</span></a>
-</span><span id="AlbumRipper-114"><a href="#AlbumRipper-114"><span class="linenos">114</span></a>    <span class="k">def</span> <span class="nf">download_album_art</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="AlbumRipper-115"><a href="#AlbumRipper-115"><span class="linenos">115</span></a>        <span class="sd">&quot;&quot;&quot;Download the album art and save as a .jpg.&quot;&quot;&quot;</span>
-</span><span id="AlbumRipper-116"><a href="#AlbumRipper-116"><span class="linenos">116</span></a>        <span class="n">file_path</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">save_path</span> <span class="o">/</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">title</span><span class="si">}</span><span class="s2">.jpg&quot;</span>
-</span><span id="AlbumRipper-117"><a href="#AlbumRipper-117"><span class="linenos">117</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="AlbumRipper-118"><a href="#AlbumRipper-118"><span class="linenos">118</span></a>            <span class="n">response</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">art_url</span><span class="p">,</span> <span class="n">headers</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">headers</span><span class="p">)</span>
-</span><span id="AlbumRipper-119"><a href="#AlbumRipper-119"><span class="linenos">119</span></a>            <span class="n">file_path</span><span class="o">.</span><span class="n">write_bytes</span><span class="p">(</span><span class="n">response</span><span class="o">.</span><span class="n">content</span><span class="p">)</span>
-</span><span id="AlbumRipper-120"><a href="#AlbumRipper-120"><span class="linenos">120</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="AlbumRipper-121"><a href="#AlbumRipper-121"><span class="linenos">121</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Failed to download art for </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="AlbumRipper-122"><a href="#AlbumRipper-122"><span class="linenos">122</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
-</span><span id="AlbumRipper-123"><a href="#AlbumRipper-123"><span class="linenos">123</span></a>
-</span><span id="AlbumRipper-124"><a href="#AlbumRipper-124"><span class="linenos">124</span></a>    <span class="k">def</span> <span class="nf">track_exists</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">track</span><span class="p">:</span> <span class="n">Track</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="AlbumRipper-125"><a href="#AlbumRipper-125"><span class="linenos">125</span></a>        <span class="sd">&quot;&quot;&quot;Return if a track already exists in self.save_path.&quot;&quot;&quot;</span>
-</span><span id="AlbumRipper-126"><a href="#AlbumRipper-126"><span class="linenos">126</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">save_path</span> <span class="o">/</span> <span class="p">(</span>
-</span><span id="AlbumRipper-127"><a href="#AlbumRipper-127"><span class="linenos">127</span></a>            <span class="n">track</span><span class="o">.</span><span class="n">title</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">no_track_number</span> <span class="k">else</span> <span class="n">track</span><span class="o">.</span><span class="n">numbered_title</span>
-</span><span id="AlbumRipper-128"><a href="#AlbumRipper-128"><span class="linenos">128</span></a>        <span class="p">)</span>
-</span><span id="AlbumRipper-129"><a href="#AlbumRipper-129"><span class="linenos">129</span></a>        <span class="k">return</span> <span class="n">path</span><span class="o">.</span><span class="n">with_suffix</span><span class="p">(</span><span class="s2">&quot;.mp3&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">exists</span><span class="p">()</span>
-</span><span id="AlbumRipper-130"><a href="#AlbumRipper-130"><span class="linenos">130</span></a>
-</span><span id="AlbumRipper-131"><a href="#AlbumRipper-131"><span class="linenos">131</span></a>    <span class="k">def</span> <span class="nf">rip</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="AlbumRipper-132"><a href="#AlbumRipper-132"><span class="linenos">132</span></a>        <span class="sd">&quot;&quot;&quot;Download and save the album tracks and album art.&quot;&quot;&quot;</span>
-</span><span id="AlbumRipper-133"><a href="#AlbumRipper-133"><span class="linenos">133</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="AlbumRipper-134"><a href="#AlbumRipper-134"><span class="linenos">134</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;No public tracks available for </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="AlbumRipper-135"><a href="#AlbumRipper-135"><span class="linenos">135</span></a>            <span class="k">return</span> <span class="kc">None</span>
-</span><span id="AlbumRipper-136"><a href="#AlbumRipper-136"><span class="linenos">136</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">make_save_path</span><span class="p">()</span>
-</span><span id="AlbumRipper-137"><a href="#AlbumRipper-137"><span class="linenos">137</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">download_album_art</span><span class="p">()</span>
-</span><span id="AlbumRipper-138"><a href="#AlbumRipper-138"><span class="linenos">138</span></a>        <span class="n">bar</span> <span class="o">=</span> <span class="n">ProgBar</span><span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span><span class="p">)</span> <span class="o">-</span> <span class="mi">1</span><span class="p">,</span> <span class="n">width_ratio</span><span class="o">=</span><span class="mf">0.5</span><span class="p">)</span>
-</span><span id="AlbumRipper-139"><a href="#AlbumRipper-139"><span class="linenos">139</span></a>        <span class="n">bar</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">subsecond_resolution</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="AlbumRipper-140"><a href="#AlbumRipper-140"><span class="linenos">140</span></a>        <span class="n">fails</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="AlbumRipper-141"><a href="#AlbumRipper-141"><span class="linenos">141</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">overwrite</span><span class="p">:</span>
-</span><span id="AlbumRipper-142"><a href="#AlbumRipper-142"><span class="linenos">142</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="AlbumRipper-143"><a href="#AlbumRipper-143"><span class="linenos">143</span></a>                <span class="n">track</span> <span class="k">for</span> <span class="n">track</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span> <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">track_exists</span><span class="p">(</span><span class="n">track</span><span class="p">)</span>
-</span><span id="AlbumRipper-144"><a href="#AlbumRipper-144"><span class="linenos">144</span></a>            <span class="p">]</span>
-</span><span id="AlbumRipper-145"><a href="#AlbumRipper-145"><span class="linenos">145</span></a>        <span class="k">for</span> <span class="n">track</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span><span class="p">:</span>
-</span><span id="AlbumRipper-146"><a href="#AlbumRipper-146"><span class="linenos">146</span></a>            <span class="n">bar</span><span class="o">.</span><span class="n">display</span><span class="p">(</span>
-</span><span id="AlbumRipper-147"><a href="#AlbumRipper-147"><span class="linenos">147</span></a>                <span class="n">suffix</span><span class="o">=</span><span class="sa">f</span><span class="s2">&quot;Downloading </span><span class="si">{</span><span class="n">track</span><span class="o">.</span><span class="n">title</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">,</span>
-</span><span id="AlbumRipper-148"><a href="#AlbumRipper-148"><span class="linenos">148</span></a>                <span class="n">counter_override</span><span class="o">=</span><span class="mi">1</span> <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span> <span class="k">else</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="AlbumRipper-149"><a href="#AlbumRipper-149"><span class="linenos">149</span></a>            <span class="p">)</span>
-</span><span id="AlbumRipper-150"><a href="#AlbumRipper-150"><span class="linenos">150</span></a>            <span class="k">try</span><span class="p">:</span>
-</span><span id="AlbumRipper-151"><a href="#AlbumRipper-151"><span class="linenos">151</span></a>                <span class="n">content</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_track_content</span><span class="p">(</span><span class="n">track</span><span class="o">.</span><span class="n">url</span><span class="p">)</span>
-</span><span id="AlbumRipper-152"><a href="#AlbumRipper-152"><span class="linenos">152</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">save_track</span><span class="p">(</span>
-</span><span id="AlbumRipper-153"><a href="#AlbumRipper-153"><span class="linenos">153</span></a>                    <span class="n">track</span><span class="o">.</span><span class="n">title</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">no_track_number</span> <span class="k">else</span> <span class="n">track</span><span class="o">.</span><span class="n">numbered_title</span><span class="p">,</span>
-</span><span id="AlbumRipper-154"><a href="#AlbumRipper-154"><span class="linenos">154</span></a>                    <span class="n">content</span><span class="p">,</span>
-</span><span id="AlbumRipper-155"><a href="#AlbumRipper-155"><span class="linenos">155</span></a>                <span class="p">)</span>
-</span><span id="AlbumRipper-156"><a href="#AlbumRipper-156"><span class="linenos">156</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="AlbumRipper-157"><a href="#AlbumRipper-157"><span class="linenos">157</span></a>                <span class="n">fails</span><span class="o">.</span><span class="n">append</span><span class="p">((</span><span class="n">track</span><span class="p">,</span> <span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">)))</span>
-</span><span id="AlbumRipper-158"><a href="#AlbumRipper-158"><span class="linenos">158</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Finished downloading </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="si">}</span><span class="s2"> in </span><span class="si">{</span><span class="n">bar</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">elapsed_str</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="AlbumRipper-159"><a href="#AlbumRipper-159"><span class="linenos">159</span></a>        <span class="k">if</span> <span class="n">fails</span><span class="p">:</span>
-</span><span id="AlbumRipper-160"><a href="#AlbumRipper-160"><span class="linenos">160</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;The following tracks failed to download:&quot;</span><span class="p">)</span>
-</span><span id="AlbumRipper-161"><a href="#AlbumRipper-161"><span class="linenos">161</span></a>            <span class="k">for</span> <span class="n">fail</span> <span class="ow">in</span> <span class="n">fails</span><span class="p">:</span>
-</span><span id="AlbumRipper-162"><a href="#AlbumRipper-162"><span class="linenos">162</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">fail</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">title</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">fail</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="AlbumRipper-74"><a href="#AlbumRipper-74"><span class="linenos"> 74</span></a><span class="k">class</span> <span class="nc">AlbumRipper</span><span class="p">:</span>
+</span><span id="AlbumRipper-75"><a href="#AlbumRipper-75"><span class="linenos"> 75</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
+</span><span id="AlbumRipper-76"><a href="#AlbumRipper-76"><span class="linenos"> 76</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">album_url</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">no_track_number</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span> <span class="n">overwrite</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="AlbumRipper-77"><a href="#AlbumRipper-77"><span class="linenos"> 77</span></a>    <span class="p">):</span>
+</span><span id="AlbumRipper-78"><a href="#AlbumRipper-78"><span class="linenos"> 78</span></a>        <span class="sd">&quot;&quot;&quot;</span>
+</span><span id="AlbumRipper-79"><a href="#AlbumRipper-79"><span class="linenos"> 79</span></a><span class="sd">        :param no_track_number: If True, don&#39;t add the track</span>
+</span><span id="AlbumRipper-80"><a href="#AlbumRipper-80"><span class="linenos"> 80</span></a><span class="sd">        number to the front of the track title.&quot;&quot;&quot;</span>
+</span><span id="AlbumRipper-81"><a href="#AlbumRipper-81"><span class="linenos"> 81</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">album</span> <span class="o">=</span> <span class="n">Album</span><span class="p">(</span><span class="n">album_url</span><span class="p">)</span>
+</span><span id="AlbumRipper-82"><a href="#AlbumRipper-82"><span class="linenos"> 82</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">no_track_number</span> <span class="o">=</span> <span class="n">no_track_number</span>
+</span><span id="AlbumRipper-83"><a href="#AlbumRipper-83"><span class="linenos"> 83</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">overwrite</span> <span class="o">=</span> <span class="n">overwrite</span>
+</span><span id="AlbumRipper-84"><a href="#AlbumRipper-84"><span class="linenos"> 84</span></a>
+</span><span id="AlbumRipper-85"><a href="#AlbumRipper-85"><span class="linenos"> 85</span></a>    <span class="k">def</span> <span class="nf">make_save_path</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="AlbumRipper-86"><a href="#AlbumRipper-86"><span class="linenos"> 86</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">save_path</span> <span class="o">=</span> <span class="n">Path</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span> <span class="o">/</span> <span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">artist</span> <span class="o">/</span> <span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">title</span>
+</span><span id="AlbumRipper-87"><a href="#AlbumRipper-87"><span class="linenos"> 87</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">save_path</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+</span><span id="AlbumRipper-88"><a href="#AlbumRipper-88"><span class="linenos"> 88</span></a>
+</span><span id="AlbumRipper-89"><a href="#AlbumRipper-89"><span class="linenos"> 89</span></a>    <span class="nd">@property</span>
+</span><span id="AlbumRipper-90"><a href="#AlbumRipper-90"><span class="linenos"> 90</span></a>    <span class="k">def</span> <span class="nf">headers</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">dict</span><span class="p">:</span>
+</span><span id="AlbumRipper-91"><a href="#AlbumRipper-91"><span class="linenos"> 91</span></a>        <span class="sd">&quot;&quot;&quot;Get a headers dict with a random useragent.&quot;&quot;&quot;</span>
+</span><span id="AlbumRipper-92"><a href="#AlbumRipper-92"><span class="linenos"> 92</span></a>        <span class="k">return</span> <span class="n">whosyouragent</span><span class="o">.</span><span class="n">get_agent</span><span class="p">(</span><span class="n">as_dict</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+</span><span id="AlbumRipper-93"><a href="#AlbumRipper-93"><span class="linenos"> 93</span></a>
+</span><span id="AlbumRipper-94"><a href="#AlbumRipper-94"><span class="linenos"> 94</span></a>    <span class="k">def</span> <span class="nf">save_track</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">track_title</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">content</span><span class="p">:</span> <span class="nb">bytes</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Path</span><span class="p">:</span>
+</span><span id="AlbumRipper-95"><a href="#AlbumRipper-95"><span class="linenos"> 95</span></a>        <span class="sd">&quot;&quot;&quot;Save track to self.save_path/{track_title}.mp3.</span>
+</span><span id="AlbumRipper-96"><a href="#AlbumRipper-96"><span class="linenos"> 96</span></a><span class="sd">        Returns the Path object for the save location.</span>
+</span><span id="AlbumRipper-97"><a href="#AlbumRipper-97"><span class="linenos"> 97</span></a>
+</span><span id="AlbumRipper-98"><a href="#AlbumRipper-98"><span class="linenos"> 98</span></a><span class="sd">        :param content: The binary data of the track.&quot;&quot;&quot;</span>
+</span><span id="AlbumRipper-99"><a href="#AlbumRipper-99"><span class="linenos"> 99</span></a>        <span class="n">file_path</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">save_path</span> <span class="o">/</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">track_title</span><span class="si">}</span><span class="s2">.mp3&quot;</span>
+</span><span id="AlbumRipper-100"><a href="#AlbumRipper-100"><span class="linenos">100</span></a>        <span class="n">file_path</span><span class="o">.</span><span class="n">write_bytes</span><span class="p">(</span><span class="n">content</span><span class="p">)</span>
+</span><span id="AlbumRipper-101"><a href="#AlbumRipper-101"><span class="linenos">101</span></a>        <span class="k">return</span> <span class="n">file_path</span>
+</span><span id="AlbumRipper-102"><a href="#AlbumRipper-102"><span class="linenos">102</span></a>
+</span><span id="AlbumRipper-103"><a href="#AlbumRipper-103"><span class="linenos">103</span></a>    <span class="k">def</span> <span class="nf">get_track_content</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">track_url</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bytes</span><span class="p">:</span>
+</span><span id="AlbumRipper-104"><a href="#AlbumRipper-104"><span class="linenos">104</span></a>        <span class="sd">&quot;&quot;&quot;Make a request to track_url and return the content.</span>
+</span><span id="AlbumRipper-105"><a href="#AlbumRipper-105"><span class="linenos">105</span></a><span class="sd">        Raises a RunTimeError exception if response.status_code != 200.&quot;&quot;&quot;</span>
+</span><span id="AlbumRipper-106"><a href="#AlbumRipper-106"><span class="linenos">106</span></a>        <span class="n">response</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="n">track_url</span><span class="p">,</span> <span class="n">headers</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">headers</span><span class="p">)</span>
+</span><span id="AlbumRipper-107"><a href="#AlbumRipper-107"><span class="linenos">107</span></a>        <span class="k">if</span> <span class="n">response</span><span class="o">.</span><span class="n">status_code</span> <span class="o">!=</span> <span class="mi">200</span><span class="p">:</span>
+</span><span id="AlbumRipper-108"><a href="#AlbumRipper-108"><span class="linenos">108</span></a>            <span class="k">raise</span> <span class="ne">RuntimeError</span><span class="p">(</span>
+</span><span id="AlbumRipper-109"><a href="#AlbumRipper-109"><span class="linenos">109</span></a>                <span class="sa">f</span><span class="s2">&quot;Downloading track failed with status code </span><span class="si">{</span><span class="n">response</span><span class="o">.</span><span class="n">status_code</span><span class="si">}</span><span class="s2">.&quot;</span>
+</span><span id="AlbumRipper-110"><a href="#AlbumRipper-110"><span class="linenos">110</span></a>            <span class="p">)</span>
+</span><span id="AlbumRipper-111"><a href="#AlbumRipper-111"><span class="linenos">111</span></a>        <span class="k">return</span> <span class="n">response</span><span class="o">.</span><span class="n">content</span>
+</span><span id="AlbumRipper-112"><a href="#AlbumRipper-112"><span class="linenos">112</span></a>
+</span><span id="AlbumRipper-113"><a href="#AlbumRipper-113"><span class="linenos">113</span></a>    <span class="k">def</span> <span class="nf">download_album_art</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="AlbumRipper-114"><a href="#AlbumRipper-114"><span class="linenos">114</span></a>        <span class="sd">&quot;&quot;&quot;Download the album art and save as a .jpg.&quot;&quot;&quot;</span>
+</span><span id="AlbumRipper-115"><a href="#AlbumRipper-115"><span class="linenos">115</span></a>        <span class="n">file_path</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">save_path</span> <span class="o">/</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">title</span><span class="si">}</span><span class="s2">.jpg&quot;</span>
+</span><span id="AlbumRipper-116"><a href="#AlbumRipper-116"><span class="linenos">116</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="AlbumRipper-117"><a href="#AlbumRipper-117"><span class="linenos">117</span></a>            <span class="n">response</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">art_url</span><span class="p">,</span> <span class="n">headers</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">headers</span><span class="p">)</span>
+</span><span id="AlbumRipper-118"><a href="#AlbumRipper-118"><span class="linenos">118</span></a>            <span class="n">file_path</span><span class="o">.</span><span class="n">write_bytes</span><span class="p">(</span><span class="n">response</span><span class="o">.</span><span class="n">content</span><span class="p">)</span>
+</span><span id="AlbumRipper-119"><a href="#AlbumRipper-119"><span class="linenos">119</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="AlbumRipper-120"><a href="#AlbumRipper-120"><span class="linenos">120</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Failed to download art for </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="AlbumRipper-121"><a href="#AlbumRipper-121"><span class="linenos">121</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
+</span><span id="AlbumRipper-122"><a href="#AlbumRipper-122"><span class="linenos">122</span></a>
+</span><span id="AlbumRipper-123"><a href="#AlbumRipper-123"><span class="linenos">123</span></a>    <span class="k">def</span> <span class="nf">track_exists</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">track</span><span class="p">:</span> <span class="n">Track</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="AlbumRipper-124"><a href="#AlbumRipper-124"><span class="linenos">124</span></a>        <span class="sd">&quot;&quot;&quot;Return if a track already exists in self.save_path.&quot;&quot;&quot;</span>
+</span><span id="AlbumRipper-125"><a href="#AlbumRipper-125"><span class="linenos">125</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">save_path</span> <span class="o">/</span> <span class="p">(</span>
+</span><span id="AlbumRipper-126"><a href="#AlbumRipper-126"><span class="linenos">126</span></a>            <span class="n">track</span><span class="o">.</span><span class="n">title</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">no_track_number</span> <span class="k">else</span> <span class="n">track</span><span class="o">.</span><span class="n">numbered_title</span>
+</span><span id="AlbumRipper-127"><a href="#AlbumRipper-127"><span class="linenos">127</span></a>        <span class="p">)</span>
+</span><span id="AlbumRipper-128"><a href="#AlbumRipper-128"><span class="linenos">128</span></a>        <span class="k">return</span> <span class="n">path</span><span class="o">.</span><span class="n">with_suffix</span><span class="p">(</span><span class="s2">&quot;.mp3&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">exists</span><span class="p">()</span>
+</span><span id="AlbumRipper-129"><a href="#AlbumRipper-129"><span class="linenos">129</span></a>
+</span><span id="AlbumRipper-130"><a href="#AlbumRipper-130"><span class="linenos">130</span></a>    <span class="k">def</span> <span class="nf">rip</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="AlbumRipper-131"><a href="#AlbumRipper-131"><span class="linenos">131</span></a>        <span class="sd">&quot;&quot;&quot;Download and save the album tracks and album art.&quot;&quot;&quot;</span>
+</span><span id="AlbumRipper-132"><a href="#AlbumRipper-132"><span class="linenos">132</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="AlbumRipper-133"><a href="#AlbumRipper-133"><span class="linenos">133</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;No public tracks available for </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="AlbumRipper-134"><a href="#AlbumRipper-134"><span class="linenos">134</span></a>            <span class="k">return</span> <span class="kc">None</span>
+</span><span id="AlbumRipper-135"><a href="#AlbumRipper-135"><span class="linenos">135</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">make_save_path</span><span class="p">()</span>
+</span><span id="AlbumRipper-136"><a href="#AlbumRipper-136"><span class="linenos">136</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">download_album_art</span><span class="p">()</span>
+</span><span id="AlbumRipper-137"><a href="#AlbumRipper-137"><span class="linenos">137</span></a>        <span class="n">bar</span> <span class="o">=</span> <span class="n">ProgBar</span><span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span><span class="p">)</span> <span class="o">-</span> <span class="mi">1</span><span class="p">,</span> <span class="n">width_ratio</span><span class="o">=</span><span class="mf">0.5</span><span class="p">)</span>
+</span><span id="AlbumRipper-138"><a href="#AlbumRipper-138"><span class="linenos">138</span></a>        <span class="n">fails</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="AlbumRipper-139"><a href="#AlbumRipper-139"><span class="linenos">139</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">overwrite</span><span class="p">:</span>
+</span><span id="AlbumRipper-140"><a href="#AlbumRipper-140"><span class="linenos">140</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="AlbumRipper-141"><a href="#AlbumRipper-141"><span class="linenos">141</span></a>                <span class="n">track</span> <span class="k">for</span> <span class="n">track</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span> <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">track_exists</span><span class="p">(</span><span class="n">track</span><span class="p">)</span>
+</span><span id="AlbumRipper-142"><a href="#AlbumRipper-142"><span class="linenos">142</span></a>            <span class="p">]</span>
+</span><span id="AlbumRipper-143"><a href="#AlbumRipper-143"><span class="linenos">143</span></a>        <span class="k">for</span> <span class="n">track</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span><span class="p">:</span>
+</span><span id="AlbumRipper-144"><a href="#AlbumRipper-144"><span class="linenos">144</span></a>            <span class="n">bar</span><span class="o">.</span><span class="n">display</span><span class="p">(</span>
+</span><span id="AlbumRipper-145"><a href="#AlbumRipper-145"><span class="linenos">145</span></a>                <span class="n">suffix</span><span class="o">=</span><span class="sa">f</span><span class="s2">&quot;Downloading </span><span class="si">{</span><span class="n">track</span><span class="o">.</span><span class="n">title</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">,</span>
+</span><span id="AlbumRipper-146"><a href="#AlbumRipper-146"><span class="linenos">146</span></a>                <span class="n">counter_override</span><span class="o">=</span><span class="mi">1</span> <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span> <span class="k">else</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="AlbumRipper-147"><a href="#AlbumRipper-147"><span class="linenos">147</span></a>            <span class="p">)</span>
+</span><span id="AlbumRipper-148"><a href="#AlbumRipper-148"><span class="linenos">148</span></a>            <span class="k">try</span><span class="p">:</span>
+</span><span id="AlbumRipper-149"><a href="#AlbumRipper-149"><span class="linenos">149</span></a>                <span class="n">content</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_track_content</span><span class="p">(</span><span class="n">track</span><span class="o">.</span><span class="n">url</span><span class="p">)</span>
+</span><span id="AlbumRipper-150"><a href="#AlbumRipper-150"><span class="linenos">150</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">save_track</span><span class="p">(</span>
+</span><span id="AlbumRipper-151"><a href="#AlbumRipper-151"><span class="linenos">151</span></a>                    <span class="n">track</span><span class="o">.</span><span class="n">title</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">no_track_number</span> <span class="k">else</span> <span class="n">track</span><span class="o">.</span><span class="n">numbered_title</span><span class="p">,</span>
+</span><span id="AlbumRipper-152"><a href="#AlbumRipper-152"><span class="linenos">152</span></a>                    <span class="n">content</span><span class="p">,</span>
+</span><span id="AlbumRipper-153"><a href="#AlbumRipper-153"><span class="linenos">153</span></a>                <span class="p">)</span>
+</span><span id="AlbumRipper-154"><a href="#AlbumRipper-154"><span class="linenos">154</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="AlbumRipper-155"><a href="#AlbumRipper-155"><span class="linenos">155</span></a>                <span class="n">fails</span><span class="o">.</span><span class="n">append</span><span class="p">((</span><span class="n">track</span><span class="p">,</span> <span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">)))</span>
+</span><span id="AlbumRipper-156"><a href="#AlbumRipper-156"><span class="linenos">156</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Finished downloading </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="si">}</span><span class="s2"> in </span><span class="si">{</span><span class="n">bar</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">elapsed_str</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="AlbumRipper-157"><a href="#AlbumRipper-157"><span class="linenos">157</span></a>        <span class="k">if</span> <span class="n">fails</span><span class="p">:</span>
+</span><span id="AlbumRipper-158"><a href="#AlbumRipper-158"><span class="linenos">158</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;The following tracks failed to download:&quot;</span><span class="p">)</span>
+</span><span id="AlbumRipper-159"><a href="#AlbumRipper-159"><span class="linenos">159</span></a>            <span class="k">for</span> <span class="n">fail</span> <span class="ow">in</span> <span class="n">fails</span><span class="p">:</span>
+</span><span id="AlbumRipper-160"><a href="#AlbumRipper-160"><span class="linenos">160</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">fail</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">title</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">fail</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             <div id="AlbumRipper.__init__" class="classattr">
                                         <input id="AlbumRipper.__init__-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
@@ -647,23 +644,23 @@
             
         <span class="name">AlbumRipper</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="n">album_url</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">no_track_number</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>,</span><span class="param">	<span class="n">overwrite</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span></span>)</span>
 
                 <label class="view-source-button" for="AlbumRipper.__init__-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#AlbumRipper.__init__"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="AlbumRipper.__init__-76"><a href="#AlbumRipper.__init__-76"><span class="linenos">76</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
-</span><span id="AlbumRipper.__init__-77"><a href="#AlbumRipper.__init__-77"><span class="linenos">77</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">album_url</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">no_track_number</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span> <span class="n">overwrite</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="AlbumRipper.__init__-78"><a href="#AlbumRipper.__init__-78"><span class="linenos">78</span></a>    <span class="p">):</span>
-</span><span id="AlbumRipper.__init__-79"><a href="#AlbumRipper.__init__-79"><span class="linenos">79</span></a>        <span class="sd">&quot;&quot;&quot;</span>
-</span><span id="AlbumRipper.__init__-80"><a href="#AlbumRipper.__init__-80"><span class="linenos">80</span></a><span class="sd">        :param no_track_number: If True, don&#39;t add the track</span>
-</span><span id="AlbumRipper.__init__-81"><a href="#AlbumRipper.__init__-81"><span class="linenos">81</span></a><span class="sd">        number to the front of the track title.&quot;&quot;&quot;</span>
-</span><span id="AlbumRipper.__init__-82"><a href="#AlbumRipper.__init__-82"><span class="linenos">82</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">album</span> <span class="o">=</span> <span class="n">Album</span><span class="p">(</span><span class="n">album_url</span><span class="p">)</span>
-</span><span id="AlbumRipper.__init__-83"><a href="#AlbumRipper.__init__-83"><span class="linenos">83</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">no_track_number</span> <span class="o">=</span> <span class="n">no_track_number</span>
-</span><span id="AlbumRipper.__init__-84"><a href="#AlbumRipper.__init__-84"><span class="linenos">84</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">overwrite</span> <span class="o">=</span> <span class="n">overwrite</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="AlbumRipper.__init__-75"><a href="#AlbumRipper.__init__-75"><span class="linenos">75</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
+</span><span id="AlbumRipper.__init__-76"><a href="#AlbumRipper.__init__-76"><span class="linenos">76</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">album_url</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">no_track_number</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span> <span class="n">overwrite</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="AlbumRipper.__init__-77"><a href="#AlbumRipper.__init__-77"><span class="linenos">77</span></a>    <span class="p">):</span>
+</span><span id="AlbumRipper.__init__-78"><a href="#AlbumRipper.__init__-78"><span class="linenos">78</span></a>        <span class="sd">&quot;&quot;&quot;</span>
+</span><span id="AlbumRipper.__init__-79"><a href="#AlbumRipper.__init__-79"><span class="linenos">79</span></a><span class="sd">        :param no_track_number: If True, don&#39;t add the track</span>
+</span><span id="AlbumRipper.__init__-80"><a href="#AlbumRipper.__init__-80"><span class="linenos">80</span></a><span class="sd">        number to the front of the track title.&quot;&quot;&quot;</span>
+</span><span id="AlbumRipper.__init__-81"><a href="#AlbumRipper.__init__-81"><span class="linenos">81</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">album</span> <span class="o">=</span> <span class="n">Album</span><span class="p">(</span><span class="n">album_url</span><span class="p">)</span>
+</span><span id="AlbumRipper.__init__-82"><a href="#AlbumRipper.__init__-82"><span class="linenos">82</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">no_track_number</span> <span class="o">=</span> <span class="n">no_track_number</span>
+</span><span id="AlbumRipper.__init__-83"><a href="#AlbumRipper.__init__-83"><span class="linenos">83</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">overwrite</span> <span class="o">=</span> <span class="n">overwrite</span>
 </span></pre></div>
 
 
             <div class="docstring"><h6 id="parameters">Parameters</h6>
 
 <ul>
 <li><strong>no_track_number</strong>:  If True, don't add the track
@@ -680,17 +677,17 @@
         <span class="def">def</span>
         <span class="name">make_save_path</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="AlbumRipper.make_save_path-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#AlbumRipper.make_save_path"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="AlbumRipper.make_save_path-86"><a href="#AlbumRipper.make_save_path-86"><span class="linenos">86</span></a>    <span class="k">def</span> <span class="nf">make_save_path</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="AlbumRipper.make_save_path-87"><a href="#AlbumRipper.make_save_path-87"><span class="linenos">87</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">save_path</span> <span class="o">=</span> <span class="n">Path</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span> <span class="o">/</span> <span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">artist</span> <span class="o">/</span> <span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">title</span>
-</span><span id="AlbumRipper.make_save_path-88"><a href="#AlbumRipper.make_save_path-88"><span class="linenos">88</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">save_path</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="AlbumRipper.make_save_path-85"><a href="#AlbumRipper.make_save_path-85"><span class="linenos">85</span></a>    <span class="k">def</span> <span class="nf">make_save_path</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="AlbumRipper.make_save_path-86"><a href="#AlbumRipper.make_save_path-86"><span class="linenos">86</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">save_path</span> <span class="o">=</span> <span class="n">Path</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span> <span class="o">/</span> <span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">artist</span> <span class="o">/</span> <span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">title</span>
+</span><span id="AlbumRipper.make_save_path-87"><a href="#AlbumRipper.make_save_path-87"><span class="linenos">87</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">save_path</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             </div>
                             <div id="AlbumRipper.headers" class="classattr">
@@ -713,22 +710,22 @@
         <span class="def">def</span>
         <span class="name">save_track</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">track_title</span><span class="p">:</span> <span class="nb">str</span>, </span><span class="param"><span class="n">content</span><span class="p">:</span> <span class="nb">bytes</span></span><span class="return-annotation">) -> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span>:</span></span>
 
                 <label class="view-source-button" for="AlbumRipper.save_track-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#AlbumRipper.save_track"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="AlbumRipper.save_track-95"><a href="#AlbumRipper.save_track-95"><span class="linenos"> 95</span></a>    <span class="k">def</span> <span class="nf">save_track</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">track_title</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">content</span><span class="p">:</span> <span class="nb">bytes</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Path</span><span class="p">:</span>
-</span><span id="AlbumRipper.save_track-96"><a href="#AlbumRipper.save_track-96"><span class="linenos"> 96</span></a>        <span class="sd">&quot;&quot;&quot;Save track to self.save_path/{track_title}.mp3.</span>
-</span><span id="AlbumRipper.save_track-97"><a href="#AlbumRipper.save_track-97"><span class="linenos"> 97</span></a><span class="sd">        Returns the Path object for the save location.</span>
-</span><span id="AlbumRipper.save_track-98"><a href="#AlbumRipper.save_track-98"><span class="linenos"> 98</span></a>
-</span><span id="AlbumRipper.save_track-99"><a href="#AlbumRipper.save_track-99"><span class="linenos"> 99</span></a><span class="sd">        :param content: The binary data of the track.&quot;&quot;&quot;</span>
-</span><span id="AlbumRipper.save_track-100"><a href="#AlbumRipper.save_track-100"><span class="linenos">100</span></a>        <span class="n">file_path</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">save_path</span> <span class="o">/</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">track_title</span><span class="si">}</span><span class="s2">.mp3&quot;</span>
-</span><span id="AlbumRipper.save_track-101"><a href="#AlbumRipper.save_track-101"><span class="linenos">101</span></a>        <span class="n">file_path</span><span class="o">.</span><span class="n">write_bytes</span><span class="p">(</span><span class="n">content</span><span class="p">)</span>
-</span><span id="AlbumRipper.save_track-102"><a href="#AlbumRipper.save_track-102"><span class="linenos">102</span></a>        <span class="k">return</span> <span class="n">file_path</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="AlbumRipper.save_track-94"><a href="#AlbumRipper.save_track-94"><span class="linenos"> 94</span></a>    <span class="k">def</span> <span class="nf">save_track</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">track_title</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">content</span><span class="p">:</span> <span class="nb">bytes</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Path</span><span class="p">:</span>
+</span><span id="AlbumRipper.save_track-95"><a href="#AlbumRipper.save_track-95"><span class="linenos"> 95</span></a>        <span class="sd">&quot;&quot;&quot;Save track to self.save_path/{track_title}.mp3.</span>
+</span><span id="AlbumRipper.save_track-96"><a href="#AlbumRipper.save_track-96"><span class="linenos"> 96</span></a><span class="sd">        Returns the Path object for the save location.</span>
+</span><span id="AlbumRipper.save_track-97"><a href="#AlbumRipper.save_track-97"><span class="linenos"> 97</span></a>
+</span><span id="AlbumRipper.save_track-98"><a href="#AlbumRipper.save_track-98"><span class="linenos"> 98</span></a><span class="sd">        :param content: The binary data of the track.&quot;&quot;&quot;</span>
+</span><span id="AlbumRipper.save_track-99"><a href="#AlbumRipper.save_track-99"><span class="linenos"> 99</span></a>        <span class="n">file_path</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">save_path</span> <span class="o">/</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">track_title</span><span class="si">}</span><span class="s2">.mp3&quot;</span>
+</span><span id="AlbumRipper.save_track-100"><a href="#AlbumRipper.save_track-100"><span class="linenos">100</span></a>        <span class="n">file_path</span><span class="o">.</span><span class="n">write_bytes</span><span class="p">(</span><span class="n">content</span><span class="p">)</span>
+</span><span id="AlbumRipper.save_track-101"><a href="#AlbumRipper.save_track-101"><span class="linenos">101</span></a>        <span class="k">return</span> <span class="n">file_path</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Save track to self.save_path/{track_title}.mp3.
 Returns the Path object for the save location.</p>
 
 <h6 id="parameters">Parameters</h6>
@@ -747,23 +744,23 @@
         <span class="def">def</span>
         <span class="name">get_track_content</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">track_url</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="nb">bytes</span>:</span></span>
 
                 <label class="view-source-button" for="AlbumRipper.get_track_content-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#AlbumRipper.get_track_content"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="AlbumRipper.get_track_content-104"><a href="#AlbumRipper.get_track_content-104"><span class="linenos">104</span></a>    <span class="k">def</span> <span class="nf">get_track_content</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">track_url</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bytes</span><span class="p">:</span>
-</span><span id="AlbumRipper.get_track_content-105"><a href="#AlbumRipper.get_track_content-105"><span class="linenos">105</span></a>        <span class="sd">&quot;&quot;&quot;Make a request to track_url and return the content.</span>
-</span><span id="AlbumRipper.get_track_content-106"><a href="#AlbumRipper.get_track_content-106"><span class="linenos">106</span></a><span class="sd">        Raises a RunTimeError exception if response.status_code != 200.&quot;&quot;&quot;</span>
-</span><span id="AlbumRipper.get_track_content-107"><a href="#AlbumRipper.get_track_content-107"><span class="linenos">107</span></a>        <span class="n">response</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="n">track_url</span><span class="p">,</span> <span class="n">headers</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">headers</span><span class="p">)</span>
-</span><span id="AlbumRipper.get_track_content-108"><a href="#AlbumRipper.get_track_content-108"><span class="linenos">108</span></a>        <span class="k">if</span> <span class="n">response</span><span class="o">.</span><span class="n">status_code</span> <span class="o">!=</span> <span class="mi">200</span><span class="p">:</span>
-</span><span id="AlbumRipper.get_track_content-109"><a href="#AlbumRipper.get_track_content-109"><span class="linenos">109</span></a>            <span class="k">raise</span> <span class="ne">RuntimeError</span><span class="p">(</span>
-</span><span id="AlbumRipper.get_track_content-110"><a href="#AlbumRipper.get_track_content-110"><span class="linenos">110</span></a>                <span class="sa">f</span><span class="s2">&quot;Downloading track failed with status code </span><span class="si">{</span><span class="n">response</span><span class="o">.</span><span class="n">status_code</span><span class="si">}</span><span class="s2">.&quot;</span>
-</span><span id="AlbumRipper.get_track_content-111"><a href="#AlbumRipper.get_track_content-111"><span class="linenos">111</span></a>            <span class="p">)</span>
-</span><span id="AlbumRipper.get_track_content-112"><a href="#AlbumRipper.get_track_content-112"><span class="linenos">112</span></a>        <span class="k">return</span> <span class="n">response</span><span class="o">.</span><span class="n">content</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="AlbumRipper.get_track_content-103"><a href="#AlbumRipper.get_track_content-103"><span class="linenos">103</span></a>    <span class="k">def</span> <span class="nf">get_track_content</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">track_url</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bytes</span><span class="p">:</span>
+</span><span id="AlbumRipper.get_track_content-104"><a href="#AlbumRipper.get_track_content-104"><span class="linenos">104</span></a>        <span class="sd">&quot;&quot;&quot;Make a request to track_url and return the content.</span>
+</span><span id="AlbumRipper.get_track_content-105"><a href="#AlbumRipper.get_track_content-105"><span class="linenos">105</span></a><span class="sd">        Raises a RunTimeError exception if response.status_code != 200.&quot;&quot;&quot;</span>
+</span><span id="AlbumRipper.get_track_content-106"><a href="#AlbumRipper.get_track_content-106"><span class="linenos">106</span></a>        <span class="n">response</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="n">track_url</span><span class="p">,</span> <span class="n">headers</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">headers</span><span class="p">)</span>
+</span><span id="AlbumRipper.get_track_content-107"><a href="#AlbumRipper.get_track_content-107"><span class="linenos">107</span></a>        <span class="k">if</span> <span class="n">response</span><span class="o">.</span><span class="n">status_code</span> <span class="o">!=</span> <span class="mi">200</span><span class="p">:</span>
+</span><span id="AlbumRipper.get_track_content-108"><a href="#AlbumRipper.get_track_content-108"><span class="linenos">108</span></a>            <span class="k">raise</span> <span class="ne">RuntimeError</span><span class="p">(</span>
+</span><span id="AlbumRipper.get_track_content-109"><a href="#AlbumRipper.get_track_content-109"><span class="linenos">109</span></a>                <span class="sa">f</span><span class="s2">&quot;Downloading track failed with status code </span><span class="si">{</span><span class="n">response</span><span class="o">.</span><span class="n">status_code</span><span class="si">}</span><span class="s2">.&quot;</span>
+</span><span id="AlbumRipper.get_track_content-110"><a href="#AlbumRipper.get_track_content-110"><span class="linenos">110</span></a>            <span class="p">)</span>
+</span><span id="AlbumRipper.get_track_content-111"><a href="#AlbumRipper.get_track_content-111"><span class="linenos">111</span></a>        <span class="k">return</span> <span class="n">response</span><span class="o">.</span><span class="n">content</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Make a request to track_url and return the content.
 Raises a RunTimeError exception if response.status_code != 200.</p>
 </div>
 
@@ -776,23 +773,23 @@
         <span class="def">def</span>
         <span class="name">download_album_art</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="AlbumRipper.download_album_art-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#AlbumRipper.download_album_art"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="AlbumRipper.download_album_art-114"><a href="#AlbumRipper.download_album_art-114"><span class="linenos">114</span></a>    <span class="k">def</span> <span class="nf">download_album_art</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="AlbumRipper.download_album_art-115"><a href="#AlbumRipper.download_album_art-115"><span class="linenos">115</span></a>        <span class="sd">&quot;&quot;&quot;Download the album art and save as a .jpg.&quot;&quot;&quot;</span>
-</span><span id="AlbumRipper.download_album_art-116"><a href="#AlbumRipper.download_album_art-116"><span class="linenos">116</span></a>        <span class="n">file_path</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">save_path</span> <span class="o">/</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">title</span><span class="si">}</span><span class="s2">.jpg&quot;</span>
-</span><span id="AlbumRipper.download_album_art-117"><a href="#AlbumRipper.download_album_art-117"><span class="linenos">117</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="AlbumRipper.download_album_art-118"><a href="#AlbumRipper.download_album_art-118"><span class="linenos">118</span></a>            <span class="n">response</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">art_url</span><span class="p">,</span> <span class="n">headers</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">headers</span><span class="p">)</span>
-</span><span id="AlbumRipper.download_album_art-119"><a href="#AlbumRipper.download_album_art-119"><span class="linenos">119</span></a>            <span class="n">file_path</span><span class="o">.</span><span class="n">write_bytes</span><span class="p">(</span><span class="n">response</span><span class="o">.</span><span class="n">content</span><span class="p">)</span>
-</span><span id="AlbumRipper.download_album_art-120"><a href="#AlbumRipper.download_album_art-120"><span class="linenos">120</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="AlbumRipper.download_album_art-121"><a href="#AlbumRipper.download_album_art-121"><span class="linenos">121</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Failed to download art for </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="AlbumRipper.download_album_art-122"><a href="#AlbumRipper.download_album_art-122"><span class="linenos">122</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="AlbumRipper.download_album_art-113"><a href="#AlbumRipper.download_album_art-113"><span class="linenos">113</span></a>    <span class="k">def</span> <span class="nf">download_album_art</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="AlbumRipper.download_album_art-114"><a href="#AlbumRipper.download_album_art-114"><span class="linenos">114</span></a>        <span class="sd">&quot;&quot;&quot;Download the album art and save as a .jpg.&quot;&quot;&quot;</span>
+</span><span id="AlbumRipper.download_album_art-115"><a href="#AlbumRipper.download_album_art-115"><span class="linenos">115</span></a>        <span class="n">file_path</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">save_path</span> <span class="o">/</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">title</span><span class="si">}</span><span class="s2">.jpg&quot;</span>
+</span><span id="AlbumRipper.download_album_art-116"><a href="#AlbumRipper.download_album_art-116"><span class="linenos">116</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="AlbumRipper.download_album_art-117"><a href="#AlbumRipper.download_album_art-117"><span class="linenos">117</span></a>            <span class="n">response</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">art_url</span><span class="p">,</span> <span class="n">headers</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">headers</span><span class="p">)</span>
+</span><span id="AlbumRipper.download_album_art-118"><a href="#AlbumRipper.download_album_art-118"><span class="linenos">118</span></a>            <span class="n">file_path</span><span class="o">.</span><span class="n">write_bytes</span><span class="p">(</span><span class="n">response</span><span class="o">.</span><span class="n">content</span><span class="p">)</span>
+</span><span id="AlbumRipper.download_album_art-119"><a href="#AlbumRipper.download_album_art-119"><span class="linenos">119</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="AlbumRipper.download_album_art-120"><a href="#AlbumRipper.download_album_art-120"><span class="linenos">120</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Failed to download art for </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="AlbumRipper.download_album_art-121"><a href="#AlbumRipper.download_album_art-121"><span class="linenos">121</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Download the album art and save as a .jpg.</p>
 </div>
 
 
@@ -804,20 +801,20 @@
         <span class="def">def</span>
         <span class="name">track_exists</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">track</span><span class="p">:</span> <span class="n"><a href="#Track">bandripper.bandripper.Track</a></span></span><span class="return-annotation">) -> <span class="nb">bool</span>:</span></span>
 
                 <label class="view-source-button" for="AlbumRipper.track_exists-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#AlbumRipper.track_exists"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="AlbumRipper.track_exists-124"><a href="#AlbumRipper.track_exists-124"><span class="linenos">124</span></a>    <span class="k">def</span> <span class="nf">track_exists</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">track</span><span class="p">:</span> <span class="n">Track</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="AlbumRipper.track_exists-125"><a href="#AlbumRipper.track_exists-125"><span class="linenos">125</span></a>        <span class="sd">&quot;&quot;&quot;Return if a track already exists in self.save_path.&quot;&quot;&quot;</span>
-</span><span id="AlbumRipper.track_exists-126"><a href="#AlbumRipper.track_exists-126"><span class="linenos">126</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">save_path</span> <span class="o">/</span> <span class="p">(</span>
-</span><span id="AlbumRipper.track_exists-127"><a href="#AlbumRipper.track_exists-127"><span class="linenos">127</span></a>            <span class="n">track</span><span class="o">.</span><span class="n">title</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">no_track_number</span> <span class="k">else</span> <span class="n">track</span><span class="o">.</span><span class="n">numbered_title</span>
-</span><span id="AlbumRipper.track_exists-128"><a href="#AlbumRipper.track_exists-128"><span class="linenos">128</span></a>        <span class="p">)</span>
-</span><span id="AlbumRipper.track_exists-129"><a href="#AlbumRipper.track_exists-129"><span class="linenos">129</span></a>        <span class="k">return</span> <span class="n">path</span><span class="o">.</span><span class="n">with_suffix</span><span class="p">(</span><span class="s2">&quot;.mp3&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">exists</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="AlbumRipper.track_exists-123"><a href="#AlbumRipper.track_exists-123"><span class="linenos">123</span></a>    <span class="k">def</span> <span class="nf">track_exists</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">track</span><span class="p">:</span> <span class="n">Track</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="AlbumRipper.track_exists-124"><a href="#AlbumRipper.track_exists-124"><span class="linenos">124</span></a>        <span class="sd">&quot;&quot;&quot;Return if a track already exists in self.save_path.&quot;&quot;&quot;</span>
+</span><span id="AlbumRipper.track_exists-125"><a href="#AlbumRipper.track_exists-125"><span class="linenos">125</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">save_path</span> <span class="o">/</span> <span class="p">(</span>
+</span><span id="AlbumRipper.track_exists-126"><a href="#AlbumRipper.track_exists-126"><span class="linenos">126</span></a>            <span class="n">track</span><span class="o">.</span><span class="n">title</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">no_track_number</span> <span class="k">else</span> <span class="n">track</span><span class="o">.</span><span class="n">numbered_title</span>
+</span><span id="AlbumRipper.track_exists-127"><a href="#AlbumRipper.track_exists-127"><span class="linenos">127</span></a>        <span class="p">)</span>
+</span><span id="AlbumRipper.track_exists-128"><a href="#AlbumRipper.track_exists-128"><span class="linenos">128</span></a>        <span class="k">return</span> <span class="n">path</span><span class="o">.</span><span class="n">with_suffix</span><span class="p">(</span><span class="s2">&quot;.mp3&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">exists</span><span class="p">()</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Return if a track already exists in self.save_path.</p>
 </div>
 
 
@@ -829,46 +826,45 @@
         <span class="def">def</span>
         <span class="name">rip</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="AlbumRipper.rip-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#AlbumRipper.rip"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="AlbumRipper.rip-131"><a href="#AlbumRipper.rip-131"><span class="linenos">131</span></a>    <span class="k">def</span> <span class="nf">rip</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="AlbumRipper.rip-132"><a href="#AlbumRipper.rip-132"><span class="linenos">132</span></a>        <span class="sd">&quot;&quot;&quot;Download and save the album tracks and album art.&quot;&quot;&quot;</span>
-</span><span id="AlbumRipper.rip-133"><a href="#AlbumRipper.rip-133"><span class="linenos">133</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="AlbumRipper.rip-134"><a href="#AlbumRipper.rip-134"><span class="linenos">134</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;No public tracks available for </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="AlbumRipper.rip-135"><a href="#AlbumRipper.rip-135"><span class="linenos">135</span></a>            <span class="k">return</span> <span class="kc">None</span>
-</span><span id="AlbumRipper.rip-136"><a href="#AlbumRipper.rip-136"><span class="linenos">136</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">make_save_path</span><span class="p">()</span>
-</span><span id="AlbumRipper.rip-137"><a href="#AlbumRipper.rip-137"><span class="linenos">137</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">download_album_art</span><span class="p">()</span>
-</span><span id="AlbumRipper.rip-138"><a href="#AlbumRipper.rip-138"><span class="linenos">138</span></a>        <span class="n">bar</span> <span class="o">=</span> <span class="n">ProgBar</span><span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span><span class="p">)</span> <span class="o">-</span> <span class="mi">1</span><span class="p">,</span> <span class="n">width_ratio</span><span class="o">=</span><span class="mf">0.5</span><span class="p">)</span>
-</span><span id="AlbumRipper.rip-139"><a href="#AlbumRipper.rip-139"><span class="linenos">139</span></a>        <span class="n">bar</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">subsecond_resolution</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="AlbumRipper.rip-140"><a href="#AlbumRipper.rip-140"><span class="linenos">140</span></a>        <span class="n">fails</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="AlbumRipper.rip-141"><a href="#AlbumRipper.rip-141"><span class="linenos">141</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">overwrite</span><span class="p">:</span>
-</span><span id="AlbumRipper.rip-142"><a href="#AlbumRipper.rip-142"><span class="linenos">142</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="AlbumRipper.rip-143"><a href="#AlbumRipper.rip-143"><span class="linenos">143</span></a>                <span class="n">track</span> <span class="k">for</span> <span class="n">track</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span> <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">track_exists</span><span class="p">(</span><span class="n">track</span><span class="p">)</span>
-</span><span id="AlbumRipper.rip-144"><a href="#AlbumRipper.rip-144"><span class="linenos">144</span></a>            <span class="p">]</span>
-</span><span id="AlbumRipper.rip-145"><a href="#AlbumRipper.rip-145"><span class="linenos">145</span></a>        <span class="k">for</span> <span class="n">track</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span><span class="p">:</span>
-</span><span id="AlbumRipper.rip-146"><a href="#AlbumRipper.rip-146"><span class="linenos">146</span></a>            <span class="n">bar</span><span class="o">.</span><span class="n">display</span><span class="p">(</span>
-</span><span id="AlbumRipper.rip-147"><a href="#AlbumRipper.rip-147"><span class="linenos">147</span></a>                <span class="n">suffix</span><span class="o">=</span><span class="sa">f</span><span class="s2">&quot;Downloading </span><span class="si">{</span><span class="n">track</span><span class="o">.</span><span class="n">title</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">,</span>
-</span><span id="AlbumRipper.rip-148"><a href="#AlbumRipper.rip-148"><span class="linenos">148</span></a>                <span class="n">counter_override</span><span class="o">=</span><span class="mi">1</span> <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span> <span class="k">else</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="AlbumRipper.rip-149"><a href="#AlbumRipper.rip-149"><span class="linenos">149</span></a>            <span class="p">)</span>
-</span><span id="AlbumRipper.rip-150"><a href="#AlbumRipper.rip-150"><span class="linenos">150</span></a>            <span class="k">try</span><span class="p">:</span>
-</span><span id="AlbumRipper.rip-151"><a href="#AlbumRipper.rip-151"><span class="linenos">151</span></a>                <span class="n">content</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_track_content</span><span class="p">(</span><span class="n">track</span><span class="o">.</span><span class="n">url</span><span class="p">)</span>
-</span><span id="AlbumRipper.rip-152"><a href="#AlbumRipper.rip-152"><span class="linenos">152</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">save_track</span><span class="p">(</span>
-</span><span id="AlbumRipper.rip-153"><a href="#AlbumRipper.rip-153"><span class="linenos">153</span></a>                    <span class="n">track</span><span class="o">.</span><span class="n">title</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">no_track_number</span> <span class="k">else</span> <span class="n">track</span><span class="o">.</span><span class="n">numbered_title</span><span class="p">,</span>
-</span><span id="AlbumRipper.rip-154"><a href="#AlbumRipper.rip-154"><span class="linenos">154</span></a>                    <span class="n">content</span><span class="p">,</span>
-</span><span id="AlbumRipper.rip-155"><a href="#AlbumRipper.rip-155"><span class="linenos">155</span></a>                <span class="p">)</span>
-</span><span id="AlbumRipper.rip-156"><a href="#AlbumRipper.rip-156"><span class="linenos">156</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="AlbumRipper.rip-157"><a href="#AlbumRipper.rip-157"><span class="linenos">157</span></a>                <span class="n">fails</span><span class="o">.</span><span class="n">append</span><span class="p">((</span><span class="n">track</span><span class="p">,</span> <span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">)))</span>
-</span><span id="AlbumRipper.rip-158"><a href="#AlbumRipper.rip-158"><span class="linenos">158</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Finished downloading </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="si">}</span><span class="s2"> in </span><span class="si">{</span><span class="n">bar</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">elapsed_str</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="AlbumRipper.rip-159"><a href="#AlbumRipper.rip-159"><span class="linenos">159</span></a>        <span class="k">if</span> <span class="n">fails</span><span class="p">:</span>
-</span><span id="AlbumRipper.rip-160"><a href="#AlbumRipper.rip-160"><span class="linenos">160</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;The following tracks failed to download:&quot;</span><span class="p">)</span>
-</span><span id="AlbumRipper.rip-161"><a href="#AlbumRipper.rip-161"><span class="linenos">161</span></a>            <span class="k">for</span> <span class="n">fail</span> <span class="ow">in</span> <span class="n">fails</span><span class="p">:</span>
-</span><span id="AlbumRipper.rip-162"><a href="#AlbumRipper.rip-162"><span class="linenos">162</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">fail</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">title</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">fail</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="AlbumRipper.rip-130"><a href="#AlbumRipper.rip-130"><span class="linenos">130</span></a>    <span class="k">def</span> <span class="nf">rip</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="AlbumRipper.rip-131"><a href="#AlbumRipper.rip-131"><span class="linenos">131</span></a>        <span class="sd">&quot;&quot;&quot;Download and save the album tracks and album art.&quot;&quot;&quot;</span>
+</span><span id="AlbumRipper.rip-132"><a href="#AlbumRipper.rip-132"><span class="linenos">132</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="AlbumRipper.rip-133"><a href="#AlbumRipper.rip-133"><span class="linenos">133</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;No public tracks available for </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="AlbumRipper.rip-134"><a href="#AlbumRipper.rip-134"><span class="linenos">134</span></a>            <span class="k">return</span> <span class="kc">None</span>
+</span><span id="AlbumRipper.rip-135"><a href="#AlbumRipper.rip-135"><span class="linenos">135</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">make_save_path</span><span class="p">()</span>
+</span><span id="AlbumRipper.rip-136"><a href="#AlbumRipper.rip-136"><span class="linenos">136</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">download_album_art</span><span class="p">()</span>
+</span><span id="AlbumRipper.rip-137"><a href="#AlbumRipper.rip-137"><span class="linenos">137</span></a>        <span class="n">bar</span> <span class="o">=</span> <span class="n">ProgBar</span><span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span><span class="p">)</span> <span class="o">-</span> <span class="mi">1</span><span class="p">,</span> <span class="n">width_ratio</span><span class="o">=</span><span class="mf">0.5</span><span class="p">)</span>
+</span><span id="AlbumRipper.rip-138"><a href="#AlbumRipper.rip-138"><span class="linenos">138</span></a>        <span class="n">fails</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="AlbumRipper.rip-139"><a href="#AlbumRipper.rip-139"><span class="linenos">139</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">overwrite</span><span class="p">:</span>
+</span><span id="AlbumRipper.rip-140"><a href="#AlbumRipper.rip-140"><span class="linenos">140</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="AlbumRipper.rip-141"><a href="#AlbumRipper.rip-141"><span class="linenos">141</span></a>                <span class="n">track</span> <span class="k">for</span> <span class="n">track</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span> <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">track_exists</span><span class="p">(</span><span class="n">track</span><span class="p">)</span>
+</span><span id="AlbumRipper.rip-142"><a href="#AlbumRipper.rip-142"><span class="linenos">142</span></a>            <span class="p">]</span>
+</span><span id="AlbumRipper.rip-143"><a href="#AlbumRipper.rip-143"><span class="linenos">143</span></a>        <span class="k">for</span> <span class="n">track</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span><span class="p">:</span>
+</span><span id="AlbumRipper.rip-144"><a href="#AlbumRipper.rip-144"><span class="linenos">144</span></a>            <span class="n">bar</span><span class="o">.</span><span class="n">display</span><span class="p">(</span>
+</span><span id="AlbumRipper.rip-145"><a href="#AlbumRipper.rip-145"><span class="linenos">145</span></a>                <span class="n">suffix</span><span class="o">=</span><span class="sa">f</span><span class="s2">&quot;Downloading </span><span class="si">{</span><span class="n">track</span><span class="o">.</span><span class="n">title</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">,</span>
+</span><span id="AlbumRipper.rip-146"><a href="#AlbumRipper.rip-146"><span class="linenos">146</span></a>                <span class="n">counter_override</span><span class="o">=</span><span class="mi">1</span> <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">tracks</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span> <span class="k">else</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="AlbumRipper.rip-147"><a href="#AlbumRipper.rip-147"><span class="linenos">147</span></a>            <span class="p">)</span>
+</span><span id="AlbumRipper.rip-148"><a href="#AlbumRipper.rip-148"><span class="linenos">148</span></a>            <span class="k">try</span><span class="p">:</span>
+</span><span id="AlbumRipper.rip-149"><a href="#AlbumRipper.rip-149"><span class="linenos">149</span></a>                <span class="n">content</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_track_content</span><span class="p">(</span><span class="n">track</span><span class="o">.</span><span class="n">url</span><span class="p">)</span>
+</span><span id="AlbumRipper.rip-150"><a href="#AlbumRipper.rip-150"><span class="linenos">150</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">save_track</span><span class="p">(</span>
+</span><span id="AlbumRipper.rip-151"><a href="#AlbumRipper.rip-151"><span class="linenos">151</span></a>                    <span class="n">track</span><span class="o">.</span><span class="n">title</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">no_track_number</span> <span class="k">else</span> <span class="n">track</span><span class="o">.</span><span class="n">numbered_title</span><span class="p">,</span>
+</span><span id="AlbumRipper.rip-152"><a href="#AlbumRipper.rip-152"><span class="linenos">152</span></a>                    <span class="n">content</span><span class="p">,</span>
+</span><span id="AlbumRipper.rip-153"><a href="#AlbumRipper.rip-153"><span class="linenos">153</span></a>                <span class="p">)</span>
+</span><span id="AlbumRipper.rip-154"><a href="#AlbumRipper.rip-154"><span class="linenos">154</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="AlbumRipper.rip-155"><a href="#AlbumRipper.rip-155"><span class="linenos">155</span></a>                <span class="n">fails</span><span class="o">.</span><span class="n">append</span><span class="p">((</span><span class="n">track</span><span class="p">,</span> <span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">)))</span>
+</span><span id="AlbumRipper.rip-156"><a href="#AlbumRipper.rip-156"><span class="linenos">156</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Finished downloading </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="si">}</span><span class="s2"> in </span><span class="si">{</span><span class="n">bar</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">elapsed_str</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="AlbumRipper.rip-157"><a href="#AlbumRipper.rip-157"><span class="linenos">157</span></a>        <span class="k">if</span> <span class="n">fails</span><span class="p">:</span>
+</span><span id="AlbumRipper.rip-158"><a href="#AlbumRipper.rip-158"><span class="linenos">158</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;The following tracks failed to download:&quot;</span><span class="p">)</span>
+</span><span id="AlbumRipper.rip-159"><a href="#AlbumRipper.rip-159"><span class="linenos">159</span></a>            <span class="k">for</span> <span class="n">fail</span> <span class="ow">in</span> <span class="n">fails</span><span class="p">:</span>
+</span><span id="AlbumRipper.rip-160"><a href="#AlbumRipper.rip-160"><span class="linenos">160</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">fail</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">title</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">fail</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Download and save the album tracks and album art.</p>
 </div>
 
 
@@ -881,61 +877,61 @@
     <span class="def">class</span>
     <span class="name">BandRipper</span>:
 
                 <label class="view-source-button" for="BandRipper-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#BandRipper"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="BandRipper-165"><a href="#BandRipper-165"><span class="linenos">165</span></a><span class="k">class</span> <span class="nc">BandRipper</span><span class="p">:</span>
-</span><span id="BandRipper-166"><a href="#BandRipper-166"><span class="linenos">166</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
-</span><span id="BandRipper-167"><a href="#BandRipper-167"><span class="linenos">167</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">band_url</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">no_track_number</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span> <span class="n">overwrite</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="BandRipper-168"><a href="#BandRipper-168"><span class="linenos">168</span></a>    <span class="p">):</span>
-</span><span id="BandRipper-169"><a href="#BandRipper-169"><span class="linenos">169</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">band_url</span> <span class="o">=</span> <span class="n">band_url</span>
-</span><span id="BandRipper-170"><a href="#BandRipper-170"><span class="linenos">170</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">albums</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="BandRipper-171"><a href="#BandRipper-171"><span class="linenos">171</span></a>        <span class="k">for</span> <span class="n">url</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_album_urls</span><span class="p">(</span><span class="n">band_url</span><span class="p">):</span>
-</span><span id="BandRipper-172"><a href="#BandRipper-172"><span class="linenos">172</span></a>            <span class="k">try</span><span class="p">:</span>
-</span><span id="BandRipper-173"><a href="#BandRipper-173"><span class="linenos">173</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">AlbumRipper</span><span class="p">(</span><span class="n">url</span><span class="p">,</span> <span class="n">no_track_number</span><span class="p">,</span> <span class="n">overwrite</span><span class="p">))</span>
-</span><span id="BandRipper-174"><a href="#BandRipper-174"><span class="linenos">174</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="BandRipper-175"><a href="#BandRipper-175"><span class="linenos">175</span></a>                <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
-</span><span id="BandRipper-176"><a href="#BandRipper-176"><span class="linenos">176</span></a>
-</span><span id="BandRipper-177"><a href="#BandRipper-177"><span class="linenos">177</span></a>    <span class="k">def</span> <span class="nf">get_album_urls</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">band_url</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
-</span><span id="BandRipper-178"><a href="#BandRipper-178"><span class="linenos">178</span></a>        <span class="sd">&quot;&quot;&quot;Get album urls from the main bandcamp url.&quot;&quot;&quot;</span>
-</span><span id="BandRipper-179"><a href="#BandRipper-179"><span class="linenos">179</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Fetching discography from </span><span class="si">{</span><span class="n">band_url</span><span class="si">}</span><span class="s2">...&quot;</span><span class="p">)</span>
-</span><span id="BandRipper-180"><a href="#BandRipper-180"><span class="linenos">180</span></a>        <span class="n">response</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="n">band_url</span><span class="p">,</span> <span class="n">headers</span><span class="o">=</span><span class="n">whosyouragent</span><span class="o">.</span><span class="n">get_agent</span><span class="p">(</span><span class="n">as_dict</span><span class="o">=</span><span class="kc">True</span><span class="p">))</span>
-</span><span id="BandRipper-181"><a href="#BandRipper-181"><span class="linenos">181</span></a>        <span class="k">if</span> <span class="n">response</span><span class="o">.</span><span class="n">status_code</span> <span class="o">!=</span> <span class="mi">200</span><span class="p">:</span>
-</span><span id="BandRipper-182"><a href="#BandRipper-182"><span class="linenos">182</span></a>            <span class="k">raise</span> <span class="ne">RuntimeError</span><span class="p">(</span>
-</span><span id="BandRipper-183"><a href="#BandRipper-183"><span class="linenos">183</span></a>                <span class="sa">f</span><span class="s2">&quot;Getting </span><span class="si">{</span><span class="n">band_url</span><span class="si">}</span><span class="s2"> failed with status code </span><span class="si">{</span><span class="n">response</span><span class="o">.</span><span class="n">status_code</span><span class="si">}</span><span class="s2">.&quot;</span>
-</span><span id="BandRipper-184"><a href="#BandRipper-184"><span class="linenos">184</span></a>            <span class="p">)</span>
-</span><span id="BandRipper-185"><a href="#BandRipper-185"><span class="linenos">185</span></a>        <span class="n">soup</span> <span class="o">=</span> <span class="n">BeautifulSoup</span><span class="p">(</span><span class="n">response</span><span class="o">.</span><span class="n">text</span><span class="p">,</span> <span class="s2">&quot;html.parser&quot;</span><span class="p">)</span>
-</span><span id="BandRipper-186"><a href="#BandRipper-186"><span class="linenos">186</span></a>        <span class="n">grid</span> <span class="o">=</span> <span class="n">soup</span><span class="o">.</span><span class="n">find</span><span class="p">(</span><span class="s2">&quot;ol&quot;</span><span class="p">,</span> <span class="n">attrs</span><span class="o">=</span><span class="p">{</span><span class="s2">&quot;id&quot;</span><span class="p">:</span> <span class="s2">&quot;music-grid&quot;</span><span class="p">})</span>
-</span><span id="BandRipper-187"><a href="#BandRipper-187"><span class="linenos">187</span></a>        <span class="n">parsed_url</span> <span class="o">=</span> <span class="n">urlparse</span><span class="p">(</span><span class="n">band_url</span><span class="p">)</span>
-</span><span id="BandRipper-188"><a href="#BandRipper-188"><span class="linenos">188</span></a>        <span class="n">base_url</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;https://</span><span class="si">{</span><span class="n">parsed_url</span><span class="o">.</span><span class="n">netloc</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="BandRipper-189"><a href="#BandRipper-189"><span class="linenos">189</span></a>        <span class="k">return</span> <span class="p">[</span><span class="n">base_url</span> <span class="o">+</span> <span class="n">album</span><span class="o">.</span><span class="n">a</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;href&quot;</span><span class="p">)</span> <span class="k">for</span> <span class="n">album</span> <span class="ow">in</span> <span class="n">grid</span><span class="o">.</span><span class="n">find_all</span><span class="p">(</span><span class="s2">&quot;li&quot;</span><span class="p">)]</span>
-</span><span id="BandRipper-190"><a href="#BandRipper-190"><span class="linenos">190</span></a>
-</span><span id="BandRipper-191"><a href="#BandRipper-191"><span class="linenos">191</span></a>    <span class="k">def</span> <span class="nf">rip</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="BandRipper-192"><a href="#BandRipper-192"><span class="linenos">192</span></a>        <span class="nb">print</span><span class="p">(</span>
-</span><span id="BandRipper-193"><a href="#BandRipper-193"><span class="linenos">193</span></a>            <span class="sa">f</span><span class="s2">&quot;Downloading </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">)</span><span class="si">}</span><span class="s2"> albums by </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">artist</span><span class="si">}</span><span class="s2">.&quot;</span>
-</span><span id="BandRipper-194"><a href="#BandRipper-194"><span class="linenos">194</span></a>        <span class="p">)</span>
-</span><span id="BandRipper-195"><a href="#BandRipper-195"><span class="linenos">195</span></a>        <span class="n">timer</span> <span class="o">=</span> <span class="n">Timer</span><span class="p">(</span><span class="n">subsecond_resolution</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-</span><span id="BandRipper-196"><a href="#BandRipper-196"><span class="linenos">196</span></a>        <span class="n">timer</span><span class="o">.</span><span class="n">start</span><span class="p">()</span>
-</span><span id="BandRipper-197"><a href="#BandRipper-197"><span class="linenos">197</span></a>        <span class="n">fails</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="BandRipper-198"><a href="#BandRipper-198"><span class="linenos">198</span></a>        <span class="k">for</span> <span class="n">album</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">:</span>
-</span><span id="BandRipper-199"><a href="#BandRipper-199"><span class="linenos">199</span></a>            <span class="k">try</span><span class="p">:</span>
-</span><span id="BandRipper-200"><a href="#BandRipper-200"><span class="linenos">200</span></a>                <span class="n">album</span><span class="o">.</span><span class="n">rip</span><span class="p">()</span>
-</span><span id="BandRipper-201"><a href="#BandRipper-201"><span class="linenos">201</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="BandRipper-202"><a href="#BandRipper-202"><span class="linenos">202</span></a>                <span class="n">fails</span><span class="o">.</span><span class="n">append</span><span class="p">((</span><span class="n">album</span><span class="p">,</span> <span class="n">e</span><span class="p">))</span>
-</span><span id="BandRipper-203"><a href="#BandRipper-203"><span class="linenos">203</span></a>        <span class="n">timer</span><span class="o">.</span><span class="n">stop</span><span class="p">()</span>
-</span><span id="BandRipper-204"><a href="#BandRipper-204"><span class="linenos">204</span></a>        <span class="n">artist</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">artist</span>
-</span><span id="BandRipper-205"><a href="#BandRipper-205"><span class="linenos">205</span></a>        <span class="nb">print</span><span class="p">(</span>
-</span><span id="BandRipper-206"><a href="#BandRipper-206"><span class="linenos">206</span></a>            <span class="sa">f</span><span class="s2">&quot;Finished downloading </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">)</span><span class="si">}</span><span class="s2"> albums by </span><span class="si">{</span><span class="n">artist</span><span class="si">}</span><span class="s2"> in </span><span class="si">{</span><span class="n">timer</span><span class="o">.</span><span class="n">elapsed_str</span><span class="si">}</span><span class="s2">.&quot;</span>
-</span><span id="BandRipper-207"><a href="#BandRipper-207"><span class="linenos">207</span></a>        <span class="p">)</span>
-</span><span id="BandRipper-208"><a href="#BandRipper-208"><span class="linenos">208</span></a>        <span class="k">if</span> <span class="n">fails</span><span class="p">:</span>
-</span><span id="BandRipper-209"><a href="#BandRipper-209"><span class="linenos">209</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;The following downloads failed:&quot;</span><span class="p">)</span>
-</span><span id="BandRipper-210"><a href="#BandRipper-210"><span class="linenos">210</span></a>            <span class="k">for</span> <span class="n">fail</span> <span class="ow">in</span> <span class="n">fails</span><span class="p">:</span>
-</span><span id="BandRipper-211"><a href="#BandRipper-211"><span class="linenos">211</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">fail</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">fail</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="BandRipper-163"><a href="#BandRipper-163"><span class="linenos">163</span></a><span class="k">class</span> <span class="nc">BandRipper</span><span class="p">:</span>
+</span><span id="BandRipper-164"><a href="#BandRipper-164"><span class="linenos">164</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
+</span><span id="BandRipper-165"><a href="#BandRipper-165"><span class="linenos">165</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">band_url</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">no_track_number</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span> <span class="n">overwrite</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="BandRipper-166"><a href="#BandRipper-166"><span class="linenos">166</span></a>    <span class="p">):</span>
+</span><span id="BandRipper-167"><a href="#BandRipper-167"><span class="linenos">167</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">band_url</span> <span class="o">=</span> <span class="n">band_url</span>
+</span><span id="BandRipper-168"><a href="#BandRipper-168"><span class="linenos">168</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">albums</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="BandRipper-169"><a href="#BandRipper-169"><span class="linenos">169</span></a>        <span class="k">for</span> <span class="n">url</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_album_urls</span><span class="p">(</span><span class="n">band_url</span><span class="p">):</span>
+</span><span id="BandRipper-170"><a href="#BandRipper-170"><span class="linenos">170</span></a>            <span class="k">try</span><span class="p">:</span>
+</span><span id="BandRipper-171"><a href="#BandRipper-171"><span class="linenos">171</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">AlbumRipper</span><span class="p">(</span><span class="n">url</span><span class="p">,</span> <span class="n">no_track_number</span><span class="p">,</span> <span class="n">overwrite</span><span class="p">))</span>
+</span><span id="BandRipper-172"><a href="#BandRipper-172"><span class="linenos">172</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="BandRipper-173"><a href="#BandRipper-173"><span class="linenos">173</span></a>                <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
+</span><span id="BandRipper-174"><a href="#BandRipper-174"><span class="linenos">174</span></a>
+</span><span id="BandRipper-175"><a href="#BandRipper-175"><span class="linenos">175</span></a>    <span class="k">def</span> <span class="nf">get_album_urls</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">band_url</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
+</span><span id="BandRipper-176"><a href="#BandRipper-176"><span class="linenos">176</span></a>        <span class="sd">&quot;&quot;&quot;Get album urls from the main bandcamp url.&quot;&quot;&quot;</span>
+</span><span id="BandRipper-177"><a href="#BandRipper-177"><span class="linenos">177</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Fetching discography from </span><span class="si">{</span><span class="n">band_url</span><span class="si">}</span><span class="s2">...&quot;</span><span class="p">)</span>
+</span><span id="BandRipper-178"><a href="#BandRipper-178"><span class="linenos">178</span></a>        <span class="n">response</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="n">band_url</span><span class="p">,</span> <span class="n">headers</span><span class="o">=</span><span class="n">whosyouragent</span><span class="o">.</span><span class="n">get_agent</span><span class="p">(</span><span class="n">as_dict</span><span class="o">=</span><span class="kc">True</span><span class="p">))</span>
+</span><span id="BandRipper-179"><a href="#BandRipper-179"><span class="linenos">179</span></a>        <span class="k">if</span> <span class="n">response</span><span class="o">.</span><span class="n">status_code</span> <span class="o">!=</span> <span class="mi">200</span><span class="p">:</span>
+</span><span id="BandRipper-180"><a href="#BandRipper-180"><span class="linenos">180</span></a>            <span class="k">raise</span> <span class="ne">RuntimeError</span><span class="p">(</span>
+</span><span id="BandRipper-181"><a href="#BandRipper-181"><span class="linenos">181</span></a>                <span class="sa">f</span><span class="s2">&quot;Getting </span><span class="si">{</span><span class="n">band_url</span><span class="si">}</span><span class="s2"> failed with status code </span><span class="si">{</span><span class="n">response</span><span class="o">.</span><span class="n">status_code</span><span class="si">}</span><span class="s2">.&quot;</span>
+</span><span id="BandRipper-182"><a href="#BandRipper-182"><span class="linenos">182</span></a>            <span class="p">)</span>
+</span><span id="BandRipper-183"><a href="#BandRipper-183"><span class="linenos">183</span></a>        <span class="n">soup</span> <span class="o">=</span> <span class="n">BeautifulSoup</span><span class="p">(</span><span class="n">response</span><span class="o">.</span><span class="n">text</span><span class="p">,</span> <span class="s2">&quot;html.parser&quot;</span><span class="p">)</span>
+</span><span id="BandRipper-184"><a href="#BandRipper-184"><span class="linenos">184</span></a>        <span class="n">grid</span> <span class="o">=</span> <span class="n">soup</span><span class="o">.</span><span class="n">find</span><span class="p">(</span><span class="s2">&quot;ol&quot;</span><span class="p">,</span> <span class="n">attrs</span><span class="o">=</span><span class="p">{</span><span class="s2">&quot;id&quot;</span><span class="p">:</span> <span class="s2">&quot;music-grid&quot;</span><span class="p">})</span>
+</span><span id="BandRipper-185"><a href="#BandRipper-185"><span class="linenos">185</span></a>        <span class="n">parsed_url</span> <span class="o">=</span> <span class="n">urlparse</span><span class="p">(</span><span class="n">band_url</span><span class="p">)</span>
+</span><span id="BandRipper-186"><a href="#BandRipper-186"><span class="linenos">186</span></a>        <span class="n">base_url</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;https://</span><span class="si">{</span><span class="n">parsed_url</span><span class="o">.</span><span class="n">netloc</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="BandRipper-187"><a href="#BandRipper-187"><span class="linenos">187</span></a>        <span class="k">return</span> <span class="p">[</span><span class="n">base_url</span> <span class="o">+</span> <span class="n">album</span><span class="o">.</span><span class="n">a</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;href&quot;</span><span class="p">)</span> <span class="k">for</span> <span class="n">album</span> <span class="ow">in</span> <span class="n">grid</span><span class="o">.</span><span class="n">find_all</span><span class="p">(</span><span class="s2">&quot;li&quot;</span><span class="p">)]</span>
+</span><span id="BandRipper-188"><a href="#BandRipper-188"><span class="linenos">188</span></a>
+</span><span id="BandRipper-189"><a href="#BandRipper-189"><span class="linenos">189</span></a>    <span class="k">def</span> <span class="nf">rip</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="BandRipper-190"><a href="#BandRipper-190"><span class="linenos">190</span></a>        <span class="nb">print</span><span class="p">(</span>
+</span><span id="BandRipper-191"><a href="#BandRipper-191"><span class="linenos">191</span></a>            <span class="sa">f</span><span class="s2">&quot;Downloading </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">)</span><span class="si">}</span><span class="s2"> albums by </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">artist</span><span class="si">}</span><span class="s2">.&quot;</span>
+</span><span id="BandRipper-192"><a href="#BandRipper-192"><span class="linenos">192</span></a>        <span class="p">)</span>
+</span><span id="BandRipper-193"><a href="#BandRipper-193"><span class="linenos">193</span></a>        <span class="n">timer</span> <span class="o">=</span> <span class="n">Timer</span><span class="p">(</span><span class="n">subsecond_resolution</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+</span><span id="BandRipper-194"><a href="#BandRipper-194"><span class="linenos">194</span></a>        <span class="n">timer</span><span class="o">.</span><span class="n">start</span><span class="p">()</span>
+</span><span id="BandRipper-195"><a href="#BandRipper-195"><span class="linenos">195</span></a>        <span class="n">fails</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="BandRipper-196"><a href="#BandRipper-196"><span class="linenos">196</span></a>        <span class="k">for</span> <span class="n">album</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">:</span>
+</span><span id="BandRipper-197"><a href="#BandRipper-197"><span class="linenos">197</span></a>            <span class="k">try</span><span class="p">:</span>
+</span><span id="BandRipper-198"><a href="#BandRipper-198"><span class="linenos">198</span></a>                <span class="n">album</span><span class="o">.</span><span class="n">rip</span><span class="p">()</span>
+</span><span id="BandRipper-199"><a href="#BandRipper-199"><span class="linenos">199</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="BandRipper-200"><a href="#BandRipper-200"><span class="linenos">200</span></a>                <span class="n">fails</span><span class="o">.</span><span class="n">append</span><span class="p">((</span><span class="n">album</span><span class="p">,</span> <span class="n">e</span><span class="p">))</span>
+</span><span id="BandRipper-201"><a href="#BandRipper-201"><span class="linenos">201</span></a>        <span class="n">timer</span><span class="o">.</span><span class="n">stop</span><span class="p">()</span>
+</span><span id="BandRipper-202"><a href="#BandRipper-202"><span class="linenos">202</span></a>        <span class="n">artist</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">artist</span>
+</span><span id="BandRipper-203"><a href="#BandRipper-203"><span class="linenos">203</span></a>        <span class="nb">print</span><span class="p">(</span>
+</span><span id="BandRipper-204"><a href="#BandRipper-204"><span class="linenos">204</span></a>            <span class="sa">f</span><span class="s2">&quot;Finished downloading </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">)</span><span class="si">}</span><span class="s2"> albums by </span><span class="si">{</span><span class="n">artist</span><span class="si">}</span><span class="s2"> in </span><span class="si">{</span><span class="n">timer</span><span class="o">.</span><span class="n">elapsed_str</span><span class="si">}</span><span class="s2">.&quot;</span>
+</span><span id="BandRipper-205"><a href="#BandRipper-205"><span class="linenos">205</span></a>        <span class="p">)</span>
+</span><span id="BandRipper-206"><a href="#BandRipper-206"><span class="linenos">206</span></a>        <span class="k">if</span> <span class="n">fails</span><span class="p">:</span>
+</span><span id="BandRipper-207"><a href="#BandRipper-207"><span class="linenos">207</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;The following downloads failed:&quot;</span><span class="p">)</span>
+</span><span id="BandRipper-208"><a href="#BandRipper-208"><span class="linenos">208</span></a>            <span class="k">for</span> <span class="n">fail</span> <span class="ow">in</span> <span class="n">fails</span><span class="p">:</span>
+</span><span id="BandRipper-209"><a href="#BandRipper-209"><span class="linenos">209</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">fail</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">fail</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             <div id="BandRipper.__init__" class="classattr">
                                         <input id="BandRipper.__init__-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
@@ -943,24 +939,24 @@
             
         <span class="name">BandRipper</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="n">band_url</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">no_track_number</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>,</span><span class="param">	<span class="n">overwrite</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span></span>)</span>
 
                 <label class="view-source-button" for="BandRipper.__init__-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#BandRipper.__init__"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="BandRipper.__init__-166"><a href="#BandRipper.__init__-166"><span class="linenos">166</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
-</span><span id="BandRipper.__init__-167"><a href="#BandRipper.__init__-167"><span class="linenos">167</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">band_url</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">no_track_number</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span> <span class="n">overwrite</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="BandRipper.__init__-168"><a href="#BandRipper.__init__-168"><span class="linenos">168</span></a>    <span class="p">):</span>
-</span><span id="BandRipper.__init__-169"><a href="#BandRipper.__init__-169"><span class="linenos">169</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">band_url</span> <span class="o">=</span> <span class="n">band_url</span>
-</span><span id="BandRipper.__init__-170"><a href="#BandRipper.__init__-170"><span class="linenos">170</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">albums</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="BandRipper.__init__-171"><a href="#BandRipper.__init__-171"><span class="linenos">171</span></a>        <span class="k">for</span> <span class="n">url</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_album_urls</span><span class="p">(</span><span class="n">band_url</span><span class="p">):</span>
-</span><span id="BandRipper.__init__-172"><a href="#BandRipper.__init__-172"><span class="linenos">172</span></a>            <span class="k">try</span><span class="p">:</span>
-</span><span id="BandRipper.__init__-173"><a href="#BandRipper.__init__-173"><span class="linenos">173</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">AlbumRipper</span><span class="p">(</span><span class="n">url</span><span class="p">,</span> <span class="n">no_track_number</span><span class="p">,</span> <span class="n">overwrite</span><span class="p">))</span>
-</span><span id="BandRipper.__init__-174"><a href="#BandRipper.__init__-174"><span class="linenos">174</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="BandRipper.__init__-175"><a href="#BandRipper.__init__-175"><span class="linenos">175</span></a>                <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="BandRipper.__init__-164"><a href="#BandRipper.__init__-164"><span class="linenos">164</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
+</span><span id="BandRipper.__init__-165"><a href="#BandRipper.__init__-165"><span class="linenos">165</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">band_url</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">no_track_number</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span> <span class="n">overwrite</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="BandRipper.__init__-166"><a href="#BandRipper.__init__-166"><span class="linenos">166</span></a>    <span class="p">):</span>
+</span><span id="BandRipper.__init__-167"><a href="#BandRipper.__init__-167"><span class="linenos">167</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">band_url</span> <span class="o">=</span> <span class="n">band_url</span>
+</span><span id="BandRipper.__init__-168"><a href="#BandRipper.__init__-168"><span class="linenos">168</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">albums</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="BandRipper.__init__-169"><a href="#BandRipper.__init__-169"><span class="linenos">169</span></a>        <span class="k">for</span> <span class="n">url</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_album_urls</span><span class="p">(</span><span class="n">band_url</span><span class="p">):</span>
+</span><span id="BandRipper.__init__-170"><a href="#BandRipper.__init__-170"><span class="linenos">170</span></a>            <span class="k">try</span><span class="p">:</span>
+</span><span id="BandRipper.__init__-171"><a href="#BandRipper.__init__-171"><span class="linenos">171</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">AlbumRipper</span><span class="p">(</span><span class="n">url</span><span class="p">,</span> <span class="n">no_track_number</span><span class="p">,</span> <span class="n">overwrite</span><span class="p">))</span>
+</span><span id="BandRipper.__init__-172"><a href="#BandRipper.__init__-172"><span class="linenos">172</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="BandRipper.__init__-173"><a href="#BandRipper.__init__-173"><span class="linenos">173</span></a>                <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             </div>
                             <div id="BandRipper.get_album_urls" class="classattr">
@@ -970,27 +966,27 @@
         <span class="def">def</span>
         <span class="name">get_album_urls</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">band_url</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span>:</span></span>
 
                 <label class="view-source-button" for="BandRipper.get_album_urls-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#BandRipper.get_album_urls"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="BandRipper.get_album_urls-177"><a href="#BandRipper.get_album_urls-177"><span class="linenos">177</span></a>    <span class="k">def</span> <span class="nf">get_album_urls</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">band_url</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
-</span><span id="BandRipper.get_album_urls-178"><a href="#BandRipper.get_album_urls-178"><span class="linenos">178</span></a>        <span class="sd">&quot;&quot;&quot;Get album urls from the main bandcamp url.&quot;&quot;&quot;</span>
-</span><span id="BandRipper.get_album_urls-179"><a href="#BandRipper.get_album_urls-179"><span class="linenos">179</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Fetching discography from </span><span class="si">{</span><span class="n">band_url</span><span class="si">}</span><span class="s2">...&quot;</span><span class="p">)</span>
-</span><span id="BandRipper.get_album_urls-180"><a href="#BandRipper.get_album_urls-180"><span class="linenos">180</span></a>        <span class="n">response</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="n">band_url</span><span class="p">,</span> <span class="n">headers</span><span class="o">=</span><span class="n">whosyouragent</span><span class="o">.</span><span class="n">get_agent</span><span class="p">(</span><span class="n">as_dict</span><span class="o">=</span><span class="kc">True</span><span class="p">))</span>
-</span><span id="BandRipper.get_album_urls-181"><a href="#BandRipper.get_album_urls-181"><span class="linenos">181</span></a>        <span class="k">if</span> <span class="n">response</span><span class="o">.</span><span class="n">status_code</span> <span class="o">!=</span> <span class="mi">200</span><span class="p">:</span>
-</span><span id="BandRipper.get_album_urls-182"><a href="#BandRipper.get_album_urls-182"><span class="linenos">182</span></a>            <span class="k">raise</span> <span class="ne">RuntimeError</span><span class="p">(</span>
-</span><span id="BandRipper.get_album_urls-183"><a href="#BandRipper.get_album_urls-183"><span class="linenos">183</span></a>                <span class="sa">f</span><span class="s2">&quot;Getting </span><span class="si">{</span><span class="n">band_url</span><span class="si">}</span><span class="s2"> failed with status code </span><span class="si">{</span><span class="n">response</span><span class="o">.</span><span class="n">status_code</span><span class="si">}</span><span class="s2">.&quot;</span>
-</span><span id="BandRipper.get_album_urls-184"><a href="#BandRipper.get_album_urls-184"><span class="linenos">184</span></a>            <span class="p">)</span>
-</span><span id="BandRipper.get_album_urls-185"><a href="#BandRipper.get_album_urls-185"><span class="linenos">185</span></a>        <span class="n">soup</span> <span class="o">=</span> <span class="n">BeautifulSoup</span><span class="p">(</span><span class="n">response</span><span class="o">.</span><span class="n">text</span><span class="p">,</span> <span class="s2">&quot;html.parser&quot;</span><span class="p">)</span>
-</span><span id="BandRipper.get_album_urls-186"><a href="#BandRipper.get_album_urls-186"><span class="linenos">186</span></a>        <span class="n">grid</span> <span class="o">=</span> <span class="n">soup</span><span class="o">.</span><span class="n">find</span><span class="p">(</span><span class="s2">&quot;ol&quot;</span><span class="p">,</span> <span class="n">attrs</span><span class="o">=</span><span class="p">{</span><span class="s2">&quot;id&quot;</span><span class="p">:</span> <span class="s2">&quot;music-grid&quot;</span><span class="p">})</span>
-</span><span id="BandRipper.get_album_urls-187"><a href="#BandRipper.get_album_urls-187"><span class="linenos">187</span></a>        <span class="n">parsed_url</span> <span class="o">=</span> <span class="n">urlparse</span><span class="p">(</span><span class="n">band_url</span><span class="p">)</span>
-</span><span id="BandRipper.get_album_urls-188"><a href="#BandRipper.get_album_urls-188"><span class="linenos">188</span></a>        <span class="n">base_url</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;https://</span><span class="si">{</span><span class="n">parsed_url</span><span class="o">.</span><span class="n">netloc</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="BandRipper.get_album_urls-189"><a href="#BandRipper.get_album_urls-189"><span class="linenos">189</span></a>        <span class="k">return</span> <span class="p">[</span><span class="n">base_url</span> <span class="o">+</span> <span class="n">album</span><span class="o">.</span><span class="n">a</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;href&quot;</span><span class="p">)</span> <span class="k">for</span> <span class="n">album</span> <span class="ow">in</span> <span class="n">grid</span><span class="o">.</span><span class="n">find_all</span><span class="p">(</span><span class="s2">&quot;li&quot;</span><span class="p">)]</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="BandRipper.get_album_urls-175"><a href="#BandRipper.get_album_urls-175"><span class="linenos">175</span></a>    <span class="k">def</span> <span class="nf">get_album_urls</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">band_url</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
+</span><span id="BandRipper.get_album_urls-176"><a href="#BandRipper.get_album_urls-176"><span class="linenos">176</span></a>        <span class="sd">&quot;&quot;&quot;Get album urls from the main bandcamp url.&quot;&quot;&quot;</span>
+</span><span id="BandRipper.get_album_urls-177"><a href="#BandRipper.get_album_urls-177"><span class="linenos">177</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Fetching discography from </span><span class="si">{</span><span class="n">band_url</span><span class="si">}</span><span class="s2">...&quot;</span><span class="p">)</span>
+</span><span id="BandRipper.get_album_urls-178"><a href="#BandRipper.get_album_urls-178"><span class="linenos">178</span></a>        <span class="n">response</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="n">band_url</span><span class="p">,</span> <span class="n">headers</span><span class="o">=</span><span class="n">whosyouragent</span><span class="o">.</span><span class="n">get_agent</span><span class="p">(</span><span class="n">as_dict</span><span class="o">=</span><span class="kc">True</span><span class="p">))</span>
+</span><span id="BandRipper.get_album_urls-179"><a href="#BandRipper.get_album_urls-179"><span class="linenos">179</span></a>        <span class="k">if</span> <span class="n">response</span><span class="o">.</span><span class="n">status_code</span> <span class="o">!=</span> <span class="mi">200</span><span class="p">:</span>
+</span><span id="BandRipper.get_album_urls-180"><a href="#BandRipper.get_album_urls-180"><span class="linenos">180</span></a>            <span class="k">raise</span> <span class="ne">RuntimeError</span><span class="p">(</span>
+</span><span id="BandRipper.get_album_urls-181"><a href="#BandRipper.get_album_urls-181"><span class="linenos">181</span></a>                <span class="sa">f</span><span class="s2">&quot;Getting </span><span class="si">{</span><span class="n">band_url</span><span class="si">}</span><span class="s2"> failed with status code </span><span class="si">{</span><span class="n">response</span><span class="o">.</span><span class="n">status_code</span><span class="si">}</span><span class="s2">.&quot;</span>
+</span><span id="BandRipper.get_album_urls-182"><a href="#BandRipper.get_album_urls-182"><span class="linenos">182</span></a>            <span class="p">)</span>
+</span><span id="BandRipper.get_album_urls-183"><a href="#BandRipper.get_album_urls-183"><span class="linenos">183</span></a>        <span class="n">soup</span> <span class="o">=</span> <span class="n">BeautifulSoup</span><span class="p">(</span><span class="n">response</span><span class="o">.</span><span class="n">text</span><span class="p">,</span> <span class="s2">&quot;html.parser&quot;</span><span class="p">)</span>
+</span><span id="BandRipper.get_album_urls-184"><a href="#BandRipper.get_album_urls-184"><span class="linenos">184</span></a>        <span class="n">grid</span> <span class="o">=</span> <span class="n">soup</span><span class="o">.</span><span class="n">find</span><span class="p">(</span><span class="s2">&quot;ol&quot;</span><span class="p">,</span> <span class="n">attrs</span><span class="o">=</span><span class="p">{</span><span class="s2">&quot;id&quot;</span><span class="p">:</span> <span class="s2">&quot;music-grid&quot;</span><span class="p">})</span>
+</span><span id="BandRipper.get_album_urls-185"><a href="#BandRipper.get_album_urls-185"><span class="linenos">185</span></a>        <span class="n">parsed_url</span> <span class="o">=</span> <span class="n">urlparse</span><span class="p">(</span><span class="n">band_url</span><span class="p">)</span>
+</span><span id="BandRipper.get_album_urls-186"><a href="#BandRipper.get_album_urls-186"><span class="linenos">186</span></a>        <span class="n">base_url</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;https://</span><span class="si">{</span><span class="n">parsed_url</span><span class="o">.</span><span class="n">netloc</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="BandRipper.get_album_urls-187"><a href="#BandRipper.get_album_urls-187"><span class="linenos">187</span></a>        <span class="k">return</span> <span class="p">[</span><span class="n">base_url</span> <span class="o">+</span> <span class="n">album</span><span class="o">.</span><span class="n">a</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;href&quot;</span><span class="p">)</span> <span class="k">for</span> <span class="n">album</span> <span class="ow">in</span> <span class="n">grid</span><span class="o">.</span><span class="n">find_all</span><span class="p">(</span><span class="s2">&quot;li&quot;</span><span class="p">)]</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Get album urls from the main bandcamp url.</p>
 </div>
 
 
@@ -1002,35 +998,35 @@
         <span class="def">def</span>
         <span class="name">rip</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="BandRipper.rip-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#BandRipper.rip"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="BandRipper.rip-191"><a href="#BandRipper.rip-191"><span class="linenos">191</span></a>    <span class="k">def</span> <span class="nf">rip</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="BandRipper.rip-192"><a href="#BandRipper.rip-192"><span class="linenos">192</span></a>        <span class="nb">print</span><span class="p">(</span>
-</span><span id="BandRipper.rip-193"><a href="#BandRipper.rip-193"><span class="linenos">193</span></a>            <span class="sa">f</span><span class="s2">&quot;Downloading </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">)</span><span class="si">}</span><span class="s2"> albums by </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">artist</span><span class="si">}</span><span class="s2">.&quot;</span>
-</span><span id="BandRipper.rip-194"><a href="#BandRipper.rip-194"><span class="linenos">194</span></a>        <span class="p">)</span>
-</span><span id="BandRipper.rip-195"><a href="#BandRipper.rip-195"><span class="linenos">195</span></a>        <span class="n">timer</span> <span class="o">=</span> <span class="n">Timer</span><span class="p">(</span><span class="n">subsecond_resolution</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-</span><span id="BandRipper.rip-196"><a href="#BandRipper.rip-196"><span class="linenos">196</span></a>        <span class="n">timer</span><span class="o">.</span><span class="n">start</span><span class="p">()</span>
-</span><span id="BandRipper.rip-197"><a href="#BandRipper.rip-197"><span class="linenos">197</span></a>        <span class="n">fails</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="BandRipper.rip-198"><a href="#BandRipper.rip-198"><span class="linenos">198</span></a>        <span class="k">for</span> <span class="n">album</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">:</span>
-</span><span id="BandRipper.rip-199"><a href="#BandRipper.rip-199"><span class="linenos">199</span></a>            <span class="k">try</span><span class="p">:</span>
-</span><span id="BandRipper.rip-200"><a href="#BandRipper.rip-200"><span class="linenos">200</span></a>                <span class="n">album</span><span class="o">.</span><span class="n">rip</span><span class="p">()</span>
-</span><span id="BandRipper.rip-201"><a href="#BandRipper.rip-201"><span class="linenos">201</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="BandRipper.rip-202"><a href="#BandRipper.rip-202"><span class="linenos">202</span></a>                <span class="n">fails</span><span class="o">.</span><span class="n">append</span><span class="p">((</span><span class="n">album</span><span class="p">,</span> <span class="n">e</span><span class="p">))</span>
-</span><span id="BandRipper.rip-203"><a href="#BandRipper.rip-203"><span class="linenos">203</span></a>        <span class="n">timer</span><span class="o">.</span><span class="n">stop</span><span class="p">()</span>
-</span><span id="BandRipper.rip-204"><a href="#BandRipper.rip-204"><span class="linenos">204</span></a>        <span class="n">artist</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">artist</span>
-</span><span id="BandRipper.rip-205"><a href="#BandRipper.rip-205"><span class="linenos">205</span></a>        <span class="nb">print</span><span class="p">(</span>
-</span><span id="BandRipper.rip-206"><a href="#BandRipper.rip-206"><span class="linenos">206</span></a>            <span class="sa">f</span><span class="s2">&quot;Finished downloading </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">)</span><span class="si">}</span><span class="s2"> albums by </span><span class="si">{</span><span class="n">artist</span><span class="si">}</span><span class="s2"> in </span><span class="si">{</span><span class="n">timer</span><span class="o">.</span><span class="n">elapsed_str</span><span class="si">}</span><span class="s2">.&quot;</span>
-</span><span id="BandRipper.rip-207"><a href="#BandRipper.rip-207"><span class="linenos">207</span></a>        <span class="p">)</span>
-</span><span id="BandRipper.rip-208"><a href="#BandRipper.rip-208"><span class="linenos">208</span></a>        <span class="k">if</span> <span class="n">fails</span><span class="p">:</span>
-</span><span id="BandRipper.rip-209"><a href="#BandRipper.rip-209"><span class="linenos">209</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;The following downloads failed:&quot;</span><span class="p">)</span>
-</span><span id="BandRipper.rip-210"><a href="#BandRipper.rip-210"><span class="linenos">210</span></a>            <span class="k">for</span> <span class="n">fail</span> <span class="ow">in</span> <span class="n">fails</span><span class="p">:</span>
-</span><span id="BandRipper.rip-211"><a href="#BandRipper.rip-211"><span class="linenos">211</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">fail</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">fail</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="BandRipper.rip-189"><a href="#BandRipper.rip-189"><span class="linenos">189</span></a>    <span class="k">def</span> <span class="nf">rip</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="BandRipper.rip-190"><a href="#BandRipper.rip-190"><span class="linenos">190</span></a>        <span class="nb">print</span><span class="p">(</span>
+</span><span id="BandRipper.rip-191"><a href="#BandRipper.rip-191"><span class="linenos">191</span></a>            <span class="sa">f</span><span class="s2">&quot;Downloading </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">)</span><span class="si">}</span><span class="s2"> albums by </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">artist</span><span class="si">}</span><span class="s2">.&quot;</span>
+</span><span id="BandRipper.rip-192"><a href="#BandRipper.rip-192"><span class="linenos">192</span></a>        <span class="p">)</span>
+</span><span id="BandRipper.rip-193"><a href="#BandRipper.rip-193"><span class="linenos">193</span></a>        <span class="n">timer</span> <span class="o">=</span> <span class="n">Timer</span><span class="p">(</span><span class="n">subsecond_resolution</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+</span><span id="BandRipper.rip-194"><a href="#BandRipper.rip-194"><span class="linenos">194</span></a>        <span class="n">timer</span><span class="o">.</span><span class="n">start</span><span class="p">()</span>
+</span><span id="BandRipper.rip-195"><a href="#BandRipper.rip-195"><span class="linenos">195</span></a>        <span class="n">fails</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="BandRipper.rip-196"><a href="#BandRipper.rip-196"><span class="linenos">196</span></a>        <span class="k">for</span> <span class="n">album</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">:</span>
+</span><span id="BandRipper.rip-197"><a href="#BandRipper.rip-197"><span class="linenos">197</span></a>            <span class="k">try</span><span class="p">:</span>
+</span><span id="BandRipper.rip-198"><a href="#BandRipper.rip-198"><span class="linenos">198</span></a>                <span class="n">album</span><span class="o">.</span><span class="n">rip</span><span class="p">()</span>
+</span><span id="BandRipper.rip-199"><a href="#BandRipper.rip-199"><span class="linenos">199</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="BandRipper.rip-200"><a href="#BandRipper.rip-200"><span class="linenos">200</span></a>                <span class="n">fails</span><span class="o">.</span><span class="n">append</span><span class="p">((</span><span class="n">album</span><span class="p">,</span> <span class="n">e</span><span class="p">))</span>
+</span><span id="BandRipper.rip-201"><a href="#BandRipper.rip-201"><span class="linenos">201</span></a>        <span class="n">timer</span><span class="o">.</span><span class="n">stop</span><span class="p">()</span>
+</span><span id="BandRipper.rip-202"><a href="#BandRipper.rip-202"><span class="linenos">202</span></a>        <span class="n">artist</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">artist</span>
+</span><span id="BandRipper.rip-203"><a href="#BandRipper.rip-203"><span class="linenos">203</span></a>        <span class="nb">print</span><span class="p">(</span>
+</span><span id="BandRipper.rip-204"><a href="#BandRipper.rip-204"><span class="linenos">204</span></a>            <span class="sa">f</span><span class="s2">&quot;Finished downloading </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">)</span><span class="si">}</span><span class="s2"> albums by </span><span class="si">{</span><span class="n">artist</span><span class="si">}</span><span class="s2"> in </span><span class="si">{</span><span class="n">timer</span><span class="o">.</span><span class="n">elapsed_str</span><span class="si">}</span><span class="s2">.&quot;</span>
+</span><span id="BandRipper.rip-205"><a href="#BandRipper.rip-205"><span class="linenos">205</span></a>        <span class="p">)</span>
+</span><span id="BandRipper.rip-206"><a href="#BandRipper.rip-206"><span class="linenos">206</span></a>        <span class="k">if</span> <span class="n">fails</span><span class="p">:</span>
+</span><span id="BandRipper.rip-207"><a href="#BandRipper.rip-207"><span class="linenos">207</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;The following downloads failed:&quot;</span><span class="p">)</span>
+</span><span id="BandRipper.rip-208"><a href="#BandRipper.rip-208"><span class="linenos">208</span></a>            <span class="k">for</span> <span class="n">fail</span> <span class="ow">in</span> <span class="n">fails</span><span class="p">:</span>
+</span><span id="BandRipper.rip-209"><a href="#BandRipper.rip-209"><span class="linenos">209</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">fail</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">fail</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             </div>
                 </section>
@@ -1041,27 +1037,27 @@
         <span class="def">def</span>
         <span class="name">page_is_discography</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">url</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="nb">bool</span>:</span></span>
 
                 <label class="view-source-button" for="page_is_discography-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#page_is_discography"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="page_is_discography-214"><a href="#page_is_discography-214"><span class="linenos">214</span></a><span class="k">def</span> <span class="nf">page_is_discography</span><span class="p">(</span><span class="n">url</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="page_is_discography-215"><a href="#page_is_discography-215"><span class="linenos">215</span></a>    <span class="sd">&quot;&quot;&quot;Returns whether the url is to a discography page or not.&quot;&quot;&quot;</span>
-</span><span id="page_is_discography-216"><a href="#page_is_discography-216"><span class="linenos">216</span></a>    <span class="n">response</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="n">url</span><span class="p">,</span> <span class="n">headers</span><span class="o">=</span><span class="n">whosyouragent</span><span class="o">.</span><span class="n">get_agent</span><span class="p">(</span><span class="n">as_dict</span><span class="o">=</span><span class="kc">True</span><span class="p">))</span>
-</span><span id="page_is_discography-217"><a href="#page_is_discography-217"><span class="linenos">217</span></a>    <span class="k">if</span> <span class="n">response</span><span class="o">.</span><span class="n">status_code</span> <span class="o">!=</span> <span class="mi">200</span><span class="p">:</span>
-</span><span id="page_is_discography-218"><a href="#page_is_discography-218"><span class="linenos">218</span></a>        <span class="k">raise</span> <span class="ne">RuntimeError</span><span class="p">(</span>
-</span><span id="page_is_discography-219"><a href="#page_is_discography-219"><span class="linenos">219</span></a>            <span class="sa">f</span><span class="s2">&quot;Getting </span><span class="si">{</span><span class="n">url</span><span class="si">}</span><span class="s2"> failed with status code </span><span class="si">{</span><span class="n">response</span><span class="o">.</span><span class="n">status_code</span><span class="si">}</span><span class="s2">.&quot;</span>
-</span><span id="page_is_discography-220"><a href="#page_is_discography-220"><span class="linenos">220</span></a>        <span class="p">)</span>
-</span><span id="page_is_discography-221"><a href="#page_is_discography-221"><span class="linenos">221</span></a>    <span class="n">soup</span> <span class="o">=</span> <span class="n">BeautifulSoup</span><span class="p">(</span><span class="n">response</span><span class="o">.</span><span class="n">text</span><span class="p">,</span> <span class="s2">&quot;html.parser&quot;</span><span class="p">)</span>
-</span><span id="page_is_discography-222"><a href="#page_is_discography-222"><span class="linenos">222</span></a>    <span class="c1"># Returns None if it doesn&#39;t exist.</span>
-</span><span id="page_is_discography-223"><a href="#page_is_discography-223"><span class="linenos">223</span></a>    <span class="n">grid</span> <span class="o">=</span> <span class="n">soup</span><span class="o">.</span><span class="n">find</span><span class="p">(</span><span class="s2">&quot;ol&quot;</span><span class="p">,</span> <span class="n">attrs</span><span class="o">=</span><span class="p">{</span><span class="s2">&quot;id&quot;</span><span class="p">:</span> <span class="s2">&quot;music-grid&quot;</span><span class="p">})</span>
-</span><span id="page_is_discography-224"><a href="#page_is_discography-224"><span class="linenos">224</span></a>    <span class="k">if</span> <span class="n">grid</span><span class="p">:</span>
-</span><span id="page_is_discography-225"><a href="#page_is_discography-225"><span class="linenos">225</span></a>        <span class="k">return</span> <span class="kc">True</span>
-</span><span id="page_is_discography-226"><a href="#page_is_discography-226"><span class="linenos">226</span></a>    <span class="k">return</span> <span class="kc">False</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="page_is_discography-212"><a href="#page_is_discography-212"><span class="linenos">212</span></a><span class="k">def</span> <span class="nf">page_is_discography</span><span class="p">(</span><span class="n">url</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="page_is_discography-213"><a href="#page_is_discography-213"><span class="linenos">213</span></a>    <span class="sd">&quot;&quot;&quot;Returns whether the url is to a discography page or not.&quot;&quot;&quot;</span>
+</span><span id="page_is_discography-214"><a href="#page_is_discography-214"><span class="linenos">214</span></a>    <span class="n">response</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="n">url</span><span class="p">,</span> <span class="n">headers</span><span class="o">=</span><span class="n">whosyouragent</span><span class="o">.</span><span class="n">get_agent</span><span class="p">(</span><span class="n">as_dict</span><span class="o">=</span><span class="kc">True</span><span class="p">))</span>
+</span><span id="page_is_discography-215"><a href="#page_is_discography-215"><span class="linenos">215</span></a>    <span class="k">if</span> <span class="n">response</span><span class="o">.</span><span class="n">status_code</span> <span class="o">!=</span> <span class="mi">200</span><span class="p">:</span>
+</span><span id="page_is_discography-216"><a href="#page_is_discography-216"><span class="linenos">216</span></a>        <span class="k">raise</span> <span class="ne">RuntimeError</span><span class="p">(</span>
+</span><span id="page_is_discography-217"><a href="#page_is_discography-217"><span class="linenos">217</span></a>            <span class="sa">f</span><span class="s2">&quot;Getting </span><span class="si">{</span><span class="n">url</span><span class="si">}</span><span class="s2"> failed with status code </span><span class="si">{</span><span class="n">response</span><span class="o">.</span><span class="n">status_code</span><span class="si">}</span><span class="s2">.&quot;</span>
+</span><span id="page_is_discography-218"><a href="#page_is_discography-218"><span class="linenos">218</span></a>        <span class="p">)</span>
+</span><span id="page_is_discography-219"><a href="#page_is_discography-219"><span class="linenos">219</span></a>    <span class="n">soup</span> <span class="o">=</span> <span class="n">BeautifulSoup</span><span class="p">(</span><span class="n">response</span><span class="o">.</span><span class="n">text</span><span class="p">,</span> <span class="s2">&quot;html.parser&quot;</span><span class="p">)</span>
+</span><span id="page_is_discography-220"><a href="#page_is_discography-220"><span class="linenos">220</span></a>    <span class="c1"># Returns None if it doesn&#39;t exist.</span>
+</span><span id="page_is_discography-221"><a href="#page_is_discography-221"><span class="linenos">221</span></a>    <span class="n">grid</span> <span class="o">=</span> <span class="n">soup</span><span class="o">.</span><span class="n">find</span><span class="p">(</span><span class="s2">&quot;ol&quot;</span><span class="p">,</span> <span class="n">attrs</span><span class="o">=</span><span class="p">{</span><span class="s2">&quot;id&quot;</span><span class="p">:</span> <span class="s2">&quot;music-grid&quot;</span><span class="p">})</span>
+</span><span id="page_is_discography-222"><a href="#page_is_discography-222"><span class="linenos">222</span></a>    <span class="k">if</span> <span class="n">grid</span><span class="p">:</span>
+</span><span id="page_is_discography-223"><a href="#page_is_discography-223"><span class="linenos">223</span></a>        <span class="k">return</span> <span class="kc">True</span>
+</span><span id="page_is_discography-224"><a href="#page_is_discography-224"><span class="linenos">224</span></a>    <span class="k">return</span> <span class="kc">False</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Returns whether the url is to a discography page or not.</p>
 </div>
 
 
@@ -1073,51 +1069,51 @@
         <span class="def">def</span>
         <span class="name">get_args</span><span class="signature pdoc-code condensed">(<span class="return-annotation">) -> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span>:</span></span>
 
                 <label class="view-source-button" for="get_args-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#get_args"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="get_args-229"><a href="#get_args-229"><span class="linenos">229</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
-</span><span id="get_args-230"><a href="#get_args-230"><span class="linenos">230</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
-</span><span id="get_args-231"><a href="#get_args-231"><span class="linenos">231</span></a>
-</span><span id="get_args-232"><a href="#get_args-232"><span class="linenos">232</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-233"><a href="#get_args-233"><span class="linenos">233</span></a>        <span class="s2">&quot;urls&quot;</span><span class="p">,</span>
-</span><span id="get_args-234"><a href="#get_args-234"><span class="linenos">234</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="get_args-235"><a href="#get_args-235"><span class="linenos">235</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
-</span><span id="get_args-236"><a href="#get_args-236"><span class="linenos">236</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The bandcamp url(s) for the album or artist.</span>
-</span><span id="get_args-237"><a href="#get_args-237"><span class="linenos">237</span></a><span class="s2">            If the url is to an artists main page,</span>
-</span><span id="get_args-238"><a href="#get_args-238"><span class="linenos">238</span></a><span class="s2">            all albums will be downloaded.</span>
-</span><span id="get_args-239"><a href="#get_args-239"><span class="linenos">239</span></a><span class="s2">            The tracks will be saved to a subdirectory of</span>
-</span><span id="get_args-240"><a href="#get_args-240"><span class="linenos">240</span></a><span class="s2">            your current directory.</span>
-</span><span id="get_args-241"><a href="#get_args-241"><span class="linenos">241</span></a><span class="s2">            If a track can&#39;t be streamed (i.e. private) it</span>
-</span><span id="get_args-242"><a href="#get_args-242"><span class="linenos">242</span></a><span class="s2">            won&#39;t be downloaded. Multiple urls can be passed.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-243"><a href="#get_args-243"><span class="linenos">243</span></a>    <span class="p">)</span>
-</span><span id="get_args-244"><a href="#get_args-244"><span class="linenos">244</span></a>
-</span><span id="get_args-245"><a href="#get_args-245"><span class="linenos">245</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-246"><a href="#get_args-246"><span class="linenos">246</span></a>        <span class="s2">&quot;-n&quot;</span><span class="p">,</span>
-</span><span id="get_args-247"><a href="#get_args-247"><span class="linenos">247</span></a>        <span class="s2">&quot;--no_track_number&quot;</span><span class="p">,</span>
-</span><span id="get_args-248"><a href="#get_args-248"><span class="linenos">248</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="get_args-249"><a href="#get_args-249"><span class="linenos">249</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; By default the track number will be added</span>
-</span><span id="get_args-250"><a href="#get_args-250"><span class="linenos">250</span></a><span class="s2">        to the front of the track title. Pass this switch</span>
-</span><span id="get_args-251"><a href="#get_args-251"><span class="linenos">251</span></a><span class="s2">        to disable the behavior.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-252"><a href="#get_args-252"><span class="linenos">252</span></a>    <span class="p">)</span>
-</span><span id="get_args-253"><a href="#get_args-253"><span class="linenos">253</span></a>
-</span><span id="get_args-254"><a href="#get_args-254"><span class="linenos">254</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-255"><a href="#get_args-255"><span class="linenos">255</span></a>        <span class="s2">&quot;-o&quot;</span><span class="p">,</span>
-</span><span id="get_args-256"><a href="#get_args-256"><span class="linenos">256</span></a>        <span class="s2">&quot;--overwrite&quot;</span><span class="p">,</span>
-</span><span id="get_args-257"><a href="#get_args-257"><span class="linenos">257</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="get_args-258"><a href="#get_args-258"><span class="linenos">258</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Pass this flag to overwrite existing files.</span>
-</span><span id="get_args-259"><a href="#get_args-259"><span class="linenos">259</span></a><span class="s2">        Otherwise don&#39;t download tracks that already exist locally.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-260"><a href="#get_args-260"><span class="linenos">260</span></a>    <span class="p">)</span>
-</span><span id="get_args-261"><a href="#get_args-261"><span class="linenos">261</span></a>
-</span><span id="get_args-262"><a href="#get_args-262"><span class="linenos">262</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
-</span><span id="get_args-263"><a href="#get_args-263"><span class="linenos">263</span></a>    <span class="n">args</span><span class="o">.</span><span class="n">urls</span> <span class="o">=</span> <span class="p">[</span><span class="n">url</span><span class="o">.</span><span class="n">strip</span><span class="p">(</span><span class="s2">&quot;/&quot;</span><span class="p">)</span> <span class="k">for</span> <span class="n">url</span> <span class="ow">in</span> <span class="n">args</span><span class="o">.</span><span class="n">urls</span><span class="p">]</span>
-</span><span id="get_args-264"><a href="#get_args-264"><span class="linenos">264</span></a>
-</span><span id="get_args-265"><a href="#get_args-265"><span class="linenos">265</span></a>    <span class="k">return</span> <span class="n">args</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="get_args-227"><a href="#get_args-227"><span class="linenos">227</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
+</span><span id="get_args-228"><a href="#get_args-228"><span class="linenos">228</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
+</span><span id="get_args-229"><a href="#get_args-229"><span class="linenos">229</span></a>
+</span><span id="get_args-230"><a href="#get_args-230"><span class="linenos">230</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-231"><a href="#get_args-231"><span class="linenos">231</span></a>        <span class="s2">&quot;urls&quot;</span><span class="p">,</span>
+</span><span id="get_args-232"><a href="#get_args-232"><span class="linenos">232</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="get_args-233"><a href="#get_args-233"><span class="linenos">233</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
+</span><span id="get_args-234"><a href="#get_args-234"><span class="linenos">234</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The bandcamp url(s) for the album or artist.</span>
+</span><span id="get_args-235"><a href="#get_args-235"><span class="linenos">235</span></a><span class="s2">            If the url is to an artists main page,</span>
+</span><span id="get_args-236"><a href="#get_args-236"><span class="linenos">236</span></a><span class="s2">            all albums will be downloaded.</span>
+</span><span id="get_args-237"><a href="#get_args-237"><span class="linenos">237</span></a><span class="s2">            The tracks will be saved to a subdirectory of</span>
+</span><span id="get_args-238"><a href="#get_args-238"><span class="linenos">238</span></a><span class="s2">            your current directory.</span>
+</span><span id="get_args-239"><a href="#get_args-239"><span class="linenos">239</span></a><span class="s2">            If a track can&#39;t be streamed (i.e. private) it</span>
+</span><span id="get_args-240"><a href="#get_args-240"><span class="linenos">240</span></a><span class="s2">            won&#39;t be downloaded. Multiple urls can be passed.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-241"><a href="#get_args-241"><span class="linenos">241</span></a>    <span class="p">)</span>
+</span><span id="get_args-242"><a href="#get_args-242"><span class="linenos">242</span></a>
+</span><span id="get_args-243"><a href="#get_args-243"><span class="linenos">243</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-244"><a href="#get_args-244"><span class="linenos">244</span></a>        <span class="s2">&quot;-n&quot;</span><span class="p">,</span>
+</span><span id="get_args-245"><a href="#get_args-245"><span class="linenos">245</span></a>        <span class="s2">&quot;--no_track_number&quot;</span><span class="p">,</span>
+</span><span id="get_args-246"><a href="#get_args-246"><span class="linenos">246</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="get_args-247"><a href="#get_args-247"><span class="linenos">247</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; By default the track number will be added</span>
+</span><span id="get_args-248"><a href="#get_args-248"><span class="linenos">248</span></a><span class="s2">        to the front of the track title. Pass this switch</span>
+</span><span id="get_args-249"><a href="#get_args-249"><span class="linenos">249</span></a><span class="s2">        to disable the behavior.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-250"><a href="#get_args-250"><span class="linenos">250</span></a>    <span class="p">)</span>
+</span><span id="get_args-251"><a href="#get_args-251"><span class="linenos">251</span></a>
+</span><span id="get_args-252"><a href="#get_args-252"><span class="linenos">252</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-253"><a href="#get_args-253"><span class="linenos">253</span></a>        <span class="s2">&quot;-o&quot;</span><span class="p">,</span>
+</span><span id="get_args-254"><a href="#get_args-254"><span class="linenos">254</span></a>        <span class="s2">&quot;--overwrite&quot;</span><span class="p">,</span>
+</span><span id="get_args-255"><a href="#get_args-255"><span class="linenos">255</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="get_args-256"><a href="#get_args-256"><span class="linenos">256</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Pass this flag to overwrite existing files.</span>
+</span><span id="get_args-257"><a href="#get_args-257"><span class="linenos">257</span></a><span class="s2">        Otherwise don&#39;t download tracks that already exist locally.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-258"><a href="#get_args-258"><span class="linenos">258</span></a>    <span class="p">)</span>
+</span><span id="get_args-259"><a href="#get_args-259"><span class="linenos">259</span></a>
+</span><span id="get_args-260"><a href="#get_args-260"><span class="linenos">260</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
+</span><span id="get_args-261"><a href="#get_args-261"><span class="linenos">261</span></a>    <span class="n">args</span><span class="o">.</span><span class="n">urls</span> <span class="o">=</span> <span class="p">[</span><span class="n">url</span><span class="o">.</span><span class="n">strip</span><span class="p">(</span><span class="s2">&quot;/&quot;</span><span class="p">)</span> <span class="k">for</span> <span class="n">url</span> <span class="ow">in</span> <span class="n">args</span><span class="o">.</span><span class="n">urls</span><span class="p">]</span>
+</span><span id="get_args-262"><a href="#get_args-262"><span class="linenos">262</span></a>
+</span><span id="get_args-263"><a href="#get_args-263"><span class="linenos">263</span></a>    <span class="k">return</span> <span class="n">args</span>
 </span></pre></div>
 
 
     
 
                 </section>
                 <section id="main">
@@ -1127,23 +1123,23 @@
         <span class="def">def</span>
         <span class="name">main</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="main-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#main"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="main-268"><a href="#main-268"><span class="linenos">268</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="main-269"><a href="#main-269"><span class="linenos">269</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
-</span><span id="main-270"><a href="#main-270"><span class="linenos">270</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
-</span><span id="main-271"><a href="#main-271"><span class="linenos">271</span></a>    <span class="k">for</span> <span class="n">url</span> <span class="ow">in</span> <span class="n">args</span><span class="o">.</span><span class="n">urls</span><span class="p">:</span>
-</span><span id="main-272"><a href="#main-272"><span class="linenos">272</span></a>        <span class="k">if</span> <span class="n">page_is_discography</span><span class="p">(</span><span class="n">url</span><span class="p">):</span>
-</span><span id="main-273"><a href="#main-273"><span class="linenos">273</span></a>            <span class="n">ripper</span> <span class="o">=</span> <span class="n">BandRipper</span><span class="p">(</span><span class="n">url</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">no_track_number</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">overwrite</span><span class="p">)</span>
-</span><span id="main-274"><a href="#main-274"><span class="linenos">274</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="main-275"><a href="#main-275"><span class="linenos">275</span></a>            <span class="n">ripper</span> <span class="o">=</span> <span class="n">AlbumRipper</span><span class="p">(</span><span class="n">url</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">no_track_number</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">overwrite</span><span class="p">)</span>
-</span><span id="main-276"><a href="#main-276"><span class="linenos">276</span></a>        <span class="n">ripper</span><span class="o">.</span><span class="n">rip</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="main-266"><a href="#main-266"><span class="linenos">266</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="main-267"><a href="#main-267"><span class="linenos">267</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
+</span><span id="main-268"><a href="#main-268"><span class="linenos">268</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
+</span><span id="main-269"><a href="#main-269"><span class="linenos">269</span></a>    <span class="k">for</span> <span class="n">url</span> <span class="ow">in</span> <span class="n">args</span><span class="o">.</span><span class="n">urls</span><span class="p">:</span>
+</span><span id="main-270"><a href="#main-270"><span class="linenos">270</span></a>        <span class="k">if</span> <span class="n">page_is_discography</span><span class="p">(</span><span class="n">url</span><span class="p">):</span>
+</span><span id="main-271"><a href="#main-271"><span class="linenos">271</span></a>            <span class="n">ripper</span> <span class="o">=</span> <span class="n">BandRipper</span><span class="p">(</span><span class="n">url</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">no_track_number</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">overwrite</span><span class="p">)</span>
+</span><span id="main-272"><a href="#main-272"><span class="linenos">272</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="main-273"><a href="#main-273"><span class="linenos">273</span></a>            <span class="n">ripper</span> <span class="o">=</span> <span class="n">AlbumRipper</span><span class="p">(</span><span class="n">url</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">no_track_number</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">overwrite</span><span class="p">)</span>
+</span><span id="main-274"><a href="#main-274"><span class="linenos">274</span></a>        <span class="n">ripper</span><span class="o">.</span><span class="n">rip</span><span class="p">()</span>
 </span></pre></div>
 
 
     
 
                 </section>
     </main>
```

#### html2text {}

```diff
@@ -33,82 +33,370 @@
 __3import re
 __4import string
 __5from dataclasses import dataclass
 __6from pathlib import Path
 __7from urllib.parse import urlparse
 __8
 __9import requests
-_10from bs4 import BeautifulSoup
-_11
-_12import whosyouragent
-_13from noiftimer import Timer
-_14from printbuddies import ProgBar
-_15
-_16root = Path(__file__).parent
+_10import whosyouragent
+_11from bs4 import BeautifulSoup
+_12from noiftimer import Timer
+_13from printbuddies import ProgBar
+_14
+_15root = Path(__file__).parent
+_16
 _17
-_18
-_19def clean_string(text: str) -> str:
-_20    """Remove punctuation and trailing spaces from text."""
-_21    return re.sub(f"[{re.escape(string.punctuation)}]", "", text).strip()
+_18def clean_string(text: str) -> str:
+_19    """Remove punctuation and trailing spaces from text."""
+_20    return re.sub(f"[{re.escape(string.punctuation)}]", "", text).strip()
+_21
 _22
-_23
-_24@dataclass
-_25class Track:
-_26    title: str
-_27    number: int
-_28    url: str
-_29
-_30    def __post_init__(self):
-_31        self.title = clean_string(self.title)
-_32
-_33    @property
-_34    def numbered_title(self):
-_35        num = str(self.number)
-_36        if len(num) == 1:
-_37            num = "0" + num
-_38        return f"{num} - {self.title}"
+_23@dataclass
+_24class Track:
+_25    title: str
+_26    number: int
+_27    url: str
+_28
+_29    def __post_init__(self):
+_30        self.title = clean_string(self.title)
+_31
+_32    @property
+_33    def numbered_title(self):
+_34        num = str(self.number)
+_35        if len(num) == 1:
+_36            num = "0" + num
+_37        return f"{num} - {self.title}"
+_38
 _39
-_40
-_41@dataclass
-_42class Album:
-_43    url: str
-_44    artist: str = None
-_45    title: str = None
-_46    tracks: list[Track] = None
-_47    art_url: str = None
-_48
-_49    def __repr__(self):
-_50        return f"{self.title} by {self.artist}"
-_51
-_52    def __post_init__(self):
-_53        response = requests.get(self.url, headers=whosyouragent.get_agent
+_40@dataclass
+_41class Album:
+_42    url: str
+_43    artist: str = None
+_44    title: str = None
+_45    tracks: list[Track] = None
+_46    art_url: str = None
+_47
+_48    def __repr__(self):
+_49        return f"{self.title} by {self.artist}"
+_50
+_51    def __post_init__(self):
+_52        response = requests.get(self.url, headers=whosyouragent.get_agent
 (as_dict=True))
-_54        if response.status_code != 200:
-_55            raise RuntimeError(
-_56                f"Getting album info failed with code
+_53        if response.status_code != 200:
+_54            raise RuntimeError(
+_55                f"Getting album info failed with code
 {response.status_code}"
-_57            )
-_58        soup = BeautifulSoup(response.text, "html.parser")
-_59        self.art_url = soup.find("meta", attrs={"property": "og:image"}).get
+_56            )
+_57        soup = BeautifulSoup(response.text, "html.parser")
+_58        self.art_url = soup.find("meta", attrs={"property": "og:image"}).get
 ("content")
-_60        for script in soup.find_all("script"):
-_61            if script.get("data-cart"):
-_62                data = script
-_63                break
-_64        data = json.loads(data.attrs["data-tralbum"])
-_65        self.artist = clean_string(data["artist"])
-_66        self.title = clean_string(data["current"]["title"])
-_67        self.tracks = [
-_68            Track(track["title"], track["track_num"], track["file"]["mp3-
+_59        for script in soup.find_all("script"):
+_60            if script.get("data-cart"):
+_61                data = script
+_62                break
+_63        data = json.loads(data.attrs["data-tralbum"])
+_64        self.artist = clean_string(data["artist"])
+_65        self.title = clean_string(data["current"]["title"])
+_66        self.tracks = [
+_67            Track(track["title"], track["track_num"], track["file"]["mp3-
 128"])
-_69            for track in data["trackinfo"]
-_70            if track.get("file")
-_71        ]
+_68            for track in data["trackinfo"]
+_69            if track.get("file")
+_70        ]
+_71
 _72
-_73
+_73class AlbumRipper:
+_74    def __init__(
+_75        self, album_url: str, no_track_number: bool = False, overwrite: bool
+= False
+_76    ):
+_77        """
+_78        :param no_track_number: If True, don't add the track
+_79        number to the front of the track title."""
+_80        self.album = Album(album_url)
+_81        self.no_track_number = no_track_number
+_82        self.overwrite = overwrite
+_83
+_84    def make_save_path(self):
+_85        self.save_path = Path.cwd() / self.album.artist / self.album.title
+_86        self.save_path.mkdir(parents=True, exist_ok=True)
+_87
+_88    @property
+_89    def headers(self) -> dict:
+_90        """Get a headers dict with a random useragent."""
+_91        return whosyouragent.get_agent(as_dict=True)
+_92
+_93    def save_track(self, track_title: str, content: bytes) -> Path:
+_94        """Save track to self.save_path/{track_title}.mp3.
+_95        Returns the Path object for the save location.
+_96
+_97        :param content: The binary data of the track."""
+_98        file_path = self.save_path / f"{track_title}.mp3"
+_99        file_path.write_bytes(content)
+100        return file_path
+101
+102    def get_track_content(self, track_url: str) -> bytes:
+103        """Make a request to track_url and return the content.
+104        Raises a RunTimeError exception if response.status_code != 200."""
+105        response = requests.get(track_url, headers=self.headers)
+106        if response.status_code != 200:
+107            raise RuntimeError(
+108                f"Downloading track failed with status code
+{response.status_code}."
+109            )
+110        return response.content
+111
+112    def download_album_art(self):
+113        """Download the album art and save as a .jpg."""
+114        file_path = self.save_path / f"{self.album.title}.jpg"
+115        try:
+116            response = requests.get(self.album.art_url,
+headers=self.headers)
+117            file_path.write_bytes(response.content)
+118        except Exception as e:
+119            print(f"Failed to download art for {self.album}.")
+120            print(e)
+121
+122    def track_exists(self, track: Track) -> bool:
+123        """Return if a track already exists in self.save_path."""
+124        path = self.save_path / (
+125            track.title if self.no_track_number else track.numbered_title
+126        )
+127        return path.with_suffix(".mp3").exists()
+128
+129    def rip(self):
+130        """Download and save the album tracks and album art."""
+131        if len(self.album.tracks) == 0:
+132            print(f"No public tracks available for {self.album}.")
+133            return None
+134        self.make_save_path()
+135        self.download_album_art()
+136        bar = ProgBar(len(self.album.tracks) - 1, width_ratio=0.5)
+137        fails = []
+138        if not self.overwrite:
+139            self.album.tracks = [
+140                track for track in self.album.tracks if not
+self.track_exists(track)
+141            ]
+142        for track in self.album.tracks:
+143            bar.display(
+144                suffix=f"Downloading {track.title}",
+145                counter_override=1 if len(self.album.tracks) == 1 else None,
+146            )
+147            try:
+148                content = self.get_track_content(track.url)
+149                self.save_track(
+150                    track.title if self.no_track_number else
+track.numbered_title,
+151                    content,
+152                )
+153            except Exception as e:
+154                fails.append((track, str(e)))
+155        print(f"Finished downloading {self.album} in
+{bar.timer.elapsed_str}.")
+156        if fails:
+157            print("The following tracks failed to download:")
+158            for fail in fails:
+159                print(f"{fail[0].title}: {fail[1]}")
+160
+161
+162class BandRipper:
+163    def __init__(
+164        self, band_url: str, no_track_number: bool = False, overwrite: bool
+= False
+165    ):
+166        self.band_url = band_url
+167        self.albums = []
+168        for url in self.get_album_urls(band_url):
+169            try:
+170                self.albums.append(AlbumRipper(url, no_track_number,
+overwrite))
+171            except Exception as e:
+172                print(e)
+173
+174    def get_album_urls(self, band_url: str) -> list[str]:
+175        """Get album urls from the main bandcamp url."""
+176        print(f"Fetching discography from {band_url}...")
+177        response = requests.get(band_url, headers=whosyouragent.get_agent
+(as_dict=True))
+178        if response.status_code != 200:
+179            raise RuntimeError(
+180                f"Getting {band_url} failed with status code
+{response.status_code}."
+181            )
+182        soup = BeautifulSoup(response.text, "html.parser")
+183        grid = soup.find("ol", attrs={"id": "music-grid"})
+184        parsed_url = urlparse(band_url)
+185        base_url = f"https://{parsed_url.netloc}"
+186        return [base_url + album.a.get("href") for album in grid.find_all
+("li")]
+187
+188    def rip(self):
+189        print(
+190            f"Downloading {len(self.albums)} albums by {self.albums
+[0].album.artist}."
+191        )
+192        timer = Timer(subsecond_resolution=True)
+193        timer.start()
+194        fails = []
+195        for album in self.albums:
+196            try:
+197                album.rip()
+198            except Exception as e:
+199                fails.append((album, e))
+200        timer.stop()
+201        artist = self.albums[0].album.artist
+202        print(
+203            f"Finished downloading {len(self.albums)} albums by {artist} in
+{timer.elapsed_str}."
+204        )
+205        if fails:
+206            print(f"The following downloads failed:")
+207            for fail in fails:
+208                print(f"{fail[0]}: {fail[1]}")
+209
+210
+211def page_is_discography(url: str) -> bool:
+212    """Returns whether the url is to a discography page or not."""
+213    response = requests.get(url, headers=whosyouragent.get_agent
+(as_dict=True))
+214    if response.status_code != 200:
+215        raise RuntimeError(
+216            f"Getting {url} failed with status code {response.status_code}."
+217        )
+218    soup = BeautifulSoup(response.text, "html.parser")
+219    # Returns None if it doesn't exist.
+220    grid = soup.find("ol", attrs={"id": "music-grid"})
+221    if grid:
+222        return True
+223    return False
+224
+225
+226def get_args() -> argparse.Namespace:
+227    parser = argparse.ArgumentParser()
+228
+229    parser.add_argument(
+230        "urls",
+231        type=str,
+232        nargs="*",
+233        help=""" The bandcamp url(s) for the album or artist.
+234            If the url is to an artists main page,
+235            all albums will be downloaded.
+236            The tracks will be saved to a subdirectory of
+237            your current directory.
+238            If a track can't be streamed (i.e. private) it
+239            won't be downloaded. Multiple urls can be passed.""",
+240    )
+241
+242    parser.add_argument(
+243        "-n",
+244        "--no_track_number",
+245        action="store_true",
+246        help=""" By default the track number will be added
+247        to the front of the track title. Pass this switch
+248        to disable the behavior.""",
+249    )
+250
+251    parser.add_argument(
+252        "-o",
+253        "--overwrite",
+254        action="store_true",
+255        help=""" Pass this flag to overwrite existing files.
+256        Otherwise don't download tracks that already exist locally.""",
+257    )
+258
+259    args = parser.parse_args()
+260    args.urls = [url.strip("/") for url in args.urls]
+261
+262    return args
+263
+264
+265def main(args: argparse.Namespace = None):
+266    if not args:
+267        args = get_args()
+268    for url in args.urls:
+269        if page_is_discography(url):
+270            ripper = BandRipper(url, args.no_track_number, args.overwrite)
+271        else:
+272            ripper = AlbumRipper(url, args.no_track_number, args.overwrite)
+273        ripper.rip()
+274
+275
+276if __name__ == "__main__":
+277    main(get_args())
+  ⁰
+def clean_string(text: str) -> str: View Source
+19def clean_string(text: str) -> str:
+20    """Remove punctuation and trailing spaces from text."""
+21    return re.sub(f"[{re.escape(string.punctuation)}]", "", text).strip()
+Remove punctuation and trailing spaces from text.
+  ⁰
+@dataclass
+class Track: View Source
+24@dataclass
+25class Track:
+26    title: str
+27    number: int
+28    url: str
+29
+30    def __post_init__(self):
+31        self.title = clean_string(self.title)
+32
+33    @property
+34    def numbered_title(self):
+35        num = str(self.number)
+36        if len(num) == 1:
+37            num = "0" + num
+38        return f"{num} - {self.title}"
+Track(title: str, number: int, url: str)
+  ⁰
+@dataclass
+class Album: View Source
+41@dataclass
+42class Album:
+43    url: str
+44    artist: str = None
+45    title: str = None
+46    tracks: list[Track] = None
+47    art_url: str = None
+48
+49    def __repr__(self):
+50        return f"{self.title} by {self.artist}"
+51
+52    def __post_init__(self):
+53        response = requests.get(self.url, headers=whosyouragent.get_agent
+(as_dict=True))
+54        if response.status_code != 200:
+55            raise RuntimeError(
+56                f"Getting album info failed with code {response.status_code}"
+57            )
+58        soup = BeautifulSoup(response.text, "html.parser")
+59        self.art_url = soup.find("meta", attrs={"property": "og:image"}).get
+("content")
+60        for script in soup.find_all("script"):
+61            if script.get("data-cart"):
+62                data = script
+63                break
+64        data = json.loads(data.attrs["data-tralbum"])
+65        self.artist = clean_string(data["artist"])
+66        self.title = clean_string(data["current"]["title"])
+67        self.tracks = [
+68            Track(track["title"], track["track_num"], track["file"]["mp3-
+128"])
+69            for track in data["trackinfo"]
+70            if track.get("file")
+71        ]
+Album(
+url: str,
+artist: str = None,
+title: str = None,
+tracks: list[bandripper.bandripper.Track] = None,
+art_url: str = None)
+  ⁰
+class AlbumRipper: View Source
 _74class AlbumRipper:
 _75    def __init__(
 _76        self, album_url: str, no_track_number: bool = False, overwrite: bool
 = False
 _77    ):
 _78        """
 _79        :param no_track_number: If True, don't add the track
@@ -168,623 +456,331 @@
 131        """Download and save the album tracks and album art."""
 132        if len(self.album.tracks) == 0:
 133            print(f"No public tracks available for {self.album}.")
 134            return None
 135        self.make_save_path()
 136        self.download_album_art()
 137        bar = ProgBar(len(self.album.tracks) - 1, width_ratio=0.5)
-138        bar.timer.subsecond_resolution = True
-139        fails = []
-140        if not self.overwrite:
-141            self.album.tracks = [
-142                track for track in self.album.tracks if not
-self.track_exists(track)
-143            ]
-144        for track in self.album.tracks:
-145            bar.display(
-146                suffix=f"Downloading {track.title}",
-147                counter_override=1 if len(self.album.tracks) == 1 else None,
-148            )
-149            try:
-150                content = self.get_track_content(track.url)
-151                self.save_track(
-152                    track.title if self.no_track_number else
-track.numbered_title,
-153                    content,
-154                )
-155            except Exception as e:
-156                fails.append((track, str(e)))
-157        print(f"Finished downloading {self.album} in
-{bar.timer.elapsed_str}.")
-158        if fails:
-159            print("The following tracks failed to download:")
-160            for fail in fails:
-161                print(f"{fail[0].title}: {fail[1]}")
-162
-163
-164class BandRipper:
-165    def __init__(
-166        self, band_url: str, no_track_number: bool = False, overwrite: bool
-= False
-167    ):
-168        self.band_url = band_url
-169        self.albums = []
-170        for url in self.get_album_urls(band_url):
-171            try:
-172                self.albums.append(AlbumRipper(url, no_track_number,
-overwrite))
-173            except Exception as e:
-174                print(e)
-175
-176    def get_album_urls(self, band_url: str) -> list[str]:
-177        """Get album urls from the main bandcamp url."""
-178        print(f"Fetching discography from {band_url}...")
-179        response = requests.get(band_url, headers=whosyouragent.get_agent
-(as_dict=True))
-180        if response.status_code != 200:
-181            raise RuntimeError(
-182                f"Getting {band_url} failed with status code
-{response.status_code}."
-183            )
-184        soup = BeautifulSoup(response.text, "html.parser")
-185        grid = soup.find("ol", attrs={"id": "music-grid"})
-186        parsed_url = urlparse(band_url)
-187        base_url = f"https://{parsed_url.netloc}"
-188        return [base_url + album.a.get("href") for album in grid.find_all
-("li")]
-189
-190    def rip(self):
-191        print(
-192            f"Downloading {len(self.albums)} albums by {self.albums
-[0].album.artist}."
-193        )
-194        timer = Timer(subsecond_resolution=True)
-195        timer.start()
-196        fails = []
-197        for album in self.albums:
-198            try:
-199                album.rip()
-200            except Exception as e:
-201                fails.append((album, e))
-202        timer.stop()
-203        artist = self.albums[0].album.artist
-204        print(
-205            f"Finished downloading {len(self.albums)} albums by {artist} in
-{timer.elapsed_str}."
-206        )
-207        if fails:
-208            print(f"The following downloads failed:")
-209            for fail in fails:
-210                print(f"{fail[0]}: {fail[1]}")
-211
-212
-213def page_is_discography(url: str) -> bool:
-214    """Returns whether the url is to a discography page or not."""
-215    response = requests.get(url, headers=whosyouragent.get_agent
-(as_dict=True))
-216    if response.status_code != 200:
-217        raise RuntimeError(
-218            f"Getting {url} failed with status code {response.status_code}."
-219        )
-220    soup = BeautifulSoup(response.text, "html.parser")
-221    # Returns None if it doesn't exist.
-222    grid = soup.find("ol", attrs={"id": "music-grid"})
-223    if grid:
-224        return True
-225    return False
-226
-227
-228def get_args() -> argparse.Namespace:
-229    parser = argparse.ArgumentParser()
-230
-231    parser.add_argument(
-232        "urls",
-233        type=str,
-234        nargs="*",
-235        help=""" The bandcamp url(s) for the album or artist.
-236            If the url is to an artists main page,
-237            all albums will be downloaded.
-238            The tracks will be saved to a subdirectory of
-239            your current directory.
-240            If a track can't be streamed (i.e. private) it
-241            won't be downloaded. Multiple urls can be passed.""",
-242    )
-243
-244    parser.add_argument(
-245        "-n",
-246        "--no_track_number",
-247        action="store_true",
-248        help=""" By default the track number will be added
-249        to the front of the track title. Pass this switch
-250        to disable the behavior.""",
-251    )
-252
-253    parser.add_argument(
-254        "-o",
-255        "--overwrite",
-256        action="store_true",
-257        help=""" Pass this flag to overwrite existing files.
-258        Otherwise don't download tracks that already exist locally.""",
-259    )
-260
-261    args = parser.parse_args()
-262    args.urls = [url.strip("/") for url in args.urls]
-263
-264    return args
-265
-266
-267def main(args: argparse.Namespace = None):
-268    if not args:
-269        args = get_args()
-270    for url in args.urls:
-271        if page_is_discography(url):
-272            ripper = BandRipper(url, args.no_track_number, args.overwrite)
-273        else:
-274            ripper = AlbumRipper(url, args.no_track_number, args.overwrite)
-275        ripper.rip()
-276
-277
-278if __name__ == "__main__":
-279    main(get_args())
-  ⁰
-def clean_string(text: str) -> str: View Source
-20def clean_string(text: str) -> str:
-21    """Remove punctuation and trailing spaces from text."""
-22    return re.sub(f"[{re.escape(string.punctuation)}]", "", text).strip()
-Remove punctuation and trailing spaces from text.
-  ⁰
-@dataclass
-class Track: View Source
-25@dataclass
-26class Track:
-27    title: str
-28    number: int
-29    url: str
-30
-31    def __post_init__(self):
-32        self.title = clean_string(self.title)
-33
-34    @property
-35    def numbered_title(self):
-36        num = str(self.number)
-37        if len(num) == 1:
-38            num = "0" + num
-39        return f"{num} - {self.title}"
-Track(title: str, number: int, url: str)
-  ⁰
-@dataclass
-class Album: View Source
-42@dataclass
-43class Album:
-44    url: str
-45    artist: str = None
-46    title: str = None
-47    tracks: list[Track] = None
-48    art_url: str = None
-49
-50    def __repr__(self):
-51        return f"{self.title} by {self.artist}"
-52
-53    def __post_init__(self):
-54        response = requests.get(self.url, headers=whosyouragent.get_agent
-(as_dict=True))
-55        if response.status_code != 200:
-56            raise RuntimeError(
-57                f"Getting album info failed with code {response.status_code}"
-58            )
-59        soup = BeautifulSoup(response.text, "html.parser")
-60        self.art_url = soup.find("meta", attrs={"property": "og:image"}).get
-("content")
-61        for script in soup.find_all("script"):
-62            if script.get("data-cart"):
-63                data = script
-64                break
-65        data = json.loads(data.attrs["data-tralbum"])
-66        self.artist = clean_string(data["artist"])
-67        self.title = clean_string(data["current"]["title"])
-68        self.tracks = [
-69            Track(track["title"], track["track_num"], track["file"]["mp3-
-128"])
-70            for track in data["trackinfo"]
-71            if track.get("file")
-72        ]
-Album(
-url: str,
-artist: str = None,
-title: str = None,
-tracks: list[bandripper.bandripper.Track] = None,
-art_url: str = None)
-  ⁰
-class AlbumRipper: View Source
-_75class AlbumRipper:
-_76    def __init__(
-_77        self, album_url: str, no_track_number: bool = False, overwrite: bool
-= False
-_78    ):
-_79        """
-_80        :param no_track_number: If True, don't add the track
-_81        number to the front of the track title."""
-_82        self.album = Album(album_url)
-_83        self.no_track_number = no_track_number
-_84        self.overwrite = overwrite
-_85
-_86    def make_save_path(self):
-_87        self.save_path = Path.cwd() / self.album.artist / self.album.title
-_88        self.save_path.mkdir(parents=True, exist_ok=True)
-_89
-_90    @property
-_91    def headers(self) -> dict:
-_92        """Get a headers dict with a random useragent."""
-_93        return whosyouragent.get_agent(as_dict=True)
-_94
-_95    def save_track(self, track_title: str, content: bytes) -> Path:
-_96        """Save track to self.save_path/{track_title}.mp3.
-_97        Returns the Path object for the save location.
-_98
-_99        :param content: The binary data of the track."""
-100        file_path = self.save_path / f"{track_title}.mp3"
-101        file_path.write_bytes(content)
-102        return file_path
-103
-104    def get_track_content(self, track_url: str) -> bytes:
-105        """Make a request to track_url and return the content.
-106        Raises a RunTimeError exception if response.status_code != 200."""
-107        response = requests.get(track_url, headers=self.headers)
-108        if response.status_code != 200:
-109            raise RuntimeError(
-110                f"Downloading track failed with status code
-{response.status_code}."
-111            )
-112        return response.content
-113
-114    def download_album_art(self):
-115        """Download the album art and save as a .jpg."""
-116        file_path = self.save_path / f"{self.album.title}.jpg"
-117        try:
-118            response = requests.get(self.album.art_url,
-headers=self.headers)
-119            file_path.write_bytes(response.content)
-120        except Exception as e:
-121            print(f"Failed to download art for {self.album}.")
-122            print(e)
-123
-124    def track_exists(self, track: Track) -> bool:
-125        """Return if a track already exists in self.save_path."""
-126        path = self.save_path / (
-127            track.title if self.no_track_number else track.numbered_title
-128        )
-129        return path.with_suffix(".mp3").exists()
-130
-131    def rip(self):
-132        """Download and save the album tracks and album art."""
-133        if len(self.album.tracks) == 0:
-134            print(f"No public tracks available for {self.album}.")
-135            return None
-136        self.make_save_path()
-137        self.download_album_art()
-138        bar = ProgBar(len(self.album.tracks) - 1, width_ratio=0.5)
-139        bar.timer.subsecond_resolution = True
-140        fails = []
-141        if not self.overwrite:
-142            self.album.tracks = [
-143                track for track in self.album.tracks if not
+138        fails = []
+139        if not self.overwrite:
+140            self.album.tracks = [
+141                track for track in self.album.tracks if not
 self.track_exists(track)
-144            ]
-145        for track in self.album.tracks:
-146            bar.display(
-147                suffix=f"Downloading {track.title}",
-148                counter_override=1 if len(self.album.tracks) == 1 else None,
-149            )
-150            try:
-151                content = self.get_track_content(track.url)
-152                self.save_track(
-153                    track.title if self.no_track_number else
+142            ]
+143        for track in self.album.tracks:
+144            bar.display(
+145                suffix=f"Downloading {track.title}",
+146                counter_override=1 if len(self.album.tracks) == 1 else None,
+147            )
+148            try:
+149                content = self.get_track_content(track.url)
+150                self.save_track(
+151                    track.title if self.no_track_number else
 track.numbered_title,
-154                    content,
-155                )
-156            except Exception as e:
-157                fails.append((track, str(e)))
-158        print(f"Finished downloading {self.album} in
+152                    content,
+153                )
+154            except Exception as e:
+155                fails.append((track, str(e)))
+156        print(f"Finished downloading {self.album} in
 {bar.timer.elapsed_str}.")
-159        if fails:
-160            print("The following tracks failed to download:")
-161            for fail in fails:
-162                print(f"{fail[0].title}: {fail[1]}")
+157        if fails:
+158            print("The following tracks failed to download:")
+159            for fail in fails:
+160                print(f"{fail[0].title}: {fail[1]}")
 ⁰
 AlbumRipper(
 album_url: str,
 no_track_number: bool = False,
 overwrite: bool = False) View Source
-76    def __init__(
-77        self, album_url: str, no_track_number: bool = False, overwrite: bool
+75    def __init__(
+76        self, album_url: str, no_track_number: bool = False, overwrite: bool
 = False
-78    ):
-79        """
-80        :param no_track_number: If True, don't add the track
-81        number to the front of the track title."""
-82        self.album = Album(album_url)
-83        self.no_track_number = no_track_number
-84        self.overwrite = overwrite
+77    ):
+78        """
+79        :param no_track_number: If True, don't add the track
+80        number to the front of the track title."""
+81        self.album = Album(album_url)
+82        self.no_track_number = no_track_number
+83        self.overwrite = overwrite
 * Parameters *
     * no_track_number: If True, don't add the track number to the front of the
       track title.
 ⁰
 def make_save_path(self): View Source
-86    def make_save_path(self):
-87        self.save_path = Path.cwd() / self.album.artist / self.album.title
-88        self.save_path.mkdir(parents=True, exist_ok=True)
+85    def make_save_path(self):
+86        self.save_path = Path.cwd() / self.album.artist / self.album.title
+87        self.save_path.mkdir(parents=True, exist_ok=True)
 headers: dict
 Get a headers dict with a random useragent.
 ⁰
 def save_track(self, track_title: str, content: bytes) -> pathlib.Path: View
 Source
-_95    def save_track(self, track_title: str, content: bytes) -> Path:
-_96        """Save track to self.save_path/{track_title}.mp3.
-_97        Returns the Path object for the save location.
-_98
-_99        :param content: The binary data of the track."""
-100        file_path = self.save_path / f"{track_title}.mp3"
-101        file_path.write_bytes(content)
-102        return file_path
+_94    def save_track(self, track_title: str, content: bytes) -> Path:
+_95        """Save track to self.save_path/{track_title}.mp3.
+_96        Returns the Path object for the save location.
+_97
+_98        :param content: The binary data of the track."""
+_99        file_path = self.save_path / f"{track_title}.mp3"
+100        file_path.write_bytes(content)
+101        return file_path
 Save track to self.save_path/{track_title}.mp3. Returns the Path object for the
 save location.
 * Parameters *
     * content: The binary data of the track.
 ⁰
 def get_track_content(self, track_url: str) -> bytes: View Source
-104    def get_track_content(self, track_url: str) -> bytes:
-105        """Make a request to track_url and return the content.
-106        Raises a RunTimeError exception if response.status_code != 200."""
-107        response = requests.get(track_url, headers=self.headers)
-108        if response.status_code != 200:
-109            raise RuntimeError(
-110                f"Downloading track failed with status code
+103    def get_track_content(self, track_url: str) -> bytes:
+104        """Make a request to track_url and return the content.
+105        Raises a RunTimeError exception if response.status_code != 200."""
+106        response = requests.get(track_url, headers=self.headers)
+107        if response.status_code != 200:
+108            raise RuntimeError(
+109                f"Downloading track failed with status code
 {response.status_code}."
-111            )
-112        return response.content
+110            )
+111        return response.content
 Make a request to track_url and return the content. Raises a RunTimeError
 exception if response.status_code != 200.
 ⁰
 def download_album_art(self): View Source
-114    def download_album_art(self):
-115        """Download the album art and save as a .jpg."""
-116        file_path = self.save_path / f"{self.album.title}.jpg"
-117        try:
-118            response = requests.get(self.album.art_url,
+113    def download_album_art(self):
+114        """Download the album art and save as a .jpg."""
+115        file_path = self.save_path / f"{self.album.title}.jpg"
+116        try:
+117            response = requests.get(self.album.art_url,
 headers=self.headers)
-119            file_path.write_bytes(response.content)
-120        except Exception as e:
-121            print(f"Failed to download art for {self.album}.")
-122            print(e)
+118            file_path.write_bytes(response.content)
+119        except Exception as e:
+120            print(f"Failed to download art for {self.album}.")
+121            print(e)
 Download the album art and save as a .jpg.
 ⁰
 def track_exists(self, track: bandripper.bandripper.Track) -> bool: View Source
-124    def track_exists(self, track: Track) -> bool:
-125        """Return if a track already exists in self.save_path."""
-126        path = self.save_path / (
-127            track.title if self.no_track_number else track.numbered_title
-128        )
-129        return path.with_suffix(".mp3").exists()
+123    def track_exists(self, track: Track) -> bool:
+124        """Return if a track already exists in self.save_path."""
+125        path = self.save_path / (
+126            track.title if self.no_track_number else track.numbered_title
+127        )
+128        return path.with_suffix(".mp3").exists()
 Return if a track already exists in self.save_path.
 ⁰
 def rip(self): View Source
-131    def rip(self):
-132        """Download and save the album tracks and album art."""
-133        if len(self.album.tracks) == 0:
-134            print(f"No public tracks available for {self.album}.")
-135            return None
-136        self.make_save_path()
-137        self.download_album_art()
-138        bar = ProgBar(len(self.album.tracks) - 1, width_ratio=0.5)
-139        bar.timer.subsecond_resolution = True
-140        fails = []
-141        if not self.overwrite:
-142            self.album.tracks = [
-143                track for track in self.album.tracks if not
+130    def rip(self):
+131        """Download and save the album tracks and album art."""
+132        if len(self.album.tracks) == 0:
+133            print(f"No public tracks available for {self.album}.")
+134            return None
+135        self.make_save_path()
+136        self.download_album_art()
+137        bar = ProgBar(len(self.album.tracks) - 1, width_ratio=0.5)
+138        fails = []
+139        if not self.overwrite:
+140            self.album.tracks = [
+141                track for track in self.album.tracks if not
 self.track_exists(track)
-144            ]
-145        for track in self.album.tracks:
-146            bar.display(
-147                suffix=f"Downloading {track.title}",
-148                counter_override=1 if len(self.album.tracks) == 1 else None,
-149            )
-150            try:
-151                content = self.get_track_content(track.url)
-152                self.save_track(
-153                    track.title if self.no_track_number else
+142            ]
+143        for track in self.album.tracks:
+144            bar.display(
+145                suffix=f"Downloading {track.title}",
+146                counter_override=1 if len(self.album.tracks) == 1 else None,
+147            )
+148            try:
+149                content = self.get_track_content(track.url)
+150                self.save_track(
+151                    track.title if self.no_track_number else
 track.numbered_title,
-154                    content,
-155                )
-156            except Exception as e:
-157                fails.append((track, str(e)))
-158        print(f"Finished downloading {self.album} in
+152                    content,
+153                )
+154            except Exception as e:
+155                fails.append((track, str(e)))
+156        print(f"Finished downloading {self.album} in
 {bar.timer.elapsed_str}.")
-159        if fails:
-160            print("The following tracks failed to download:")
-161            for fail in fails:
-162                print(f"{fail[0].title}: {fail[1]}")
+157        if fails:
+158            print("The following tracks failed to download:")
+159            for fail in fails:
+160                print(f"{fail[0].title}: {fail[1]}")
 Download and save the album tracks and album art.
   ⁰
 class BandRipper: View Source
-165class BandRipper:
-166    def __init__(
-167        self, band_url: str, no_track_number: bool = False, overwrite: bool
+163class BandRipper:
+164    def __init__(
+165        self, band_url: str, no_track_number: bool = False, overwrite: bool
 = False
-168    ):
-169        self.band_url = band_url
-170        self.albums = []
-171        for url in self.get_album_urls(band_url):
-172            try:
-173                self.albums.append(AlbumRipper(url, no_track_number,
+166    ):
+167        self.band_url = band_url
+168        self.albums = []
+169        for url in self.get_album_urls(band_url):
+170            try:
+171                self.albums.append(AlbumRipper(url, no_track_number,
 overwrite))
-174            except Exception as e:
-175                print(e)
-176
-177    def get_album_urls(self, band_url: str) -> list[str]:
-178        """Get album urls from the main bandcamp url."""
-179        print(f"Fetching discography from {band_url}...")
-180        response = requests.get(band_url, headers=whosyouragent.get_agent
+172            except Exception as e:
+173                print(e)
+174
+175    def get_album_urls(self, band_url: str) -> list[str]:
+176        """Get album urls from the main bandcamp url."""
+177        print(f"Fetching discography from {band_url}...")
+178        response = requests.get(band_url, headers=whosyouragent.get_agent
 (as_dict=True))
-181        if response.status_code != 200:
-182            raise RuntimeError(
-183                f"Getting {band_url} failed with status code
+179        if response.status_code != 200:
+180            raise RuntimeError(
+181                f"Getting {band_url} failed with status code
 {response.status_code}."
-184            )
-185        soup = BeautifulSoup(response.text, "html.parser")
-186        grid = soup.find("ol", attrs={"id": "music-grid"})
-187        parsed_url = urlparse(band_url)
-188        base_url = f"https://{parsed_url.netloc}"
-189        return [base_url + album.a.get("href") for album in grid.find_all
+182            )
+183        soup = BeautifulSoup(response.text, "html.parser")
+184        grid = soup.find("ol", attrs={"id": "music-grid"})
+185        parsed_url = urlparse(band_url)
+186        base_url = f"https://{parsed_url.netloc}"
+187        return [base_url + album.a.get("href") for album in grid.find_all
 ("li")]
-190
-191    def rip(self):
-192        print(
-193            f"Downloading {len(self.albums)} albums by {self.albums
+188
+189    def rip(self):
+190        print(
+191            f"Downloading {len(self.albums)} albums by {self.albums
 [0].album.artist}."
-194        )
-195        timer = Timer(subsecond_resolution=True)
-196        timer.start()
-197        fails = []
-198        for album in self.albums:
-199            try:
-200                album.rip()
-201            except Exception as e:
-202                fails.append((album, e))
-203        timer.stop()
-204        artist = self.albums[0].album.artist
-205        print(
-206            f"Finished downloading {len(self.albums)} albums by {artist} in
+192        )
+193        timer = Timer(subsecond_resolution=True)
+194        timer.start()
+195        fails = []
+196        for album in self.albums:
+197            try:
+198                album.rip()
+199            except Exception as e:
+200                fails.append((album, e))
+201        timer.stop()
+202        artist = self.albums[0].album.artist
+203        print(
+204            f"Finished downloading {len(self.albums)} albums by {artist} in
 {timer.elapsed_str}."
-207        )
-208        if fails:
-209            print(f"The following downloads failed:")
-210            for fail in fails:
-211                print(f"{fail[0]}: {fail[1]}")
+205        )
+206        if fails:
+207            print(f"The following downloads failed:")
+208            for fail in fails:
+209                print(f"{fail[0]}: {fail[1]}")
 ⁰
 BandRipper(
 band_url: str,
 no_track_number: bool = False,
 overwrite: bool = False) View Source
-166    def __init__(
-167        self, band_url: str, no_track_number: bool = False, overwrite: bool
+164    def __init__(
+165        self, band_url: str, no_track_number: bool = False, overwrite: bool
 = False
-168    ):
-169        self.band_url = band_url
-170        self.albums = []
-171        for url in self.get_album_urls(band_url):
-172            try:
-173                self.albums.append(AlbumRipper(url, no_track_number,
+166    ):
+167        self.band_url = band_url
+168        self.albums = []
+169        for url in self.get_album_urls(band_url):
+170            try:
+171                self.albums.append(AlbumRipper(url, no_track_number,
 overwrite))
-174            except Exception as e:
-175                print(e)
+172            except Exception as e:
+173                print(e)
 ⁰
 def get_album_urls(self, band_url: str) -> list[str]: View Source
-177    def get_album_urls(self, band_url: str) -> list[str]:
-178        """Get album urls from the main bandcamp url."""
-179        print(f"Fetching discography from {band_url}...")
-180        response = requests.get(band_url, headers=whosyouragent.get_agent
+175    def get_album_urls(self, band_url: str) -> list[str]:
+176        """Get album urls from the main bandcamp url."""
+177        print(f"Fetching discography from {band_url}...")
+178        response = requests.get(band_url, headers=whosyouragent.get_agent
 (as_dict=True))
-181        if response.status_code != 200:
-182            raise RuntimeError(
-183                f"Getting {band_url} failed with status code
+179        if response.status_code != 200:
+180            raise RuntimeError(
+181                f"Getting {band_url} failed with status code
 {response.status_code}."
-184            )
-185        soup = BeautifulSoup(response.text, "html.parser")
-186        grid = soup.find("ol", attrs={"id": "music-grid"})
-187        parsed_url = urlparse(band_url)
-188        base_url = f"https://{parsed_url.netloc}"
-189        return [base_url + album.a.get("href") for album in grid.find_all
+182            )
+183        soup = BeautifulSoup(response.text, "html.parser")
+184        grid = soup.find("ol", attrs={"id": "music-grid"})
+185        parsed_url = urlparse(band_url)
+186        base_url = f"https://{parsed_url.netloc}"
+187        return [base_url + album.a.get("href") for album in grid.find_all
 ("li")]
 Get album urls from the main bandcamp url.
 ⁰
 def rip(self): View Source
-191    def rip(self):
-192        print(
-193            f"Downloading {len(self.albums)} albums by {self.albums
+189    def rip(self):
+190        print(
+191            f"Downloading {len(self.albums)} albums by {self.albums
 [0].album.artist}."
-194        )
-195        timer = Timer(subsecond_resolution=True)
-196        timer.start()
-197        fails = []
-198        for album in self.albums:
-199            try:
-200                album.rip()
-201            except Exception as e:
-202                fails.append((album, e))
-203        timer.stop()
-204        artist = self.albums[0].album.artist
-205        print(
-206            f"Finished downloading {len(self.albums)} albums by {artist} in
+192        )
+193        timer = Timer(subsecond_resolution=True)
+194        timer.start()
+195        fails = []
+196        for album in self.albums:
+197            try:
+198                album.rip()
+199            except Exception as e:
+200                fails.append((album, e))
+201        timer.stop()
+202        artist = self.albums[0].album.artist
+203        print(
+204            f"Finished downloading {len(self.albums)} albums by {artist} in
 {timer.elapsed_str}."
-207        )
-208        if fails:
-209            print(f"The following downloads failed:")
-210            for fail in fails:
-211                print(f"{fail[0]}: {fail[1]}")
+205        )
+206        if fails:
+207            print(f"The following downloads failed:")
+208            for fail in fails:
+209                print(f"{fail[0]}: {fail[1]}")
   ⁰
 def page_is_discography(url: str) -> bool: View Source
-214def page_is_discography(url: str) -> bool:
-215    """Returns whether the url is to a discography page or not."""
-216    response = requests.get(url, headers=whosyouragent.get_agent
+212def page_is_discography(url: str) -> bool:
+213    """Returns whether the url is to a discography page or not."""
+214    response = requests.get(url, headers=whosyouragent.get_agent
 (as_dict=True))
-217    if response.status_code != 200:
-218        raise RuntimeError(
-219            f"Getting {url} failed with status code {response.status_code}."
-220        )
-221    soup = BeautifulSoup(response.text, "html.parser")
-222    # Returns None if it doesn't exist.
-223    grid = soup.find("ol", attrs={"id": "music-grid"})
-224    if grid:
-225        return True
-226    return False
+215    if response.status_code != 200:
+216        raise RuntimeError(
+217            f"Getting {url} failed with status code {response.status_code}."
+218        )
+219    soup = BeautifulSoup(response.text, "html.parser")
+220    # Returns None if it doesn't exist.
+221    grid = soup.find("ol", attrs={"id": "music-grid"})
+222    if grid:
+223        return True
+224    return False
 Returns whether the url is to a discography page or not.
   ⁰
 def get_args() -> argparse.Namespace: View Source
-229def get_args() -> argparse.Namespace:
-230    parser = argparse.ArgumentParser()
-231
-232    parser.add_argument(
-233        "urls",
-234        type=str,
-235        nargs="*",
-236        help=""" The bandcamp url(s) for the album or artist.
-237            If the url is to an artists main page,
-238            all albums will be downloaded.
-239            The tracks will be saved to a subdirectory of
-240            your current directory.
-241            If a track can't be streamed (i.e. private) it
-242            won't be downloaded. Multiple urls can be passed.""",
-243    )
-244
-245    parser.add_argument(
-246        "-n",
-247        "--no_track_number",
-248        action="store_true",
-249        help=""" By default the track number will be added
-250        to the front of the track title. Pass this switch
-251        to disable the behavior.""",
-252    )
-253
-254    parser.add_argument(
-255        "-o",
-256        "--overwrite",
-257        action="store_true",
-258        help=""" Pass this flag to overwrite existing files.
-259        Otherwise don't download tracks that already exist locally.""",
-260    )
-261
-262    args = parser.parse_args()
-263    args.urls = [url.strip("/") for url in args.urls]
-264
-265    return args
+227def get_args() -> argparse.Namespace:
+228    parser = argparse.ArgumentParser()
+229
+230    parser.add_argument(
+231        "urls",
+232        type=str,
+233        nargs="*",
+234        help=""" The bandcamp url(s) for the album or artist.
+235            If the url is to an artists main page,
+236            all albums will be downloaded.
+237            The tracks will be saved to a subdirectory of
+238            your current directory.
+239            If a track can't be streamed (i.e. private) it
+240            won't be downloaded. Multiple urls can be passed.""",
+241    )
+242
+243    parser.add_argument(
+244        "-n",
+245        "--no_track_number",
+246        action="store_true",
+247        help=""" By default the track number will be added
+248        to the front of the track title. Pass this switch
+249        to disable the behavior.""",
+250    )
+251
+252    parser.add_argument(
+253        "-o",
+254        "--overwrite",
+255        action="store_true",
+256        help=""" Pass this flag to overwrite existing files.
+257        Otherwise don't download tracks that already exist locally.""",
+258    )
+259
+260    args = parser.parse_args()
+261    args.urls = [url.strip("/") for url in args.urls]
+262
+263    return args
   ⁰
 def main(args: argparse.Namespace = None): View Source
-268def main(args: argparse.Namespace = None):
-269    if not args:
-270        args = get_args()
-271    for url in args.urls:
-272        if page_is_discography(url):
-273            ripper = BandRipper(url, args.no_track_number, args.overwrite)
-274        else:
-275            ripper = AlbumRipper(url, args.no_track_number, args.overwrite)
-276        ripper.rip()
+266def main(args: argparse.Namespace = None):
+267    if not args:
+268        args = get_args()
+269    for url in args.urls:
+270        if page_is_discography(url):
+271            ripper = BandRipper(url, args.no_track_number, args.overwrite)
+272        else:
+273            ripper = AlbumRipper(url, args.no_track_number, args.overwrite)
+274        ripper.rip()
```

### Comparing `bandripper-0.1.4/src/bandripper/bandripper.py` & `bandripper-0.1.5/src/bandripper/bandripper.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 import re
 import string
 from dataclasses import dataclass
 from pathlib import Path
 from urllib.parse import urlparse
 
 import requests
-from bs4 import BeautifulSoup
-
 import whosyouragent
+from bs4 import BeautifulSoup
 from noiftimer import Timer
 from printbuddies import ProgBar
 
 root = Path(__file__).parent
 
 
 def clean_string(text: str) -> str:
@@ -131,15 +130,14 @@
         """Download and save the album tracks and album art."""
         if len(self.album.tracks) == 0:
             print(f"No public tracks available for {self.album}.")
             return None
         self.make_save_path()
         self.download_album_art()
         bar = ProgBar(len(self.album.tracks) - 1, width_ratio=0.5)
-        bar.timer.subsecond_resolution = True
         fails = []
         if not self.overwrite:
             self.album.tracks = [
                 track for track in self.album.tracks if not self.track_exists(track)
             ]
         for track in self.album.tracks:
             bar.display(
```

### Comparing `bandripper-0.1.4/LICENSE.txt` & `bandripper-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bandripper-0.1.4/README.md` & `bandripper-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `bandripper-0.1.4/pyproject.toml` & `bandripper-0.1.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 00000030: 6261 636b 656e 6420 3d20 2268 6174 6368  backend = "hatch
 00000040: 6c69 6e67 2e62 7569 6c64 220d 0a0d 0a5b  ling.build"....[
 00000050: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000060: 2022 6261 6e64 7269 7070 6572 220d 0a64   "bandripper"..d
 00000070: 6573 6372 6970 7469 6f6e 203d 2022 5269  escription = "Ri
 00000080: 7020 6d70 3373 2066 726f 6d20 6261 6e64  p mp3s from band
 00000090: 6361 6d70 2e22 0d0a 7665 7273 696f 6e20  camp."..version 
-000000a0: 3d20 2230 2e31 2e34 220d 0a72 6571 7569  = "0.1.4"..requi
+000000a0: 3d20 2230 2e31 2e35 220d 0a72 6571 7569  = "0.1.5"..requi
 000000b0: 7265 732d 7079 7468 6f6e 203d 2022 3e3d  res-python = ">=
-000000c0: 332e 3722 0d0a 6465 7065 6e64 656e 6369  3.7"..dependenci
+000000c0: 332e 3922 0d0a 6465 7065 6e64 656e 6369  3.9"..dependenci
 000000d0: 6573 203d 205b 2272 6571 7565 7374 7322  es = ["requests"
 000000e0: 2c20 2262 7334 222c 2022 7768 6f73 796f  , "bs4", "whosyo
 000000f0: 7572 6167 656e 7422 2c20 226e 6f69 6674  uragent", "noift
 00000100: 696d 6572 222c 2022 7072 696e 7462 7564  imer", "printbud
 00000110: 6469 6573 222c 2022 7079 7465 7374 225d  dies", "pytest"]
 00000120: 0d0a 7265 6164 6d65 203d 2022 5245 4144  ..readme = "READ
 00000130: 4d45 2e6d 6422 0d0a 6b65 7977 6f72 6473  ME.md"..keywords
```

### Comparing `bandripper-0.1.4/PKG-INFO` & `bandripper-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: bandripper
-Version: 0.1.4
+Version: 0.1.5
 Summary: Rip mp3s from bandcamp.
 Project-URL: Homepage, https://github.com/matt-manes/bandripper
 Project-URL: Documentation, https://github.com/matt-manes/bandripper/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/bandripper/tree/main/src/bandripper
 Author-email: Matt Manes <mattmanes@pm.me>
 License-File: LICENSE.txt
 Keywords: audio,bandcamp,download,downloader,music
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Requires-Dist: bs4
 Requires-Dist: noiftimer
 Requires-Dist: printbuddies
 Requires-Dist: pytest
 Requires-Dist: requests
 Requires-Dist: whosyouragent
 Description-Content-Type: text/markdown
```

