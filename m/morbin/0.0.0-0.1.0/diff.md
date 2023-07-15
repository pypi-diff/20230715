# Comparing `tmp/morbin-0.0.0.tar.gz` & `tmp/morbin-0.1.0.tar.gz`

## Comparing `morbin-0.0.0.tar` & `morbin-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 morbin-0.0.0/docs/index.html
--rw-r--r--   0        0        0    34165 2020-02-02 00:00:00.000000 morbin-0.0.0/docs/morbin.html
--rw-r--r--   0        0        0    26137 2020-02-02 00:00:00.000000 morbin-0.0.0/docs/search.js
--rw-r--r--   0        0        0    96520 2020-02-02 00:00:00.000000 morbin-0.0.0/docs/morbin/morbin.html
--rw-r--r--   0        0        0    42501 2020-02-02 00:00:00.000000 morbin-0.0.0/docs/morbin/template.html
--rw-r--r--   0        0        0   112076 2020-02-02 00:00:00.000000 morbin-0.0.0/imgs/full.png
--rw-r--r--   0        0        0    86504 2020-02-02 00:00:00.000000 morbin-0.0.0/imgs/functions.png
--rw-r--r--   0        0        0    29813 2020-02-02 00:00:00.000000 morbin-0.0.0/imgs/output.png
--rw-r--r--   0        0        0    36400 2020-02-02 00:00:00.000000 morbin-0.0.0/imgs/template.png
--rw-r--r--   0        0        0    58761 2020-02-02 00:00:00.000000 morbin-0.0.0/imgs/use.png
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 morbin-0.0.0/src/morbin/__init__.py
--rw-r--r--   0        0        0     3651 2020-02-02 00:00:00.000000 morbin-0.0.0/src/morbin/morbin.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 morbin-0.0.0/src/morbin/template.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 morbin-0.0.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 morbin-0.0.0/LICENSE.txt
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 morbin-0.0.0/README.md
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 morbin-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 morbin-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 morbin-0.1.0/docs/index.html
+-rw-r--r--   0        0        0    34165 2020-02-02 00:00:00.000000 morbin-0.1.0/docs/morbin.html
+-rw-r--r--   0        0        0    26240 2020-02-02 00:00:00.000000 morbin-0.1.0/docs/search.js
+-rw-r--r--   0        0        0   100453 2020-02-02 00:00:00.000000 morbin-0.1.0/docs/morbin/morbin.html
+-rw-r--r--   0        0        0    42501 2020-02-02 00:00:00.000000 morbin-0.1.0/docs/morbin/template.html
+-rw-r--r--   0        0        0   112076 2020-02-02 00:00:00.000000 morbin-0.1.0/imgs/full.png
+-rw-r--r--   0        0        0    86504 2020-02-02 00:00:00.000000 morbin-0.1.0/imgs/functions.png
+-rw-r--r--   0        0        0    29813 2020-02-02 00:00:00.000000 morbin-0.1.0/imgs/output.png
+-rw-r--r--   0        0        0    36400 2020-02-02 00:00:00.000000 morbin-0.1.0/imgs/template.png
+-rw-r--r--   0        0        0    58761 2020-02-02 00:00:00.000000 morbin-0.1.0/imgs/use.png
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 morbin-0.1.0/src/morbin/__init__.py
+-rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 morbin-0.1.0/src/morbin/morbin.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 morbin-0.1.0/src/morbin/template.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 morbin-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 morbin-0.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 morbin-0.1.0/README.md
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 morbin-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 morbin-0.1.0/PKG-INFO
```

### Comparing `morbin-0.0.0/docs/morbin.html` & `morbin-0.1.0/docs/morbin.html`

 * *Files identical despite different names*

### Comparing `morbin-0.0.0/docs/search.js` & `morbin-0.1.0/docs/search.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -693,22 +693,22 @@
         "kind": "module",
         "doc": "<p></p>\n"
     }, {
         "fullname": "morbin.morbin.Output",
         "modulename": "morbin.morbin",
         "qualname": "Output",
         "kind": "class",
-        "doc": "<p>Dataclass representing the output of a terminal command.</p>\n\n<h4 id=\"fields\">Fields:</h4>\n\n<ul>\n<li><code>return_code</code></li>\n<li><code>stdout</code></li>\n<li><code>stderr</code></li>\n</ul>\n"
+        "doc": "<p>Dataclass representing the output of a terminal command.</p>\n\n<h4 id=\"fields\">Fields:</h4>\n\n<ul>\n<li><code>return_code: list[int]</code></li>\n<li><code>stdout: str</code></li>\n<li><code>stderr: str</code></li>\n</ul>\n"
     }, {
         "fullname": "morbin.morbin.Output.__init__",
         "modulename": "morbin.morbin",
         "qualname": "Output.__init__",
         "kind": "function",
         "doc": "<p></p>\n",
-        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">return_code</span><span class=\"p\">:</span> <span class=\"nb\">int</span>, </span><span class=\"param\"><span class=\"n\">stdout</span><span class=\"p\">:</span> <span class=\"nb\">str</span> <span class=\"o\">=</span> <span class=\"s1\">&#39;&#39;</span>, </span><span class=\"param\"><span class=\"n\">stderr</span><span class=\"p\">:</span> <span class=\"nb\">str</span> <span class=\"o\">=</span> <span class=\"s1\">&#39;&#39;</span></span>)</span>"
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">return_code</span><span class=\"p\">:</span> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"nb\">int</span><span class=\"p\">]</span>, </span><span class=\"param\"><span class=\"n\">stdout</span><span class=\"p\">:</span> <span class=\"nb\">str</span> <span class=\"o\">=</span> <span class=\"s1\">&#39;&#39;</span>, </span><span class=\"param\"><span class=\"n\">stderr</span><span class=\"p\">:</span> <span class=\"nb\">str</span> <span class=\"o\">=</span> <span class=\"s1\">&#39;&#39;</span></span>)</span>"
     }, {
         "fullname": "morbin.morbin.Morbin",
         "modulename": "morbin.morbin",
         "qualname": "Morbin",
         "kind": "class",
         "doc": "<p></p>\n"
     }, {
```

### Comparing `morbin-0.0.0/docs/morbin/morbin.html` & `morbin-0.1.0/docs/morbin/morbin.html`

 * *Files 2% similar despite different names*

```diff
@@ -90,121 +90,129 @@
                         <div class="pdoc-code codehilite"><pre><span></span><span id="L-1"><a href="#L-1"><span class="linenos">  1</span></a><span class="kn">import</span> <span class="nn">argparse</span>
 </span><span id="L-2"><a href="#L-2"><span class="linenos">  2</span></a><span class="kn">import</span> <span class="nn">shlex</span>
 </span><span id="L-3"><a href="#L-3"><span class="linenos">  3</span></a><span class="kn">import</span> <span class="nn">subprocess</span>
 </span><span id="L-4"><a href="#L-4"><span class="linenos">  4</span></a><span class="kn">from</span> <span class="nn">contextlib</span> <span class="kn">import</span> <span class="n">contextmanager</span>
 </span><span id="L-5"><a href="#L-5"><span class="linenos">  5</span></a><span class="kn">from</span> <span class="nn">dataclasses</span> <span class="kn">import</span> <span class="n">dataclass</span>
 </span><span id="L-6"><a href="#L-6"><span class="linenos">  6</span></a>
 </span><span id="L-7"><a href="#L-7"><span class="linenos">  7</span></a><span class="kn">from</span> <span class="nn">pathier</span> <span class="kn">import</span> <span class="n">Pathier</span>
-</span><span id="L-8"><a href="#L-8"><span class="linenos">  8</span></a>
-</span><span id="L-9"><a href="#L-9"><span class="linenos">  9</span></a><span class="n">root</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="vm">__file__</span><span class="p">)</span><span class="o">.</span><span class="n">parent</span>
-</span><span id="L-10"><a href="#L-10"><span class="linenos"> 10</span></a>
+</span><span id="L-8"><a href="#L-8"><span class="linenos">  8</span></a><span class="kn">from</span> <span class="nn">typing_extensions</span> <span class="kn">import</span> <span class="n">Self</span>
+</span><span id="L-9"><a href="#L-9"><span class="linenos">  9</span></a>
+</span><span id="L-10"><a href="#L-10"><span class="linenos"> 10</span></a><span class="n">root</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="vm">__file__</span><span class="p">)</span><span class="o">.</span><span class="n">parent</span>
 </span><span id="L-11"><a href="#L-11"><span class="linenos"> 11</span></a>
-</span><span id="L-12"><a href="#L-12"><span class="linenos"> 12</span></a><span class="nd">@dataclass</span>
-</span><span id="L-13"><a href="#L-13"><span class="linenos"> 13</span></a><span class="k">class</span> <span class="nc">Output</span><span class="p">:</span>
-</span><span id="L-14"><a href="#L-14"><span class="linenos"> 14</span></a>    <span class="sd">&quot;&quot;&quot;Dataclass representing the output of a terminal command.</span>
-</span><span id="L-15"><a href="#L-15"><span class="linenos"> 15</span></a>
-</span><span id="L-16"><a href="#L-16"><span class="linenos"> 16</span></a><span class="sd">    #### Fields:</span>
-</span><span id="L-17"><a href="#L-17"><span class="linenos"> 17</span></a><span class="sd">    * `return_code`</span>
-</span><span id="L-18"><a href="#L-18"><span class="linenos"> 18</span></a><span class="sd">    * `stdout`</span>
-</span><span id="L-19"><a href="#L-19"><span class="linenos"> 19</span></a><span class="sd">    * `stderr`&quot;&quot;&quot;</span>
-</span><span id="L-20"><a href="#L-20"><span class="linenos"> 20</span></a>
-</span><span id="L-21"><a href="#L-21"><span class="linenos"> 21</span></a>    <span class="n">return_code</span><span class="p">:</span> <span class="nb">int</span>
-</span><span id="L-22"><a href="#L-22"><span class="linenos"> 22</span></a>    <span class="n">stdout</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="L-23"><a href="#L-23"><span class="linenos"> 23</span></a>    <span class="n">stderr</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="L-24"><a href="#L-24"><span class="linenos"> 24</span></a>
+</span><span id="L-12"><a href="#L-12"><span class="linenos"> 12</span></a>
+</span><span id="L-13"><a href="#L-13"><span class="linenos"> 13</span></a><span class="nd">@dataclass</span>
+</span><span id="L-14"><a href="#L-14"><span class="linenos"> 14</span></a><span class="k">class</span> <span class="nc">Output</span><span class="p">:</span>
+</span><span id="L-15"><a href="#L-15"><span class="linenos"> 15</span></a>    <span class="sd">&quot;&quot;&quot;Dataclass representing the output of a terminal command.</span>
+</span><span id="L-16"><a href="#L-16"><span class="linenos"> 16</span></a>
+</span><span id="L-17"><a href="#L-17"><span class="linenos"> 17</span></a><span class="sd">    #### Fields:</span>
+</span><span id="L-18"><a href="#L-18"><span class="linenos"> 18</span></a><span class="sd">    * `return_code: list[int]`</span>
+</span><span id="L-19"><a href="#L-19"><span class="linenos"> 19</span></a><span class="sd">    * `stdout: str`</span>
+</span><span id="L-20"><a href="#L-20"><span class="linenos"> 20</span></a><span class="sd">    * `stderr: str`&quot;&quot;&quot;</span>
+</span><span id="L-21"><a href="#L-21"><span class="linenos"> 21</span></a>
+</span><span id="L-22"><a href="#L-22"><span class="linenos"> 22</span></a>    <span class="n">return_code</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">int</span><span class="p">]</span>
+</span><span id="L-23"><a href="#L-23"><span class="linenos"> 23</span></a>    <span class="n">stdout</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="L-24"><a href="#L-24"><span class="linenos"> 24</span></a>    <span class="n">stderr</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
 </span><span id="L-25"><a href="#L-25"><span class="linenos"> 25</span></a>
-</span><span id="L-26"><a href="#L-26"><span class="linenos"> 26</span></a><span class="k">class</span> <span class="nc">Morbin</span><span class="p">:</span>
-</span><span id="L-27"><a href="#L-27"><span class="linenos"> 27</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">capture_output</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span> <span class="n">shell</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">):</span>
-</span><span id="L-28"><a href="#L-28"><span class="linenos"> 28</span></a>        <span class="sd">&quot;&quot;&quot;Command bindings should return an `Output` object.</span>
-</span><span id="L-29"><a href="#L-29"><span class="linenos"> 29</span></a>
-</span><span id="L-30"><a href="#L-30"><span class="linenos"> 30</span></a><span class="sd">        If `capture_output` is `True` or the `capturing_output` context manager is used,</span>
-</span><span id="L-31"><a href="#L-31"><span class="linenos"> 31</span></a><span class="sd">        the command&#39;s output will be available via `Output.stdout` and `Output.stderr`.</span>
+</span><span id="L-26"><a href="#L-26"><span class="linenos"> 26</span></a>    <span class="k">def</span> <span class="fm">__add__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">output</span><span class="p">:</span> <span class="n">Self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
+</span><span id="L-27"><a href="#L-27"><span class="linenos"> 27</span></a>        <span class="k">return</span> <span class="n">Output</span><span class="p">(</span>
+</span><span id="L-28"><a href="#L-28"><span class="linenos"> 28</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">return_code</span> <span class="o">+</span> <span class="n">output</span><span class="o">.</span><span class="n">return_code</span><span class="p">,</span>
+</span><span id="L-29"><a href="#L-29"><span class="linenos"> 29</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">stdout</span> <span class="o">+</span> <span class="n">output</span><span class="o">.</span><span class="n">stdout</span><span class="p">,</span>
+</span><span id="L-30"><a href="#L-30"><span class="linenos"> 30</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">stderr</span> <span class="o">+</span> <span class="n">output</span><span class="o">.</span><span class="n">stderr</span><span class="p">,</span>
+</span><span id="L-31"><a href="#L-31"><span class="linenos"> 31</span></a>        <span class="p">)</span>
 </span><span id="L-32"><a href="#L-32"><span class="linenos"> 32</span></a>
-</span><span id="L-33"><a href="#L-33"><span class="linenos"> 33</span></a><span class="sd">        This property can be used to parse and use the command output or to simply execute commands &quot;silently&quot;.</span>
-</span><span id="L-34"><a href="#L-34"><span class="linenos"> 34</span></a>
-</span><span id="L-35"><a href="#L-35"><span class="linenos"> 35</span></a><span class="sd">        The return code will also be available via `Output.return_code`.</span>
-</span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a>
-</span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a><span class="sd">        If `shell` is `True`, commands will be executed in the system shell (necessary on Windows for builtin shell commands like `cd` and `dir`).</span>
-</span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a>
-</span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a><span class="sd">        [Security concerns using shell = True](https://docs.python.org/3/library/subprocess.html#security-considerations)</span>
+</span><span id="L-33"><a href="#L-33"><span class="linenos"> 33</span></a>
+</span><span id="L-34"><a href="#L-34"><span class="linenos"> 34</span></a><span class="k">class</span> <span class="nc">Morbin</span><span class="p">:</span>
+</span><span id="L-35"><a href="#L-35"><span class="linenos"> 35</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">capture_output</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span> <span class="n">shell</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">):</span>
+</span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a>        <span class="sd">&quot;&quot;&quot;Command bindings should return an `Output` object.</span>
+</span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a>
+</span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a><span class="sd">        If `capture_output` is `True` or the `capturing_output` context manager is used,</span>
+</span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a><span class="sd">        the command&#39;s output will be available via `Output.stdout` and `Output.stderr`.</span>
 </span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a>
-</span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="L-42"><a href="#L-42"><span class="linenos"> 42</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">capture_output</span> <span class="o">=</span> <span class="n">capture_output</span>
-</span><span id="L-43"><a href="#L-43"><span class="linenos"> 43</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">shell</span> <span class="o">=</span> <span class="n">shell</span>
+</span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a><span class="sd">        This property can be used to parse and use the command output or to simply execute commands &quot;silently&quot;.</span>
+</span><span id="L-42"><a href="#L-42"><span class="linenos"> 42</span></a>
+</span><span id="L-43"><a href="#L-43"><span class="linenos"> 43</span></a><span class="sd">        The return code will also be available via `Output.return_code`.</span>
 </span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a>
-</span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a>    <span class="nd">@property</span>
-</span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a>    <span class="k">def</span> <span class="nf">capture_output</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a>        <span class="sd">&quot;&quot;&quot;If `True`, member functions will return the generated `stdout` as a string,</span>
-</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a><span class="sd">        otherwise they return the command&#39;s exit code as a string (so my type checker doesn&#39;t throw a fit about ints.).&quot;&quot;&quot;</span>
-</span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_capture_output</span>
-</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a>
-</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a>    <span class="nd">@capture_output</span><span class="o">.</span><span class="n">setter</span>
-</span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a>    <span class="k">def</span> <span class="nf">capture_output</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">should_capture</span><span class="p">:</span> <span class="nb">bool</span><span class="p">):</span>
-</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_capture_output</span> <span class="o">=</span> <span class="n">should_capture</span>
-</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a>
-</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a>    <span class="nd">@property</span>
-</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a>    <span class="k">def</span> <span class="nf">shell</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a>        <span class="sd">&quot;&quot;&quot;If `True`, commands will be executed in the system shell.&quot;&quot;&quot;</span>
-</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_shell</span>
-</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a>
-</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a>    <span class="nd">@shell</span><span class="o">.</span><span class="n">setter</span>
-</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a>    <span class="k">def</span> <span class="nf">shell</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">should_use</span><span class="p">:</span> <span class="nb">bool</span><span class="p">):</span>
-</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_shell</span> <span class="o">=</span> <span class="n">should_use</span>
-</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a>
-</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a>    <span class="nd">@contextmanager</span>
-</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a>    <span class="k">def</span> <span class="nf">capturing_output</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a>        <span class="sd">&quot;&quot;&quot;Ensures `self.capture_output` is `True` while within the context.</span>
+</span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a><span class="sd">        If `shell` is `True`, commands will be executed in the system shell (necessary on Windows for builtin shell commands like `cd` and `dir`).</span>
+</span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a>
+</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a><span class="sd">        [Security concerns using shell = True](https://docs.python.org/3/library/subprocess.html#security-considerations)</span>
+</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a>
+</span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">capture_output</span> <span class="o">=</span> <span class="n">capture_output</span>
+</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">shell</span> <span class="o">=</span> <span class="n">shell</span>
+</span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a>
+</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a>    <span class="nd">@property</span>
+</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a>    <span class="k">def</span> <span class="nf">capture_output</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a>        <span class="sd">&quot;&quot;&quot;If `True`, member functions will return the generated `stdout` as a string,</span>
+</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a><span class="sd">        otherwise they return the command&#39;s exit code as a string (so my type checker doesn&#39;t throw a fit about ints.).&quot;&quot;&quot;</span>
+</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_capture_output</span>
+</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a>
+</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a>    <span class="nd">@capture_output</span><span class="o">.</span><span class="n">setter</span>
+</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a>    <span class="k">def</span> <span class="nf">capture_output</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">should_capture</span><span class="p">:</span> <span class="nb">bool</span><span class="p">):</span>
+</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_capture_output</span> <span class="o">=</span> <span class="n">should_capture</span>
+</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a>
+</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a>    <span class="nd">@property</span>
+</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a>    <span class="k">def</span> <span class="nf">shell</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a>        <span class="sd">&quot;&quot;&quot;If `True`, commands will be executed in the system shell.&quot;&quot;&quot;</span>
+</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_shell</span>
 </span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a>
-</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a><span class="sd">        Upon exiting the context, `self.capture_output` will be set back to whatever it was when the context was entered.&quot;&quot;&quot;</span>
-</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a>        <span class="n">original_state</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">capture_output</span>
-</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">capture_output</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a>        <span class="k">yield</span> <span class="bp">self</span>
-</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">capture_output</span> <span class="o">=</span> <span class="n">original_state</span>
-</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a>
-</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a>    <span class="k">def</span> <span class="nf">execute</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">program</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Output</span><span class="p">:</span>
-</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a>        <span class="n">command</span> <span class="o">=</span> <span class="p">[</span><span class="n">program</span><span class="p">]</span> <span class="o">+</span> <span class="n">shlex</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
-</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">capture_output</span><span class="p">:</span>
-</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a>            <span class="n">output</span> <span class="o">=</span> <span class="n">subprocess</span><span class="o">.</span><span class="n">run</span><span class="p">(</span>
-</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a>                <span class="n">command</span><span class="p">,</span>
-</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a>                <span class="n">stdout</span><span class="o">=</span><span class="n">subprocess</span><span class="o">.</span><span class="n">PIPE</span><span class="p">,</span>
-</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a>                <span class="n">stderr</span><span class="o">=</span><span class="n">subprocess</span><span class="o">.</span><span class="n">PIPE</span><span class="p">,</span>
-</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a>                <span class="n">text</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span>
-</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a>                <span class="n">shell</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">shell</span><span class="p">,</span>
-</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a>            <span class="p">)</span>
-</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a>            <span class="k">return</span> <span class="n">Output</span><span class="p">(</span><span class="n">output</span><span class="o">.</span><span class="n">returncode</span><span class="p">,</span> <span class="n">output</span><span class="o">.</span><span class="n">stdout</span><span class="p">,</span> <span class="n">output</span><span class="o">.</span><span class="n">stderr</span><span class="p">)</span>
-</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>            <span class="n">output</span> <span class="o">=</span> <span class="n">subprocess</span><span class="o">.</span><span class="n">run</span><span class="p">(</span><span class="n">command</span><span class="p">,</span> <span class="n">shell</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">shell</span><span class="p">)</span>
-</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>            <span class="k">return</span> <span class="n">Output</span><span class="p">(</span><span class="n">output</span><span class="o">.</span><span class="n">returncode</span><span class="p">)</span>
-</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>
-</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>
-</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
-</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
-</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a>
-</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a>        <span class="s2">&quot;name&quot;</span><span class="p">,</span>
-</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The program name to create a template subclass of Morbin for. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a>    <span class="p">)</span>
-</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
-</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a>
-</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>    <span class="k">return</span> <span class="n">args</span>
-</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>
-</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>
-</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
-</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
-</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>    <span class="n">template</span> <span class="o">=</span> <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;template.py&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span>
-</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a>    <span class="n">template</span> <span class="o">=</span> <span class="n">template</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;Program&quot;</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="o">.</span><span class="n">capitalize</span><span class="p">())</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span>
-</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>        <span class="s2">&quot;program&quot;</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span>
-</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>    <span class="p">)</span>
-</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>    <span class="p">(</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span> <span class="o">/</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2">.py&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">template</span><span class="p">)</span>
-</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>
-</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>
-</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
-</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>    <span class="n">main</span><span class="p">(</span><span class="n">get_args</span><span class="p">())</span>
+</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a>    <span class="nd">@shell</span><span class="o">.</span><span class="n">setter</span>
+</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a>    <span class="k">def</span> <span class="nf">shell</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">should_use</span><span class="p">:</span> <span class="nb">bool</span><span class="p">):</span>
+</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_shell</span> <span class="o">=</span> <span class="n">should_use</span>
+</span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a>
+</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a>    <span class="nd">@contextmanager</span>
+</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a>    <span class="k">def</span> <span class="nf">capturing_output</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a>        <span class="sd">&quot;&quot;&quot;Ensures `self.capture_output` is `True` while within the context.</span>
+</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a>
+</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a><span class="sd">        Upon exiting the context, `self.capture_output` will be set back to whatever it was when the context was entered.&quot;&quot;&quot;</span>
+</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a>        <span class="n">original_state</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">capture_output</span>
+</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">capture_output</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a>        <span class="k">yield</span> <span class="bp">self</span>
+</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">capture_output</span> <span class="o">=</span> <span class="n">original_state</span>
+</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a>
+</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a>    <span class="k">def</span> <span class="nf">execute</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">program</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Output</span><span class="p">:</span>
+</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a>        <span class="n">command</span> <span class="o">=</span> <span class="p">[</span><span class="n">program</span><span class="p">]</span> <span class="o">+</span> <span class="n">shlex</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
+</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">capture_output</span><span class="p">:</span>
+</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a>            <span class="n">output</span> <span class="o">=</span> <span class="n">subprocess</span><span class="o">.</span><span class="n">run</span><span class="p">(</span>
+</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>                <span class="n">command</span><span class="p">,</span>
+</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>                <span class="n">stdout</span><span class="o">=</span><span class="n">subprocess</span><span class="o">.</span><span class="n">PIPE</span><span class="p">,</span>
+</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>                <span class="n">stderr</span><span class="o">=</span><span class="n">subprocess</span><span class="o">.</span><span class="n">PIPE</span><span class="p">,</span>
+</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>                <span class="n">text</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span>
+</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>                <span class="n">shell</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">shell</span><span class="p">,</span>
+</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>            <span class="p">)</span>
+</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a>            <span class="k">return</span> <span class="n">Output</span><span class="p">([</span><span class="n">output</span><span class="o">.</span><span class="n">returncode</span><span class="p">],</span> <span class="n">output</span><span class="o">.</span><span class="n">stdout</span><span class="p">,</span> <span class="n">output</span><span class="o">.</span><span class="n">stderr</span><span class="p">)</span>
+</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a>            <span class="n">output</span> <span class="o">=</span> <span class="n">subprocess</span><span class="o">.</span><span class="n">run</span><span class="p">(</span><span class="n">command</span><span class="p">,</span> <span class="n">shell</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">shell</span><span class="p">)</span>
+</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>            <span class="k">return</span> <span class="n">Output</span><span class="p">([</span><span class="n">output</span><span class="o">.</span><span class="n">returncode</span><span class="p">])</span>
+</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a>
+</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a>
+</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
+</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
+</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>
+</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>        <span class="s2">&quot;name&quot;</span><span class="p">,</span>
+</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The program name to create a template subclass of Morbin for. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>    <span class="p">)</span>
+</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
+</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a>
+</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>    <span class="k">return</span> <span class="n">args</span>
+</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>
+</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>
+</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
+</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
+</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>    <span class="n">template</span> <span class="o">=</span> <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;template.py&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span>
+</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>    <span class="n">template</span> <span class="o">=</span> <span class="n">template</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;Program&quot;</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="o">.</span><span class="n">capitalize</span><span class="p">())</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span>
+</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>        <span class="s2">&quot;program&quot;</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span>
+</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>    <span class="p">)</span>
+</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>    <span class="p">(</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span> <span class="o">/</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2">.py&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">template</span><span class="p">)</span>
+</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>
+</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>
+</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
+</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>    <span class="n">main</span><span class="p">(</span><span class="n">get_args</span><span class="p">())</span>
 </span></pre></div>
 
 
             </section>
                 <section id="Output">
                             <input id="Output-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr class">
@@ -213,45 +221,52 @@
     <span class="def">class</span>
     <span class="name">Output</span>:
 
                 <label class="view-source-button" for="Output-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Output"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Output-13"><a href="#Output-13"><span class="linenos">13</span></a><span class="nd">@dataclass</span>
-</span><span id="Output-14"><a href="#Output-14"><span class="linenos">14</span></a><span class="k">class</span> <span class="nc">Output</span><span class="p">:</span>
-</span><span id="Output-15"><a href="#Output-15"><span class="linenos">15</span></a>    <span class="sd">&quot;&quot;&quot;Dataclass representing the output of a terminal command.</span>
-</span><span id="Output-16"><a href="#Output-16"><span class="linenos">16</span></a>
-</span><span id="Output-17"><a href="#Output-17"><span class="linenos">17</span></a><span class="sd">    #### Fields:</span>
-</span><span id="Output-18"><a href="#Output-18"><span class="linenos">18</span></a><span class="sd">    * `return_code`</span>
-</span><span id="Output-19"><a href="#Output-19"><span class="linenos">19</span></a><span class="sd">    * `stdout`</span>
-</span><span id="Output-20"><a href="#Output-20"><span class="linenos">20</span></a><span class="sd">    * `stderr`&quot;&quot;&quot;</span>
-</span><span id="Output-21"><a href="#Output-21"><span class="linenos">21</span></a>
-</span><span id="Output-22"><a href="#Output-22"><span class="linenos">22</span></a>    <span class="n">return_code</span><span class="p">:</span> <span class="nb">int</span>
-</span><span id="Output-23"><a href="#Output-23"><span class="linenos">23</span></a>    <span class="n">stdout</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="Output-24"><a href="#Output-24"><span class="linenos">24</span></a>    <span class="n">stderr</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Output-14"><a href="#Output-14"><span class="linenos">14</span></a><span class="nd">@dataclass</span>
+</span><span id="Output-15"><a href="#Output-15"><span class="linenos">15</span></a><span class="k">class</span> <span class="nc">Output</span><span class="p">:</span>
+</span><span id="Output-16"><a href="#Output-16"><span class="linenos">16</span></a>    <span class="sd">&quot;&quot;&quot;Dataclass representing the output of a terminal command.</span>
+</span><span id="Output-17"><a href="#Output-17"><span class="linenos">17</span></a>
+</span><span id="Output-18"><a href="#Output-18"><span class="linenos">18</span></a><span class="sd">    #### Fields:</span>
+</span><span id="Output-19"><a href="#Output-19"><span class="linenos">19</span></a><span class="sd">    * `return_code: list[int]`</span>
+</span><span id="Output-20"><a href="#Output-20"><span class="linenos">20</span></a><span class="sd">    * `stdout: str`</span>
+</span><span id="Output-21"><a href="#Output-21"><span class="linenos">21</span></a><span class="sd">    * `stderr: str`&quot;&quot;&quot;</span>
+</span><span id="Output-22"><a href="#Output-22"><span class="linenos">22</span></a>
+</span><span id="Output-23"><a href="#Output-23"><span class="linenos">23</span></a>    <span class="n">return_code</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">int</span><span class="p">]</span>
+</span><span id="Output-24"><a href="#Output-24"><span class="linenos">24</span></a>    <span class="n">stdout</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="Output-25"><a href="#Output-25"><span class="linenos">25</span></a>    <span class="n">stderr</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="Output-26"><a href="#Output-26"><span class="linenos">26</span></a>
+</span><span id="Output-27"><a href="#Output-27"><span class="linenos">27</span></a>    <span class="k">def</span> <span class="fm">__add__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">output</span><span class="p">:</span> <span class="n">Self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
+</span><span id="Output-28"><a href="#Output-28"><span class="linenos">28</span></a>        <span class="k">return</span> <span class="n">Output</span><span class="p">(</span>
+</span><span id="Output-29"><a href="#Output-29"><span class="linenos">29</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">return_code</span> <span class="o">+</span> <span class="n">output</span><span class="o">.</span><span class="n">return_code</span><span class="p">,</span>
+</span><span id="Output-30"><a href="#Output-30"><span class="linenos">30</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">stdout</span> <span class="o">+</span> <span class="n">output</span><span class="o">.</span><span class="n">stdout</span><span class="p">,</span>
+</span><span id="Output-31"><a href="#Output-31"><span class="linenos">31</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">stderr</span> <span class="o">+</span> <span class="n">output</span><span class="o">.</span><span class="n">stderr</span><span class="p">,</span>
+</span><span id="Output-32"><a href="#Output-32"><span class="linenos">32</span></a>        <span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Dataclass representing the output of a terminal command.</p>
 
 <h4 id="fields">Fields:</h4>
 
 <ul>
-<li><code>return_code</code></li>
-<li><code>stdout</code></li>
-<li><code>stderr</code></li>
+<li><code>return_code: list[int]</code></li>
+<li><code>stdout: str</code></li>
+<li><code>stderr: str</code></li>
 </ul>
 </div>
 
 
                             <div id="Output.__init__" class="classattr">
                                 <div class="attr function">
             
-        <span class="name">Output</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">return_code</span><span class="p">:</span> <span class="nb">int</span>, </span><span class="param"><span class="n">stdout</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s1">&#39;&#39;</span>, </span><span class="param"><span class="n">stderr</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s1">&#39;&#39;</span></span>)</span>
+        <span class="name">Output</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">return_code</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">int</span><span class="p">]</span>, </span><span class="param"><span class="n">stdout</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s1">&#39;&#39;</span>, </span><span class="param"><span class="n">stderr</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s1">&#39;&#39;</span></span>)</span>
 
         
     </div>
     <a class="headerlink" href="#Output.__init__"></a>
     
     
 
@@ -264,76 +279,76 @@
     <span class="def">class</span>
     <span class="name">Morbin</span>:
 
                 <label class="view-source-button" for="Morbin-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Morbin"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Morbin-27"><a href="#Morbin-27"><span class="linenos">27</span></a><span class="k">class</span> <span class="nc">Morbin</span><span class="p">:</span>
-</span><span id="Morbin-28"><a href="#Morbin-28"><span class="linenos">28</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">capture_output</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span> <span class="n">shell</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">):</span>
-</span><span id="Morbin-29"><a href="#Morbin-29"><span class="linenos">29</span></a>        <span class="sd">&quot;&quot;&quot;Command bindings should return an `Output` object.</span>
-</span><span id="Morbin-30"><a href="#Morbin-30"><span class="linenos">30</span></a>
-</span><span id="Morbin-31"><a href="#Morbin-31"><span class="linenos">31</span></a><span class="sd">        If `capture_output` is `True` or the `capturing_output` context manager is used,</span>
-</span><span id="Morbin-32"><a href="#Morbin-32"><span class="linenos">32</span></a><span class="sd">        the command&#39;s output will be available via `Output.stdout` and `Output.stderr`.</span>
-</span><span id="Morbin-33"><a href="#Morbin-33"><span class="linenos">33</span></a>
-</span><span id="Morbin-34"><a href="#Morbin-34"><span class="linenos">34</span></a><span class="sd">        This property can be used to parse and use the command output or to simply execute commands &quot;silently&quot;.</span>
-</span><span id="Morbin-35"><a href="#Morbin-35"><span class="linenos">35</span></a>
-</span><span id="Morbin-36"><a href="#Morbin-36"><span class="linenos">36</span></a><span class="sd">        The return code will also be available via `Output.return_code`.</span>
-</span><span id="Morbin-37"><a href="#Morbin-37"><span class="linenos">37</span></a>
-</span><span id="Morbin-38"><a href="#Morbin-38"><span class="linenos">38</span></a><span class="sd">        If `shell` is `True`, commands will be executed in the system shell (necessary on Windows for builtin shell commands like `cd` and `dir`).</span>
-</span><span id="Morbin-39"><a href="#Morbin-39"><span class="linenos">39</span></a>
-</span><span id="Morbin-40"><a href="#Morbin-40"><span class="linenos">40</span></a><span class="sd">        [Security concerns using shell = True](https://docs.python.org/3/library/subprocess.html#security-considerations)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Morbin-35"><a href="#Morbin-35"><span class="linenos">35</span></a><span class="k">class</span> <span class="nc">Morbin</span><span class="p">:</span>
+</span><span id="Morbin-36"><a href="#Morbin-36"><span class="linenos">36</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">capture_output</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span> <span class="n">shell</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">):</span>
+</span><span id="Morbin-37"><a href="#Morbin-37"><span class="linenos">37</span></a>        <span class="sd">&quot;&quot;&quot;Command bindings should return an `Output` object.</span>
+</span><span id="Morbin-38"><a href="#Morbin-38"><span class="linenos">38</span></a>
+</span><span id="Morbin-39"><a href="#Morbin-39"><span class="linenos">39</span></a><span class="sd">        If `capture_output` is `True` or the `capturing_output` context manager is used,</span>
+</span><span id="Morbin-40"><a href="#Morbin-40"><span class="linenos">40</span></a><span class="sd">        the command&#39;s output will be available via `Output.stdout` and `Output.stderr`.</span>
 </span><span id="Morbin-41"><a href="#Morbin-41"><span class="linenos">41</span></a>
-</span><span id="Morbin-42"><a href="#Morbin-42"><span class="linenos">42</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="Morbin-43"><a href="#Morbin-43"><span class="linenos">43</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">capture_output</span> <span class="o">=</span> <span class="n">capture_output</span>
-</span><span id="Morbin-44"><a href="#Morbin-44"><span class="linenos">44</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">shell</span> <span class="o">=</span> <span class="n">shell</span>
+</span><span id="Morbin-42"><a href="#Morbin-42"><span class="linenos">42</span></a><span class="sd">        This property can be used to parse and use the command output or to simply execute commands &quot;silently&quot;.</span>
+</span><span id="Morbin-43"><a href="#Morbin-43"><span class="linenos">43</span></a>
+</span><span id="Morbin-44"><a href="#Morbin-44"><span class="linenos">44</span></a><span class="sd">        The return code will also be available via `Output.return_code`.</span>
 </span><span id="Morbin-45"><a href="#Morbin-45"><span class="linenos">45</span></a>
-</span><span id="Morbin-46"><a href="#Morbin-46"><span class="linenos">46</span></a>    <span class="nd">@property</span>
-</span><span id="Morbin-47"><a href="#Morbin-47"><span class="linenos">47</span></a>    <span class="k">def</span> <span class="nf">capture_output</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="Morbin-48"><a href="#Morbin-48"><span class="linenos">48</span></a>        <span class="sd">&quot;&quot;&quot;If `True`, member functions will return the generated `stdout` as a string,</span>
-</span><span id="Morbin-49"><a href="#Morbin-49"><span class="linenos">49</span></a><span class="sd">        otherwise they return the command&#39;s exit code as a string (so my type checker doesn&#39;t throw a fit about ints.).&quot;&quot;&quot;</span>
-</span><span id="Morbin-50"><a href="#Morbin-50"><span class="linenos">50</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_capture_output</span>
-</span><span id="Morbin-51"><a href="#Morbin-51"><span class="linenos">51</span></a>
-</span><span id="Morbin-52"><a href="#Morbin-52"><span class="linenos">52</span></a>    <span class="nd">@capture_output</span><span class="o">.</span><span class="n">setter</span>
-</span><span id="Morbin-53"><a href="#Morbin-53"><span class="linenos">53</span></a>    <span class="k">def</span> <span class="nf">capture_output</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">should_capture</span><span class="p">:</span> <span class="nb">bool</span><span class="p">):</span>
-</span><span id="Morbin-54"><a href="#Morbin-54"><span class="linenos">54</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_capture_output</span> <span class="o">=</span> <span class="n">should_capture</span>
-</span><span id="Morbin-55"><a href="#Morbin-55"><span class="linenos">55</span></a>
-</span><span id="Morbin-56"><a href="#Morbin-56"><span class="linenos">56</span></a>    <span class="nd">@property</span>
-</span><span id="Morbin-57"><a href="#Morbin-57"><span class="linenos">57</span></a>    <span class="k">def</span> <span class="nf">shell</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="Morbin-58"><a href="#Morbin-58"><span class="linenos">58</span></a>        <span class="sd">&quot;&quot;&quot;If `True`, commands will be executed in the system shell.&quot;&quot;&quot;</span>
-</span><span id="Morbin-59"><a href="#Morbin-59"><span class="linenos">59</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_shell</span>
-</span><span id="Morbin-60"><a href="#Morbin-60"><span class="linenos">60</span></a>
-</span><span id="Morbin-61"><a href="#Morbin-61"><span class="linenos">61</span></a>    <span class="nd">@shell</span><span class="o">.</span><span class="n">setter</span>
-</span><span id="Morbin-62"><a href="#Morbin-62"><span class="linenos">62</span></a>    <span class="k">def</span> <span class="nf">shell</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">should_use</span><span class="p">:</span> <span class="nb">bool</span><span class="p">):</span>
-</span><span id="Morbin-63"><a href="#Morbin-63"><span class="linenos">63</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_shell</span> <span class="o">=</span> <span class="n">should_use</span>
-</span><span id="Morbin-64"><a href="#Morbin-64"><span class="linenos">64</span></a>
-</span><span id="Morbin-65"><a href="#Morbin-65"><span class="linenos">65</span></a>    <span class="nd">@contextmanager</span>
-</span><span id="Morbin-66"><a href="#Morbin-66"><span class="linenos">66</span></a>    <span class="k">def</span> <span class="nf">capturing_output</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Morbin-67"><a href="#Morbin-67"><span class="linenos">67</span></a>        <span class="sd">&quot;&quot;&quot;Ensures `self.capture_output` is `True` while within the context.</span>
+</span><span id="Morbin-46"><a href="#Morbin-46"><span class="linenos">46</span></a><span class="sd">        If `shell` is `True`, commands will be executed in the system shell (necessary on Windows for builtin shell commands like `cd` and `dir`).</span>
+</span><span id="Morbin-47"><a href="#Morbin-47"><span class="linenos">47</span></a>
+</span><span id="Morbin-48"><a href="#Morbin-48"><span class="linenos">48</span></a><span class="sd">        [Security concerns using shell = True](https://docs.python.org/3/library/subprocess.html#security-considerations)</span>
+</span><span id="Morbin-49"><a href="#Morbin-49"><span class="linenos">49</span></a>
+</span><span id="Morbin-50"><a href="#Morbin-50"><span class="linenos">50</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="Morbin-51"><a href="#Morbin-51"><span class="linenos">51</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">capture_output</span> <span class="o">=</span> <span class="n">capture_output</span>
+</span><span id="Morbin-52"><a href="#Morbin-52"><span class="linenos">52</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">shell</span> <span class="o">=</span> <span class="n">shell</span>
+</span><span id="Morbin-53"><a href="#Morbin-53"><span class="linenos">53</span></a>
+</span><span id="Morbin-54"><a href="#Morbin-54"><span class="linenos">54</span></a>    <span class="nd">@property</span>
+</span><span id="Morbin-55"><a href="#Morbin-55"><span class="linenos">55</span></a>    <span class="k">def</span> <span class="nf">capture_output</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="Morbin-56"><a href="#Morbin-56"><span class="linenos">56</span></a>        <span class="sd">&quot;&quot;&quot;If `True`, member functions will return the generated `stdout` as a string,</span>
+</span><span id="Morbin-57"><a href="#Morbin-57"><span class="linenos">57</span></a><span class="sd">        otherwise they return the command&#39;s exit code as a string (so my type checker doesn&#39;t throw a fit about ints.).&quot;&quot;&quot;</span>
+</span><span id="Morbin-58"><a href="#Morbin-58"><span class="linenos">58</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_capture_output</span>
+</span><span id="Morbin-59"><a href="#Morbin-59"><span class="linenos">59</span></a>
+</span><span id="Morbin-60"><a href="#Morbin-60"><span class="linenos">60</span></a>    <span class="nd">@capture_output</span><span class="o">.</span><span class="n">setter</span>
+</span><span id="Morbin-61"><a href="#Morbin-61"><span class="linenos">61</span></a>    <span class="k">def</span> <span class="nf">capture_output</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">should_capture</span><span class="p">:</span> <span class="nb">bool</span><span class="p">):</span>
+</span><span id="Morbin-62"><a href="#Morbin-62"><span class="linenos">62</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_capture_output</span> <span class="o">=</span> <span class="n">should_capture</span>
+</span><span id="Morbin-63"><a href="#Morbin-63"><span class="linenos">63</span></a>
+</span><span id="Morbin-64"><a href="#Morbin-64"><span class="linenos">64</span></a>    <span class="nd">@property</span>
+</span><span id="Morbin-65"><a href="#Morbin-65"><span class="linenos">65</span></a>    <span class="k">def</span> <span class="nf">shell</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="Morbin-66"><a href="#Morbin-66"><span class="linenos">66</span></a>        <span class="sd">&quot;&quot;&quot;If `True`, commands will be executed in the system shell.&quot;&quot;&quot;</span>
+</span><span id="Morbin-67"><a href="#Morbin-67"><span class="linenos">67</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_shell</span>
 </span><span id="Morbin-68"><a href="#Morbin-68"><span class="linenos">68</span></a>
-</span><span id="Morbin-69"><a href="#Morbin-69"><span class="linenos">69</span></a><span class="sd">        Upon exiting the context, `self.capture_output` will be set back to whatever it was when the context was entered.&quot;&quot;&quot;</span>
-</span><span id="Morbin-70"><a href="#Morbin-70"><span class="linenos">70</span></a>        <span class="n">original_state</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">capture_output</span>
-</span><span id="Morbin-71"><a href="#Morbin-71"><span class="linenos">71</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">capture_output</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="Morbin-72"><a href="#Morbin-72"><span class="linenos">72</span></a>        <span class="k">yield</span> <span class="bp">self</span>
-</span><span id="Morbin-73"><a href="#Morbin-73"><span class="linenos">73</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">capture_output</span> <span class="o">=</span> <span class="n">original_state</span>
-</span><span id="Morbin-74"><a href="#Morbin-74"><span class="linenos">74</span></a>
-</span><span id="Morbin-75"><a href="#Morbin-75"><span class="linenos">75</span></a>    <span class="k">def</span> <span class="nf">execute</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">program</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Output</span><span class="p">:</span>
-</span><span id="Morbin-76"><a href="#Morbin-76"><span class="linenos">76</span></a>        <span class="n">command</span> <span class="o">=</span> <span class="p">[</span><span class="n">program</span><span class="p">]</span> <span class="o">+</span> <span class="n">shlex</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
-</span><span id="Morbin-77"><a href="#Morbin-77"><span class="linenos">77</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">capture_output</span><span class="p">:</span>
-</span><span id="Morbin-78"><a href="#Morbin-78"><span class="linenos">78</span></a>            <span class="n">output</span> <span class="o">=</span> <span class="n">subprocess</span><span class="o">.</span><span class="n">run</span><span class="p">(</span>
-</span><span id="Morbin-79"><a href="#Morbin-79"><span class="linenos">79</span></a>                <span class="n">command</span><span class="p">,</span>
-</span><span id="Morbin-80"><a href="#Morbin-80"><span class="linenos">80</span></a>                <span class="n">stdout</span><span class="o">=</span><span class="n">subprocess</span><span class="o">.</span><span class="n">PIPE</span><span class="p">,</span>
-</span><span id="Morbin-81"><a href="#Morbin-81"><span class="linenos">81</span></a>                <span class="n">stderr</span><span class="o">=</span><span class="n">subprocess</span><span class="o">.</span><span class="n">PIPE</span><span class="p">,</span>
-</span><span id="Morbin-82"><a href="#Morbin-82"><span class="linenos">82</span></a>                <span class="n">text</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span>
-</span><span id="Morbin-83"><a href="#Morbin-83"><span class="linenos">83</span></a>                <span class="n">shell</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">shell</span><span class="p">,</span>
-</span><span id="Morbin-84"><a href="#Morbin-84"><span class="linenos">84</span></a>            <span class="p">)</span>
-</span><span id="Morbin-85"><a href="#Morbin-85"><span class="linenos">85</span></a>            <span class="k">return</span> <span class="n">Output</span><span class="p">(</span><span class="n">output</span><span class="o">.</span><span class="n">returncode</span><span class="p">,</span> <span class="n">output</span><span class="o">.</span><span class="n">stdout</span><span class="p">,</span> <span class="n">output</span><span class="o">.</span><span class="n">stderr</span><span class="p">)</span>
-</span><span id="Morbin-86"><a href="#Morbin-86"><span class="linenos">86</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="Morbin-87"><a href="#Morbin-87"><span class="linenos">87</span></a>            <span class="n">output</span> <span class="o">=</span> <span class="n">subprocess</span><span class="o">.</span><span class="n">run</span><span class="p">(</span><span class="n">command</span><span class="p">,</span> <span class="n">shell</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">shell</span><span class="p">)</span>
-</span><span id="Morbin-88"><a href="#Morbin-88"><span class="linenos">88</span></a>            <span class="k">return</span> <span class="n">Output</span><span class="p">(</span><span class="n">output</span><span class="o">.</span><span class="n">returncode</span><span class="p">)</span>
+</span><span id="Morbin-69"><a href="#Morbin-69"><span class="linenos">69</span></a>    <span class="nd">@shell</span><span class="o">.</span><span class="n">setter</span>
+</span><span id="Morbin-70"><a href="#Morbin-70"><span class="linenos">70</span></a>    <span class="k">def</span> <span class="nf">shell</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">should_use</span><span class="p">:</span> <span class="nb">bool</span><span class="p">):</span>
+</span><span id="Morbin-71"><a href="#Morbin-71"><span class="linenos">71</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_shell</span> <span class="o">=</span> <span class="n">should_use</span>
+</span><span id="Morbin-72"><a href="#Morbin-72"><span class="linenos">72</span></a>
+</span><span id="Morbin-73"><a href="#Morbin-73"><span class="linenos">73</span></a>    <span class="nd">@contextmanager</span>
+</span><span id="Morbin-74"><a href="#Morbin-74"><span class="linenos">74</span></a>    <span class="k">def</span> <span class="nf">capturing_output</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Morbin-75"><a href="#Morbin-75"><span class="linenos">75</span></a>        <span class="sd">&quot;&quot;&quot;Ensures `self.capture_output` is `True` while within the context.</span>
+</span><span id="Morbin-76"><a href="#Morbin-76"><span class="linenos">76</span></a>
+</span><span id="Morbin-77"><a href="#Morbin-77"><span class="linenos">77</span></a><span class="sd">        Upon exiting the context, `self.capture_output` will be set back to whatever it was when the context was entered.&quot;&quot;&quot;</span>
+</span><span id="Morbin-78"><a href="#Morbin-78"><span class="linenos">78</span></a>        <span class="n">original_state</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">capture_output</span>
+</span><span id="Morbin-79"><a href="#Morbin-79"><span class="linenos">79</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">capture_output</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="Morbin-80"><a href="#Morbin-80"><span class="linenos">80</span></a>        <span class="k">yield</span> <span class="bp">self</span>
+</span><span id="Morbin-81"><a href="#Morbin-81"><span class="linenos">81</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">capture_output</span> <span class="o">=</span> <span class="n">original_state</span>
+</span><span id="Morbin-82"><a href="#Morbin-82"><span class="linenos">82</span></a>
+</span><span id="Morbin-83"><a href="#Morbin-83"><span class="linenos">83</span></a>    <span class="k">def</span> <span class="nf">execute</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">program</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Output</span><span class="p">:</span>
+</span><span id="Morbin-84"><a href="#Morbin-84"><span class="linenos">84</span></a>        <span class="n">command</span> <span class="o">=</span> <span class="p">[</span><span class="n">program</span><span class="p">]</span> <span class="o">+</span> <span class="n">shlex</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
+</span><span id="Morbin-85"><a href="#Morbin-85"><span class="linenos">85</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">capture_output</span><span class="p">:</span>
+</span><span id="Morbin-86"><a href="#Morbin-86"><span class="linenos">86</span></a>            <span class="n">output</span> <span class="o">=</span> <span class="n">subprocess</span><span class="o">.</span><span class="n">run</span><span class="p">(</span>
+</span><span id="Morbin-87"><a href="#Morbin-87"><span class="linenos">87</span></a>                <span class="n">command</span><span class="p">,</span>
+</span><span id="Morbin-88"><a href="#Morbin-88"><span class="linenos">88</span></a>                <span class="n">stdout</span><span class="o">=</span><span class="n">subprocess</span><span class="o">.</span><span class="n">PIPE</span><span class="p">,</span>
+</span><span id="Morbin-89"><a href="#Morbin-89"><span class="linenos">89</span></a>                <span class="n">stderr</span><span class="o">=</span><span class="n">subprocess</span><span class="o">.</span><span class="n">PIPE</span><span class="p">,</span>
+</span><span id="Morbin-90"><a href="#Morbin-90"><span class="linenos">90</span></a>                <span class="n">text</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span>
+</span><span id="Morbin-91"><a href="#Morbin-91"><span class="linenos">91</span></a>                <span class="n">shell</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">shell</span><span class="p">,</span>
+</span><span id="Morbin-92"><a href="#Morbin-92"><span class="linenos">92</span></a>            <span class="p">)</span>
+</span><span id="Morbin-93"><a href="#Morbin-93"><span class="linenos">93</span></a>            <span class="k">return</span> <span class="n">Output</span><span class="p">([</span><span class="n">output</span><span class="o">.</span><span class="n">returncode</span><span class="p">],</span> <span class="n">output</span><span class="o">.</span><span class="n">stdout</span><span class="p">,</span> <span class="n">output</span><span class="o">.</span><span class="n">stderr</span><span class="p">)</span>
+</span><span id="Morbin-94"><a href="#Morbin-94"><span class="linenos">94</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="Morbin-95"><a href="#Morbin-95"><span class="linenos">95</span></a>            <span class="n">output</span> <span class="o">=</span> <span class="n">subprocess</span><span class="o">.</span><span class="n">run</span><span class="p">(</span><span class="n">command</span><span class="p">,</span> <span class="n">shell</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">shell</span><span class="p">)</span>
+</span><span id="Morbin-96"><a href="#Morbin-96"><span class="linenos">96</span></a>            <span class="k">return</span> <span class="n">Output</span><span class="p">([</span><span class="n">output</span><span class="o">.</span><span class="n">returncode</span><span class="p">])</span>
 </span></pre></div>
 
 
     
 
                             <div id="Morbin.__init__" class="classattr">
                                         <input id="Morbin.__init__-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
@@ -341,31 +356,31 @@
             
         <span class="name">Morbin</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">capture_output</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>, </span><span class="param"><span class="n">shell</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span></span>)</span>
 
                 <label class="view-source-button" for="Morbin.__init__-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Morbin.__init__"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Morbin.__init__-28"><a href="#Morbin.__init__-28"><span class="linenos">28</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">capture_output</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span> <span class="n">shell</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">):</span>
-</span><span id="Morbin.__init__-29"><a href="#Morbin.__init__-29"><span class="linenos">29</span></a>        <span class="sd">&quot;&quot;&quot;Command bindings should return an `Output` object.</span>
-</span><span id="Morbin.__init__-30"><a href="#Morbin.__init__-30"><span class="linenos">30</span></a>
-</span><span id="Morbin.__init__-31"><a href="#Morbin.__init__-31"><span class="linenos">31</span></a><span class="sd">        If `capture_output` is `True` or the `capturing_output` context manager is used,</span>
-</span><span id="Morbin.__init__-32"><a href="#Morbin.__init__-32"><span class="linenos">32</span></a><span class="sd">        the command&#39;s output will be available via `Output.stdout` and `Output.stderr`.</span>
-</span><span id="Morbin.__init__-33"><a href="#Morbin.__init__-33"><span class="linenos">33</span></a>
-</span><span id="Morbin.__init__-34"><a href="#Morbin.__init__-34"><span class="linenos">34</span></a><span class="sd">        This property can be used to parse and use the command output or to simply execute commands &quot;silently&quot;.</span>
-</span><span id="Morbin.__init__-35"><a href="#Morbin.__init__-35"><span class="linenos">35</span></a>
-</span><span id="Morbin.__init__-36"><a href="#Morbin.__init__-36"><span class="linenos">36</span></a><span class="sd">        The return code will also be available via `Output.return_code`.</span>
-</span><span id="Morbin.__init__-37"><a href="#Morbin.__init__-37"><span class="linenos">37</span></a>
-</span><span id="Morbin.__init__-38"><a href="#Morbin.__init__-38"><span class="linenos">38</span></a><span class="sd">        If `shell` is `True`, commands will be executed in the system shell (necessary on Windows for builtin shell commands like `cd` and `dir`).</span>
-</span><span id="Morbin.__init__-39"><a href="#Morbin.__init__-39"><span class="linenos">39</span></a>
-</span><span id="Morbin.__init__-40"><a href="#Morbin.__init__-40"><span class="linenos">40</span></a><span class="sd">        [Security concerns using shell = True](https://docs.python.org/3/library/subprocess.html#security-considerations)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Morbin.__init__-36"><a href="#Morbin.__init__-36"><span class="linenos">36</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">capture_output</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span> <span class="n">shell</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">):</span>
+</span><span id="Morbin.__init__-37"><a href="#Morbin.__init__-37"><span class="linenos">37</span></a>        <span class="sd">&quot;&quot;&quot;Command bindings should return an `Output` object.</span>
+</span><span id="Morbin.__init__-38"><a href="#Morbin.__init__-38"><span class="linenos">38</span></a>
+</span><span id="Morbin.__init__-39"><a href="#Morbin.__init__-39"><span class="linenos">39</span></a><span class="sd">        If `capture_output` is `True` or the `capturing_output` context manager is used,</span>
+</span><span id="Morbin.__init__-40"><a href="#Morbin.__init__-40"><span class="linenos">40</span></a><span class="sd">        the command&#39;s output will be available via `Output.stdout` and `Output.stderr`.</span>
 </span><span id="Morbin.__init__-41"><a href="#Morbin.__init__-41"><span class="linenos">41</span></a>
-</span><span id="Morbin.__init__-42"><a href="#Morbin.__init__-42"><span class="linenos">42</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="Morbin.__init__-43"><a href="#Morbin.__init__-43"><span class="linenos">43</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">capture_output</span> <span class="o">=</span> <span class="n">capture_output</span>
-</span><span id="Morbin.__init__-44"><a href="#Morbin.__init__-44"><span class="linenos">44</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">shell</span> <span class="o">=</span> <span class="n">shell</span>
+</span><span id="Morbin.__init__-42"><a href="#Morbin.__init__-42"><span class="linenos">42</span></a><span class="sd">        This property can be used to parse and use the command output or to simply execute commands &quot;silently&quot;.</span>
+</span><span id="Morbin.__init__-43"><a href="#Morbin.__init__-43"><span class="linenos">43</span></a>
+</span><span id="Morbin.__init__-44"><a href="#Morbin.__init__-44"><span class="linenos">44</span></a><span class="sd">        The return code will also be available via `Output.return_code`.</span>
+</span><span id="Morbin.__init__-45"><a href="#Morbin.__init__-45"><span class="linenos">45</span></a>
+</span><span id="Morbin.__init__-46"><a href="#Morbin.__init__-46"><span class="linenos">46</span></a><span class="sd">        If `shell` is `True`, commands will be executed in the system shell (necessary on Windows for builtin shell commands like `cd` and `dir`).</span>
+</span><span id="Morbin.__init__-47"><a href="#Morbin.__init__-47"><span class="linenos">47</span></a>
+</span><span id="Morbin.__init__-48"><a href="#Morbin.__init__-48"><span class="linenos">48</span></a><span class="sd">        [Security concerns using shell = True](https://docs.python.org/3/library/subprocess.html#security-considerations)</span>
+</span><span id="Morbin.__init__-49"><a href="#Morbin.__init__-49"><span class="linenos">49</span></a>
+</span><span id="Morbin.__init__-50"><a href="#Morbin.__init__-50"><span class="linenos">50</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="Morbin.__init__-51"><a href="#Morbin.__init__-51"><span class="linenos">51</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">capture_output</span> <span class="o">=</span> <span class="n">capture_output</span>
+</span><span id="Morbin.__init__-52"><a href="#Morbin.__init__-52"><span class="linenos">52</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">shell</span> <span class="o">=</span> <span class="n">shell</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Command bindings should return an <code><a href="#Output">Output</a></code> object.</p>
 
 <p>If <code><a href="#Morbin.capture_output">capture_output</a></code> is <code>True</code> or the <code><a href="#Morbin.capturing_output">capturing_output</a></code> context manager is used,
 the command's output will be available via <code>Output.stdout</code> and <code>Output.stderr</code>.</p>
@@ -416,23 +431,23 @@
         <span class="def">def</span>
         <span class="name">capturing_output</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="Morbin.capturing_output-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Morbin.capturing_output"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Morbin.capturing_output-65"><a href="#Morbin.capturing_output-65"><span class="linenos">65</span></a>    <span class="nd">@contextmanager</span>
-</span><span id="Morbin.capturing_output-66"><a href="#Morbin.capturing_output-66"><span class="linenos">66</span></a>    <span class="k">def</span> <span class="nf">capturing_output</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Morbin.capturing_output-67"><a href="#Morbin.capturing_output-67"><span class="linenos">67</span></a>        <span class="sd">&quot;&quot;&quot;Ensures `self.capture_output` is `True` while within the context.</span>
-</span><span id="Morbin.capturing_output-68"><a href="#Morbin.capturing_output-68"><span class="linenos">68</span></a>
-</span><span id="Morbin.capturing_output-69"><a href="#Morbin.capturing_output-69"><span class="linenos">69</span></a><span class="sd">        Upon exiting the context, `self.capture_output` will be set back to whatever it was when the context was entered.&quot;&quot;&quot;</span>
-</span><span id="Morbin.capturing_output-70"><a href="#Morbin.capturing_output-70"><span class="linenos">70</span></a>        <span class="n">original_state</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">capture_output</span>
-</span><span id="Morbin.capturing_output-71"><a href="#Morbin.capturing_output-71"><span class="linenos">71</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">capture_output</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="Morbin.capturing_output-72"><a href="#Morbin.capturing_output-72"><span class="linenos">72</span></a>        <span class="k">yield</span> <span class="bp">self</span>
-</span><span id="Morbin.capturing_output-73"><a href="#Morbin.capturing_output-73"><span class="linenos">73</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">capture_output</span> <span class="o">=</span> <span class="n">original_state</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Morbin.capturing_output-73"><a href="#Morbin.capturing_output-73"><span class="linenos">73</span></a>    <span class="nd">@contextmanager</span>
+</span><span id="Morbin.capturing_output-74"><a href="#Morbin.capturing_output-74"><span class="linenos">74</span></a>    <span class="k">def</span> <span class="nf">capturing_output</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Morbin.capturing_output-75"><a href="#Morbin.capturing_output-75"><span class="linenos">75</span></a>        <span class="sd">&quot;&quot;&quot;Ensures `self.capture_output` is `True` while within the context.</span>
+</span><span id="Morbin.capturing_output-76"><a href="#Morbin.capturing_output-76"><span class="linenos">76</span></a>
+</span><span id="Morbin.capturing_output-77"><a href="#Morbin.capturing_output-77"><span class="linenos">77</span></a><span class="sd">        Upon exiting the context, `self.capture_output` will be set back to whatever it was when the context was entered.&quot;&quot;&quot;</span>
+</span><span id="Morbin.capturing_output-78"><a href="#Morbin.capturing_output-78"><span class="linenos">78</span></a>        <span class="n">original_state</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">capture_output</span>
+</span><span id="Morbin.capturing_output-79"><a href="#Morbin.capturing_output-79"><span class="linenos">79</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">capture_output</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="Morbin.capturing_output-80"><a href="#Morbin.capturing_output-80"><span class="linenos">80</span></a>        <span class="k">yield</span> <span class="bp">self</span>
+</span><span id="Morbin.capturing_output-81"><a href="#Morbin.capturing_output-81"><span class="linenos">81</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">capture_output</span> <span class="o">=</span> <span class="n">original_state</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Ensures <code>self.capture_output</code> is <code>True</code> while within the context.</p>
 
 <p>Upon exiting the context, <code>self.capture_output</code> will be set back to whatever it was when the context was entered.</p>
 </div>
@@ -446,28 +461,28 @@
         <span class="def">def</span>
         <span class="name">execute</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">program</span><span class="p">:</span> <span class="nb">str</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="n"><a href="#Output">morbin.morbin.Output</a></span>:</span></span>
 
                 <label class="view-source-button" for="Morbin.execute-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Morbin.execute"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Morbin.execute-75"><a href="#Morbin.execute-75"><span class="linenos">75</span></a>    <span class="k">def</span> <span class="nf">execute</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">program</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Output</span><span class="p">:</span>
-</span><span id="Morbin.execute-76"><a href="#Morbin.execute-76"><span class="linenos">76</span></a>        <span class="n">command</span> <span class="o">=</span> <span class="p">[</span><span class="n">program</span><span class="p">]</span> <span class="o">+</span> <span class="n">shlex</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
-</span><span id="Morbin.execute-77"><a href="#Morbin.execute-77"><span class="linenos">77</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">capture_output</span><span class="p">:</span>
-</span><span id="Morbin.execute-78"><a href="#Morbin.execute-78"><span class="linenos">78</span></a>            <span class="n">output</span> <span class="o">=</span> <span class="n">subprocess</span><span class="o">.</span><span class="n">run</span><span class="p">(</span>
-</span><span id="Morbin.execute-79"><a href="#Morbin.execute-79"><span class="linenos">79</span></a>                <span class="n">command</span><span class="p">,</span>
-</span><span id="Morbin.execute-80"><a href="#Morbin.execute-80"><span class="linenos">80</span></a>                <span class="n">stdout</span><span class="o">=</span><span class="n">subprocess</span><span class="o">.</span><span class="n">PIPE</span><span class="p">,</span>
-</span><span id="Morbin.execute-81"><a href="#Morbin.execute-81"><span class="linenos">81</span></a>                <span class="n">stderr</span><span class="o">=</span><span class="n">subprocess</span><span class="o">.</span><span class="n">PIPE</span><span class="p">,</span>
-</span><span id="Morbin.execute-82"><a href="#Morbin.execute-82"><span class="linenos">82</span></a>                <span class="n">text</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span>
-</span><span id="Morbin.execute-83"><a href="#Morbin.execute-83"><span class="linenos">83</span></a>                <span class="n">shell</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">shell</span><span class="p">,</span>
-</span><span id="Morbin.execute-84"><a href="#Morbin.execute-84"><span class="linenos">84</span></a>            <span class="p">)</span>
-</span><span id="Morbin.execute-85"><a href="#Morbin.execute-85"><span class="linenos">85</span></a>            <span class="k">return</span> <span class="n">Output</span><span class="p">(</span><span class="n">output</span><span class="o">.</span><span class="n">returncode</span><span class="p">,</span> <span class="n">output</span><span class="o">.</span><span class="n">stdout</span><span class="p">,</span> <span class="n">output</span><span class="o">.</span><span class="n">stderr</span><span class="p">)</span>
-</span><span id="Morbin.execute-86"><a href="#Morbin.execute-86"><span class="linenos">86</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="Morbin.execute-87"><a href="#Morbin.execute-87"><span class="linenos">87</span></a>            <span class="n">output</span> <span class="o">=</span> <span class="n">subprocess</span><span class="o">.</span><span class="n">run</span><span class="p">(</span><span class="n">command</span><span class="p">,</span> <span class="n">shell</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">shell</span><span class="p">)</span>
-</span><span id="Morbin.execute-88"><a href="#Morbin.execute-88"><span class="linenos">88</span></a>            <span class="k">return</span> <span class="n">Output</span><span class="p">(</span><span class="n">output</span><span class="o">.</span><span class="n">returncode</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Morbin.execute-83"><a href="#Morbin.execute-83"><span class="linenos">83</span></a>    <span class="k">def</span> <span class="nf">execute</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">program</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Output</span><span class="p">:</span>
+</span><span id="Morbin.execute-84"><a href="#Morbin.execute-84"><span class="linenos">84</span></a>        <span class="n">command</span> <span class="o">=</span> <span class="p">[</span><span class="n">program</span><span class="p">]</span> <span class="o">+</span> <span class="n">shlex</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
+</span><span id="Morbin.execute-85"><a href="#Morbin.execute-85"><span class="linenos">85</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">capture_output</span><span class="p">:</span>
+</span><span id="Morbin.execute-86"><a href="#Morbin.execute-86"><span class="linenos">86</span></a>            <span class="n">output</span> <span class="o">=</span> <span class="n">subprocess</span><span class="o">.</span><span class="n">run</span><span class="p">(</span>
+</span><span id="Morbin.execute-87"><a href="#Morbin.execute-87"><span class="linenos">87</span></a>                <span class="n">command</span><span class="p">,</span>
+</span><span id="Morbin.execute-88"><a href="#Morbin.execute-88"><span class="linenos">88</span></a>                <span class="n">stdout</span><span class="o">=</span><span class="n">subprocess</span><span class="o">.</span><span class="n">PIPE</span><span class="p">,</span>
+</span><span id="Morbin.execute-89"><a href="#Morbin.execute-89"><span class="linenos">89</span></a>                <span class="n">stderr</span><span class="o">=</span><span class="n">subprocess</span><span class="o">.</span><span class="n">PIPE</span><span class="p">,</span>
+</span><span id="Morbin.execute-90"><a href="#Morbin.execute-90"><span class="linenos">90</span></a>                <span class="n">text</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span>
+</span><span id="Morbin.execute-91"><a href="#Morbin.execute-91"><span class="linenos">91</span></a>                <span class="n">shell</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">shell</span><span class="p">,</span>
+</span><span id="Morbin.execute-92"><a href="#Morbin.execute-92"><span class="linenos">92</span></a>            <span class="p">)</span>
+</span><span id="Morbin.execute-93"><a href="#Morbin.execute-93"><span class="linenos">93</span></a>            <span class="k">return</span> <span class="n">Output</span><span class="p">([</span><span class="n">output</span><span class="o">.</span><span class="n">returncode</span><span class="p">],</span> <span class="n">output</span><span class="o">.</span><span class="n">stdout</span><span class="p">,</span> <span class="n">output</span><span class="o">.</span><span class="n">stderr</span><span class="p">)</span>
+</span><span id="Morbin.execute-94"><a href="#Morbin.execute-94"><span class="linenos">94</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="Morbin.execute-95"><a href="#Morbin.execute-95"><span class="linenos">95</span></a>            <span class="n">output</span> <span class="o">=</span> <span class="n">subprocess</span><span class="o">.</span><span class="n">run</span><span class="p">(</span><span class="n">command</span><span class="p">,</span> <span class="n">shell</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">shell</span><span class="p">)</span>
+</span><span id="Morbin.execute-96"><a href="#Morbin.execute-96"><span class="linenos">96</span></a>            <span class="k">return</span> <span class="n">Output</span><span class="p">([</span><span class="n">output</span><span class="o">.</span><span class="n">returncode</span><span class="p">])</span>
 </span></pre></div>
 
 
     
 
                             </div>
                 </section>
@@ -478,25 +493,25 @@
         <span class="def">def</span>
         <span class="name">get_args</span><span class="signature pdoc-code condensed">(<span class="return-annotation">) -> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span>:</span></span>
 
                 <label class="view-source-button" for="get_args-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#get_args"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="get_args-91"><a href="#get_args-91"><span class="linenos"> 91</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
-</span><span id="get_args-92"><a href="#get_args-92"><span class="linenos"> 92</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
-</span><span id="get_args-93"><a href="#get_args-93"><span class="linenos"> 93</span></a>
-</span><span id="get_args-94"><a href="#get_args-94"><span class="linenos"> 94</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-95"><a href="#get_args-95"><span class="linenos"> 95</span></a>        <span class="s2">&quot;name&quot;</span><span class="p">,</span>
-</span><span id="get_args-96"><a href="#get_args-96"><span class="linenos"> 96</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="get_args-97"><a href="#get_args-97"><span class="linenos"> 97</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The program name to create a template subclass of Morbin for. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-98"><a href="#get_args-98"><span class="linenos"> 98</span></a>    <span class="p">)</span>
-</span><span id="get_args-99"><a href="#get_args-99"><span class="linenos"> 99</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
-</span><span id="get_args-100"><a href="#get_args-100"><span class="linenos">100</span></a>
-</span><span id="get_args-101"><a href="#get_args-101"><span class="linenos">101</span></a>    <span class="k">return</span> <span class="n">args</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="get_args-99"><a href="#get_args-99"><span class="linenos"> 99</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
+</span><span id="get_args-100"><a href="#get_args-100"><span class="linenos">100</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
+</span><span id="get_args-101"><a href="#get_args-101"><span class="linenos">101</span></a>
+</span><span id="get_args-102"><a href="#get_args-102"><span class="linenos">102</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-103"><a href="#get_args-103"><span class="linenos">103</span></a>        <span class="s2">&quot;name&quot;</span><span class="p">,</span>
+</span><span id="get_args-104"><a href="#get_args-104"><span class="linenos">104</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="get_args-105"><a href="#get_args-105"><span class="linenos">105</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The program name to create a template subclass of Morbin for. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-106"><a href="#get_args-106"><span class="linenos">106</span></a>    <span class="p">)</span>
+</span><span id="get_args-107"><a href="#get_args-107"><span class="linenos">107</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
+</span><span id="get_args-108"><a href="#get_args-108"><span class="linenos">108</span></a>
+</span><span id="get_args-109"><a href="#get_args-109"><span class="linenos">109</span></a>    <span class="k">return</span> <span class="n">args</span>
 </span></pre></div>
 
 
     
 
                 </section>
                 <section id="main">
@@ -506,22 +521,22 @@
         <span class="def">def</span>
         <span class="name">main</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="main-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#main"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="main-104"><a href="#main-104"><span class="linenos">104</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="main-105"><a href="#main-105"><span class="linenos">105</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
-</span><span id="main-106"><a href="#main-106"><span class="linenos">106</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
-</span><span id="main-107"><a href="#main-107"><span class="linenos">107</span></a>    <span class="n">template</span> <span class="o">=</span> <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;template.py&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span>
-</span><span id="main-108"><a href="#main-108"><span class="linenos">108</span></a>    <span class="n">template</span> <span class="o">=</span> <span class="n">template</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;Program&quot;</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="o">.</span><span class="n">capitalize</span><span class="p">())</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span>
-</span><span id="main-109"><a href="#main-109"><span class="linenos">109</span></a>        <span class="s2">&quot;program&quot;</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span>
-</span><span id="main-110"><a href="#main-110"><span class="linenos">110</span></a>    <span class="p">)</span>
-</span><span id="main-111"><a href="#main-111"><span class="linenos">111</span></a>    <span class="p">(</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span> <span class="o">/</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2">.py&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">template</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="main-112"><a href="#main-112"><span class="linenos">112</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="main-113"><a href="#main-113"><span class="linenos">113</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
+</span><span id="main-114"><a href="#main-114"><span class="linenos">114</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
+</span><span id="main-115"><a href="#main-115"><span class="linenos">115</span></a>    <span class="n">template</span> <span class="o">=</span> <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;template.py&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span>
+</span><span id="main-116"><a href="#main-116"><span class="linenos">116</span></a>    <span class="n">template</span> <span class="o">=</span> <span class="n">template</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;Program&quot;</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="o">.</span><span class="n">capitalize</span><span class="p">())</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span>
+</span><span id="main-117"><a href="#main-117"><span class="linenos">117</span></a>        <span class="s2">&quot;program&quot;</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span>
+</span><span id="main-118"><a href="#main-118"><span class="linenos">118</span></a>    <span class="p">)</span>
+</span><span id="main-119"><a href="#main-119"><span class="linenos">119</span></a>    <span class="p">(</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span> <span class="o">/</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2">.py&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">template</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                 </section>
     </main>
```

#### html2text {}

```diff
@@ -20,247 +20,262 @@
 __1import argparse
 __2import shlex
 __3import subprocess
 __4from contextlib import contextmanager
 __5from dataclasses import dataclass
 __6
 __7from pathier import Pathier
-__8
-__9root = Pathier(__file__).parent
-_10
+__8from typing_extensions import Self
+__9
+_10root = Pathier(__file__).parent
 _11
-_12@dataclass
-_13class Output:
-_14    """Dataclass representing the output of a terminal command.
-_15
-_16    #### Fields:
-_17    * `return_code`
-_18    * `stdout`
-_19    * `stderr`"""
-_20
-_21    return_code: int
-_22    stdout: str = ""
-_23    stderr: str = ""
-_24
+_12
+_13@dataclass
+_14class Output:
+_15    """Dataclass representing the output of a terminal command.
+_16
+_17    #### Fields:
+_18    * `return_code: list[int]`
+_19    * `stdout: str`
+_20    * `stderr: str`"""
+_21
+_22    return_code: list[int]
+_23    stdout: str = ""
+_24    stderr: str = ""
 _25
-_26class Morbin:
-_27    def __init__(self, capture_output: bool = False, shell: bool = False):
-_28        """Command bindings should return an `Output` object.
-_29
-_30        If `capture_output` is `True` or the `capturing_output` context
+_26    def __add__(self, output: Self) -> Self:
+_27        return Output(
+_28            self.return_code + output.return_code,
+_29            self.stdout + output.stdout,
+_30            self.stderr + output.stderr,
+_31        )
+_32
+_33
+_34class Morbin:
+_35    def __init__(self, capture_output: bool = False, shell: bool = False):
+_36        """Command bindings should return an `Output` object.
+_37
+_38        If `capture_output` is `True` or the `capturing_output` context
 manager is used,
-_31        the command's output will be available via `Output.stdout` and
+_39        the command's output will be available via `Output.stdout` and
 `Output.stderr`.
-_32
-_33        This property can be used to parse and use the command output or to
+_40
+_41        This property can be used to parse and use the command output or to
 simply execute commands "silently".
-_34
-_35        The return code will also be available via `Output.return_code`.
-_36
-_37        If `shell` is `True`, commands will be executed in the system shell
+_42
+_43        The return code will also be available via `Output.return_code`.
+_44
+_45        If `shell` is `True`, commands will be executed in the system shell
 (necessary on Windows for builtin shell commands like `cd` and `dir`).
-_38
-_39        [Security concerns using shell = True](https://docs.python.org/3/
+_46
+_47        [Security concerns using shell = True](https://docs.python.org/3/
 library/subprocess.html#security-considerations)
-_40
-_41        """
-_42        self.capture_output = capture_output
-_43        self.shell = shell
-_44
-_45    @property
-_46    def capture_output(self) -> bool:
-_47        """If `True`, member functions will return the generated `stdout` as
+_48
+_49        """
+_50        self.capture_output = capture_output
+_51        self.shell = shell
+_52
+_53    @property
+_54    def capture_output(self) -> bool:
+_55        """If `True`, member functions will return the generated `stdout` as
 a string,
-_48        otherwise they return the command's exit code as a string (so my
+_56        otherwise they return the command's exit code as a string (so my
 type checker doesn't throw a fit about ints.)."""
-_49        return self._capture_output
-_50
-_51    @capture_output.setter
-_52    def capture_output(self, should_capture: bool):
-_53        self._capture_output = should_capture
-_54
-_55    @property
-_56    def shell(self) -> bool:
-_57        """If `True`, commands will be executed in the system shell."""
-_58        return self._shell
-_59
-_60    @shell.setter
-_61    def shell(self, should_use: bool):
-_62        self._shell = should_use
-_63
-_64    @contextmanager
-_65    def capturing_output(self):
-_66        """Ensures `self.capture_output` is `True` while within the context.
+_57        return self._capture_output
+_58
+_59    @capture_output.setter
+_60    def capture_output(self, should_capture: bool):
+_61        self._capture_output = should_capture
+_62
+_63    @property
+_64    def shell(self) -> bool:
+_65        """If `True`, commands will be executed in the system shell."""
+_66        return self._shell
 _67
-_68        Upon exiting the context, `self.capture_output` will be set back to
+_68    @shell.setter
+_69    def shell(self, should_use: bool):
+_70        self._shell = should_use
+_71
+_72    @contextmanager
+_73    def capturing_output(self):
+_74        """Ensures `self.capture_output` is `True` while within the context.
+_75
+_76        Upon exiting the context, `self.capture_output` will be set back to
 whatever it was when the context was entered."""
-_69        original_state = self.capture_output
-_70        self.capture_output = True
-_71        yield self
-_72        self.capture_output = original_state
-_73
-_74    def execute(self, program: str, args: str) -> Output:
-_75        command = [program] + shlex.split(args)
-_76        if self.capture_output:
-_77            output = subprocess.run(
-_78                command,
-_79                stdout=subprocess.PIPE,
-_80                stderr=subprocess.PIPE,
-_81                text=True,
-_82                shell=self.shell,
-_83            )
-_84            return Output(output.returncode, output.stdout, output.stderr)
-_85        else:
-_86            output = subprocess.run(command, shell=self.shell)
-_87            return Output(output.returncode)
-_88
-_89
-_90def get_args() -> argparse.Namespace:
-_91    parser = argparse.ArgumentParser()
-_92
-_93    parser.add_argument(
-_94        "name",
-_95        type=str,
-_96        help=""" The program name to create a template subclass of Morbin
+_77        original_state = self.capture_output
+_78        self.capture_output = True
+_79        yield self
+_80        self.capture_output = original_state
+_81
+_82    def execute(self, program: str, args: str) -> Output:
+_83        command = [program] + shlex.split(args)
+_84        if self.capture_output:
+_85            output = subprocess.run(
+_86                command,
+_87                stdout=subprocess.PIPE,
+_88                stderr=subprocess.PIPE,
+_89                text=True,
+_90                shell=self.shell,
+_91            )
+_92            return Output([output.returncode], output.stdout, output.stderr)
+_93        else:
+_94            output = subprocess.run(command, shell=self.shell)
+_95            return Output([output.returncode])
+_96
+_97
+_98def get_args() -> argparse.Namespace:
+_99    parser = argparse.ArgumentParser()
+100
+101    parser.add_argument(
+102        "name",
+103        type=str,
+104        help=""" The program name to create a template subclass of Morbin
 for. """,
-_97    )
-_98    args = parser.parse_args()
-_99
-100    return args
-101
-102
-103def main(args: argparse.Namespace | None = None):
-104    if not args:
-105        args = get_args()
-106    template = (root / "template.py").read_text()
-107    template = template.replace("Program", args.name.capitalize()).replace(
-108        "program", args.name
-109    )
-110    (Pathier.cwd() / f"{args.name}.py").write_text(template)
-111
-112
-113if __name__ == "__main__":
-114    main(get_args())
+105    )
+106    args = parser.parse_args()
+107
+108    return args
+109
+110
+111def main(args: argparse.Namespace | None = None):
+112    if not args:
+113        args = get_args()
+114    template = (root / "template.py").read_text()
+115    template = template.replace("Program", args.name.capitalize()).replace(
+116        "program", args.name
+117    )
+118    (Pathier.cwd() / f"{args.name}.py").write_text(template)
+119
+120
+121if __name__ == "__main__":
+122    main(get_args())
   ⁰
 @dataclass
 class Output: View Source
-13@dataclass
-14class Output:
-15    """Dataclass representing the output of a terminal command.
-16
-17    #### Fields:
-18    * `return_code`
-19    * `stdout`
-20    * `stderr`"""
-21
-22    return_code: int
-23    stdout: str = ""
-24    stderr: str = ""
+14@dataclass
+15class Output:
+16    """Dataclass representing the output of a terminal command.
+17
+18    #### Fields:
+19    * `return_code: list[int]`
+20    * `stdout: str`
+21    * `stderr: str`"""
+22
+23    return_code: list[int]
+24    stdout: str = ""
+25    stderr: str = ""
+26
+27    def __add__(self, output: Self) -> Self:
+28        return Output(
+29            self.return_code + output.return_code,
+30            self.stdout + output.stdout,
+31            self.stderr + output.stderr,
+32        )
 Dataclass representing the output of a terminal command.
 *** Fields: ***
-    * return_code
-    * stdout
-    * stderr
-Output(return_code: int, stdout: str = '', stderr: str = '')
+    * return_code: list[int]
+    * stdout: str
+    * stderr: str
+Output(return_code: list[int], stdout: str = '', stderr: str = '')
   ⁰
 class Morbin: View Source
-27class Morbin:
-28    def __init__(self, capture_output: bool = False, shell: bool = False):
-29        """Command bindings should return an `Output` object.
-30
-31        If `capture_output` is `True` or the `capturing_output` context
+35class Morbin:
+36    def __init__(self, capture_output: bool = False, shell: bool = False):
+37        """Command bindings should return an `Output` object.
+38
+39        If `capture_output` is `True` or the `capturing_output` context
 manager is used,
-32        the command's output will be available via `Output.stdout` and
+40        the command's output will be available via `Output.stdout` and
 `Output.stderr`.
-33
-34        This property can be used to parse and use the command output or to
+41
+42        This property can be used to parse and use the command output or to
 simply execute commands "silently".
-35
-36        The return code will also be available via `Output.return_code`.
-37
-38        If `shell` is `True`, commands will be executed in the system shell
+43
+44        The return code will also be available via `Output.return_code`.
+45
+46        If `shell` is `True`, commands will be executed in the system shell
 (necessary on Windows for builtin shell commands like `cd` and `dir`).
-39
-40        [Security concerns using shell = True](https://docs.python.org/3/
+47
+48        [Security concerns using shell = True](https://docs.python.org/3/
 library/subprocess.html#security-considerations)
-41
-42        """
-43        self.capture_output = capture_output
-44        self.shell = shell
-45
-46    @property
-47    def capture_output(self) -> bool:
-48        """If `True`, member functions will return the generated `stdout` as
+49
+50        """
+51        self.capture_output = capture_output
+52        self.shell = shell
+53
+54    @property
+55    def capture_output(self) -> bool:
+56        """If `True`, member functions will return the generated `stdout` as
 a string,
-49        otherwise they return the command's exit code as a string (so my type
+57        otherwise they return the command's exit code as a string (so my type
 checker doesn't throw a fit about ints.)."""
-50        return self._capture_output
-51
-52    @capture_output.setter
-53    def capture_output(self, should_capture: bool):
-54        self._capture_output = should_capture
-55
-56    @property
-57    def shell(self) -> bool:
-58        """If `True`, commands will be executed in the system shell."""
-59        return self._shell
-60
-61    @shell.setter
-62    def shell(self, should_use: bool):
-63        self._shell = should_use
-64
-65    @contextmanager
-66    def capturing_output(self):
-67        """Ensures `self.capture_output` is `True` while within the context.
+58        return self._capture_output
+59
+60    @capture_output.setter
+61    def capture_output(self, should_capture: bool):
+62        self._capture_output = should_capture
+63
+64    @property
+65    def shell(self) -> bool:
+66        """If `True`, commands will be executed in the system shell."""
+67        return self._shell
 68
-69        Upon exiting the context, `self.capture_output` will be set back to
+69    @shell.setter
+70    def shell(self, should_use: bool):
+71        self._shell = should_use
+72
+73    @contextmanager
+74    def capturing_output(self):
+75        """Ensures `self.capture_output` is `True` while within the context.
+76
+77        Upon exiting the context, `self.capture_output` will be set back to
 whatever it was when the context was entered."""
-70        original_state = self.capture_output
-71        self.capture_output = True
-72        yield self
-73        self.capture_output = original_state
-74
-75    def execute(self, program: str, args: str) -> Output:
-76        command = [program] + shlex.split(args)
-77        if self.capture_output:
-78            output = subprocess.run(
-79                command,
-80                stdout=subprocess.PIPE,
-81                stderr=subprocess.PIPE,
-82                text=True,
-83                shell=self.shell,
-84            )
-85            return Output(output.returncode, output.stdout, output.stderr)
-86        else:
-87            output = subprocess.run(command, shell=self.shell)
-88            return Output(output.returncode)
+78        original_state = self.capture_output
+79        self.capture_output = True
+80        yield self
+81        self.capture_output = original_state
+82
+83    def execute(self, program: str, args: str) -> Output:
+84        command = [program] + shlex.split(args)
+85        if self.capture_output:
+86            output = subprocess.run(
+87                command,
+88                stdout=subprocess.PIPE,
+89                stderr=subprocess.PIPE,
+90                text=True,
+91                shell=self.shell,
+92            )
+93            return Output([output.returncode], output.stdout, output.stderr)
+94        else:
+95            output = subprocess.run(command, shell=self.shell)
+96            return Output([output.returncode])
 ⁰
 Morbin(capture_output: bool = False, shell: bool = False) View Source
-28    def __init__(self, capture_output: bool = False, shell: bool = False):
-29        """Command bindings should return an `Output` object.
-30
-31        If `capture_output` is `True` or the `capturing_output` context
+36    def __init__(self, capture_output: bool = False, shell: bool = False):
+37        """Command bindings should return an `Output` object.
+38
+39        If `capture_output` is `True` or the `capturing_output` context
 manager is used,
-32        the command's output will be available via `Output.stdout` and
+40        the command's output will be available via `Output.stdout` and
 `Output.stderr`.
-33
-34        This property can be used to parse and use the command output or to
+41
+42        This property can be used to parse and use the command output or to
 simply execute commands "silently".
-35
-36        The return code will also be available via `Output.return_code`.
-37
-38        If `shell` is `True`, commands will be executed in the system shell
+43
+44        The return code will also be available via `Output.return_code`.
+45
+46        If `shell` is `True`, commands will be executed in the system shell
 (necessary on Windows for builtin shell commands like `cd` and `dir`).
-39
-40        [Security concerns using shell = True](https://docs.python.org/3/
+47
+48        [Security concerns using shell = True](https://docs.python.org/3/
 library/subprocess.html#security-considerations)
-41
-42        """
-43        self.capture_output = capture_output
-44        self.shell = shell
+49
+50        """
+51        self.capture_output = capture_output
+52        self.shell = shell
 Command bindings should return an Output object.
 If capture_output is True or the capturing_output context manager is used, the
 command's output will be available via Output.stdout and Output.stderr.
 This property can be used to parse and use the command output or to simply
 execute commands "silently".
 The return code will also be available via Output.return_code.
 If shell is True, commands will be executed in the system shell (necessary on
@@ -271,61 +286,61 @@
 otherwise they return the command's exit code as a string (so my type checker
 doesn't throw a fit about ints.).
 shell: bool
 If True, commands will be executed in the system shell.
 ⁰
 @contextmanager
 def capturing_output(self): View Source
-65    @contextmanager
-66    def capturing_output(self):
-67        """Ensures `self.capture_output` is `True` while within the context.
-68
-69        Upon exiting the context, `self.capture_output` will be set back to
+73    @contextmanager
+74    def capturing_output(self):
+75        """Ensures `self.capture_output` is `True` while within the context.
+76
+77        Upon exiting the context, `self.capture_output` will be set back to
 whatever it was when the context was entered."""
-70        original_state = self.capture_output
-71        self.capture_output = True
-72        yield self
-73        self.capture_output = original_state
+78        original_state = self.capture_output
+79        self.capture_output = True
+80        yield self
+81        self.capture_output = original_state
 Ensures self.capture_output is True while within the context.
 Upon exiting the context, self.capture_output will be set back to whatever it
 was when the context was entered.
 ⁰
 def execute(self, program: str, args: str) -> morbin.morbin.Output: View Source
-75    def execute(self, program: str, args: str) -> Output:
-76        command = [program] + shlex.split(args)
-77        if self.capture_output:
-78            output = subprocess.run(
-79                command,
-80                stdout=subprocess.PIPE,
-81                stderr=subprocess.PIPE,
-82                text=True,
-83                shell=self.shell,
-84            )
-85            return Output(output.returncode, output.stdout, output.stderr)
-86        else:
-87            output = subprocess.run(command, shell=self.shell)
-88            return Output(output.returncode)
+83    def execute(self, program: str, args: str) -> Output:
+84        command = [program] + shlex.split(args)
+85        if self.capture_output:
+86            output = subprocess.run(
+87                command,
+88                stdout=subprocess.PIPE,
+89                stderr=subprocess.PIPE,
+90                text=True,
+91                shell=self.shell,
+92            )
+93            return Output([output.returncode], output.stdout, output.stderr)
+94        else:
+95            output = subprocess.run(command, shell=self.shell)
+96            return Output([output.returncode])
   ⁰
 def get_args() -> argparse.Namespace: View Source
-_91def get_args() -> argparse.Namespace:
-_92    parser = argparse.ArgumentParser()
-_93
-_94    parser.add_argument(
-_95        "name",
-_96        type=str,
-_97        help=""" The program name to create a template subclass of Morbin
+_99def get_args() -> argparse.Namespace:
+100    parser = argparse.ArgumentParser()
+101
+102    parser.add_argument(
+103        "name",
+104        type=str,
+105        help=""" The program name to create a template subclass of Morbin
 for. """,
-_98    )
-_99    args = parser.parse_args()
-100
-101    return args
+106    )
+107    args = parser.parse_args()
+108
+109    return args
   ⁰
 def main(args: argparse.Namespace | None = None): View Source
-104def main(args: argparse.Namespace | None = None):
-105    if not args:
-106        args = get_args()
-107    template = (root / "template.py").read_text()
-108    template = template.replace("Program", args.name.capitalize()).replace(
-109        "program", args.name
-110    )
-111    (Pathier.cwd() / f"{args.name}.py").write_text(template)
+112def main(args: argparse.Namespace | None = None):
+113    if not args:
+114        args = get_args()
+115    template = (root / "template.py").read_text()
+116    template = template.replace("Program", args.name.capitalize()).replace(
+117        "program", args.name
+118    )
+119    (Pathier.cwd() / f"{args.name}.py").write_text(template)
```

### Comparing `morbin-0.0.0/docs/morbin/template.html` & `morbin-0.1.0/docs/morbin/template.html`

 * *Files identical despite different names*

### Comparing `morbin-0.0.0/imgs/full.png` & `morbin-0.1.0/imgs/full.png`

 * *Files identical despite different names*

### Comparing `morbin-0.0.0/imgs/functions.png` & `morbin-0.1.0/imgs/functions.png`

 * *Files identical despite different names*

### Comparing `morbin-0.0.0/imgs/output.png` & `morbin-0.1.0/imgs/output.png`

 * *Files identical despite different names*

### Comparing `morbin-0.0.0/imgs/template.png` & `morbin-0.1.0/imgs/template.png`

 * *Files identical despite different names*

### Comparing `morbin-0.0.0/imgs/use.png` & `morbin-0.1.0/imgs/use.png`

 * *Files identical despite different names*

### Comparing `morbin-0.0.0/src/morbin/morbin.py` & `morbin-0.1.0/src/morbin/morbin.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 import argparse
 import shlex
 import subprocess
 from contextlib import contextmanager
 from dataclasses import dataclass
 
 from pathier import Pathier
+from typing_extensions import Self
 
 root = Pathier(__file__).parent
 
 
 @dataclass
 class Output:
     """Dataclass representing the output of a terminal command.
 
     #### Fields:
-    * `return_code`
-    * `stdout`
-    * `stderr`"""
+    * `return_code: list[int]`
+    * `stdout: str`
+    * `stderr: str`"""
 
-    return_code: int
+    return_code: list[int]
     stdout: str = ""
     stderr: str = ""
 
+    def __add__(self, output: Self) -> Self:
+        return Output(
+            self.return_code + output.return_code,
+            self.stdout + output.stdout,
+            self.stderr + output.stderr,
+        )
+
 
 class Morbin:
     def __init__(self, capture_output: bool = False, shell: bool = False):
         """Command bindings should return an `Output` object.
 
         If `capture_output` is `True` or the `capturing_output` context manager is used,
         the command's output will be available via `Output.stdout` and `Output.stderr`.
@@ -77,18 +85,18 @@
             output = subprocess.run(
                 command,
                 stdout=subprocess.PIPE,
                 stderr=subprocess.PIPE,
                 text=True,
                 shell=self.shell,
             )
-            return Output(output.returncode, output.stdout, output.stderr)
+            return Output([output.returncode], output.stdout, output.stderr)
         else:
             output = subprocess.run(command, shell=self.shell)
-            return Output(output.returncode)
+            return Output([output.returncode])
 
 
 def get_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser()
 
     parser.add_argument(
         "name",
```

### Comparing `morbin-0.0.0/LICENSE.txt` & `morbin-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `morbin-0.0.0/pyproject.toml` & `morbin-0.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "morbin"
 description = "Base class for creating modules that are bindings for command line tools."
-version = "0.0.0"
+version = "0.1.0"
 requires-python = ">=3.10"
-dependencies = ["pathier", "pytest"]
+dependencies = ["pathier", "pytest", "typing_extensions"]
 readme = "README.md"
 keywords = ["cli", "terminal", "binding", "bindings", "morbius", "morbin", "morph"]
 classifiers = ["Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent"]
 
 [[project.authors]]
 name = "Matt Manes"
 email = "mattmanes@pm.me"
```

### Comparing `morbin-0.0.0/PKG-INFO` & `morbin-0.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: morbin
-Version: 0.0.0
+Version: 0.1.0
 Summary: Base class for creating modules that are bindings for command line tools.
 Project-URL: Homepage, https://github.com/matt-manes/morbin
 Project-URL: Documentation, https://github.com/matt-manes/morbin/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/morbin/tree/main/src/morbin
 Author-email: Matt Manes <mattmanes@pm.me>
 License-File: LICENSE.txt
 Keywords: binding,bindings,cli,morbin,morbius,morph,terminal
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: pathier
 Requires-Dist: pytest
+Requires-Dist: typing-extensions
 Description-Content-Type: text/markdown
 
 # morbin
 
 Base class for creating modules that are bindings for command line tools.
 
 ## Installation
@@ -40,14 +41,35 @@
 ![](/imgs/template.png)
 Additional functions should be built on top of this `git` function and return its output.<br>
 
 After adding functions for `git add`, `git commit`, and `git log` the class should look like this:
 ![](/imgs/functions.png)
 
 The `Output` object each function returns is a `dataclass` with three fields: `return_code`, `stdout`, and `stderr`.<br>
-![](/imgs/output.png)
+<pre>
+@dataclass
+class Output:
+    """Dataclass representing the output of a terminal command.
+
+    #### Fields:
+    * `return_code: list[int]`
+    * `stdout: str`
+    * `stderr: str`"""
+
+    return_code: list[int]
+    stdout: str = ""
+    stderr: str = ""
+
+    def __add__(self, output: Self) -> Self:
+        return Output(
+            self.return_code + output.return_code,
+            self.stdout + output.stdout,
+            self.stderr + output.stderr,
+        )
+</pre>
+
 
 By default `stdout` and `stderr` are not captured.<br>
 They are sent to wherever they normally would be and the `stdout` and `stderr` fields of the `Output` object will be empty strings.<br>
 `stdout` and `stderr` can be captured by either setting the `capture_output` property of a class instance to `True` 
 or by using the `capturing_output` context manager as demonstrated below:
 ![](/imgs/use.png)
```

